# Comparing `tmp/wow_ai_sdk-0.1.3.tar.gz` & `tmp/wow_ai_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_sdk-0.1.3.tar", max compression
+gzip compressed data, was "wow_ai_sdk-0.1.4.tar", max compression
```

## Comparing `wow_ai_sdk-0.1.3.tar` & `wow_ai_sdk-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7857 2023-06-30 11:57:05.323031 wow_ai_sdk-0.1.3/README.md
--rw-r--r--   0        0        0      262 2023-07-18 02:55:48.257797 wow_ai_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      149 2023-01-28 11:24:39.272410 wow_ai_sdk-0.1.3/wow_ai_sdk/__init__.py
--rw-r--r--   0        0        0     8869 2023-01-28 11:24:39.458541 wow_ai_sdk-0.1.3/wow_ai_sdk/client.py
--rw-r--r--   0        0        0     7914 2023-01-28 11:24:40.157550 wow_ai_sdk-0.1.3/wow_ai_sdk/data_manager.py
--rw-r--r--   0        0        0    66648 2023-07-15 09:22:29.068399 wow_ai_sdk-0.1.3/wow_ai_sdk/project.py
--rw-r--r--   0        0        0     1325 2023-01-28 11:24:40.436036 wow_ai_sdk-0.1.3/wow_ai_sdk/users.py
--rw-r--r--   0        0        0     4218 2023-01-28 11:24:40.801400 wow_ai_sdk-0.1.3/wow_ai_sdk/utils.py
--rw-r--r--   0        0        0     1889 2023-01-28 11:24:41.002364 wow_ai_sdk-0.1.3/wow_ai_sdk/workspaces.py
--rw-r--r--   0        0        0     8289 1970-01-01 00:00:00.000000 wow_ai_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7857 2023-06-30 11:57:05.323031 wow_ai_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0      262 2023-07-18 03:05:19.660262 wow_ai_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-01-28 11:24:39.272410 wow_ai_sdk-0.1.4/wow_ai_sdk/__init__.py
+-rw-r--r--   0        0        0     8908 2023-07-18 03:05:07.528378 wow_ai_sdk-0.1.4/wow_ai_sdk/client.py
+-rw-r--r--   0        0        0     7914 2023-01-28 11:24:40.157550 wow_ai_sdk-0.1.4/wow_ai_sdk/data_manager.py
+-rw-r--r--   0        0        0    66648 2023-07-15 09:22:29.068399 wow_ai_sdk-0.1.4/wow_ai_sdk/project.py
+-rw-r--r--   0        0        0     1325 2023-01-28 11:24:40.436036 wow_ai_sdk-0.1.4/wow_ai_sdk/users.py
+-rw-r--r--   0        0        0     4218 2023-01-28 11:24:40.801400 wow_ai_sdk-0.1.4/wow_ai_sdk/utils.py
+-rw-r--r--   0        0        0     1889 2023-01-28 11:24:41.002364 wow_ai_sdk-0.1.4/wow_ai_sdk/workspaces.py
+-rw-r--r--   0        0        0     8289 1970-01-01 00:00:00.000000 wow_ai_sdk-0.1.4/PKG-INFO
```

### Comparing `wow_ai_sdk-0.1.3/README.md` & `wow_ai_sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.3/wow_ai_sdk/client.py` & `wow_ai_sdk-0.1.4/wow_ai_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,17 @@
             Cookies that will be passed to each http request.
         """
         self.url = url.rstrip('/')
         self.session = session or self.get_session()
 
         # set api key or get it using credentials (username and password)
         if api_key is not None:
-            credentials = ClientCredentials(api_key=api_key)
-        self.api_key = credentials.api_key if credentials.api_key else self.get_api_key(credentials)
+            self.api_key = api_key
+            # credentials = ClientCredentials(api_key=api_key)
+        # self.api_key = credentials.api_key if credentials.api_key else self.get_api_key(credentials)
 
         # set headers
         self.headers = {'Authorization': f'Token {self.api_key}'}
         if extra_headers:
             self.headers.update(extra_headers)
 
         # Set cookies
```

### Comparing `wow_ai_sdk-0.1.3/wow_ai_sdk/data_manager.py` & `wow_ai_sdk-0.1.4/wow_ai_sdk/data_manager.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.3/wow_ai_sdk/project.py` & `wow_ai_sdk-0.1.4/wow_ai_sdk/project.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.3/wow_ai_sdk/users.py` & `wow_ai_sdk-0.1.4/wow_ai_sdk/users.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.3/wow_ai_sdk/utils.py` & `wow_ai_sdk-0.1.4/wow_ai_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.3/wow_ai_sdk/workspaces.py` & `wow_ai_sdk-0.1.4/wow_ai_sdk/workspaces.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.3/PKG-INFO` & `wow_ai_sdk-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ai-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.inc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

