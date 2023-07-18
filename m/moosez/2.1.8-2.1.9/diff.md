# Comparing `tmp/moosez-2.1.8.tar.gz` & `tmp/moosez-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.1.8.tar", last modified: Sun Jul  2 12:54:44 2023, max compression
+gzip compressed data, was "moosez-2.1.9.tar", last modified: Mon Jul 10 10:12:47 2023, max compression
```

## Comparing `moosez-2.1.8.tar` & `moosez-2.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:54:44.413198 moosez-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 12:54:35.000000 moosez-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-02 12:54:44.413198 moosez-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-02 12:54:35.000000 moosez-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:54:44.413198 moosez-2.1.8/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-02 12:54:35.000000 moosez-2.1.8/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:54:44.413198 moosez-2.1.8/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 12:54:44.000000 moosez-2.1.8/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 12:54:44.413198 moosez-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-02 12:54:35.000000 moosez-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:12:47.490094 moosez-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 10:12:36.000000 moosez-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-10 10:12:47.490094 moosez-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-10 10:12:36.000000 moosez-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:12:47.486094 moosez-2.1.9/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-10 10:12:36.000000 moosez-2.1.9/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:12:47.490094 moosez-2.1.9/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 10:12:47.000000 moosez-2.1.9/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:12:47.490094 moosez-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-10 10:12:36.000000 moosez-2.1.9/setup.py
```

### Comparing `moosez-2.1.8/LICENSE` & `moosez-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/PKG-INFO` & `moosez-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.8
+Version: 2.1.9
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.1.8/README.md` & `moosez-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/moosez/constants.py` & `moosez-2.1.9/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/moosez/display.py` & `moosez-2.1.9/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/moosez/download.py` & `moosez-2.1.9/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/moosez/file_utilities.py` & `moosez-2.1.9/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/moosez/image_processing.py` & `moosez-2.1.9/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/moosez/input_validation.py` & `moosez-2.1.9/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/moosez/moosez.py` & `moosez-2.1.9/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/moosez/predict.py` & `moosez-2.1.9/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/moosez/resources.py` & `moosez-2.1.9/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.1.8/moosez.egg-info/PKG-INFO` & `moosez-2.1.9/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.1.8
+Version: 2.1.9
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.1.8/setup.py` & `moosez-2.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.1.8',
+    version='2.1.9',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
@@ -47,15 +47,15 @@
         'pyfiglet~=0.8.post1',
         'natsort~=8.1.0',
         'pillow>=9.2.0',
         'colorama~=0.4.6',
         'dask~=2023.6.0',
         'rich',
         'pandas',
-        'dicom2nifti~=2.4.8'
+        'dcm2niix'
     ],
     entry_points={
         'console_scripts': [
             'moosez=moosez.moosez:main',
         ],
     },
 )
```

