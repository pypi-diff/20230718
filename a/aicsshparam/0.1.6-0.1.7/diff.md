# Comparing `tmp/aicsshparam-0.1.6.tar.gz` & `tmp/aicsshparam-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicsshparam-0.1.6.tar", last modified: Tue Apr 18 02:56:19 2023, max compression
+gzip compressed data, was "aicsshparam-0.1.7.tar", last modified: Tue Jul 18 17:32:51 2023, max compression
```

## Comparing `aicsshparam-0.1.6.tar` & `aicsshparam-0.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:56:19.413527 aicsshparam-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-18 02:56:19.413527 aicsshparam-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:56:19.409527 aicsshparam-0.1.6/aicsshparam/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/aicsshparam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:56:19.409527 aicsshparam-0.1.6/aicsshparam/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/aicsshparam/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/aicsshparam/shparam.py
--rw-r--r--   0 runner    (1001) docker     (123)    19075 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/aicsshparam/shtools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:56:19.409527 aicsshparam-0.1.6/aicsshparam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:56:19.413527 aicsshparam-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)   621959 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/logo.gif
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/pc12.png
--rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/table1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/table2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-18 02:56:19.413527 aicsshparam-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/aicsshparam/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/aicsshparam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/aicsshparam/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/aicsshparam/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/aicsshparam/shparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19075 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/aicsshparam/shtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/aicsshparam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 17:32:51.000000 aicsshparam-0.1.7/aicsshparam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   621959 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/logo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/pc12.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/table1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/docs/table2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 17:32:51.989806 aicsshparam-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-18 17:32:46.000000 aicsshparam-0.1.7/setup.py
```

### Comparing `aicsshparam-0.1.6/CONTRIBUTING.md` & `aicsshparam-0.1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/LICENSE` & `aicsshparam-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/PKG-INFO` & `aicsshparam-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicsshparam
-Version: 0.1.6
+Version: 0.1.7
 Summary: Spherical harmonics parametrization for 3D starlike shapes
 Home-page: https://github.com/AllenCell/aics-shparam
 Author: Matheus Viana
 Author-email: matheus.viana@alleninstitute.org
 License: Allen Institute Software License
 Keywords: aicsshparam
 Platform: UNKNOWN
@@ -18,28 +18,28 @@
 Description-Content-Type: text/markdown
 Provides-Extra: setup
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
-# AICS Spherical Hamonics Parametrization
+# AICS Spherical Harmonics Parametrization
 
 [![Build Status](https://github.com/AllenCell/aics-shparam/workflows/Build%20Main/badge.svg)](https://github.com/AllenCell/aics-shparam/actions)
 [![Documentation](https://github.com/AllenCell/aics-shparam/workflows/Documentation/badge.svg)](https://AllenCell.github.io/aics-shparam/)
 
-### Spherical harmonics parametrization for 3D starlike shapes. 
+### Spherical harmonics parametrization for 3D starlike shapes.
 
-![Parameterization of cell and nuclear shape](docs/logo.gif)
+![Parameterization of cell and nuclear shape](https://github.com/AllenCell/aics-shparam/blob/main/docs/logo.gif?raw=true)
 
 ## Installation:
 
 **Stable Release**: `pip install aicsshparam`
 
-**Build from source to make customization**: 
+**Build from source to make customization**:
 
 ```console
 git clone git@github.com:AllenCell/aics-shparam.git
 cd aics-shparam
 pip install -e .
 ```
 
@@ -56,15 +56,15 @@
 from aicsshparam import shtools, shparam
 from skimage.morphology import ball, cube, octahedron
 np.random.seed(42) # for reproducibility
 ```
 
 ```python
 # Function that returns binary images containing one of the three
-# shapes: cubes, spheres octahedrons of random sizes. 
+# shapes: cubes, spheres octahedrons of random sizes.
 def get_random_3d_shape():
     idx = np.random.choice([0, 1, 2], 1)[0]
     element = [ball, cube, octahedron][idx]
     label = ['ball', 'cube', 'octahedron'][idx]
     img = element(10 + int(10 * np.random.rand()))
     img = np.pad(img, ((1, 1), (1, 1), (1, 1)))
     img = img.reshape(1, *img.shape)
@@ -82,21 +82,21 @@
     # Get a random shape
     label, img = get_random_3d_shape()
     # Parameterize with L=4, which corresponds to50 coefficients
     # in total
     (coeffs, _), _ = shparam.get_shcoeffs(image=img, lmax=4)
     coeffs.update({'label': label})
     df_coeffs = df_coeffs.append(coeffs, ignore_index=True)
- 
+
 # Vizualize the resulting dataframe
 with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
     display(df_coeffs)
 ```
 
-![Coefficients dataframe](docs/table1.jpg)
+![Coefficients dataframe](https://github.com/AllenCell/aics-shparam/blob/main/docs/table1.jpg?raw=true)
 
 ```python
 # Let's use PCA to reduce the dimensionality of the coefficients
 # dataframe from 51 down to 2.
 pca = PCA(n_components=2)
 trans = pca.fit_transform(df_coeffs.drop(columns=['label']))
 df_trans = pd.DataFrame(trans)
@@ -104,38 +104,39 @@
 df_trans['label'] = df_coeffs.label
 
 # Vizualize the resulting dataframe
 with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
     display(df_trans)
 ```
 
-![PCA dataframe](docs/table2.jpg)
+![PCA dataframe](https://github.com/AllenCell/aics-shparam/blob/main/docs/table2.jpg?raw=true)
 
 ```python
 # Scatter plot to show how similar shapes are grouped together.
 fig, ax = plt.subplots(1,1, figsize=(3,3))
 for label, df_label in df_trans.groupby('label'):
     ax.scatter(df_label.PC1, df_label.PC2, label=label, s=50)
 plt.legend(loc='upper left', bbox_to_anchor=(1.05, 1))
 plt.xlabel('PC1')
 plt.ylabel('PC2')
 plt.show()
 ```
 
-![PC1 vs. PC2](docs/pc12.png)
+![PC1 vs. PC2](https://github.com/AllenCell/aics-shparam/blob/main/docs/pc12.png?raw=true)
 
 
 ## Reference
 
 For an example of how this package was used to analyse a dataset of over 200k single-cell images at the Allen Institute for Cell Science, please check out our paper in [bioaRxiv](https://www.biorxiv.org/content/10.1101/2020.12.08.415562v1).
 
 ## Development
 See [CONTRIBUTING.md](CONTRIBUTING.md) for information related to developing the code.
 
 
 ## Questions?
 
-If you have any questions, feel free to leave a comment in our Allen Cell forum: [https://forum.allencell.org/](https://forum.allencell.org/). 
+If you have any questions, feel free to leave a comment in our Allen Cell forum: [https://forum.allencell.org/](https://forum.allencell.org/).
+
 
+_Free software: Allen Institute Software License_
 
-***Free software: Allen Institute Software License***
```

### Comparing `aicsshparam-0.1.6/README.md` & `aicsshparam-0.1.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# AICS Spherical Hamonics Parametrization
+# AICS Spherical Harmonics Parametrization
 
 [![Build Status](https://github.com/AllenCell/aics-shparam/workflows/Build%20Main/badge.svg)](https://github.com/AllenCell/aics-shparam/actions)
 [![Documentation](https://github.com/AllenCell/aics-shparam/workflows/Documentation/badge.svg)](https://AllenCell.github.io/aics-shparam/)
 
-### Spherical harmonics parametrization for 3D starlike shapes. 
+### Spherical harmonics parametrization for 3D starlike shapes.
 
-![Parameterization of cell and nuclear shape](docs/logo.gif)
+![Parameterization of cell and nuclear shape](https://github.com/AllenCell/aics-shparam/blob/main/docs/logo.gif?raw=true)
 
 ## Installation:
 
 **Stable Release**: `pip install aicsshparam`
 
-**Build from source to make customization**: 
+**Build from source to make customization**:
 
 ```console
 git clone git@github.com:AllenCell/aics-shparam.git
 cd aics-shparam
 pip install -e .
 ```
 
@@ -32,15 +32,15 @@
 from aicsshparam import shtools, shparam
 from skimage.morphology import ball, cube, octahedron
 np.random.seed(42) # for reproducibility
 ```
 
 ```python
 # Function that returns binary images containing one of the three
-# shapes: cubes, spheres octahedrons of random sizes. 
+# shapes: cubes, spheres octahedrons of random sizes.
 def get_random_3d_shape():
     idx = np.random.choice([0, 1, 2], 1)[0]
     element = [ball, cube, octahedron][idx]
     label = ['ball', 'cube', 'octahedron'][idx]
     img = element(10 + int(10 * np.random.rand()))
     img = np.pad(img, ((1, 1), (1, 1), (1, 1)))
     img = img.reshape(1, *img.shape)
@@ -58,21 +58,21 @@
     # Get a random shape
     label, img = get_random_3d_shape()
     # Parameterize with L=4, which corresponds to50 coefficients
     # in total
     (coeffs, _), _ = shparam.get_shcoeffs(image=img, lmax=4)
     coeffs.update({'label': label})
     df_coeffs = df_coeffs.append(coeffs, ignore_index=True)
- 
+
 # Vizualize the resulting dataframe
 with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
     display(df_coeffs)
 ```
 
-![Coefficients dataframe](docs/table1.jpg)
+![Coefficients dataframe](https://github.com/AllenCell/aics-shparam/blob/main/docs/table1.jpg?raw=true)
 
 ```python
 # Let's use PCA to reduce the dimensionality of the coefficients
 # dataframe from 51 down to 2.
 pca = PCA(n_components=2)
 trans = pca.fit_transform(df_coeffs.drop(columns=['label']))
 df_trans = pd.DataFrame(trans)
@@ -80,37 +80,37 @@
 df_trans['label'] = df_coeffs.label
 
 # Vizualize the resulting dataframe
 with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
     display(df_trans)
 ```
 
-![PCA dataframe](docs/table2.jpg)
+![PCA dataframe](https://github.com/AllenCell/aics-shparam/blob/main/docs/table2.jpg?raw=true)
 
 ```python
 # Scatter plot to show how similar shapes are grouped together.
 fig, ax = plt.subplots(1,1, figsize=(3,3))
 for label, df_label in df_trans.groupby('label'):
     ax.scatter(df_label.PC1, df_label.PC2, label=label, s=50)
 plt.legend(loc='upper left', bbox_to_anchor=(1.05, 1))
 plt.xlabel('PC1')
 plt.ylabel('PC2')
 plt.show()
 ```
 
-![PC1 vs. PC2](docs/pc12.png)
+![PC1 vs. PC2](https://github.com/AllenCell/aics-shparam/blob/main/docs/pc12.png?raw=true)
 
 
 ## Reference
 
 For an example of how this package was used to analyse a dataset of over 200k single-cell images at the Allen Institute for Cell Science, please check out our paper in [bioaRxiv](https://www.biorxiv.org/content/10.1101/2020.12.08.415562v1).
 
 ## Development
 See [CONTRIBUTING.md](CONTRIBUTING.md) for information related to developing the code.
 
 
 ## Questions?
 
-If you have any questions, feel free to leave a comment in our Allen Cell forum: [https://forum.allencell.org/](https://forum.allencell.org/). 
+If you have any questions, feel free to leave a comment in our Allen Cell forum: [https://forum.allencell.org/](https://forum.allencell.org/).
 
 
-***Free software: Allen Institute Software License***
+_Free software: Allen Institute Software License_
```

### Comparing `aicsshparam-0.1.6/aicsshparam/shparam.py` & `aicsshparam-0.1.7/aicsshparam/shparam.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,94 +12,102 @@
     image: np.array,
     lmax: int,
     sigma: float = 0,
     compute_lcc: bool = True,
     alignment_2d: bool = True,
     make_unique: bool = False,
 ):
-    """Compute spherical harmonics coefficients that describe an object stored as
+    """
+    Compute spherical harmonics coefficients that describe an object stored as
     an image.
 
-        Calculates the spherical harmonics coefficients that parametrize the shape
-        formed by the foreground set of voxels in the input image. The input image
-        does not need to be binary and all foreground voxels (background=0) are used
-        in the computation. Foreground voxels must form a single connected component.
-        If you are sure that this is the case for the input image, you can set
-        compute_lcc to False to speed up the calculation. In addition, the shape is
-        expected to be centered in the input image.
-
-        Parameters
-        ----------
-        image : ndarray
-            Input image. Expected to have shape ZYX.
-        lmax : int
-            Order of the spherical harmonics parametrization. The higher the order
-            the more shape details are represented.
-        Returns
-        -------
-        coeffs_dict : dict
-            Dictionary with the spherical harmonics coefficients and the mean square
-            error between input and its parametrization
-        grid_rec : ndarray
-            Parametric grid representing sh parametrization
-        image_ : ndarray
-            Input image after pre-processing (lcc calculation, smooth and binarization).
-        mesh : vtkPolyData
-            Polydata representation of image_.
-        grid_down : ndarray
-            Parametric grid representing input object.
-        transform : tuple of floats
-            (xc, yc, zc, angle) if alignment_2d is True or
-            (xc, yc, zc) if alignment_2d is False. (xc, yc, zc) are the coordinates
-            of the shape centroid after alignment; angle is the angle used to align
-            the image
-
-        Other parameters
-        ----------------
-        sigma : float, optional
-            The degree of smooth to be applied to the input image, default is 0 (no
-            smooth)
-        compute_lcc : bool, optional
-            Whether to compute the largest connected component before appliying the
-            spherical harmonic parametrization, default is True. Set compute_lcc to
-            False in case you are sure the input image contains a single connected
-            component. It is crucial that parametrization is calculated on a single
-            connected component object.
-        alignment_2d : bool
-            Wheather the image should be aligned in 2d. Default is True.
-        make_unique : bool
-            Set true to make sure the alignment rotation is unique.
-
-        Notes
-        -----
-        Alignment mode '2d' allows for keeping the z axis unchanged which might be
-        important for some applications.
-
-        Examples
-        --------
-            import numpy as np
-            from aicsshparam import shparam, shtools
-
-            img = np.ones((32,32,32), dtype=np.uint8)
-
-            (coeffs, grid_rec), (image_, mesh, grid, transform) =
-                shparam.get_shcoeffs(image=img, lmax=2)
-            mse = shtools.get_reconstruction_error(grid, grid_rec)
+    Calculates the spherical harmonics coefficients that parametrize the shape
+    formed by the foreground set of voxels in the input image. The input image
+    does not need to be binary and all foreground voxels (background=0) are used
+    in the computation. Foreground voxels must form a single connected component.
+    If you are sure that this is the case for the input image, you can set
+    compute_lcc to False to speed up the calculation. In addition, the shape is
+    expected to be centered in the input image.
+
+    Parameters
+    ----------
+    image : ndarray
+        Input image. Expected to have shape ZYX.
+    lmax : int
+        Order of the spherical harmonics parametrization. The higher the order
+        the more shape details are represented.
+
+    Returns
+    -------
+    coeffs_dict : dict
+        Dictionary with the spherical harmonics coefficients and the mean square
+        error between input and its parametrization
+    grid_rec : ndarray
+        Parametric grid representing sh parametrization
+    image\\_ : ndarray
+        Input image after pre-processing (lcc calculation, smooth and binarization).
+    mesh : vtkPolyData
+        Polydata representation of image\\_.
+    grid_down : ndarray
+        Parametric grid representing input object.
+    transform : tuple of floats
+        (xc, yc, zc, angle) if alignment_2d is True or
+        (xc, yc, zc) if alignment_2d is False. (xc, yc, zc) are the coordinates
+        of the shape centroid after alignment; angle is the angle used to align
+        the image
+
+    Other parameters
+    ----------------
+    sigma : float, optional
+        The degree of smooth to be applied to the input image, default is 0 (no
+        smooth)
+    compute_lcc : bool, optional
+        Whether to compute the largest connected component before applying the
+        spherical harmonic parametrization, default is True. Set compute_lcc to
+        False in case you are sure the input image contains a single connected
+        component. It is crucial that parametrization is calculated on a single
+        connected component object.
+    alignment_2d : bool
+        Whether the image should be aligned in 2d. Default is True.
+    make_unique : bool
+        Set true to make sure the alignment rotation is unique.
+
+    Notes
+    -----
+    Alignment mode '2d' allows for keeping the z axis unchanged which might be
+    important for some applications.
+
+    Examples
+    --------
+
+    .. code-block:: python
+
+        import numpy as np
+        from aicsshparam import shparam, shtools
+
+        img = np.ones((32,32,32), dtype=np.uint8)
+
+        (coeffs, grid_rec), (image_, mesh, grid, transform) =
+            shparam.get_shcoeffs(image=img, lmax=2)
+        mse = shtools.get_reconstruction_error(grid, grid_rec)
+
+        print('Coefficients:', coeffs)
 
-            print('Coefficients:', coeffs)
         >>> Coefficients: {'shcoeffs_L0M0C': 18.31594310878251, 'shcoeffs_L0M1C': 0.0,
         'shcoeffs_L0M2C': 0.0, 'shcoeffs_L1M0C': 0.020438775421611564, 'shcoeffs_L1M1C':
         -0.0030960466571801513, 'shcoeffs_L1M2C': 0.0, 'shcoeffs_L2M0C':
         -0.0185688727281408, 'shcoeffs_L2M1C': -2.9925077712704384e-05,
         'shcoeffs_L2M2C': -0.009087503958673892, 'shcoeffs_L0M0S': 0.0,
         'shcoeffs_L0M1S': 0.0, 'shcoeffs_L0M2S': 0.0, 'shcoeffs_L1M0S': 0.0,
         'shcoeffs_L1M1S': 3.799611612562637e-05, 'shcoeffs_L1M2S': 0.0,
         'shcoeffs_L2M0S': 0.0, 'shcoeffs_L2M1S': 3.672543904347801e-07,
         'shcoeffs_L2M2S': 0.0002230857005948496}
-            print('Error:', mse)
+
+        print('Error:', mse)
+
         >>> Error: 2.3738182456948795
     """
 
     if len(image.shape) != 3:
         raise ValueError(
             "Incorrect dimensions: {}. Expected 3 dimensions.".format(image.shape)
         )
```

### Comparing `aicsshparam-0.1.6/aicsshparam/shtools.py` & `aicsshparam-0.1.7/aicsshparam/shtools.py`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/aicsshparam.egg-info/PKG-INFO` & `aicsshparam-0.1.7/aicsshparam.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicsshparam
-Version: 0.1.6
+Version: 0.1.7
 Summary: Spherical harmonics parametrization for 3D starlike shapes
 Home-page: https://github.com/AllenCell/aics-shparam
 Author: Matheus Viana
 Author-email: matheus.viana@alleninstitute.org
 License: Allen Institute Software License
 Keywords: aicsshparam
 Platform: UNKNOWN
@@ -18,28 +18,28 @@
 Description-Content-Type: text/markdown
 Provides-Extra: setup
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
-# AICS Spherical Hamonics Parametrization
+# AICS Spherical Harmonics Parametrization
 
 [![Build Status](https://github.com/AllenCell/aics-shparam/workflows/Build%20Main/badge.svg)](https://github.com/AllenCell/aics-shparam/actions)
 [![Documentation](https://github.com/AllenCell/aics-shparam/workflows/Documentation/badge.svg)](https://AllenCell.github.io/aics-shparam/)
 
-### Spherical harmonics parametrization for 3D starlike shapes. 
+### Spherical harmonics parametrization for 3D starlike shapes.
 
-![Parameterization of cell and nuclear shape](docs/logo.gif)
+![Parameterization of cell and nuclear shape](https://github.com/AllenCell/aics-shparam/blob/main/docs/logo.gif?raw=true)
 
 ## Installation:
 
 **Stable Release**: `pip install aicsshparam`
 
-**Build from source to make customization**: 
+**Build from source to make customization**:
 
 ```console
 git clone git@github.com:AllenCell/aics-shparam.git
 cd aics-shparam
 pip install -e .
 ```
 
@@ -56,15 +56,15 @@
 from aicsshparam import shtools, shparam
 from skimage.morphology import ball, cube, octahedron
 np.random.seed(42) # for reproducibility
 ```
 
 ```python
 # Function that returns binary images containing one of the three
-# shapes: cubes, spheres octahedrons of random sizes. 
+# shapes: cubes, spheres octahedrons of random sizes.
 def get_random_3d_shape():
     idx = np.random.choice([0, 1, 2], 1)[0]
     element = [ball, cube, octahedron][idx]
     label = ['ball', 'cube', 'octahedron'][idx]
     img = element(10 + int(10 * np.random.rand()))
     img = np.pad(img, ((1, 1), (1, 1), (1, 1)))
     img = img.reshape(1, *img.shape)
@@ -82,21 +82,21 @@
     # Get a random shape
     label, img = get_random_3d_shape()
     # Parameterize with L=4, which corresponds to50 coefficients
     # in total
     (coeffs, _), _ = shparam.get_shcoeffs(image=img, lmax=4)
     coeffs.update({'label': label})
     df_coeffs = df_coeffs.append(coeffs, ignore_index=True)
- 
+
 # Vizualize the resulting dataframe
 with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
     display(df_coeffs)
 ```
 
-![Coefficients dataframe](docs/table1.jpg)
+![Coefficients dataframe](https://github.com/AllenCell/aics-shparam/blob/main/docs/table1.jpg?raw=true)
 
 ```python
 # Let's use PCA to reduce the dimensionality of the coefficients
 # dataframe from 51 down to 2.
 pca = PCA(n_components=2)
 trans = pca.fit_transform(df_coeffs.drop(columns=['label']))
 df_trans = pd.DataFrame(trans)
@@ -104,38 +104,39 @@
 df_trans['label'] = df_coeffs.label
 
 # Vizualize the resulting dataframe
 with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
     display(df_trans)
 ```
 
-![PCA dataframe](docs/table2.jpg)
+![PCA dataframe](https://github.com/AllenCell/aics-shparam/blob/main/docs/table2.jpg?raw=true)
 
 ```python
 # Scatter plot to show how similar shapes are grouped together.
 fig, ax = plt.subplots(1,1, figsize=(3,3))
 for label, df_label in df_trans.groupby('label'):
     ax.scatter(df_label.PC1, df_label.PC2, label=label, s=50)
 plt.legend(loc='upper left', bbox_to_anchor=(1.05, 1))
 plt.xlabel('PC1')
 plt.ylabel('PC2')
 plt.show()
 ```
 
-![PC1 vs. PC2](docs/pc12.png)
+![PC1 vs. PC2](https://github.com/AllenCell/aics-shparam/blob/main/docs/pc12.png?raw=true)
 
 
 ## Reference
 
 For an example of how this package was used to analyse a dataset of over 200k single-cell images at the Allen Institute for Cell Science, please check out our paper in [bioaRxiv](https://www.biorxiv.org/content/10.1101/2020.12.08.415562v1).
 
 ## Development
 See [CONTRIBUTING.md](CONTRIBUTING.md) for information related to developing the code.
 
 
 ## Questions?
 
-If you have any questions, feel free to leave a comment in our Allen Cell forum: [https://forum.allencell.org/](https://forum.allencell.org/). 
+If you have any questions, feel free to leave a comment in our Allen Cell forum: [https://forum.allencell.org/](https://forum.allencell.org/).
+
 
+_Free software: Allen Institute Software License_
 
-***Free software: Allen Institute Software License***
```

### Comparing `aicsshparam-0.1.6/aicsshparam.egg-info/SOURCES.txt` & `aicsshparam-0.1.7/aicsshparam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/aicsshparam.egg-info/requires.txt` & `aicsshparam-0.1.7/aicsshparam.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 numpy>=1.18.1
 scipy>=1.4.1
 scikit-image>=0.16.2
 scikit-learn>=0.22.1
 vtk>=9.0.1
-pyshtools==4.9.1
+pyshtools>=4.9.1
 
 [all]
 numpy>=1.18.1
 scipy>=1.4.1
 scikit-image>=0.16.2
 scikit-learn>=0.22.1
 vtk>=9.0.1
-pyshtools==4.9.1
+pyshtools>=4.9.1
 pytest-runner>=5.2
 black>=22.10.0
 flake8>=3.8.3
 flake8-debugger>=3.2.1
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
 bump2version>=1.0.1
 coverage>=5.1
 ipython>=7.15.0
 m2r2>=0.2.7
 pytest-runner>=5.2
-Sphinx>=3.4.3
-sphinx_rtd_theme>=0.5.1
+sphinx>=7.0.1
+furo>=2023.5.20
 tox>=3.15.2
 twine>=3.1.1
 wheel>=0.34.2
 
 [dev]
 pytest-runner>=5.2
 black>=22.10.0
@@ -39,16 +39,16 @@
 pytest-cov>=2.9.0
 pytest-raises>=0.11
 bump2version>=1.0.1
 coverage>=5.1
 ipython>=7.15.0
 m2r2>=0.2.7
 pytest-runner>=5.2
-Sphinx>=3.4.3
-sphinx_rtd_theme>=0.5.1
+sphinx>=7.0.1
+furo>=2023.5.20
 tox>=3.15.2
 twine>=3.1.1
 wheel>=0.34.2
 
 [setup]
 pytest-runner>=5.2
```

### Comparing `aicsshparam-0.1.6/docs/Makefile` & `aicsshparam-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/docs/conf.py` & `aicsshparam-0.1.7/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
 
-import sphinx_rtd_theme
-
 import aicsshparam
 
 sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- General configuration ---------------------------------------------
 
@@ -83,15 +81,15 @@
 release = aicsshparam.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -102,29 +100,24 @@
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "sphinx_rtd_theme"
+html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
-#
-html_theme_options = {
-    "collapse_navigation": False,
-    "prev_next_buttons_location": "top",
-}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
+# html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "aicsshparamdoc"
```

### Comparing `aicsshparam-0.1.6/docs/installation.rst` & `aicsshparam-0.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/docs/logo.gif` & `aicsshparam-0.1.7/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/docs/make.bat` & `aicsshparam-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/docs/pc12.png` & `aicsshparam-0.1.7/docs/pc12.png`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/docs/table1.jpg` & `aicsshparam-0.1.7/docs/table1.jpg`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/docs/table2.jpg` & `aicsshparam-0.1.7/docs/table2.jpg`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.6/setup.py` & `aicsshparam-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,28 +26,28 @@
     *setup_requirements,
     *test_requirements,
     "bump2version>=1.0.1",
     "coverage>=5.1",
     "ipython>=7.15.0",
     "m2r2>=0.2.7",
     "pytest-runner>=5.2",
-    "Sphinx>=3.4.3",
-    "sphinx_rtd_theme>=0.5.1",
+    "sphinx>=7.0.1",
+    "furo>=2023.5.20",
     "tox>=3.15.2",
     "twine>=3.1.1",
     "wheel>=0.34.2",
 ]
 
 requirements = [
     'numpy>=1.18.1',
     'scipy>=1.4.1',
     'scikit-image>=0.16.2',
     'scikit-learn>=0.22.1',
     'vtk>=9.0.1',
-    'pyshtools==4.9.1'
+    'pyshtools>=4.9.1'
 ]
 
 extra_requirements = {
     "setup": setup_requirements,
     "test": test_requirements,
     "dev": dev_requirements,
     "all": [
@@ -80,10 +80,10 @@
     setup_requires=setup_requirements,
     test_suite="aicsshparam/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/AllenCell/aics-shparam",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="0.1.6",
+    version="0.1.7",
     zip_safe=False,
 )
```

