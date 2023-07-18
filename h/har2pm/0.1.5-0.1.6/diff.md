# Comparing `tmp/har2pm-0.1.5.tar.gz` & `tmp/har2pm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2pm-0.1.5.tar", max compression
+gzip compressed data, was "har2pm-0.1.6.tar", max compression
```

## Comparing `har2pm-0.1.5.tar` & `har2pm-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       50 2023-07-14 10:20:04.533135 har2pm-0.1.5/har2pm/__init__.py
--rw-r--r--   0        0        0     1106 2023-07-17 03:34:06.940299 har2pm-0.1.5/har2pm/cli.py
--rw-r--r--   0        0        0     3680 2023-07-17 09:57:27.197777 har2pm-0.1.5/har2pm/common.py
--rw-r--r--   0        0        0     1851 2023-07-17 03:34:06.940299 har2pm-0.1.5/har2pm/har2postman.py
--rw-r--r--   0        0        0     1083 2023-07-14 10:20:04.532132 har2pm-0.1.5/LICENSE
--rw-r--r--   0        0        0      689 2023-07-17 09:57:43.827275 har2pm-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      604 2023-07-14 10:20:04.532132 har2pm-0.1.5/README.md
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 har2pm-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-07-14 10:20:04.533135 har2pm-0.1.6/har2pm/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-17 03:34:06.940299 har2pm-0.1.6/har2pm/cli.py
+-rw-r--r--   0        0        0     3699 2023-07-18 03:14:00.937089 har2pm-0.1.6/har2pm/common.py
+-rw-r--r--   0        0        0     1851 2023-07-17 03:34:06.940299 har2pm-0.1.6/har2pm/har2postman.py
+-rw-r--r--   0        0        0     1083 2023-07-14 10:20:04.532132 har2pm-0.1.6/LICENSE
+-rw-r--r--   0        0        0      689 2023-07-18 03:10:43.309890 har2pm-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-07-14 10:20:04.532132 har2pm-0.1.6/README.md
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 har2pm-0.1.6/PKG-INFO
```

### Comparing `har2pm-0.1.5/har2pm/cli.py` & `har2pm-0.1.6/har2pm/cli.py`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.5/har2pm/common.py` & `har2pm-0.1.6/har2pm/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         ]
         :return: [
             {"key": "123", "value": "321"},
             ...
         ]
         """
 
-    black_list = ['content-length']
+    black_list = ['content-length', 'accept-encoding']
 
     har_headers = list(filter(lambda x: x not in black_list, har_headers))
 
     def extract(header):
         header['key'] = header.pop('name')
         return header
```

### Comparing `har2pm-0.1.5/har2pm/har2postman.py` & `har2pm-0.1.6/har2pm/har2postman.py`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.5/LICENSE` & `har2pm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.5/pyproject.toml` & `har2pm-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "har2pm"
-version = "0.1.5"
+version = "0.1.6"
 description = "Convert HAR(HTTP Archive) to Postman Collection"
 authors = ["ysansan"]
 license = "MIT"
 homepage = "https://github.com/whitexie/Har2Postman"
 repository = "https://github.com/whitexie/Har2Postman"
 keywords = ["har", "postman"]
 readme = "README.md"
```

### Comparing `har2pm-0.1.5/README.md` & `har2pm-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.5/PKG-INFO` & `har2pm-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2pm
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convert HAR(HTTP Archive) to Postman Collection
 Home-page: https://github.com/whitexie/Har2Postman
 License: MIT
 Keywords: har,postman
 Author: ysansan
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

