# Comparing `tmp/pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0.tar.gz` & `tmp/pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0.tar", last modified: Tue Jul 18 04:57:39 2023, max compression
+gzip compressed data, was "pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1.tar", last modified: Tue Jul 18 05:00:05 2023, max compression
```

## Comparing `pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0.tar` & `pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 04:57:39.577505 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/
--rw-rw-rw-   0        0        0     1961 2023-07-18 04:57:39.577505 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-07-18 04:57:10.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-18 04:57:39.561879 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic/__init__.py
--rw-rw-rw-   0        0        0      344 2023-06-23 04:05:13.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic/check.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic/main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 04:57:39.577505 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0     1961 2023-07-18 04:57:39.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-18 04:57:39.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 04:57:39.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-07-18 04:57:39.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-18 04:57:39.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 04:57:39.577505 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/setup.cfg
--rw-rw-rw-   0        0        0     2014 2023-07-18 04:56:58.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:00:05.770536 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/
+-rw-rw-rw-   0        0        0     2165 2023-07-18 05:00:05.770536 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-07-18 04:57:10.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-18 05:00:05.754905 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic/__init__.py
+-rw-rw-rw-   0        0        0      344 2023-06-23 04:05:13.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic/check.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic/main.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:00:05.770536 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0     2165 2023-07-18 05:00:05.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-18 05:00:05.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 05:00:05.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-07-18 05:00:05.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-18 05:00:05.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 05:00:05.770536 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/setup.cfg
+-rw-rw-rw-   0        0        0     2214 2023-07-18 04:59:51.000000 pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/setup.py
```

### Comparing `pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/PKG-INFO` & `pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf_docx_pic
-Version: 4.1.0.1.0.3.2023.7.18.0
+Version: 4.1.0.1.0.3.2023.7.18.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
@@ -15,14 +15,18 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
```

### Comparing `pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic/main.py` & `pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic/main.py`

 * *Files identical despite different names*

### Comparing `pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/pdf_docx_pic.egg-info/PKG-INFO` & `pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/pdf_docx_pic.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 4.1.0.1.0.3.2023.7.18.0
+Version: 4.1.0.1.0.3.2023.7.18.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
@@ -15,14 +15,18 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
```

### Comparing `pdf_docx_pic-4.1.0.1.0.3.2023.7.18.0/setup.py` & `pdf_docx_pic-4.1.0.1.0.3.2023.7.18.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 c.check()
 
 a = open(".\\README.rst", mode='r', encoding = 'UTF-8').read()
 
 setup(
     name = "pdf_docx_pic",
-    version = "4.1.0.1.0.3.2023.7.18.0",
+    version = "4.1.0.1.0.3.2023.7.18.1",
     packages = find_packages(),
     python_requires = ">=2.6, <=3.12",
     classifiers = [
         "Development Status :: 4 - Beta",
         "Development Status :: 5 - Production/Stable",
         "Framework :: Jupyter :: JupyterLab :: 4",
         "Framework :: Django :: 4",
@@ -25,14 +25,18 @@
         "Operating System :: Microsoft :: Windows :: Windows 8.1",
         "Operating System :: Microsoft :: Windows :: Windows 10",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Operating System :: POSIX",
         "Natural Language :: Chinese (Simplified)",
         "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
```

