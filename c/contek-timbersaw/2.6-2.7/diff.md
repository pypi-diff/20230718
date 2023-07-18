# Comparing `tmp/contek-timbersaw-2.6.tar.gz` & `tmp/contek-timbersaw-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contek-timbersaw-2.6.tar", last modified: Fri May 19 09:12:50 2023, max compression
+gzip compressed data, was "contek-timbersaw-2.7.tar", last modified: Tue Jul 18 07:24:15 2023, max compression
```

## Comparing `contek-timbersaw-2.6.tar` & `contek-timbersaw-2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 09:12:50.693042 contek-timbersaw-2.6/
--rw-rw-rw-   0        0        0     1082 2022-03-24 03:32:36.000000 contek-timbersaw-2.6/LICENSE.txt
--rw-rw-rw-   0        0        0     2154 2023-05-19 09:12:50.692040 contek-timbersaw-2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1650 2022-05-30 04:03:41.000000 contek-timbersaw-2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 09:12:50.685034 contek-timbersaw-2.6/contek_timbersaw/
--rw-rw-rw-   0        0        0     2348 2023-05-19 09:12:03.000000 contek-timbersaw-2.6/contek_timbersaw/__init__.py
--rw-rw-rw-   0        0        0     1916 2022-10-08 08:47:49.000000 contek-timbersaw-2.6/contek_timbersaw/async_compressor.py
--rw-rw-rw-   0        0        0     1195 2022-10-08 08:47:49.000000 contek-timbersaw-2.6/contek_timbersaw/deleter.py
--rw-rw-rw-   0        0        0     2517 2022-10-08 08:47:49.000000 contek-timbersaw-2.6/contek_timbersaw/timed_rolling_file_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:12:50.691039 contek-timbersaw-2.6/contek_timbersaw.egg-info/
--rw-rw-rw-   0        0        0     2154 2023-05-19 09:12:50.000000 contek-timbersaw-2.6/contek_timbersaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-05-19 09:12:50.000000 contek-timbersaw-2.6/contek_timbersaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 09:12:50.000000 contek-timbersaw-2.6/contek_timbersaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-19 09:12:50.000000 contek-timbersaw-2.6/contek_timbersaw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-19 09:12:28.000000 contek-timbersaw-2.6/contek_timbersaw.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-19 09:12:50.693042 contek-timbersaw-2.6/setup.cfg
--rw-rw-rw-   0        0        0      795 2023-05-19 09:11:52.000000 contek-timbersaw-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:24:15.790159 contek-timbersaw-2.7/
+-rw-rw-rw-   0        0        0     1082 2022-03-24 03:32:36.000000 contek-timbersaw-2.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     2155 2023-07-18 07:24:15.790159 contek-timbersaw-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1650 2022-05-30 04:03:41.000000 contek-timbersaw-2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 07:24:15.783153 contek-timbersaw-2.7/contek_timbersaw/
+-rw-rw-rw-   0        0        0     2412 2023-07-18 07:23:30.000000 contek-timbersaw-2.7/contek_timbersaw/__init__.py
+-rw-rw-rw-   0        0        0     1916 2022-10-08 08:47:49.000000 contek-timbersaw-2.7/contek_timbersaw/async_compressor.py
+-rw-rw-rw-   0        0        0     1195 2022-10-08 08:47:49.000000 contek-timbersaw-2.7/contek_timbersaw/deleter.py
+-rw-rw-rw-   0        0        0     2517 2022-10-08 08:47:49.000000 contek-timbersaw-2.7/contek_timbersaw/timed_rolling_file_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:24:15.789158 contek-timbersaw-2.7/contek_timbersaw.egg-info/
+-rw-rw-rw-   0        0        0     2155 2023-07-18 07:24:15.000000 contek-timbersaw-2.7/contek_timbersaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-07-18 07:24:15.000000 contek-timbersaw-2.7/contek_timbersaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 07:24:15.000000 contek-timbersaw-2.7/contek_timbersaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-18 07:24:15.000000 contek-timbersaw-2.7/contek_timbersaw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 07:24:15.000000 contek-timbersaw-2.7/contek_timbersaw.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-07-18 07:24:15.790159 contek-timbersaw-2.7/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-07-18 07:23:52.000000 contek-timbersaw-2.7/setup.py
```

### Comparing `contek-timbersaw-2.6/LICENSE.txt` & `contek-timbersaw-2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contek-timbersaw-2.6/PKG-INFO` & `contek-timbersaw-2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: contek-timbersaw
-Version: 2.6
+Version: 2.7
 Summary: Timbersaw for automatic logging configuration
 Home-page: https://github.com/contek-io/contek-timbersaw
 Author: contek_bjy
 Author-email: bjy@contek.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Timbersaw Logging Configurator
 
 ```timbersaw``` is a an automatic logging configurator.
```

### Comparing `contek-timbersaw-2.6/README.md` & `contek-timbersaw-2.7/README.md`

 * *Files identical despite different names*

### Comparing `contek-timbersaw-2.6/contek_timbersaw/__init__.py` & `contek-timbersaw-2.7/contek_timbersaw/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging.config
 import os
 import sys
 import time
+from typing import Optional
 
 from contek_timbersaw.timed_rolling_file_handler import TimedRollingFileHandler
 
 
 def setup():
     log_format = os.getenv(
         'log_format',
@@ -29,31 +30,31 @@
     stream_handler = logging.StreamHandler()
     stream_handler.setFormatter(formatter)
     stream_handler.setStream(sys.stdout)
     logger.addHandler(stream_handler)
     logger.setLevel(logging.INFO)
     logger.propagate = True
 
-    def add_file_handler(level, retention_days, compression_format=None):
-        file_dir = os.path.join(log_root, level.lower())
+    def add_file_handler(level: int, retention_days: int, compression_format: Optional[str] = None):
+        file_dir = os.path.join(log_root, logging.getLevelName(level).lower())
         os.makedirs(file_dir, exist_ok=True)
         handler = TimedRollingFileHandler(
             file_dir,
             compression_format=compression_format,
             retention=retention_days * 24 * 60 * 60,
             when=log_rolling,
             utc=log_utc,
         )
         handler.setFormatter(formatter)
-        handler.setLevel(logging.getLevelNamesMapping()[level])
+        handler.setLevel(level)
         logger.addHandler(handler)
 
-    add_file_handler('INFO', log_info_retention_days, 'gz')
-    add_file_handler('WARN', log_warn_retention_days)
-    add_file_handler('ERROR', log_error_retention_days)
+    add_file_handler(logging.INFO, log_info_retention_days, 'gz')
+    add_file_handler(logging.WARN, log_warn_retention_days)
+    add_file_handler(logging.ERROR, log_error_retention_days)
 
     def handle_exception(exc_type, exc_value, exc_traceback) -> None:
         if issubclass(exc_type, KeyboardInterrupt):
             sys.__excepthook__(exc_type, exc_value, exc_traceback)
             return
 
         logger.exception(
```

### Comparing `contek-timbersaw-2.6/contek_timbersaw/async_compressor.py` & `contek-timbersaw-2.7/contek_timbersaw/async_compressor.py`

 * *Files identical despite different names*

### Comparing `contek-timbersaw-2.6/contek_timbersaw/deleter.py` & `contek-timbersaw-2.7/contek_timbersaw/deleter.py`

 * *Files identical despite different names*

### Comparing `contek-timbersaw-2.6/contek_timbersaw/timed_rolling_file_handler.py` & `contek-timbersaw-2.7/contek_timbersaw/timed_rolling_file_handler.py`

 * *Files identical despite different names*

### Comparing `contek-timbersaw-2.6/contek_timbersaw.egg-info/PKG-INFO` & `contek-timbersaw-2.7/contek_timbersaw.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: contek-timbersaw
-Version: 2.6
+Version: 2.7
 Summary: Timbersaw for automatic logging configuration
 Home-page: https://github.com/contek-io/contek-timbersaw
 Author: contek_bjy
 Author-email: bjy@contek.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Timbersaw Logging Configurator
 
 ```timbersaw``` is a an automatic logging configurator.
```

### Comparing `contek-timbersaw-2.6/setup.py` & `contek-timbersaw-2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='contek-timbersaw',
-    version='2.6',
+    version='2.7',
     description='Timbersaw for automatic logging configuration',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.10',
     py_modules=["contek_timbersaw"],
     url='https://github.com/contek-io/contek-timbersaw',
     author='contek_bjy',
     author_email='bjy@contek.io',
     license='MIT',
     install_requires=[],
     zip_safe=True,
```

