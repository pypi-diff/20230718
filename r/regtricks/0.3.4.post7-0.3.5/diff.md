# Comparing `tmp/regtricks-0.3.4.post7.tar.gz` & `tmp/regtricks-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regtricks-0.3.4.post7.tar", last modified: Thu Jul  6 10:08:25 2023, max compression
+gzip compressed data, was "regtricks-0.3.5.tar", last modified: Tue Jul 18 09:27:28 2023, max compression
```

## Comparing `regtricks-0.3.4.post7.tar` & `regtricks-0.3.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-06 10:08:25.568839 regtricks-0.3.4.post7/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1479 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/LICENSE
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       42 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/MANIFEST.in
--rw-r--r--   0 thomaskirk   (501) staff       (20)     1102 2023-07-06 10:08:25.568677 regtricks-0.3.4.post7/PKG-INFO
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      790 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/README.md
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-06 10:08:25.566561 regtricks-0.3.4.post7/regtricks/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      425 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/regtricks/__init__.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       76 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks/_version.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     7508 2022-01-05 10:40:43.000000 regtricks-0.3.4.post7/regtricks/application_helpers.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    15290 2022-02-12 22:48:27.000000 regtricks-0.3.4.post7/regtricks/fnirt_coefficients.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11764 2022-10-27 12:09:55.000000 regtricks-0.3.4.post7/regtricks/image_space.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8120 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/regtricks/multiplication.py
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-06 10:08:25.568467 regtricks-0.3.4.post7/regtricks/transforms/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      215 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/regtricks/transforms/__init__.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11571 2023-07-06 10:05:32.000000 regtricks-0.3.4.post7/regtricks/transforms/linear.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14937 2020-11-23 18:51:42.000000 regtricks-0.3.4.post7/regtricks/transforms/nonlinear.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8452 2022-05-09 11:26:49.000000 regtricks-0.3.4.post7/regtricks/transforms/transform.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3258 2020-10-30 18:59:14.000000 regtricks-0.3.4.post7/regtricks/wrappers.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     4387 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/regtricks/x5_interface.py
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-06 10:08:25.567884 regtricks-0.3.4.post7/regtricks.egg-info/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1102 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks.egg-info/PKG-INFO
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      561 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks.egg-info/SOURCES.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)        1 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks.egg-info/dependency_links.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       26 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks.egg-info/requires.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       10 2023-07-06 10:08:25.000000 regtricks-0.3.4.post7/regtricks.egg-info/top_level.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       25 2020-10-22 13:00:54.000000 regtricks-0.3.4.post7/requirements.txt
--rw-r--r--   0 thomaskirk   (501) staff       (20)       38 2023-07-06 10:08:25.568955 regtricks-0.3.4.post7/setup.cfg
--rwxr-xr-x   0 thomaskirk   (501) staff       (20)     3590 2022-02-12 22:43:08.000000 regtricks-0.3.4.post7/setup.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-18 09:27:28.030603 regtricks-0.3.5/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1479 2020-10-22 13:00:54.000000 regtricks-0.3.5/LICENSE
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       42 2020-10-22 13:00:54.000000 regtricks-0.3.5/MANIFEST.in
+-rw-r--r--   0 thomaskirk   (501) staff       (20)     1096 2023-07-18 09:27:28.030427 regtricks-0.3.5/PKG-INFO
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      790 2020-10-22 13:00:54.000000 regtricks-0.3.5/README.md
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-18 09:27:28.027974 regtricks-0.3.5/regtricks/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      425 2020-10-22 13:00:54.000000 regtricks-0.3.5/regtricks/__init__.py
+-rw-r--r--   0 thomaskirk   (501) staff       (20)       71 2023-07-18 09:27:27.000000 regtricks-0.3.5/regtricks/_version.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     7424 2023-07-10 10:27:24.000000 regtricks-0.3.5/regtricks/application_helpers.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    15302 2023-07-09 12:24:53.000000 regtricks-0.3.5/regtricks/fnirt_coefficients.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11883 2023-07-10 10:23:15.000000 regtricks-0.3.5/regtricks/image_space.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8120 2020-10-22 13:00:54.000000 regtricks-0.3.5/regtricks/multiplication.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-18 09:27:28.030044 regtricks-0.3.5/regtricks/transforms/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      215 2020-10-22 13:00:54.000000 regtricks-0.3.5/regtricks/transforms/__init__.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11570 2023-07-09 13:14:48.000000 regtricks-0.3.5/regtricks/transforms/linear.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14424 2023-07-10 10:04:05.000000 regtricks-0.3.5/regtricks/transforms/nonlinear.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     9471 2023-07-11 08:12:57.000000 regtricks-0.3.5/regtricks/transforms/transform.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3238 2023-07-09 13:15:39.000000 regtricks-0.3.5/regtricks/wrappers.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     4387 2020-10-22 13:00:54.000000 regtricks-0.3.5/regtricks/x5_interface.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-07-18 09:27:28.029029 regtricks-0.3.5/regtricks.egg-info/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1096 2023-07-18 09:27:27.000000 regtricks-0.3.5/regtricks.egg-info/PKG-INFO
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      561 2023-07-18 09:27:27.000000 regtricks-0.3.5/regtricks.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)        1 2023-07-18 09:27:27.000000 regtricks-0.3.5/regtricks.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       26 2023-07-18 09:27:27.000000 regtricks-0.3.5/regtricks.egg-info/requires.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       10 2023-07-18 09:27:27.000000 regtricks-0.3.5/regtricks.egg-info/top_level.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       25 2020-10-22 13:00:54.000000 regtricks-0.3.5/requirements.txt
+-rw-r--r--   0 thomaskirk   (501) staff       (20)       38 2023-07-18 09:27:28.030748 regtricks-0.3.5/setup.cfg
+-rwxr-xr-x   0 thomaskirk   (501) staff       (20)     3590 2022-02-12 22:43:08.000000 regtricks-0.3.5/setup.py
```

### Comparing `regtricks-0.3.4.post7/LICENSE` & `regtricks-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post7/PKG-INFO` & `regtricks-0.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtricks
-Version: 0.3.4.post7
+Version: 0.3.5
 Summary: Tools for manipulating and applying registrations
 Home-page: https://github.com/tomfrankkirk/regtricks
 Author: Tom Kirk
 Author-email: thomas.kirk@eng.ox.ac.uk
 License: BSD-3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `regtricks-0.3.4.post7/README.md` & `regtricks-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post7/regtricks/application_helpers.py` & `regtricks-0.3.5/regtricks/application_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 import functools
 import multiprocessing as mp 
-import tempfile 
-import os.path as op 
-import subprocess
-import os 
-import shutil 
-import itertools
+from pathlib import Path 
 
 import nibabel
 from nibabel import Nifti1Image, MGHImage
 from fsl.data.image import Image as FSLImage
-from fsl.wrappers import applywarp
 import numpy as np 
 from scipy.ndimage import map_coordinates
 
-from regtricks.image_space import ImageSpace
-
 
 def src_load_helper(src):
-    if isinstance(src, str):
+    if isinstance(src, (str, Path)):
         src = nibabel.load(src)
         data = src.get_fdata()
     elif isinstance(src, (Nifti1Image, MGHImage)):
         data = src.get_fdata()
     elif isinstance(src, FSLImage):
         data = src.data
     else: 
@@ -66,15 +58,16 @@
        (np.ndarray), sized as out_size, interpolated output 
     """
 
     # We transform a bool mask along with the input data to guard
     # against spline interpolation artefacts in the transformed data 
     superfactor = kwargs.pop('superfactor')
     ijk, scale = transform.resolve(src_spc, ref_spc, idx)
-    interp = map_coordinates(data, ijk, **kwargs)
+    interp = map_coordinates(data, ijk, mode='constant', 
+                             prefilter=True, **kwargs)
 
     # If the fill value has been specified, set the min/max
     # range for clipping in light of this 
     if 'cval' in kwargs:
         cval = kwargs['cval']
         cmin = data.min() if cval > data.min() else cval
         cmax = data.max() if cval < data.max() else cval
```

### Comparing `regtricks-0.3.4.post7/regtricks/fnirt_coefficients.py` & `regtricks-0.3.5/regtricks/fnirt_coefficients.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from distutils.log import warn
 import tempfile 
 import subprocess
 import os.path as op 
 import warnings 
+from pathlib import Path
 
 import nibabel 
 import numpy as np 
 
 from regtricks.image_space import ImageSpace
 from regtricks.application_helpers import aff_trans
 
 class FNIRTCoefficients(object):
     """
     Private encapsulation of FNIRT warp field. Only to be used 
     from within a NonLinearTransformation
 
     Args: 
         coeffs; nibabel object or path to coefficients file
-        src: str or ImageSpace, path to original source for transform
-        ref: str or ImageSpace, path to original reference for transform
+        src: Pathlike or ImageSpace, path to original source for transform
+        ref: Pathlike or ImageSpace, path to original reference for transform
         constrain_jac (bool/tuple): constrain the Jacobian of the transform
             (default False). If True, default limits of (0.01, 100) are used, 
             otherwise the limits (min,max) can be passed directly. 
     """
 
     def __init__(self, coeffs, src, ref, constrain_jac=False):
-        if isinstance(coeffs, str):
+        if isinstance(coeffs, (str, Path)):
             coeffs = nibabel.load(coeffs)
         else: 
             assert isinstance(coeffs, nibabel.Nifti1Image)
 
         if not isinstance(ref, ImageSpace):
             ref = ImageSpace(ref)
         self.ref_spc = ref
```

### Comparing `regtricks-0.3.4.post7/regtricks/image_space.py` & `regtricks-0.3.5/regtricks/image_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,38 +3,39 @@
 inverse, of an image. Used for resampling operations between different 
 spaces and also for saving images into said space (eg, save PV estimates 
 into the space of an image)
 """
 
 import copy 
 from textwrap import dedent
+from pathlib import Path
 
 import nibabel
 import numpy as np 
 from nibabel import Nifti1Image, MGHImage
 from fsl.data.image import Image as FSLImage
 
 
 class ImageSpace(object):
     """
     Voxel grid of an image, ignoring actual image data. 
 
     Args: 
-        img: path to image, nibabel Nifti/MGH or FSL Image object
+        img: Pathlike to image, nibabel Nifti/MGH or FSL Image object
     
     Attributes: 
         size: array of voxel counts in each dimension 
         vox_size: array of voxel size in each dimension 
         vox2world: 4x4 affine to transform voxel coords -> world
         world2vox: inverse of above 
     """
 
     def __init__(self, img):
 
-        if isinstance(img, str):
+        if isinstance(img, (str, Path)):
             fname = img 
             img = nibabel.load(img)
         else: 
             assert isinstance(img, (Nifti1Image, MGHImage, FSLImage))
             if type(img) is FSLImage:
                 img = img.nibImage
             fname = img.get_filename()
@@ -287,16 +288,20 @@
         nii = nibabel.nifti1.Nifti1Image(data, self.vox2world)
         return nii 
 
 
     def save_image(self, data, path):
         """Save 3D or 4D data array at path using this image's voxel grid"""
 
+        if not isinstance(path, str): 
+            path = str(path)
+
         if not (path.endswith('.nii') or path.endswith('.nii.gz')):
             path += '.nii.gz'
+            
         nii = self.make_nifti(data)
         nibabel.save(nii, path)
 
 
     def ijk_grid(self, indexing='ij'):
         """
         Return a 4D matrix of voxel indices for this space. Default indexing
```

### Comparing `regtricks-0.3.4.post7/regtricks/multiplication.py` & `regtricks-0.3.5/regtricks/multiplication.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post7/regtricks/transforms/linear.py` & `regtricks-0.3.5/regtricks/transforms/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 import os.path as op 
 from textwrap import dedent
 import glob 
 import os 
+from pathlib import Path 
 
-import nibabel
-from nibabel import Nifti1Image, MGHImage
 import numpy as np 
-from fsl.data.image import Image as FSLImage
 
 from regtricks.image_space import ImageSpace
-from regtricks import x5_interface as x5 
 from regtricks import application_helpers as apply
-from regtricks import multiplication as multiply
 from regtricks.transforms.transform import Transform
 
 class Registration(Transform):
     """
     Affine (4x4) transformation between two images.
 
     Args: 
-        src2ref (str/np.ndarray): path to text-like file to load or np.ndarray
+        src2ref (Pathlike, np.ndarray): path to text-like file to load or np.ndarray
     """
 
     def __init__(self, src2ref):
         Transform.__init__(self)
 
-        if isinstance(src2ref, str): 
+        if isinstance(src2ref, (str, Path)): 
             src2ref = np.loadtxt(src2ref)
 
         if (src2ref.shape != (4,4) 
             or (np.abs(src2ref[3,:] - [0,0,0,1]) > 1e-9).any()):
             raise RuntimeError("src2ref must be a 4x4 affine matrix, where ",
                                "the last row is [0,0,0,1].")
 
@@ -38,23 +34,23 @@
     @classmethod
     def from_flirt(cls, src2ref, src, ref):
         """
         Load an affine (4x4) transformation between two images directly from 
         FLIRT's -omat output. 
 
         Args: 
-            src2ref (str/np.ndarray): path to text-like file to load or np.ndarray
+            src2ref (Pathlike, np.ndarray): path to text-like file to load or np.ndarray
             src: the source of the transform 
             ref: the reference (or target) of the transform 
 
         Returns: 
             Registration object
         """
 
-        if isinstance(src2ref, str): 
+        if isinstance(src2ref, (str, Path)): 
             src2ref = np.loadtxt(src2ref)
 
         if not isinstance(src, ImageSpace):
             src = ImageSpace(src)
         src_spc = src 
         if not isinstance(ref, ImageSpace):
             ref = ImageSpace(ref)
@@ -163,14 +159,17 @@
             name order (all files will be loaded), or a list of individual
             filenames, or a list of np.arrays 
     """
 
     def __init__(self, mats):
         Transform.__init__(self)
 
+        if isinstance(mats, Path): 
+            mats = str(mats)
+
         if isinstance(mats, str):
             if op.isdir(mats): 
                 mats = sorted(glob.glob(op.join(mats, '*')))
                 if not mats: 
                     raise RuntimeError("Did not find any matrices in %s" % mats)
             else: 
                 mat = np.loadtxt(mats)
@@ -180,15 +179,15 @@
                 mats = [ mat[i*4:(i+1)*4,:] for i in range(mat.shape[0] // 4) ]
 
         if not mats: 
             raise RuntimeError("No matrices provided")
         
         self.__transforms = []
         for mat in mats:
-            if isinstance(mat, (np.ndarray, str)): 
+            if isinstance(mat, (np.ndarray, str, Path)): 
                 m = Registration(mat)
             else: 
                 m = mat 
             self.__transforms.append(m)
 
     def from_flirt(self, *args):
         raise NotImplementedError("Use the MotionCorrection.from_mcflirt() method")
@@ -207,14 +206,17 @@
             src: source of the transforms (ie, the image being corrected)
             ref: the target of the transforms (normally same as src)
 
         Returns: 
             MotionCorrection 
         """
 
+        if isinstance(mats, Path): 
+            mats = str(mats)
+
         if isinstance(mats, str):
             mats = sorted(glob.glob(op.join(mats, '*')))
             if not mats: 
                 raise RuntimeError("Did not find any matrices in %s" % mats)
 
         if isinstance(mats, np.ndarray):
             if mats.ndim == 3:
```

### Comparing `regtricks-0.3.4.post7/regtricks/transforms/nonlinear.py` & `regtricks-0.3.5/regtricks/transforms/nonlinear.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,14 @@
 
 class NonLinearRegistration(Transform):
     """
     Non linear registration transformation. Currently only FSL FNIRT warps
     are supported. Note that the --premat and --postmat used by FSL command
     line tools should not be supplied here. Instead, defined them as 
     Registration objects and use chain() to concatenate them with NLRs. 
-
-    
-    Args: 
-        warp (path): FNIRT coefficient field 
-        src (path/ImageSpace): source image used for generating FNIRT coefficients
-        ref (path/ImageSpace): reference image used for generating FNIRT coefficients 
-        intensity_correct: intensity correct output via the Jacobian determinant
-            of this warp (when self.apply_to*() is called)
-        constrain_jac (bool/array-like): constrain Jacobian for intensity
-            correction (default False). If True, limits of (0.01, 100) will 
-            be used, or explicit limits can be given as (min, max)
     """
 
     def __init__():
 
         raise NotImplementedError("Currently only FNIRT supported, use "
                                 "NonLinearRegistration.from_fnirt() instead")
 
@@ -48,23 +37,23 @@
         """
         FNIRT non-linear registration from a coefficients file. If a pre-warp
         and post-warp transformation need to be applied, create these as 
         separate Registration objects and combine them via chain, ie, 
         combined = chain(pre, non-linear, post)
 
         Args: 
-            coefficients (str/nibabel NIFTI): FNIRT coefficients 
-            src (str/ImageSpace): the source of the warp 
-            ref (str/ImageSpace): the reference of the warp 
-            intensity_correct (bool): whether to apply intensity correction via
-                the determinant of the warp's Jacobian (default false)
+            coefficients (Pathlike): FNIRT coefficient field 
+            src (Pathlike, ImageSpace): source image used for generating FNIRT coefficients
+            ref (Pathlike, ImageSpace): reference image used for generating FNIRT coefficients 
+            intensity_correct: intensity correct output via the Jacobian determinant
+                of this warp (when self.apply_to*() is called)
             constrain_jac (bool/array-like): constrain Jacobian for intensity
                 correction (default False). If True, limits of (0.01, 100) will 
                 be used, or explicit limits can be given as (min, max)
-
+                
         Returns: 
             NonLinearRegistration object 
         """
 
         warp = FNIRTCoefficients(coefficients, src, ref, constrain_jac)
         return NonLinearRegistration._manual_construct(warp, 
             np.eye(4), np.eye(4), intensity_correct)
```

### Comparing `regtricks-0.3.4.post7/regtricks/transforms/transform.py` & `regtricks-0.3.5/regtricks/transforms/transform.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os.path as op 
 from textwrap import dedent
 from multiprocessing import cpu_count
 
 from nibabel import Nifti1Image, MGHImage
 import numpy as np 
 from fsl.data.image import Image as FSLImage
+from scipy.ndimage import binary_fill_holes
 
 from regtricks.image_space import ImageSpace
 from regtricks import x5_interface as x5 
 from regtricks import application_helpers as apply
 from regtricks import multiplication as multiply
 
 # cache for intensity correction?
@@ -99,72 +100,79 @@
             return multiply.nonlinearreg(other, self)
         elif high_type is NonLinearMotionCorrection:
             return multiply.nonlinearmoco(other, self)
         else: 
             raise NotImplementedError("Not Transformation objects")
 
     def apply_to_image(self, src, ref, order=3, superfactor=True, 
-                        cores=cpu_count(), cval=0.0, **kwargs):
+                        mask=True, cval=0.0, cores=cpu_count(), **kwargs):
         """
         Applies transformation to data array. If a registration is applied 
         to 4D data, the same transformation will be applied to all volumes 
         in the series. 
 
         Args:   
-            src (str/NII/MGZ/FSLImage): image to transform 
-            ref (str/NII/MGZ/FSLImage/ImageSpace): target space for data 
+            src (Pathlike/NII/MGZ/FSLImage): image to transform 
+            ref (Pathlike/NII/MGZ/FSLImage/ImageSpace): target space for data 
             order (int): 0 for NN, 1 for linear, 2-5 for splines. 
             superfactor (bool/int/iterable): default True for any order > 0,
                 (chosen automatically); intermediate super-sampling (replicates
                 applywarp -super), enabled by default when resampling from 
                 high to low resolution. Set as False to disable, or set an 
                 int/iterable to manually specify level for each image dimension. 
+            mask (bool): for order > 1, mask output to remove negligible 
+                values due to spline artefact 
+            cval (float): fill value for background, used for correcting
+                spline artefact
             cores (int): CPU cores to use for 4D data
-            cval (float): fill value for locations outside of the image
             **kwargs: passed on to scipy.ndimage.map_coordinates
 
         Returns: 
             (np.array) transformed image data in ref voxel grid.
         """
 
         data, creator = apply.src_load_helper(src)
-        resamp = self.apply_to_array(data, src, ref, order, superfactor, 
-                                     cores, cval, **kwargs)
+        resamp = self.apply_to_array(data, src=src, ref=ref, order=order, 
+                                     superfactor=superfactor, mask=mask, 
+                                     cores=cores, cval=cval, **kwargs)
         if not isinstance(ref, ImageSpace):
             ref = ImageSpace(ref)
         
         if creator is MGHImage:
             ret = MGHImage(resamp, ref.vox2world, ref.header)
             return ret 
         else: 
             ret = Nifti1Image(resamp, ref.vox2world, ref.header)
             if creator is FSLImage:
                 return FSLImage(ret)
             else: 
                 return ret 
 
     def apply_to_array(self, data, src, ref, order=3, superfactor=True,
-                        cores=cpu_count(), cval=0.0, **kwargs):
+                        mask=True, cval=0.0, cores=cpu_count(), **kwargs):
         """
         Applies transformation to data array. If a registration is applied 
         to 4D data, the same transformation will be applied to all volumes 
         in the series. 
 
         Args:   
             data (array): 3D or 4D array. 
-            src (str/NII/MGZ/FSLImage/ImageSpace): current space of data 
-            ref (str/NII/MGZ/FSLImage/ImageSpace): target space for data 
+            src (Pathlike/NII/MGZ/FSLImage/ImageSpace): current space of data 
+            ref (Pathlike/NII/MGZ/FSLImage/ImageSpace): target space for data 
             order (int): 0 for NN, 1 for linear, 2-5 for splines. 
             superfactor (bool/int/iterable): default True for any order > 0,
                 (chosen automatically); intermediate super-sampling (replicates
                 applywarp -super), enabled by default when resampling from 
                 high to low resolution. Set as False to disable, or set an 
                 int/iterable to manually specify level for each image dimension. 
+            mask (bool): for order > 1, mask output to remove negligible 
+                values due to spline artefact 
+            cval (float): fill value for background, used for correcting
+                spline artefact
             cores (int): CPU cores to use for 4D data
-            cval (float): fill value for locations outside of the image
             **kwargs: passed on to scipy.ndimage.map_coordinates
 
         Returns: 
             (np.array) transformed image data in ref voxel grid.
         """
 
         if not isinstance(src, ImageSpace):
@@ -190,15 +198,17 @@
             superfactor = np.ones(3)
         superfactor = superfactor.astype(int)
 
         if (superfactor < 1).any(): 
             raise ValueError("Superfactor must be integer > 0")
 
         if (superfactor != 1).any(): 
-            ref = ref.resize_voxels(1 / superfactor, 'ceil')
+            super_ref = ref.resize_voxels(1 / superfactor, 'ceil')
+        else: 
+            super_ref = ref 
 
         if not ((data.ndim in (3,4)) and (np.array_equal(src.size, data.shape[:3]))): 
             raise ValueError("Data shape {} does not match source space {}"
                                 .format(data.shape, src.size))
 
         # Force to float data 
         if data.dtype.kind != 'f': 
@@ -211,10 +221,21 @@
             cores = min([cores, data.shape[-1]])
 
         kwargs.update({
             'cval': cval,
             'superfactor': superfactor,
             'order': order
             })
-        resamp = apply.despatch(data, self, src, ref, cores, **kwargs)
+        resamp = apply.despatch(data, self, src, super_ref, cores, **kwargs)
+
+        if mask and (order > 1): 
+            mvol = (data != cval) 
+            while mvol.ndim < 4: 
+                mvol = mvol[...,None]
+            mvol = np.stack([ binary_fill_holes(mvol[...,idx]) for idx in range(mvol.shape[3]) ], axis=-1) 
+            if mvol.ndim > data.ndim: 
+                mvol = np.squeeze(mvol)
+            mres = self.apply_to_array(mvol, src, ref, order=1, mask=False)
+            mres = (np.squeeze(mres) > 0.5)
+            resamp[~mres] = cval 
 
         return resamp
```

### Comparing `regtricks-0.3.4.post7/regtricks/wrappers.py` & `regtricks-0.3.5/regtricks/wrappers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import tempfile
 import os.path as op 
 import shutil
+from pathlib import Path
 
-import numpy as np
 import nibabel
 from fsl.wrappers.flirt import flirt as flirt_cmd
 from fsl.wrappers.flirt import mcflirt as mcflirt_cmd
 from fsl.wrappers.fnirt import fnirt as fnirt_cmd 
-from fsl.data.image import Image as FSLImage
 
 from regtricks.transforms import Registration, MotionCorrection, NonLinearRegistration
 
 def flirt(src, ref, **kwargs):
     """
     FLIRT registration wrapper. If any of the output arguments are given
     (out/o and omat), FLIRT will run in command line mode and save the 
@@ -43,24 +42,24 @@
     MCFLIRT motion correction wrapper. If an output path is given, MCFLIRT
     will run in command line mode, save the output and return None. If no
     output path is given, a MotionCorrection and Nibabel image for the frame
     used as the reference will be returned. See fsl.wrappers.flirt.mcflirt
     for full docs. 
 
     Args: 
-        src: image to register
+        src: (Pathlike) image to register
         refvol: target frame to register on to, default is N/2
         out: where to save output
         **kwargs: as for MCFLIRT
     
     Returns: 
         MotionCorrection object
     """
 
-    if isinstance(src, str):
+    if isinstance(src, (str, Path)):
         src_path = src 
         src = nibabel.load(src)
 
     if (refvol == -1) and (refvol not in kwargs):
         refvol = src.shape[-1] // 2
         kwargs['refvol'] = refvol
     else:
```

### Comparing `regtricks-0.3.4.post7/regtricks/x5_interface.py` & `regtricks-0.3.5/regtricks/x5_interface.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post7/regtricks.egg-info/PKG-INFO` & `regtricks-0.3.5/regtricks.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtricks
-Version: 0.3.4.post7
+Version: 0.3.5
 Summary: Tools for manipulating and applying registrations
 Home-page: https://github.com/tomfrankkirk/regtricks
 Author: Tom Kirk
 Author-email: thomas.kirk@eng.ox.ac.uk
 License: BSD-3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `regtricks-0.3.4.post7/regtricks.egg-info/SOURCES.txt` & `regtricks-0.3.5/regtricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4.post7/setup.py` & `regtricks-0.3.5/setup.py`

 * *Files identical despite different names*

