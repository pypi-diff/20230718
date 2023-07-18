# Comparing `tmp/iimcsim-0.0.6.tar.gz` & `tmp/iimcsim-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iimcsim-0.0.6.tar", last modified: Tue Jul 18 15:22:44 2023, max compression
+gzip compressed data, was "iimcsim-0.0.7.tar", last modified: Tue Jul 18 16:08:28 2023, max compression
```

## Comparing `iimcsim-0.0.6.tar` & `iimcsim-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 15:22:44.138536 iimcsim-0.0.6/
--rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4260 2023-07-18 15:22:44.138536 iimcsim-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3620 2023-05-19 12:30:35.000000 iimcsim-0.0.6/README.md
--rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      747 2023-07-18 15:22:44.148572 iimcsim-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 15:22:44.063042 iimcsim-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 15:22:44.110287 iimcsim-0.0.6/src/iimcsim/
--rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.0.6/src/iimcsim/MC.py
--rw-rw-rw-   0        0        0    11861 2023-06-20 08:51:34.000000 iimcsim-0.0.6/src/iimcsim/MonteCarlo.py
--rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.0.6/src/iimcsim/__init__.py
--rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.0.6/src/iimcsim/data_gen.py
--rw-rw-rw-   0        0        0      661 2023-07-18 15:21:44.000000 iimcsim-0.0.6/src/iimcsim/data_gen_run.py
--rw-rw-rw-   0        0        0     2237 2023-05-22 08:36:01.000000 iimcsim-0.0.6/src/iimcsim/eda.py
--rw-rw-rw-   0        0        0     2624 2023-05-22 08:34:48.000000 iimcsim-0.0.6/src/iimcsim/shape_ext.py
--rw-rw-rw-   0        0        0    17269 2023-05-19 11:37:01.000000 iimcsim-0.0.6/src/iimcsim/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-18 15:22:44.133216 iimcsim-0.0.6/src/iimcsim.egg-info/
--rw-rw-rw-   0        0        0     4260 2023-07-18 15:22:44.000000 iimcsim-0.0.6/src/iimcsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-07-18 15:22:44.000000 iimcsim-0.0.6/src/iimcsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 15:22:44.000000 iimcsim-0.0.6/src/iimcsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-18 15:22:44.000000 iimcsim-0.0.6/src/iimcsim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 15:22:44.137110 iimcsim-0.0.6/tests/
--rw-rw-rw-   0        0        0       50 2023-07-18 15:18:19.000000 iimcsim-0.0.6/tests/test_mc.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:08:28.177735 iimcsim-0.0.7/
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4260 2023-07-18 16:08:28.178744 iimcsim-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3620 2023-05-19 12:30:35.000000 iimcsim-0.0.7/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      747 2023-07-18 16:08:28.184728 iimcsim-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 16:08:28.116202 iimcsim-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 16:08:28.148844 iimcsim-0.0.7/src/iimcsim/
+-rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.0.7/src/iimcsim/MC.py
+-rw-rw-rw-   0        0        0    11861 2023-06-20 08:51:34.000000 iimcsim-0.0.7/src/iimcsim/MonteCarlo.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.0.7/src/iimcsim/__init__.py
+-rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.0.7/src/iimcsim/data_gen.py
+-rw-rw-rw-   0        0        0      661 2023-07-18 15:21:44.000000 iimcsim-0.0.7/src/iimcsim/data_gen_run.py
+-rw-rw-rw-   0        0        0     2392 2023-07-18 16:06:09.000000 iimcsim-0.0.7/src/iimcsim/eda.py
+-rw-rw-rw-   0        0        0     2624 2023-05-22 08:34:48.000000 iimcsim-0.0.7/src/iimcsim/shape_ext.py
+-rw-rw-rw-   0        0        0    17269 2023-05-19 11:37:01.000000 iimcsim-0.0.7/src/iimcsim/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:08:28.172218 iimcsim-0.0.7/src/iimcsim.egg-info/
+-rw-rw-rw-   0        0        0     4260 2023-07-18 16:08:28.000000 iimcsim-0.0.7/src/iimcsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-07-18 16:08:28.000000 iimcsim-0.0.7/src/iimcsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 16:08:28.000000 iimcsim-0.0.7/src/iimcsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 16:08:28.000000 iimcsim-0.0.7/src/iimcsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 16:08:28.174213 iimcsim-0.0.7/tests/
+-rw-rw-rw-   0        0        0      951 2023-07-18 16:07:30.000000 iimcsim-0.0.7/tests/test_mc.py
```

### Comparing `iimcsim-0.0.6/PKG-INFO` & `iimcsim-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.0.6
+Version: 0.0.7
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
-Metadata-Version: 2.1 Name: iimcsim Version: 0.0.6 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.0.7 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

### Comparing `iimcsim-0.0.6/README.md` & `iimcsim-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.6/setup.cfg` & `iimcsim-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 696d 6373 696d 0d0a 7665 7273   = iimcsim..vers
-00000020: 696f 6e20 3d20 302e 302e 360d 0a61 7574  ion = 0.0.6..aut
+00000020: 696f 6e20 3d20 302e 302e 370d 0a61 7574  ion = 0.0.7..aut
 00000030: 686f 7220 3d20 4a69 6761 7220 4268 616e  hor = Jigar Bhan
 00000040: 6465 7269 0d0a 6175 7468 6f72 5f65 6d61  deri..author_ema
 00000050: 696c 203d 206a 6967 6172 6268 616e 6465  il = jigarbhande
 00000060: 7269 4067 6d61 696c 2e63 6f6d 0d0a 6465  ri@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 7061  scription = A pa
 00000080: 636b 6167 6520 666f 7220 4d6f 6e74 652d  ckage for Monte-
 00000090: 4361 726c 6f20 7369 6d75 6c61 7469 6f6e  Carlo simulation
```

### Comparing `iimcsim-0.0.6/src/iimcsim/MC.py` & `iimcsim-0.0.7/src/iimcsim/MC.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.6/src/iimcsim/MonteCarlo.py` & `iimcsim-0.0.7/src/iimcsim/MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.6/src/iimcsim/data_gen.py` & `iimcsim-0.0.7/src/iimcsim/data_gen.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.6/src/iimcsim/data_gen_run.py` & `iimcsim-0.0.7/src/iimcsim/data_gen_run.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.6/src/iimcsim/eda.py` & `iimcsim-0.0.7/src/iimcsim/eda.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import iimcsim.tools as fg
 import numpy as np
 from iimcsim.shape_ext import shape_generator
 
+class eda:
 
-def shapes_extraction(calib_data_path='../src/data/calib_ch0.npy',
-                      high_rate_path = '../src/data/shaula_00000-003_ch0.npy',
-                      data_save_path='../src/data/',
-                      bins = 21400
-                      ):
-    # required files
-    # calib.npy and shaula_00000-003_ch0.npy
-    select_files = shape_generator(calib_data_path, high_rate_path,data_save_path)
-    generate_shapes = select_files.generator(bin_num=bins)
-    shapes, save_path = select_files.scalar(generate_shapes)
-    # generated file
-    # shaula_00000-003_ch0_shapes.npy
-    return shapes
-
-def pulse_sh_plat(shapes_path = '../src/data/shaula_00000-003_ch0_shapes.npy',
-                  pulse_info_path = '../src/data/',
-                  plat_size_sel = 1,
-                  plot_save_path = '../plots/',
-                  lst=[3,4,5]):
-    uniq_shape = np.load(shapes_path)
-    # Generate data of extracted pulse, individually; pulse height, pulse width, skewness, kurtosis in dataframe format
-    df = fg.pulse_data(uniq_shape)
-    df.to_csv('calib_pulse_data.csv')
-    fg.skew_kurt(df, plat_size_sel, plot_save_path)
-    platauless_uniq_shapes, uniq_shapes = fg.filter_shapes_based_on_plat_size(df, uniq_shape, platau_removal=True, lst=lst, save_path=pulse_info_path)
-    return platauless_uniq_shapes, uniq_shapes
-
-
-shapes = shapes_extraction(r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data\calib_ch0.npy",
-                           r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data\shaula_00000-003_ch0.npy",
-                           r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data")
-
-pulse_sh_plat(r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data\shaula_00000-003_ch0_shapes.npy",
-              r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data",
-              plot_save_path = './')
+    def __init__(self):
+        pass
+
+    def shapes_extraction(self, calib_data_path='../src/data/calib_ch0.npy',
+                        high_rate_path = '../src/data/shaula_00000-003_ch0.npy',
+                        data_save_path='../src/data/',
+                        bins = 21400
+                        ):
+        # required files
+        # calib.npy and shaula_00000-003_ch0.npy
+        select_files = shape_generator(calib_data_path, high_rate_path,data_save_path)
+        generate_shapes = select_files.generator(bin_num=bins)
+        shapes, save_path = select_files.scalar(generate_shapes)
+        # generated file
+        # shaula_00000-003_ch0_shapes.npy
+        return shapes
+
+    def pulse_sh_plat(self, shapes_path = '../src/data/shaula_00000-003_ch0_shapes.npy',
+                    pulse_info_path = '../src/data/',
+                    plat_size_sel = 1,
+                    plot_save_path = '../plots/',
+                    lst=[3,4,5]):
+        uniq_shape = np.load(shapes_path)
+        # Generate data of extracted pulse, individually; pulse height, pulse width, skewness, kurtosis in dataframe format
+        df = fg.pulse_data(uniq_shape)
+        df.to_csv('calib_pulse_data.csv')
+        fg.skew_kurt(df, plat_size_sel, plot_save_path)
+        platauless_uniq_shapes, uniq_shapes = fg.filter_shapes_based_on_plat_size(df, uniq_shape, platau_removal=True, lst=lst, save_path=pulse_info_path)
+        return platauless_uniq_shapes, uniq_shapes
+
+
+#shapes = shapes_extraction(r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data\calib_ch0.npy",
+#                           r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data\shaula_00000-003_ch0.npy",
+#                           r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data")
+
+#pulse_sh_plat(r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data\shaula_00000-003_ch0_shapes.npy",
+#              r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data",
+#              plot_save_path = './')
```

### Comparing `iimcsim-0.0.6/src/iimcsim/shape_ext.py` & `iimcsim-0.0.7/src/iimcsim/shape_ext.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.6/src/iimcsim/tools.py` & `iimcsim-0.0.7/src/iimcsim/tools.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.0.6/src/iimcsim.egg-info/PKG-INFO` & `iimcsim-0.0.7/src/iimcsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.0.6
+Version: 0.0.7
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
-Metadata-Version: 2.1 Name: iimcsim Version: 0.0.6 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.0.7 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
```

