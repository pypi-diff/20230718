# Comparing `tmp/twinthread-1.2.6.tar.gz` & `tmp/twinthread-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinthread-1.2.6.tar", max compression
+gzip compressed data, was "twinthread-1.2.7.tar", max compression
```

## Comparing `twinthread-1.2.6.tar` & `twinthread-1.2.7.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      496 2023-07-06 15:22:50.191881 twinthread-1.2.6/pyproject.toml
--rw-r--r--   0        0        0    12529 2023-07-06 15:22:50.192313 twinthread-1.2.6/twinthread/__init__.py
--rw-r--r--   0        0        0   353428 2023-07-06 15:21:20.531839 twinthread-1.2.6/twinthread/dataset
--rw-r--r--   0        0        0      660 2023-06-20 21:09:20.015296 twinthread-1.2.6/twinthread/exec_task.py
--rw-r--r--   0        0        0     3256 2023-07-06 14:42:59.491212 twinthread-1.2.6/twinthread/jupyter.py
--rw-r--r--   0        0        0      725 2023-07-06 14:42:59.491287 twinthread-1.2.6/twinthread/string_handling.py
--rw-r--r--   0        0        0      317 2023-07-06 15:16:26.171750 twinthread-1.2.6/twinthread/testing.py
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 twinthread-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0      498 2023-07-18 13:44:48.658757 twinthread-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0    12529 2023-07-18 13:44:48.659109 twinthread-1.2.7/twinthread/__init__.py
+-rw-r--r--   0        0        0   353428 2023-07-06 19:42:44.427954 twinthread-1.2.7/twinthread/dataset
+-rw-r--r--   0        0        0   353428 2023-07-06 19:23:32.239544 twinthread-1.2.7/twinthread/datasetx
+-rw-r--r--   0        0        0      660 2023-06-20 21:09:20.015296 twinthread-1.2.7/twinthread/exec_task.py
+-rw-r--r--   0        0        0     3256 2023-07-06 14:42:59.491212 twinthread-1.2.7/twinthread/jupyter.py
+-rw-r--r--   0        0        0   353428 2023-07-06 19:19:29.787532 twinthread-1.2.7/twinthread/something_else
+-rw-r--r--   0        0        0      725 2023-07-06 14:42:59.491287 twinthread-1.2.7/twinthread/string_handling.py
+-rw-r--r--   0        0        0      319 2023-07-06 19:42:15.326322 twinthread-1.2.7/twinthread/testing.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 twinthread-1.2.7/PKG-INFO
```

### Comparing `twinthread-1.2.6/twinthread/__init__.py` & `twinthread-1.2.7/twinthread/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from _plotly_utils.utils import PlotlyJSONEncoder
 
 from .jupyter import register_jupyter
 from .string_handling import task_string_to_context
 
 __author__ = """Brad Johnson"""
 __email__ = "brad.johnson@twinthread.com"
-__version__ = "1.2.6"
+__version__ = "1.2.7"
 
 import re
 import json
 import simplejson
 import requests
 import pandas as pd
 from io import StringIO
```

### Comparing `twinthread-1.2.6/twinthread/dataset` & `twinthread-1.2.7/twinthread/dataset`

 * *Files identical despite different names*

### Comparing `twinthread-1.2.6/twinthread/exec_task.py` & `twinthread-1.2.7/twinthread/exec_task.py`

 * *Files identical despite different names*

### Comparing `twinthread-1.2.6/twinthread/jupyter.py` & `twinthread-1.2.7/twinthread/jupyter.py`

 * *Files identical despite different names*

### Comparing `twinthread-1.2.6/twinthread/string_handling.py` & `twinthread-1.2.7/twinthread/string_handling.py`

 * *Files identical despite different names*

### Comparing `twinthread-1.2.6/PKG-INFO` & `twinthread-1.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: twinthread
-Version: 1.2.6
+Version: 1.2.7
 Summary: 
 Author: Brent Baumgartner
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-storage-blob (>=12.13.0,<13.0.0)
-Requires-Dist: ipython (==8.8.0)
+Requires-Dist: ipython (>=8.10.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: plotly (>=4.8.1,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests_toolbelt (>=0.10.0,<0.11.0)
 Requires-Dist: simplejson (>=3.17.0,<4.0.0)
 Requires-Dist: urllib3 (==1.26.15)
```

