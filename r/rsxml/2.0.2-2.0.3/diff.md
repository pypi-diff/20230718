# Comparing `tmp/rsxml-2.0.2.tar.gz` & `tmp/rsxml-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsxml-2.0.2.tar", last modified: Mon Jul 10 19:32:25 2023, max compression
+gzip compressed data, was "rsxml-2.0.3.tar", last modified: Tue Jul 18 20:02:54 2023, max compression
```

## Comparing `rsxml-2.0.2.tar` & `rsxml-2.0.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.555820 rsxml-2.0.2/
--rw-r--r--   0 matt       (501) staff       (20)     1072 2023-07-05 23:12:54.000000 rsxml-2.0.2/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     7076 2023-07-10 19:32:25.555911 rsxml-2.0.2/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     6578 2023-07-05 23:39:56.000000 rsxml-2.0.2/README.md
--rw-r--r--   0 matt       (501) staff       (20)      864 2023-07-05 23:36:34.000000 rsxml-2.0.2/pyproject.toml
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.547584 rsxml-2.0.2/rsxml/
--rw-r--r--   0 matt       (501) staff       (20)      385 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)       22 2023-07-10 19:31:56.000000 rsxml-2.0.2/rsxml/__version__.py
--rw-r--r--   0 matt       (501) staff       (20)    13856 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/api.py
--rw-r--r--   0 matt       (501) staff       (20)      151 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/constants.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.550208 rsxml-2.0.2/rsxml/debug/
--rw-r--r--   0 matt       (501) staff       (20)      102 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/debug/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     8354 2023-07-07 15:26:31.000000 rsxml-2.0.2/rsxml/debug/debug_proc.py
--rw-r--r--   0 matt       (501) staff       (20)     3120 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/debug/loop_timer.py
--rw-r--r--   0 matt       (501) staff       (20)     1906 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/debug/timer.py
--rw-r--r--   0 matt       (501) staff       (20)     8508 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/debug/timer_buckets.py
--rw-r--r--   0 matt       (501) staff       (20)     3081 2023-07-06 15:41:36.000000 rsxml-2.0.2/rsxml/dotenv.py
--rw-r--r--   0 matt       (501) staff       (20)     1741 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/etag.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.550791 rsxml-2.0.2/rsxml/logging/
--rw-r--r--   0 matt       (501) staff       (20)        0 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/logging/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     9170 2023-07-07 16:12:54.000000 rsxml-2.0.2/rsxml/logging/logger.py
--rw-r--r--   0 matt       (501) staff       (20)     3716 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/logging/progress_bar.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.553953 rsxml-2.0.2/rsxml/project_xml/
--rw-r--r--   0 matt       (501) staff       (20)     3871 2023-07-10 16:15:20.000000 rsxml-2.0.2/rsxml/project_xml/Analysis.py
--rw-r--r--   0 matt       (501) staff       (20)     9317 2023-07-10 19:19:25.000000 rsxml-2.0.2/rsxml/project_xml/Dataset.py
--rw-r--r--   0 matt       (501) staff       (20)     9370 2023-07-10 19:18:19.000000 rsxml-2.0.2/rsxml/project_xml/Geopackage.py
--rw-r--r--   0 matt       (501) staff       (20)     6502 2023-07-10 15:33:03.000000 rsxml-2.0.2/rsxml/project_xml/MetaData.py
--rw-r--r--   0 matt       (501) staff       (20)    10537 2023-07-10 18:51:44.000000 rsxml-2.0.2/rsxml/project_xml/Project.py
--rw-r--r--   0 matt       (501) staff       (20)     3712 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/project_xml/ProjectBounds.py
--rw-r--r--   0 matt       (501) staff       (20)     3462 2023-07-07 18:42:13.000000 rsxml-2.0.2/rsxml/project_xml/ProjectValidation.py
--rw-r--r--   0 matt       (501) staff       (20)     3852 2023-07-10 15:40:00.000000 rsxml-2.0.2/rsxml/project_xml/QAQCEvent.py
--rw-r--r--   0 matt       (501) staff       (20)     6170 2023-07-10 15:36:29.000000 rsxml-2.0.2/rsxml/project_xml/RSObj.py
--rw-r--r--   0 matt       (501) staff       (20)     7317 2023-07-10 19:14:21.000000 rsxml-2.0.2/rsxml/project_xml/Realization.py
--rw-r--r--   0 matt       (501) staff       (20)     1174 2023-07-10 18:52:07.000000 rsxml-2.0.2/rsxml/project_xml/Warehouse.py
--rw-r--r--   0 matt       (501) staff       (20)      320 2023-07-10 18:40:08.000000 rsxml-2.0.2/rsxml/project_xml/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)      421 2023-07-10 16:10:03.000000 rsxml-2.0.2/rsxml/project_xml/common.py
--rw-r--r--   0 matt       (501) staff       (20)     1329 2023-07-07 19:16:00.000000 rsxml-2.0.2/rsxml/rspaths.py
--rw-r--r--   0 matt       (501) staff       (20)     7339 2023-07-06 15:22:35.000000 rsxml-2.0.2/rsxml/util.py
--rw-r--r--   0 matt       (501) staff       (20)     2059 2023-07-07 18:19:48.000000 rsxml-2.0.2/rsxml/validation.py
--rw-r--r--   0 matt       (501) staff       (20)      371 2023-07-05 23:12:54.000000 rsxml-2.0.2/rsxml/xml.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.548956 rsxml-2.0.2/rsxml.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     7076 2023-07-10 19:32:25.000000 rsxml-2.0.2/rsxml.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     1152 2023-07-10 19:32:25.000000 rsxml-2.0.2/rsxml.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-07-10 19:32:25.000000 rsxml-2.0.2/rsxml.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 16:11:44.000000 rsxml-2.0.2/rsxml.egg-info/not-zip-safe
--rw-r--r--   0 matt       (501) staff       (20)       59 2023-07-10 19:32:25.000000 rsxml-2.0.2/rsxml.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)        6 2023-07-10 19:32:25.000000 rsxml-2.0.2/rsxml.egg-info/top_level.txt
--rw-r--r--   0 matt       (501) staff       (20)       79 2023-07-10 19:32:25.556175 rsxml-2.0.2/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)     1257 2023-07-06 15:45:55.000000 rsxml-2.0.2/setup.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-10 19:32:25.555568 rsxml-2.0.2/tests/
--rw-r--r--   0 matt       (501) staff       (20)     2302 2023-07-05 23:12:54.000000 rsxml-2.0.2/tests/test_dotenv.py
--rw-r--r--   0 matt       (501) staff       (20)     1131 2023-07-05 23:12:54.000000 rsxml-2.0.2/tests/test_etags.py
--rw-r--r--   0 matt       (501) staff       (20)     1837 2023-07-10 16:11:30.000000 rsxml-2.0.2/tests/test_load_samples.py
--rw-r--r--   0 matt       (501) staff       (20)     2952 2023-07-07 19:18:01.000000 rsxml-2.0.2/tests/test_paths.py
--rw-r--r--   0 matt       (501) staff       (20)    15389 2023-07-07 22:57:09.000000 rsxml-2.0.2/tests/test_project_xml.py
--rw-r--r--   0 matt       (501) staff       (20)     7503 2023-07-05 23:12:54.000000 rsxml-2.0.2/tests/test_timers.py
--rw-r--r--   0 matt       (501) staff       (20)     3204 2023-07-05 23:27:33.000000 rsxml-2.0.2/tests/test_util.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-18 20:02:54.139132 rsxml-2.0.3/
+-rw-r--r--   0 matt       (501) staff       (20)     1072 2023-07-13 21:28:07.000000 rsxml-2.0.3/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     7076 2023-07-18 20:02:54.139266 rsxml-2.0.3/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     6578 2023-07-13 21:28:07.000000 rsxml-2.0.3/README.md
+-rw-r--r--   0 matt       (501) staff       (20)      864 2023-07-13 21:28:07.000000 rsxml-2.0.3/pyproject.toml
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-18 20:02:54.124769 rsxml-2.0.3/rsxml/
+-rw-r--r--   0 matt       (501) staff       (20)      385 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)       22 2023-07-18 20:02:05.000000 rsxml-2.0.3/rsxml/__version__.py
+-rw-r--r--   0 matt       (501) staff       (20)    13856 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/api.py
+-rw-r--r--   0 matt       (501) staff       (20)      151 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/constants.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-18 20:02:54.131997 rsxml-2.0.3/rsxml/debug/
+-rw-r--r--   0 matt       (501) staff       (20)      102 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/debug/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     8354 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/debug/debug_proc.py
+-rw-r--r--   0 matt       (501) staff       (20)     3120 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/debug/loop_timer.py
+-rw-r--r--   0 matt       (501) staff       (20)     1906 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/debug/timer.py
+-rw-r--r--   0 matt       (501) staff       (20)     8508 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/debug/timer_buckets.py
+-rw-r--r--   0 matt       (501) staff       (20)     3081 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/dotenv.py
+-rw-r--r--   0 matt       (501) staff       (20)     1741 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/etag.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-18 20:02:54.133021 rsxml-2.0.3/rsxml/logging/
+-rw-r--r--   0 matt       (501) staff       (20)        0 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/logging/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     9582 2023-07-18 20:01:52.000000 rsxml-2.0.3/rsxml/logging/logger.py
+-rw-r--r--   0 matt       (501) staff       (20)     3716 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/logging/progress_bar.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-18 20:02:54.137322 rsxml-2.0.3/rsxml/project_xml/
+-rw-r--r--   0 matt       (501) staff       (20)     3871 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/Analysis.py
+-rw-r--r--   0 matt       (501) staff       (20)     9317 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/Dataset.py
+-rw-r--r--   0 matt       (501) staff       (20)     9370 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/Geopackage.py
+-rw-r--r--   0 matt       (501) staff       (20)     6502 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/MetaData.py
+-rw-r--r--   0 matt       (501) staff       (20)    10537 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/Project.py
+-rw-r--r--   0 matt       (501) staff       (20)     3712 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/project_xml/ProjectBounds.py
+-rw-r--r--   0 matt       (501) staff       (20)     3462 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/ProjectValidation.py
+-rw-r--r--   0 matt       (501) staff       (20)     3852 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/QAQCEvent.py
+-rw-r--r--   0 matt       (501) staff       (20)     6170 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/RSObj.py
+-rw-r--r--   0 matt       (501) staff       (20)     7317 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/Realization.py
+-rw-r--r--   0 matt       (501) staff       (20)     1174 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/Warehouse.py
+-rw-r--r--   0 matt       (501) staff       (20)      320 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)      421 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/project_xml/common.py
+-rw-r--r--   0 matt       (501) staff       (20)     1329 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/rspaths.py
+-rw-r--r--   0 matt       (501) staff       (20)     7339 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/util.py
+-rw-r--r--   0 matt       (501) staff       (20)     2059 2023-07-18 19:53:38.000000 rsxml-2.0.3/rsxml/validation.py
+-rw-r--r--   0 matt       (501) staff       (20)      371 2023-07-13 21:28:07.000000 rsxml-2.0.3/rsxml/xml.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-18 20:02:54.129654 rsxml-2.0.3/rsxml.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)     7076 2023-07-18 20:02:54.000000 rsxml-2.0.3/rsxml.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     1152 2023-07-18 20:02:54.000000 rsxml-2.0.3/rsxml.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-07-18 20:02:54.000000 rsxml-2.0.3/rsxml.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 16:11:44.000000 rsxml-2.0.3/rsxml.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (501) staff       (20)       59 2023-07-18 20:02:54.000000 rsxml-2.0.3/rsxml.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)        6 2023-07-18 20:02:54.000000 rsxml-2.0.3/rsxml.egg-info/top_level.txt
+-rw-r--r--   0 matt       (501) staff       (20)       79 2023-07-18 20:02:54.139562 rsxml-2.0.3/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)     1257 2023-07-13 21:28:07.000000 rsxml-2.0.3/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-18 20:02:54.138899 rsxml-2.0.3/tests/
+-rw-r--r--   0 matt       (501) staff       (20)     2302 2023-07-13 21:28:07.000000 rsxml-2.0.3/tests/test_dotenv.py
+-rw-r--r--   0 matt       (501) staff       (20)     1131 2023-07-13 21:28:07.000000 rsxml-2.0.3/tests/test_etags.py
+-rw-r--r--   0 matt       (501) staff       (20)     1837 2023-07-18 19:53:38.000000 rsxml-2.0.3/tests/test_load_samples.py
+-rw-r--r--   0 matt       (501) staff       (20)     2952 2023-07-18 19:53:38.000000 rsxml-2.0.3/tests/test_paths.py
+-rw-r--r--   0 matt       (501) staff       (20)    15389 2023-07-18 19:53:38.000000 rsxml-2.0.3/tests/test_project_xml.py
+-rw-r--r--   0 matt       (501) staff       (20)     7503 2023-07-13 21:28:07.000000 rsxml-2.0.3/tests/test_timers.py
+-rw-r--r--   0 matt       (501) staff       (20)     3204 2023-07-13 21:28:07.000000 rsxml-2.0.3/tests/test_util.py
```

### Comparing `rsxml-2.0.2/LICENSE` & `rsxml-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/PKG-INFO` & `rsxml-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsxml
-Version: 2.0.2
+Version: 2.0.3
 Summary: Riverscapes XML helpers for use across Python3 open-source GIS Stack
 Home-page: https://github.com/Riverscapes/RiverscapesXML
 Author: Matt Reimer
 Author-email: info@northarrowresearch.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rsxml-2.0.2/README.md` & `rsxml-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/pyproject.toml` & `rsxml-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/api.py` & `rsxml-2.0.3/rsxml/api.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/debug/debug_proc.py` & `rsxml-2.0.3/rsxml/debug/debug_proc.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/debug/loop_timer.py` & `rsxml-2.0.3/rsxml/debug/loop_timer.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/debug/timer.py` & `rsxml-2.0.3/rsxml/debug/timer.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/debug/timer_buckets.py` & `rsxml-2.0.3/rsxml/debug/timer_buckets.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/dotenv.py` & `rsxml-2.0.3/rsxml/dotenv.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/etag.py` & `rsxml-2.0.3/rsxml/etag.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/logging/logger.py` & `rsxml-2.0.3/rsxml/logging/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,27 @@
         def __init__(self):
             self.initialized = False
             self.verbose = False
             self.logpath = None
             self.handler = None
             self.logger = logging.getLogger("LOGGER")
             logging.addLevelName(25, 'TITLE')
-            self.loglevels = logging.getLevelNamesMapping()
+            # self.loglevels = logging.getLevelNamesMapping() # THIS IS PYTHON 3.11 only
+            # These are more or less constants so we can define them here
+            self.loglevels = {
+                'CRITICAL': 50,
+                'FATAL': 50,
+                'ERROR': 40,
+                'WARN': 30,
+                'WARNING': 30,
+                'INFO': 20,
+                'DEBUG': 10,
+                'NOTSET': 0,
+                'TITLE': 25,
+            }
 
         def setup(self, log_path=None, verbose=False, log_level: int = None):
             """_summary_
 
             Args:
                 logPath (_type_, optional): _description_. Defaults to None.
                 verbose (bool, optional): _description_. Defaults to False.
```

### Comparing `rsxml-2.0.2/rsxml/logging/progress_bar.py` & `rsxml-2.0.3/rsxml/logging/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/Analysis.py` & `rsxml-2.0.3/rsxml/project_xml/Analysis.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/Dataset.py` & `rsxml-2.0.3/rsxml/project_xml/Dataset.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/Geopackage.py` & `rsxml-2.0.3/rsxml/project_xml/Geopackage.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/MetaData.py` & `rsxml-2.0.3/rsxml/project_xml/MetaData.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/Project.py` & `rsxml-2.0.3/rsxml/project_xml/Project.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/ProjectBounds.py` & `rsxml-2.0.3/rsxml/project_xml/ProjectBounds.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/ProjectValidation.py` & `rsxml-2.0.3/rsxml/project_xml/ProjectValidation.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/QAQCEvent.py` & `rsxml-2.0.3/rsxml/project_xml/QAQCEvent.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/RSObj.py` & `rsxml-2.0.3/rsxml/project_xml/RSObj.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/Realization.py` & `rsxml-2.0.3/rsxml/project_xml/Realization.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/project_xml/Warehouse.py` & `rsxml-2.0.3/rsxml/project_xml/Warehouse.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/rspaths.py` & `rsxml-2.0.3/rsxml/rspaths.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/util.py` & `rsxml-2.0.3/rsxml/util.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml/validation.py` & `rsxml-2.0.3/rsxml/validation.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/rsxml.egg-info/PKG-INFO` & `rsxml-2.0.3/rsxml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsxml
-Version: 2.0.2
+Version: 2.0.3
 Summary: Riverscapes XML helpers for use across Python3 open-source GIS Stack
 Home-page: https://github.com/Riverscapes/RiverscapesXML
 Author: Matt Reimer
 Author-email: info@northarrowresearch.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rsxml-2.0.2/rsxml.egg-info/SOURCES.txt` & `rsxml-2.0.3/rsxml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/setup.py` & `rsxml-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/tests/test_dotenv.py` & `rsxml-2.0.3/tests/test_dotenv.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/tests/test_etags.py` & `rsxml-2.0.3/tests/test_etags.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/tests/test_load_samples.py` & `rsxml-2.0.3/tests/test_load_samples.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/tests/test_paths.py` & `rsxml-2.0.3/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/tests/test_project_xml.py` & `rsxml-2.0.3/tests/test_project_xml.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/tests/test_timers.py` & `rsxml-2.0.3/tests/test_timers.py`

 * *Files identical despite different names*

### Comparing `rsxml-2.0.2/tests/test_util.py` & `rsxml-2.0.3/tests/test_util.py`

 * *Files identical despite different names*

