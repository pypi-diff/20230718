# Comparing `tmp/qfitswidget-0.9.5.tar.gz` & `tmp/qfitswidget-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfitswidget-0.9.5.tar", max compression
+gzip compressed data, was "qfitswidget-0.9.6.tar", max compression
```

## Comparing `qfitswidget-0.9.5.tar` & `qfitswidget-0.9.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/LICENSE
--rw-r--r--   0        0        0      591 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/pyproject.toml
--rw-r--r--   0        0        0       37 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/__init__.py
--rw-r--r--   0        0        0     2262 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/navigationtoolbar.py
--rw-r--r--   0        0        0     1549 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/norm.py
--rw-r--r--   0        0        0    24258 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/qfitswidget.py
--rw-r--r--   0        0        0        0 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/qt/__init__.py
--rw-r--r--   0        0        0     6960 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/qt/fitswidget.py
--rw-r--r--   0        0        0     8226 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/qt/fitswidget.ui
--rw-r--r--   0        0        0      765 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/qt/resources/image-solid.svg
--rw-r--r--   0        0        0     4689 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/qt/resources.py
--rw-r--r--   0        0        0       95 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/qt/resources.rc
--rw-r--r--   0        0        0     8268 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/qt/settings.py
--rw-r--r--   0        0        0     5685 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/qt/settings.ui
--rw-r--r--   0        0        0     3934 2023-07-18 10:53:15.698881 qfitswidget-0.9.5/qfitswidget/settings.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 qfitswidget-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/LICENSE
+-rw-r--r--   0        0        0      591 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/__init__.py
+-rw-r--r--   0        0        0     2262 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/navigationtoolbar.py
+-rw-r--r--   0        0        0     1549 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/norm.py
+-rw-r--r--   0        0        0    24258 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/qfitswidget.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/qt/__init__.py
+-rw-r--r--   0        0        0     6960 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/qt/fitswidget.py
+-rw-r--r--   0        0        0     8226 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/qt/fitswidget.ui
+-rw-r--r--   0        0        0      765 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/qt/resources/image-solid.svg
+-rw-r--r--   0        0        0     4689 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/qt/resources.py
+-rw-r--r--   0        0        0       95 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/qt/resources.rc
+-rw-r--r--   0        0        0     8268 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/qt/settings.py
+-rw-r--r--   0        0        0     5685 2023-07-18 10:53:58.097087 qfitswidget-0.9.6/qfitswidget/qt/settings.ui
+-rw-r--r--   0        0        0     3934 2023-07-18 10:53:58.101087 qfitswidget-0.9.6/qfitswidget/settings.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 qfitswidget-0.9.6/PKG-INFO
```

### Comparing `qfitswidget-0.9.5/LICENSE` & `qfitswidget-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/pyproject.toml` & `qfitswidget-0.9.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "qfitswidget"
 packages = [{ include = "qfitswidget" }]
-version = "0.9.5"
+version = "0.9.6"
 description = "PyQt widget for displaying FITS files"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 matplotlib = "^3.7.1"
```

### Comparing `qfitswidget-0.9.5/qfitswidget/navigationtoolbar.py` & `qfitswidget-0.9.6/qfitswidget/navigationtoolbar.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/qfitswidget/norm.py` & `qfitswidget-0.9.6/qfitswidget/norm.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/qfitswidget/qfitswidget.py` & `qfitswidget-0.9.6/qfitswidget/qfitswidget.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/qfitswidget/qt/fitswidget.py` & `qfitswidget-0.9.6/qfitswidget/qt/fitswidget.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/qfitswidget/qt/fitswidget.ui` & `qfitswidget-0.9.6/qfitswidget/qt/fitswidget.ui`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/qfitswidget/qt/resources/image-solid.svg` & `qfitswidget-0.9.6/qfitswidget/qt/resources/image-solid.svg`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/qfitswidget/qt/resources.py` & `qfitswidget-0.9.6/qfitswidget/qt/resources.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/qfitswidget/qt/settings.py` & `qfitswidget-0.9.6/qfitswidget/qt/settings.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/qfitswidget/qt/settings.ui` & `qfitswidget-0.9.6/qfitswidget/qt/settings.ui`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/qfitswidget/settings.py` & `qfitswidget-0.9.6/qfitswidget/settings.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.5/PKG-INFO` & `qfitswidget-0.9.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfitswidget
-Version: 0.9.5
+Version: 0.9.6
 Summary: PyQt widget for displaying FITS files
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

