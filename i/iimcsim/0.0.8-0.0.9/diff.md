# Comparing `tmp/iimcsim-0.0.8.tar.gz` & `tmp/iimcsim-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iimcsim-0.0.8.tar", last modified: Tue Jul 18 17:00:08 2023, max compression
+gzip compressed data, was "iimcsim-0.0.9.tar", last modified: Tue Jul 18 17:06:07 2023, max compression
```

## Comparing `iimcsim-0.0.8.tar` & `iimcsim-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 17:00:08.229690 iimcsim-0.0.8/
--rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4260 2023-07-18 17:00:08.229690 iimcsim-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3620 2023-05-19 12:30:35.000000 iimcsim-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      747 2023-07-18 17:00:08.232197 iimcsim-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 17:00:08.170438 iimcsim-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 17:00:08.205954 iimcsim-0.0.8/src/iimcsim/
--rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.0.8/src/iimcsim/MC.py
--rw-rw-rw-   0        0        0    11861 2023-06-20 08:51:34.000000 iimcsim-0.0.8/src/iimcsim/MonteCarlo.py
--rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.0.8/src/iimcsim/__init__.py
--rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.0.8/src/iimcsim/data_gen.py
--rw-rw-rw-   0        0        0      661 2023-07-18 15:21:44.000000 iimcsim-0.0.8/src/iimcsim/data_gen_run.py
--rw-rw-rw-   0        0        0     2392 2023-07-18 16:06:09.000000 iimcsim-0.0.8/src/iimcsim/eda.py
--rw-rw-rw-   0        0        0     2683 2023-07-18 16:59:35.000000 iimcsim-0.0.8/src/iimcsim/shape_ext.py
--rw-rw-rw-   0        0        0    17269 2023-05-19 11:37:01.000000 iimcsim-0.0.8/src/iimcsim/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:00:08.225701 iimcsim-0.0.8/src/iimcsim.egg-info/
--rw-rw-rw-   0        0        0     4260 2023-07-18 17:00:08.000000 iimcsim-0.0.8/src/iimcsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-07-18 17:00:08.000000 iimcsim-0.0.8/src/iimcsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:00:08.000000 iimcsim-0.0.8/src/iimcsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-18 17:00:08.000000 iimcsim-0.0.8/src/iimcsim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 17:00:08.227695 iimcsim-0.0.8/tests/
--rw-rw-rw-   0        0        0      951 2023-07-18 16:07:30.000000 iimcsim-0.0.8/tests/test_mc.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:06:07.311998 iimcsim-0.0.9/
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4260 2023-07-18 17:06:07.313355 iimcsim-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3620 2023-05-19 12:30:35.000000 iimcsim-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      747 2023-07-18 17:06:07.314890 iimcsim-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 17:06:07.222098 iimcsim-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 17:06:07.279635 iimcsim-0.0.9/src/iimcsim/
+-rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.0.9/src/iimcsim/MC.py
+-rw-rw-rw-   0        0        0    11861 2023-06-20 08:51:34.000000 iimcsim-0.0.9/src/iimcsim/MonteCarlo.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.0.9/src/iimcsim/__init__.py
+-rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.0.9/src/iimcsim/data_gen.py
+-rw-rw-rw-   0        0        0      661 2023-07-18 15:21:44.000000 iimcsim-0.0.9/src/iimcsim/data_gen_run.py
+-rw-rw-rw-   0        0        0     2392 2023-07-18 16:06:09.000000 iimcsim-0.0.9/src/iimcsim/eda.py
+-rw-rw-rw-   0        0        0     2698 2023-07-18 17:05:44.000000 iimcsim-0.0.9/src/iimcsim/shape_ext.py
+-rw-rw-rw-   0        0        0    17269 2023-05-19 11:37:01.000000 iimcsim-0.0.9/src/iimcsim/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:06:07.307503 iimcsim-0.0.9/src/iimcsim.egg-info/
+-rw-rw-rw-   0        0        0     4260 2023-07-18 17:06:07.000000 iimcsim-0.0.9/src/iimcsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-07-18 17:06:07.000000 iimcsim-0.0.9/src/iimcsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:06:07.000000 iimcsim-0.0.9/src/iimcsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 17:06:07.000000 iimcsim-0.0.9/src/iimcsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 17:06:07.309498 iimcsim-0.0.9/tests/
+-rw-rw-rw-   0        0        0      951 2023-07-18 16:07:30.000000 iimcsim-0.0.9/tests/test_mc.py
```

### Comparing `iimcsim-0.0.8/PKG-INFO` & `iimcsim-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for Monte-Carlo simulation for Intensity Interferometry
 Home-page: https://github.com/jigar2099/photon_position_reconstruction/tree/main
 Author: Jigar Bhanderi
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/jigar2099/photon_position_reconstruction/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iimcsim Version: 0.0.8 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.0.9 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

### Comparing `iimcsim-0.0.8/README.md` & `iimcsim-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.8/setup.cfg` & `iimcsim-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 696d 6373 696d 0d0a 7665 7273   = iimcsim..vers
-00000020: 696f 6e20 3d20 302e 302e 380d 0a61 7574  ion = 0.0.8..aut
+00000020: 696f 6e20 3d20 302e 302e 390d 0a61 7574  ion = 0.0.9..aut
 00000030: 686f 7220 3d20 4a69 6761 7220 4268 616e  hor = Jigar Bhan
 00000040: 6465 7269 0d0a 6175 7468 6f72 5f65 6d61  deri..author_ema
 00000050: 696c 203d 206a 6967 6172 6268 616e 6465  il = jigarbhande
 00000060: 7269 4067 6d61 696c 2e63 6f6d 0d0a 6465  ri@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 7061  scription = A pa
 00000080: 636b 6167 6520 666f 7220 4d6f 6e74 652d  ckage for Monte-
 00000090: 4361 726c 6f20 7369 6d75 6c61 7469 6f6e  Carlo simulation
```

### Comparing `iimcsim-0.0.8/src/iimcsim/MC.py` & `iimcsim-0.0.9/src/iimcsim/MC.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.8/src/iimcsim/MonteCarlo.py` & `iimcsim-0.0.9/src/iimcsim/MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.8/src/iimcsim/data_gen.py` & `iimcsim-0.0.9/src/iimcsim/data_gen.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.8/src/iimcsim/data_gen_run.py` & `iimcsim-0.0.9/src/iimcsim/data_gen_run.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.8/src/iimcsim/eda.py` & `iimcsim-0.0.9/src/iimcsim/eda.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.8/src/iimcsim/shape_ext.py` & `iimcsim-0.0.9/src/iimcsim/shape_ext.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         arr0 = -np.load(self.calib_file)[:bin_num] + threshold
         arr = np.where(arr0<0,0,arr0)
         arr_sub = arr-1
         arr_threshold = np.where(arr_sub<0,0,arr_sub)#/np.max(arr_sub)
         #print('calib_shape:',arr_w.shape)
         #print('arr:',arr.shape)
         #print('arr_sub_shape : ', arr_sub.shape)
-        #arr_threshold = arr_w.reshape(np.int(arr_w.shape[0]/100),100)
+        arr_threshold = arr_threshold.reshape(np.int(arr_threshold.shape[0]/100),100)
 
         rate = []
         ind = []
         val = []
         for i in range(arr_threshold.shape[0]):
             alp = arr_threshold[i].reshape(arr_threshold[i].shape[0],)
             peak_val, peak_ind = find_peaks(alp, height=0)
```

### Comparing `iimcsim-0.0.8/src/iimcsim/tools.py` & `iimcsim-0.0.9/src/iimcsim/tools.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.8/src/iimcsim.egg-info/PKG-INFO` & `iimcsim-0.0.9/src/iimcsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for Monte-Carlo simulation for Intensity Interferometry
 Home-page: https://github.com/jigar2099/photon_position_reconstruction/tree/main
 Author: Jigar Bhanderi
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/jigar2099/photon_position_reconstruction/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iimcsim Version: 0.0.8 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.0.9 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

### Comparing `iimcsim-0.0.8/tests/test_mc.py` & `iimcsim-0.0.9/tests/test_mc.py`

 * *Files identical despite different names*

