# Comparing `tmp/puma-hep-0.2.6.tar.gz` & `tmp/puma-hep-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puma-hep-0.2.6.tar", last modified: Thu Jun  1 08:56:53 2023, max compression
+gzip compressed data, was "puma-hep-0.2.7.tar", last modified: Tue Jul 18 08:34:29 2023, max compression
```

## Comparing `puma-hep-0.2.6.tar` & `puma-hep-0.2.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.839696 puma-hep-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-01 08:56:43.000000 puma-hep-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:56:43.000000 puma-hep-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-01 08:56:53.839696 puma-hep-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-01 08:56:43.000000 puma-hep-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.835696 puma-hep-0.2.6/puma/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/fraction_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22871 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/histogram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.835696 puma-hep-0.2.6/puma/hlplots/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/hlplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/hlplots/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/hlplots/tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/line_plot_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/pie.py
--rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/roc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.835696 puma-hep-0.2.6/puma/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.835696 puma-hep-0.2.6/puma/tests/hlplots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/hlplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/hlplots/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/hlplots/test_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27274 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_line_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_pie_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18908 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_roc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_var_vs_eff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_var_vs_var.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.835696 puma-hep-0.2.6/puma/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/test_discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/test_histogram_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.839696 puma-hep-0.2.6/puma/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/utils/discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/utils/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/utils/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/var_vs_eff.py
--rw-r--r--   0 runner    (1001) docker     (123)    13851 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/var_vs_var.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.839696 puma-hep-0.2.6/puma_hep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-01 08:56:43.000000 puma-hep-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-01 08:56:53.839696 puma-hep-0.2.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-06-01 08:56:43.000000 puma-hep-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:29.286224 puma-hep-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-18 08:34:19.000000 puma-hep-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:34:19.000000 puma-hep-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-18 08:34:29.286224 puma-hep-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-18 08:34:19.000000 puma-hep-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:29.274224 puma-hep-0.2.7/puma/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/fraction_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30686 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/histogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:29.274224 puma-hep-0.2.7/puma/hlplots/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/hlplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/hlplots/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/hlplots/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/line_plot_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/roc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:29.278224 puma-hep-0.2.7/puma/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:29.278224 puma-hep-0.2.7/puma/tests/hlplots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/hlplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/hlplots/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/hlplots/test_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/test_line_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/test_pie_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/test_plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18908 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/test_roc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/test_var_vs_eff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/test_var_vs_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:29.282224 puma-hep-0.2.7/puma/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/utils/test_discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/utils/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/utils/test_histogram_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/utils/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:29.282224 puma-hep-0.2.7/puma/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/utils/discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/utils/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/utils/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/var_vs_eff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13851 2023-07-18 08:34:19.000000 puma-hep-0.2.7/puma/var_vs_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:34:29.282224 puma-hep-0.2.7/puma_hep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-18 08:34:29.000000 puma-hep-0.2.7/puma_hep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-18 08:34:29.000000 puma-hep-0.2.7/puma_hep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:34:29.000000 puma-hep-0.2.7/puma_hep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:34:29.000000 puma-hep-0.2.7/puma_hep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 08:34:29.000000 puma-hep-0.2.7/puma_hep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 08:34:29.000000 puma-hep-0.2.7/puma_hep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-18 08:34:19.000000 puma-hep-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-18 08:34:29.286224 puma-hep-0.2.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-07-18 08:34:19.000000 puma-hep-0.2.7/setup.py
```

### Comparing `puma-hep-0.2.6/LICENSE` & `puma-hep-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/PKG-INFO` & `puma-hep-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puma-hep
-Version: 0.2.6
+Version: 0.2.7
 Summary: Plotting API for HEP flavour tagging plots.
 Home-page: https://github.com/umami-hep/puma
 Keywords: machine learning,flavour tagging,plots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `puma-hep-0.2.6/README.md` & `puma-hep-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/histogram.py` & `puma-hep-0.2.7/puma/roc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,635 +1,614 @@
-"""Histogram plot functions."""
-
+"""ROC curve functions."""
 from __future__ import annotations
 
 import matplotlib as mpl
+import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
 from ftag import Flavour, Flavours
+from scipy.interpolate import pchip
 
+from puma.metrics import rej_err
 from puma.plot_base import PlotBase, PlotLineObject
-from puma.utils import get_good_colours, global_config, logger
-from puma.utils.histogram import hist_ratio, hist_w_unc
+from puma.utils import get_good_colours, get_good_linestyles, logger
 
 
-class Histogram(PlotLineObject):
-    """
-    Histogram class storing info about histogram and allows to calculate ratio w.r.t
-    other histograms.
-    """
+class Roc(PlotLineObject):
+    """Represent a single ROC curve and allows to calculate ratio w.r.t other ROCs."""
 
     def __init__(
         self,
-        values: np.ndarray,
-        weights: np.ndarray = None,
-        ratio_group: str = None,
-        flavour: str | Flavour = None,
-        add_flavour_label: bool = True,
-        histtype: str = "step",
+        sig_eff: np.ndarray,
+        bkg_rej: np.ndarray,
+        n_test: int = None,
+        rej_class: str | Flavour = None,
+        signal_class: str = None,
+        key: str = None,
         **kwargs,
     ) -> None:
-        """Initialise properties of histogram curve object.
+        """Initialise properties of roc curve object.
 
         Parameters
         ----------
-        values : np.ndarray
-            Input data for the histogram
-        weights : np.ndarray, optional
-            Weights for the input data. Has to be an array of same length as the input
-            data with a weight for each entry. If not specified, weight 1 will be given
-            to each entry. The uncertainties are calculated as the square root of the
-            squared weights (for each bin separately). By default None.
-        ratio_group : str, optional
-            Name of the ratio group this histogram is compared with. The ratio group
-            allows you to compare different groups of histograms within one plot.
-            By default None
-        flavour: str | Flavour, optional
-            If set, the correct colour and a label prefix will be extracted from
-            `puma.utils.global_config` set for this histogram.
-            Allowed values are e.g. "bjets", "cjets", "ujets", "bbjets", ...
-            By default None
-        add_flavour_label : bool, optional
-            Set to False to suppress the automatic addition of the flavour label prefix
-            in the label of the curve (i.e. "$b$-jets" in the case of b-jets).
-            This is ignored if `flavour` is not set. By default True
-        histtype: str, optional
-            `histtype` parameter which is handed to matplotlib.hist() when plotting the
-            histograms. Supported values are "bar", "barstacked", "step", "stepfilled".
-            By default "step"
+        sig_eff : np.array
+            Array of signal efficiencies
+        bkg_rej : np.array
+            Array of background rejection
+        n_test : int
+            Number of events used to calculate the background efficiencies,
+            by default None
+        signal_class : str
+            Signal class, e.g. for b-tagging "bjets", by default None
+        rej_class : str or Flavour
+            Rejection class, e.g. for b-tagging anc charm rejection "cjets",
+            by default None
+        key : str
+            Identifier for roc curve e.g. tagger, by default None
         **kwargs : kwargs
-            Keyword arguments passed to `puma.plot_base.PlotLineObject`
+            Keyword arguments passed to `puma.PlotLineObject`
 
         Raises
         ------
         ValueError
-            If input data is not of type np.ndarray or list
-        ValueError
-            If weights are specified but have different length as the input values
+            If `sig_eff` and `bkg_rej` have a different shape
         """
         super().__init__(**kwargs)
-
-        if isinstance(values, (np.ndarray, list, pd.core.series.Series)):
-            values = np.array(values)
-            if len(values) == 0:
-                logger.warning("Histogram is empty.")
-        else:
+        if len(sig_eff) != len(bkg_rej):
             raise ValueError(
-                "Invalid type of histogram input data. Allowed values are "
-                "numpy.ndarray, list, pandas.core.series.Series"
+                f"The shape of `sig_eff` ({np.shape(sig_eff)}) and `bkg_rej` "
+                f"({np.shape(bkg_rej)}) have to be identical."
             )
-        if weights is not None and len(values) != len(weights):
-            raise ValueError("`values` and `weights` are not of same length.")
-
-        self.values = values
-        self.weights = weights
-        self.ratio_group = ratio_group
-        self.flavour = Flavours[flavour] if isinstance(flavour, str) else flavour
-        self.add_flavour_label = add_flavour_label
-        self.histtype = histtype
-
-        # Set histogram attributes to None. They will be defined when the histograms
-        # are plotted
-        self.bin_edges = None
-        self.hist = None
-        self.unc = None
-        self.band = None
-        self.key = None
-
-        label = (
-            kwargs["label"] if "label" in kwargs and kwargs["label"] is not None else ""
+        self.sig_eff = sig_eff
+        self.bkg_rej = bkg_rej
+        self.n_test = None if n_test is None else int(n_test)
+        self.signal_class = signal_class
+        self.rej_class = (
+            Flavours[rej_class] if isinstance(rej_class, str) else rej_class
         )
-        # If flavour was specified, extract configuration from global config
-        if self.flavour is not None:
-            if self.flavour in Flavours:
-                # Use globally defined flavour colour if not specified
-                if self.colour is None:
-                    self.colour = self.flavour.colour
-                    logger.debug("Histogram colour was set to %s", self.colour)
-                # Add globally defined flavour label if not suppressed
-                if self.add_flavour_label:
-                    global_flavour_label = self.flavour.label
-                    self.label = f"{global_flavour_label} {label}"
-                else:
-                    self.label = label
-                logger.debug("Histogram label was set to %s", {self.label})
-            else:
-                logger.warning(
-                    "The flavour '%s' was not found in the global config.", self.flavour
-                )
+        self.key = key
 
-    def divide(self, other):
-        """Calculate ratio between two class objects.
+    def binomial_error(self, norm: bool = False, n_test: int = None) -> np.ndarray:
+        """Calculate binomial error of roc curve.
 
         Parameters
         ----------
-        other : histogram class
-            Second histogram object to calculate ratio with
+        norm : bool
+            If True calulate relative error, by default False
+        n_test : int
+            Number of events used to calculate the background efficiencies,
+            by default None
 
         Returns
         -------
-        np.ndarray
-            Ratio
-        np.ndarray
-            Ratio error
+        numpy.array
+            Binomial error
+
         Raises
         ------
         ValueError
-            If binning is not identical between 2 objects
-        ValueError
-            If hist attribute is not set for one of the two histograms
-        ValueError
-            If bin_edges attribute is not set for one of the two histograms
+            If no `n_test` was provided
         """
-        if (
-            self.bin_edges is None
-            or other.bin_edges is None
-            or self.hist is None
-            or other.hist is None
+        if n_test is None:
+            n_test = self.n_test
+        if n_test is None:
+            raise ValueError("No `n_test` provided, cannot calculate binomial error!")
+        return rej_err(self.bkg_rej[self.non_zero_mask], n_test, norm=norm)
+
+    def divide(self, roc_comp, inverse: bool = False):
+        """Calculate ratio between the roc curve and another roc.
+
+        Parameters
+        ----------
+        roc_comp : roc class
+            Second roc curve to calculate ratio with
+        inverse : bool
+            If False the ratio is calculated `this_roc / roc_comp`,
+            if True the inverse is calculated
+
+        Returns
+        -------
+        np.array
+            Signal efficiency used for the ratio calculation which is the overlapping
+            interval of the two roc curves
+        np.array
+            Ratio
+        np.array or None
+            Ratio_err if `n_test` was provided to class
+        """
+        # if same objects return array with value 1
+        if np.array_equal(
+            np.array([self.sig_eff, self.bkg_rej]),
+            np.array([roc_comp.sig_eff, roc_comp.bkg_rej]),
         ):
-            raise ValueError(
-                "Can't divide histograms since bin edges and counts are not available "
-                "for both histogram. Bins are filled when they are plotted."
-            )
+            logger.debug("roc objects are identical -> ratio is 1.")
+            ratio = np.ones(len(self.sig_eff))
+            if self.n_test is None:
+                return self.sig_eff, ratio, None
+            ratio_err = self.binomial_error(norm=True) * ratio
+            return self.sig_eff, ratio, ratio_err
+
+        # get overlapping sig_eff interval of the two roc curves
+        min_eff = max(self.sig_eff.min(), roc_comp.sig_eff.min())
+        max_eff = min(self.sig_eff.max(), roc_comp.sig_eff.max())
+        eff_mask = np.all([self.sig_eff >= min_eff, self.sig_eff <= max_eff], axis=0)
+        ratio_sig_eff = self.sig_eff[eff_mask]
+
+        # Ratio of interpolated rejection functions
+        ratio = self.fct_inter(ratio_sig_eff) / roc_comp.fct_inter(ratio_sig_eff)
+        if inverse:
+            ratio = 1 / ratio
+        if self.n_test is None:
+            return ratio_sig_eff, ratio, None
+        ratio_err = self.binomial_error(norm=True) * ratio
+        return ratio_sig_eff, ratio, ratio_err[eff_mask]
 
-        if not np.all(self.bin_edges == other.bin_edges):
-            raise ValueError("The binning of the two given objects do not match.")
+    @property
+    def fct_inter(self):
+        """
+        Interpolate the rejection function for better ratio calculation plotting etc.
 
-        # Bins where the reference histogram is empty/zero, are given a ratio of np.inf
-        # which means that the ratio plot will not have any entry in these bins.
-        ratio, ratio_unc = hist_ratio(
-            numerator=self.hist,
-            denominator=other.hist,
-            numerator_unc=self.unc,
-            denominator_unc=other.unc,
-            step=False,
-        )
-        # To use the matplotlib.step() function later on, the first bin is duplicated
-        ratio = np.append(np.array([ratio[0]]), ratio)
-        ratio_unc = np.append(np.array([ratio_unc[0]]), ratio_unc)
+        Returns
+        -------
+        pchip
+            Interpolation function
+        """
+        return pchip(self.sig_eff, self.bkg_rej)
 
-        return (ratio, ratio_unc)
+    @property
+    def non_zero_mask(self):
+        """Masking points where rejection is 0 and no signal efficiency change present.
 
+        Returns
+        -------
+        numpy.array
+            Masked indices
+        """
+        # Mask the points where there was no change in the signal eff
+        delta_x = np.concatenate((np.ones(1), np.diff(self.sig_eff)))
 
-class HistogramPlot(PlotBase):
-    """Histogram plot class."""
+        # Also mask the rejections that are 0
+        nonzero = (self.bkg_rej != 0) & (delta_x > 0)
+        if self.xmin is not None:
+            nonzero = nonzero & (self.sig_eff >= self.xmin)
+        if self.xmax is not None:
+            nonzero = nonzero & (self.sig_eff <= self.xmax)
+        return nonzero
+
+    @property
+    def non_zero(self):
+        """Abstraction of `non_zero_mask`.
 
-    def __init__(
-        self,
-        bins=40,
-        bins_range: tuple = None,
-        discrete_vals: list = None,
-        norm: bool = True,
-        logy: bool = False,
-        bin_width_in_ylabel: bool = False,
-        underoverflow: bool = False,
-        grid: bool = False,
-        **kwargs,
-    ) -> None:
-        """histogram plot properties.
+        Returns
+        -------
+        numpy.array
+            Masked signal efficiency
+        numpy.array
+            Masked background rejection
+        """
+        return self.sig_eff[self.non_zero_mask], self.bkg_rej[self.non_zero_mask]
+
+
+class RocPlot(PlotBase):
+    """ROC plot class."""
+
+    def __init__(self, grid: bool = True, **kwargs) -> None:
+        """ROC plot properties.
 
         Parameters
         ----------
-        bins : int or numpy.ndarray or list, optional
-            If bins is an int, it defines the number of equal-width bins in the given
-            range. If bins is a sequence, it defines a monotonically increasing array
-            of bin edges, including the rightmost edge, allowing for non-uniform
-            bin widths (like in numpy.histogram). By default 40
-        bins_range : tuple, optional
-            Tuple of two floats, specifying the range for the binning. If bins_range is
-            specified and bins is an integer, equal-width bins from bins_range[0] to
-            bins_range[1] are used for the histogram (like in numpy.histogram).
-            By default None
-        discrete_vals : list, optional
-            List of values if a variable only has discrete values. If discrete_vals is
-            specified only the bins containing these values are plotted.
-            By default None.
-        norm : bool, optional
-            Specify if the histograms are normalised, this means that histograms are
-            divided by the total numer of counts. Therefore, the sum of the bin counts
-            is equal to one, but NOT the area under the curve, which would be
-            sum(bin_counts * bin_width). By default True.
-        logy : bool, optional
-            Set log scale on y-axis, by default False.
-        bin_width_in_ylabel : bool, optional
-            Specify if the bin width should be added to the ylabel, by default False
-        underoverflow : bool, optional
-            Option to include under- and overflow values in outermost bins.
         grid : bool, optional
             Set the grid for the plots.
         **kwargs : kwargs
             Keyword arguments from `puma.PlotObject`
-
-        Raises
-        ------
-        ValueError
-            If n_ratio_panels > 1
         """
-        # TODO: use union operator `|` for multiple types of `bins` in python 3.10
-
         super().__init__(grid=grid, **kwargs)
-        self.logy = logy
-        self.bins = bins
-        self.bins_range = bins_range
-        self.discrete_vals = discrete_vals
-        self.bin_width_in_ylabel = bin_width_in_ylabel
-        self.norm = norm
-        self.underoverflow = underoverflow
-        self.plot_objects = {}
-        self.add_order = []
-        self.ratios_objects = {}
-        self.reference_object = None
-
-        if self.n_ratio_panels > 1:
-            raise ValueError("Not more than one ratio panel supported.")
+        self.test = ""
+        self.rocs = {}
+        self.roc_ratios = {}
+        self.rej_axes = {}
+        self.rej_class_ls = {}
+        self.label_colours = {}
+        self.leg_rej_labels = {}
+        self.reference_roc = None
         self.initialise_figure()
+        self.eff_min, self.eff_max = (1, 0)
+        self.default_linestyles = get_good_linestyles()
+        self.legend_flavs = None
+        self.leg_rej_loc = "lower left"
 
-    def add(self, histogram: object, key: str = None, reference: bool = False):
-        """Adding histogram object to figure.
+    def add_roc(self, roc_curve: object, key: str = None, reference: bool = False):
+        """Adding puma.Roc object to figure.
 
         Parameters
         ----------
-        histogram : Histogram class
-            Histogram curve
+        roc_curve : puma.Roc
+            ROC curve
         key : str, optional
-            Unique identifier for histogram, by default None
+            Unique identifier for roc_curve, by default None
         reference : bool, optional
-            If this histogram is used as reference for ratio calculation, by default
-            False
+            If roc is used as reference for ratio calculation, by default False
 
         Raises
         ------
         KeyError
             If unique identifier key is used twice
         """
         if key is None:
-            key = len(self.plot_objects) + 1
-        if key in self.plot_objects:
-            raise KeyError(f"Duplicated key {key} already used for unique identifier.")
-
-        # Add key to histogram object
-        histogram.key = key
-        logger.debug("Adding histogram %s", key)
-
-        # Set linestyle
-        if histogram.linestyle is None:
-            histogram.linestyle = "-"
-        # Set colours
-        if histogram.colour is None:
-            histogram.colour = get_good_colours()[len(self.plot_objects)]
-        # Set alpha
-        if histogram.alpha is None:
-            histogram.alpha = 1
-        # Set linewidth
-        if histogram.linewidth is None:
-            histogram.linewidth = 1.6
-
-        self.plot_objects[key] = histogram
-        self.add_order.append(key)
-        if reference is True:
-            self.set_reference(key)
+            key = len(self.rocs) + 1
+        if key in self.rocs:
+            raise KeyError(
+                f"Duplicated key {key} already used for roc unique identifier."
+            )
+
+        self.rocs[key] = roc_curve
+        # set linestyle
+        if roc_curve.rej_class not in self.rej_class_ls:
+            self.rej_class_ls[roc_curve.rej_class] = (
+                self.default_linestyles[len(self.rej_class_ls)]
+                if roc_curve.linestyle is None
+                else roc_curve.linestyle
+            )
+        elif (
+            roc_curve.linestyle != self.rej_class_ls[roc_curve.rej_class]
+            and roc_curve.linestyle is not None
+        ):
+            logger.warning(
+                (
+                    "You specified a different linestyle for the same rejection class "
+                    "%s. Will keep the linestyle defined first."
+                ),
+                roc_curve.rej_class,
+            )
+        if roc_curve.linestyle is None:
+            roc_curve.linestyle = self.rej_class_ls[roc_curve.rej_class]
+
+        # set colours
+        if roc_curve.label not in self.label_colours:
+            self.label_colours[roc_curve.label] = (
+                get_good_colours()[len(self.label_colours)]
+                if roc_curve.colour is None
+                else roc_curve.colour
+            )
+        elif (
+            roc_curve.colour != self.label_colours[roc_curve.label]
+            and roc_curve.colour is not None
+        ):
+            logger.warning(
+                (
+                    "You specified a different colour for the same label"
+                    " %s. This will lead to a mismatch in the line colours"
+                    " and the legend."
+                ),
+                roc_curve.label,
+            )
+        if roc_curve.colour is None:
+            roc_curve.colour = self.label_colours[roc_curve.label]
+
+        if reference:
+            logger.debug(
+                "Setting roc %s as reference for %s.", key, roc_curve.rej_class
+            )
+            self.set_roc_reference(key, roc_curve.rej_class)
 
-    def set_reference(self, key: str):
-        """Setting the reference histogram curves used in the ratios.
+    def set_roc_reference(self, key: str, rej_class: Flavour):
+        """Setting the reference roc curves used in the ratios.
 
         Parameters
         ----------
         key : str
-            Unique identifier of histogram object
+            Unique identifier of roc object
+        rej_class : str
+            Rejection class encoded in roc curve
+
+        Raises
+        ------
+        ValueError
+            If more rejection classes are set than actual ratio panels available.
         """
-        if self.reference_object is None:
-            self.reference_object = [key]
+        if self.reference_roc is None:
+            self.reference_roc = {}
+            self.reference_roc[rej_class] = key
+        elif rej_class not in self.reference_roc:
+            if len(self.reference_roc) >= self.n_ratio_panels:
+                raise ValueError(
+                    "You cannot set more rejection classes than available ratio panels."
+                )
+            self.reference_roc[rej_class] = key
         else:
-            self.reference_object.append(key)
-        logger.debug("Adding '%s' to reference histogram(s)", key)
+            logger.warning(
+                (
+                    "You specified a second roc curve %s as reference for ratio. "
+                    "Using it as new reference instead of %s."
+                ),
+                key,
+                self.reference_roc[rej_class],
+            )
+            self.reference_roc[rej_class] = key
 
-    def plot(self, **kwargs):
-        """Plotting curves. This also generates the bins of the histograms that are
-        added to the plot. Plot objects are drawn in the same order as they were added
-        to the plot.
+    def set_ratio_class(self, ratio_panel: int, rej_class: str | Flavour):
+        """Associate the rejection class to a ratio panel adn set the legend label.
 
         Parameters
         ----------
-        **kwargs: kwargs
-            Keyword arguments passed to matplotlib.axes.Axes.hist()
-
-        Returns
-        -------
-        Line2D
-            matplotlib Line2D object
+        ratio_panel : int
+            Ratio panel either 1 or 2
+        rej_class : Flavour
+            Rejeciton class associated to that panel
 
         Raises
         ------
         ValueError
-            If specified bins type is not supported.
+            if requested ratio panels and given ratio_panel do not match.
         """
-        if self.ylabel is not None and self.norm and "norm" not in self.ylabel.lower():
-            logger.warning(
-                "You are plotting normalised distributions but 'norm' is not "
-                "included in your y-label."
-            )
-        plt_handles = []
-
-        # Calculate bins of stacked histograms to ensure all histograms fit in plot
-        if isinstance(self.bins, (np.ndarray, list)):
-            logger.debug("Using bin edges defined in plot instance.")
-            if self.bins_range is not None:
-                logger.warning(
-                    "You defined a range for the histogram, but also an array with "
-                    "the bin edges. The range will be ignored."
-                )
-        elif isinstance(self.bins, int):
-            logger.debug("Calculating bin edges of %i equal-width bins", self.bins)
-            _, self.bins = np.histogram(
-                np.hstack([elem.values for elem in self.plot_objects.values()]),
-                bins=self.bins,
-                range=self.bins_range,
-            )
-        else:
+        rej_class = Flavours[rej_class] if isinstance(rej_class, str) else rej_class
+        if self.n_ratio_panels < ratio_panel:
             raise ValueError(
-                "Unsupported type for bins. Supported types: int, numpy.array, list"
-            )
-
-        # Loop over all plot objects and plot them
-        bins = self.bins
-        for key in self.add_order:
-            elem = self.plot_objects[key]
-
-            elem.bin_edges, elem.hist, elem.unc, elem.band = hist_w_unc(
-                elem.values,
-                weights=elem.weights,
-                bins=self.bins,
-                bins_range=self.bins_range,
-                normed=self.norm,
-                underoverflow=self.underoverflow,
-            )
-
-            if self.discrete_vals is not None:
-                # bins are recalculated for the discrete values
-                bins = self.get_discrete_values(elem)
-
-            # Plot histogram
-            self.axis_top.hist(
-                x=bins[:-1],
-                bins=bins,
-                weights=elem.hist,
-                histtype=elem.histtype,
-                color=elem.colour,
-                label=elem.label,
-                alpha=elem.alpha,
-                linewidth=elem.linewidth,
-                linestyle=elem.linestyle,
-                **kwargs,
-            )
-
-            # Plot histogram uncertainty
-            if self.draw_errors:
-                self.axis_top.hist(
-                    x=bins[:-1],
-                    bins=bins,
-                    bottom=elem.band,
-                    weights=elem.unc * 2,
-                    **global_config["hist_err_style"],
-                )
-
-            plt_handles.append(
-                mpl.lines.Line2D(
-                    [],
-                    [],
-                    color=elem.colour,
-                    label=elem.label,
-                    alpha=elem.alpha,
-                    linewidth=elem.linewidth,
-                    linestyle=elem.linestyle,
-                )
+                "Requested ratio panels and given ratio_panel do not match."
             )
+        self.rej_axes[rej_class] = self.ratio_axes[ratio_panel - 1]
+        label = rej_class.label.replace("jets", "jet")
+        self.set_ratio_label(ratio_panel, f"{label} ratio")
+        self.leg_rej_labels[rej_class] = rej_class.label
 
-        if self.draw_errors:
-            plt_handles.append(
-                mpl.patches.Patch(
-                    label="stat. uncertainty", **global_config["hist_err_style"]
-                )
-            )
-
-        if self.discrete_vals is not None:
-            self.bins = bins
-
-        self.plotting_done = True
-        return plt_handles
-
-    def get_discrete_values(self, elem: object):
-        """Get discrete values of a variable and adjust the
-        bins accordingly.
-
-        Parameters
-        ----------
-        elem : histogram class
-            Histogram we want to calculate the bins containing discrete values for
-
-        Returns
-        -------
-        bins : numpy.ndarray
-            Recalculated bins including only the discrete values
+    def add_ratios(self):
+        """Calculating ratios.
 
         Raises
         ------
         ValueError
-            If the bin width is larger than 1 such that potentially not
-            all discrete values are in a seperate bin
+            If number of reference rocs and ratio panels don't match
         ValueError
-            If the number of bins is set to 1 such that no values can be
-            distinguished
+            If no ratio classes are set
         """
-        if len(elem.bin_edges) > 1:
-            if abs(elem.bin_edges[1] - elem.bin_edges[0]) <= 1:
-                indice = []
-                for i in range(len(elem.bin_edges) - 1):
-                    # Only keep this bin edge if one of the discrete
-                    # values is withing this and the next bin edge
-                    # TODO: This has to be improved.
-                    # The current implementation
-                    #       a)  requires to specify a range which includes all the
-                    #           specified value --> this could be done automatically?
-                    #       b)  crashes if the specified range ends at a value which
-                    #           is equal to a value in self.discrete_vals (since we
-                    #           do not accept "<=" in the last bin)
-                    for discrete_val in self.discrete_vals:
-                        if elem.bin_edges[i] <= discrete_val < elem.bin_edges[i + 1]:
-                            indice.append(i)
-                elem.hist = elem.hist[indice]
-                elem.unc = elem.unc[indice]
-                elem.band = elem.band[indice]
-                bins = np.linspace(
-                    0, len(self.discrete_vals), len(self.discrete_vals) + 1
-                )
-                elem.bin_edges = bins
-                self.axis_top.set_xticks(bins[:-1] + 0.5)
-                self.axis_top.set_xticklabels(self.discrete_vals, rotation=33)
-            else:
-                raise ValueError(
-                    "Bin width is larger than 1. Choose a binning with a bin"
-                    " width<= 1 to plot only discrete values."
-                )
-        else:
+        if len(self.reference_roc) != self.n_ratio_panels:
             raise ValueError(
-                "Choose a binning with more than one bin in order to plot only discrete"
-                " values."
+                f"{len(self.reference_roc)} reference rocs defined but requested "
+                f"{self.n_ratio_panels} ratio panels."
+            )
+        if len(self.rej_axes) != self.n_ratio_panels:
+            raise ValueError(
+                "Ratio classes not set, set them first with `set_ratio_class`."
             )
 
-        return bins
-
-    def get_reference_histo(self, histo):
-        """Get reference histogram from list of references.
+        for rej_class, axis in self.rej_axes.items():
+            self.plot_ratios(axis=axis, rej_class=rej_class)
 
-        Parameters
-        ----------
-        histo : puma.histogram.Histogram
-            Histogram we want to calculate the ratio for
+    def get_xlim_auto(self):
+        """Returns min and max efficiency values.
 
         Returns
         -------
-        reference_histo_name : str, int
-            Identifier of the corresponding reference histogram
-
-        Raises
-        ------
-        ValueError
-            If no reference histo was found or multiple matches.
+        float
+            Min and max efficiency values
         """
-        matches = 0
-        reference_histo = None
+        for elem in self.rocs.values():
+            self.eff_min = min(np.min(elem.sig_eff), self.eff_min)
+            self.eff_max = max(np.max(elem.sig_eff), self.eff_min)
 
-        for key in self.reference_object:
-            reference_candidate = self.plot_objects[key]
-            if histo.ratio_group is not None:
-                if histo.ratio_group == reference_candidate.ratio_group:
-                    matches += 1
-                    reference_histo = reference_candidate
-            else:
-                matches += 1
-                reference_histo = reference_candidate
+        return self.eff_min, self.eff_max
 
-        if matches != 1:
-            raise ValueError(
-                f"Found {matches} matching reference candidates, but only one match is"
-                " allowed."
-            )
+    def plot_ratios(self, axis: plt.axis, rej_class: str):
+        """Plotting ratio curves.
 
-        logger.debug(
-            "Reference histogram for '%s' is '%s'", histo.key, reference_histo.key
-        )
+        Parameters
+        ----------
+        axis : plt.axis
+            matplotlib axis object
+        rej_class : str
+            Rejection class
+        """
+        for key, elem in self.rocs.items():
+            if elem.rej_class != rej_class:
+                continue
+            ratio_sig_eff, ratio, ratio_err = elem.divide(
+                self.rocs[self.reference_roc[rej_class]]
+            )
+            self.roc_ratios[key] = (ratio_sig_eff, ratio, ratio_err)
+            axis.plot(
+                ratio_sig_eff,
+                ratio,
+                color=elem.colour,
+                linestyle=elem.linestyle,
+                linewidth=1.6,
+            )
+            if ratio_err is not None:
+                axis.fill_between(
+                    ratio_sig_eff,
+                    ratio - ratio_err,
+                    ratio + ratio_err,
+                    color=elem.colour,
+                    alpha=0.3,
+                    zorder=1,
+                )
 
-        return reference_histo
+    def set_leg_rej_loc(self, option: str):
+        """Set the position of the rejection class legend. Only if 2 ratio panels are
+        defined.
 
-    def plot_ratios(self):
-        """Plotting ratio histograms.
+        Parameters
+        ----------
+        option : str
+            Defines where to place the legend for rejection class. Accepts all options
+            from `matplotlib.axes.Axes.legend` as well as the option `ratio_legend`,
+            which adds the legend into the ratio panels
 
         Raises
         ------
         ValueError
-            If no reference histogram is defined
+            If not 2 ratios requested
         """
-        if self.reference_object is None:
-            raise ValueError("Please specify a reference curve.")
+        if self.n_ratio_panels != 2:
+            raise ValueError("For a rejection class legend you need 2 ratio panels.")
 
-        for key in self.add_order:
-            elem = self.plot_objects[key]
+        self.leg_rej_loc = option
 
-            if elem.bin_edges is None:
-                raise ValueError(
-                    "Bin edges of plot object not set. This is done in "
-                    "histogram_plot.plot(), so it has to be called before "
-                    "plot_ratios() is called."
-                )
-
-            ratio, ratio_unc = elem.divide(self.get_reference_histo(elem))
+    def make_split_legend(self, handles):
+        """Draw legend for the case of 2 ratios, splitting up legend into models and
+        rejection class.
 
-            ratio_unc_band_low = np.nan_to_num(ratio - ratio_unc, nan=0, posinf=0)
-            ratio_unc_band_high = np.nan_to_num(ratio + ratio_unc, nan=0, posinf=0)
-
-            # Plot the ratio values with the step function
-            self.ratio_axes[0].step(
-                x=elem.bin_edges,
-                y=ratio,
-                color=elem.colour,
-                linewidth=elem.linewidth,
-                linestyle=elem.linestyle,
-            )
-
-            # Plot the ratio uncertainty
-            if self.draw_errors:
-                self.ratio_axes[0].fill_between(
-                    x=elem.bin_edges,
-                    y1=ratio_unc_band_low,
-                    y2=ratio_unc_band_high,
-                    step="pre",
-                    facecolor="none",
-                    edgecolor=global_config["hist_err_style"]["edgecolor"],
-                    linewidth=global_config["hist_err_style"]["linewidth"],
-                    hatch=global_config["hist_err_style"]["hatch"],
-                )
-
-    def add_bin_width_to_ylabel(self):
-        """Adds the bin width to the ylabel of a histogram plot. If the bin with is
-        smaller than 0.01, scientific notation will be used.
+        Parameters
+        ----------
+        handles : list
+            List of Line2D objects to extract info for legend
 
         Raises
         ------
         ValueError
-            If plotting_done is False (therefore `bins` is not yet calculated)
+            If not 2 ratios requested
         """
-        if self.plotting_done is False:
-            raise ValueError(
-                "`add_bin_width_to_ylabel` should be called after plotting, since bins "
-                "are calculated during plotting."
-            )
+        if self.n_ratio_panels < 2:
+            raise ValueError("For a split legend you need 2 ratio panels.")
+
+        if self.leg_rej_loc == "ratio_legend":
+            for rej_class, axis in self.rej_axes.items():
+                legend_line = mpl.lines.Line2D(
+                    [],
+                    [],
+                    color="k",
+                    label=self.leg_rej_labels[rej_class],
+                    linestyle=self.rej_class_ls[rej_class],
+                )
+                axis.legend(
+                    handles=[legend_line],
+                    labels=[legend_line.get_label()],
+                    loc="upper right",
+                    fontsize=self.leg_fontsize,
+                )
 
-        bin_width = abs(self.bins[1] - self.bins[0])
-        if bin_width < 1e-2:
-            self.ylabel = f"{self.ylabel} / {bin_width:.0e}"
         else:
-            self.ylabel = f"{self.ylabel} / {bin_width:.2f}"
-        self.set_ylabel(self.axis_top)
+            line_list_rej = []
+            for rej_class in self.rej_axes:
+                line_list_rej.append(
+                    mpl.lines.Line2D(
+                        [],
+                        [],
+                        color="k",
+                        label=self.leg_rej_labels[rej_class],
+                        linestyle=self.rej_class_ls[rej_class],
+                    )
+                )
+
+            self.legend_flavs = self.axis_top.legend(
+                handles=line_list_rej,
+                labels=[handle.get_label() for handle in line_list_rej],
+                loc=self.leg_rej_loc,
+                fontsize=self.leg_fontsize,
+                ncol=self.leg_ncol,
+            )
+
+            # Add the second legend to plot
+            self.axis_top.add_artist(self.legend_flavs)
+
+        # Get the labels for the legends
+        labels_list = []
+        lines_list = []
+
+        for line in handles:
+            if line.get_label() not in labels_list:
+                labels_list.append(line.get_label())
+                lines_list.append(line)
+
+        # Define the legend
+        self.axis_top.legend(
+            handles=lines_list,
+            labels=labels_list,
+            loc=self.leg_loc,
+            fontsize=self.leg_fontsize,
+            ncol=self.leg_ncol,
+        )
 
-    def draw(self, labelpad: int = None):
-        """Draw figure.
+    def draw(
+        self,
+        labelpad: int = None,
+    ):
+        """Draw plotting.
 
         Parameters
         ----------
         labelpad : int, optional
             Spacing in points from the axes bounding box including
-            ticks and tick labels, by default "ratio"
-
+            ticks and tick labels, by default None
         """
-        plt_handles = self.plot()
-
-        if self.n_ratio_panels > 0:
-            self.plot_ratios()
+        plt_handles = self.plot_roc()
+        xmin, xmax = self.get_xlim_auto()
 
         self.set_xlim(
-            self.bins[0] if self.xmin is None else self.xmin,
-            self.bins[-1] if self.xmax is None else self.xmax,
+            xmin if self.xmin is None else self.xmin,
+            xmax if self.xmax is None else self.xmax,
         )
+        if self.n_ratio_panels > 0:
+            self.add_ratios()
+        self.set_title()
         self.set_log()
         self.set_y_lim()
         self.set_xlabel()
-        self.set_tick_params()
         self.set_ylabel(self.axis_top)
 
-        if self.n_ratio_panels > 0:
+        for i, axis in enumerate(self.rej_axes.values()):
             self.set_ylabel(
-                self.ratio_axes[0],
-                self.ylabel_ratio[0],
+                axis,
+                self.ylabel_ratio[i],
                 align_right=False,
                 labelpad=labelpad,
             )
 
-        if self.bin_width_in_ylabel is True:
-            self.add_bin_width_to_ylabel()
-
-        legend_axis = self.axis_top
+        if self.n_ratio_panels < 2:
+            self.make_legend(plt_handles, ax_mpl=self.axis_top)
+        else:
+            if not self.leg_rej_labels:
+                for rej_class in self.rej_axes:
+                    self.leg_rej_labels[rej_class] = rej_class
 
-        self.make_legend(plt_handles, ax_mpl=legend_axis)
-        self.set_title()
+            self.make_split_legend(handles=plt_handles)
 
-        if self.apply_atlas_style:
+        self.plotting_done = True
+        if self.apply_atlas_style is True:
             self.atlasify()
+            # atlasify can only handle one legend. Therefore, we remove the frame of
+            # the second legend by hand
+            if self.legend_flavs is not None:
+                self.legend_flavs.set_frame_on(False)
+
+    def plot_roc(self, **kwargs) -> mpl.lines.Line2D:
+        """Plotting roc curves.
+
+        Parameters
+        ----------
+        **kwargs: kwargs
+            Keyword arguments passed to plt.axis.plot
+
+        Returns
+        -------
+        Line2D
+            matplotlib Line2D object
+        """
+        plt_handles = []
+        for key, elem in self.rocs.items():
+            plt_handles = plt_handles + self.axis_top.plot(
+                elem.sig_eff[elem.non_zero_mask],
+                elem.bkg_rej[elem.non_zero_mask],
+                linestyle=elem.linestyle,
+                color=elem.colour,
+                label=elem.label if elem is not None else key,
+                zorder=2,
+                **kwargs,
+            )
+            if elem.n_test is not None:
+                # if uncertainties are available for roc plotting their uncertainty as
+                # a band around the roc itself
+                rej_band_down = (
+                    elem.bkg_rej[elem.non_zero_mask]
+                    - elem.binomial_error()[elem.non_zero_mask]
+                )
+                rej_band_up = (
+                    elem.bkg_rej[elem.non_zero_mask]
+                    + elem.binomial_error()[elem.non_zero_mask]
+                )
+                self.axis_top.fill_between(
+                    elem.sig_eff[elem.non_zero_mask],
+                    rej_band_down,
+                    rej_band_up,
+                    color=elem.colour,
+                    alpha=0.3,
+                    zorder=2,
+                )
+        return plt_handles
```

### Comparing `puma-hep-0.2.6/puma/hlplots/results.py` & `puma-hep-0.2.7/puma/hlplots/results.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/hlplots/tagger.py` & `puma-hep-0.2.7/puma/hlplots/tagger.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/line_plot_2d.py` & `puma-hep-0.2.7/puma/line_plot_2d.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/metrics.py` & `puma-hep-0.2.7/puma/metrics.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/pie.py` & `puma-hep-0.2.7/puma/pie.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/plot_base.py` & `puma-hep-0.2.7/puma/plot_base.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/hlplots/test_results.py` & `puma-hep-0.2.7/puma/tests/hlplots/test_results.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/hlplots/test_tagger.py` & `puma-hep-0.2.7/puma/tests/hlplots/test_tagger.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/test_histogram.py` & `puma-hep-0.2.7/puma/tests/test_histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,20 @@
         n_random = 10_000
         self.hist_1 = Histogram(
             np.random.normal(size=n_random), label=f"N={n_random:_}"
         )
         self.hist_2 = Histogram(
             np.random.normal(size=2 * n_random), label=f"N={2*n_random:_}"
         )
+        self.data_hist = Histogram(
+            np.random.normal(size=3 * n_random),
+            label=f"Toy Data, N={3*n_random:_}",
+            is_data=True,
+            colour="k",
+        )
 
         # Set up directories for comparison plots
         self.tmp_dir = tempfile.TemporaryDirectory()
         self.actual_plots_dir = f"{self.tmp_dir.name}/"
         self.expected_plots_dir = os.path.join(
             os.path.dirname(__file__), "expected_plots"
         )
@@ -197,14 +203,47 @@
         hist_plot.savefig(f"{self.actual_plots_dir}/{plotname}")
         # Uncomment line below to update expected image
         # hist_plot.savefig(f"{self.expected_plots_dir}/{plotname}")
         self.assertIsNone(
             compare_images(
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
+                tol=1,
+            )
+        )
+
+    def test_data_mc(self):
+        """Check if data mc looks good"""
+        hist_plot = HistogramPlot(
+            bins=20,
+            bins_range=[-2, 2],
+            atlas_brand="",
+            atlas_first_tag="Simulation, $\\sqrt{s}=13$ TeV",
+            atlas_second_tag="Second tag with additional\ndistance from first tag",
+            figsize=(5, 4),
+            ylabel="Number of jets",
+            n_ratio_panels=1,
+            atlas_second_tag_distance=0.3,
+            stacked=True,
+            norm=False,
+        )
+        hist_plot.add(self.hist_1)
+        hist_plot.add(self.hist_2)
+        hist_plot.add(self.data_hist)
+        hist_plot.draw()
+        hist_plot.add_bin_width_to_ylabel()
+
+        plotname = "test_histogram_data_mc.png"
+        hist_plot.savefig(f"{self.actual_plots_dir}/{plotname}")
+        # Uncomment line below to update expected image
+        # hist_plot.savefig(f"{self.expected_plots_dir}/{plotname}")
+        self.assertIsNone(
+            compare_images(
+                f"{self.actual_plots_dir}/{plotname}",
+                f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_discrete_values(self):
         """check if discrete values are working properly."""
         hist_plot = HistogramPlot(
```

### Comparing `puma-hep-0.2.6/puma/tests/test_line_2d.py` & `puma-hep-0.2.7/puma/tests/test_line_2d.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/test_metrics.py` & `puma-hep-0.2.7/puma/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/test_pie_chart.py` & `puma-hep-0.2.7/puma/tests/test_pie_chart.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/test_plot_base.py` & `puma-hep-0.2.7/puma/tests/test_plot_base.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/test_roc.py` & `puma-hep-0.2.7/puma/tests/test_roc.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/test_var_vs_eff.py` & `puma-hep-0.2.7/puma/tests/test_var_vs_eff.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/test_var_vs_var.py` & `puma-hep-0.2.7/puma/tests/test_var_vs_var.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/utils/test_discriminant.py` & `puma-hep-0.2.7/puma/tests/utils/test_discriminant.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/utils/test_generate.py` & `puma-hep-0.2.7/puma/tests/utils/test_generate.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/utils/test_histogram_utils.py` & `puma-hep-0.2.7/puma/tests/utils/test_histogram_utils.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/tests/utils/test_utils.py` & `puma-hep-0.2.7/puma/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/utils/discriminant.py` & `puma-hep-0.2.7/puma/utils/discriminant.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/utils/generate.py` & `puma-hep-0.2.7/puma/utils/generate.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/utils/histogram.py` & `puma-hep-0.2.7/puma/utils/histogram.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/utils/logging.py` & `puma-hep-0.2.7/puma/utils/logging.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/var_vs_eff.py` & `puma-hep-0.2.7/puma/var_vs_eff.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma/var_vs_var.py` & `puma-hep-0.2.7/puma/var_vs_var.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.6/puma_hep.egg-info/PKG-INFO` & `puma-hep-0.2.7/puma_hep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puma-hep
-Version: 0.2.6
+Version: 0.2.7
 Summary: Plotting API for HEP flavour tagging plots.
 Home-page: https://github.com/umami-hep/puma
 Keywords: machine learning,flavour tagging,plots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `puma-hep-0.2.6/puma_hep.egg-info/SOURCES.txt` & `puma-hep-0.2.7/puma_hep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

