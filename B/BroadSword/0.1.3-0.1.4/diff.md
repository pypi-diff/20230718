# Comparing `tmp/BroadSword-0.1.3.tar.gz` & `tmp/BroadSword-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BroadSword-0.1.3.tar", last modified: Mon Jul 17 22:08:31 2023, max compression
+gzip compressed data, was "BroadSword-0.1.4.tar", last modified: Mon Jul 17 22:20:41 2023, max compression
```

## Comparing `BroadSword-0.1.3.tar` & `BroadSword-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:31.249608 BroadSword-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-17 22:08:20.000000 BroadSword-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-17 22:08:31.249608 BroadSword-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 22:08:20.000000 BroadSword-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 22:08:20.000000 BroadSword-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-17 22:08:31.249608 BroadSword-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:31.245608 BroadSword-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:31.249608 BroadSword-0.1.3/src/BroadSword/
--rw-r--r--   0 runner    (1001) docker     (123)    29710 2023-07-17 22:08:20.000000 BroadSword-0.1.3/src/BroadSword/BroadSword.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:08:20.000000 BroadSword-0.1.3/src/BroadSword/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-07-17 22:08:20.000000 BroadSword-0.1.3/src/BroadSword/libmatrices.so
--rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-07-17 22:08:20.000000 BroadSword-0.1.3/src/BroadSword/libmatrices_ARM64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-07-17 22:08:20.000000 BroadSword-0.1.3/src/BroadSword/libmatrices_x86_64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-17 22:08:20.000000 BroadSword-0.1.3/src/BroadSword/matrices.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:31.249608 BroadSword-0.1.3/src/BroadSword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-17 22:08:31.000000 BroadSword-0.1.3/src/BroadSword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 22:08:31.000000 BroadSword-0.1.3/src/BroadSword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:08:31.000000 BroadSword-0.1.3/src/BroadSword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 22:08:31.000000 BroadSword-0.1.3/src/BroadSword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 22:08:31.000000 BroadSword-0.1.3/src/BroadSword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:08:31.000000 BroadSword-0.1.3/src/BroadSword.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:20:41.540843 BroadSword-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-17 22:20:29.000000 BroadSword-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-17 22:20:41.540843 BroadSword-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 22:20:29.000000 BroadSword-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 22:20:29.000000 BroadSword-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-17 22:20:41.540843 BroadSword-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:20:41.532843 BroadSword-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:20:41.536843 BroadSword-0.1.4/src/BroadSword/
+-rw-r--r--   0 runner    (1001) docker     (123)    29722 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/BroadSword.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/libmatrices.so
+-rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/libmatrices_ARM64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/libmatrices_x86_64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-17 22:20:29.000000 BroadSword-0.1.4/src/BroadSword/matrices.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:20:41.540843 BroadSword-0.1.4/src/BroadSword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:20:41.000000 BroadSword-0.1.4/src/BroadSword.egg-info/zip-safe
```

### Comparing `BroadSword-0.1.3/LICENSE` & `BroadSword-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.3/PKG-INFO` & `BroadSword-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BroadSword-0.1.3/README.md` & `BroadSword-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.3/setup.cfg` & `BroadSword-0.1.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = BroadSword
-version = 0.1.3
+version = 0.1.4
 author = Cody Somers
 author_email = cas003@usask.ca
 description = Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Cody-Somers/BroadSword
 project_urls =
```

### Comparing `BroadSword-0.1.3/src/BroadSword/BroadSword.py` & `BroadSword-0.1.4/src/BroadSword/BroadSword.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,24 +84,24 @@
         fermi : float
             Specify the fermi energy for the ground state calculated spectra. Found in .scf2
         """
 
         with open(basedir+"/"+XES, "r") as xesFile: # Measured XES
             df = pd.read_csv(xesFile, delimiter='\s+',header=None) # Change to '\s*' and specify engine='python' if this breaks in jupyter notebook
             c1 = 0
-            max = 0
+            maxEXP = 0
             for i in range(len(df)): 
                 ExpSXS[0][c1][0] = df[0][c1] # Energy
                 ExpSXS[1][c1][0] = df[1][c1] # Counts
+                if ExpSXS[1][c1][0] > maxEXP:
+                    maxEXP = ExpSXS[1][c1][0]
                 c1 += 1
-                if ExpSXS[1][c1][0] > max:
-                    max = ExpSXS[1][c1][0]
             ExpSXSCount[0] = c1 # Length of data points
             for i in range(ExpSXSCount[0]):
-                ExpSXS[1][i][0] = ExpSXS[1][i][0]/max
+                ExpSXS[1][i][0] = ExpSXS[1][i][0]/maxEXP
 
         with open(basedir+"/"+XANES, "r") as xanesFile: # Measured XANES
             df = pd.read_csv(xanesFile, delimiter='\s+',header=None)
             c1 = 0
             for i in range(len(df)):
                 ExpSXS[0][c1][1] = df[0][c1] # Energy
                 ExpSXS[1][c1][1] = df[1][c1] # Counts
```

### Comparing `BroadSword-0.1.3/src/BroadSword/libmatrices.so` & `BroadSword-0.1.4/src/BroadSword/libmatrices.so`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.3/src/BroadSword/libmatrices_ARM64.dylib` & `BroadSword-0.1.4/src/BroadSword/libmatrices_ARM64.dylib`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.3/src/BroadSword/libmatrices_x86_64.dylib` & `BroadSword-0.1.4/src/BroadSword/libmatrices_x86_64.dylib`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.3/src/BroadSword/matrices.c` & `BroadSword-0.1.4/src/BroadSword/matrices.c`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1.3/src/BroadSword.egg-info/PKG-INFO` & `BroadSword-0.1.4/src/BroadSword.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

