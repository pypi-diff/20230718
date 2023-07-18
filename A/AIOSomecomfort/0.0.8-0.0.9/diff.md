# Comparing `tmp/AIOSomecomfort-0.0.8.tar.gz` & `tmp/AIOSomecomfort-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIOSomecomfort-0.0.8.tar", last modified: Wed Feb 15 18:27:22 2023, max compression
+gzip compressed data, was "AIOSomecomfort-0.0.9.tar", last modified: Sat Feb 25 14:32:46 2023, max compression
```

## Comparing `AIOSomecomfort-0.0.8.tar` & `AIOSomecomfort-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 18:27:22.851014 AIOSomecomfort-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-02-15 18:27:22.823014 AIOSomecomfort-0.0.8/AIOSomecomfort.egg-info/
--rw-rw-rw-   0        0        0     3781 2023-02-15 18:27:21.000000 AIOSomecomfort-0.0.8/AIOSomecomfort.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-02-15 18:27:22.000000 AIOSomecomfort-0.0.8/AIOSomecomfort.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 18:27:22.000000 AIOSomecomfort-0.0.8/AIOSomecomfort.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-02-15 18:27:22.000000 AIOSomecomfort-0.0.8/AIOSomecomfort.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-02-15 18:27:22.000000 AIOSomecomfort-0.0.8/AIOSomecomfort.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2023-01-11 14:41:52.000000 AIOSomecomfort-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       51 2023-01-16 12:38:00.000000 AIOSomecomfort-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3781 2023-02-15 18:27:22.848013 AIOSomecomfort-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3066 2023-01-16 12:50:15.000000 AIOSomecomfort-0.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-15 18:27:22.843011 AIOSomecomfort-0.0.8/aiosomecomfort/
--rw-rw-rw-   0        0        0     8631 2023-02-15 18:07:19.000000 AIOSomecomfort-0.0.8/aiosomecomfort/__init__.py
--rw-rw-rw-   0        0        0    10152 2023-02-15 13:06:57.000000 AIOSomecomfort-0.0.8/aiosomecomfort/device.py
--rw-rw-rw-   0        0        0      429 2023-01-19 13:11:11.000000 AIOSomecomfort-0.0.8/aiosomecomfort/exceptions.py
--rw-rw-rw-   0        0        0     1225 2023-02-15 12:47:46.000000 AIOSomecomfort-0.0.8/aiosomecomfort/location.py
--rw-rw-rw-   0        0        0       28 2023-01-16 12:05:05.000000 AIOSomecomfort-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-15 18:27:22.852026 AIOSomecomfort-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-02-15 18:25:29.000000 AIOSomecomfort-0.0.8/setup.py
--rw-rw-rw-   0        0        0       18 2023-01-11 14:41:53.000000 AIOSomecomfort-0.0.8/test_requirements.txt
+drwxrwxrwx   0        0        0        0 2023-02-25 14:32:46.057109 AIOSomecomfort-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-02-25 14:32:46.021588 AIOSomecomfort-0.0.9/AIOSomecomfort.egg-info/
+-rw-rw-rw-   0        0        0     3781 2023-02-25 14:32:44.000000 AIOSomecomfort-0.0.9/AIOSomecomfort.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-02-25 14:32:45.000000 AIOSomecomfort-0.0.9/AIOSomecomfort.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-25 14:32:44.000000 AIOSomecomfort-0.0.9/AIOSomecomfort.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-02-25 14:32:45.000000 AIOSomecomfort-0.0.9/AIOSomecomfort.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-02-25 14:32:45.000000 AIOSomecomfort-0.0.9/AIOSomecomfort.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2023-01-11 14:41:52.000000 AIOSomecomfort-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-01-16 12:38:00.000000 AIOSomecomfort-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3781 2023-02-25 14:32:46.055116 AIOSomecomfort-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3066 2023-01-16 12:50:15.000000 AIOSomecomfort-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-02-25 14:32:46.047114 AIOSomecomfort-0.0.9/aiosomecomfort/
+-rw-rw-rw-   0        0        0     8724 2023-02-25 14:27:22.000000 AIOSomecomfort-0.0.9/aiosomecomfort/__init__.py
+-rw-rw-rw-   0        0        0    10271 2023-02-25 14:07:30.000000 AIOSomecomfort-0.0.9/aiosomecomfort/device.py
+-rw-rw-rw-   0        0        0      429 2023-01-19 13:11:11.000000 AIOSomecomfort-0.0.9/aiosomecomfort/exceptions.py
+-rw-rw-rw-   0        0        0     1225 2023-02-15 12:47:46.000000 AIOSomecomfort-0.0.9/aiosomecomfort/location.py
+-rw-rw-rw-   0        0        0       28 2023-01-16 12:05:05.000000 AIOSomecomfort-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-02-25 14:32:46.059109 AIOSomecomfort-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-02-25 14:30:53.000000 AIOSomecomfort-0.0.9/setup.py
+-rw-rw-rw-   0        0        0       18 2023-01-11 14:41:53.000000 AIOSomecomfort-0.0.9/test_requirements.txt
```

### Comparing `AIOSomecomfort-0.0.8/AIOSomecomfort.egg-info/PKG-INFO` & `AIOSomecomfort-0.0.9/AIOSomecomfort.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AIOSomecomfort
-Version: 0.0.8
+Version: 0.0.9
 Summary: A client for Honeywell's US-based cloud devices
 Home-page: https://github.com/mkmer/AIOSomecomfort
-Download-URL: https://github.com/mkmer/AIOSomecomfort/archive/refs/tags/0.0.8.tar.gz
+Download-URL: https://github.com/mkmer/AIOSomecomfort/archive/refs/tags/0.0.9.tar.gz
 Author: Mike Kasper
 Author-email: m_kasper@sbcglobal.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIOSomecomfort-0.0.8/LICENSE` & `AIOSomecomfort-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AIOSomecomfort-0.0.8/PKG-INFO` & `AIOSomecomfort-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AIOSomecomfort
-Version: 0.0.8
+Version: 0.0.9
 Summary: A client for Honeywell's US-based cloud devices
 Home-page: https://github.com/mkmer/AIOSomecomfort
-Download-URL: https://github.com/mkmer/AIOSomecomfort/archive/refs/tags/0.0.8.tar.gz
+Download-URL: https://github.com/mkmer/AIOSomecomfort/archive/refs/tags/0.0.9.tar.gz
 Author: Mike Kasper
 Author-email: m_kasper@sbcglobal.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIOSomecomfort-0.0.8/README.rst` & `AIOSomecomfort-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `AIOSomecomfort-0.0.8/aiosomecomfort/__init__.py` & `AIOSomecomfort-0.0.9/aiosomecomfort/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             "UserName": self._username,
             "Password": self._password,
             "RememberMe": "false",
         }
         self._headers["Content-Type"] = "application/x-www-form-urlencoded"
         # can't use params because AIOHttp doesn't URL encode like API expects (%40 for @)
         url = URL(f"{url}?{urllib.urlencode(params)}", encoded=True)
+        self._session.cookie_jar.clear_domain(url)
         resp = await self._session.post(
             url, timeout=self._timeout, headers=self._headers
         )
 
         # The TUREHOME cookie is malformed in some way - need to clear the expiration to make it work with AIOhttp
         cookies = resp.cookies
         if AUTH_COOKIE in cookies:
@@ -88,15 +89,16 @@
         ) or resp2.status == 401:
             _LOG.error(
                 "Login as %s failed - null cookie or Unauthorized %s",
                 self._username,
                 resp2.status,
             )
             raise AuthError(
-                f"Login as {self._username} failed - null cookie or Unauthorized {resp2.status}"
+                "Login as %s failed - null cookie or Unauthorized %s"
+                % (self._username, resp2.status)
             )
 
         elif resp2.status != 200:
             _LOG.error("Connection error %s", resp2.status)
             raise ConnectionError("Connection error %s" % resp2.status)
 
     async def _request_json(self, method: str, *args, **kwargs):
@@ -116,16 +118,16 @@
 
         req = args[0].replace(self._baseurl, "")
 
         if resp.status == 200 and resp.content_type == "application/json":
             return await resp.json()
 
         elif resp.status == 401:
-            _LOG.error("API Rate Limited at login.")
-            raise APIRateLimited("API Rate Limited at login.")
+            _LOG.error("401 Error at update (Key expired?).")
+            raise APIRateLimited("401 Error at update (Key Expired?).")
 
         elif resp.status == 503:
             _LOG.error("Service Unavailable.")
             raise ConnectionError("Service Unavailable.")
 
         else:  # Some other non 200 status
             _LOG.error("API returned %s from %s request", resp.status, req)
```

### Comparing `AIOSomecomfort-0.0.8/aiosomecomfort/device.py` & `AIOSomecomfort-0.0.9/aiosomecomfort/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,19 @@
     def current_temperature(self):
         """The current measured ambient temperature"""
         return self._data["uiData"]["DispTemperature"]
 
     @property
     def current_humidity(self):
         """The current measured ambient humidity"""
-        return self._data["uiData"]["IndoorHumidity"]
+        return (
+            self._data["uiData"].get("IndoorHumidity")
+            if self._data["uiData"].get("IndoorHumidity") <= 100
+            else None
+        )
 
     @property
     def equipment_output_status(self):
         """The current equipment output status"""
         if self._data["uiData"]["EquipmentOutputStatus"] in (0, None):
             if self.fan_running:
                 return "fan"
```

### Comparing `AIOSomecomfort-0.0.8/aiosomecomfort/location.py` & `AIOSomecomfort-0.0.9/aiosomecomfort/location.py`

 * *Files identical despite different names*

### Comparing `AIOSomecomfort-0.0.8/setup.py` & `AIOSomecomfort-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 tests_require = list(val.strip() for val in open("test_requirements.txt"))
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="AIOSomecomfort",
-    version="0.0.8",
+    version="0.0.9",
     description="A client for Honeywell's US-based cloud devices",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/plain",
     author="Mike Kasper",
     author_email="m_kasper@sbcglobal.net",
     url="https://github.com/mkmer/AIOSomecomfort",
-    download_url="https://github.com/mkmer/AIOSomecomfort/archive/refs/tags/0.0.8.tar.gz",
+    download_url="https://github.com/mkmer/AIOSomecomfort/archive/refs/tags/0.0.9.tar.gz",
     packages=["aiosomecomfort"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

