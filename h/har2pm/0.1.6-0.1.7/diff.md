# Comparing `tmp/har2pm-0.1.6.tar.gz` & `tmp/har2pm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2pm-0.1.6.tar", max compression
+gzip compressed data, was "har2pm-0.1.7.tar", max compression
```

## Comparing `har2pm-0.1.6.tar` & `har2pm-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       50 2023-07-14 10:20:04.533135 har2pm-0.1.6/har2pm/__init__.py
--rw-r--r--   0        0        0     1106 2023-07-17 03:34:06.940299 har2pm-0.1.6/har2pm/cli.py
--rw-r--r--   0        0        0     3699 2023-07-18 03:14:00.937089 har2pm-0.1.6/har2pm/common.py
--rw-r--r--   0        0        0     1851 2023-07-17 03:34:06.940299 har2pm-0.1.6/har2pm/har2postman.py
--rw-r--r--   0        0        0     1083 2023-07-14 10:20:04.532132 har2pm-0.1.6/LICENSE
--rw-r--r--   0        0        0      689 2023-07-18 03:10:43.309890 har2pm-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      604 2023-07-14 10:20:04.532132 har2pm-0.1.6/README.md
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 har2pm-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-07-14 10:20:04.533135 har2pm-0.1.7/har2pm/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-17 03:34:06.940299 har2pm-0.1.7/har2pm/cli.py
+-rw-r--r--   0        0        0     3723 2023-07-18 03:33:17.277795 har2pm-0.1.7/har2pm/common.py
+-rw-r--r--   0        0        0     1851 2023-07-17 03:34:06.940299 har2pm-0.1.7/har2pm/har2postman.py
+-rw-r--r--   0        0        0     1083 2023-07-14 10:20:04.532132 har2pm-0.1.7/LICENSE
+-rw-r--r--   0        0        0      689 2023-07-18 03:33:43.534800 har2pm-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-07-14 10:20:04.532132 har2pm-0.1.7/README.md
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 har2pm-0.1.7/PKG-INFO
```

### Comparing `har2pm-0.1.6/har2pm/cli.py` & `har2pm-0.1.7/har2pm/cli.py`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.6/har2pm/common.py` & `har2pm-0.1.7/har2pm/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             {"key": "123", "value": "321"},
             ...
         ]
         """
 
     black_list = ['content-length', 'accept-encoding']
 
-    har_headers = list(filter(lambda x: x not in black_list, har_headers))
+    har_headers = list(filter(lambda x: x.get('name', '').lower() not in black_list, har_headers))
 
     def extract(header):
         header['key'] = header.pop('name')
         return header
 
     return list(map(extract, har_headers))
```

### Comparing `har2pm-0.1.6/har2pm/har2postman.py` & `har2pm-0.1.7/har2pm/har2postman.py`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.6/LICENSE` & `har2pm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.6/pyproject.toml` & `har2pm-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "har2pm"
-version = "0.1.6"
+version = "0.1.7"
 description = "Convert HAR(HTTP Archive) to Postman Collection"
 authors = ["ysansan"]
 license = "MIT"
 homepage = "https://github.com/whitexie/Har2Postman"
 repository = "https://github.com/whitexie/Har2Postman"
 keywords = ["har", "postman"]
 readme = "README.md"
```

### Comparing `har2pm-0.1.6/README.md` & `har2pm-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.6/PKG-INFO` & `har2pm-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2pm
-Version: 0.1.6
+Version: 0.1.7
 Summary: Convert HAR(HTTP Archive) to Postman Collection
 Home-page: https://github.com/whitexie/Har2Postman
 License: MIT
 Keywords: har,postman
 Author: ysansan
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

