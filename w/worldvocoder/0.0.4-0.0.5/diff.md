# Comparing `tmp/worldvocoder-0.0.4.tar.gz` & `tmp/worldvocoder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worldvocoder-0.0.4.tar", last modified: Wed Jul  5 16:30:39 2023, max compression
+gzip compressed data, was "worldvocoder-0.0.5.tar", last modified: Tue Jul 18 18:53:30 2023, max compression
```

## Comparing `worldvocoder-0.0.4.tar` & `worldvocoder-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-07-05 16:30:39.743472 worldvocoder-0.0.4/
--rw-r--r--   0 julianvanasse   (501) staff       (20)     1119 2023-05-27 21:20:51.000000 worldvocoder-0.0.4/LICENSE.txt
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3133 2023-07-05 16:30:39.743548 worldvocoder-0.0.4/PKG-INFO
--rw-r--r--   0 julianvanasse   (501) staff       (20)     2514 2023-06-08 22:48:56.000000 worldvocoder-0.0.4/README.md
--rw-r--r--   0 julianvanasse   (501) staff       (20)      443 2023-07-05 16:30:30.000000 worldvocoder-0.0.4/pyproject.toml
--rw-r--r--   0 julianvanasse   (501) staff       (20)      539 2023-07-05 16:30:39.743825 worldvocoder-0.0.4/setup.cfg
--rw-r--r--   0 julianvanasse   (501) staff       (20)      261 2023-06-07 18:55:58.000000 worldvocoder-0.0.4/setup.py
-drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-07-05 16:30:39.742750 worldvocoder-0.0.4/worldvocoder/
--rw-r--r--   0 julianvanasse   (501) staff       (20)       36 2023-06-07 18:23:35.000000 worldvocoder-0.0.4/worldvocoder/__init__.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     8151 2023-06-07 18:37:40.000000 worldvocoder-0.0.4/worldvocoder/cheaptrick.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    12066 2023-07-05 16:29:52.000000 worldvocoder-0.0.4/worldvocoder/d4c.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    11051 2023-06-07 20:00:18.000000 worldvocoder-0.0.4/worldvocoder/d4cRequiem.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    19600 2023-06-07 18:36:09.000000 worldvocoder-0.0.4/worldvocoder/dio.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3109 2023-06-07 18:38:11.000000 worldvocoder-0.0.4/worldvocoder/get_seeds_signals.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    27292 2023-06-07 19:34:25.000000 worldvocoder-0.0.4/worldvocoder/harvest.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    16426 2023-06-04 21:59:46.000000 worldvocoder-0.0.4/worldvocoder/main.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3371 2023-06-07 18:36:47.000000 worldvocoder-0.0.4/worldvocoder/stonemask.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     5949 2023-05-27 21:20:51.000000 worldvocoder-0.0.4/worldvocoder/swipe.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)    10742 2023-07-05 15:21:43.000000 worldvocoder-0.0.4/worldvocoder/synthesis.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     7101 2023-06-07 18:39:12.000000 worldvocoder-0.0.4/worldvocoder/synthesisRequiem.py
--rw-r--r--   0 julianvanasse   (501) staff       (20)     9540 2023-07-05 15:22:41.000000 worldvocoder-0.0.4/worldvocoder/synthesis_a.py
-drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-07-05 16:30:39.743360 worldvocoder-0.0.4/worldvocoder.egg-info/
--rw-r--r--   0 julianvanasse   (501) staff       (20)     3133 2023-07-05 16:30:39.000000 worldvocoder-0.0.4/worldvocoder.egg-info/PKG-INFO
--rw-r--r--   0 julianvanasse   (501) staff       (20)      532 2023-07-05 16:30:39.000000 worldvocoder-0.0.4/worldvocoder.egg-info/SOURCES.txt
--rw-r--r--   0 julianvanasse   (501) staff       (20)        1 2023-07-05 16:30:39.000000 worldvocoder-0.0.4/worldvocoder.egg-info/dependency_links.txt
--rw-r--r--   0 julianvanasse   (501) staff       (20)       13 2023-07-05 16:30:39.000000 worldvocoder-0.0.4/worldvocoder.egg-info/top_level.txt
+drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-07-18 18:53:30.527123 worldvocoder-0.0.5/
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     1119 2023-05-27 21:20:51.000000 worldvocoder-0.0.5/LICENSE.txt
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3133 2023-07-18 18:53:30.527204 worldvocoder-0.0.5/PKG-INFO
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     2514 2023-06-08 22:48:56.000000 worldvocoder-0.0.5/README.md
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      443 2023-07-18 18:53:22.000000 worldvocoder-0.0.5/pyproject.toml
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      539 2023-07-18 18:53:30.527570 worldvocoder-0.0.5/setup.cfg
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      261 2023-06-07 18:55:58.000000 worldvocoder-0.0.5/setup.py
+drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-07-18 18:53:30.526286 worldvocoder-0.0.5/worldvocoder/
+-rw-r--r--   0 julianvanasse   (501) staff       (20)       36 2023-06-07 18:23:35.000000 worldvocoder-0.0.5/worldvocoder/__init__.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     8151 2023-06-07 18:37:40.000000 worldvocoder-0.0.5/worldvocoder/cheaptrick.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    12066 2023-07-05 16:29:52.000000 worldvocoder-0.0.5/worldvocoder/d4c.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    11051 2023-06-07 20:00:18.000000 worldvocoder-0.0.5/worldvocoder/d4cRequiem.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    19600 2023-06-07 18:36:09.000000 worldvocoder-0.0.5/worldvocoder/dio.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3109 2023-06-07 18:38:11.000000 worldvocoder-0.0.5/worldvocoder/get_seeds_signals.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    27292 2023-06-07 19:34:25.000000 worldvocoder-0.0.5/worldvocoder/harvest.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    16426 2023-06-04 21:59:46.000000 worldvocoder-0.0.5/worldvocoder/main.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3371 2023-06-07 18:36:47.000000 worldvocoder-0.0.5/worldvocoder/stonemask.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     5949 2023-05-27 21:20:51.000000 worldvocoder-0.0.5/worldvocoder/swipe.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)    10779 2023-07-18 18:31:44.000000 worldvocoder-0.0.5/worldvocoder/synthesis.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     7101 2023-06-07 18:39:12.000000 worldvocoder-0.0.5/worldvocoder/synthesisRequiem.py
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     9540 2023-07-05 15:22:41.000000 worldvocoder-0.0.5/worldvocoder/synthesis_a.py
+drwxr-xr-x   0 julianvanasse   (501) staff       (20)        0 2023-07-18 18:53:30.526994 worldvocoder-0.0.5/worldvocoder.egg-info/
+-rw-r--r--   0 julianvanasse   (501) staff       (20)     3133 2023-07-18 18:53:30.000000 worldvocoder-0.0.5/worldvocoder.egg-info/PKG-INFO
+-rw-r--r--   0 julianvanasse   (501) staff       (20)      532 2023-07-18 18:53:30.000000 worldvocoder-0.0.5/worldvocoder.egg-info/SOURCES.txt
+-rw-r--r--   0 julianvanasse   (501) staff       (20)        1 2023-07-18 18:53:30.000000 worldvocoder-0.0.5/worldvocoder.egg-info/dependency_links.txt
+-rw-r--r--   0 julianvanasse   (501) staff       (20)       13 2023-07-18 18:53:30.000000 worldvocoder-0.0.5/worldvocoder.egg-info/top_level.txt
```

### Comparing `worldvocoder-0.0.4/LICENSE.txt` & `worldvocoder-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/PKG-INFO` & `worldvocoder-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worldvocoder
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python implementation of WORLD vocoder.
 Home-page: https://github.com/javanasse/Python-WORLD
 Download-URL: https://github.com/javanasse/Python-WORLD/archive/refs/tags/v0.tar.gz
 Author: JulianArmandVanasse
 Author-email: Julian <julian.vanasse@gmail.com>
 Project-URL: Homepage, https://github.com/javanasse/worldvocoder
 Classifier: Programming Language :: Python :: 3
```

### Comparing `worldvocoder-0.0.4/README.md` & `worldvocoder-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/setup.cfg` & `worldvocoder-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = worldvocoder
-version = 0.0.3
+version = 0.0.5
 author = JulianArmandVanasse
 author_email = julian.vanasse@gmail.com
 description = Python package for WORLD vocoder
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/javanasse/Python-WORLD
 classifiers =
```

### Comparing `worldvocoder-0.0.4/worldvocoder/cheaptrick.py` & `worldvocoder-0.0.5/worldvocoder/cheaptrick.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder/d4c.py` & `worldvocoder-0.0.5/worldvocoder/d4c.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder/d4cRequiem.py` & `worldvocoder-0.0.5/worldvocoder/d4cRequiem.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder/dio.py` & `worldvocoder-0.0.5/worldvocoder/dio.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder/get_seeds_signals.py` & `worldvocoder-0.0.5/worldvocoder/get_seeds_signals.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder/harvest.py` & `worldvocoder-0.0.5/worldvocoder/harvest.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder/main.py` & `worldvocoder-0.0.5/worldvocoder/main.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder/stonemask.py` & `worldvocoder-0.0.5/worldvocoder/stonemask.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder/swipe.py` & `worldvocoder-0.0.5/worldvocoder/swipe.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder/synthesis.py` & `worldvocoder-0.0.5/worldvocoder/synthesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         if n != int(n) or n <= 0:
             raise ValueError('n must be a nonnegative integer')
         if n < N_b:
             n = N_b
         N_fft = 2**nextpow2(n)
     else:
 
-        if N_x > N_b:
+        if np.floor(np.log2(N_x)) > np.ceil(np.log2(N_b)):
 
             # When the filter length is smaller than the signal,
             # choose the FFT length and block size that minimize the
             # FLOPS cost. Since the cost for a length-N FFT is
             # (N/2)*log2(N) and the filtering operation of each block
             # involves 2 FFT operations and N multiplications, the
             # cost of the overlap-add method for 1 length-N block is
```

### Comparing `worldvocoder-0.0.4/worldvocoder/synthesisRequiem.py` & `worldvocoder-0.0.5/worldvocoder/synthesisRequiem.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder/synthesis_a.py` & `worldvocoder-0.0.5/worldvocoder/synthesis_a.py`

 * *Files identical despite different names*

### Comparing `worldvocoder-0.0.4/worldvocoder.egg-info/PKG-INFO` & `worldvocoder-0.0.5/worldvocoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worldvocoder
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python implementation of WORLD vocoder.
 Home-page: https://github.com/javanasse/Python-WORLD
 Download-URL: https://github.com/javanasse/Python-WORLD/archive/refs/tags/v0.tar.gz
 Author: JulianArmandVanasse
 Author-email: Julian <julian.vanasse@gmail.com>
 Project-URL: Homepage, https://github.com/javanasse/worldvocoder
 Classifier: Programming Language :: Python :: 3
```

### Comparing `worldvocoder-0.0.4/worldvocoder.egg-info/SOURCES.txt` & `worldvocoder-0.0.5/worldvocoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

