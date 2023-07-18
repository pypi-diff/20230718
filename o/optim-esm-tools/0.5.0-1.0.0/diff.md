# Comparing `tmp/optim_esm_tools-0.5.0.tar.gz` & `tmp/optim_esm_tools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optim_esm_tools-0.5.0.tar", last modified: Wed Jul 12 12:47:32 2023, max compression
+gzip compressed data, was "optim_esm_tools-1.0.0.tar", last modified: Tue Jul 18 09:37:36 2023, max compression
```

## Comparing `optim_esm_tools-0.5.0.tar` & `optim_esm_tools-1.0.0.tar`

### file list

```diff
@@ -1,53 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.691658 optim_esm_tools-0.5.0/optim_esm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/_test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/optim_esm_tools/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/calculate_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/cmip_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/query_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    25466 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/tipping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/analyze/xarray_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/optim_esm_tools/cmip_files/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/cmip_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/optim_esm_conf.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/optim_esm_tools/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/plotting/map_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/plotting/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/optim_esm_tools/synda_files/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/synda_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/synda_files/format_synda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/synda_files/synda_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/optim_esm_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 12:47:32.000000 optim_esm_tools-0.5.0/optim_esm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 12:47:32.699658 optim_esm_tools-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:32.695658 optim_esm_tools-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_area_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_pangeo_download.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-12 12:47:29.000000 optim_esm_tools-0.5.0/test/test_xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.616131 optim_esm_tools-1.0.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/bin/oet_plot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.616131 optim_esm_tools-1.0.0/optim_esm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/_test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/optim_esm_tools/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/cmip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25670 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/tipping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/analyze/xarray_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/optim_esm_conf.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/optim_esm_tools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15918 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/plotting/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/plotting/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/optim_esm_tools/synda_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/synda_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/synda_files/synda_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/optim_esm_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.616131 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 09:37:36.000000 optim_esm_tools-1.0.0/optim_esm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:37:36.620131 optim_esm_tools-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_pangeo_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-18 09:37:33.000000 optim_esm_tools-1.0.0/test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-0.5.0/PKG-INFO` & `optim_esm_tools-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim_esm_tools
-Version: 0.5.0
+Version: 1.0.0
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,32 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        1.0.0 / 2023-07-18
+        ------------------
+        **major change**
+        * Harmonize preprocessing with `cdo` by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/81
+        
+        **minor changes**
+        * Plotting routine for masked regions by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/82
+        * Plot region mask by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/85
+        * Add plot maker by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/83
+        
+        **patches**
+        * Raise error for invalid dates by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/84
+        * [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in https://github.com/JoranAngevaare/optim_esm_tools/pull/86
+        * Ready for release v1.0.0 by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/87
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.5.0...v1.0.0
+        
+        
         0.5.0 / 2023-07-07
         ------------------
         **Last release before refactoring pre-processing**
         *Next release will use CDO tools instead of xMip tools to do pre-processing for reliability reasons*
         
         * Lon and lat coords for clustering by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/79
         * Queriable area field by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/80
```

### Comparing `optim_esm_tools-0.5.0/README.md` & `optim_esm_tools-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools/_test_utils.py` & `optim_esm_tools-1.0.0/optim_esm_tools/_test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,37 +36,39 @@
     data = list(ddict.values())[0]
 
     data = data.mean(set(data.dims) - {'x', 'y', 'lat', 'lon', 'time'})
     if query['variable_id'] != 'tas':
         raise ValueError(
             'Only tas for now as only areacella is hardcoded (see line below)'
         )
-    data.attrs.update(dict(external_variables='areacella'))
+    data.attrs.update(dict(external_variables='areacella', variable_id='tas'))
     os.makedirs(dest_folder, exist_ok=True)
+    assert data.attrs.get('variable_id')
     data.to_netcdf(write_to)
     return write_to
 
 
 def year_means(path, refresh=True):
     new_dir = os.path.split(path.replace('Amon', 'AYear'))[0]
     new_dest = os.path.join(new_dir, 'test_merged.nc')
     if os.path.exists(new_dest) and not refresh:
         print(f'File at {new_dest} already exists')
         return new_dest
     import cftime
     import optim_esm_tools as oet
 
-    data = oet.cmip_files.io.load_glob(path)
+    data = oet.analyze.io.load_glob(path)
 
     data = data.groupby('time.year').mean('time')
     data = data.rename(year='time')
     data['time'] = [cftime.DatetimeNoLeap(y, 1, 1) for y in data['time']]
-
+    data.attrs.update(dict(external_variables='areacella', variable_id='tas'))
     os.makedirs(new_dir, exist_ok=True)
     assert os.path.exists(new_dir)
+    assert data.attrs.get('variable_id')
     data.to_netcdf(new_dest)
     return new_dest
 
 
 def get_synda_loc():
     return os.path.join(
         os.environ.get('ST_HOME', os.path.join(os.path.abspath('.'), 'cmip')), 'data'
@@ -100,19 +102,19 @@
     # Add some NaN values just as an example
     if add_nans:
         data[:, :, len(lon) // 2 + 30 : len(lon) // 2 + 50] = np.nan
 
     ds_dummy = xr.Dataset(
         data_vars=dict(
             var=(
-                ('time', 'x', 'y'),
+                ('time', 'lat', 'lon'),
                 data,
             )
         ),
         coords=dict(
             time=time,
-            lon=lon,
             lat=lat,
+            lon=lon,
         ),
-        attrs=dict(source_id='bla'),
+        attrs=dict(source_id='bla', variable_id='var'),
     )
     return ds_dummy
```

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools/analyze/clustering.py` & `optim_esm_tools-1.0.0/optim_esm_tools/analyze/clustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,25 @@
     min_samples: int = 10,
     cluster_opts: ty.Optional[dict] = None,
 ) -> ty.List[np.ndarray]:
     """Build clusters based on a list of coordinates, use halfsine metric for spherical spatiol data
 
     Args:
         coordinates_deg (np.ndarray): set of xy coordinates in degrees
+        weights (ty.Optional[np.ndarray], optional): weights (in the range [0,1]) corresponding to each coordinate
         max_distance_km (ty.Union[float, int], optional): max distance to other points to consider part of
             cluster (see DBSCAN(eps=<..>)). Defaults to 750.
         only_core (bool, optional): Use only core samples. Defaults to True.
-        min_sample (int): Minimum number of samples in cluster. Defaults to 20.
+        min_samples (int): Minimum number of samples in cluster. Defaults to 20.
         cluster_opts (ty.Optional[dict], optional): Additional options passed to sklearn.cluster.DBSCAN. Defaults to None.
 
     Returns:
         ty.List[np.ndarray]: list of clustered points (in radians)
     """
-    if cluster_opts is None:
-        cluster_opts = dict()
+    cluster_opts = cluster_opts or dict()
     for class_label, v in dict(algorithm='ball_tree', metric='haversine').items():
         cluster_opts.setdefault(class_label, v)
     cluster_opts['min_samples'] = min_samples
 
     from sklearn.cluster import DBSCAN
     import numpy as np
 
@@ -86,21 +86,21 @@
     max_distance_km: ty.Union[str, float, int] = 'infer',
     **kw,
 ) -> ty.Tuple[ty.List[np.ndarray], ty.List[np.ndarray]]:
     """Build set of clusters and masks based on the global mask, basically a utility wrapper arround build_clusters'
 
     Args:
         global_mask (np.ndarray): full 2d mask of the data
-        x_coord (np.array): all x values
-        y_coord (np.array): all y values
+        lon_coord (np.array): all longitude values
+        lat_coord (np.array): all latitude values
+        show_tqdm (bool, optional): use verboose progressbar. Defaults to False.
         max_distance_km (ty.Union[str, float, int]): find an appropriate distance
             threshold for build_clusters' max_distance_km argument. If nothing is
             provided, make a guess based on the distance between grid cells.
             Defaults to 'infer'.
-        show_tqdm (bool, optional): use verboose progressbar. Defaults to False.
 
     Returns:
         ty.List[ty.List[np.ndarray], ty.List[np.ndarray]]: Return two lists, containing the masks, and clusters respectively.
     """
     lon, lat = _check_input(global_mask, lon_coord, lat_coord)
     xy_data = np.array([lon[global_mask], lat[global_mask]])
 
@@ -108,16 +108,16 @@
         warn(f'No data from this mask {xy_data}!')
         return [], []
 
     if max_distance_km == 'infer':
         max_distance_km = _infer_max_step_size(lon_coord.flatten(), lat_coord.flatten())
 
     masks, clusters = _build_cluster_with_kw(
-        lon_coord,
-        lat_coord,
+        lon,
+        lat,
         coordinates_deg=xy_data,
         show_tqdm=show_tqdm,
         max_distance_km=max_distance_km,
         **kw,
     )
 
     return masks, clusters
@@ -125,29 +125,30 @@
 
 @timed()
 def build_weighted_cluster(
     weights: np.ndarray,
     lon_coord: np.array,
     lat_coord: np.array,
     show_tqdm: bool = False,
-    threshold=0.99,
+    threshold: ty.Optional[float] = 0.99,
     max_distance_km: ty.Union[str, float, int] = 'infer',
     **kw,
 ) -> ty.Tuple[ty.List[np.ndarray], ty.List[np.ndarray]]:
     """Build set of clusters and masks based on the weights (which should be a grid)'
 
     Args:
         weights (np.ndarray): normalized score data (values in [0,1])
-        lon_coord (np.array): all lon values
-        lat_coord (np.array): all lat values
+        lon_coord (np.array): all longitude values
+        lat_coord (np.array): all latitude values
         max_distance_km (ty.Union[str, float, int]): find an appropriate distance
             threshold for build_clusters' max_distance_km argument. If nothing is
             provided, make a guess based on the distance between grid cells.
             Defaults to 'infer'.
         show_tqdm (bool, optional): use verboose progressbar. Defaults to False.
+        threshold: float, min value of the passed weights. Defaults to 0.99.
 
     Returns:
         ty.List[ty.List[np.ndarray], ty.List[np.ndarray]]: Return two lists, containing the masks, and clusters respectively.
     """
 
     lon, lat = _check_input(weights, lon_coord, lat_coord)
     xy_data = np.array([lon.flatten(), lat.flatten()])
@@ -167,28 +168,30 @@
         **kw,
     )
 
     return masks, clusters
 
 
 def _check_input(data, lon_coord, lat_coord):
+    """Check for consistancy and if we need to convert the lon/lat coordinates to a meshgrid"""
     if len(lon_coord.shape) <= 1:
-        get_logger.warning('Expected lon and lat values, but got x, y values')
+        get_logger().warning('Expected lon and lat values, but got x, y values')
         # seperate x, y values, bad practice?
         lon, lat = np.meshgrid(lon_coord, lat_coord)
     else:
         lon, lat = lon_coord, lat_coord
 
     if data.shape != lon.shape or data.shape != lat.shape:
         message = f'Wrong input {data.shape} != {lon.shape, lat.shape}'
         raise ValueError(message)
     return lon, lat
 
 
 def _build_cluster_with_kw(lon, lat, show_tqdm=False, **cluster_kw):
+    """Overlapping logic between functions to get the masks and clusters"""
     masks = []
     clusters = [np.rad2deg(cluster) for cluster in build_clusters(**cluster_kw)]
     if lat.shape != lon.shape:
         raise ValueError(f'Got inconsistent input {lat.shape} != {lon.shape}')
     for cluster in clusters:
         mask = np.zeros(lat.shape, np.bool_)
         for s_x, s_y in tqdm(cluster, desc='fill_mask', disable=not show_tqdm):
```

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools/analyze/cmip_handler.py` & `optim_esm_tools-1.0.0/optim_esm_tools/analyze/cmip_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,42 @@
 # -*- coding: utf-8 -*-
-import optim_esm_tools as oet
-
 import os
 import xarray as xr
 
 import typing as ty
 from warnings import warn
 
-from optim_esm_tools.utils import deprecated
-
-from .globals import _CMIP_HANDLER_VERSION, _FOLDER_FMT
-from .xarray_tools import _native_date_fmt, _remove_any_none_times, detrend
-from optim_esm_tools.plotting.map_maker import MapMaker, make_title
+from .globals import _FOLDER_FMT
+import optim_esm_tools as oet
 from optim_esm_tools.analyze import tipping_criteria
 
 
-def transform_ds(
+def add_conditions_to_ds(
     ds: xr.Dataset,
     calculate_conditions: ty.Tuple[tipping_criteria._Condition] = None,
     condition_kwargs: ty.Mapping = None,
     variable_of_interest: ty.Tuple[str] = ('tas',),
-    max_time: ty.Optional[ty.Tuple[int, int, int]] = (2100, 1, 1),
-    min_time: ty.Optional[ty.Tuple[int, int, int]] = None,
-    strict: bool = True,
-    _time_var='time',
-    _detrend_type='linear',
-    _ma_window: int = 10,
+    _ma_window: int = None,
 ) -> xr.Dataset:
     """Transform the dataset to get it ready for handling in optim_esm_tools
 
     Args:
         ds (xr.Dataset): input dataset
         calculate_conditions (ty.Tuple[tipping_criteria._Condition], optional): Calculate the results of these tipping conditions. Defaults to None.
         condition_kwargs (ty.Mapping, optional): kwargs for the tipping conditions. Defaults to None.
         variable_of_interest (ty.Tuple[str], optional): Variables to handle. Defaults to ('tas',).
-        max_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to (2100, 1, 1).
-        min_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to None.
-        strict (bool, optional): raise errors on loading, if any. Defaults to True.
-        _time_var (str, optional): Name of the time dimention. Defaults to 'time'.
-        _detrend_type (str, optional): Type of detrending applied. Defaults to 'linear'.
         _ma_window (int, optional): Moving average window (assumed to be years). Defaults to 10.
 
     Raises:
         ValueError: If there are multiple tipping conditions with the same short_description
 
     Returns:
         xr.Dataset: The fully initiallized dataset
     """
+    _ma_window = _ma_window or oet.config.config['analyze']['moving_average_years']
     if calculate_conditions is None:
         calculate_conditions = (
             tipping_criteria.StartEndDifference,
             tipping_criteria.StdDetrended,
             tipping_criteria.MaxJump,
             tipping_criteria.MaxDerivitive,
             tipping_criteria.MaxJumpAndStd,
@@ -58,24 +44,14 @@
     if len(set(desc := (c.short_description for c in calculate_conditions))) != len(
         calculate_conditions
     ):
         raise ValueError(f'One or more non unique descriptions {desc}')
     if condition_kwargs is None:
         condition_kwargs = dict()
 
-    ds = _calculate_variables(
-        ds,
-        min_time,
-        max_time,
-        variable_of_interest,
-        strict,
-        _ma_window,
-        _detrend_type,
-        _time_var,
-    )
     for variable in oet.utils.to_str_tuple(variable_of_interest):
         for cls in calculate_conditions:
             condition = cls(**condition_kwargs, variable=variable)
             condition_array = condition.calculate(ds)
             condition_array = condition_array.assign_attrs(
                 dict(
                     short_description=cls.short_description,
@@ -87,151 +63,139 @@
     return ds
 
 
 @oet.utils.add_load_kw
 @oet.utils.timed()
 def read_ds(
     base: str,
-    variable_of_interest: ty.Tuple[str] = ('tas',),
+    variable_of_interest: ty.Tuple[str] = None,
     max_time: ty.Optional[ty.Tuple[int, int, int]] = (2100, 1, 1),
     min_time: ty.Optional[ty.Tuple[int, int, int]] = None,
     apply_transform: bool = True,
-    add_area: bool = True,
-    area_query_kwargs: ty.Optional[ty.Mapping] = None,
+    pre_process: bool = True,
     strict: bool = True,
     load: bool = False,
-    _ma_window: int = 10,
+    _ma_window: ty.Optional[int] = None,
     _cache: bool = True,
-    _file_name: str = 'merged.nc',
+    _file_name: str = None,
     **kwargs,
 ) -> xr.Dataset:
     """Read a dataset from a folder called "base".
 
     Args:
         base (str): Folder to load the data from
         variable_of_interest (ty.Tuple[str], optional): Variables to handle. Defaults to ('tas',).
         max_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to (2100, 1, 1).
         min_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to None.
         apply_transform: (bool, optional): Apply analysis specific postprocessing algoritms. Defaults to True.
-        add_area (bool, optional): Search for cell area information. Defaults to True.
+        pre_process (bool, optional): Should be true, this pre-processing of the data is required later on. Defaults to True.
         area_query_kwargs (ty.Mapping, optional): additionall keyword arguments for searching.
         strict (bool, optional): raise errors on loading, if any. Defaults to True.
         load (bool, optional): apply dataset.load to dataset directly. Defaults to False.
         _ma_window (int, optional): Moving average window (assumed to be years). Defaults to 10.
         _cache (bool, optional): cache the dataset with it's extra fields to alow faster (re)loading. Defaults to True.
+        _file_name (str, optional): name to match. Defaults to configs settings.
 
     kwargs:
         any kwargs are passed onto transfor_ds.
 
     Returns:
         xr.Dataset: An xarray dataset with the appropriate variables
     """
+    log = oet.config.get_logger()
+    _file_name = _file_name or oet.config.config['CMIP_files']['base_name']
+    _ma_window = _ma_window or oet.config.config['analyze']['moving_average_years']
+    data_path = os.path.join(base, _file_name)
+    variable_of_interest = (
+        variable_of_interest or oet.analyze.pre_process._read_variable_id(data_path)
+    )
+
+    if not isinstance(variable_of_interest, str):
+        raise ValueError('Only single vars supported')
     if kwargs:
-        oet.config.get_logger().error(f'Not really advised yet to call with {kwargs}')
+        log.error(f'Not really advised yet to call with {kwargs}')
         _cache = False
     if not apply_transform:
         # Don't cache the partial ds
         _cache = False
 
-    oet.config.get_logger().debug(f'read_ds {variable_of_interest}')
-    post_processed_file = _name_cache_file(
+    log.debug(f'read_ds {variable_of_interest}')
+    res_file = _name_cache_file(
         base,
         variable_of_interest,
         min_time,
         max_time,
         _ma_window,
-        _CMIP_HANDLER_VERSION,
     )
 
-    if os.path.exists(post_processed_file) and _cache:
-        return oet.analyze.io.load_glob(post_processed_file)
+    if os.path.exists(res_file) and _cache:
+        return oet.analyze.io.load_glob(res_file)
 
-    data_path = os.path.join(base, _file_name)
     if not os.path.exists(data_path):
         message = f'No dataset at {data_path}'
         if strict:
             raise FileNotFoundError(message)
         warn(message)
         return None
 
+    temp_file = os.path.join(base, 'temp_final.nc')
+    if pre_process:
+        data_path = oet.analyze.pre_process.pre_process(
+            source=data_path,
+            max_time=max_time,
+            min_time=min_time,
+            save_as=temp_file,
+            _ma_window=_ma_window,
+            variable_id=variable_of_interest,
+        )
+    else:
+        log.warning(
+            f'Not preprocessing file is dangerous, dimentions may differ wildly!'
+        )
     data_set = oet.analyze.io.load_glob(data_path, load=load)
-    data_set = oet.analyze.io.recast(data_set)
-    if add_area:
-        area_query_kwargs = area_query_kwargs or dict()
-        data_set = _add_area(data_set, strict, path=data_path, **area_query_kwargs)
+
+    if os.path.exists(temp_file):
+        # Maybe we can make this optional, but, for now, let's prevent double caching of
+        # res_file and temp_file
+        os.remove(temp_file)
 
     if apply_transform:
-        data_set = transform_ds(
+        data_set = add_conditions_to_ds(
             data_set,
             variable_of_interest=variable_of_interest,
-            max_time=max_time,
-            min_time=min_time,
             _ma_window=_ma_window,
-            strict=strict,
             **kwargs,
         )
 
     folders = base.split(os.sep)
 
     # start with -1 (for i==0)
     metadata = {k: folders[-i - 1] for i, k in enumerate(_FOLDER_FMT[::-1])}
-    metadata.update(
-        dict(path=base, file=post_processed_file, running_mean_period=_ma_window)
-    )
+    metadata.update(dict(path=base, file=res_file, running_mean_period=_ma_window))
 
     data_set.attrs.update(metadata)
 
     if _cache:
-        oet.config.get_logger().info(f'Write {post_processed_file}')
-        data_set.to_netcdf(post_processed_file)
-    return data_set
-
+        log.info(f'Write {res_file}')
+        data_set.to_netcdf(res_file)
 
-def _add_area(
-    data_set,
-    strict,
-    _change_logging=True,
-    **kw,
-):
-    import logging
-    import numpy as np
-
-    data_set = data_set.copy()
-    shape = len(data_set['y']), len(data_set['x'])
-
-    data_set['cell_area'] = (
-        ('y', 'x'),
-        np.ones(shape) * 180 * 360 / np.product(shape),
-    )
-    return data_set
-
-    if _change_logging:
-        # Intake-esm is so verbose...
-        logging.getLogger().setLevel(logging.ERROR)
-    try:
-        data_set = oet.analyze.query_metric.add_area_to_ds(data_set, **kw)
-    except oet.analyze.query_metric.NoMatchFoundError:
-        if strict:
-            # If you are really desperate pass method='brute_force'
-            raise
-    finally:
-        from optim_esm_tools.config import config
-
-        logging.getLogger().setLevel(config['log']['logging_level'].upper())
     return data_set
 
 
 def _name_cache_file(
     base,
     variable_of_interest,
     min_time,
     max_time,
     _ma_window,
-    version,
+    version=None,
 ):
+    """Get a file name that identifies the settings"""
+    version = version or oet.config.config['versions']['cmip_handler']
+    _ma_window = _ma_window or oet.config.config['analyze']['moving_average_years']
     path = os.path.join(
         base,
         f'{variable_of_interest}'
         f'_s{tuple(min_time) if min_time else ""}'
         f'_e{tuple(max_time) if max_time else ""}'
         f'_ma{_ma_window}'
         f'_optimesm_v{version}.nc',
@@ -243,54 +207,7 @@
         .replace('[', '')
         .replace(' ', '_')
         .replace(',', '')
         .replace('\'', '')
     )
     oet.config.get_logger().debug(f'got {normalized_path}')
     return normalized_path
-
-
-@oet.utils.timed()
-def _calculate_variables(
-    data_set,
-    min_time,
-    max_time,
-    variable_of_interest,
-    strict,
-    _ma_window,
-    _detrend_type,
-    _time_var,
-):
-    if min_time or max_time:
-        time_slice = [
-            _native_date_fmt(data_set[_time_var], d) if d is not None else None
-            for d in [min_time, max_time]
-        ]
-        data_set = data_set.sel(**{_time_var: slice(*time_slice)})
-
-    # Detrend and run_mean on the fly
-    for variable in variable_of_interest:
-        if (ds_len := len(data_set[variable])) < _ma_window:
-            message = f'This data set is shorter {ds_len} than the moving average window ({_ma_window})'
-            if strict:
-                raise ValueError(message)
-            oet.config.get_logger().warning(message)
-
-        # NB these are DataArrays not Datasets!
-        run_mean = data_set[variable].rolling(time=_ma_window, center=True).mean()
-        kw = dict(dimension=_time_var, detrend_type=_detrend_type)
-        detrended = detrend(data_set[variable], **kw)
-        detrended_run_mean = detrend(_remove_any_none_times(run_mean, _time_var), **kw)
-
-        for det in detrended, detrended_run_mean:
-            det.attrs.update(data_set[variable].attrs.copy())
-
-        data_set[f'{variable}_run_mean_{_ma_window}'] = run_mean
-        data_set[f'{variable}_detrend'] = detrended
-        data_set[f'{variable}_detrend_run_mean_{_ma_window}'] = detrended_run_mean
-    return data_set
-
-
-# class MapMaker(MapMaker):
-#     @depricated
-#     def __init__(self, *a, **kw):
-#         return super().__init__(*a, **kw)
```

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools/analyze/find_matches.py` & `optim_esm_tools-1.0.0/optim_esm_tools/analyze/find_matches.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools/analyze/region_finding.py` & `optim_esm_tools-1.0.0/optim_esm_tools/analyze/region_finding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import optim_esm_tools as oet
 from optim_esm_tools.plotting.map_maker import MapMaker, HistoricalMapMaker
 from optim_esm_tools.analyze import tipping_criteria
-from optim_esm_tools.analyze.cmip_handler import transform_ds, read_ds
+from optim_esm_tools.analyze.cmip_handler import read_ds
 from optim_esm_tools.analyze.clustering import (
     build_cluster_mask,
     build_weighted_cluster,
 )
 from optim_esm_tools.plotting.plot import setup_map, _show
-from optim_esm_tools.analyze.tipping_criteria import var_to_perc, rank2d
+from optim_esm_tools.analyze.tipping_criteria import rank2d
 from optim_esm_tools.analyze.find_matches import base_from_path
 
-
-import os
-
 import numpy as np
-import xarray as xr
-
 import matplotlib.pyplot as plt
 import logging
+import xarray as xr
 
 import typing as ty
 from functools import wraps
 import inspect
 import matplotlib.pyplot as plt
 import immutabledict
 
@@ -30,31 +26,26 @@
 # >>> scipy.stats.norm.cdf(3)
 # 0.9986501019683699
 # >> scipy.stats.norm.cdf(2)
 # 0.9772498680518208
 _two_sigma_percent = 97.72498680518208
 
 
-# TODO this has too many hardcoded defaults
-def mask_xr_ds(data_set, da_mask, masked_dims=('x', 'y'), keep_dims=('time',)):
+def mask_xr_ds(data_set, da_mask, masked_dims=None):
+    if masked_dims is None:
+        masked_dims = oet.config.config['analyze']['lon_lat_dim'].split(',')
+
     ds_start = data_set.copy()
-    no_drop = set(masked_dims) | set(keep_dims)
-    for spurious_dim in set(data_set.dims) - no_drop:
-        message = (
-            f'Spurious coordinate {spurious_dim} dropping for safety. Keep {no_drop}'
-        )
-        oet.config.get_logger().warn(message)
-        data_set = data_set.mean(spurious_dim)
     for k, data_array in data_set.data_vars.items():
         if all(dim in list(data_array.dims) for dim in masked_dims):
             # First dim is time?
-            if 'time' == data_array.dims[0] and data_array.shape[1:] == da_mask.T.shape:
-                da_mask = da_mask.T
-            elif data_array.shape == da_mask.T.shape:
-                da_mask = da_mask.T
+            if (
+                'time' == data_array.dims[0] and data_array.shape[1:] == da_mask.T.shape
+            ) or data_array.shape == da_mask.T.shape:
+                raise ValueError(f'Please make "{k}" lat, lon, now "{data_array.dims}"')
             da = data_set[k].where(da_mask, drop=False)
             da = da.assign_attrs(ds_start[k].attrs)
             data_set[k] = da
     data_set = data_set.assign_attrs(ds_start.attrs)
     return data_set
 
 
@@ -103,50 +94,43 @@
     show: bool = True
 
     criteria = (tipping_criteria.StdDetrended, tipping_criteria.MaxJump)
     extra_opt = None
 
     def __init__(
         self,
-        variable='tas',
+        variable=None,
         path=None,
         data_set=None,
-        transform=True,
         save_kw=None,
         extra_opt=None,
         read_ds_kw=None,
     ) -> None:
-        read_ds_kw = dict() if read_ds_kw is None else read_ds_kw
-        if path is None:
-            if transform:
-                self.log.warning(
-                    f'Best is to start {self.__class__.__name__} from a synda path'
-                )
-                self.data_set = transform_ds(data_set)
-            else:
-                self.data_set = data_set
-        else:
+        read_ds_kw = read_ds_kw or dict()
+        if path is None and data_set:
+            self.data_set = data_set
+        elif path:
             self.data_set = read_ds(path, **read_ds_kw)
+        else:
+            raise ValueError('Both path and data_set are None?!')
 
-        if save_kw is None:
-            save_kw = dict(
-                save_in='./',
-                file_types=(
-                    'png',
-                    'pdf',
-                ),
-                skip=False,
-                sub_dir=None,
-            )
-        if extra_opt is None:
-            extra_opt = dict(show_basic=True)
+        save_kw = save_kw or dict(
+            save_in='./',
+            file_types=(
+                'png',
+                'pdf',
+            ),
+            skip=False,
+            sub_dir=None,
+        )
+        extra_opt = extra_opt or dict(show_basic=True)
         extra_opt.update(dict(read_ds_kw=read_ds_kw))
         self.extra_opt = extra_opt
         self.save_kw = save_kw
-        self.variable = variable
+        self.variable = variable or self.data_set.attrs.get('variable_id', 'NO_VAR_ID!')
 
     @property
     def log(self):
         if self._logger is None:
             self._logger = oet.config.get_logger()
         return self._logger
 
@@ -185,19 +169,30 @@
             if mask is None or not np.sum(mask):
                 return 0
         except Exception as e:
             print(mask)
             raise ValueError(
                 mask,
             ) from e
-        if self.data_set['cell_area'].shape == mask.shape:
-            return self.data_set['cell_area'].values[mask]
-        if self.data_set['cell_area'].shape == mask.T.shape:
-            return self.data_set['cell_area'].values[mask.T]
-        raise ValueError
+        self.check_shape(mask)
+        return self.data_set['cell_area'].values[mask]
+
+    def check_shape(
+        self, data: ty.Union[np.ndarray, xr.DataArray], compare_with='cell_area'
+    ):
+        shape_should_be = self.data_set[compare_with].shape
+        if data.shape == shape_should_be:
+            return
+        error_message = f'Got {data.shape}, expected {shape_should_be}'
+        if name := getattr(data, 'name', False):
+            error_message = f'For {name}: ' + error_message
+        if dims := getattr(data, 'dims', False):
+            error_message = f'{error_message}. Dims are {dims}, expected'
+        error_message += f'for {self.data_set[compare_with].dims}'
+        raise ValueError(error_message)
 
     @apply_options
     def mask_is_large_enough(self, mask, min_area_sq=0):
         return self.mask_area(mask).sum() >= min_area_sq
 
     def filter_masks_and_clusters(self, masks_and_clusters):
         if not len(masks_and_clusters[0]):
@@ -208,63 +203,80 @@
             if self.mask_is_large_enough(m):
                 ret_m.append(m)
                 ret_c.append(c)
 
         self.log.warn(f'Keeping {len(ret_m)}/{len(masks_and_clusters[0])} of masks')
         return ret_m, ret_c
 
+    @plt_show
+    def summarize_mask(self, mask, m_i):
+        self._summarize_mask(mask)
+        plt.suptitle(self.title + f' cluster {m_i}')
+        self.save(f'{self.title_label}_cluster_{m_i}')
+
+    def _summarize_mask(self, mask, plot=None):
+        axes = oet.plotting.map_maker.summarize_mask(self.data_set, mask, plot=plot)
+        return axes
+
+    def make_mask_figures(self, masks):
+        for m_i, mask in enumerate(masks):
+            if np.sum(mask) == 0:
+                continue
+            self.summarize_mask(mask, m_i)
+
 
 class MaxRegion(RegionExtractor):
     def get_masks(self) -> dict:
         """Get mask for max of ii and iii and a box arround that"""
-        labels = [crit.short_description for crit in self.criteria]
 
         def _val(label):
             return self.data_set[label].values
 
         def _max(label):
             return _val(label)[~np.isnan(_val(label))].max()
 
-        masks = {label: _val(label) == _max(label) for label in labels}
+        masks = [_val(label) == _max(label) for label in self._labels]
         return masks, [None for _ in range(len(masks))]
 
     @apply_options
     def filter_masks_and_clusters(self, masks_and_clusters, min_area_km_sq=0):
         """Wrap filter to work on dicts"""
         if min_area_km_sq:
             message = f'Calling {self.__class__.__name__}.filter_masks_and_clusters is nonsensical as masks are single grid cells'
-            oet.config.get_logger().warning(message)
+            self.log.warning(message)
         return masks_and_clusters
 
     @plt_show
     def plot_masks(self, masks, ax=None, legend=True):
         masks = masks[0]
         self._plot_masks(masks=masks, ax=ax, legend=legend)
         self.save(f'{self.title_label}_map_maxes_{"-".join(self.labels)}')
 
+        self.make_mask_figures(masks)
+
     @apply_options
     def _plot_masks(self, masks, ax=None, legend=True):
         points = {}
-        for key, mask_2d in masks.items():
+        for key, mask_2d in zip(self._labels, masks):
             points[key] = self._mask_to_coord(mask_2d)
         if ax is None:
             oet.plotting.plot.setup_map()
             ax = plt.gca()
         for i, (label, xy) in enumerate(zip(self.labels, points.values())):
             ax.scatter(*xy, marker='oxv^'[i], label=f'Maximum {label}')
         if legend:
             ax.legend(**oet.utils.legend_kw())
         plt.suptitle(self.title, y=0.95)
         plt.ylim(-90, 90)
         plt.xlim(-180, 180)
 
     def _mask_to_coord(self, mask_2d):
         arg_mask = np.argwhere(mask_2d)[0]
-        x = self.data_set.x[arg_mask[1]]
-        y = self.data_set.y[arg_mask[0]]
+        x = self.data_set.lon[arg_mask[1]]
+        y = self.data_set.lat[arg_mask[0]]
         return x, y
 
     def _plot_basic_map(self):
         mm = MapMaker(self.data_set)
         axes = mm.plot_selected(items=self.labels)
         masks = self.get_masks()
         for ax in axes:
@@ -277,35 +289,41 @@
         res = self._plot_mask_time_series(masks, time_series_joined=time_series_joined)
         if time_series_joined:
             self.save(f'{self.title_label}_time_series_maxes_{"-".join(self.labels)}')
         return res
 
     @apply_options
     def _plot_mask_time_series(
-        self, masks_and_clusters, time_series_joined=True, only_rm=False, axes=None
+        self,
+        masks_and_clusters,
+        time_series_joined=True,
+        only_rm=False,
+        axes=None,
+        _ma_window=None,
     ):
+        _ma_window = _ma_window or oet.config.config['analyze']['moving_average_years']
         masks = masks_and_clusters[0]
         legend_kw = oet.utils.legend_kw(
             loc='upper left', bbox_to_anchor=None, mode=None, ncol=2
         )
-        for label, mask_2d in zip(self.labels, masks.values()):
+        for label, mask_2d in zip(self._labels, masks):
             x, y = self._mask_to_coord(mask_2d)
             plot_labels = {
                 f'{self.variable}': f'{label} at {x:.1f}:{y:.1f}',
                 f'{self.variable}_detrend': f'{label} at {x:.1f}:{y:.1f}',
-                f'{self.variable}_detrend_run_mean_10': f'$RM_{{10}}$ {label} at {x:.1f}:{y:.1f}',
-                f'{self.variable}_run_mean_10': f'$RM_{{10}}$ {label} at {x:.1f}:{y:.1f}',
+                f'{self.variable}_detrend_run_mean_{_ma_window}': f'$RM_{{{_ma_window}}}$ {label} at {x:.1f}:{y:.1f}',
+                f'{self.variable}_run_mean_{_ma_window}': f'$RM_{{{_ma_window}}}$ {label} at {x:.1f}:{y:.1f}',
             }
             argwhere = np.argwhere(mask_2d)[0]
-            ds_sel = self.data_set.isel(x=argwhere[1], y=argwhere[0])
+            ds_sel = self.data_set.isel(lat=argwhere[0], lon=argwhere[1])
             mm_sel = MapMaker(ds_sel)
             axes = mm_sel.time_series(
                 variable=self.variable,
                 other_dim=(),
-                interval=False,
+                show_std=False,
                 labels=plot_labels,
                 axes=axes,
                 only_rm=only_rm,
             )
             if time_series_joined is False:
                 axes = None
                 plt.suptitle(f'Max. {label} {self.title}', y=0.95)
@@ -314,27 +332,31 @@
         if not time_series_joined:
             return
 
         for ax in axes:
             ax.legend(**legend_kw)
         plt.suptitle(f'Max. {"-".join(self.labels)} {self.title}', y=0.95)
 
+    @property
+    def _labels(self):
+        return [crit.short_description for crit in self.criteria]
+
 
 class Percentiles(RegionExtractor):
     @oet.utils.check_accepts(
         accepts=immutabledict.immutabledict(cluster_method=('weighted', 'masked'))
     )
     @apply_options
     def get_masks(self, cluster_method='masked') -> dict:
         if cluster_method == 'weighted':
             masks, clusters = self._get_masks_weighted()
         else:
             masks, clusters = self._get_masks_masked()
-        if len(masks) and masks[0].shape == self.data_set['cell_area'].values.T.shape:
-            masks = [m.T for m in masks]
+        if len(masks):
+            self.check_shape(masks[0])
         return masks, clusters
 
     @apply_options
     def _get_masks_weighted(
         self,
         min_weight=0.95,
         lon_lat_dim=('lon', 'lat'),
@@ -349,16 +371,16 @@
             sums.append(vals)
 
         tot_sum = np.zeros_like(sums[0])
         for s in sums:
             tot_sum += s
         tot_sum /= len(sums)
 
-        if tot_sum.T.shape == self.data_set[lon_lat_dim[0]].shape:
-            tot_sum = tot_sum.T
+        self.check_shape(tot_sum)
+
         masks, clusters = build_weighted_cluster(
             weights=tot_sum,
             lon_coord=self.data_set[lon_lat_dim[0]].values,
             lat_coord=self.data_set[lon_lat_dim[1]].values,
             threshold=min_weight,
         )
         return masks, clusters
@@ -377,16 +399,17 @@
             arr_no_nan = arr[~np.isnan(arr)]
             thr = np.percentile(arr_no_nan, percentiles)
             masks.append(arr >= thr)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
-        if all_mask.T.shape == self.data_set[lon_lat_dim[0]].shape:
-            all_mask = all_mask.T
+
+        self.check_shape(all_mask)
+
         masks, clusters = build_cluster_mask(
             all_mask,
             lon_coord=self.data_set[lon_lat_dim[0]].values,
             lat_coord=self.data_set[lon_lat_dim[1]].values,
         )
         return masks, clusters
 
@@ -398,14 +421,16 @@
         self._plot_masks(
             masks_and_clusters=masks_and_clusters,
             ax=ax,
             legend=legend,
         )
         self.save(f'{self.title_label}_map_clusters_{"-".join(self.labels)}')
 
+        self.make_mask_figures(masks_and_clusters[0])
+
     @apply_options
     def _plot_masks(
         self,
         masks_and_clusters,
         scatter_medians=True,
         ax=None,
         legend=True,
@@ -413,26 +438,27 @@
         cluster_kw=None,
     ):
         ds_dummy = self.data_set.copy()
         masks, clusters = masks_and_clusters
         all_masks = np.zeros(ds_dummy['cell_area'].shape, np.float64)
         all_masks[:] = np.nan
         for m, _ in zip(masks, clusters):
-            if all_masks.shape == m.T.shape:
-                m = m.T
+            self.check_shape(m)
             all_masks[m] = self.mask_area(m).sum()
 
         if ax is None:
             setup_map()
             ax = plt.gca()
+
+        # Remember, cell_area is in m^2, hence the 1e6 below. Should we get this from the attrs?
         if mask_cbar_kw is None:
             mask_cbar_kw = dict(extend='neither', label='Area per cluster [km$^2$]')
         mask_cbar_kw.setdefault('orientation', 'horizontal')
 
-        ds_dummy['area_square'] = (ds_dummy['cell_area'].dims, all_masks)
+        ds_dummy['area_square'] = (ds_dummy['cell_area'].dims, all_masks / 1e6)
 
         ds_dummy['area_square'].plot(cbar_kwargs=mask_cbar_kw, vmin=0, extend='neither')
         plt.title('')
         if scatter_medians:
             if cluster_kw is None:
                 cluster_kw = dict()
             for m_i, cluster in enumerate(clusters):
@@ -474,40 +500,45 @@
         )
         if time_series_joined and masks_and_clusters:
             self.save(f'{self.title_label}_time_series_all_clusters')
         return res
 
     @apply_options
     def _plot_mask_time_series(
-        self, masks_and_clusters, time_series_joined=True, only_rm=None, axes=None
+        self,
+        masks_and_clusters,
+        time_series_joined=True,
+        only_rm=None,
+        axes=None,
+        _ma_window=None,
     ):
         if only_rm is None:
             only_rm = (
                 True
                 if (len(masks_and_clusters[0]) > 1 and time_series_joined)
                 else False
             )
+        _ma_window = _ma_window or oet.config.config['analyze']['moving_average_years']
         masks, clusters = masks_and_clusters
         legend_kw = oet.utils.legend_kw(
             loc='upper left', bbox_to_anchor=None, mode=None, ncol=4
         )
         for m_i, (mask, cluster) in enumerate(zip(masks, clusters)):
             x, y = np.median(cluster, axis=0)
             plot_labels = {
                 f'{self.variable}': f'Cluster {m_i} near ~{x:.1f}:{y:.1f}',
                 f'{self.variable}_detrend': f'Cluster {m_i} near ~{x:.1f}:{y:.1f}',
-                f'{self.variable}_detrend_run_mean_10': f'Cluster {m_i} $RM_{{10}}$ near ~{x:.1f}:{y:.1f}',
-                f'{self.variable}_run_mean_10': f'Cluster {m_i} $RM_{{10}}$ near ~{x:.1f}:{y:.1f}',
+                f'{self.variable}_detrend_run_mean_{_ma_window}': f'Cluster {m_i} $RM_{{{_ma_window}}}$ near ~{x:.1f}:{y:.1f}',
+                f'{self.variable}_run_mean_{_ma_window}': f'Cluster {m_i} $RM_{{{_ma_window}}}$ near ~{x:.1f}:{y:.1f}',
             }
             ds_sel = mask_xr_ds(self.data_set.copy(), mask)
             mm_sel = MapMaker(ds_sel)
             axes = mm_sel.time_series(
                 variable=self.variable,
-                other_dim=('x', 'y'),
-                interval=True,
+                show_std=True,
                 labels=plot_labels,
                 axes=axes,
                 only_rm=only_rm,
             )
             if time_series_joined == False:
                 axes = None
                 plt.suptitle(f'Cluster. {m_i} {self.title}', y=0.95)
@@ -526,16 +557,15 @@
     @apply_options
     def get_masks(
         self,
         percentiles_historical=_two_sigma_percent,
         read_ds_kw=None,
         lon_lat_dim=('lon', 'lat'),
     ) -> dict:
-        if read_ds_kw is None:
-            read_ds_kw = dict()
+        read_ds_kw = read_ds_kw or dict()
         for k, v in dict(min_time=None, max_time=None).items():
             read_ds_kw.setdefault(k, v)
 
         historical_ds = self.get_historical_ds(read_ds_kw=read_ds_kw)
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
@@ -547,27 +577,20 @@
             )
             masks.append(arr >= thr)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
 
-        if all_mask.T.shape == self.data_set[lon_lat_dim[0]].shape:
-            all_mask = all_mask.T
-        assert all_mask.shape == self.data_set[lon_lat_dim[0]].shape, (
-            all_mask.shape,
-            self.data_set[lon_lat_dim[0]].shape,
-        )
+        self.check_shape(all_mask)
         masks, clusters = build_cluster_mask(
             all_mask,
             lon_coord=self.data_set[lon_lat_dim[0]].values,
             lat_coord=self.data_set[lon_lat_dim[1]].values,
         )
-        if len(masks) and masks[0].shape == self.data_set['cell_area'].values.T.shape:
-            masks = [m.T for m in masks]
         return masks, clusters
 
     @apply_options
     def find_historical(
         self,
         match_to='piControl',
         look_back_extra=0,
@@ -576,18 +599,18 @@
     ):
         from optim_esm_tools.config import config
 
         base = base_from_path(
             self.data_set.attrs['path'], look_back_extra=look_back_extra
         )
 
-        search = oet.cmip_files.find_matches.folder_to_dict(self.data_set.attrs['path'])
+        search = oet.analyze.find_matches.folder_to_dict(self.data_set.attrs['path'])
         search['activity_id'] = 'CMIP'
         if search['experiment_id'] == match_to:
-            raise NotImplementedError()
+            raise NotImplementedError(f'Cannot match {match_to} to itself!')
         search['experiment_id'] = match_to
         if search_kw:
             search.update(search_kw)
         if query_updates is None:
             query_updates = [
                 dict(),
                 dict(variant_label='*'),
@@ -598,23 +621,22 @@
 
         for try_n, update_query in enumerate(query_updates):
             if try_n:
                 self.log.warning(
                     f'No results after {try_n} try, retying with {update_query}'
                 )
             search.update(update_query)
-            this_try = oet.cmip_files.find_matches.find_matches(base, **search)
+            this_try = oet.analyze.find_matches.find_matches(base, **search)
             if this_try:
                 return this_try
         raise RuntimeError(f'Looked for {search}, in {base} found nothing')
 
     @apply_options
     def get_historical_ds(self, read_ds_kw=None, **kw):
-        if read_ds_kw is None:
-            read_ds_kw = dict()
+        read_ds_kw = read_ds_kw or dict()
         for k, v in dict(min_time=None, max_time=None).items():
             read_ds_kw.setdefault(k, v)
         historical_path = self.find_historical(**kw)[0]
         return read_ds(historical_path, **read_ds_kw)
 
 
 class ProductPercentiles(Percentiles):
@@ -626,31 +648,29 @@
     @apply_options
     def get_masks(self, cluster_method='masked') -> dict:
         """Get mask for max of ii and iii and a box arround that"""
         if cluster_method == 'weighted':
             masks, clusters = self._get_masks_weighted()
         else:
             masks, clusters = self._get_masks_masked()
-        if len(masks) and masks[0].shape == self.data_set['cell_area'].values.T.shape:
-            masks = [m.T for m in masks]
+        if len(masks):
+            self.check_shape(masks[0])
         return masks, clusters
 
     @apply_options
     def _get_masks_weighted(self, min_weight=0.95, lon_lat_dim=('lon', 'lat')):
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         ds = self.data_set.copy()
         combined_score = np.ones_like(ds[labels[0]].values)
 
         for label in labels:
             combined_score *= rank2d(ds[label].values)
-
-        if combined_score.T.shape == self.data_set[lon_lat_dim[0]].shape:
-            combined_score = combined_score.T
+        self.check_shape(combined_score)
         masks, clusters = build_weighted_cluster(
             weights=combined_score,
             lon_coord=self.data_set[lon_lat_dim[0]].values,
             lat_coord=self.data_set[lon_lat_dim[1]].values,
             threshold=min_weight,
         )
         return masks, clusters
@@ -667,32 +687,30 @@
         combined_score = np.ones_like(ds[labels[0]].values)
         for label in labels:
             combined_score *= rank2d(ds[label].values)
 
         # Combined score is fraction, not percent!
         all_mask = combined_score > (product_percentiles / 100)
 
-        if all_mask.T.shape == self.data_set[lon_lat_dim[0]].shape:
-            all_mask = all_mask.T
+        self.check_shape(all_mask)
 
         masks, clusters = build_cluster_mask(
             all_mask,
             lon_coord=self.data_set[lon_lat_dim[0]].values,
             lat_coord=self.data_set[lon_lat_dim[1]].values,
         )
         return masks, clusters
 
 
 class LocalHistory(PercentilesHistory):
     @apply_options
     def get_masks(
         self, n_times_historical=4, read_ds_kw=None, lon_lat_dim=('lon', 'lat')
     ) -> dict:
-        if read_ds_kw is None:
-            read_ds_kw = dict()
+        read_ds_kw = read_ds_kw or dict()
         for k, v in dict(min_time=None, max_time=None).items():
             read_ds_kw.setdefault(k, v)
 
         historical_ds = self.get_historical_ds(read_ds_kw=read_ds_kw)
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
@@ -706,30 +724,31 @@
             mask_no_std = (arr_historical == 0) & (arr > 0)
             masks.append(mask_divide | mask_no_std)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
 
-        if all_mask.T.shape == self.data_set[lon_lat_dim[0]].shape:
-            all_mask = all_mask.T
+        self.check_shape(all_mask)
+
         masks, clusters = build_cluster_mask(
             all_mask,
             lon_coord=self.data_set[lon_lat_dim[0]].values,
             lat_coord=self.data_set[lon_lat_dim[1]].values,
         )
         return masks, clusters
 
     @apply_options
-    def _plot_basic_map(self, normalizations=None, read_ds_kw=None):
-        if read_ds_kw is None:
-            read_ds_kw = dict()
+    def _plot_basic_map(self, historical_normalizations=None, read_ds_kw=None):
+        read_ds_kw = read_ds_kw or dict()
         for k, v in dict(min_time=None, max_time=None).items():
             read_ds_kw.setdefault(k, v)
         ds_historical = self.get_historical_ds(read_ds_kw=read_ds_kw)
 
         mm = HistoricalMapMaker(
-            self.data_set, ds_historical=ds_historical, normalizations=normalizations
+            self.data_set,
+            ds_historical=ds_historical,
+            normalizations=historical_normalizations,
         )
         mm.plot_selected()
         plt.suptitle(self.title, y=0.95)
         return mm
```

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools/analyze/tipping_criteria.py` & `optim_esm_tools-1.0.0/optim_esm_tools/analyze/tipping_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     def calculate(self, data_set):
         return running_mean_diff(
             data_set,
             variable=self.variable,
             time_var=self.time_var,
             naming='{variable}_run_mean_{running_mean}',
             running_mean=self.running_mean,
-            # TODO
             # Pass kw arguments on? I think not
             _t_0_date=None,
             _t_1_date=None,
             **self.defaults,
         )
```

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools/config.py` & `optim_esm_tools-1.0.0/optim_esm_tools/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else:
     _warn_later = True
     config_path = os.path.join(root_folder, 'optim_esm_tools', 'optim_esm_conf.ini')
 
 config = configparser.ConfigParser()
 config.sections()
 config.read(config_path)
-
+# oet.config.config.read_dict({'boo':{'bar':'bla'}})
 _logger = {}
 
 
 def get_logger(name='oet'):
     if name not in _logger:
         logging.basicConfig(
             level=getattr(logging, config['log']['logging_level'].upper()),
```

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools/plotting/map_maker.py` & `optim_esm_tools-1.0.0/optim_esm_tools/plotting/map_maker.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,54 +6,51 @@
 import typing as ty
 import collections
 from warnings import warn
 
 import matplotlib.pyplot as plt
 
 from immutabledict import immutabledict
-from .plot import default_variable_labels
+from .plot import *
+from matplotlib.colors import LogNorm
 
 # import xrft
 
 from optim_esm_tools.analyze.globals import _SECONDS_TO_YEAR
 from optim_esm_tools.analyze import tipping_criteria
 
 
 class MapMaker(object):
     data_set: xr.Dataset
     labels = tuple('i ii iii iv v vi vii viii ix x'.split())
     kw: ty.Mapping
     contitions: ty.Mapping
+    normalizations: ty.Optional[ty.Mapping] = None
+    _cache: bool = False
 
     def __init__(
         self,
         data_set: xr.Dataset,
         normalizations: ty.Union[None, ty.Mapping, ty.Iterable] = None,
         **conditions,
     ):
         self.data_set = data_set
         self.set_kw()
         self.set_conditions(**conditions)
         if normalizations is not None:
             self.set_normalizations(normalizations)
 
     def set_kw(self):
-        import cartopy.crs as ccrs
-
         self.kw = immutabledict(
             fig=dict(dpi=200, figsize=(14, 10)),
             title=dict(fontsize=12),
             gridspec=dict(hspace=0.3),
             cbar=dict(orientation='horizontal', extend='both'),
-            plot=dict(transform=ccrs.PlateCarree()),
-            subplot=dict(
-                projection=ccrs.PlateCarree(
-                    central_longitude=0.0,
-                ),
-            ),
+            plot=dict(transform=get_cartopy_projection()),
+            subplot=dict(projection=get_cartopy_projection()),
         )
 
     def set_conditions(self, **condition_kwargs):
         conditions = [
             cls(**condition_kwargs)
             for cls in [
                 tipping_criteria.StartEndDifference,
@@ -65,18 +62,14 @@
         ]
 
         self.conditions = {
             label: condition for label, condition in zip(self.labels, conditions)
         }
         self.labels = tuple(self.conditions.keys())
 
-    normalizations: ty.Optional[ty.Mapping] = None
-
-    _cache: bool = False
-
     def get_normalizations(self, normalizations=None):
         normalizations_start = (
             normalizations.copy() if normalizations is not None else None
         )
 
         if normalizations is None and self.normalizations is not None:
             # once set, they should be retrievable
@@ -192,243 +185,184 @@
 
     def __getattr__(self, item):
         if item in self.conditions:
             condition = self.conditions[item]
             return self.data_set[condition.short_description]
         return self.__getattribute__(item)
 
-    @staticmethod
-    def _ts_single(time_val, mean, std, plot_kw, fill_kw):
-        if fill_kw is None:
-            fill_kw = dict(alpha=0.4, step='mid')
-        l = mean.plot(**plot_kw)
-
-        if std is not None:
-            # TODO, make this more elegant!
-            # import cftime
-            # plt.fill_between(   [cftime.real_datetime(dd.year, dd.month, dd.day) for dd in time_val], mean - std, mean+std, **fill_kw)
-
-            (mean - std).plot(color=l[0]._color, alpha=0.4)
-            (mean + std).plot(color=l[0]._color, alpha=0.4)
-
     def _ts(
         self,
         variable,
-        ds=None,
-        time='time',
-        other_dim=(),
-        running_mean=10,
-        fill_kw=None,
-        labels=dict(),
+        running_mean=None,
+        no_rm=False,
         only_rm=False,
-        **plot_kw,
+        labels=None,
+        **kw,
     ):
-        if ds is None:
-            ds = self.data_set
-        if not only_rm:
-            mean, std = self._mean_and_std(ds, variable, other_dim)
-            # return mean, std
-            plot_kw['label'] = labels.get(variable, variable)
-            self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
-
-        mean, std = self._mean_and_std(
-            ds, f'{variable}_run_mean_{running_mean}', other_dim
-        )
-        plot_kw['label'] = labels.get(
-            f'{variable}_run_mean_{running_mean}',
-            f'{variable} running mean {running_mean}',
-        )
-        self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
-
-        plt.ylabel(f'{self.variable_name(variable)} [{self.unit(variable)}]')
-        plt.legend()
-        plt.title('')
+        variable = variable or self.variable
+        rm = running_mean or oet.config.config['analyze']['moving_average_years']
+        _vars = [variable, f'{variable}_run_mean_{rm}']
+        assert no_rm + only_rm < 2, 'Cannot show nothing?!'
+
+        if isinstance(labels, ty.Mapping):
+            labels = [labels.get(k, k) for k in _vars]
+
+        if only_rm or no_rm:
+            keep_idx = slice(0, 1) if no_rm else slice(-1, None)
+            _vars = _vars[keep_idx]
+            if labels is not None:
+                labels = labels[keep_idx]
+
+        self._ts_for_vars(_vars, labels=labels, **kw)
+
+    def _ts_for_vars(self, variables, labels=None, **plot_kw):
+        variables = oet.utils.to_str_tuple(variables)
+        labels = labels or [None] * len(variables)
+        if not len(variables) == len(labels):
+            raise ValueError(
+                f'Inconsistent number of vars and labels {variables, labels}'
+            )
+        plot_kw.setdefault('ds', self.data_set)
+        assert 'ds' in plot_kw
+        for v, l in zip(variables, labels):
+            l = l or default_variable_labels().get(v, v)
+            plot_simple(var=v, label=l, **plot_kw)
 
     def _det_ts(
         self,
         variable,
-        ds=None,
-        time='time',
-        other_dim=(),
-        running_mean=10,
-        fill_kw=None,
-        labels=dict(),
-        only_rm=False,
         **plot_kw,
     ):
-        if ds is None:
-            ds = self.data_set
-        if not only_rm:
-            mean, std = self._mean_and_std(ds, f'{variable}_detrend', other_dim)
-            plot_kw['label'] = labels.get(
-                f'{variable}_detrend', f'detrended {variable}'
-            )
-            self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
-
-        mean, std = self._mean_and_std(
-            ds, f'{variable}_detrend_run_mean_{running_mean}', other_dim
-        )
-        plot_kw['label'] = labels.get(
-            f'{variable}_detrend_run_mean_{running_mean}',
-            f'detrended {variable} running mean {running_mean}',
+        self._ts(
+            f'{variable}_detrend',
+            **plot_kw,
         )
-        self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
-        plt.ylabel(f'Detrend {self.variable_name(variable)} [{self.unit(variable)}]')
-        plt.legend()
-        plt.title('')
 
     def _ddt_ts(
         self,
         variable,
         ds=None,
         time='time',
-        other_dim=(),
-        running_mean=10,
-        fill_kw=None,
-        labels=dict(),
-        only_rm=False,
+        running_mean=None,
         **plot_kw,
     ):
-        if ds is None:
-            ds = self.data_set
-        variable_rm = f'{variable}_run_mean_{running_mean}'
-
-        da = ds[variable]
-        da_rm = ds[variable_rm]
-
-        if other_dim:
-            da = da.mean(other_dim)
-            da_rm = da_rm.mean(other_dim)
-        if not only_rm:
+        ds = (ds or self.data_set).copy()
+
+        rm = running_mean or oet.config.config['analyze']['moving_average_years']
+        var_rm = f'{variable}_run_mean_{rm}'
+
+        for var in variable, var_rm:
             # Dropna should take care of any nones in the data-array
-            dy_dt = da.dropna(time).differentiate(time)
+            da = ds[var]
+            # non_time_dim = set(da.dims) - {'time'}
+            # if non_time_dim:
+            #     da = da.mean(non_time_dim)
+            dy_dt = da.differentiate(time)
             dy_dt *= _SECONDS_TO_YEAR
-            # mean, std = self._mean_and_std(dy_dt, variable=None, other_dim=other_dim)
-            # plot_kw['label'] = variable
-            # self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
-            label = labels.get(variable, variable)
-            dy_dt.plot(label=label, **plot_kw)
-
-        dy_dt_rm = da_rm.dropna(time).differentiate(time)
-        dy_dt_rm *= _SECONDS_TO_YEAR
-        label = f"{labels.get(variable_rm, f'{variable} running mean {running_mean}')}"
-        dy_dt_rm.plot(label=label, **plot_kw)
-        # mean, std = self._mean_and_std(dy_dt_rm, variable=None, other_dim=other_dim)
-        # plot_kw['label'] = variable
-        # self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
-
-        plt.ylim(dy_dt_rm.min() / 1.05, dy_dt_rm.max() * 1.05)
-        plt.ylabel(
-            f'$\partial \mathrm{{{self.variable_name(variable)}}} /\partial t$ [{self.unit(variable)}/yr]'
+            ds[f'dt_{var}'] = dy_dt
+
+        plot_kw['ds'] = ds
+        # need to extract labels as derivatives have no defaults
+        labels = plot_kw.pop('labels', None) or default_variable_labels()
+        self._ts(
+            f'dt_{variable}',
+            labels=[labels.get(var, var) for var in (variable, var_rm)],
+            **plot_kw,
         )
+
+        plt.ylim(ds[f'dt_{var_rm}'].min() / 1.05, ds[f'dt_{var_rm}'].max() * 1.05)
+        ylab = f'$\partial \mathrm{{{self.variable_name(variable)}}} /\partial t$ [{self.unit(variable)}/yr]'
+        plt.ylabel(ylab)
         plt.legend()
         plt.title('')
 
-    @staticmethod
-    def _mean_and_std(ds, variable, other_dim):
-        if variable is None:
-            da = ds
-        else:
-            da = ds[variable]
-        if other_dim is None:
-            return da, None
-        return da.mean(other_dim), da.std(other_dim)
-
     @oet.utils.timed()
     def time_series(
         self,
-        variable='tas',
-        time='time',
-        other_dim=('x', 'y'),
-        running_mean=10,
-        interval=True,
+        variable=None,
+        other_dim=None,
+        running_mean=None,
+        interval=None,
         axes=None,
         **kw,
     ):
         ds = self.data_set
-        if interval is False:
-            ds = ds.copy().mean(other_dim)
-            other_dim = None
-
-        plot_kw = dict(**kw)
+        variable = variable or self.variable
+        other_dim = (
+            other_dim
+            if other_dim is not None
+            else oet.config.config['analyze']['lon_lat_dim'].split(',')
+        )
+        rm = running_mean or oet.config.config['analyze']['moving_average_years']
+        if interval is not None:
+            oet.config.get_logger().warning('Interval kwarg is replaced by show_std')
+            kw['show_std'] = interval
 
+        plot_kw = dict(variable=variable, ds=ds, running_mean=rm, **kw)
         if axes is None:
             _, axes = plt.subplots(3, 1, figsize=(12, 10), gridspec_kw=dict(hspace=0.3))
 
         plt.sca(axes[0])
-        self._ts(
-            variable, ds=ds, running_mean=running_mean, other_dim=other_dim, **plot_kw
-        )
+        self._ts(**plot_kw)
 
         plt.sca(axes[1])
-        self._det_ts(
-            variable, ds=ds, running_mean=running_mean, other_dim=other_dim, **plot_kw
-        )
+        self._det_ts(**plot_kw)
 
         plt.sca(axes[2])
         self._ddt_ts(
-            variable,
-            ds=ds,
-            time=time,
-            running_mean=running_mean,
-            other_dim=other_dim,
             **plot_kw,
         )
 
         return axes
 
     @property
-    def ds(self):
-        warn(
-            f'Calling {self.__class__.__name__}.ds is depricated, use {self.__class__.__name__}.ds'
-        )
-        return self.data_set
-
-    @property
     def dataset(self):
         warn(f'Calling {self.__class__.__name__}.data_set not .dataset')
         return self.data_set
 
     @property
     def title(self):
         return make_title(self.data_set)
 
+    @property
+    def variable(self):
+        return self.data_set.attrs['variable_id']
+
     def variable_name(self, variable):
         return default_variable_labels().get(
             variable,
             variable,  # self.data_set[variable].attrs.get('long_name', variable)
         )
 
     def unit(self, variable):
-        if 'units' not in self.data_set[variable].attrs:
-            oet.config.get_logger().warning(
-                f'No units for {variable} in {self.data_set}'
-            )
-            # raise ValueError( self.data_set.attrs, self.data_set[variable].attrs, variable)
-        return self.data_set[variable].attrs.get('units', f'?').replace('%', '\%')
+        return get_unit(self.data_set, variable)
 
 
 class HistoricalMapMaker(MapMaker):
     def __init__(self, *args, ds_historical=None, **kwargs):
         if ds_historical is None:
             raise ValueError('Argument ds_historical is required')
         self.ds_historical = ds_historical
         super().__init__(*args, **kwargs)
 
     @staticmethod
     def calculate_ratio_and_max(da, da_historical):
-        result = da / da_historical
+        mask_divide_by_zero = (da_historical == 0) & (da > 0)
+        denominator = da_historical.values
+        denominator[denominator == 0] = np.inf
+        result = da / denominator
         ret_array = result.values
         if len(ret_array) == 0:
             raise ValueError(
                 f'Empty ret array, perhaps {da.shape} and {da_historical.shape} don\'t match?'
                 f'\nGot\n{ret_array}\n{result}\n{da}\n{da_historical}'
             )
         max_val = np.nanmax(ret_array)
-        mask_divide_by_zero = (da_historical == 0) & (da > 0)
+
+        # Anything clearly larger than the max val
         ret_array[mask_divide_by_zero.values] = 10 * max_val
         result.data = ret_array
         return result, max_val
 
     def set_norm_for_item(self, item, max_val):
         current_norm = self.get_normalizations()
         low, high = current_norm.get(item, [None, None])
@@ -463,11 +397,93 @@
 
     def __getattr__(self, item):
         if item in self.conditions:
             return self.get_compare(item)
         return self.__getattribute__(item)
 
 
+def plot_simple(ds, var, other_dim=None, show_std=False, std_kw=None, **kw):
+    if other_dim is None:
+        other_dim = set(ds[var].dims) - {'time'}
+    mean = ds[var].mean(other_dim)
+    l = mean.plot(**kw)
+    if show_std:
+        std_kw = std_kw or dict()
+        for k, v in kw.items():
+            std_kw.setdefault(k, v)
+        std_kw.setdefault('alpha', 0.4)
+        std_kw.pop('label', None)
+        std = ds[var].std(other_dim)
+        (mean - std).plot(color=l[0]._color, **std_kw)
+        (mean + std).plot(color=l[0]._color, **std_kw)
+
+    set_y_lim_var(var)
+    plt.ylabel(
+        f'{oet.plotting.plot.default_variable_labels().get(var, var)} [{get_unit(ds, var)}]'
+    )
+    plt.title('')
+
+
+@oet.utils.check_accepts(accepts=dict(plot=('i', 'ii', 'iii', 'iv', 'v', None)))
+def summarize_mask(
+    data_set, one_mask, plot_kw=None, other_dim=None, plot='v', fig_kw=None
+):
+    plot_kw = plot_kw or dict(show_std=True)
+    other_dim = other_dim or oet.config.config['analyze']['lon_lat_dim'].split(',')
+    fig_kw = fig_kw or dict(
+        mosaic='a.\nb.',
+        figsize=(17, 6),
+        gridspec_kw=dict(width_ratios=[1, 1], wspace=0.1, hspace=0.05),
+    )
+
+    ds_sel = oet.analyze.region_finding.mask_xr_ds(data_set.copy(), one_mask)
+    mm_sel = MapMaker(ds_sel)
+    fig, axes = plt.subplot_mosaic(**fig_kw)
+
+    axes['b'].sharex(axes['a'])
+
+    plt.sca(axes['a'])
+    var = mm_sel.variable
+    plot_simple(ds_sel, var, **plot_kw)
+
+    plt.sca(axes['b'])
+    var = f'{mm_sel.variable}_detrend'
+    plot_simple(ds_sel, var, **plot_kw)
+
+    if plot is None:
+        ds_dummy = ds_sel.copy()
+        ds_dummy['cell_area'] /= 1e6
+
+        ax = fig.add_subplot(1, 2, 2, projection=get_cartopy_projection())
+        tot_area = float(ds_dummy['cell_area'].sum(skipna=True))
+
+        ds_dummy['cell_area'].values[ds_dummy['cell_area'] > 0] = tot_area
+        ds_dummy['cell_area'].plot(
+            vmin=1,
+            vmax=510100000,
+            norm=LogNorm(),
+            cbar_kwargs={
+                **mm_sel.kw.get('cbar', {}),
+                **dict(extend='neither', label='Sum of area [km$^2$]'),
+            },
+        )
+        ax.coastlines()
+        exponent = int(np.log10(tot_area))
+
+        plt.title(f'Area ${tot_area/(10**exponent):.1f}\\times10^{exponent}$ km$^2$')
+        gl = ax.gridlines(draw_labels=True)
+        gl.top_labels = False
+        gl.right_labels = False
+    else:
+        ax = fig.add_subplot(1, 2, 2, projection=get_cartopy_projection())
+        mm_sel.plot_i(label=plot, ax=ax, coastlines=True)
+    plt.suptitle(mm_sel.title, y=0.97)
+    axes = list(axes.values()) + [ax]
+    # Remove labels of top left axis.
+    plt.setp(axes[0].get_xticklabels(), visible=False)
+    return axes
+
+
 def make_title(ds):
     return '{institution_id} {source_id} {experiment_id} {variant_label} {variable_id} {version}'.format(
         **ds.attrs
     )
```

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools/synda_files/synda_files.py` & `optim_esm_tools-1.0.0/optim_esm_tools/synda_files/synda_files.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools/utils.py` & `optim_esm_tools-1.0.0/optim_esm_tools/utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools.egg-info/PKG-INFO` & `optim_esm_tools-1.0.0/optim_esm_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim-esm-tools
-Version: 0.5.0
+Version: 1.0.0
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,32 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        1.0.0 / 2023-07-18
+        ------------------
+        **major change**
+        * Harmonize preprocessing with `cdo` by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/81
+        
+        **minor changes**
+        * Plotting routine for masked regions by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/82
+        * Plot region mask by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/85
+        * Add plot maker by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/83
+        
+        **patches**
+        * Raise error for invalid dates by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/84
+        * [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in https://github.com/JoranAngevaare/optim_esm_tools/pull/86
+        * Ready for release v1.0.0 by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/87
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.5.0...v1.0.0
+        
+        
         0.5.0 / 2023-07-07
         ------------------
         **Last release before refactoring pre-processing**
         *Next release will use CDO tools instead of xMip tools to do pre-processing for reliability reasons*
         
         * Lon and lat coords for clustering by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/79
         * Queriable area field by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/80
```

### Comparing `optim_esm_tools-0.5.0/optim_esm_tools.egg-info/SOURCES.txt` & `optim_esm_tools-1.0.0/optim_esm_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+bin/oet_plot
 optim_esm_tools/__init__.py
 optim_esm_tools/_test_utils.py
 optim_esm_tools/config.py
 optim_esm_tools/optim_esm_conf.ini
 optim_esm_tools/utils.py
 optim_esm_tools.egg-info/PKG-INFO
 optim_esm_tools.egg-info/SOURCES.txt
 optim_esm_tools.egg-info/dependency_links.txt
 optim_esm_tools.egg-info/not-zip-safe
 optim_esm_tools.egg-info/requires.txt
 optim_esm_tools.egg-info/top_level.txt
 optim_esm_tools/analyze/__init__.py
-optim_esm_tools/analyze/calculate_metric.py
 optim_esm_tools/analyze/clustering.py
 optim_esm_tools/analyze/cmip_handler.py
 optim_esm_tools/analyze/find_matches.py
 optim_esm_tools/analyze/globals.py
 optim_esm_tools/analyze/io.py
-optim_esm_tools/analyze/query_metric.py
+optim_esm_tools/analyze/pre_process.py
 optim_esm_tools/analyze/region_finding.py
 optim_esm_tools/analyze/tipping_criteria.py
 optim_esm_tools/analyze/xarray_tools.py
-optim_esm_tools/cmip_files/__init__.py
 optim_esm_tools/plotting/__init__.py
 optim_esm_tools/plotting/map_maker.py
 optim_esm_tools/plotting/plot.py
 optim_esm_tools/synda_files/__init__.py
-optim_esm_tools/synda_files/format_synda.py
 optim_esm_tools/synda_files/synda_files.py
-test/test_area_query.py
 test/test_basics.py
 test/test_clustering.py
 test/test_find_matches.py
 test/test_pangeo_download.py
 test/test_plotting.py
 test/test_region_finding.py
 test/test_utils.py
```

### Comparing `optim_esm_tools-0.5.0/setup.py` & `optim_esm_tools-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
 requirements = open_requirements('requirements.txt')
 
 setuptools.setup(
     name='optim_esm_tools',
-    version='0.5.0',
+    version='1.0.0',
     description='Tools for OptimESM',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='Joran R. Angevaare',
     url='https://github.com/JoranAngevaare/optim_esm_tools',
     packages=setuptools.find_packages(),
     package_dir={
         'optim_esm_tools': 'optim_esm_tools',
     },
     package_data={
         'optim_esm_tools': ['data/*', 'optim_esm_tools/*', '*.ini*'],
     },
+    scripts=['bin/oet_plot'],
     setup_requires=['pytest-runner'],
     install_requires=requirements,
     python_requires='>=3.8',
     tests_require=requirements + open_requirements('requirements_tests.txt'),
-    scripts=[],
     keywords=[],
     classifiers=[
         'Intended Audience :: Science/Research',
         'Development Status :: 2 - Pre-Alpha',
         'Programming Language :: Python :: 3.8',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
```

### Comparing `optim_esm_tools-0.5.0/test/test_clustering.py` & `optim_esm_tools-1.0.0/test/test_clustering.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 
 def test_clustering_empty():
     ds = optim_esm_tools._test_utils.minimal_xr_ds().copy()
     ds['var'] = (ds['var'].dims, np.zeros_like(ds['var']))
     ds = ds.isel(time=0)
     assert np.all(np.shape(ds['var']) > np.array([2, 2]))
-    lat, lon = np.meshgrid(ds['y'], ds['x'])
-    clusters, masks = clustering.build_cluster_mask(ds['var'] > 0, lon, lat)
+
+    clusters, masks = clustering.build_cluster_mask(ds['var'] > 0, ds['lon'], ds['lat'])
     assert len(clusters) == len(masks) == 0
 
 
 def test_clustering_double_blob(npoints=100, res_x=3, res_y=3):
     ds = optim_esm_tools._test_utils.minimal_xr_ds().copy()
     ds = ds.isel(time=0)
 
@@ -28,15 +28,18 @@
             np.clip(np.random.normal(y, res_y, npoints).astype(int), 0, len_y),
         ):
             arr[x_i][y_i] += 1
 
     assert np.sum(arr) == 2 * npoints
     ds['var'] = (ds['var'].dims, arr)
     assert np.all(np.shape(ds['var']) > np.array([2, 2]))
-    lat, lon = np.meshgrid(ds['y'], ds['x'])
+    (
+        lon,
+        lat,
+    ) = np.meshgrid(ds['lon'], ds['lat'])
     clusters, masks = clustering.build_cluster_mask(
         ds['var'] > 1,
         lon,
         lat,
         max_distance_km=1000,
         min_samples=2,
     )
```

### Comparing `optim_esm_tools-0.5.0/test/test_region_finding.py` & `optim_esm_tools-1.0.0/test/test_region_finding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import unittest
 import optim_esm_tools._test_utils
 from optim_esm_tools.analyze import region_finding
+from optim_esm_tools.analyze.cmip_handler import read_ds
 import tempfile
 import os
 
 
 class Work(unittest.TestCase):
     """
     Note of caution! cache=True can lead to funky behavoir!
@@ -25,14 +26,15 @@
         assert year_path
         assert os.path.exists(year_path)
         return year_path
 
     def test_max_region(self, make='MaxRegion', new_opt=None, skip_save=True):
         cls = getattr(region_finding, make)
         file_path = self.get_path('ssp585', refresh=False)
+
         head, tail = os.path.split(file_path)
         extra_opt = dict(
             time_series_joined=True,
             scatter_medians=True,
             percentiles=50,
             search_kw=dict(required_file=tail),
         )
@@ -42,26 +44,25 @@
             save_kw = dict(
                 save_in=temp_dir,
                 sub_dir=None,
                 file_types=('png',),
                 dpi=25,
                 skip=skip_save,
             )
-            ## REMEMBER THE CACHE = TRUE!
+
             region_finder = cls(
                 path=head,
                 read_ds_kw=dict(
                     _file_name=tail, _cache=os.environ.get('_CACHE_TRUE', 0)
                 ),
-                transform=True,
                 save_kw=save_kw,
                 extra_opt=extra_opt,
             )
             region_finder.show = False
-            ## REMEMBER THE CACHE = TRUE!
+
             region_finder.workflow()
             return region_finder
 
     def test_max_region_wo_time_series(self):
         self.test_max_region('MaxRegion', new_opt=dict(time_series_joined=False))
 
     def test_percentiles(self):
@@ -82,7 +83,19 @@
     def test_local_history(self):
         self.test_max_region('LocalHistory')
 
     def test_percentiles_product_weighted(self):
         self.test_max_region(
             'ProductPercentiles', new_opt=dict(cluster_method='weighted')
         )
+
+    def test_error_message(self, make='MaxRegion'):
+        cls = getattr(region_finding, make)
+        file_path = self.get_path('ssp585', refresh=False)
+        head, tail = os.path.split(file_path)
+        ds = read_ds(
+            head,
+            _file_name=tail,
+        )
+        region = cls(data_set=ds)
+        with self.assertRaises(ValueError):
+            region.check_shape(ds['cell_area'].T)
```

### Comparing `optim_esm_tools-0.5.0/test/test_utils.py` & `optim_esm_tools-1.0.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.5.0/test/test_viewer.py` & `optim_esm_tools-1.0.0/test/test_viewer.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.5.0/test/test_workflow.py` & `optim_esm_tools-1.0.0/test/test_workflow.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,53 +5,73 @@
 import matplotlib.pyplot as plt
 import subprocess
 from optim_esm_tools._test_utils import synda_test_available, get_example_data_loc
 
 
 @unittest.skipIf(not synda_test_available(), 'synda data not available')
 class TestMapMaker(unittest.TestCase):
-    # example_data_set = oet._test_utils.EXAMPLE_DATA_SET
+    name_merged = 'test_merged.nc'
 
     def from_amon_to_ayear(self):
         if os.path.exists(self.ayear_file):
             return
 
         os.makedirs(os.path.split(self.ayear_file)[0], exist_ok=1)
-        # Doesn't work?
-        # cdo.Cdo().yearmonmean(self.amon_file, self.ayear_file)
+        import cdo
+
         cmd = f'cdo yearmonmean {self.amon_file} {self.ayear_file}'
         print(cmd)
-        subprocess.call(cmd, shell=True)
+        cdo.Cdo().yearmonmean(input=self.amon_file, output=self.ayear_file)
         assert os.path.exists(self.ayear_file), self.ayear_file
 
     @classmethod
     def setUpClass(cls):
         cls.base = os.path.join(os.environ['ST_HOME'], 'data')
         cls.amon_file = get_example_data_loc()
         cls.ayear_file = os.path.join(
-            os.path.split(cls.amon_file.replace('Amon', 'AYear'))[0], 'merged.nc'
+            os.path.split(cls.amon_file.replace('Amon', 'AYear'))[0], cls.name_merged
         )
 
+    def tearDown(self) -> None:
+        assert os.path.exists(self.ayear_file)
+        return super().tearDown()
+
     def setUp(self):
         self.from_amon_to_ayear()
+        assert os.path.exists(self.ayear_file)
         super().setUp()
 
     def test_read_data(self):
-        dataset = oet.cmip_files.io.load_glob(self.ayear_file)
+        dataset = oet.analyze.io.load_glob(self.ayear_file)
 
     def test_make_map(self):
-        data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
+        data_set = oet.analyze.cmip_handler.read_ds(
+            os.path.split(self.ayear_file)[0], _file_name=self.name_merged
+        )
         oet.plotting.map_maker.MapMaker(data_set=data_set).plot_all(2)
         plt.clf()
 
-    def test_map_maker_time_series(self):
-        data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
-        oet.plotting.map_maker.MapMaker(data_set=data_set).time_series()
+    def test_map_maker_time_series(self, **kw):
+        data_set = oet.analyze.cmip_handler.read_ds(
+            os.path.split(self.ayear_file)[0], _file_name=self.name_merged
+        )
+        oet.plotting.map_maker.MapMaker(data_set=data_set).time_series(**kw)
         plt.clf()
 
+    def test_map_maker_time_series_only_running_mean(self):
+        self.test_map_maker_time_series(only_rm=True)
+
+    def test_date_out_of_range(self):
+        with self.assertRaises(oet.analyze.pre_process.NoDataInTimeRangeError):
+            oet.read_ds(
+                os.path.split(self.ayear_file)[0],
+                _file_name=self.name_merged,
+                min_time=(3000, 1, 1),
+            )
+
     @classmethod
     def tearDownClass(cls) -> None:
         os.remove(cls.ayear_file)
         return super().tearDownClass()
 
 
 class Units(unittest.TestCase):
```

