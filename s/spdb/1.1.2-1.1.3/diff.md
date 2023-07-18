# Comparing `tmp/spdb-1.1.2.tar.gz` & `tmp/spdb-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdb-1.1.2.tar", last modified: Tue Jul 18 18:07:03 2023, max compression
+gzip compressed data, was "spdb-1.1.3.tar", last modified: Tue Jul 18 18:08:59 2023, max compression
```

## Comparing `spdb-1.1.2.tar` & `spdb-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-18 18:07:03.353579 spdb-1.1.2/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.1.2/LICENSE
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5469 2023-07-18 18:07:03.353579 spdb-1.1.2/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4986 2023-07-18 12:48:35.000000 spdb-1.1.2/README.md
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      468 2023-07-18 18:06:51.000000 spdb-1.1.2/pyproject.toml
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-18 18:07:03.353579 spdb-1.1.2/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-18 18:06:57.000000 spdb-1.1.2/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-18 18:07:03.350245 spdb-1.1.2/spdb/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      229 2023-07-18 12:50:28.000000 spdb-1.1.2/spdb/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2622 2023-07-18 18:06:48.000000 spdb-1.1.2/spdb/db.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.1.2/spdb/generator_utils.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.1.2/spdb/otp.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1366 2023-07-18 13:08:42.000000 spdb-1.1.2/spdb/quotes.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2223 2023-07-18 12:58:01.000000 spdb-1.1.2/spdb/restr.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      370 2023-07-18 13:07:31.000000 spdb-1.1.2/spdb/textvalidator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 17:51:56.000000 spdb-1.1.2/spdb/token_generator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.1.2/spdb/utils.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-18 18:07:03.350245 spdb-1.1.2/spdb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5469 2023-07-18 18:07:03.000000 spdb-1.1.2/spdb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      360 2023-07-18 18:07:03.000000 spdb-1.1.2/spdb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-18 18:07:03.000000 spdb-1.1.2/spdb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-18 11:02:48.000000 spdb-1.1.2/spdb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-18 18:07:03.000000 spdb-1.1.2/spdb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-18 18:07:03.000000 spdb-1.1.2/spdb.egg-info/top_level.txt
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-18 18:08:59.063941 spdb-1.1.3/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.1.3/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5469 2023-07-18 18:08:59.063941 spdb-1.1.3/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4986 2023-07-18 12:48:35.000000 spdb-1.1.3/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      468 2023-07-18 18:08:50.000000 spdb-1.1.3/pyproject.toml
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-18 18:08:59.063941 spdb-1.1.3/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-18 18:08:46.000000 spdb-1.1.3/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-18 18:08:59.063941 spdb-1.1.3/spdb/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      229 2023-07-18 12:50:28.000000 spdb-1.1.3/spdb/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2630 2023-07-18 18:08:40.000000 spdb-1.1.3/spdb/db.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.1.3/spdb/generator_utils.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.1.3/spdb/otp.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1366 2023-07-18 13:08:42.000000 spdb-1.1.3/spdb/quotes.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2223 2023-07-18 12:58:01.000000 spdb-1.1.3/spdb/restr.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      370 2023-07-18 13:07:31.000000 spdb-1.1.3/spdb/textvalidator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 17:51:56.000000 spdb-1.1.3/spdb/token_generator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.1.3/spdb/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-18 18:08:59.063941 spdb-1.1.3/spdb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5469 2023-07-18 18:08:58.000000 spdb-1.1.3/spdb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      360 2023-07-18 18:08:59.000000 spdb-1.1.3/spdb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-18 18:08:58.000000 spdb-1.1.3/spdb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-18 11:02:48.000000 spdb-1.1.3/spdb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-18 18:08:58.000000 spdb-1.1.3/spdb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-18 18:08:58.000000 spdb-1.1.3/spdb.egg-info/top_level.txt
```

### Comparing `spdb-1.1.2/LICENSE` & `spdb-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spdb-1.1.2/PKG-INFO` & `spdb-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spdb
-Version: 1.1.2
+Version: 1.1.3
 Summary: Sassy Python Database (and auth) utils
 Author-email: Mrybs <mrybs2@gmail.com>
 Project-URL: Homepage, https://github.com/mrybs/spdb
 Project-URL: Bug Tracker, https://github.com/mrybs/spdb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spdb-1.1.2/README.md` & `spdb-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `spdb-1.1.2/spdb/db.py` & `spdb-1.1.3/spdb/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,17 +60,17 @@
 
 
 	@staticmethod
 	def json_to_object(Class, JSON: dict):
 		try:
 			return Class.fromJSON(JSON)
 		except NameError:
-			return self.dict_to_object(Class, JSON)
+			return Database.dict_to_object(Class, JSON)
 		except KeyError:
-			return self.dict_to_object(Class, JSON)
+			return Database.dict_to_object(Class, JSON)
 
 
 	def read_json(self, name: str, data_id: str) -> dict:
 		objects = self.execute(f'select data from {name} where id = \'{data_id}\'')
 		if len(objects) == 0:
 			return {}
 		return json.loads(objects[0][0])
```

### Comparing `spdb-1.1.2/spdb/generator_utils.py` & `spdb-1.1.3/spdb/generator_utils.py`

 * *Files identical despite different names*

### Comparing `spdb-1.1.2/spdb/otp.py` & `spdb-1.1.3/spdb/otp.py`

 * *Files identical despite different names*

### Comparing `spdb-1.1.2/spdb/quotes.py` & `spdb-1.1.3/spdb/quotes.py`

 * *Files identical despite different names*

### Comparing `spdb-1.1.2/spdb/restr.py` & `spdb-1.1.3/spdb/restr.py`

 * *Files identical despite different names*

### Comparing `spdb-1.1.2/spdb/token_generator.py` & `spdb-1.1.3/spdb/token_generator.py`

 * *Files identical despite different names*

### Comparing `spdb-1.1.2/spdb.egg-info/PKG-INFO` & `spdb-1.1.3/spdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spdb
-Version: 1.1.2
+Version: 1.1.3
 Summary: Sassy Python Database (and auth) utils
 Author-email: Mrybs <mrybs2@gmail.com>
 Project-URL: Homepage, https://github.com/mrybs/spdb
 Project-URL: Bug Tracker, https://github.com/mrybs/spdb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

