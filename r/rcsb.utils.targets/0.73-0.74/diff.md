# Comparing `tmp/rcsb.utils.targets-0.73.tar.gz` & `tmp/rcsb.utils.targets-0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.targets-0.73.tar", last modified: Wed Jul  5 13:34:44 2023, max compression
+gzip compressed data, was "rcsb.utils.targets-0.74.tar", last modified: Tue Jul 18 14:28:39 2023, max compression
```

## Comparing `rcsb.utils.targets-0.73.tar` & `rcsb.utils.targets-0.74.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-05 13:34:44.867374 rcsb.utils.targets-0.73/
--rw-r--r--   0 vsts      (1001) docker     (122)     6139 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-07-05 13:34:44.867374 rcsb.utils.targets-0.73/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      953 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-05 13:34:44.859373 rcsb.utils.targets-0.73/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-05 13:34:44.863374 rcsb.utils.targets-0.73/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-05 13:34:44.867374 rcsb.utils.targets-0.73/rcsb/utils/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)     9534 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetOntologyProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/DrugBankTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9506 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/IMGTTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20796 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/IMGTTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9154 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/SAbDabTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/rcsb/utils/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-05 13:34:44.863374 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-07-05 13:34:44.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-07-05 13:34:44.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-05 13:34:44.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-05 13:21:55.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-07-05 13:34:44.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-07-05 13:34:44.000000 rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-07-05 13:34:44.867374 rcsb.utils.targets-0.73/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-07-05 13:20:56.000000 rcsb.utils.targets-0.73/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 14:28:39.793338 rcsb.utils.targets-0.74/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6192 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-07-18 14:28:39.793338 rcsb.utils.targets-0.74/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      953 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 14:28:39.789338 rcsb.utils.targets-0.74/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 14:28:39.789338 rcsb.utils.targets-0.74/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 14:28:39.793338 rcsb.utils.targets-0.74/rcsb/utils/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9534 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/CARDTargetAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/CARDTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/CARDTargetOntologyProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/CARDTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19280 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5382 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8956 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/ChEMBLTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/DrugBankTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9506 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/IMGTTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20796 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/IMGTTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/PharosTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/PharosTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9154 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/PharosTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/SAbDabTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/rcsb/utils/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-18 14:28:39.789338 rcsb.utils.targets-0.74/rcsb.utils.targets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-07-18 14:28:39.000000 rcsb.utils.targets-0.74/rcsb.utils.targets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-07-18 14:28:39.000000 rcsb.utils.targets-0.74/rcsb.utils.targets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-18 14:28:39.000000 rcsb.utils.targets-0.74/rcsb.utils.targets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-18 14:15:55.000000 rcsb.utils.targets-0.74/rcsb.utils.targets.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-07-18 14:28:39.000000 rcsb.utils.targets-0.74/rcsb.utils.targets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-07-18 14:28:39.000000 rcsb.utils.targets-0.74/rcsb.utils.targets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-07-18 14:28:39.793338 rcsb.utils.targets-0.74/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-07-18 14:14:41.000000 rcsb.utils.targets-0.74/setup.py
```

### Comparing `rcsb.utils.targets-0.73/HISTORY.txt` & `rcsb.utils.targets-0.74/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,8 +58,9 @@
   24-Mar-2023  - V0.66 In PharosTargetProvider(), download sql file to separate dir
   11-Apr-2023  - V0.67 Fix issue with CARD lineage tree building--handle cases with two parents at same depth; Add treeNodeList building and exporting
   27-Apr-2023  - V0.68 Update CARD treeNodeList building
    2-May-2023  - V0.69 Remove depth field from CARD lineage tree
    5-May-2023  - V0.70 Actually check cache files exist in PharosTargetProvider testCache()
   22-May-2023  - V0.71 Add retries to tox task for MMseqs2 download
   13-Jun-2023  - V0.72 Improve logging
-   3-Jul-2023  - V0.73 imgt.org no longer supports http
+   3-Jul-2023  - V0.73 imgt.org no longer supports http
+  18-Jul-2023  - V0.74 Update baseVersion for ChEMBL
```

### Comparing `rcsb.utils.targets-0.73/LICENSE` & `rcsb.utils.targets-0.74/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/PKG-INFO` & `rcsb.utils.targets-0.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.73
+Version: 0.74
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.73/README.md` & `rcsb.utils.targets-0.74/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetAnnotationProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/CARDTargetAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetFeatureProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/CARDTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetOntologyProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/CARDTargetOntologyProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/CARDTargetProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/CARDTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetActivityProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/ChEMBLTargetActivityProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
 #  File:           ChEMBLTargetActivityProvider.py
 #  Date:           9-Nov-2020 jdw
 #
 #  Updated:
 #   9-Feb-2023 aae  Update ChEMBL baseVersion to 31
+#  18-Jul-2023 dwp  Update ChEMBL baseVersion to 33
 ##
 """
 Accessors for ChEMBL target activity data.
 
 """
 
 import datetime
@@ -122,15 +123,15 @@
     def __init__(self, cachePath, useCache):
         #
         self.__cachePath = cachePath
         self.__dirName = "ChEMBL-target-activity"
         super(ChEMBLTargetActivityProvider, self).__init__(self.__cachePath, [self.__dirName])
         self.__dirPath = os.path.join(self.__cachePath, self.__dirName)
         self.__mU = MarshalUtil(workPath=self.__cachePath)
-        baseVersion = 31
+        baseVersion = 33
         self.__version = baseVersion
         logger.info("ChEMBL API MAX_LIMIT %r", Settings.Instance().MAX_LIMIT)  # pylint: disable=no-member
         self.__aD, self.__allIdD = self.__reload(self.__dirPath, useCache)
 
     def testCache(self, minCount=0):
         if minCount == 0:
             return True
```

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
 #  File:           ChEMBLTargetMechanismProvider.py
 #  Date:           9-Nov-2020 jdw
 #
 #  Updated:
 #   9-Feb-2023 aae  Update ChEMBL baseVersion to 31
+#  18-Jul-2023 dwp  Update ChEMBL baseVersion to 33
 ##
 """
 Accessors for ChEMBL target mechanism data.
 
 """
 
 import datetime
@@ -35,15 +36,15 @@
     def __init__(self, cachePath, useCache):
         #
         self.__cachePath = cachePath
         self.__dirName = "ChEMBL-target-mechanism"
         super(ChEMBLTargetMechanismProvider, self).__init__(self.__cachePath, [self.__dirName])
         self.__dirPath = os.path.join(self.__cachePath, self.__dirName)
         self.__mU = MarshalUtil(workPath=self.__cachePath)
-        baseVersion = 31
+        baseVersion = 33
         self.__version = baseVersion
         logger.info("ChEMBL API MAX_LIMIT %r", Settings.Instance().MAX_LIMIT)  # pylint: disable=no-member
         self.__aD = self.__reload(self.__dirPath, useCache)
 
     def testCache(self, minCount=0):
         if minCount == 0:
             return True
```

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/ChEMBLTargetProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/ChEMBLTargetProvider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
 #  File:           ChEMBLTargetProvider.py
 #  Date:           9-Nov-2020 jdw
 #
 #  Updated:
 #   9-Feb-2023 aae  Update ChEMBL baseVersion to 31
+#  18-Jul-2023 dwp  Update ChEMBL baseVersion to 33
 ##
 """
 Accessors for ChEMBL target assignments.
 
 """
 
 import logging
@@ -27,15 +28,15 @@
 class ChEMBLTargetProvider:
     """Accessors for ChEMBL target assignments."""
 
     def __init__(self, cachePath, useCache, **kwargs):
         #
         self.__cachePath = cachePath
         self.__dirPath = os.path.join(self.__cachePath, "ChEMBL-targets")
-        baseVersion = 31
+        baseVersion = 33
         self.__version = baseVersion
         self.__mapD = self.__reload(self.__dirPath, baseVersion, useCache, **kwargs)
         #
 
     def testCache(self, minCount=0):
         return self.__mapD and len(self.__mapD) > minCount
```

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/DrugBankTargetCofactorProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/DrugBankTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/DrugBankTargetProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/DrugBankTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/IMGTTargetFeatureProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/IMGTTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/IMGTTargetProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/IMGTTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetActivityProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/PharosTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetCofactorProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/PharosTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/PharosTargetProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/PharosTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/SAbDabTargetFeatureProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/SAbDabTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb/utils/targets/SAbDabTargetProvider.py` & `rcsb.utils.targets-0.74/rcsb/utils/targets/SAbDabTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/PKG-INFO` & `rcsb.utils.targets-0.74/rcsb.utils.targets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.73
+Version: 0.74
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.73/rcsb.utils.targets.egg-info/SOURCES.txt` & `rcsb.utils.targets-0.74/rcsb.utils.targets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.73/setup.py` & `rcsb.utils.targets-0.74/setup.py`

 * *Files identical despite different names*

