# Comparing `tmp/garth-0.1.2.tar.gz` & `tmp/garth-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.1.2.tar", last modified: Sun Jul 16 23:03:12 2023, max compression
+gzip compressed data, was "garth-0.1.3.tar", last modified: Tue Jul 18 12:41:56 2023, max compression
```

## Comparing `garth-0.1.2.tar` & `garth-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.2/README.md
--rw-r--r--   0        0        0       55 2023-07-16 13:04:44.324498 garth-0.1.2/garth/__init__.py
--rw-r--r--   0        0        0      986 2023-07-16 18:57:12.229760 garth-0.1.2/garth/auth_token.py
--rw-r--r--   0        0        0     2219 2023-07-16 18:38:38.109518 garth-0.1.2/garth/http.py
--rw-r--r--   0        0        0     2716 2023-07-16 19:10:10.106829 garth-0.1.2/garth/sso.py
--rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.2/garth/version.py
--rw-r--r--   0        0        0      531 2023-07-16 23:03:12.697787 garth-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      282 1970-01-01 00:00:00.000000 garth-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.3/README.md
+-rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.3/garth/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.3/garth/auth_token.py
+-rw-r--r--   0        0        0     2669 2023-07-18 12:35:24.342092 garth-0.1.3/garth/http.py
+-rw-r--r--   0        0        0     2523 2023-07-18 12:39:28.223048 garth-0.1.3/garth/sso.py
+-rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.3/garth/version.py
+-rw-r--r--   0        0        0      531 2023-07-18 12:41:56.248396 garth-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      282 1970-01-01 00:00:00.000000 garth-0.1.3/PKG-INFO
```

### Comparing `garth-0.1.2/garth/auth_token.py` & `garth-0.1.3/garth/auth_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,16 @@
     refresh_token: str
     expires_in: int
     expires_at: int
     refresh_token_expires_in: int
     refresh_token_expires_at: int
 
     @classmethod
-    def login(cls, *args, **kwargs) -> tuple["AuthToken", str]:
-        token, username = sso.login(*args, **kwargs)
-        return cls(**token), username
+    def login(cls, *args, **kwargs) -> "AuthToken":
+        return cls(**sso.login(*args, **kwargs))
 
     def refresh(self, **kwargs):
         if self.refresh_expired:
             token = sso.exchange(**kwargs)
         else:
             token = self.__class__(**sso.refresh(self.refresh_token, **kwargs))
         self.__dict__.update(token.__dict__)
```

### Comparing `garth-0.1.2/garth/http.py` & `garth-0.1.3/garth/http.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from requests import Session
 
 from .auth_token import AuthToken
 
 
 USER_AGENT = {
     "User-Agent": (
@@ -36,14 +38,25 @@
         if username:
             self.username = username
         if cookies:
             self.sess.cookies.update(cookies)
         if domain:
             self.domain = domain
 
+    @property
+    def username(self) -> str:
+        if hasattr(self, "_username") and self._username:
+            return self._username
+        resp = self.get("connect", "/modern")
+        m = re.search(r'userName":"(.+?)"', resp.text)
+        if not m:
+            raise Exception("Couldn't find username")
+        self._username = m.group(1)
+        return self._username
+
     def request(
         self,
         method: str,
         subdomain: str,
         path: str,
         /,
         api: bool = False,
@@ -70,15 +83,17 @@
         return self.request("GET", *args, **kwargs)
 
     def post(self, *args, **kwargs):
         return self.request("POST", *args, **kwargs)
 
     def login(self, *args):
         if not self.auth_token:
-            token, username = AuthToken.login(*args, client=self)
+            token = AuthToken.login(*args, client=self)
             self.auth_token = token
-            self.username = username
         else:
             self.auth_token.refresh(client=self)
 
+    def connectapi(self, path: str, **kwargs):
+        return self.get("connect", path, api=True, **kwargs)
+
 
 client = Client()
```

### Comparing `garth-0.1.2/garth/sso.py` & `garth-0.1.3/garth/sso.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 
 from . import http
 
 
 def login(
     email: str, password: str, /, client: Optional["http.Client"] = None
-) -> tuple[dict, str]:
+) -> dict:
     client = client or http.client
 
     # Define params based on domain
     SSO = f"https://sso.{client.domain}/sso"
     SSO_EMBED = f"{SSO}/embed"
     SSO_EMBED_PARAMS = [
         ("id", "gauth-widget"),
@@ -57,25 +57,19 @@
 
     # Parse ticket
     m = re.search(r'embed\?ticket=([^"]+)"', resp.text)
     if not m:
         raise Exception("Could not find Service Ticket")
     ticket = m.group(1)
 
-    # Get username
-    resp = client.get("connect", "/modern", params=dict(ticket=ticket))
-    m = re.search(r'userName":"(.+?)"', resp.text)
-    if not m:
-        raise Exception("Could not find username")
-    username = m.group(1)
-
-    # Create oauth exchange token
+    # Exchange ticket for token
+    client.get("connect", "/modern", params=dict(ticket=ticket))
     token = exchange(client)
 
-    return token, username
+    return token
 
 
 def exchange(client: Optional["http.Client"] = None) -> dict:
     client = client or http.client
     token = client.post("connect", "/modern/di-oauth/exchange").json()
     return _set_expirations(token)
```

### Comparing `garth-0.1.2/pyproject.toml` & `garth-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "garth"
-version = "0.1.2"
+version = "0.1.3"
 description = "Garmin SSO auth"
 authors = [
     { name = "Matin Tamizi", email = "mtamizi@duck.com" },
 ]
 dependencies = [
     "fire>=0.5.0",
     "requests>=2.27.0",
```

