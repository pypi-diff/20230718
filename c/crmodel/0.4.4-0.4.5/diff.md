# Comparing `tmp/crmodel-0.4.4.tar.gz` & `tmp/crmodel-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crmodel-0.4.4.tar", last modified: Thu Jul 13 08:56:40 2023, max compression
+gzip compressed data, was "crmodel-0.4.5.tar", last modified: Tue Jul 18 10:20:00 2023, max compression
```

## Comparing `crmodel-0.4.4.tar` & `crmodel-0.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-07-13 08:56:40.629834 crmodel-0.4.4/
--rw-r--r--   0 jeremy     (501) staff       (20)    35147 2023-07-13 08:43:59.000000 crmodel-0.4.4/LICENSE
--rw-r--r--   0 jeremy     (501) staff       (20)       63 2023-07-13 08:43:59.000000 crmodel-0.4.4/MANIFEST.in
--rw-r--r--   0 jeremy     (501) staff       (20)     1725 2023-07-13 08:56:40.629666 crmodel-0.4.4/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)     1120 2023-07-13 08:43:59.000000 crmodel-0.4.4/README.md
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-07-13 08:56:40.628653 crmodel-0.4.4/crmodel/
--rw-r--r--   0 jeremy     (501) staff       (20)     1071 2023-07-13 08:43:59.000000 crmodel-0.4.4/crmodel/config.py
--rw-r--r--   0 jeremy     (501) staff       (20)    18474 2023-07-13 08:43:59.000000 crmodel-0.4.4/crmodel/crmodel.py
--rw-r--r--   0 jeremy     (501) staff       (20)     7941 2023-07-13 08:43:59.000000 crmodel-0.4.4/crmodel/model.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1769 2023-07-13 08:43:59.000000 crmodel-0.4.4/crmodel/segmentationReader.py
--rw-r--r--   0 jeremy     (501) staff       (20)     8394 2023-07-13 08:43:59.000000 crmodel-0.4.4/crmodel/utils.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-07-13 08:56:40.629459 crmodel-0.4.4/crmodel.egg-info/
--rw-r--r--   0 jeremy     (501) staff       (20)     1725 2023-07-13 08:56:40.000000 crmodel-0.4.4/crmodel.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)      310 2023-07-13 08:56:40.000000 crmodel-0.4.4/crmodel.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-07-13 08:56:40.000000 crmodel-0.4.4/crmodel.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (501) staff       (20)      121 2023-07-13 08:56:40.000000 crmodel-0.4.4/crmodel.egg-info/requires.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        8 2023-07-13 08:56:40.000000 crmodel-0.4.4/crmodel.egg-info/top_level.txt
--rw-r--r--   0 jeremy     (501) staff       (20)      121 2023-07-13 08:51:50.000000 crmodel-0.4.4/requirements.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-07-13 08:56:40.629883 crmodel-0.4.4/setup.cfg
--rw-r--r--   0 jeremy     (501) staff       (20)     1092 2023-07-13 08:52:04.000000 crmodel-0.4.4/setup.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-07-18 10:20:00.229256 crmodel-0.4.5/
+-rw-r--r--   0 jeremy     (501) staff       (20)    35147 2023-07-13 08:43:59.000000 crmodel-0.4.5/LICENSE
+-rw-r--r--   0 jeremy     (501) staff       (20)       63 2023-07-13 08:43:59.000000 crmodel-0.4.5/MANIFEST.in
+-rw-r--r--   0 jeremy     (501) staff       (20)     1725 2023-07-18 10:20:00.229104 crmodel-0.4.5/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)     1120 2023-07-13 08:43:59.000000 crmodel-0.4.5/README.md
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-07-18 10:20:00.227924 crmodel-0.4.5/crmodel/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1071 2023-07-13 08:43:59.000000 crmodel-0.4.5/crmodel/config.py
+-rw-r--r--   0 jeremy     (501) staff       (20)    18474 2023-07-13 08:43:59.000000 crmodel-0.4.5/crmodel/crmodel.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     7941 2023-07-13 09:11:30.000000 crmodel-0.4.5/crmodel/model.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1769 2023-07-13 08:43:59.000000 crmodel-0.4.5/crmodel/segmentationReader.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     8394 2023-07-13 08:43:59.000000 crmodel-0.4.5/crmodel/utils.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-07-18 10:20:00.228844 crmodel-0.4.5/crmodel.egg-info/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1725 2023-07-18 10:20:00.000000 crmodel-0.4.5/crmodel.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)      310 2023-07-18 10:20:00.000000 crmodel-0.4.5/crmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-07-18 10:20:00.000000 crmodel-0.4.5/crmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)      121 2023-07-18 10:20:00.000000 crmodel-0.4.5/crmodel.egg-info/requires.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        8 2023-07-18 10:20:00.000000 crmodel-0.4.5/crmodel.egg-info/top_level.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)      121 2023-07-18 10:18:28.000000 crmodel-0.4.5/requirements.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-07-18 10:20:00.229298 crmodel-0.4.5/setup.cfg
+-rw-r--r--   0 jeremy     (501) staff       (20)     1092 2023-07-18 10:19:33.000000 crmodel-0.4.5/setup.py
```

### Comparing `crmodel-0.4.4/LICENSE` & `crmodel-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.4/PKG-INFO` & `crmodel-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crmodel
-Version: 0.4.4
+Version: 0.4.5
 Summary: crmodel is a python package that produces the crossroadsdesriber model from OpenStreetMap. See doi.org/10.5194/agile-giss-3-40-2022 for further informations.
 Home-page: https://github.com/jeremyk6/crmodel
 Author: Jérémy Kalsron
 Author-email: jeremy.kalsron@gmail.com  
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crmodel-0.4.4/README.md` & `crmodel-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.4/crmodel/config.py` & `crmodel-0.4.5/crmodel/config.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.4/crmodel/crmodel.py` & `crmodel-0.4.5/crmodel/crmodel.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.4/crmodel/model.py` & `crmodel-0.4.5/crmodel/model.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.4/crmodel/segmentationReader.py` & `crmodel-0.4.5/crmodel/segmentationReader.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.4/crmodel/utils.py` & `crmodel-0.4.5/crmodel/utils.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.4/crmodel.egg-info/PKG-INFO` & `crmodel-0.4.5/crmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crmodel
-Version: 0.4.4
+Version: 0.4.5
 Summary: crmodel is a python package that produces the crossroadsdesriber model from OpenStreetMap. See doi.org/10.5194/agile-giss-3-40-2022 for further informations.
 Home-page: https://github.com/jeremyk6/crmodel
 Author: Jérémy Kalsron
 Author-email: jeremy.kalsron@gmail.com  
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crmodel-0.4.4/setup.py` & `crmodel-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # The requirements file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="crmodel",
-    version="0.4.4",
+    version="0.4.5",
     description="crmodel is a python package that produces the crossroadsdesriber model from OpenStreetMap. See doi.org/10.5194/agile-giss-3-40-2022 for further informations.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jeremyk6/crmodel",
     author="Jérémy Kalsron",
     author_email="jeremy.kalsron@gmail.com  ",
     license="AGPL-3.0",
```

