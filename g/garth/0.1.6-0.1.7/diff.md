# Comparing `tmp/garth-0.1.6.tar.gz` & `tmp/garth-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.1.6.tar", last modified: Tue Jul 18 14:02:55 2023, max compression
+gzip compressed data, was "garth-0.1.7.tar", last modified: Tue Jul 18 15:02:52 2023, max compression
```

## Comparing `garth-0.1.6.tar` & `garth-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.6/README.md
--rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.6/garth/__init__.py
--rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.6/garth/auth_token.py
--rw-r--r--   0        0        0     2922 2023-07-18 13:33:15.604447 garth-0.1.6/garth/http.py
--rw-r--r--   0        0        0     2535 2023-07-18 13:27:16.619857 garth-0.1.6/garth/sso.py
--rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.6/garth/version.py
--rw-r--r--   0        0        0      512 2023-07-18 14:02:55.534572 garth-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 garth-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.7/README.md
+-rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.7/garth/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.7/garth/auth_token.py
+-rw-r--r--   0        0        0     2930 2023-07-18 14:39:54.464611 garth-0.1.7/garth/http.py
+-rw-r--r--   0        0        0     2780 2023-07-18 15:01:10.701790 garth-0.1.7/garth/sso.py
+-rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.7/garth/version.py
+-rw-r--r--   0        0        0      512 2023-07-18 15:02:52.033505 garth-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 garth-0.1.7/PKG-INFO
```

### Comparing `garth-0.1.6/garth/auth_token.py` & `garth-0.1.7/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.6/garth/http.py` & `garth-0.1.7/garth/http.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import re
 
+from requests.cookies import RequestsCookieJar
 from requests import Session
 
 from .auth_token import AuthToken
 
 
 USER_AGENT = {
     "User-Agent": (
@@ -27,23 +28,20 @@
         self.configure(**kwargs)
 
     def configure(
         self,
         /,
         auth_token: AuthToken | None = None,
         username: str | None = None,
-        cookies: dict | None = None,
         domain: str | None = None,  # Set to "garmin.cn" for China
     ):
         if auth_token:
             self.auth_token = auth_token
         if username:
             self.username = username
-        if cookies:
-            self.sess.cookies.update(cookies)
         if domain:
             self.domain = domain
 
     @property
     def username(self) -> str:
         if hasattr(self, "_username") and self._username:
             return self._username
@@ -83,14 +81,15 @@
         return self.request("GET", *args, **kwargs)
 
     def post(self, *args, **kwargs):
         return self.request("POST", *args, **kwargs)
 
     def login(self, *args):
         if not self.auth_token:
+            self.cookies = RequestsCookieJar()  # Clear cookies
             token = AuthToken.login(*args, client=self)
             self.auth_token = token
         else:
             self.auth_token.refresh(client=self)
 
     def connectapi(self, path: str, **kwargs):
         return self.get("connect", path, api=True, **kwargs).json()
```

### Comparing `garth-0.1.6/garth/sso.py` & `garth-0.1.7/garth/sso.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,23 @@
         ("source", SSO_EMBED),
         ("redirectAfterAccountLoginUrl", SSO_EMBED),
         ("redirectAfterAccountCreationUrl", SSO_EMBED),
         ("gauthHost", SSO_EMBED),
     ]
 
     # Set cookies
-    client.get("sso", "/sso/embed", params=SSO_EMBED_PARAMS)
+    resp = client.get("sso", "/sso/embed", params=SSO_EMBED_PARAMS)
 
     # Get CSRF token
-    resp = client.get("sso", "/sso/signin", params=SIGNIN_PARAMS)
+    resp = client.get(
+        "sso",
+        "/sso/signin",
+        params=SIGNIN_PARAMS,
+        headers=dict(referer=resp.url),
+    )
     m = re.search(r'name="_csrf" value="(.+?)"', resp.text)
     if not m:
         raise Exception("Could not find CSRF token")
     csrf_token = m.group(1)
 
     # Sign in
     data = dict(
@@ -45,36 +50,45 @@
         _csrf=csrf_token,
     )
     resp = client.post(
         "sso",
         "/sso/signin",
         params=SIGNIN_PARAMS,
         data=data,
-        headers=dict(Referer=resp.url),
+        headers=dict(referer=resp.url),
     )
     m = re.search(r"<title>(.+?)</title>", resp.text)
     if not (m and m.group(1) == "Success"):
         raise Exception("Login failed")
 
     # Parse ticket
     m = re.search(r'embed\?ticket=([^"]+)"', resp.text)
     if not m:
         raise Exception("Could not find Service Ticket")
     ticket = m.group(1)
 
     # Exchange SSO Ticket for Connect Token
-    client.get("connect", "/modern", params=dict(ticket=ticket))
+    client.get(
+        "connect",
+        "/modern",
+        params=dict(ticket=ticket),
+        headers=dict(referer=resp.url),
+    )
     token = exchange(client)
 
     return token
 
 
 def exchange(client: Optional["http.Client"] = None) -> dict:
     client = client or http.client
-    token = client.post("connect", "/modern/di-oauth/exchange").json()
+    token = client.post(
+        "connect",
+        "/modern/di-oauth/exchange",
+        headers=dict(referer=f"https://connect.{client.domain}/modern"),
+    ).json()
     return _set_expirations(token)
 
 
 def refresh(
     refresh_token: str, /, client: Optional["http.Client"] = None
 ) -> dict:
     client = client or http.client
```

### Comparing `garth-0.1.6/pyproject.toml` & `garth-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "garth"
-version = "0.1.6"
+version = "0.1.7"
 description = "Garmin SSO auth"
 authors = [
     { name = "Matin Tamizi", email = "mtamizi@duck.com" },
 ]
 dependencies = [
     "requests>=2.27.0",
 ]
```

