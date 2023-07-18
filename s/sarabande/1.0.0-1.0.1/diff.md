# Comparing `tmp/sarabande-1.0.0.tar.gz` & `tmp/sarabande-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarabande-1.0.0.tar", last modified: Mon Jun 19 01:13:40 2023, max compression
+gzip compressed data, was "sarabande-1.0.1.tar", last modified: Tue Jul 18 01:48:43 2023, max compression
```

## Comparing `sarabande-1.0.0.tar` & `sarabande-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-06-19 01:13:40.871656 sarabande-1.0.0/
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     1070 2023-06-17 09:16:47.000000 sarabande-1.0.0/LICENSE
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      106 2023-06-17 09:16:47.000000 sarabande-1.0.0/MANIFEST.in
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     5690 2023-06-19 01:13:40.871656 sarabande-1.0.0/PKG-INFO
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     4498 2023-06-19 01:00:32.000000 sarabande-1.0.0/README.md
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      116 2023-06-17 09:16:48.000000 sarabande-1.0.0/pyproject.toml
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)       12 2023-06-17 09:16:48.000000 sarabande-1.0.0/requirements.txt
-drwxr-xr-x   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-06-19 01:13:40.868656 sarabande-1.0.0/sarabande/
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)  2300096 2023-06-17 09:16:48.000000 sarabande-1.0.0/sarabande/CG_Coeffs.npy
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      151 2023-06-17 09:16:48.000000 sarabande-1.0.0/sarabande/__init__.py
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     3080 2023-06-17 09:16:48.000000 sarabande-1.0.0/sarabande/boot_up.py
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)    22727 2023-06-19 00:58:19.000000 sarabande-1.0.0/sarabande/calc_PCF.py
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     8432 2023-06-17 09:16:48.000000 sarabande-1.0.0/sarabande/main.py
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-06-18 14:41:44.000000 sarabande-1.0.0/sarabande/untitled.py
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)    17256 2023-06-17 09:16:48.000000 sarabande-1.0.0/sarabande/utils.py
-drwxr-xr-x   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-06-19 01:13:40.870656 sarabande-1.0.0/sarabande.egg-info/
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     5690 2023-06-19 01:13:40.000000 sarabande-1.0.0/sarabande.egg-info/PKG-INFO
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      360 2023-06-19 01:13:40.000000 sarabande-1.0.0/sarabande.egg-info/SOURCES.txt
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)        1 2023-06-19 01:13:40.000000 sarabande-1.0.0/sarabande.egg-info/dependency_links.txt
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)       10 2023-06-19 01:13:40.000000 sarabande-1.0.0/sarabande.egg-info/top_level.txt
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)       98 2023-06-19 01:13:40.872656 sarabande-1.0.0/setup.cfg
--rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     2219 2023-06-19 01:00:35.000000 sarabande-1.0.0/setup.py
+drwxr-xr-x   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-07-18 01:48:43.441289 sarabande-1.0.1/
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     1070 2023-07-02 07:36:33.000000 sarabande-1.0.1/LICENSE
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      106 2023-07-02 07:36:33.000000 sarabande-1.0.1/MANIFEST.in
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     6289 2023-07-18 01:48:43.441289 sarabande-1.0.1/PKG-INFO
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     4498 2023-07-02 07:36:33.000000 sarabande-1.0.1/README.md
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      116 2023-07-02 07:36:33.000000 sarabande-1.0.1/pyproject.toml
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)       12 2023-07-02 07:36:33.000000 sarabande-1.0.1/requirements.txt
+drwxr-xr-x   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-07-18 01:48:43.438289 sarabande-1.0.1/sarabande/
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)  2300096 2023-07-02 07:36:33.000000 sarabande-1.0.1/sarabande/CG_Coeffs.npy
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      151 2023-07-02 07:36:33.000000 sarabande-1.0.1/sarabande/__init__.py
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     3080 2023-07-02 07:36:33.000000 sarabande-1.0.1/sarabande/boot_up.py
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)    22730 2023-07-02 08:15:45.000000 sarabande-1.0.1/sarabande/calc_PCF.py
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     8432 2023-07-02 07:36:33.000000 sarabande-1.0.1/sarabande/main.py
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-07-02 07:36:33.000000 sarabande-1.0.1/sarabande/untitled.py
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)    17256 2023-07-02 07:36:33.000000 sarabande-1.0.1/sarabande/utils.py
+drwxr-xr-x   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-07-18 01:48:43.440289 sarabande-1.0.1/sarabande.egg-info/
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     6289 2023-07-18 01:48:43.000000 sarabande-1.0.1/sarabande.egg-info/PKG-INFO
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      360 2023-07-18 01:48:43.000000 sarabande-1.0.1/sarabande.egg-info/SOURCES.txt
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)        1 2023-07-18 01:48:43.000000 sarabande-1.0.1/sarabande.egg-info/dependency_links.txt
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)       10 2023-07-18 01:48:43.000000 sarabande-1.0.1/sarabande.egg-info/top_level.txt
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)       98 2023-07-18 01:48:43.442289 sarabande-1.0.1/setup.cfg
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     2219 2023-07-02 08:14:05.000000 sarabande-1.0.1/setup.py
```

### Comparing `sarabande-1.0.0/LICENSE` & `sarabande-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sarabande-1.0.0/PKG-INFO` & `sarabande-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,96 @@
 Metadata-Version: 2.1
 Name: sarabande
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tool for measuring 3/4 PCFs on discrete periodic data.
 Home-page: https://github.com/James11222/sarabande/
 Author: James Sunseri
 Author-email: jamessunseri@berkeley.edu
 License: MIT
 Project-URL: Bug Reports, https://github.com/James11222/sarabande/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Check out my Website!, http://www.jamessunseri.com
 Project-URL: Source, https://github.com/James11222/sarabande/
+Description: [![codecov](https://codecov.io/gh/James11222/sarabande/branch/main/graph/badge.svg?token=47GPJCFZLE)](https://codecov.io/gh/James11222/sarabande) 
+        ![PyPI](https://img.shields.io/pypi/v/sarabande?color=blue%20&label=PyPi%20)
+        
+        <p align="center">
+          <img src="logo/logo_text_dm.png#gh-dark-mode-only" width="100%">
+          <img src="logo/logo_text.png#gh-light-mode-only" width="100%">
+        </p>
+        
+        A useful `python` package to measure the 3/4 PCFs of discrete periodic data in NlogN time. This is done using Fast Fourier Transforms. 
+        
+        
+        ## Installation: 
+        The package is available on PyPi via the command `pip install sarabande`. To check if the code is working properly after pip installation, run 
+        
+        ```python
+        import sarabande
+        
+        sarabande.check_install()
+        ```
+        which will display a message stating if the package was properly installed.
+        
+        ## Basic Usage:
+        
+        ```python
+        import sarabande
+        
+        NPCF_obj = sarabande.measure(**kwargs)
+        sarabande.calc_zeta(NPCF_obj)
+        zeta = NPCF_obj.zeta
+        ```
+        
+        Where `**kwargs` can be any of the arguments to the measure constructor function. The possible arguments are:
+        
+        `Args:`
+        
+        * `nPCF` ([`int`]): Must be either 3 or 4. Determines how many points we use in our nPCF.
+        * `projected` ([`bool`]): Flag to determine whether the user wants a projected 3/4 PCF or the Full. Defaults to False.
+            - if `projected`:
+                - `m_max` ([`int`]): If user chooses projected, we set an m_max (similar to the `ell_max` in 3D)
+            - if not `projected`:
+                - `ell_max` ([`int`]): If user choosees not projected (full nPCF) then ell_max is the highest order for calculation.
+        
+        * `density_field_data` ([`ndarray`]): A square ndarray of data that is periodic. Must be 2D for projected and 3D for full.
+        * `save_dir` ([`string`]): A string to tell the algorithm where to save and store files. All temporary files will be stored here.
+        * `save_name` ([`string`]): A string to tell the algorithm what to name the files.
+        * `nbins` ([`int`]): Number of bins to be used in nPCF calculation.
+        * `bin_spacing` ([`string`]): A string to determine the spacing of bins. Options are `'LIN'`, `'INV'`, or `'LOG'`
+        * `bin_min` ([`int`]): The lower bound of the inner most bin. Default is 1. Optional.
+        * `physical_boxsize` ([`float`]): An optional parameter if using a physical scale. The length of one side of the data.
+        * `rmin` ([`float`]): minimum calculation distance (determins `bin_min`)
+        * `rmax` ([`float`]): maximum calculation distance (determins `bin_max`)
+        * `normalize` ([`bool`]): A boolean flag to normalize the 3/4 PCFs. Defaults to True. Can't use normalize without giving a `physical_boxsize`, `rmin`, and `rmax` first.
+        * `particles_on_grid` ([`bool`]): An optional boolean flag to modify the normalization scheme slightly. This is recommended if you are working with particles on the grid mesh where a given cell corresponds to a particle. 
+        
+        We note that the `calc_zeta` method has an optional boolean argument `verbose_flag` which can be turned on and off depending on if the user wants to see the steps of the code printed. We also add an optional boolean argument `parallelized` which can be turned on and off if the user wishes to compute the Full 4PCF serially. This is added due to the instability of `concurrent.futures` and parallel processing in python across different machines. 
+        
+        We also provide an implementation of the connected 4PCF, this will be further documented in a future paper.
+        
+        For an example, please visit the demo notebook in the analysis notebooks folder: `notebooks/Application_Example.ipynb`
+        
+         ## Workflow:    
+        The map of SARABANDE is as follows:
+        
+        <p align="center">
+          <img src="notebooks/paper_figures/workflow_dm.png#gh-dark-mode-only" width="100%">
+          <img src="notebooks/paper_figures/workflow.png#gh-light-mode-only" width="100%">
+        </p>
+        
+        For more information about each algorithm, please read [Sunseri et al. 2022](https://ui.adsabs.harvard.edu/abs/2022arXiv221010206S/abstract)
+        
+        ## Coverage [![codecov](https://codecov.io/gh/James11222/sarabande/branch/main/graph/badge.svg?token=47GPJCFZLE)](https://codecov.io/gh/James11222/sarabande) 
+        We provide a sunburst plot of the code coverage for sarabande below provided by codecov.io. The inner-most circle is the entire project, moving away from the center are folders then, finally, a single file. The size and color of each slice is representing the number of statements and the coverage, respectively.
+        
+        <p align="center">
+          <img src="https://codecov.io/gh/James11222/sarabande/branch/main/graphs/sunburst.svg?token=47GPJCFZLE">
+        </p>
+        
 Keywords: npcf,3pcf,4pcf,cosmology,hydrodynamics
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,85 +98,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![codecov](https://codecov.io/gh/James11222/sarabande/branch/main/graph/badge.svg?token=47GPJCFZLE)](https://codecov.io/gh/James11222/sarabande) 
-![PyPI](https://img.shields.io/pypi/v/sarabande?color=blue%20&label=PyPi%20)
-
-<p align="center">
-  <img src="logo/logo_text_dm.png#gh-dark-mode-only" width="100%">
-  <img src="logo/logo_text.png#gh-light-mode-only" width="100%">
-</p>
-
-A useful `python` package to measure the 3/4 PCFs of discrete periodic data in NlogN time. This is done using Fast Fourier Transforms. 
-
-
-## Installation: 
-The package is available on PyPi via the command `pip install sarabande`. To check if the code is working properly after pip installation, run 
-
-```python
-import sarabande
-
-sarabande.check_install()
-```
-which will display a message stating if the package was properly installed.
-
-## Basic Usage:
-
-```python
-import sarabande
-
-NPCF_obj = sarabande.measure(**kwargs)
-sarabande.calc_zeta(NPCF_obj)
-zeta = NPCF_obj.zeta
-```
-
-Where `**kwargs` can be any of the arguments to the measure constructor function. The possible arguments are:
-
-`Args:`
-
-* `nPCF` ([`int`]): Must be either 3 or 4. Determines how many points we use in our nPCF.
-* `projected` ([`bool`]): Flag to determine whether the user wants a projected 3/4 PCF or the Full. Defaults to False.
-    - if `projected`:
-        - `m_max` ([`int`]): If user chooses projected, we set an m_max (similar to the `ell_max` in 3D)
-    - if not `projected`:
-        - `ell_max` ([`int`]): If user choosees not projected (full nPCF) then ell_max is the highest order for calculation.
-
-* `density_field_data` ([`ndarray`]): A square ndarray of data that is periodic. Must be 2D for projected and 3D for full.
-* `save_dir` ([`string`]): A string to tell the algorithm where to save and store files. All temporary files will be stored here.
-* `save_name` ([`string`]): A string to tell the algorithm what to name the files.
-* `nbins` ([`int`]): Number of bins to be used in nPCF calculation.
-* `bin_spacing` ([`string`]): A string to determine the spacing of bins. Options are `'LIN'`, `'INV'`, or `'LOG'`
-* `bin_min` ([`int`]): The lower bound of the inner most bin. Default is 1. Optional.
-* `physical_boxsize` ([`float`]): An optional parameter if using a physical scale. The length of one side of the data.
-* `rmin` ([`float`]): minimum calculation distance (determins `bin_min`)
-* `rmax` ([`float`]): maximum calculation distance (determins `bin_max`)
-* `normalize` ([`bool`]): A boolean flag to normalize the 3/4 PCFs. Defaults to True. Can't use normalize without giving a `physical_boxsize`, `rmin`, and `rmax` first.
-* `particles_on_grid` ([`bool`]): An optional boolean flag to modify the normalization scheme slightly. This is recommended if you are working with particles on the grid mesh where a given cell corresponds to a particle. 
-
-We note that the `calc_zeta` method has an optional boolean argument `verbose_flag` which can be turned on and off depending on if the user wants to see the steps of the code printed. We also add an optional boolean argument `parallelized` which can be turned on and off if the user wishes to compute the Full 4PCF serially. This is added due to the instability of `concurrent.futures` and parallel processing in python across different machines. 
-
-We also provide an implementation of the connected 4PCF, this will be further documented in a future paper.
-
-For an example, please visit the demo notebook in the analysis notebooks folder: `notebooks/Application_Example.ipynb`
-
- ## Workflow:    
-The map of SARABANDE is as follows:
-
-<p align="center">
-  <img src="notebooks/paper_figures/workflow_dm.png#gh-dark-mode-only" width="100%">
-  <img src="notebooks/paper_figures/workflow.png#gh-light-mode-only" width="100%">
-</p>
-
-For more information about each algorithm, please read [Sunseri et al. 2022](https://ui.adsabs.harvard.edu/abs/2022arXiv221010206S/abstract)
-
-## Coverage [![codecov](https://codecov.io/gh/James11222/sarabande/branch/main/graph/badge.svg?token=47GPJCFZLE)](https://codecov.io/gh/James11222/sarabande) 
-We provide a sunburst plot of the code coverage for sarabande below provided by codecov.io. The inner-most circle is the entire project, moving away from the center are folders then, finally, a single file. The size and color of each slice is representing the number of statements and the coverage, respectively.
-
-<p align="center">
-  <img src="https://codecov.io/gh/James11222/sarabande/branch/main/graphs/sunburst.svg?token=47GPJCFZLE">
-</p>
```

### Comparing `sarabande-1.0.0/README.md` & `sarabande-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sarabande-1.0.0/sarabande/CG_Coeffs.npy` & `sarabande-1.0.1/sarabande/CG_Coeffs.npy`

 * *Files identical despite different names*

### Comparing `sarabande-1.0.0/sarabande/boot_up.py` & `sarabande-1.0.1/sarabande/boot_up.py`

 * *Files identical despite different names*

### Comparing `sarabande-1.0.0/sarabande/calc_PCF.py` & `sarabande-1.0.1/sarabande/calc_PCF.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
                     disconnected_piece = 2 * S(m_3) * coupling_phase * (np.sum(measure_obj.density_field_data * a_lmb_1.conjugate()) * np.sum(a_lmb_2.conjugate() * a_lmb_3.conjugate())
                                                                       + np.sum(measure_obj.density_field_data * a_lmb_2.conjugate()) * np.sum(a_lmb_3.conjugate() * a_lmb_1.conjugate()) 
                                                                       + np.sum(measure_obj.density_field_data * a_lmb_3.conjugate()) * np.sum(a_lmb_1.conjugate() * a_lmb_2.conjugate()))
                 else:
                     disconnected_piece = 0
                     
 
-                if calc_odd_modes == True and (l1 + l2 + l3)%2 != 0:
+                if calc_odd_modes == True and (l_1 + l_2 + l_3)%2 != 0:
                     full_piece = 2 * S(m_3) * coupling_phase * np.sum(measure_obj.density_field_data * np.imag(a_lmb_1 * a_lmb_2 * a_lmb_3))
                     disconnected_piece = np.imag(disconnected_piece)
                 else:
                     full_piece = 2 * S(m_3) * coupling_phase * np.sum(measure_obj.density_field_data * np.real(a_lmb_1 * a_lmb_2 * a_lmb_3))
                     disconnected_piece = np.real(disconnected_piece)
```

### Comparing `sarabande-1.0.0/sarabande/main.py` & `sarabande-1.0.1/sarabande/main.py`

 * *Files identical despite different names*

### Comparing `sarabande-1.0.0/sarabande/utils.py` & `sarabande-1.0.1/sarabande/utils.py`

 * *Files identical despite different names*

### Comparing `sarabande-1.0.0/sarabande.egg-info/PKG-INFO` & `sarabande-1.0.1/sarabande.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,96 @@
 Metadata-Version: 2.1
 Name: sarabande
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tool for measuring 3/4 PCFs on discrete periodic data.
 Home-page: https://github.com/James11222/sarabande/
 Author: James Sunseri
 Author-email: jamessunseri@berkeley.edu
 License: MIT
 Project-URL: Bug Reports, https://github.com/James11222/sarabande/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Check out my Website!, http://www.jamessunseri.com
 Project-URL: Source, https://github.com/James11222/sarabande/
+Description: [![codecov](https://codecov.io/gh/James11222/sarabande/branch/main/graph/badge.svg?token=47GPJCFZLE)](https://codecov.io/gh/James11222/sarabande) 
+        ![PyPI](https://img.shields.io/pypi/v/sarabande?color=blue%20&label=PyPi%20)
+        
+        <p align="center">
+          <img src="logo/logo_text_dm.png#gh-dark-mode-only" width="100%">
+          <img src="logo/logo_text.png#gh-light-mode-only" width="100%">
+        </p>
+        
+        A useful `python` package to measure the 3/4 PCFs of discrete periodic data in NlogN time. This is done using Fast Fourier Transforms. 
+        
+        
+        ## Installation: 
+        The package is available on PyPi via the command `pip install sarabande`. To check if the code is working properly after pip installation, run 
+        
+        ```python
+        import sarabande
+        
+        sarabande.check_install()
+        ```
+        which will display a message stating if the package was properly installed.
+        
+        ## Basic Usage:
+        
+        ```python
+        import sarabande
+        
+        NPCF_obj = sarabande.measure(**kwargs)
+        sarabande.calc_zeta(NPCF_obj)
+        zeta = NPCF_obj.zeta
+        ```
+        
+        Where `**kwargs` can be any of the arguments to the measure constructor function. The possible arguments are:
+        
+        `Args:`
+        
+        * `nPCF` ([`int`]): Must be either 3 or 4. Determines how many points we use in our nPCF.
+        * `projected` ([`bool`]): Flag to determine whether the user wants a projected 3/4 PCF or the Full. Defaults to False.
+            - if `projected`:
+                - `m_max` ([`int`]): If user chooses projected, we set an m_max (similar to the `ell_max` in 3D)
+            - if not `projected`:
+                - `ell_max` ([`int`]): If user choosees not projected (full nPCF) then ell_max is the highest order for calculation.
+        
+        * `density_field_data` ([`ndarray`]): A square ndarray of data that is periodic. Must be 2D for projected and 3D for full.
+        * `save_dir` ([`string`]): A string to tell the algorithm where to save and store files. All temporary files will be stored here.
+        * `save_name` ([`string`]): A string to tell the algorithm what to name the files.
+        * `nbins` ([`int`]): Number of bins to be used in nPCF calculation.
+        * `bin_spacing` ([`string`]): A string to determine the spacing of bins. Options are `'LIN'`, `'INV'`, or `'LOG'`
+        * `bin_min` ([`int`]): The lower bound of the inner most bin. Default is 1. Optional.
+        * `physical_boxsize` ([`float`]): An optional parameter if using a physical scale. The length of one side of the data.
+        * `rmin` ([`float`]): minimum calculation distance (determins `bin_min`)
+        * `rmax` ([`float`]): maximum calculation distance (determins `bin_max`)
+        * `normalize` ([`bool`]): A boolean flag to normalize the 3/4 PCFs. Defaults to True. Can't use normalize without giving a `physical_boxsize`, `rmin`, and `rmax` first.
+        * `particles_on_grid` ([`bool`]): An optional boolean flag to modify the normalization scheme slightly. This is recommended if you are working with particles on the grid mesh where a given cell corresponds to a particle. 
+        
+        We note that the `calc_zeta` method has an optional boolean argument `verbose_flag` which can be turned on and off depending on if the user wants to see the steps of the code printed. We also add an optional boolean argument `parallelized` which can be turned on and off if the user wishes to compute the Full 4PCF serially. This is added due to the instability of `concurrent.futures` and parallel processing in python across different machines. 
+        
+        We also provide an implementation of the connected 4PCF, this will be further documented in a future paper.
+        
+        For an example, please visit the demo notebook in the analysis notebooks folder: `notebooks/Application_Example.ipynb`
+        
+         ## Workflow:    
+        The map of SARABANDE is as follows:
+        
+        <p align="center">
+          <img src="notebooks/paper_figures/workflow_dm.png#gh-dark-mode-only" width="100%">
+          <img src="notebooks/paper_figures/workflow.png#gh-light-mode-only" width="100%">
+        </p>
+        
+        For more information about each algorithm, please read [Sunseri et al. 2022](https://ui.adsabs.harvard.edu/abs/2022arXiv221010206S/abstract)
+        
+        ## Coverage [![codecov](https://codecov.io/gh/James11222/sarabande/branch/main/graph/badge.svg?token=47GPJCFZLE)](https://codecov.io/gh/James11222/sarabande) 
+        We provide a sunburst plot of the code coverage for sarabande below provided by codecov.io. The inner-most circle is the entire project, moving away from the center are folders then, finally, a single file. The size and color of each slice is representing the number of statements and the coverage, respectively.
+        
+        <p align="center">
+          <img src="https://codecov.io/gh/James11222/sarabande/branch/main/graphs/sunburst.svg?token=47GPJCFZLE">
+        </p>
+        
 Keywords: npcf,3pcf,4pcf,cosmology,hydrodynamics
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,85 +98,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![codecov](https://codecov.io/gh/James11222/sarabande/branch/main/graph/badge.svg?token=47GPJCFZLE)](https://codecov.io/gh/James11222/sarabande) 
-![PyPI](https://img.shields.io/pypi/v/sarabande?color=blue%20&label=PyPi%20)
-
-<p align="center">
-  <img src="logo/logo_text_dm.png#gh-dark-mode-only" width="100%">
-  <img src="logo/logo_text.png#gh-light-mode-only" width="100%">
-</p>
-
-A useful `python` package to measure the 3/4 PCFs of discrete periodic data in NlogN time. This is done using Fast Fourier Transforms. 
-
-
-## Installation: 
-The package is available on PyPi via the command `pip install sarabande`. To check if the code is working properly after pip installation, run 
-
-```python
-import sarabande
-
-sarabande.check_install()
-```
-which will display a message stating if the package was properly installed.
-
-## Basic Usage:
-
-```python
-import sarabande
-
-NPCF_obj = sarabande.measure(**kwargs)
-sarabande.calc_zeta(NPCF_obj)
-zeta = NPCF_obj.zeta
-```
-
-Where `**kwargs` can be any of the arguments to the measure constructor function. The possible arguments are:
-
-`Args:`
-
-* `nPCF` ([`int`]): Must be either 3 or 4. Determines how many points we use in our nPCF.
-* `projected` ([`bool`]): Flag to determine whether the user wants a projected 3/4 PCF or the Full. Defaults to False.
-    - if `projected`:
-        - `m_max` ([`int`]): If user chooses projected, we set an m_max (similar to the `ell_max` in 3D)
-    - if not `projected`:
-        - `ell_max` ([`int`]): If user choosees not projected (full nPCF) then ell_max is the highest order for calculation.
-
-* `density_field_data` ([`ndarray`]): A square ndarray of data that is periodic. Must be 2D for projected and 3D for full.
-* `save_dir` ([`string`]): A string to tell the algorithm where to save and store files. All temporary files will be stored here.
-* `save_name` ([`string`]): A string to tell the algorithm what to name the files.
-* `nbins` ([`int`]): Number of bins to be used in nPCF calculation.
-* `bin_spacing` ([`string`]): A string to determine the spacing of bins. Options are `'LIN'`, `'INV'`, or `'LOG'`
-* `bin_min` ([`int`]): The lower bound of the inner most bin. Default is 1. Optional.
-* `physical_boxsize` ([`float`]): An optional parameter if using a physical scale. The length of one side of the data.
-* `rmin` ([`float`]): minimum calculation distance (determins `bin_min`)
-* `rmax` ([`float`]): maximum calculation distance (determins `bin_max`)
-* `normalize` ([`bool`]): A boolean flag to normalize the 3/4 PCFs. Defaults to True. Can't use normalize without giving a `physical_boxsize`, `rmin`, and `rmax` first.
-* `particles_on_grid` ([`bool`]): An optional boolean flag to modify the normalization scheme slightly. This is recommended if you are working with particles on the grid mesh where a given cell corresponds to a particle. 
-
-We note that the `calc_zeta` method has an optional boolean argument `verbose_flag` which can be turned on and off depending on if the user wants to see the steps of the code printed. We also add an optional boolean argument `parallelized` which can be turned on and off if the user wishes to compute the Full 4PCF serially. This is added due to the instability of `concurrent.futures` and parallel processing in python across different machines. 
-
-We also provide an implementation of the connected 4PCF, this will be further documented in a future paper.
-
-For an example, please visit the demo notebook in the analysis notebooks folder: `notebooks/Application_Example.ipynb`
-
- ## Workflow:    
-The map of SARABANDE is as follows:
-
-<p align="center">
-  <img src="notebooks/paper_figures/workflow_dm.png#gh-dark-mode-only" width="100%">
-  <img src="notebooks/paper_figures/workflow.png#gh-light-mode-only" width="100%">
-</p>
-
-For more information about each algorithm, please read [Sunseri et al. 2022](https://ui.adsabs.harvard.edu/abs/2022arXiv221010206S/abstract)
-
-## Coverage [![codecov](https://codecov.io/gh/James11222/sarabande/branch/main/graph/badge.svg?token=47GPJCFZLE)](https://codecov.io/gh/James11222/sarabande) 
-We provide a sunburst plot of the code coverage for sarabande below provided by codecov.io. The inner-most circle is the entire project, moving away from the center are folders then, finally, a single file. The size and color of each slice is representing the number of statements and the coverage, respectively.
-
-<p align="center">
-  <img src="https://codecov.io/gh/James11222/sarabande/branch/main/graphs/sunburst.svg?token=47GPJCFZLE">
-</p>
```

### Comparing `sarabande-1.0.0/setup.py` & `sarabande-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name='sarabande',  # Required
-    version='1.0.0',  # Required
+    version='1.0.1',  # Required
     description='Tool for measuring 3/4 PCFs on discrete periodic data.',  # Optional
     long_description=(here / 'README.md').read_text(encoding='utf-8'),  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/James11222/sarabande/',  # Optional
 
     author='James Sunseri',  # Optional
```

