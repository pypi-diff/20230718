# Comparing `tmp/exma-0.6.0.tar.gz` & `tmp/exma-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exma-0.6.0.tar", last modified: Fri Jun  2 15:49:31 2023, max compression
+gzip compressed data, was "exma-0.6.1.tar", last modified: Tue Jul 18 17:44:40 2023, max compression
```

## Comparing `exma-0.6.0.tar` & `exma-0.6.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:49:31.141818 exma-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-02 15:49:18.000000 exma-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-02 15:49:18.000000 exma-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-02 15:49:31.141818 exma-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-02 15:49:18.000000 exma-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:49:31.141818 exma-0.6.0/exma/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-02 15:49:18.000000 exma-0.6.0/exma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-06-02 15:49:18.000000 exma-0.6.0/exma/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-06-02 15:49:18.000000 exma-0.6.0/exma/cn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-06-02 15:49:18.000000 exma-0.6.0/exma/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-02 15:49:18.000000 exma-0.6.0/exma/distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-02 15:49:18.000000 exma-0.6.0/exma/electrochemistry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:49:31.141818 exma-0.6.0/exma/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-02 15:49:18.000000 exma-0.6.0/exma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-06-02 15:49:18.000000 exma-0.6.0/exma/io/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-06-02 15:49:18.000000 exma-0.6.0/exma/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-06-02 15:49:18.000000 exma-0.6.0/exma/io/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:49:31.141818 exma-0.6.0/exma/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/cn.c
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/cn.h
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/pbc_distances.c
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/pbc_distances.h
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/rdf.c
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/rdf.h
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-02 15:49:18.000000 exma-0.6.0/exma/msd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-02 15:49:18.000000 exma-0.6.0/exma/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-02 15:49:18.000000 exma-0.6.0/exma/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-02 15:49:18.000000 exma-0.6.0/exma/vacf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:49:31.141818 exma-0.6.0/exma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-02 15:49:31.000000 exma-0.6.0/exma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-02 15:49:31.000000 exma-0.6.0/exma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:49:31.000000 exma-0.6.0/exma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 15:49:31.000000 exma-0.6.0/exma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-02 15:49:31.000000 exma-0.6.0/exma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:49:31.141818 exma-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-02 15:49:18.000000 exma-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:44:40.865525 exma-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 17:44:27.000000 exma-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-18 17:44:27.000000 exma-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-18 17:44:40.865525 exma-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-18 17:44:27.000000 exma-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:44:40.865525 exma-0.6.1/exma/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-18 17:44:27.000000 exma-0.6.1/exma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-18 17:44:27.000000 exma-0.6.1/exma/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-18 17:44:27.000000 exma-0.6.1/exma/cn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-18 17:44:27.000000 exma-0.6.1/exma/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-18 17:44:27.000000 exma-0.6.1/exma/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-18 17:44:27.000000 exma-0.6.1/exma/electrochemistry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:44:40.865525 exma-0.6.1/exma/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-07-18 17:44:27.000000 exma-0.6.1/exma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-18 17:44:27.000000 exma-0.6.1/exma/io/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-07-18 17:44:27.000000 exma-0.6.1/exma/io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-07-18 17:44:27.000000 exma-0.6.1/exma/io/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:44:40.865525 exma-0.6.1/exma/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-18 17:44:27.000000 exma-0.6.1/exma/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-18 17:44:27.000000 exma-0.6.1/exma/lib/cn.c
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-18 17:44:27.000000 exma-0.6.1/exma/lib/cn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-18 17:44:27.000000 exma-0.6.1/exma/lib/pbc_distances.c
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-18 17:44:27.000000 exma-0.6.1/exma/lib/pbc_distances.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-18 17:44:27.000000 exma-0.6.1/exma/lib/rdf.c
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-18 17:44:27.000000 exma-0.6.1/exma/lib/rdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-18 17:44:27.000000 exma-0.6.1/exma/msd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-18 17:44:27.000000 exma-0.6.1/exma/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-18 17:44:27.000000 exma-0.6.1/exma/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-18 17:44:27.000000 exma-0.6.1/exma/vacf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:44:40.865525 exma-0.6.1/exma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-18 17:44:40.000000 exma-0.6.1/exma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-18 17:44:40.000000 exma-0.6.1/exma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:44:40.000000 exma-0.6.1/exma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-18 17:44:40.000000 exma-0.6.1/exma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 17:44:40.000000 exma-0.6.1/exma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:44:40.865525 exma-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-18 17:44:27.000000 exma-0.6.1/setup.py
```

### Comparing `exma-0.6.0/LICENSE` & `exma-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/PKG-INFO` & `exma-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: exma
-Version: 0.6.0
-Summary: extendable molecular dynamics analyzer
+Version: 0.6.1
+Summary: A Python library with C extensions to analyze and manipulate molecular dynamics trajectories and electrochemical data.
 Home-page: https://github.com/fernandezfran/exma
 Author: Francisco Fernandez
 Author-email: ffernandev@gmail.com
 License: MIT
 Keywords: exma,molecular-dynamics,data-analysis
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `exma-0.6.0/README.md` & `exma-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/__init__.py` & `exma-0.6.1/exma/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # ============================================================================
 # CONSTANTS
 # ============================================================================
 
 __author__ = """Francisco Fernandez"""
 __email__ = "ffernandev@gmail.com"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 
 # ============================================================================
 # IMPORTS
 # ============================================================================
 
 # core
```

### Comparing `exma-0.6.0/exma/cluster.py` & `exma-0.6.1/exma/cluster.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/cn.py` & `exma-0.6.1/exma/cn.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/core.py` & `exma-0.6.1/exma/core.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/distances.py` & `exma-0.6.1/exma/distances.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/electrochemistry.py` & `exma-0.6.1/exma/electrochemistry.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/io/__init__.py` & `exma-0.6.1/exma/io/__init__.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/io/positions.py` & `exma-0.6.1/exma/io/positions.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/io/reader.py` & `exma-0.6.1/exma/io/reader.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/io/writer.py` & `exma-0.6.1/exma/io/writer.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/lib/cn.c` & `exma-0.6.1/exma/lib/cn.c`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/lib/pbc_distances.c` & `exma-0.6.1/exma/lib/pbc_distances.c`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/lib/rdf.c` & `exma-0.6.1/exma/lib/rdf.c`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/msd.py` & `exma-0.6.1/exma/msd.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/rdf.py` & `exma-0.6.1/exma/rdf.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/statistics.py` & `exma-0.6.1/exma/statistics.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma/vacf.py` & `exma-0.6.1/exma/vacf.py`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/exma.egg-info/PKG-INFO` & `exma-0.6.1/exma.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: exma
-Version: 0.6.0
-Summary: extendable molecular dynamics analyzer
+Version: 0.6.1
+Summary: A Python library with C extensions to analyze and manipulate molecular dynamics trajectories and electrochemical data.
 Home-page: https://github.com/fernandezfran/exma
 Author: Francisco Fernandez
 Author-email: ffernandev@gmail.com
 License: MIT
 Keywords: exma,molecular-dynamics,data-analysis
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `exma-0.6.0/exma.egg-info/SOURCES.txt` & `exma-0.6.1/exma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exma-0.6.0/setup.py` & `exma-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,23 +57,28 @@
         if line.startswith("__version__ = "):
             VERSION = line.split("=", 1)[-1].replace('"', "").strip()
             break
 
 with open("README.md") as file_readme:
     LONG_DESCRIPTION = file_readme.read()
 
+SHORT_DESCRIPTION = (
+    "A Python library with C extensions to analyze and manipulate molecular "
+    "dynamics trajectories and electrochemical data."
+)
+
 
 # =============================================================================
 # FUNCTIONS
 # =============================================================================
 
 setup(
     name="exma",
     version=VERSION,
-    description="extendable molecular dynamics analyzer",
+    description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     author="Francisco Fernandez",
     author_email="ffernandev@gmail.com",
     url="https://github.com/fernandezfran/exma",
     license="MIT",
```

