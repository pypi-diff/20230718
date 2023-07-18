# Comparing `tmp/uncertainty-datatypes-1.0.2.tar.gz` & `tmp/uncertainty-datatypes-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncertainty-datatypes-1.0.2.tar", last modified: Tue Jul 18 13:52:23 2023, max compression
+gzip compressed data, was "uncertainty-datatypes-1.0.3.tar", last modified: Tue Jul 18 13:56:00 2023, max compression
```

## Comparing `uncertainty-datatypes-1.0.2.tar` & `uncertainty-datatypes-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:52:23.323691 uncertainty-datatypes-1.0.2/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.2/LICENSE
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10278 2023-07-18 13:52:23.323514 uncertainty-datatypes-1.0.2/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9507 2023-07-18 13:42:07.000000 uncertainty-datatypes-1.0.2/README.md
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:52:23.322036 uncertainty-datatypes-1.0.2/Uncertainty_Datatypes.egg-info/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10278 2023-07-18 13:52:23.000000 uncertainty-datatypes-1.0.2/Uncertainty_Datatypes.egg-info/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      665 2023-07-18 13:52:23.000000 uncertainty-datatypes-1.0.2/Uncertainty_Datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-18 13:52:23.000000 uncertainty-datatypes-1.0.2/Uncertainty_Datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-18 13:52:23.000000 uncertainty-datatypes-1.0.2/Uncertainty_Datatypes.egg-info/requires.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       11 2023-07-18 13:52:23.000000 uncertainty-datatypes-1.0.2/Uncertainty_Datatypes.egg-info/top_level.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-18 13:52:16.000000 uncertainty-datatypes-1.0.2/pyproject.toml
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-18 13:52:23.323727 uncertainty-datatypes-1.0.2/setup.cfg
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:52:23.322500 uncertainty-datatypes-1.0.2/test/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4428 2023-07-18 10:58:49.000000 uncertainty-datatypes-1.0.2/test/test_ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    13629 2023-07-18 11:54:36.000000 uncertainty-datatypes-1.0.2/test/test_ufloat.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      773 2023-07-18 08:46:41.000000 uncertainty-datatypes-1.0.2/test/test_ufuncs.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    12724 2023-07-18 11:52:34.000000 uncertainty-datatypes-1.0.2/test/test_uint.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:52:23.323131 uncertainty-datatypes-1.0.2/udatatypes/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.2/udatatypes/__init__.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.2/udatatypes/result.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4228 2023-07-18 09:14:56.000000 uncertainty-datatypes-1.0.2/udatatypes/ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20250 2023-07-18 13:47:37.000000 uncertainty-datatypes-1.0.2/udatatypes/unumbers.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4136 2023-07-18 13:12:04.000000 uncertainty-datatypes-1.0.2/udatatypes/utypes.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:56:00.096875 uncertainty-datatypes-1.0.3/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.3/LICENSE
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10278 2023-07-18 13:56:00.096702 uncertainty-datatypes-1.0.3/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9507 2023-07-18 13:42:07.000000 uncertainty-datatypes-1.0.3/README.md
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:56:00.095201 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10278 2023-07-18 13:56:00.000000 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      665 2023-07-18 13:56:00.000000 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-18 13:56:00.000000 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-18 13:56:00.000000 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/requires.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       11 2023-07-18 13:56:00.000000 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/top_level.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-18 13:55:47.000000 uncertainty-datatypes-1.0.3/pyproject.toml
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-18 13:56:00.096915 uncertainty-datatypes-1.0.3/setup.cfg
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:56:00.095669 uncertainty-datatypes-1.0.3/test/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4428 2023-07-18 10:58:49.000000 uncertainty-datatypes-1.0.3/test/test_ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    13629 2023-07-18 11:54:36.000000 uncertainty-datatypes-1.0.3/test/test_ufloat.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      773 2023-07-18 08:46:41.000000 uncertainty-datatypes-1.0.3/test/test_ufuncs.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    12724 2023-07-18 11:52:34.000000 uncertainty-datatypes-1.0.3/test/test_uint.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:56:00.096262 uncertainty-datatypes-1.0.3/udatatypes/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.3/udatatypes/__init__.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.3/udatatypes/result.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4311 2023-07-18 13:55:19.000000 uncertainty-datatypes-1.0.3/udatatypes/ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20250 2023-07-18 13:47:37.000000 uncertainty-datatypes-1.0.3/udatatypes/unumbers.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4136 2023-07-18 13:12:04.000000 uncertainty-datatypes-1.0.3/udatatypes/utypes.py
```

### Comparing `uncertainty-datatypes-1.0.2/LICENSE` & `uncertainty-datatypes-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.2/PKG-INFO` & `uncertainty-datatypes-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uncertainty-datatypes
-Version: 1.0.2
+Version: 1.0.3
 Summary: Uncertainty Datatypes Library
 Author: Atenea Research Group, University of Malaga, Spain
 Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
 Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `uncertainty-datatypes-1.0.2/README.md` & `uncertainty-datatypes-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.2/Uncertainty_Datatypes.egg-info/PKG-INFO` & `uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uncertainty-datatypes
-Version: 1.0.2
+Version: 1.0.3
 Summary: Uncertainty Datatypes Library
 Author: Atenea Research Group, University of Malaga, Spain
 Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
 Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `uncertainty-datatypes-1.0.2/Uncertainty_Datatypes.egg-info/SOURCES.txt` & `uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.2/test/test_ubool.py` & `uncertainty-datatypes-1.0.3/test/test_ubool.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.2/test/test_ufloat.py` & `uncertainty-datatypes-1.0.3/test/test_ufloat.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.2/test/test_ufuncs.py` & `uncertainty-datatypes-1.0.3/test/test_ufuncs.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.2/test/test_uint.py` & `uncertainty-datatypes-1.0.3/test/test_uint.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.2/udatatypes/ubool.py` & `uncertainty-datatypes-1.0.3/udatatypes/ubool.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,17 @@
 
     def copy(self) -> ubool:
         return ubool(self.c)
 
     ''' Conversions '''
     def __str__(self) -> str:
         return 'ubool({:5.3f})'.format(self.c)
+    
+    def __repr__(self) -> str:
+        return 'ubool({:5.3f})'.format(self.c)
 
     def tobool(self, c: float = None) -> bool:
         if c is None:
             c = self.__class__.CERTAINTY
         return self.c >= c
     
     def __bool__(self) -> bool:
```

### Comparing `uncertainty-datatypes-1.0.2/udatatypes/unumbers.py` & `uncertainty-datatypes-1.0.3/udatatypes/unumbers.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.2/udatatypes/utypes.py` & `uncertainty-datatypes-1.0.3/udatatypes/utypes.py`

 * *Files identical despite different names*

