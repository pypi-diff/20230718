# Comparing `tmp/steroid-0.0b0.tar.gz` & `tmp/steroid-0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steroid-0.0b0.tar", max compression
+gzip compressed data, was "steroid-0.1b0.tar", max compression
```

## Comparing `steroid-0.0b0.tar` & `steroid-0.1b0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1078 2023-07-18 18:42:23.446195 steroid-0.0b0/LICENSE
--rw-r--r--   0        0        0       69 2023-07-18 18:42:23.446195 steroid-0.0b0/README.md
--rw-r--r--   0        0        0      894 2023-07-18 18:42:38.650411 steroid-0.0b0/pyproject.toml
--rw-r--r--   0        0        0      808 2023-07-18 18:42:23.446195 steroid-0.0b0/steroid/app.py
--rw-r--r--   0        0        0     1925 2023-07-18 18:42:23.446195 steroid-0.0b0/steroid/common.py
--rw-r--r--   0        0        0      313 2023-07-18 18:42:23.446195 steroid-0.0b0/steroid/utils.py
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 steroid-0.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-18 18:45:38.812868 steroid-0.1b0/LICENSE
+-rw-r--r--   0        0        0       69 2023-07-18 18:45:38.812868 steroid-0.1b0/README.md
+-rw-r--r--   0        0        0      894 2023-07-18 18:45:56.120805 steroid-0.1b0/pyproject.toml
+-rw-r--r--   0        0        0      806 2023-07-18 18:45:38.812868 steroid-0.1b0/steroid/app.py
+-rw-r--r--   0        0        0     1924 2023-07-18 18:45:38.812868 steroid-0.1b0/steroid/common.py
+-rw-r--r--   0        0        0      313 2023-07-18 18:45:38.812868 steroid-0.1b0/steroid/utils.py
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 steroid-0.1b0/PKG-INFO
```

### Comparing `steroid-0.0b0/LICENSE` & `steroid-0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `steroid-0.0b0/pyproject.toml` & `steroid-0.1b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [project.urls]
 "Homepage" = "https://github.com/struckchure/steroid"
 "Bug Tracker" = "https://github.com/struckchure/steroid/issues"
 
 [tool.poetry]
 name = "steroid"
-version = "v0.0b"
+version = "v0.1b"
 authors = [
   "Mohammed Al Ameen <ameenmohammed2311@gmail.com>"
 ]
 description = "Steroid"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `steroid-0.0b0/steroid/app.py` & `steroid-0.1b0/steroid/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import uvicorn
 from fastapi import FastAPI
 
-from steroids.common import Controller
-from steroids.utils import removeLeadingOrTrailingSlash
+from steroid.common import Controller
+from steroid.utils import removeLeadingOrTrailingSlash
 
 app = FastAPI()
 
 
 class CreateApp:
     _APP: FastAPI = None
```

### Comparing `steroid-0.0b0/steroid/common.py` & `steroid-0.1b0/steroid/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from typing import Any
 
 from fastapi.routing import APIRouter
 
-from steroids.utils import formatPath
+from steroid.utils import formatPath
 
 
 class Controller:
     def __init__(self, path: str = "", *args, **kwargs):
         self.router = APIRouter()
 
         self.path = formatPath(path)
```

### Comparing `steroid-0.0b0/PKG-INFO` & `steroid-0.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steroid
-Version: 0.0b0
+Version: 0.1b0
 Summary: Steroid
 Author: Mohammed Al Ameen
 Author-email: ameenmohammed2311@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

