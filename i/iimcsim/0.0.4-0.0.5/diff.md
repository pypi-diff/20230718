# Comparing `tmp/iimcsim-0.0.4.tar.gz` & `tmp/iimcsim-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iimcsim-0.0.4.tar", last modified: Mon May 22 08:41:26 2023, max compression
+gzip compressed data, was "iimcsim-0.0.5.tar", last modified: Tue Jul 18 15:00:36 2023, max compression
```

## Comparing `iimcsim-0.0.4.tar` & `iimcsim-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 08:41:26.520135 iimcsim-0.0.4/
--rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4260 2023-05-22 08:41:26.521140 iimcsim-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3620 2023-05-19 12:30:35.000000 iimcsim-0.0.4/README.md
--rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      747 2023-05-22 08:41:26.529188 iimcsim-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-22 08:41:26.008562 iimcsim-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 08:41:26.424758 iimcsim-0.0.4/src/iimcsim/
--rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.0.4/src/iimcsim/MC.py
--rw-rw-rw-   0        0        0    11861 2023-05-19 11:37:00.000000 iimcsim-0.0.4/src/iimcsim/MonteCarlo.py
--rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.0.4/src/iimcsim/__init__.py
--rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.0.4/src/iimcsim/data_gen.py
--rw-rw-rw-   0        0        0      574 2023-05-22 07:30:47.000000 iimcsim-0.0.4/src/iimcsim/data_gen_run.py
--rw-rw-rw-   0        0        0     2237 2023-05-22 08:36:01.000000 iimcsim-0.0.4/src/iimcsim/eda.py
--rw-rw-rw-   0        0        0     2624 2023-05-22 08:34:48.000000 iimcsim-0.0.4/src/iimcsim/shape_ext.py
--rw-rw-rw-   0        0        0    17269 2023-05-19 11:37:01.000000 iimcsim-0.0.4/src/iimcsim/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:41:26.511035 iimcsim-0.0.4/src/iimcsim.egg-info/
--rw-rw-rw-   0        0        0     4260 2023-05-22 08:41:25.000000 iimcsim-0.0.4/src/iimcsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-05-22 08:41:25.000000 iimcsim-0.0.4/src/iimcsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 08:41:25.000000 iimcsim-0.0.4/src/iimcsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 08:41:25.000000 iimcsim-0.0.4/src/iimcsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 15:00:36.311039 iimcsim-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4260 2023-07-18 15:00:36.312035 iimcsim-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3620 2023-05-19 12:30:35.000000 iimcsim-0.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      747 2023-07-18 15:00:36.320801 iimcsim-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 15:00:36.236289 iimcsim-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 15:00:36.283981 iimcsim-0.0.5/src/iimcsim/
+-rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.0.5/src/iimcsim/MC.py
+-rw-rw-rw-   0        0        0    11861 2023-06-20 08:51:34.000000 iimcsim-0.0.5/src/iimcsim/MonteCarlo.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.0.5/src/iimcsim/__init__.py
+-rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.0.5/src/iimcsim/data_gen.py
+-rw-rw-rw-   0        0        0      573 2023-07-18 14:57:50.000000 iimcsim-0.0.5/src/iimcsim/data_gen_run.py
+-rw-rw-rw-   0        0        0     2237 2023-05-22 08:36:01.000000 iimcsim-0.0.5/src/iimcsim/eda.py
+-rw-rw-rw-   0        0        0     2624 2023-05-22 08:34:48.000000 iimcsim-0.0.5/src/iimcsim/shape_ext.py
+-rw-rw-rw-   0        0        0    17269 2023-05-19 11:37:01.000000 iimcsim-0.0.5/src/iimcsim/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:00:36.309019 iimcsim-0.0.5/src/iimcsim.egg-info/
+-rw-rw-rw-   0        0        0     4260 2023-07-18 15:00:36.000000 iimcsim-0.0.5/src/iimcsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-07-18 15:00:36.000000 iimcsim-0.0.5/src/iimcsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 15:00:36.000000 iimcsim-0.0.5/src/iimcsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 15:00:36.000000 iimcsim-0.0.5/src/iimcsim.egg-info/top_level.txt
```

### Comparing `iimcsim-0.0.4/PKG-INFO` & `iimcsim-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: iimcsim Version: 0.0.4 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.0.5 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

### Comparing `iimcsim-0.0.4/README.md` & `iimcsim-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.4/setup.cfg` & `iimcsim-0.0.5/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 696d 6373 696d 0d0a 7665 7273   = iimcsim..vers
-00000020: 696f 6e20 3d20 302e 302e 340d 0a61 7574  ion = 0.0.4..aut
+00000020: 696f 6e20 3d20 302e 302e 350d 0a61 7574  ion = 0.0.5..aut
 00000030: 686f 7220 3d20 4a69 6761 7220 4268 616e  hor = Jigar Bhan
 00000040: 6465 7269 0d0a 6175 7468 6f72 5f65 6d61  deri..author_ema
 00000050: 696c 203d 206a 6967 6172 6268 616e 6465  il = jigarbhande
 00000060: 7269 4067 6d61 696c 2e63 6f6d 0d0a 6465  ri@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 7061  scription = A pa
 00000080: 636b 6167 6520 666f 7220 4d6f 6e74 652d  ckage for Monte-
 00000090: 4361 726c 6f20 7369 6d75 6c61 7469 6f6e  Carlo simulation
```

### Comparing `iimcsim-0.0.4/src/iimcsim/MC.py` & `iimcsim-0.0.5/src/iimcsim/MC.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.4/src/iimcsim/MonteCarlo.py` & `iimcsim-0.0.5/src/iimcsim/MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.4/src/iimcsim/data_gen.py` & `iimcsim-0.0.5/src/iimcsim/data_gen.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.4/src/iimcsim/data_gen_run.py` & `iimcsim-0.0.5/src/iimcsim/data_gen_run.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 def generate_data(train_exe = 50,
                 name = './src/data/plateauless_uniq_pulses_345.npy',
                 samp_size = 256,
                 max_num_photon = 60,
                 folder_name = 'sh06x2'):
     data_gen.generator(samp_size, max_num_photon, name, train_exe, folder_name)
-#generate_data()
+generate_data()
```

### Comparing `iimcsim-0.0.4/src/iimcsim/eda.py` & `iimcsim-0.0.5/src/iimcsim/eda.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.4/src/iimcsim/shape_ext.py` & `iimcsim-0.0.5/src/iimcsim/shape_ext.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.4/src/iimcsim/tools.py` & `iimcsim-0.0.5/src/iimcsim/tools.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.4/src/iimcsim.egg-info/PKG-INFO` & `iimcsim-0.0.5/src/iimcsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: iimcsim Version: 0.0.4 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.0.5 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

