# Comparing `tmp/garth-0.1.5.tar.gz` & `tmp/garth-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.1.5.tar", last modified: Tue Jul 18 12:50:59 2023, max compression
+gzip compressed data, was "garth-0.1.6.tar", last modified: Tue Jul 18 14:02:55 2023, max compression
```

## Comparing `garth-0.1.5.tar` & `garth-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.5/README.md
--rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.5/garth/__init__.py
--rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.5/garth/auth_token.py
--rw-r--r--   0        0        0     2676 2023-07-18 12:47:12.835198 garth-0.1.5/garth/http.py
--rw-r--r--   0        0        0     2523 2023-07-18 12:39:28.223048 garth-0.1.5/garth/sso.py
--rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.5/garth/version.py
--rw-r--r--   0        0        0      512 2023-07-18 12:50:59.550039 garth-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 garth-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.6/README.md
+-rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.6/garth/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.6/garth/auth_token.py
+-rw-r--r--   0        0        0     2922 2023-07-18 13:33:15.604447 garth-0.1.6/garth/http.py
+-rw-r--r--   0        0        0     2535 2023-07-18 13:27:16.619857 garth-0.1.6/garth/sso.py
+-rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.6/garth/version.py
+-rw-r--r--   0        0        0      512 2023-07-18 14:02:55.534572 garth-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 garth-0.1.6/PKG-INFO
```

### Comparing `garth-0.1.5/garth/auth_token.py` & `garth-0.1.6/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.5/garth/http.py` & `garth-0.1.6/garth/http.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import re
 
 from requests import Session
 
 from .auth_token import AuthToken
 
 
@@ -56,20 +57,19 @@
     def request(
         self,
         method: str,
         subdomain: str,
         path: str,
         /,
         api: bool = False,
-        headers: dict | None = None,
+        headers: dict = {},
         **kwargs,
     ):
         url = f"https://{subdomain}.{self.domain}{path}"
         if api:
-            headers = headers or {}
             if self.auth_token and self.auth_token.expired:
                 self.auth_token.refresh(client=self)
             headers["Authorization"] = str(self.auth_token)
             headers["di-backend"] = f"connectapi.{self.domain}"
         resp = self.sess.request(
             method,
             url,
@@ -91,9 +91,18 @@
             self.auth_token = token
         else:
             self.auth_token.refresh(client=self)
 
     def connectapi(self, path: str, **kwargs):
         return self.get("connect", path, api=True, **kwargs).json()
 
+    def save_session(self, path: str):
+        with open(path, "w") as f:
+            json.dump(self.sess.cookies.get_dict(), f)
+
+    def resume_session(self, path: str):
+        with open(path) as f:
+            cookies = json.load(f)
+        self.sess.cookies.update(cookies)
+
 
 client = Client()
```

### Comparing `garth-0.1.5/garth/sso.py` & `garth-0.1.6/garth/sso.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     # Parse ticket
     m = re.search(r'embed\?ticket=([^"]+)"', resp.text)
     if not m:
         raise Exception("Could not find Service Ticket")
     ticket = m.group(1)
 
-    # Exchange ticket for token
+    # Exchange SSO Ticket for Connect Token
     client.get("connect", "/modern", params=dict(ticket=ticket))
     token = exchange(client)
 
     return token
 
 
 def exchange(client: Optional["http.Client"] = None) -> dict:
```

### Comparing `garth-0.1.5/pyproject.toml` & `garth-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "garth"
-version = "0.1.5"
+version = "0.1.6"
 description = "Garmin SSO auth"
 authors = [
     { name = "Matin Tamizi", email = "mtamizi@duck.com" },
 ]
 dependencies = [
     "requests>=2.27.0",
 ]
```

