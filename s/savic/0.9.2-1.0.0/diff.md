# Comparing `tmp/savic-0.9.2.tar.gz` & `tmp/savic-1.0.0.tar.gz`

## Comparing `savic-0.9.2.tar` & `savic-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_C_C.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_C_CA.py
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_C_CB.py
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_C_CBA.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_Core.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_CoreAlpha.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_CoreBeam.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_CoreBeamAlpha.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_Input_Sort.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_P_C.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_P_CA.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_P_CB.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_P_CBA.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_Q_C.py
--rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_Q_CA.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_Q_CB.py
--rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/SAVIC_Q_CBA.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/Output/ML/models/GMM_C/00_dummy.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/Output/ML/models/GMM_CA/00_dummy.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/Output/ML/models/GMM_CB/00_dummy.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/Output/ML/models/GMM_CBA/00_dummy.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.2/src/savic/tutorial/00_dummy.txt
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 savic-0.9.2/LICENSE
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 savic-0.9.2/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 savic-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 savic-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_C_C.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_C_CA.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_C_CB.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_C_CBA.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_Core.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_CoreAlpha.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_CoreBeam.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_CoreBeamAlpha.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_Input_Sort.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_P_C.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_P_CA.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_P_CB.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_P_CBA.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_Q_C.py
+-rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_Q_CA.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_Q_CB.py
+-rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/SAVIC_Q_CBA.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/Output/ML/models/GMM_C/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/Output/ML/models/GMM_CA/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/Output/ML/models/GMM_CB/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/Output/ML/models/GMM_CBA/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-1.0.0/src/savic/tutorial/00_dummy.txt
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 savic-1.0.0/LICENSE
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 savic-1.0.0/README.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 savic-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 savic-1.0.0/PKG-INFO
```

### Comparing `savic-0.9.2/src/savic/SAVIC.py` & `savic-1.0.0/src/savic/SAVIC.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_C_C.py` & `savic-1.0.0/src/savic/SAVIC_C_C.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_C_CA.py` & `savic-1.0.0/src/savic/SAVIC_C_CA.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_C_CB.py` & `savic-1.0.0/src/savic/SAVIC_C_CB.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_C_CBA.py` & `savic-1.0.0/src/savic/SAVIC_C_CBA.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_Input_Sort.py` & `savic-1.0.0/src/savic/SAVIC_Input_Sort.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_P_C.py` & `savic-1.0.0/src/savic/SAVIC_P_C.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_P_CA.py` & `savic-1.0.0/src/savic/SAVIC_P_CA.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_P_CB.py` & `savic-1.0.0/src/savic/SAVIC_P_CB.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_Q_C.py` & `savic-1.0.0/src/savic/SAVIC_Q_C.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_Q_CA.py` & `savic-1.0.0/src/savic/SAVIC_Q_CA.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_Q_CB.py` & `savic-1.0.0/src/savic/SAVIC_Q_CB.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/SAVIC_Q_CBA.py` & `savic-1.0.0/src/savic/SAVIC_Q_CBA.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/__init__.py` & `savic-1.0.0/src/savic/__init__.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/src/savic/tutorial.py` & `savic-1.0.0/src/savic/tutorial.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/LICENSE` & `savic-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `savic-0.9.2/pyproject.toml` & `savic-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "savic"
-version = "0.9.2"
+version = "1.0.0"
 authors = [
   { name="Mihailo Martinovic", email="mmartinovic@arizona.edu" },
 ]
 description = "SAVIC package"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `savic-0.9.2/PKG-INFO` & `savic-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savic
-Version: 0.9.2
+Version: 1.0.0
 Summary: SAVIC package
 Project-URL: Homepage, https://pypi.org/project/savic/
 Project-URL: History, https://test.pypi.org/project/savic-test/
 Project-URL: Source, https://github.com/MihailoMartinovic/SAVIC
 Author-email: Mihailo Martinovic <mmartinovic@arizona.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

