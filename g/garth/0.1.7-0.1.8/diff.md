# Comparing `tmp/garth-0.1.7.tar.gz` & `tmp/garth-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.1.7.tar", last modified: Tue Jul 18 15:02:52 2023, max compression
+gzip compressed data, was "garth-0.1.8.tar", last modified: Tue Jul 18 18:28:02 2023, max compression
```

## Comparing `garth-0.1.7.tar` & `garth-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.7/README.md
--rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.7/garth/__init__.py
--rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.7/garth/auth_token.py
--rw-r--r--   0        0        0     2930 2023-07-18 14:39:54.464611 garth-0.1.7/garth/http.py
--rw-r--r--   0        0        0     2780 2023-07-18 15:01:10.701790 garth-0.1.7/garth/sso.py
--rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.7/garth/version.py
--rw-r--r--   0        0        0      512 2023-07-18 15:02:52.033505 garth-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 garth-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.8/README.md
+-rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.8/garth/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.8/garth/auth_token.py
+-rw-r--r--   0        0        0     2930 2023-07-18 14:39:54.464611 garth-0.1.8/garth/http.py
+-rw-r--r--   0        0        0     3605 2023-07-18 18:25:44.073499 garth-0.1.8/garth/sso.py
+-rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.8/garth/version.py
+-rw-r--r--   0        0        0      512 2023-07-18 18:28:02.766786 garth-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 garth-0.1.8/PKG-INFO
```

### Comparing `garth-0.1.7/garth/auth_token.py` & `garth-0.1.8/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.7/garth/http.py` & `garth-0.1.8/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.7/garth/sso.py` & `garth-0.1.8/garth/sso.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import re
 import time
 from typing import Optional
 
 from . import http
 
 
+CSRF_RE = re.compile(r'name="_csrf"\s+value="(.+?)"')
+TITLE_RE = re.compile(r"<title>(.+?)</title>")
+
+
 def login(
     email: str, password: str, /, client: Optional["http.Client"] = None
 ) -> dict:
     client = client or http.client
 
     # Define params based on domain
     SSO = f"https://sso.{client.domain}/sso"
@@ -33,35 +37,49 @@
     # Get CSRF token
     resp = client.get(
         "sso",
         "/sso/signin",
         params=SIGNIN_PARAMS,
         headers=dict(referer=resp.url),
     )
-    m = re.search(r'name="_csrf" value="(.+?)"', resp.text)
-    if not m:
-        raise Exception("Could not find CSRF token")
-    csrf_token = m.group(1)
+    csrf_token = _get_csrf_token(resp.text)
 
-    # Sign in
-    data = dict(
-        username=email,
-        password=password,
-        embed="true",
-        _csrf=csrf_token,
-    )
+    # Submit login form with email and password
     resp = client.post(
         "sso",
         "/sso/signin",
         params=SIGNIN_PARAMS,
-        data=data,
         headers=dict(referer=resp.url),
+        data=dict(
+            username=email,
+            password=password,
+            embed="true",
+            _csrf=csrf_token,
+        ),
     )
-    m = re.search(r"<title>(.+?)</title>", resp.text)
-    if not (m and m.group(1) == "Success"):
+    title = _get_title(resp.text)
+
+    # Handle MFA
+    if "MFA" in title:
+        csrf_token = _get_csrf_token(resp.text)
+        mfa_code = input("Enter MFA code: ")
+        resp = client.post(
+            "sso",
+            "/sso/verifyMFA/loginEnterMfaCode",
+            params=SIGNIN_PARAMS,
+            headers=dict(referer=resp.url),
+            data={
+                "mfa-code": mfa_code,
+                "embed": "true",
+                "_csrf": csrf_token,
+                "fromPage": "setupEnterMfaCode",
+            },
+        )
+
+    if _get_title(resp.text) != "Success":
         raise Exception("Login failed")
 
     # Parse ticket
     m = re.search(r'embed\?ticket=([^"]+)"', resp.text)
     if not m:
         raise Exception("Could not find Service Ticket")
     ticket = m.group(1)
@@ -103,7 +121,21 @@
 
 def _set_expirations(token: dict) -> dict:
     token["expires_at"] = int(time.time() + token["expires_in"])
     token["refresh_token_expires_at"] = int(
         time.time() + token["refresh_token_expires_in"]
     )
     return token
+
+
+def _get_csrf_token(html: str) -> str:
+    m = CSRF_RE.search(html)
+    if not m:
+        raise Exception("Couldn't find CSRF token")
+    return m.group(1)
+
+
+def _get_title(html: str) -> str:
+    m = TITLE_RE.search(html)
+    if not m:
+        raise Exception("Couldn't find title")
+    return m.group(1)
```

### Comparing `garth-0.1.7/pyproject.toml` & `garth-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "garth"
-version = "0.1.7"
+version = "0.1.8"
 description = "Garmin SSO auth"
 authors = [
     { name = "Matin Tamizi", email = "mtamizi@duck.com" },
 ]
 dependencies = [
     "requests>=2.27.0",
 ]
```

