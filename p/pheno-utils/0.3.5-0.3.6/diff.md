# Comparing `tmp/pheno-utils-0.3.5.tar.gz` & `tmp/pheno-utils-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.5.tar", last modified: Thu Jul 13 10:33:06 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.6.tar", last modified: Tue Jul 18 11:25:53 2023, max compression
```

## Comparing `pheno-utils-0.3.5.tar` & `pheno-utils-0.3.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:33:05.999109 pheno-utils-0.3.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-13 10:33:05.997610 pheno-utils-0.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-13 10:31:33.000000 pheno-utils-0.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:33:05.952057 pheno-utils-0.3.5/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17797 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16963 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5322 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    19901 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)    13210 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:33:05.990569 pheno-utils-0.3.5/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.5/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      143 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      961 2023-07-13 10:28:37.000000 pheno-utils-0.3.5/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 10:33:05.999719 pheno-utils-0.3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2560 2023-06-21 16:13:16.000000 pheno-utils-0.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:25:53.637899 pheno-utils-0.3.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-07-18 11:25:53.636137 pheno-utils-0.3.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-13 10:31:33.000000 pheno-utils-0.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:25:53.586105 pheno-utils-0.3.6/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17749 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16402 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    19976 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-07-18 11:24:27.000000 pheno-utils-0.3.6/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:25:53.624369 pheno-utils-0.3.6/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.6/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-18 11:25:53.000000 pheno-utils-0.3.6/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      942 2023-07-18 11:24:00.000000 pheno-utils-0.3.6/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 11:25:53.638702 pheno-utils-0.3.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-06-21 16:13:16.000000 pheno-utils-0.3.6/setup.py
```

### Comparing `pheno-utils-0.3.5/LICENSE` & `pheno-utils-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/PKG-INFO` & `pheno-utils-0.3.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.5
+Version: 0.3.6
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
-Author: hrossman
-Author-email: hagairossman@gmail.com
+Author: pheno.ai
+Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pheno-utils-0.3.5/README.md` & `pheno-utils-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/pheno_utils/_modidx.py` & `pheno-utils-0.3.6/pheno_utils/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
                 'lib_path': 'pheno_utils'},
   'syms': { 'pheno_utils.age_reference_plots': { 'pheno_utils.age_reference_plots.AgeRefPlot': ( 'age_reference_plots.html#agerefplot',
                                                                                                  'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.AgeRefPlot.__init__': ( 'age_reference_plots.html#agerefplot.__init__',
                                                                                                           'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.AgeRefPlot.calc_linear_fit': ( 'age_reference_plots.html#agerefplot.calc_linear_fit',
                                                                                                                  'pheno_utils/age_reference_plots.py'),
-                                                 'pheno_utils.age_reference_plots.AgeRefPlot.calc_smooth_percentiles': ( 'age_reference_plots.html#agerefplot.calc_smooth_percentiles',
-                                                                                                                         'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.AgeRefPlot.plot': ( 'age_reference_plots.html#agerefplot.plot',
                                                                                                       'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.AgeRefPlot.plot_agehist': ( 'age_reference_plots.html#agerefplot.plot_agehist',
                                                                                                               'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.AgeRefPlot.plot_ornaments': ( 'age_reference_plots.html#agerefplot.plot_ornaments',
                                                                                                                 'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.AgeRefPlot.plot_percentiles': ( 'age_reference_plots.html#agerefplot.plot_percentiles',
@@ -26,15 +24,17 @@
                                                  'pheno_utils.age_reference_plots.AgeRefPlot.plot_valhist': ( 'age_reference_plots.html#agerefplot.plot_valhist',
                                                                                                               'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.GenderAgeRefPlot': ( 'age_reference_plots.html#genderagerefplot',
                                                                                                        'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.GenderAgeRefPlot.__init__': ( 'age_reference_plots.html#genderagerefplot.__init__',
                                                                                                                 'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.GenderAgeRefPlot.plot': ( 'age_reference_plots.html#genderagerefplot.plot',
-                                                                                                            'pheno_utils/age_reference_plots.py')},
+                                                                                                            'pheno_utils/age_reference_plots.py'),
+                                                 'pheno_utils.age_reference_plots.get_gam_expectiles': ( 'age_reference_plots.html#get_gam_expectiles',
+                                                                                                         'pheno_utils/age_reference_plots.py')},
             'pheno_utils.basic_analysis': { 'pheno_utils.basic_analysis.assign_nearest_research_stage': ( 'basic_analysis.html#assign_nearest_research_stage',
                                                                                                           'pheno_utils/basic_analysis.py'),
                                             'pheno_utils.basic_analysis.custom_describe': ( 'basic_analysis.html#custom_describe',
                                                                                             'pheno_utils/basic_analysis.py')},
             'pheno_utils.basic_plots': { 'pheno_utils.basic_plots.hist_ecdf_plots': ( 'basic_plots.html#hist_ecdf_plots',
                                                                                       'pheno_utils/basic_plots.py'),
                                          'pheno_utils.basic_plots.show_fundus': ( 'basic_plots.html#show_fundus',
```

### Comparing `pheno-utils-0.3.5/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.6/pheno_utils/age_reference_plots.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,67 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_age_reference_plots.ipynb.
 
 # %% auto 0
-__all__ = ['AgeRefPlot', 'GenderAgeRefPlot']
+__all__ = ['get_gam_expectiles', 'AgeRefPlot', 'GenderAgeRefPlot']
 
 # %% ../nbs/03_age_reference_plots.ipynb 3
 from .config import *
 
-from typing import Dict, List, Callable, Optional, Union
+from typing import Dict, List, Callable, Optional, Union, Tuple
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import importlib
 from scipy.stats import linregress
 from sklearn.linear_model import HuberRegressor
+from numpy import ndarray
+
 
 # %% ../nbs/03_age_reference_plots.ipynb 4
 try:
-    importlib.import_module("tsmoothie")
+    importlib.import_module("pygam")
 except ImportError:
-    raise ImportError("The 'tsmoothie' library is not installed. Please install it using 'pip install tsmoothie' before running this script.")
+    raise ImportError("The 'pygam' library is not installed. Please install it using 'pip install pygam' before running this script.")
 
-from tsmoothie.smoother import SplineSmoother, LowessSmoother
+from pygam import ExpectileGAM
 
 # %% ../nbs/03_age_reference_plots.ipynb 5
+def get_gam_expectiles(X: ndarray, y: ndarray, expectiles: List[float] = [0.03, 0.1, 0.5, 0.9, 0.97]) -> Tuple[ndarray, Dict[str, ndarray]]:
+    """
+    Fit Expectile Generalized Additive Models (GAMs) for given expectiles.
+
+    Args:
+        X (ndarray): Feature data for the model.
+        y (ndarray): Target variable for the model.
+        expectiles (List[float]): List of expectiles to fit. Default is [0.03, 0.1, 0.5, 0.9, 0.97].
+
+    Returns:
+        Tuple[ndarray, Dict[str, ndarray]]: A tuple containing a grid of X values for prediction and a dictionary with expectiles as keys and their corresponding model predictions as values.
+    """
+
+    # Fit the median model first by Cross-Validation
+    gam50 = ExpectileGAM(expectile=0.5).gridsearch(X, y, progress=False)
+
+    # Copy the smoothing to the other models
+    lam = gam50.lam
+
+    # Generate a grid of X values for prediction
+    XX = gam50.generate_X_grid(term=0, n=500)
+
+    # Initialize dictionary to store the GAM expectiles
+    gam_expectiles = {}
+
+    # Fit all wanted expectiles and store their predictions
+    for expectile in expectiles:
+      gam = ExpectileGAM(expectile=expectile, lam=lam).fit(X, y)
+      gam_expectiles[expectile] = gam.predict(XX)
+
+    return XX, gam_expectiles
+
+# %% ../nbs/03_age_reference_plots.ipynb 6
 class AgeRefPlot:
     def __init__(
         self,
         data: pd.DataFrame,
         val_col: str,
         age_col: str = "age_at_research_stage",
         sex_col: str = "sex",
@@ -34,18 +69,17 @@
         val_color: Optional[str] = None,
         ax_main: Optional[plt.Axes] = None,
         ax_agehist: Optional[plt.Axes] = None,
         ax_valhist: Optional[plt.Axes] = None,
         age_bins: Optional[np.ndarray] = None,
         val_bins: Optional[np.ndarray] = None,
         linear_fit: bool = True,
-        lowess: bool = False,
+        expectiles: Optional[List] = [0.03, 0.1, 0.5, 0.9, 0.97],
         top_disp_perc: float = 99,
         bottom_disp_perc: float = 1,
-        percentiles_type: str = 'summary',
         robust: bool = True,
         scale: float = 1.,
         transform: Optional[Callable] = None,
         make_fig: bool = True
     ) -> None:
         """
         Initializes the AgeRefPlot class.
@@ -59,18 +93,17 @@
             val_color (Optional[str], optional): The color to use for the value plot. Defaults to None.
             ax_main (Optional[plt.Axes], optional): The main axis for the plot. Defaults to None.
             ax_agehist (Optional[plt.Axes], optional): The axis for the age histogram. Defaults to None.
             ax_valhist (Optional[plt.Axes], optional): The axis for the value histogram. Defaults to None.
             age_bins (Optional[np.ndarray], optional): The age bins for the histograms. Defaults to None.
             val_bins (Optional[np.ndarray], optional): The value bins for the histograms. Defaults to None.
             linear_fit (bool, optional): Whether to perform a linear fit on the data. Defaults to True.
-            lowess (bool, optional): Whether to perform lowess smoothing on the data. Defaults to False.
+            expectiles (Optional[List], optional): Whether to calculate and shpe gam expectiles or not. Defaults to [0.03, 0.1, 0.5, 0.9, 0.97].
             top_disp_perc (float, optional): The top percentile to use for display. Defaults to 99.
             bottom_disp_perc (float, optional): The bottom percentile to use for display. Defaults to 1.
-            percentiles_type (str, optional): The type of percentiles to use. Must be one of ['summary', '1-percent intervals', '5-percent intervals', '10-percent intervals']. Defaults to 'summary'.
             robust (bool, optional): Whether to use a robust regression method (HuberRegressor) instead of ordinary least squares for linear_fit. Defaults to True.
             scale (float, optional): The scaling factor for the value column. Defaults to 1.
             transform (Optional[Callable], optional): The transformation function to apply to the value column. Defaults
             make_fig (bool, optional): Whether to create a new figure if axes are not provided. Defaults to True.
         """
         self.data = data.dropna(subset=[age_col, val_col]).copy()
         self.data = self.data.sort_values(by=age_col)
@@ -80,39 +113,36 @@
         self.val_col = val_col
         self.age_col = age_col
         self.sex_col = sex_col
         self.transform = transform
         self.scale = scale
         self.sex = sex
         self.linear_fit = linear_fit
-        self.lowess = lowess
+        self.expectiles = expectiles
         # Cut data for display only removing outliers
         self.top_disp_perc = top_disp_perc/100
         self.bottom_disp_perc = bottom_disp_perc/100
         quantiles = self.data[[val_col]].quantile([self.bottom_disp_perc, self.top_disp_perc])
         self.disp_data = self.data[(self.data[val_col] > quantiles.loc[self.bottom_disp_perc, val_col]) &
                                    (self.data[val_col] < quantiles.loc[self.top_disp_perc, val_col])].copy()
-        # Check validity of percentiles option
-        assert percentiles_type in ['summary', '1-percent intervals', '5-percent intervals', '10-percent intervals']
-        self.percentiles_type = percentiles_type
         self.robust = robust
         self.slope = np.nan
         self.intercept = np.nan
 
         if val_color is None:
             self.val_color = {0: FEMALE_COLOR, 1: MALE_COLOR}.get(self.sex, ALL_COLOR)
         self.ref_color = REF_COLOR
 
         if age_bins is None:
             age_bins = np.arange(35, 75, 1)
         self.age_bins = age_bins
         self.min_age = self.age_bins[0]
         self.max_age = self.age_bins[-1]
 
-        self.smooth_percentiles_dict = None
+        self.expectiles_dict = None
 
         if val_bins is None:
             val_bins = np.linspace(
                 self.disp_data[self.val_col].min(), self.disp_data[self.val_col].max(), 50
             )
         self.val_bins = val_bins
 
@@ -168,85 +198,57 @@
             alpha=0.4,
             marker="o",
             facecolors="none",
             linewidths=1,
             color=self.val_color,
         )
 
-    def calc_smooth_percentiles(self):
-        def _get_percentiles_for_summary(percentiles_str):
-            percentiles_strs = {}
-            if percentiles_str == 'summary':
-                percentiles_strs = {0.1: ['10', '90'], 0.03: ['3', '97']}
-            elif percentiles_str == '1-percent intervals':
-                for i in np.arange(1, 50):
-                    percentiles_strs.update({i/100: [str(i), str(100-i)]})
-            elif percentiles_str == '5-percent intervals':
-                for i in np.arange(1, 50, 5):
-                    percentiles_strs.update({i/100: [str(i), str(100-i)]})
-                percentiles_strs.update({0.03: ['3', '97']})
-            elif percentiles_str == '10-percent intervals':
-                for i in np.arange(1, 50, 10):
-                    percentiles_strs.update({i/100: [str(i), str(100-i)]})
-                percentiles_strs.update({0.03: ['3', '97']})
-            return percentiles_strs
-
-        if self.lowess:
-            smoother = LowessSmoother(smooth_fraction=0.2, iterations=1)
-        else:
-            smoother = SplineSmoother(n_knots=6, spline_type="natural_cubic_spline")
-        smoother.smooth(self.data[self.val_col])
-
-        percentiles_dict = _get_percentiles_for_summary(self.percentiles_type)
-        self.smooth_percentiles_dict = {
-            'age': self.data[self.age_col],
-            '50': smoother.smooth_data[0],
-        }
-
-        for percent in percentiles_dict.keys():
-            low, high = smoother.get_intervals("prediction_interval", confidence=percent)
-            low_str = percentiles_dict[percent][0]
-            high_str = percentiles_dict[percent][1]
-            self.smooth_percentiles_dict.update({low_str: low[0], high_str: high[0]})
-
     def plot_percentiles(self):
-        if self.smooth_percentiles_dict is None:
-            self.calc_smooth_percentiles()
-        for perc_str in ['3', '10', '50', '90', '97']:
-            perc_vector = self.smooth_percentiles_dict[perc_str]
-            if perc_str == "age":
-                continue
+        # fetch percentiles if needed by fitting a GAM
+        if self.expectiles_dict is None:
+            X, y = self.data[[self.age_col]].values, self.data[self.val_col].values
+            XX, self.expectiles_dict = get_gam_expectiles(X, y, self.expectiles)
+
+        middle_index = len(self.expectiles) // 2
+
+        # plot expectiles curves
+        for perc_str in self.expectiles:
+            perc_vector = self.expectiles_dict[perc_str]
             self.ax_main.plot(
-                self.smooth_percentiles_dict["age"],
+                XX,
                 perc_vector,
                 color=self.ref_color,
                 alpha=0.5,
                 lw=2,
                 ls=":",
             )
             self.ax_main.text(
-                x=self.smooth_percentiles_dict["age"].max(),
+                x=XX.max(),
                 y=perc_vector[-1],
                 s=perc_str,
                 alpha=0.5,
             )
-        self.ax_main.fill_between(
-            self.smooth_percentiles_dict["age"],
-            self.smooth_percentiles_dict["10"],
-            self.smooth_percentiles_dict["90"],
-            alpha=0.1,
-            color=REF_COLOR,
-        )
-        self.ax_main.fill_between(
-            self.smooth_percentiles_dict["age"],
-            self.smooth_percentiles_dict["3"],
-            self.smooth_percentiles_dict["97"],
-            alpha=0.05,
-            color=REF_COLOR,
-        )
+
+        # fill between curves
+        if len(self.expectiles) > 2:
+            self.ax_main.fill_between(
+                XX.squeeze(),
+                self.expectiles_dict[(self.expectiles[middle_index - 1])],
+                self.expectiles_dict[(self.expectiles[middle_index + 1])],
+                alpha=0.1,
+                color=self.ref_color,
+            )
+        if len(self.expectiles) > 4:
+            self.ax_main.fill_between(
+                XX.squeeze(),
+                self.expectiles_dict[(self.expectiles[middle_index - 2])],
+                self.expectiles_dict[(self.expectiles[middle_index + 2])],
+                alpha=0.05,
+                color=self.ref_color,
+            )
 
     def calc_linear_fit(self):
         # get coeffs of linear fit
         if self.robust:
             huber = HuberRegressor().fit(
                 self.data[[self.age_col]].values, self.data[[self.val_col]].values.ravel()
             )
@@ -281,91 +283,94 @@
             # font="Roboto Condensed",
         )
 
     def plot(self):
         ax = self.ax_main
         ax.spines["right"].set_visible(False)
         ax.spines["top"].set_visible(False)
-        ax.set_xlabel("Age")
-        xticks = (np.sort(np.unique(np.floor(self.age_bins / 10) * 10))).astype(int)
-        xticks = np.append(xticks, xticks[-1] + 10)
-        ax.set_xticks(xticks)
-        ax.set_xticklabels(xticks)
-        ax.set_xlim(xticks[0], xticks[-1] + 1)
-        ax.set_ylabel(self.val_col)
 
         ax = self.ax_agehist
-        self.ax_main.get_shared_x_axes().join(self.ax_main, self.ax_agehist)
-        ax.set_xticklabels([]), ax.set_yticks([])
+        self.ax_main.sharex(self.ax_agehist)
+        ax.set_yticks([])
         ax.spines["right"].set_visible(False)
         ax.spines["left"].set_visible(False)
         ax.spines["top"].set_visible(False)
+        ax.tick_params(labelbottom=False) # hides x-tick labels
 
         ax = self.ax_valhist
-        self.ax_main.get_shared_y_axes().join(self.ax_main, self.ax_valhist)
-        ax.set_yticklabels([]), ax.set_xticks([])
+        self.ax_main.sharey(self.ax_valhist)
+        ax.set_xticks([])
         ax.spines["right"].set_visible(False)
         ax.spines["bottom"].set_visible(False)
         ax.spines["top"].set_visible(False)
-        
+        ax.tick_params(labelleft=False) # hides y-tick labels
+
+
+        ax = self.ax_main
+        ax.set_xlabel("Age")
+        xticks = (np.sort(np.unique(np.floor(self.age_bins / 10) * 10))).astype(int)
+        xticks = np.append(xticks, xticks[-1] + 10)
+        ax.set_xticks(xticks)
+        ax.set_xticklabels(xticks)
+        ax.set_xlim(xticks[0], xticks[-1] + 1)
+        ax.set_ylabel(self.val_col)
+
         self.plot_scatter()
         self.plot_percentiles()
         self.plot_ornaments()
         self.plot_agehist()
         self.plot_valhist()
 
-# %% ../nbs/03_age_reference_plots.ipynb 7
+
+# %% ../nbs/03_age_reference_plots.ipynb 8
 class GenderAgeRefPlot(AgeRefPlot):
     def __init__(
         self, 
         data: pd.DataFrame,
         val_col: str,
         age_col: str = "age_at_research_stage",
         sex_col: str = "sex",
         age_bins: Optional[np.ndarray] = None,
         val_bins: Optional[np.ndarray] = None,
         linear_fit: bool = True,
-        lowess: bool = False,
+        expectiles: Optional[List] = [0.03, 0.1, 0.5, 0.9, 0.97],
         top_disp_perc: float = 99,
         bottom_disp_perc: float = 1,
-        percentiles_type: str = 'summary',
         robust: bool = True,
         scale: float = 1.,
         transform: Optional[Callable] = None,
     ) -> None:
         """Initializes the GenderAgeRefPlot class.
 
         Args:
             data (pd.DataFrame): The input data containing age, value, and gender columns.
             val_col (str): The name of the value column in the data.
             age_col (str): The name of the age column in the DataFrame.
             sex_col (str): The name of the sex column in the DataFrame.
             age_bins (np.ndarray, optional): An array of age bin edges.
             val_bins (np.ndarray, optional): An array of value bin edges.
             linear_fit (bool, optional): Whether to fit a linear regression line. Defaults to True.
-            lowess (bool, optional): Whether to fit a LOWESS curve. Defaults to False.
+            expectiles (Optional[List], optional): Whether to calculate and shpe gam expectiles or not. Defaults to [0.03, 0.1, 0.5, 0.9, 0.97].
             top_disp_perc (float, optional): The top percentile for data display. Defaults to 99.
             bottom_disp_perc (float, optional): The bottom percentile for data display. Defaults to 1.
-            percentiles_type (str, optional): The type of percentile calculation. Defaults to 'summary'.
             robust (bool, optional): Whether to use a robust linear regression. Defaults to True.
             scale (float, optional): The scaling factor for the data. Defaults to 1.
             transform (Callable, optional): An optional function to apply to the data. Defaults to None.
         """
         super().__init__(
             data=data,
             val_col=val_col,
             age_col=age_col,
             sex_col=sex_col,
             age_bins=age_bins,
             val_bins=val_bins,
             linear_fit=linear_fit,
-            lowess=lowess,
+            expectiles=expectiles,
             top_disp_perc=top_disp_perc,
             bottom_disp_perc=bottom_disp_perc,
-            percentiles_type=percentiles_type,
             robust=robust,
             scale=scale,
             transform=transform,
             make_fig=False
         )
 
     def plot(self) -> None:
@@ -392,15 +397,15 @@
             ax_agehist=ax_dict["A"],
             ax_valhist=ax_dict["E"],
             age_bins=self.age_bins,
             val_bins=self.val_bins,
             linear_fit=self.linear_fit,
             top_disp_perc=self.top_disp_perc*100,
             bottom_disp_perc=self.bottom_disp_perc*100,
-            percentiles_type=self.percentiles_type,
+            expectiles=self.expectiles,
             robust=self.robust,
         )
         self.female_refplot.plot()
 
         self.male_refplot = AgeRefPlot(
             data=self.data[self.data["sex"]==1],
             val_col=self.val_col,
@@ -411,11 +416,11 @@
             ax_agehist=ax_dict["B"],
             ax_valhist=ax_dict["F"],
             age_bins=self.age_bins,
             val_bins=self.val_bins,
             linear_fit=self.linear_fit,
             top_disp_perc=self.top_disp_perc*100,
             bottom_disp_perc=self.bottom_disp_perc*100,
-            percentiles_type=self.percentiles_type,
+            expectiles=self.expectiles,
             robust=self.robust,
         )
         self.male_refplot.plot()
```

### Comparing `pheno-utils-0.3.5/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.6/pheno_utils/basic_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 
 # %% ../nbs/07_basic_analysis.ipynb 3
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 from typing import List, Any, Dict, Union, Optional
+import importlib
 
+# %% ../nbs/07_basic_analysis.ipynb 4
+try:
+    importlib.import_module("smart_open")
+except:
+    print("smart_open not installed, please pip install smart-open")
+
+from smart_open import open
 
 # %% ../nbs/07_basic_analysis.ipynb 5
 from .config import generate_synthetic_data
 
 # %% ../nbs/07_basic_analysis.ipynb 6
 def custom_describe(df: pd.DataFrame) -> pd.DataFrame:
     """
```

### Comparing `pheno-utils-0.3.5/pheno_utils/basic_plots.py` & `pheno-utils-0.3.6/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.6/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.6/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.6/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/pheno_utils/config.py` & `pheno-utils-0.3.6/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/pheno_utils/dates_plots.py` & `pheno-utils-0.3.6/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.6/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/pheno_utils/meta_loader.py` & `pheno-utils-0.3.6/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.6/pheno_utils/pheno_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/05_pheno_loader.ipynb.
 
 # %% auto 0
 __all__ = ['PhenoLoader']
 
 # %% ../nbs/05_pheno_loader.ipynb 3
 from glob import glob
+import traceback
+
 import os
 import re
 from typing import List, Any, Dict, Union
 import warnings
 import logging
 
 import numpy as np
@@ -338,24 +340,27 @@
         age_df = pd.read_parquet(age_path.replace('events', 'population'))
 
         # trying a workaround for a pandas deprecation warning
         age_sex = self.dfs['age_sex']
         try:
             age_df['birth_date'] = pd.to_datetime(
                 age_df['year_of_birth'].astype(str) + '-' + age_df['month_of_birth'].astype(str))
+
             missing_age_sex = align_df.loc[ind, [date]].join(age_df[['sex', 'birth_date']])\
-                .assign(age=lambda x: ((x[date].dt.date - x['birth_date'].dt.date).dt.days / 365.25).round(1))\
+                .assign(age=lambda x: ((x[date] - x['birth_date']).dt.days / 365.25).round(1))\
                 [['age', 'sex']]
             age_sex = age_sex.join(missing_age_sex, rsuffix='_miss')
 
         except Exception as e:
             if self.errors == 'raise':
+                print("Exception occurred:\n", traceback.format_exc())
                 raise(e)
             elif self.errors == 'warn':
                 warnings.warn(f'Error joining on {date}: {e}')
+
             age_sex = age_sex.join(age_df[['sex']], rsuffix='_miss').assign(age_miss=np.nan)
 
         age_sex['age'] = age_sex['age'].fillna(age_sex['age_miss'])
         age_sex['sex'] = age_sex['sex'].fillna(age_sex['sex_miss'])
         self.dfs['age_sex'] = age_sex[['age', 'sex']]
 
     def __load_dataframes__(self) -> None:
```

### Comparing `pheno-utils-0.3.5/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.6/pheno_utils/sleep_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         ax[i,0].set_xlabel('')
         ax[i,0].set_xticklabels([])
     if ax is None:
         print('entered')
         ax[-1,0].set_xlabel('Time')
         ax[-1,0].set_xlim(data[time_col].min(), data[time_col].max())
         format_xticks(ax[-1,0])
-    plt.tight_layout()
+
 
     return ax
 
 
 def format_xticks(ax, format='%m/%d %H:%M'):
     """ format datestrings on x axis """
     xticks = ax.get_xticks()
```

### Comparing `pheno-utils-0.3.5/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.6/pheno_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.5
+Version: 0.3.6
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
-Author: hrossman
-Author-email: hagairossman@gmail.com
+Author: pheno.ai
+Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pheno-utils-0.3.5/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.6/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.5/settings.ini` & `pheno-utils-0.3.6/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pheno-utils
 lib_name = pheno-utils
-version = 0.3.5
+version = 0.3.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pheno_utils
 nbs_path = nbs
 recursive = True
@@ -14,23 +14,23 @@
 branch = main
 custom_sidebar = True
 doc_host = https://pheno-ai.github.io
 doc_baseurl = /pheno-utils
 git_url = https://github.com/pheno-ai/pheno-utils
 title = pheno-utils
 audience = Developers
-author = hrossman
-author_email = hagairossman@gmail.com
-copyright = 2023 onwards, hrossman
+author = pheno.ai
+author_email = hagai@pheno.ai
+copyright = 2023 onwards, pheno.ai
 description = Pheno data utils - viz, loaders, mergers
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = pheno-ai
-requirements = fastcore pandas==1.5.2 numpy scipy fastparquet matplotlib seaborn scikit-learn pyCompare tsmoothie smart_open neurokit2 "dask[dataframe]"
+requirements = fastcore pandas numpy scipy fastparquet matplotlib seaborn scikit-learn pyCompare pygam smart_open neurokit2 "dask[dataframe]"
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `pheno-utils-0.3.5/setup.py` & `pheno-utils-0.3.6/setup.py`

 * *Files identical despite different names*

