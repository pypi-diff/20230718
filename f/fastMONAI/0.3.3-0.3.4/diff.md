# Comparing `tmp/fastMONAI-0.3.3.tar.gz` & `tmp/fastMONAI-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastMONAI-0.3.3.tar", last modified: Fri Jul 14 13:46:06 2023, max compression
+gzip compressed data, was "fastMONAI-0.3.4.tar", last modified: Tue Jul 18 14:17:50 2023, max compression
```

## Comparing `fastMONAI-0.3.3.tar` & `fastMONAI-0.3.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-14 13:46:06.873309 fastMONAI-0.3.3/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1101 2023-07-12 10:04:27.000000 fastMONAI-0.3.3/CONTRIBUTING.md
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    11337 2022-08-29 15:09:22.000000 fastMONAI-0.3.3/LICENSE
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      111 2022-08-29 15:09:22.000000 fastMONAI-0.3.3/MANIFEST.in
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-14 13:46:06.873309 fastMONAI-0.3.3/PKG-INFO
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4664 2023-03-31 13:03:15.000000 fastMONAI-0.3.3/README.md
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-14 13:46:06.873309 fastMONAI-0.3.3/fastMONAI/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       22 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/__init__.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    27510 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/_modidx.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4948 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/dataset_info.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    11016 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/external_data.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      590 2022-12-13 11:40:31.000000 fastMONAI-0.3.3/fastMONAI/research_utils.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1406 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/utils.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      360 2022-12-13 12:10:38.000000 fastMONAI-0.3.3/fastMONAI/vision_all.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9070 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_augmentation.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     7428 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_core.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    10491 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_data.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3744 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_inference.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3591 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_loss.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3549 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_metrics.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3095 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_plot.py
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-14 13:46:06.873309 fastMONAI-0.3.3/fastMONAI.egg-info/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/PKG-INFO
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      657 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/SOURCES.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/dependency_links.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       40 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/entry_points.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2022-08-29 15:24:47.000000 fastMONAI-0.3.3/fastMONAI.egg-info/not-zip-safe
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      133 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/requires.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       10 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/top_level.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1218 2023-07-14 13:40:38.000000 fastMONAI-0.3.3/settings.ini
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       38 2023-07-14 13:46:06.873309 fastMONAI-0.3.3/setup.cfg
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2541 2022-08-29 15:09:22.000000 fastMONAI-0.3.3/setup.py
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-18 14:17:50.479285 fastMONAI-0.3.4/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1101 2023-07-12 10:04:27.000000 fastMONAI-0.3.4/CONTRIBUTING.md
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    11337 2022-08-29 15:09:22.000000 fastMONAI-0.3.4/LICENSE
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      111 2022-08-29 15:09:22.000000 fastMONAI-0.3.4/MANIFEST.in
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-18 14:17:50.479285 fastMONAI-0.3.4/PKG-INFO
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4664 2023-03-31 13:03:15.000000 fastMONAI-0.3.4/README.md
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-18 14:17:50.479285 fastMONAI-0.3.4/fastMONAI/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       22 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/__init__.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    27510 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/_modidx.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4948 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/dataset_info.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    10964 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/external_data.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      590 2022-12-13 11:40:31.000000 fastMONAI-0.3.4/fastMONAI/research_utils.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1406 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/utils.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      360 2022-12-13 12:10:38.000000 fastMONAI-0.3.4/fastMONAI/vision_all.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9070 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/vision_augmentation.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     7590 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/vision_core.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    10491 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/vision_data.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3744 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/vision_inference.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3591 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/vision_loss.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3549 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/vision_metrics.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3095 2023-07-18 14:05:28.000000 fastMONAI-0.3.4/fastMONAI/vision_plot.py
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-18 14:17:50.479285 fastMONAI-0.3.4/fastMONAI.egg-info/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-18 14:17:50.000000 fastMONAI-0.3.4/fastMONAI.egg-info/PKG-INFO
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      657 2023-07-18 14:17:50.000000 fastMONAI-0.3.4/fastMONAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2023-07-18 14:17:50.000000 fastMONAI-0.3.4/fastMONAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       40 2023-07-18 14:17:50.000000 fastMONAI-0.3.4/fastMONAI.egg-info/entry_points.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2022-08-29 15:24:47.000000 fastMONAI-0.3.4/fastMONAI.egg-info/not-zip-safe
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      150 2023-07-18 14:17:50.000000 fastMONAI-0.3.4/fastMONAI.egg-info/requires.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       10 2023-07-18 14:17:50.000000 fastMONAI-0.3.4/fastMONAI.egg-info/top_level.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1235 2023-07-17 12:37:09.000000 fastMONAI-0.3.4/settings.ini
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       38 2023-07-18 14:17:50.479285 fastMONAI-0.3.4/setup.cfg
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2541 2022-08-29 15:09:22.000000 fastMONAI-0.3.4/setup.py
```

### Comparing `fastMONAI-0.3.3/CONTRIBUTING.md` & `fastMONAI-0.3.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/LICENSE` & `fastMONAI-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/PKG-INFO` & `fastMONAI-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastMONAI
-Version: 0.3.3
+Version: 0.3.4
 Summary: fastMONAI library
 Home-page: https://github.com/MMIV-ML/fastMONAI
 Author: Satheshkumar Kaliyugarasan
 Author-email: skka@hvl.no
 License: Apache Software License 2.0
 Keywords: deep learning,medical imaging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastMONAI-0.3.3/README.md` & `fastMONAI-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI/_modidx.py` & `fastMONAI-0.3.4/fastMONAI/_modidx.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI/dataset_info.py` & `fastMONAI-0.3.4/fastMONAI/dataset_info.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI/external_data.py` & `fastMONAI-0.3.4/fastMONAI/external_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     EXAMPLE_SPINE_DATA = 'https://drive.google.com/uc?id=1Ms3Q6MYQrQUA_PKZbJ2t2NeYFQ5jloMh'
     MEDMNIST_DICT = {'OrganMNIST3D': 'https://zenodo.org/record/6496656/files/organmnist3d.npz?download=1',	
                      'NoduleMNIST3D': 'https://zenodo.org/record/6496656/files/nodulemnist3d.npz?download=1',
                      'AdrenalMNIST3D': 'https://zenodo.org/record/6496656/files/adrenalmnist3d.npz?download=1',	
                      'FractureMNIST3D': 'https://zenodo.org/record/6496656/files/fracturemnist3d.npz?download=1',
                      'VesselMNIST3D': 'https://zenodo.org/record/6496656/files/vesselmnist3d.npz?download=1', 
                      'SynapseMNIST3D': 'https://zenodo.org/record/6496656/files/synapsemnist3d.npz?download=1'}
-    EXAMPLE_EC_DATA = 'https://drive.google.com/uc?id=1cjOBhkdRsoX3unxHiL377R5j8ottN4An'
+    EXAMPLE_EC_DATA = 'https://drive.google.com/uc?id=1yOmbA9-nKfzzsfysgp9OcPw8GAarXPvE'
 
 # %% ../nbs/09_external_data.ipynb 4
 def _process_ixi_xls(xls_path: (str, Path), img_path: Path) -> pd.DataFrame:
     """Private method to process the demographic information for the IXI dataset.
 
     Args:
         xls_path: File path to the xls file with the demographic information.
@@ -284,17 +284,14 @@
 
     dataset_file_path.unlink()
 
     return train_val_df, test_df
 
 # %% ../nbs/09_external_data.ipynb 19
 def download_example_endometrial_cancer_data(path: (str, Path) = '../data') -> Path:
-    study = 'ec'
     
     download_and_extract(
         url=MURLs.EXAMPLE_EC_DATA, 
         filepath='ec.zip', 
         output_dir=path
     )
     Path('ec.zip').unlink()
-    
-    return Path(path) / study
```

### Comparing `fastMONAI-0.3.3/fastMONAI/research_utils.py` & `fastMONAI-0.3.4/fastMONAI/research_utils.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI/utils.py` & `fastMONAI-0.3.4/fastMONAI/utils.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI/vision_augmentation.py` & `fastMONAI-0.3.4/fastMONAI/vision_augmentation.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI/vision_core.py` & `fastMONAI-0.3.4/fastMONAI/vision_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """
     org_img = LabelMap(file_path) if dtype is MedMask else ScalarImage(file_path) #_load(file_path, dtype=dtype) 
     input_img, org_size = _preprocess(org_img, reorder, resample)
     
     return org_img, input_img, org_size
 
 # %% ../nbs/01_vision_core.ipynb 7
-def _multi_channel(image_paths: list, reorder: bool, resample: list, dtype, only_tensor: bool):
+def _multi_channel(image_paths: (L, list), reorder: bool, resample: list, dtype, only_tensor: bool):
     """
     Load and preprocess multisequence data.
 
     Args:
         image_paths: List of image paths (e.g., T1, T2, T1CE, DWI).
         reorder: Whether to reorder data for canonical (RAS+) orientation.
         resample: Whether to resample image to different voxel sizes and dimensions.
@@ -80,36 +80,39 @@
        return dtype(tensor) 
 
     input_img.set_data(tensor)
     return org_img, input_img, org_size
 
 
 # %% ../nbs/01_vision_core.ipynb 8
-def med_img_reader(file_path: (str, Path), dtype=torch.Tensor, reorder: bool = False,
+def med_img_reader(file_path: (str, Path, L, list), dtype=torch.Tensor, reorder: bool = False,
                    resample: list = None, only_tensor: bool = True
 ):
     """Loads and preprocesses a medical image.
 
     Args:
-        file_path: Path to the image. Can be a string or a Path object.
+        file_path: Path to the image. Can be a string, Path object or a list.
         dtype: Datatype for the return value. Defaults to torch.Tensor.
         reorder: Whether to reorder the data to be closest to canonical 
             (RAS+) orientation. Defaults to False.
         resample: Whether to resample image to different voxel sizes and 
             image dimensions. Defaults to None.
         only_tensor: Whether to return only image tensor. Defaults to True.
 
     Returns:
         The preprocessed image. Returns only the image tensor if 
         only_tensor is True, otherwise returns original image, 
         preprocessed image, and original size.
     """
-    if isinstance(file_path, str) and ';' in file_path:
-        return _multi_channel(
-            file_path.split(';'), reorder, resample, dtype, only_tensor)
+    # if isinstance(file_path, str) and ';' in file_path:
+    #     return _multi_channel(
+    #         file_path.split(';'), reorder, resample, dtype, only_tensor)
+    
+    if isinstance(file_path, (L, list)):
+        return _multi_channel(file_path, reorder, resample, dtype, only_tensor)
 
     org_img, input_img, org_size = _load_and_preprocess(
         file_path, reorder, resample, dtype)
 
     if only_tensor:
         return dtype(input_img.data.type(torch.float))
 
@@ -130,15 +133,15 @@
     
     _bypass_type = torch.Tensor
     _show_args = {'cmap':'gray'}
     resample, reorder = None, False
     affine_matrix = None
 
     @classmethod
-    def create(cls, fn: (Path, str, torch.Tensor), **kwargs) -> torch.Tensor:
+    def create(cls, fn: (Path, str, L, list, torch.Tensor), **kwargs) -> torch.Tensor: 
         """
         Opens a medical image and casts it to MedBase object.
         If `fn` is a torch.Tensor, it's cast to MedBase object.
 
         Args:
             fn : (Path, str, torch.Tensor)
                 Image path or a 4D torch.Tensor.
```

### Comparing `fastMONAI-0.3.3/fastMONAI/vision_data.py` & `fastMONAI-0.3.4/fastMONAI/vision_data.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI/vision_inference.py` & `fastMONAI-0.3.4/fastMONAI/vision_inference.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI/vision_loss.py` & `fastMONAI-0.3.4/fastMONAI/vision_loss.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI/vision_metrics.py` & `fastMONAI-0.3.4/fastMONAI/vision_metrics.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI/vision_plot.py` & `fastMONAI-0.3.4/fastMONAI/vision_plot.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/fastMONAI.egg-info/PKG-INFO` & `fastMONAI-0.3.4/fastMONAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastMONAI
-Version: 0.3.3
+Version: 0.3.4
 Summary: fastMONAI library
 Home-page: https://github.com/MMIV-ML/fastMONAI
 Author: Satheshkumar Kaliyugarasan
 Author-email: skka@hvl.no
 License: Apache Software License 2.0
 Keywords: deep learning,medical imaging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastMONAI-0.3.3/fastMONAI.egg-info/SOURCES.txt` & `fastMONAI-0.3.4/fastMONAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.3/settings.ini` & `fastMONAI-0.3.4/settings.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified
 # see https://github.com/fastai/nbdev/blob/master/settings.ini for examples
 
 ### Python Library ###
 lib_name = fastMONAI
 min_python = 3.7
-version = 0.3.3
+version = 0.3.4
 ### OPTIONAL ###
 
-requirements = fastai==2.7.12 monai==1.2.0 torchio==0.18.91 xlrd>=1.2.0 scikit-image==0.19.3 huggingface-hub gdown
+requirements = fastai==2.7.12 monai==1.2.0 torchio==0.18.91 xlrd>=1.2.0 scikit-image==0.19.3 imagedata==2.1.3 huggingface-hub gdown
 dev_requirements = ipywidgets nbdev tabulate
 
 ### nbdev ###
 nbs_path = nbs
 doc_path = _docs
 recursive = False
 tst_flags = notest
```

### Comparing `fastMONAI-0.3.3/setup.py` & `fastMONAI-0.3.4/setup.py`

 * *Files identical despite different names*

