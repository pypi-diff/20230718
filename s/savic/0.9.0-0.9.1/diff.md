# Comparing `tmp/savic-0.9.0.tar.gz` & `tmp/savic-0.9.1.tar.gz`

## Comparing `savic-0.9.0.tar` & `savic-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_C_C.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_C_CA.py
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_C_CB.py
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_C_CBA.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Core.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_CoreAlpha.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_CoreBeam.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_CoreBeamAlpha.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Input_Sort.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_P_C.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_P_CA.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_P_CB.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_P_CBA.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Q_C.py
--rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Q_CA.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Q_CB.py
--rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/SAVIC_Q_CBA.py
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/Output/ML/models/GMM_C/00_dummy.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/Output/ML/models/GMM_CA/00_dummy.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/Output/ML/models/GMM_CB/00_dummy.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/Output/ML/models/GMM_CBA/00_dummy.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.0/src/savic/tutorial/00_dummy.txt
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 savic-0.9.0/LICENSE
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 savic-0.9.0/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 savic-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 savic-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_C_C.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_C_CA.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_C_CB.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_C_CBA.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_Core.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_CoreAlpha.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_CoreBeam.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_CoreBeamAlpha.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_Input_Sort.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_P_C.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_P_CA.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_P_CB.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_P_CBA.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_Q_C.py
+-rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_Q_CA.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_Q_CB.py
+-rw-r--r--   0        0        0    12383 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/SAVIC_Q_CBA.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/Output/ML/models/GMM_C/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/Output/ML/models/GMM_CA/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/Output/ML/models/GMM_CB/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/Output/ML/models/GMM_CBA/00_dummy.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 savic-0.9.1/src/savic/tutorial/00_dummy.txt
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 savic-0.9.1/LICENSE
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 savic-0.9.1/README.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 savic-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 savic-0.9.1/PKG-INFO
```

### Comparing `savic-0.9.0/src/savic/SAVIC.py` & `savic-0.9.1/src/savic/SAVIC.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_C_C.py` & `savic-0.9.1/src/savic/SAVIC_C_C.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_C_CA.py` & `savic-0.9.1/src/savic/SAVIC_C_CA.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_C_CB.py` & `savic-0.9.1/src/savic/SAVIC_C_CB.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_C_CBA.py` & `savic-0.9.1/src/savic/SAVIC_C_CBA.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_Input_Sort.py` & `savic-0.9.1/src/savic/SAVIC_Input_Sort.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_P_C.py` & `savic-0.9.1/src/savic/SAVIC_P_C.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_P_CA.py` & `savic-0.9.1/src/savic/SAVIC_P_CA.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_P_CB.py` & `savic-0.9.1/src/savic/SAVIC_P_CB.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_Q_C.py` & `savic-0.9.1/src/savic/SAVIC_Q_C.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_Q_CA.py` & `savic-0.9.1/src/savic/SAVIC_Q_CA.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_Q_CB.py` & `savic-0.9.1/src/savic/SAVIC_Q_CB.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/SAVIC_Q_CBA.py` & `savic-0.9.1/src/savic/SAVIC_Q_CBA.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/src/savic/__init__.py` & `savic-0.9.1/src/savic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         if '/' in name:
             print(name.split('/'))
             wget.download(url_, out = path_ + name.split('/')[0] + '/')
         else:
             wget.download(url_, out = path_)
         print('')
 
-names = ['SAVIC_Examples.h5', 'SAVIC_readme.pdf', 'savicing.ipynb', 'Article_I_Statistical_Trends.pdf', 'Article_II_Classification_and_Multidimensional_Mapping.pdf']
+names = ['SAVIC_Examples.h5', 'SAVIC_readme.pdf', 'SAVIC_testing.ipynb', 'Article_I_Statistical_Trends.pdf', 'Article_II_Classification_and_Multidimensional_Mapping.pdf']
 
 path_ = os.path.dirname(np.__file__.replace('numpy','savic').replace('__init__.py', '')) + '/tutorial/'
 
 for name in names:
     is_file_ = os.path.isfile(path_+name)
     if is_file_:
         size_ = os.path.getsize(path_+name)
```

### Comparing `savic-0.9.0/src/savic/tutorial.py` & `savic-0.9.1/src/savic/tutorial.py`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/LICENSE` & `savic-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `savic-0.9.0/pyproject.toml` & `savic-0.9.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "savic"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
   { name="Mihailo Martinovic", email="mmartinovic@arizona.edu" },
 ]
 description = "SAVIC package"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `savic-0.9.0/PKG-INFO` & `savic-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savic
-Version: 0.9.0
+Version: 0.9.1
 Summary: SAVIC package
 Project-URL: Homepage, https://pypi.org/project/savic/
 Project-URL: History, https://test.pypi.org/project/savic-test/
 Project-URL: Source, https://github.com/MihailoMartinovic/SAVIC
 Author-email: Mihailo Martinovic <mmartinovic@arizona.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

