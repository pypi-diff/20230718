# Comparing `tmp/pywatershed-0.1.2.tar.gz` & `tmp/pywatershed-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywatershed-0.1.2.tar", last modified: Fri Apr 28 17:03:17 2023, max compression
+gzip compressed data, was "pywatershed-0.2.0.tar", last modified: Tue Jul 18 19:39:28 2023, max compression
```

## Comparing `pywatershed-0.1.2.tar` & `pywatershed-0.2.0.tar`

### file list

```diff
@@ -1,90 +1,82 @@
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.893545 pywatershed-0.1.2/
--rw-r--r--   0 jdhughes (179580369) 286921933      958 2023-04-28 15:05:53.000000 pywatershed-0.1.2/.gitignore
--rw-r--r--   0 jdhughes (179580369) 286921933       50 2023-04-27 14:17:27.000000 pywatershed-0.1.2/.mf6_ci_ref_remote
--rw-r--r--   0 jdhughes (179580369) 286921933     1231 2023-04-27 14:17:27.000000 pywatershed-0.1.2/DISCLAIMER.md
--rw-r--r--   0 jdhughes (179580369) 286921933     6555 2023-04-27 14:17:27.000000 pywatershed-0.1.2/LICENSE
--rw-r--r--   0 jdhughes (179580369) 286921933      218 2023-04-28 14:41:12.000000 pywatershed-0.1.2/MANIFEST.in
--rw-r--r--   0 jdhughes (179580369) 286921933    11436 2023-04-28 17:03:17.892827 pywatershed-0.1.2/PKG-INFO
--rw-r--r--   0 jdhughes (179580369) 286921933    10289 2023-04-28 17:02:42.000000 pywatershed-0.1.2/README.md
--rw-r--r--   0 jdhughes (179580369) 286921933     2416 2023-04-28 16:55:55.000000 pywatershed-0.1.2/pyproject.toml
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.678964 pywatershed-0.1.2/pywatershed/
--rw-r--r--   0 jdhughes (179580369) 286921933      140 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/MANIFEST.in
--rw-r--r--   0 jdhughes (179580369) 286921933     1146 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/__init__.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.693740 pywatershed-0.1.2/pywatershed/analysis/
--rw-r--r--   0 jdhughes (179580369) 286921933       74 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/analysis/__init__.py
--rw-r--r--   0 jdhughes (179580369) 286921933     7242 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/analysis/model_graph.py
--rw-r--r--   0 jdhughes (179580369) 286921933     9907 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/analysis/process_plot.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.699432 pywatershed-0.1.2/pywatershed/analysis/utils/
--rw-r--r--   0 jdhughes (179580369) 286921933        0 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/analysis/utils/__init__.py
--rw-r--r--   0 jdhughes (179580369) 286921933    49899 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/analysis/utils/colorbrewer.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.715409 pywatershed-0.1.2/pywatershed/atmosphere/
--rw-r--r--   0 jdhughes (179580369) 286921933    30633 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/atmosphere/PRMSAtmosphere.py
--rw-r--r--   0 jdhughes (179580369) 286921933    15953 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/atmosphere/PRMSSolarGeometry.py
--rw-r--r--   0 jdhughes (179580369) 286921933       92 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/atmosphere/__init__.py
--rw-r--r--   0 jdhughes (179580369) 286921933     1623 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/atmosphere/solar_constants.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.750640 pywatershed-0.1.2/pywatershed/base/
--rw-r--r--   0 jdhughes (179580369) 286921933      253 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/base/__init__.py
--rw-r--r--   0 jdhughes (179580369) 286921933      342 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/base/accessor.py
--rw-r--r--   0 jdhughes (179580369) 286921933     3188 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/base/adapter.py
--rw-r--r--   0 jdhughes (179580369) 286921933    23133 2023-04-28 15:04:05.000000 pywatershed-0.1.2/pywatershed/base/budget.py
--rw-r--r--   0 jdhughes (179580369) 286921933     6929 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/base/control.py
--rw-r--r--   0 jdhughes (179580369) 286921933    29034 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/base/data_model.py
--rw-r--r--   0 jdhughes (179580369) 286921933     8156 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/base/meta.py
--rw-r--r--   0 jdhughes (179580369) 286921933    10684 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/base/model.py
--rw-r--r--   0 jdhughes (179580369) 286921933     1729 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/base/parameters.py
--rw-r--r--   0 jdhughes (179580369) 286921933    20236 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/base/storageUnit.py
--rw-r--r--   0 jdhughes (179580369) 286921933     2014 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/base/timeseries.py
--rw-r--r--   0 jdhughes (179580369) 286921933     2047 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/constants.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.804371 pywatershed-0.1.2/pywatershed/hydrology/
--rw-r--r--   0 jdhughes (179580369) 286921933    11221 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSCanopy.f90
--rw-r--r--   0 jdhughes (179580369) 286921933    22780 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSCanopy.py
--rw-r--r--   0 jdhughes (179580369) 286921933     4836 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSCanopy.pyf
--rw-r--r--   0 jdhughes (179580369) 286921933     5902 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSChannel.f90
--rw-r--r--   0 jdhughes (179580369) 286921933    22286 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSChannel.py
--rw-r--r--   0 jdhughes (179580369) 286921933     2139 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSChannel.pyf
--rw-r--r--   0 jdhughes (179580369) 286921933     4928 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSEt.py
--rw-r--r--   0 jdhughes (179580369) 286921933     1959 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSGroundwater.f90
--rw-r--r--   0 jdhughes (179580369) 286921933     7406 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSGroundwater.py
--rw-r--r--   0 jdhughes (179580369) 286921933     1613 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSGroundwater.pyf
--rw-r--r--   0 jdhughes (179580369) 286921933    47982 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSRunoff.py
--rw-r--r--   0 jdhughes (179580369) 286921933   122612 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSSnow.py
--rw-r--r--   0 jdhughes (179580369) 286921933    49110 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/PRMSSoilzone.py
--rw-r--r--   0 jdhughes (179580369) 286921933    10656 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/Starfit.py
--rw-r--r--   0 jdhughes (179580369) 286921933      251 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/hydrology/__init__.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.813871 pywatershed-0.1.2/pywatershed/parameters/
--rw-r--r--   0 jdhughes (179580369) 286921933       94 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/parameters/__init__.py
--rw-r--r--   0 jdhughes (179580369) 286921933    10862 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/parameters/prms_parameters.py
--rw-r--r--   0 jdhughes (179580369) 286921933     3783 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/parameters/starfit_parameters.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.644271 pywatershed-0.1.2/pywatershed/static/
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.829041 pywatershed-0.1.2/pywatershed/static/metadata/
--rw-r--r--   0 jdhughes (179580369) 286921933    28511 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/static/metadata/control.yaml
--rw-r--r--   0 jdhughes (179580369) 286921933     2459 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/static/metadata/dimensions.yaml
--rw-r--r--   0 jdhughes (179580369) 286921933    83393 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/static/metadata/parameters.yaml
--rw-r--r--   0 jdhughes (179580369) 286921933    75665 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/static/metadata/variables.yaml
--rw-r--r--   0 jdhughes (179580369) 286921933     5668 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/static/metadata/xml_to_yaml.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.891677 pywatershed-0.1.2/pywatershed/utils/
--rw-r--r--   0 jdhughes (179580369) 286921933      367 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/__init__.py
--rw-r--r--   0 jdhughes (179580369) 286921933     8316 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/cbh_utils.py
--rw-r--r--   0 jdhughes (179580369) 286921933     1498 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/control.py
--rw-r--r--   0 jdhughes (179580369) 286921933     9618 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/csv_utils.py
--rw-r--r--   0 jdhughes (179580369) 286921933     6225 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/dis_hru.py
--rw-r--r--   0 jdhughes (179580369) 286921933      494 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/formatting.py
--rw-r--r--   0 jdhughes (179580369) 286921933    22741 2023-04-28 15:04:06.000000 pywatershed-0.1.2/pywatershed/utils/netcdf_utils.py
--rw-r--r--   0 jdhughes (179580369) 286921933    12834 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/parameters.py
--rw-r--r--   0 jdhughes (179580369) 286921933    13621 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/prms5_file_util.py
--rw-r--r--   0 jdhughes (179580369) 286921933    11748 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/prms5util.py
--rw-r--r--   0 jdhughes (179580369) 286921933    16128 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/prms_to_mf6.py
--rw-r--r--   0 jdhughes (179580369) 286921933     4544 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/separate_nhm_params.py
--rw-r--r--   0 jdhughes (179580369) 286921933     1392 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/time_utils.py
--rw-r--r--   0 jdhughes (179580369) 286921933      392 2023-04-27 14:17:27.000000 pywatershed-0.1.2/pywatershed/utils/utils.py
--rw-r--r--   0 jdhughes (179580369) 286921933       71 2023-04-28 16:33:18.000000 pywatershed-0.1.2/pywatershed/version.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-04-28 17:03:17.682900 pywatershed-0.1.2/pywatershed.egg-info/
--rw-r--r--   0 jdhughes (179580369) 286921933    11436 2023-04-28 17:03:17.000000 pywatershed-0.1.2/pywatershed.egg-info/PKG-INFO
--rw-r--r--   0 jdhughes (179580369) 286921933     2424 2023-04-28 17:03:17.000000 pywatershed-0.1.2/pywatershed.egg-info/SOURCES.txt
--rw-r--r--   0 jdhughes (179580369) 286921933        1 2023-04-28 17:03:17.000000 pywatershed-0.1.2/pywatershed.egg-info/dependency_links.txt
--rw-r--r--   0 jdhughes (179580369) 286921933        1 2023-04-27 14:27:25.000000 pywatershed-0.1.2/pywatershed.egg-info/not-zip-safe
--rw-r--r--   0 jdhughes (179580369) 286921933      323 2023-04-28 17:03:17.000000 pywatershed-0.1.2/pywatershed.egg-info/requires.txt
--rw-r--r--   0 jdhughes (179580369) 286921933       12 2023-04-28 17:03:17.000000 pywatershed-0.1.2/pywatershed.egg-info/top_level.txt
--rw-r--r--   0 jdhughes (179580369) 286921933      779 2023-04-27 14:17:27.000000 pywatershed-0.1.2/readthedocs.yml
--rw-r--r--   0 jdhughes (179580369) 286921933       38 2023-04-28 17:03:17.893715 pywatershed-0.1.2/setup.cfg
--rw-r--r--   0 jdhughes (179580369) 286921933      954 2023-04-28 16:55:22.000000 pywatershed-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.202687 pywatershed-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-18 19:38:35.000000 pywatershed-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-18 19:38:35.000000 pywatershed-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-18 19:39:28.202687 pywatershed-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-18 19:38:35.000000 pywatershed-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.194687 pywatershed-0.2.0/pywatershed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.194687 pywatershed-0.2.0/pywatershed/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/analysis/model_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/analysis/process_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.194687 pywatershed-0.2.0/pywatershed/analysis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/analysis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50088 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/analysis/utils/colorbrewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.198687 pywatershed-0.2.0/pywatershed/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30420 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/atmosphere/prms_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/atmosphere/prms_solar_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/atmosphere/solar_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.198687 pywatershed-0.2.0/pywatershed/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23425 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/conservative_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36641 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32582 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/base/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.198687 pywatershed-0.2.0/pywatershed/hydrology/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/hydrology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21839 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/hydrology/prms_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20861 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/hydrology/prms_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/hydrology/prms_et.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/hydrology/prms_groundwater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44575 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/hydrology/prms_runoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117886 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/hydrology/prms_snow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44571 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/hydrology/prms_soilzone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/hydrology/starfit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.198687 pywatershed-0.2.0/pywatershed/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/parameters/prms_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/parameters/starfit_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.194687 pywatershed-0.2.0/pywatershed/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.198687 pywatershed-0.2.0/pywatershed/static/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    28511 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/static/metadata/control.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/static/metadata/dimensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    83790 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/static/metadata/parameters.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    76228 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/static/metadata/variables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/static/metadata/xml_to_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.202687 pywatershed-0.2.0/pywatershed/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/cbh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/csv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/dis_hru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22724 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/netcdf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16371 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/parse_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/prms5_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/prms5util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/prms_to_mf6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/separate_nhm_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 19:38:36.000000 pywatershed-0.2.0/pywatershed/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:39:28.194687 pywatershed-0.2.0/pywatershed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-18 19:39:28.000000 pywatershed-0.2.0/pywatershed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-18 19:39:28.000000 pywatershed-0.2.0/pywatershed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:39:28.000000 pywatershed-0.2.0/pywatershed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:38:53.000000 pywatershed-0.2.0/pywatershed.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-18 19:39:28.000000 pywatershed-0.2.0/pywatershed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 19:39:28.000000 pywatershed-0.2.0/pywatershed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:39:28.202687 pywatershed-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-18 19:38:36.000000 pywatershed-0.2.0/setup.py
```

### Comparing `pywatershed-0.1.2/LICENSE` & `pywatershed-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/PKG-INFO` & `pywatershed-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,232 +1,198 @@
 Metadata-Version: 2.1
 Name: pywatershed
-Version: 0.1.2
+Version: 0.2.0
 Summary: pywatershed is a Python package for hydrologic modeling
 Author-email: USGS Enterprise Capacity Team <modflow@usgs.gov>
 Maintainer-email: "James L. McCreight" <jmccreight@usgs.gov>, "Joseph D. Hughes" <jdhughes@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://pywatershed.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/EC-USGS/pywatershed/issues
 Project-URL: Source Code, https://github.com/EC-USGS/pywatershed
 Keywords: hydrology,PRMS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.8
+Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: test
+Provides-Extra: optional
+Provides-Extra: doc
+Provides-Extra: all
 License-File: LICENSE
 
 # pywatershed
-[![ci-badge](https://github.com/ec-usgs/pywatershed/workflows/CI/badge.svg?branch=main)](https://github.com/ec-usgs/pywatershed/actions?query=workflow%3ACI)
+
+[![ci-badge](https://github.com/ec-usgs/pywatershed/workflows/CI/badge.svg?branch=develop)](https://github.com/ec-usgs/pywatershed/actions?query=workflow%3ACI)
 [![codecov-badge](https://codecov.io/gh/ec-usgs/pywatershed/branch/main/graph/badge.svg)](https://codecov.io/gh/ec-usgs/pywatershed)
 [![Documentation Status](https://readthedocs.org/projects/pywatershed/badge/?version=latest)](https://pywatershed.readthedocs.io/en/latest/?badge=latest)
+[![asv](http://img.shields.io/badge/benchmarked%20by-asv-green.svg?style=flat)](https://github.com/ec-usgs/pywatershed)
+[![Formatted with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+
+[![Available on pypi](https://img.shields.io/pypi/v/pywatershed.svg)](https://pypi.python.org/pypi/pywatershed)
+[![PyPI Status](https://img.shields.io/pypi/status/pywatershed.svg)](https://pypi.python.org/pypi/pywatershed)
+[![PyPI Versions](https://img.shields.io/pypi/pyversions/pywatershed.svg)](https://pypi.python.org/pypi/pywatershed)
+
+[![WholeTale](https://raw.githubusercontent.com/whole-tale/wt-design-docs/master/badges/wholetale-explore.svg)](https://dashboard.wholetale.org/run/64ae29e8a887f48b9f173678?tab=metadata)
+
 
-[![PyPI Version](https://img.shields.io/pypi/v/pywatershed.png)](https://pypi.python.org/pypi/pywatershed)
-[![PyPI Status](https://img.shields.io/pypi/status/pywatershed.png)](https://pypi.python.org/pypi/pywatershed)
-[![PyPI Versions](https://img.shields.io/pypi/pyversions/pywatershed.png)](https://pypi.python.org/pypi/pywatershed)
+<!-- START doctoc generated TOC please keep comment here to allow auto update -->
+<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
+**Table of Contents**
 
-[//]: # (<img src="https://raw.githubusercontent.com/ec-usgs/pywatershed/main/resources/images/prms_flow.png" alt="prms_flow" style="width:50;height:20">)
+- [Purpose](#purpose)
+- [Installation](#installation)
+- [Contributing](#contributing)
+- [Example Notebooks](#example-notebooks)
+- [Overview of Repository Contents](#overview-of-repository-contents)
+- [Disclaimer](#disclaimer)
+
+<!-- END doctoc generated TOC please keep comment here to allow auto update -->
+
+## Purpose
 
-Purpose
-=========
 The purpose of this repository is to refactor and redesign the [PRMS modeling
 system](https://www.usgs.gov/software/precipitation-runoff-modeling-system-prms)
 while maintaining its functionality. Code modernization is a step towards
 unification with [MODFLOW 6 (MF6)](https://github.com/MODFLOW-USGS/modflow6).
 
-The following motivations are taken from our
-[AGU poster from December 2022](https://agu2022fallmeeting-agu.ipostersessions.com/default.aspx?s=05-E1-C6-40-DF-0D-4D-C7-4E-DE-D2-61-02-05-8F-0A)
+The following motivations are taken from our [AGU poster from December
+2022](https://agu2022fallmeeting-agu.ipostersessions.com/default.aspx?s=05-E1-C6-40-DF-0D-4D-C7-4E-DE-D2-61-02-05-8F-0A)
 which provides additional details on motivations, project status, and current
 directions of this project as of approximately January 2023.
 
-Goals of the USGS Enterprise Capacity (EC) project include:
-  * A sustainable integrated, hydrologic modeling framework for the U.S. Geological Survey (USGS)
-  * Interoperable modeling across the USGS, partner agencies, and academia
-
-Goals for EC Watershed Modeling:
-  * Couple the Precipitation-Runoff Modeling System (PRMS, e.g. Regan et al, 2018)  with MODFLOW 6 (MF6, e.g. Langevin et al, 2017) in a sustainable way
-  * Redesign PRMS to be more modern and flexible
-  * Prioritize process representations in the current National Hydrological Model (NHM) based on PRMS 5.2.1
-
-Prototype an EC watershed model: "pywatershed"
-  * Redesign PRMS quickly in python
-  * Couple to MF6 via BMI/XMI interface (Hughes et al, 2021; Hutton et al, 2020)
-  * Establish a prototyping ground for EC codes that couples to the compiled framework: low cost proof of concepts (at the price of potentially less computational performance)
-  * Enable process representation hypothesis testing
-  * Use cutting-edge techniques and technologies to improve models
-  * Machine learning, automatic differentiation
-  * Address challenges of modeling across space and time scales
-  * Transition prototype watershed model to compiled EC code
-
-
-Installation and Python Environments
-=====================================
-This installation assumes you do not need to run automated tests locally. See
-the following "Developer Installation" section for complete installation
-instructions.
-
-To install the software you will need Python >= 3.8. We recommend installing
-the python package dependencies using anaconda or miniconda. Most users will
-likely want to create the `pyws_nb` conda environment by running
-
-```conda env create -f examples/examples_env.yml```.
-
-One could also do
-
-```pip install -r examples/exampes_env.txt```
-
-but this is not guaranteed.
-
-Once the environment is established, activate the environment and install
-pywatershed
-
-`conda activate pyws_nb; cd pywatershed; pip install .`
-
-If you would like to compile the fortran computational kernels for
-certain physical process representations (not required), you'll need a fortran
-compiler and you will run
-
-`export PYWS_FORTRAN=true; cd pywatershed;  pip install .`
-
-See Developer Requirements below for more details.
-
-
-Developer Installation
-=======================
-Git is required if you plan to contribute code back to the repository.
-
-C and Fortran compilers are required. We are currently using gnu (gcc, gfortran)
-11 and 12 as well as intel (icc, ifort) 2021 on Windows, Linux, and MacOS
-(including Apple Silicon). Both of these are freely obtainable but the installation
-process varies widely. We are looking for a conda-based approach to obtaining
-compilers, but currently do not have a solution. Compilers are needed for
-two applications:
-
-  1. Compiling and running C/Fortran PRMS code to generate testing/verification data
-  2. Compiling (installing) and running fortran backends/kernels for some hydrological
-     process representations in pywatershed
-
-On Apple Silicon, the PRMS source code is only currently known to compile with intel while
-the fortran kernels in pywatershed only compile with gnu.
-
-Python >= 3.8 is required. Three different python environments are specified within the repository.
-These are:
-
-* Minimal (for developing/testing), 'pyws': ci/requirements/environment.yml
-* Notebooks (~= minimal + jupyter), 'pyws_nb': examples/examples_env.yml
-* Documentation (only if you want to build the documentation), 'pyws-docs': ci/requirements/doc.yml
-
-We recommend (because we test it in CI) using anacoda or miniconda to establish these environments
-with the following commands
-
-```conda env create -f path/to/env_of_choice.yml```
-
-which will create the environment with "name" specified on the first line of the file, given before the path
-to the file above.
-
-More detailed python environment installation instructions using conda can be found in
-`examples/00_python_virtual_env.ipynb`.
-
-There are also .txt equivalents that can be used for installing from pip, like so:
-
-```pip install -r env_of_choice.txt```
-
-though these are not comprehensive installs as with conda and not tested.
-
-Once the python environment and dependencies are established and activated (`conda activate env_of_choice`),
-pywatershed is installed for development into that environment with the following command
-
-`cd pywatershed; pip install -e .`
-
-The numpy extension F2PY is used to provide fortran compiled kernels of core calculations to boost
-performance. F2PY is documented [within numpy](https://numpy.org/doc/stable/f2py/index.html). This
-repository is configured NOT to compile on install by default. Currently, we have not established
-this compilation procedure for Windows. On linux and MacOS, compilation of fortran kernels on package
-installation is achieved by the following code:
-
-```
-export SETUPTOOLS_ENABLE_FEATURES="legacy-editable"
-export CC=path/to/gcc  # for example
-export FC=path/to/gfortran  # for example
-export PYWS_FORTRAN=true
-cd path/to/pywatershed
-pip install -e .
-```
-
-Once the dependencies are available, we want to verify the software by running its test suite. The
-following testing procedures are also covered in the notebook `examples/01_automated_testing.ipynb`.
-To run the tests, we first need to generate the test data. This consists of running PRMS
-and then converting the output to netcdf:
-
-```
-cd path/to/pywatershed/test_data/scripts
-pytest -v -n=4 test_run_domains.py
-pytest -v -n=8 test_nc_domains.py
-```
-
-Finally, run the tests themselves,
-
-```
-cd path/to/pywatershed/autotest
-pytest -v -n=8
-```
-
-All tests should pass, XPASS, or XFAIL. XFAIL is an expected failure.
-
-
-Contributing
-============
-We welcome community development! Please file Issues and/or Pull Requests in the appropriate places on github. The continuous
-integration (CI) procedure is the first gate keeper for new code contribution. The CI procedure is defined by
-`.github/workflows/ci.yaml`. This includes running the formatting and linting packages `isort`, `black`, and
-`flake8` in addition to generating the test data and running the tests in `autotest/`. New codes need new tests so they can
-be verified moving ahead in time.
-
-
-Example Notebooks
-==================
-Jupyter notebooks containing examples are found in the
-[examples/](https://github.com/EC-USGS/pywatershed/tree/main/examples) directory. Numbered notebooks are tested.
-Notebooks 00 and 01 walk the user through the setting the python environment and running the software tests.
-Notebook 02 demonstrates modeling with pywatershed. Non-numbered notebooks cover additional topics. These notebooks
-are note yet covered by testing and so may be expected to have some issues until they are added to testing.
-
-
-Overview of Repository Contents
-==========
-The contents of directories at this level is described. Therein you may discover another README.md for more information.
-
-```
-.github/    Github actions for deploying continuous integration (CI)
-autotest/   pywatershed package testing using pytest
-bin/        PRMS executables distributed
-ci/         Python environments for CI
-doc/        Package/code documentation source code
-examples/   How to use the package, mostly jupyter notebooks
-prms_src/   PRMS source used for generating executables in bin/
-pywatershed/      Package source
-reference/  Ancillary materials for development
-resources/  Static stuff like images
-test_data/  Data used for automated testing
-```
-
-
-Disclaimer
-==========
-
-This information is preliminary or provisional and is subject to revision. It is being provided to meet the need for timely best science. The information has not received final approval by the U.S. Geological Survey (USGS) and is provided on the condition that neither the USGS nor the U.S. Government shall be held liable for any damages resulting from the authorized or unauthorized use of the information.
+Goals of the USGS Enterprise Capacity (EC) project include: * A sustainable
+integrated, hydrologic modeling framework for the U.S. Geological Survey (USGS)
+* Interoperable modeling across the USGS, partner agencies, and academia
+
+Goals for EC Watershed Modeling: * Couple the Precipitation-Runoff Modeling
+System (PRMS, e.g. Regan et al, 2018)  with MODFLOW 6 (MF6, e.g. Langevin et al,
+2017) in a sustainable way * Redesign PRMS to be more modern and flexible *
+Prioritize process representations in the current National Hydrological Model
+(NHM) based on PRMS 5.2.1
+
+Prototype an EC watershed model: "pywatershed" * Redesign PRMS quickly in python
+* Couple to MF6 via BMI/XMI interface (Hughes et al, 2021; Hutton et al, 2020) *
+Establish a prototyping ground for EC codes that couples to the compiled
+framework: low cost proof of concepts (at the price of potentially less
+computational performance) * Enable process representation hypothesis testing *
+Use cutting-edge techniques and technologies to improve models * Machine
+learning, automatic differentiation * Address challenges of modeling across
+space and time scales * Transition prototype watershed model to compiled EC code
+
+## Installation
+
+To install the software you will need Python 3.9 or 3.10.
+
+We currently recommend dependencies be installed with
+[Mamba](https://mamba.readthedocs.io/en/latest/) which will be much faster than
+Ananconda (but the conda command can also be used). An environment containing
+all core and optional dependencies can be created from the project root with:
+
+```mamba env create -f environment_w_jupyter.yml```
+
+(The environment `environment.yml` does not contain jupyter or jupyterlab
+in order to not interfere with installation in WholeTale, see Example
+Notebooks seection below.)
+
+The `pywatershed` package is [available on
+PyPI](https://pypi.org/project/pywatershed/). At the moment, the installation
+may not be reliable on all platforms and we are working to fix this.
+
+Using PyPI (with the above caveat), `pywatershed` can be installed with:
+
+``` pip install pywatershed ```
+
+A number of extra dependencies are needed to run the example notebooks. These
+can be installed with pip with
+
+``` pip install "pywatershed[optional]" ```
+
+These installation steps are suitable for `pywatershed` end users. See the
+[developer documentation](./DEVELOPER.md) for detailed instructions on
+configuring a development environment.
+
+## Contributing
+
+See the [developer documentation](./DEVELOPER.md) for instructions on setting up
+a development environment. See the [contribution guide](./CONTRIBUTING.md) to
+contribute to this project.
+
+## Example Notebooks
+
+For introductory example notebooks, look in the
+[`examples/`](https://github.com/EC-USGS/pywatershed/tree/main/examples>)
+directory in the repository. Numbered starting at 00, these are meant to be
+completed in order. Non-numbered notebooks coveradditional topics. These
+notebooks are note yet covered by testing and so may be expected to have some
+issues until they are added to testing. In `examples/developer/` there are
+notebooks of interest to developers who may want to learn about running the
+software tests.
+
+Though no notebook outputs are saved in Github, these notebooks can easily
+navigated to and run in WholeTale containers (free but sign-up or log-in
+required). This is a very easy and quick way to get started without needing to
+install pywatershed requirements yourself. WholeTale is an NSF funded project
+and supports logins from many institutions, e.g. the USGS, and you may not need
+to register.
+
+There are containers for both the `main` and `develop` branches.
+
+[![WholeTale](https://raw.githubusercontent.com/whole-tale/wt-design-docs/master/badges/wholetale-explore.svg)](https://dashboard.wholetale.org)
+* [WholeTale container for latest release (main
+  branch)](https://dashboard.wholetale.org/run/64ae29e8a887f48b9f173678?tab=metadata)
+* [WholeTale container for develop
+  branch](https://dashboard.wholetale.org/run/64ae25c3a887f48b9f1735c8?tab=metadata)
+
+WholeTale will give you a jupyter-lab running in the root of this
+repository. You can navigate to `examples/` and then open and run the notebooks
+of your choice.  The develop container may require the user to update the
+repository (`git pull origin`) to stay current with development.
+
+## Overview of Repository Contents
+
+The contents of directories at this level is described. Therein you may discover
+another README.md for more information.
+
+```
+.github/: Github actions, scripts and Python environments for continuous integration (CI) and releasing,
+asv_benchmarks/: preformance benchmarking by ASV
+autotest/: pywatershed package testing using pytest
+autotest_exs/: pywatershed example notebook testing using pytest
+bin/:PRMS executables distributed
+doc/:Package/code documentation source code
+evaluation/: tools for evaluation of pywatershed
+examples/:How to use the package, mostly jupyter notebooks
+prms_src/:PRMS source used for generating executables in bin/
+pywatershed/:Package source
+reference/:Ancillary materials for development
+resources/:Static stuff like images
+test_data/:Data used for automated testing
+```
+
+## Disclaimer
+
+This information is preliminary or provisional and is subject to revision. It is
+being provided to meet the need for timely best science. The information has not
+received final approval by the U.S. Geological Survey (USGS) and is provided on
+the condition that neither the USGS nor the U.S. Government shall be held liable
+for any damages resulting from the authorized or unauthorized use of the
+information.
 
 From: https://www2.usgs.gov/fsp/fsp_disclaimers.asp#5
 
-This software is in the public domain because it contains materials that originally came from the U.S. Geological Survey, an agency of the United States Department of Interior. For more information, see the [official USGS copyright policy](https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits "official USGS copyright policy")
-
-Although this software program has been used by the USGS, no warranty, expressed or implied, is made by the USGS or the U.S. Government as to the accuracy and functioning of the program and related program material nor shall the fact of distribution constitute any such warranty, and no responsibility is assumed by the USGS in connection therewith.
-This software is provided "AS IS."
+This software is in the public domain because it contains materials that
+originally came from the U.S. Geological Survey, an agency of the United States
+Department of Interior. For more information, see the [official USGS copyright
+policy](https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits
+"official USGS copyright policy")
+
+Although this software program has been used by the USGS, no warranty, expressed
+or implied, is made by the USGS or the U.S. Government as to the accuracy and
+functioning of the program and related program material nor shall the fact of
+distribution constitute any such warranty, and no responsibility is assumed by
+the USGS in connection therewith.  This software is provided "AS IS."
```

### Comparing `pywatershed-0.1.2/README.md` & `pywatershed-0.2.0/pywatershed.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,206 +1,198 @@
+Metadata-Version: 2.1
+Name: pywatershed
+Version: 0.2.0
+Summary: pywatershed is a Python package for hydrologic modeling
+Author-email: USGS Enterprise Capacity Team <modflow@usgs.gov>
+Maintainer-email: "James L. McCreight" <jmccreight@usgs.gov>, "Joseph D. Hughes" <jdhughes@usgs.gov>
+License: CC0
+Project-URL: Documentation, https://pywatershed.readthedocs.io
+Project-URL: Bug Tracker, https://github.com/EC-USGS/pywatershed/issues
+Project-URL: Source Code, https://github.com/EC-USGS/pywatershed
+Keywords: hydrology,PRMS
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Hydrology
+Requires-Python: <3.11,>=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: test
+Provides-Extra: optional
+Provides-Extra: doc
+Provides-Extra: all
+License-File: LICENSE
+
 # pywatershed
-[![ci-badge](https://github.com/ec-usgs/pywatershed/workflows/CI/badge.svg?branch=main)](https://github.com/ec-usgs/pywatershed/actions?query=workflow%3ACI)
+
+[![ci-badge](https://github.com/ec-usgs/pywatershed/workflows/CI/badge.svg?branch=develop)](https://github.com/ec-usgs/pywatershed/actions?query=workflow%3ACI)
 [![codecov-badge](https://codecov.io/gh/ec-usgs/pywatershed/branch/main/graph/badge.svg)](https://codecov.io/gh/ec-usgs/pywatershed)
 [![Documentation Status](https://readthedocs.org/projects/pywatershed/badge/?version=latest)](https://pywatershed.readthedocs.io/en/latest/?badge=latest)
+[![asv](http://img.shields.io/badge/benchmarked%20by-asv-green.svg?style=flat)](https://github.com/ec-usgs/pywatershed)
+[![Formatted with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+
+[![Available on pypi](https://img.shields.io/pypi/v/pywatershed.svg)](https://pypi.python.org/pypi/pywatershed)
+[![PyPI Status](https://img.shields.io/pypi/status/pywatershed.svg)](https://pypi.python.org/pypi/pywatershed)
+[![PyPI Versions](https://img.shields.io/pypi/pyversions/pywatershed.svg)](https://pypi.python.org/pypi/pywatershed)
+
+[![WholeTale](https://raw.githubusercontent.com/whole-tale/wt-design-docs/master/badges/wholetale-explore.svg)](https://dashboard.wholetale.org/run/64ae29e8a887f48b9f173678?tab=metadata)
 
-[![PyPI Version](https://img.shields.io/pypi/v/pywatershed.png)](https://pypi.python.org/pypi/pywatershed)
-[![PyPI Status](https://img.shields.io/pypi/status/pywatershed.png)](https://pypi.python.org/pypi/pywatershed)
-[![PyPI Versions](https://img.shields.io/pypi/pyversions/pywatershed.png)](https://pypi.python.org/pypi/pywatershed)
 
-[//]: # (<img src="https://raw.githubusercontent.com/ec-usgs/pywatershed/main/resources/images/prms_flow.png" alt="prms_flow" style="width:50;height:20">)
+<!-- START doctoc generated TOC please keep comment here to allow auto update -->
+<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
+**Table of Contents**
+
+- [Purpose](#purpose)
+- [Installation](#installation)
+- [Contributing](#contributing)
+- [Example Notebooks](#example-notebooks)
+- [Overview of Repository Contents](#overview-of-repository-contents)
+- [Disclaimer](#disclaimer)
+
+<!-- END doctoc generated TOC please keep comment here to allow auto update -->
+
+## Purpose
 
-Purpose
-=========
 The purpose of this repository is to refactor and redesign the [PRMS modeling
 system](https://www.usgs.gov/software/precipitation-runoff-modeling-system-prms)
 while maintaining its functionality. Code modernization is a step towards
 unification with [MODFLOW 6 (MF6)](https://github.com/MODFLOW-USGS/modflow6).
 
-The following motivations are taken from our
-[AGU poster from December 2022](https://agu2022fallmeeting-agu.ipostersessions.com/default.aspx?s=05-E1-C6-40-DF-0D-4D-C7-4E-DE-D2-61-02-05-8F-0A)
+The following motivations are taken from our [AGU poster from December
+2022](https://agu2022fallmeeting-agu.ipostersessions.com/default.aspx?s=05-E1-C6-40-DF-0D-4D-C7-4E-DE-D2-61-02-05-8F-0A)
 which provides additional details on motivations, project status, and current
 directions of this project as of approximately January 2023.
 
-Goals of the USGS Enterprise Capacity (EC) project include:
-  * A sustainable integrated, hydrologic modeling framework for the U.S. Geological Survey (USGS)
-  * Interoperable modeling across the USGS, partner agencies, and academia
-
-Goals for EC Watershed Modeling:
-  * Couple the Precipitation-Runoff Modeling System (PRMS, e.g. Regan et al, 2018)  with MODFLOW 6 (MF6, e.g. Langevin et al, 2017) in a sustainable way
-  * Redesign PRMS to be more modern and flexible
-  * Prioritize process representations in the current National Hydrological Model (NHM) based on PRMS 5.2.1
-
-Prototype an EC watershed model: "pywatershed"
-  * Redesign PRMS quickly in python
-  * Couple to MF6 via BMI/XMI interface (Hughes et al, 2021; Hutton et al, 2020)
-  * Establish a prototyping ground for EC codes that couples to the compiled framework: low cost proof of concepts (at the price of potentially less computational performance)
-  * Enable process representation hypothesis testing
-  * Use cutting-edge techniques and technologies to improve models
-  * Machine learning, automatic differentiation
-  * Address challenges of modeling across space and time scales
-  * Transition prototype watershed model to compiled EC code
-
-
-Installation and Python Environments
-=====================================
-This installation assumes you do not need to run automated tests locally. See
-the following "Developer Installation" section for complete installation
-instructions.
-
-To install the software you will need Python >= 3.8. We recommend installing
-the python package dependencies using anaconda or miniconda. Most users will
-likely want to create the `pyws_nb` conda environment by running
-
-```conda env create -f examples/examples_env.yml```.
-
-One could also do
-
-```pip install -r examples/exampes_env.txt```
-
-but this is not guaranteed.
-
-Once the environment is established, activate the environment and install
-pywatershed
-
-`conda activate pyws_nb; cd pywatershed; pip install .`
-
-If you would like to compile the fortran computational kernels for
-certain physical process representations (not required), you'll need a fortran
-compiler and you will run
-
-`export PYWS_FORTRAN=true; cd pywatershed;  pip install .`
-
-See Developer Requirements below for more details.
-
-
-Developer Installation
-=======================
-Git is required if you plan to contribute code back to the repository.
-
-C and Fortran compilers are required. We are currently using gnu (gcc, gfortran)
-11 and 12 as well as intel (icc, ifort) 2021 on Windows, Linux, and MacOS
-(including Apple Silicon). Both of these are freely obtainable but the installation
-process varies widely. We are looking for a conda-based approach to obtaining
-compilers, but currently do not have a solution. Compilers are needed for
-two applications:
-
-  1. Compiling and running C/Fortran PRMS code to generate testing/verification data
-  2. Compiling (installing) and running fortran backends/kernels for some hydrological
-     process representations in pywatershed
-
-On Apple Silicon, the PRMS source code is only currently known to compile with intel while
-the fortran kernels in pywatershed only compile with gnu.
-
-Python >= 3.8 is required. Three different python environments are specified within the repository.
-These are:
-
-* Minimal (for developing/testing), 'pyws': ci/requirements/environment.yml
-* Notebooks (~= minimal + jupyter), 'pyws_nb': examples/examples_env.yml
-* Documentation (only if you want to build the documentation), 'pyws-docs': ci/requirements/doc.yml
-
-We recommend (because we test it in CI) using anacoda or miniconda to establish these environments
-with the following commands
-
-```conda env create -f path/to/env_of_choice.yml```
-
-which will create the environment with "name" specified on the first line of the file, given before the path
-to the file above.
-
-More detailed python environment installation instructions using conda can be found in
-`examples/00_python_virtual_env.ipynb`.
-
-There are also .txt equivalents that can be used for installing from pip, like so:
-
-```pip install -r env_of_choice.txt```
-
-though these are not comprehensive installs as with conda and not tested.
-
-Once the python environment and dependencies are established and activated (`conda activate env_of_choice`),
-pywatershed is installed for development into that environment with the following command
-
-`cd pywatershed; pip install -e .`
-
-The numpy extension F2PY is used to provide fortran compiled kernels of core calculations to boost
-performance. F2PY is documented [within numpy](https://numpy.org/doc/stable/f2py/index.html). This
-repository is configured NOT to compile on install by default. Currently, we have not established
-this compilation procedure for Windows. On linux and MacOS, compilation of fortran kernels on package
-installation is achieved by the following code:
-
-```
-export SETUPTOOLS_ENABLE_FEATURES="legacy-editable"
-export CC=path/to/gcc  # for example
-export FC=path/to/gfortran  # for example
-export PYWS_FORTRAN=true
-cd path/to/pywatershed
-pip install -e .
-```
-
-Once the dependencies are available, we want to verify the software by running its test suite. The
-following testing procedures are also covered in the notebook `examples/01_automated_testing.ipynb`.
-To run the tests, we first need to generate the test data. This consists of running PRMS
-and then converting the output to netcdf:
-
-```
-cd path/to/pywatershed/test_data/scripts
-pytest -v -n=4 test_run_domains.py
-pytest -v -n=8 test_nc_domains.py
-```
-
-Finally, run the tests themselves,
-
-```
-cd path/to/pywatershed/autotest
-pytest -v -n=8
-```
-
-All tests should pass, XPASS, or XFAIL. XFAIL is an expected failure.
-
-
-Contributing
-============
-We welcome community development! Please file Issues and/or Pull Requests in the appropriate places on github. The continuous
-integration (CI) procedure is the first gate keeper for new code contribution. The CI procedure is defined by
-`.github/workflows/ci.yaml`. This includes running the formatting and linting packages `isort`, `black`, and
-`flake8` in addition to generating the test data and running the tests in `autotest/`. New codes need new tests so they can
-be verified moving ahead in time.
-
-
-Example Notebooks
-==================
-Jupyter notebooks containing examples are found in the
-[examples/](https://github.com/EC-USGS/pywatershed/tree/main/examples) directory. Numbered notebooks are tested.
-Notebooks 00 and 01 walk the user through the setting the python environment and running the software tests.
-Notebook 02 demonstrates modeling with pywatershed. Non-numbered notebooks cover additional topics. These notebooks
-are note yet covered by testing and so may be expected to have some issues until they are added to testing.
-
-
-Overview of Repository Contents
-==========
-The contents of directories at this level is described. Therein you may discover another README.md for more information.
-
-```
-.github/    Github actions for deploying continuous integration (CI)
-autotest/   pywatershed package testing using pytest
-bin/        PRMS executables distributed
-ci/         Python environments for CI
-doc/        Package/code documentation source code
-examples/   How to use the package, mostly jupyter notebooks
-prms_src/   PRMS source used for generating executables in bin/
-pywatershed/      Package source
-reference/  Ancillary materials for development
-resources/  Static stuff like images
-test_data/  Data used for automated testing
-```
-
-
-Disclaimer
-==========
-
-This information is preliminary or provisional and is subject to revision. It is being provided to meet the need for timely best science. The information has not received final approval by the U.S. Geological Survey (USGS) and is provided on the condition that neither the USGS nor the U.S. Government shall be held liable for any damages resulting from the authorized or unauthorized use of the information.
+Goals of the USGS Enterprise Capacity (EC) project include: * A sustainable
+integrated, hydrologic modeling framework for the U.S. Geological Survey (USGS)
+* Interoperable modeling across the USGS, partner agencies, and academia
+
+Goals for EC Watershed Modeling: * Couple the Precipitation-Runoff Modeling
+System (PRMS, e.g. Regan et al, 2018)  with MODFLOW 6 (MF6, e.g. Langevin et al,
+2017) in a sustainable way * Redesign PRMS to be more modern and flexible *
+Prioritize process representations in the current National Hydrological Model
+(NHM) based on PRMS 5.2.1
+
+Prototype an EC watershed model: "pywatershed" * Redesign PRMS quickly in python
+* Couple to MF6 via BMI/XMI interface (Hughes et al, 2021; Hutton et al, 2020) *
+Establish a prototyping ground for EC codes that couples to the compiled
+framework: low cost proof of concepts (at the price of potentially less
+computational performance) * Enable process representation hypothesis testing *
+Use cutting-edge techniques and technologies to improve models * Machine
+learning, automatic differentiation * Address challenges of modeling across
+space and time scales * Transition prototype watershed model to compiled EC code
+
+## Installation
+
+To install the software you will need Python 3.9 or 3.10.
+
+We currently recommend dependencies be installed with
+[Mamba](https://mamba.readthedocs.io/en/latest/) which will be much faster than
+Ananconda (but the conda command can also be used). An environment containing
+all core and optional dependencies can be created from the project root with:
+
+```mamba env create -f environment_w_jupyter.yml```
+
+(The environment `environment.yml` does not contain jupyter or jupyterlab
+in order to not interfere with installation in WholeTale, see Example
+Notebooks seection below.)
+
+The `pywatershed` package is [available on
+PyPI](https://pypi.org/project/pywatershed/). At the moment, the installation
+may not be reliable on all platforms and we are working to fix this.
+
+Using PyPI (with the above caveat), `pywatershed` can be installed with:
+
+``` pip install pywatershed ```
+
+A number of extra dependencies are needed to run the example notebooks. These
+can be installed with pip with
+
+``` pip install "pywatershed[optional]" ```
+
+These installation steps are suitable for `pywatershed` end users. See the
+[developer documentation](./DEVELOPER.md) for detailed instructions on
+configuring a development environment.
+
+## Contributing
+
+See the [developer documentation](./DEVELOPER.md) for instructions on setting up
+a development environment. See the [contribution guide](./CONTRIBUTING.md) to
+contribute to this project.
+
+## Example Notebooks
+
+For introductory example notebooks, look in the
+[`examples/`](https://github.com/EC-USGS/pywatershed/tree/main/examples>)
+directory in the repository. Numbered starting at 00, these are meant to be
+completed in order. Non-numbered notebooks coveradditional topics. These
+notebooks are note yet covered by testing and so may be expected to have some
+issues until they are added to testing. In `examples/developer/` there are
+notebooks of interest to developers who may want to learn about running the
+software tests.
+
+Though no notebook outputs are saved in Github, these notebooks can easily
+navigated to and run in WholeTale containers (free but sign-up or log-in
+required). This is a very easy and quick way to get started without needing to
+install pywatershed requirements yourself. WholeTale is an NSF funded project
+and supports logins from many institutions, e.g. the USGS, and you may not need
+to register.
+
+There are containers for both the `main` and `develop` branches.
+
+[![WholeTale](https://raw.githubusercontent.com/whole-tale/wt-design-docs/master/badges/wholetale-explore.svg)](https://dashboard.wholetale.org)
+* [WholeTale container for latest release (main
+  branch)](https://dashboard.wholetale.org/run/64ae29e8a887f48b9f173678?tab=metadata)
+* [WholeTale container for develop
+  branch](https://dashboard.wholetale.org/run/64ae25c3a887f48b9f1735c8?tab=metadata)
+
+WholeTale will give you a jupyter-lab running in the root of this
+repository. You can navigate to `examples/` and then open and run the notebooks
+of your choice.  The develop container may require the user to update the
+repository (`git pull origin`) to stay current with development.
+
+## Overview of Repository Contents
+
+The contents of directories at this level is described. Therein you may discover
+another README.md for more information.
+
+```
+.github/: Github actions, scripts and Python environments for continuous integration (CI) and releasing,
+asv_benchmarks/: preformance benchmarking by ASV
+autotest/: pywatershed package testing using pytest
+autotest_exs/: pywatershed example notebook testing using pytest
+bin/:PRMS executables distributed
+doc/:Package/code documentation source code
+evaluation/: tools for evaluation of pywatershed
+examples/:How to use the package, mostly jupyter notebooks
+prms_src/:PRMS source used for generating executables in bin/
+pywatershed/:Package source
+reference/:Ancillary materials for development
+resources/:Static stuff like images
+test_data/:Data used for automated testing
+```
+
+## Disclaimer
+
+This information is preliminary or provisional and is subject to revision. It is
+being provided to meet the need for timely best science. The information has not
+received final approval by the U.S. Geological Survey (USGS) and is provided on
+the condition that neither the USGS nor the U.S. Government shall be held liable
+for any damages resulting from the authorized or unauthorized use of the
+information.
 
 From: https://www2.usgs.gov/fsp/fsp_disclaimers.asp#5
 
-This software is in the public domain because it contains materials that originally came from the U.S. Geological Survey, an agency of the United States Department of Interior. For more information, see the [official USGS copyright policy](https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits "official USGS copyright policy")
-
-Although this software program has been used by the USGS, no warranty, expressed or implied, is made by the USGS or the U.S. Government as to the accuracy and functioning of the program and related program material nor shall the fact of distribution constitute any such warranty, and no responsibility is assumed by the USGS in connection therewith.
-This software is provided "AS IS."
+This software is in the public domain because it contains materials that
+originally came from the U.S. Geological Survey, an agency of the United States
+Department of Interior. For more information, see the [official USGS copyright
+policy](https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits
+"official USGS copyright policy")
+
+Although this software program has been used by the USGS, no warranty, expressed
+or implied, is made by the USGS or the U.S. Government as to the accuracy and
+functioning of the program and related program material nor shall the fact of
+distribution constitute any such warranty, and no responsibility is assumed by
+the USGS in connection therewith.  This software is provided "AS IS."
```

### Comparing `pywatershed-0.1.2/pyproject.toml` & `pywatershed-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -18,64 +18,83 @@
 keywords = ["hydrology", "PRMS"]
 license = { text = "CC0" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Hydrology",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9,<3.11"
 dependencies = [
     "numpy >=1.15.0",
-    "matplotlib  >=1.4.0",
+    "matplotlib >=1.4.0",
     "epiweeks",
     "netCDF4",
     "networkx",
     "numpy",
     "numba",
-    "pandas",
+    "pandas >= 1.4.0",
     "pint",
-    "pydot",
-    "xarray",
-    "cartopy",
-    "geopandas",
-    "hvplot",
-    "shapely",
-    "ipython",
-    "xmltodict",
     "pyyaml",
+    "tqdm",
+    "xarray >= 2023.5.0",
+    "xmltodict",
 ]
 dynamic = ["version", "readme"]
 
 [project.optional-dependencies]
 lint = [
     "cffconvert",
     "black",
     "click",
     "isort",
     "flake8",
     "pylint",
     "flynt",
+    "pre-commit",
 ]
 test = [
     "pywatershed[lint]",
     "coverage",
     "flaky",
+    "flopy",
+    "filelock",
     "modflow-devtools",
+    "pre-commit",
     "pytest",
     "pytest-cov",
     "pytest-env",
     "pytest-order",
     "pytest-xdist",
 ]
+optional = [
+    "pydot",
+    "geos",
+    "cartopy",
+    "geopandas",
+    "hvplot",
+    "shapely <2.0.0",
+    "ipython",
+    "jupyter",
+    "jupyterlab",
+]
+doc = [
+    "ipython",
+    "jinja2<3.1",
+    "sphinx",
+    "sphinx-book-theme>=0.3.3",
+    "sphinx-autosummary-accessors",
+    "sphinx-copybutton"
+]
+all = [
+    "pywatershed[lint, test, optional, doc]",
+]
 
 [project.urls]
 Documentation = "https://pywatershed.readthedocs.io"
 "Bug Tracker" = "https://github.com/EC-USGS/pywatershed/issues"
 "Source Code" = "https://github.com/EC-USGS/pywatershed"
 
 [tool.setuptools]
@@ -87,14 +106,15 @@
 readme = { file = ["README.md"], content-type = "text/markdown" }
 
 [tool.setuptools.packages.find]
 include = ["pywatershed", "pywatershed.*"]
 
 [tool.setuptools.package-data]
 "pywatershed.static.metadata" = ["*.yaml"]
+"pywatershed.data" = ["*.nc"]
 
 [tool.black]
 line-length = 79
 target_version = ["py39"]
 
 [tool.flynt]
 line-length = 79
```

### Comparing `pywatershed-0.1.2/pywatershed/__init__.py` & `pywatershed-0.2.0/pywatershed/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from .analysis.model_graph import ModelGraph
 from .analysis.utils.colorbrewer import ColorBrewer
-from .atmosphere.PRMSAtmosphere import PRMSAtmosphere
-from .atmosphere.PRMSSolarGeometry import PRMSSolarGeometry
+from .atmosphere.prms_atmosphere import PRMSAtmosphere
+from .atmosphere.prms_solar_geometry import PRMSSolarGeometry
 from .base import meta
-from .base.accessor import Accessor
 from .base.adapter import Adapter
 from .base.budget import Budget
 from .base.control import Control
 from .base.model import Model
 from .base.parameters import Parameters
-from .base.storageUnit import StorageUnit
+from .base.process import Process
 from .base.timeseries import TimeseriesArray
-from .hydrology.PRMSCanopy import PRMSCanopy
-from .hydrology.PRMSChannel import PRMSChannel
-from .hydrology.PRMSEt import PRMSEt
-from .hydrology.PRMSGroundwater import PRMSGroundwater
-from .hydrology.PRMSRunoff import PRMSRunoff
-from .hydrology.PRMSSnow import PRMSSnow
-from .hydrology.PRMSSoilzone import PRMSSoilzone
+from .hydrology.prms_canopy import PRMSCanopy
+from .hydrology.prms_channel import PRMSChannel
+from .hydrology.prms_et import PRMSEt
+from .hydrology.prms_groundwater import PRMSGroundwater
+from .hydrology.prms_runoff import PRMSRunoff
+from .hydrology.prms_snow import PRMSSnow
+from .hydrology.prms_soilzone import PRMSSoilzone
+from .hydrology.starfit import Starfit
 from .utils import (
     ControlVariables,
     NetCdfCompare,
     NetCdfRead,
     NetCdfWrite,
     Soltab,
 )
 from .utils.csv_utils import CsvFile
-from .version import __author__, __author_email__, __version__
+from .version import __version__
 
 __all__ = [
     "analysis",
     "atmosphere",
     "base",
     "hydrology",
     "utils",
```

### Comparing `pywatershed-0.1.2/pywatershed/analysis/model_graph.py` & `pywatershed-0.2.0/pywatershed/analysis/model_graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,146 +1,142 @@
 import pathlib as pl
 import tempfile
 import warnings
+from pprint import pprint
 
+from ..base.conservative_process import ConservativeProcess
 from ..base.model import Model
-
-try:
-    import pydot
-
-    has_pydot = True
-except ModuleNotFoundError:
-    has_pydot = False
-
-try:
-    from IPython.display import SVG, display
-
-    has_ipython = True
-except ModuleNotFoundError:
-    has_ipython = False
+from ..utils import import_optional_dependency
 
 
 class ModelGraph:
     def __init__(
         self,
         model: Model,
         show_params: bool = False,
         process_colors: dict = None,
         node_penwidth: int = 2,
         default_edge_color: str = "black",
         from_file_edge_color: str = None,
         node_spacing: float = 2.75,
         hide_variables: bool = True,
     ):
-        if not has_pydot:
-            warnings.warn("pydot not available")
+        self.pydot = import_optional_dependency("pydot")
+        self.graph = None
 
         self.model = model
         self.show_params = show_params
         self.process_colors = process_colors
         self.node_penwidth = node_penwidth
         self.default_edge_color = default_edge_color
         if not from_file_edge_color:
             self.from_file_edge_color = default_edge_color
         else:
             self.from_file_edge_color = from_file_edge_color
         self.node_spacing = node_spacing
         self.hide_variables = hide_variables
 
-        self.graph = None
-
         return
 
     def build_graph(self):
         # Build the process nodes in the graph
         self._current_pos = self.node_spacing
         self.process_nodes = {}
         for process in self.model.process_order:
             self.process_nodes[process] = self._process_node(
-                self.model.processes[process], show_params=self.show_params
+                process,
+                self.model.processes[process],
+                show_params=self.show_params,
             )
 
         # Solve the connections
-        files = []
-        connections = []
+        self.files = []
+        self.connections = []
         for process in self.model.process_order:
             frm_already = []
             for var, frm in self.model.process_input_from[process].items():
                 var_con = f":{var}"
+
                 if self.hide_variables:
                     var_con = ""
                     if frm in frm_already:
                         # print(f"skipping: {frm}")
                         continue
                     else:
                         frm_already += [frm]
                         # print(frm_already)
 
                 if not isinstance(frm, pl.Path):
                     color = self.default_edge_color
                     if self.process_colors:
                         color = self.process_colors[frm]
-                    connections += [
-                        (f"{frm}{var_con}", f"{process}{var_con}", color)
+                    self.connections += [
+                        (
+                            f"{frm}{var_con}",
+                            f"{process}{var_con}",
+                            color,
+                        )
                     ]
+
                 else:
                     file_name = frm.name
-                    files += [file_name]
-                    connections += [
+                    self.files += [file_name]
+                    self.connections += [
                         (
                             f"Files:{file_name.split('.')[0]}",
                             f"{process}{var_con}",
                             self.from_file_edge_color,
                         )
                     ]
 
         # Build the file node, reset the position
         self._current_pos = 0
-        self.file_node = self._file_node(files)
+        self.file_node = self._file_node(self.files)
 
         # build the graph
-        self.graph = pydot.Dot(
+        self.graph = self.pydot.Dot(
             graph_type="digraph",
             layout="neato",
             splines="polyline",
         )
 
         self.graph.add_node(self.file_node)
 
         for process in self.model.process_order:
             self.graph.add_node(self.process_nodes[process])
 
-        for con in connections:
-            self.graph.add_edge(pydot.Edge(con[0], con[1], color=con[2]))
+        for con in self.connections:
+            self.graph.add_edge(self.pydot.Edge(con[0], con[1], color=con[2]))
 
         return
 
-    def SVG(self, verbose: bool = False):
+    def SVG(self, verbose: bool = False, dpi=45):
         """Display an SVG in jupyter notebook (via tempfile)."""
 
-        if not has_ipython:
-            warnings.warn("IPython is not available")
+        ipdisplay = import_optional_dependency("IPython.display")
+
         tmp_file = pl.Path(tempfile.NamedTemporaryFile().name)
         if self.graph is None:
             self.build_graph()
-        self.graph.write_svg(tmp_file)
+        self.graph.write_svg(tmp_file, prog=["dot", f"-Gdpi={dpi}"])
         if verbose:
             print(f"Displaying SVG written to temp file: {tmp_file}")
 
-        display(SVG(tmp_file))
+        ipdisplay.display(ipdisplay.SVG(tmp_file))
         return
 
-    def _process_node(self, process, show_params: bool = False):
+    def _process_node(self, process_name, process, show_params: bool = False):
         inputs = process.get_inputs()
         variables = process.get_variables()
         params = process.get_parameters()
         cls = process.__class__.__name__
 
         label = (
             f'<<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="1">\n'
+            f'    <TR><TD COLSPAN="6">"{process_name}"</TD></TR>\n'
             f'    <TR><TD COLSPAN="6">{cls}</TD></TR>\n'
         )
 
         category_colors = {
             "inputs": "lightblue",
             "params": "orange",
             "variables": "lightgreen",
@@ -150,19 +146,22 @@
             "inputs": inputs,
             "params": params,
             "variables": variables,
         }
         if not show_params:
             _ = show_categories.pop("params")
 
-        mass_budget_vars = [
-            var
-            for comp, vars in process.get_mass_budget_terms().items()
-            for var in vars
-        ]
+        if isinstance(process, ConservativeProcess):
+            mass_budget_vars = [
+                var
+                for comp, vars in process.get_mass_budget_terms().items()
+                for var in vars
+            ]
+        else:
+            mass_budget_vars = []
 
         for varset_name, varset in show_categories.items():
             n_vars = len(varset)
             if not n_vars:
                 continue
 
             varset_col_span = 2
@@ -179,29 +178,28 @@
             label += f"    </TR>\n"
 
             for ii, vv in enumerate(sorted(varset)):
                 border_color_str = ""
                 if vv in mass_budget_vars:
                     border_color_str = 'border="1" COLOR="BLUE"'
                 label += f"    <TR>\n"
-                label += f'        <TD COLSPAN="4" BGCOLOR="{category_colors[varset_name]}" {border_color_str} PORT="{vv}" ><FONT POINT-SIZE="9.0">{vv}</FONT></TD>\n'
+                label += f'        <TD COLSPAN="4" BGCOLOR="{category_colors[varset_name]}" {border_color_str} PORT="{vv}"><FONT POINT-SIZE="9.0">{vv}</FONT></TD>\n'
                 label += f"    </TR>\n"
 
         label += f"</TABLE>>\n"
         label = label
 
         color_str = ""
         if self.process_colors:
-            color_str = f'"{self.process_colors[cls]}"'
+            color_str = f'"{self.process_colors[process_name]}"'
 
-        node = pydot.Node(
-            cls,
+        node = self.pydot.Node(
+            process_name,
             label=label,
             pos=f'"{self._current_pos},0!"',
-            # shape="process",
             shape="box",
             color=color_str,
             penwidth=f'"{self.node_penwidth}"',
         )
         self._current_pos += self.node_spacing
 
         return node
@@ -216,15 +214,15 @@
         for file in files:
             label += f"    <TR>\n"
             label += f'        <TD COLSPAN="1"  BGCOLOR="gray50" PORT="{file.split(".")[0]}"><FONT POINT-SIZE="9.0">{file}</FONT></TD>\n'
             label += f"    </TR>\n"
 
         label += f"</TABLE>>\n"
         label = label
-        node = pydot.Node(
+        node = self.pydot.Node(
             "Files",
             label=label,
             pos=f'"{self._current_pos},0!"',
             shape="note",
             color=f'"{self.from_file_edge_color}"',
             penwidth=f'"{self.node_penwidth}"',
         )
```

### Comparing `pywatershed-0.1.2/pywatershed/analysis/process_plot.py` & `pywatershed-0.2.0/pywatershed/analysis/process_plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,84 +1,42 @@
 import pathlib as pl
 from textwrap import wrap
 
-try:
-    import cartopy.crs as ccrs
-
-    has_cartopy = True
-except ModuleNotFoundError:
-    has_cartopy = False
-
-try:
-    import geopandas as gpd
-
-    has_geopandas = True
-except ModuleNotFoundError:
-    has_geopandas = False
-
-try:
-    import hvplot.pandas  # noqa
-
-    has_hvplot = True
-except ModuleNotFoundError:
-    has_hvplot = False
-
+import matplotlib as mpl
+import matplotlib.pyplot as plt
 import numpy as np
-
-try:
-    import matplotlib as mpl
-    import matplotlib.pyplot as plt
-    from matplotlib.collections import LineCollection, PatchCollection
-    from matplotlib.colors import Normalize
-    from matplotlib.patches import Polygon
-
-    has_matplotlib = True
-except ModuleNotFoundError:
-    has_matplotlib = False
-
 import pandas as pd
-
-try:
-    import shapely
-
-    has_shapely = True
-except ModuleNotFoundError:
-    has_shapely = False
-
+from matplotlib.collections import LineCollection, PatchCollection
+from matplotlib.colors import Normalize
+from matplotlib.patches import Polygon
 
 from ..base import meta
 from ..base.model import Model
-from ..base.storageUnit import StorageUnit
+from ..base.process import Process
+from ..utils.optional_import import import_optional_dependency
 
 
 class ProcessPlot:
     def __init__(
         self,
         gis_dir: pl.Path,
         hru_shp_file_name: str = "HRU_subset.shp",
         seg_shp_file_name: str = "Segments_subset.shp",
     ):
-        if (
-            (not has_cartopy)
-            or (not has_geopandas)
-            or (not has_hvplot)
-            or (not has_matplotlib)
-            or (not has_shapely)
-        ):
-            msg = "Some required modules for ProcessPlot are not present."
-            raise ModuleNotFoundError(msg)
+        gpd = import_optional_dependency("geopandas")
 
         self.hru_shapefile = gis_dir / hru_shp_file_name
         self.seg_shapefile = gis_dir / seg_shp_file_name
 
         # HRU one-time setups
         self.hru_gdf = (
             gpd.read_file(self.hru_shapefile)
-            # .drop("nhm_id", axis=1)
-            .rename(columns={"nhru_v1_1": "nhm_id"}).set_index("nhm_id")
+            .drop("nhm_id", axis=1)
+            .rename(columns={"nhru_v1_1": "nhm_id"})
+            .set_index("nhm_id")
         )
 
         # segment one-time setup
         self.seg_gdf = gpd.read_file(self.seg_shapefile)
         # if (self.__seg_poly.crs.name == "USA_Contiguous_Albers_Equal_Area_Conic_USGS_version"):
         # print("Overriding USGS aea crs with EPSG:5070")
         self.seg_gdf.crs = "EPSG:5070"
@@ -89,31 +47,31 @@
             .drop("model_idx", axis=1)
             .rename(columns={"nsegment_v": "nhm_seg"})
             .set_index("nhm_seg")
         )
 
         return
 
-    def plot(self, var_name: str, process: StorageUnit, cmap: str = None):
-        var_dims = list(
-            meta.get_vars(var_name)[var_name]["dimensions"].values()
-        )
+    def plot(self, var_name: str, process: Process, cmap: str = None):
+        var_dims = list(meta.get_vars(var_name)[var_name]["dims"])
         if "nsegment" in var_dims:
             if not cmap:
                 cmap = "cool"
-            return self.plot_seg_var(self, var_name, process, cmap)
+            return self.plot_seg_var(var_name, process, cmap)
         elif "nhru" in var_dims:
-            return self.plot_hru_var(self, var_name, process)
+            return self.plot_hru_var(var_name, process)
         else:
             raise ValueError()
 
-    def plot_seg_var(self, var_name: str, process: StorageUnit, cmap="cool"):
+    def plot_seg_var(self, var_name: str, process: Process, cmap="cool"):
+        ccrs = import_optional_dependency("cartopy.crs")
+
         data_df = pd.DataFrame(
             {
-                "nhm_seg": process.control.params.parameters["nhm_seg"],
+                "nhm_seg": process.params.coords["nhm_seg"],
                 var_name: process[var_name],
             }
         ).set_index("nhm_seg")
 
         minx, miny, maxx, maxy = self.hru_gdf.geometry.total_bounds
         hru_geoms_exploded = self.hru_gdf.explode().reset_index(
             level=1, drop=True
@@ -187,33 +145,44 @@
             params_vars = list(set(proc.variables) | set(proc.parameters))
             if var_name in params_vars:
                 process = proc
                 break
 
         data_df = pd.DataFrame(
             {
-                "nhm_id": process.control.params.parameters["nhm_id"],
+                "nhm_id": process.params.coords["nhm_id"],
                 var_name: process[var_name],
             }
         ).set_index("nhm_id")
         return data_df
 
-    def plot_hru(
+    def plot_hru_var(
         self,
         var_name: str,
-        model: Model = None,
+        process: Process,
         data: np.ndarray = None,
         data_units: str = None,
         nhm_id: np.ndarray = None,
     ):
+        _ = import_optional_dependency("hvplot.pandas")
+
+        ccrs = import_optional_dependency("cartopy.crs")
+
         if data is None:
-            data_df = self.get_hru_var(var_name, model)
+            # data_df = self.get_hru_var(var_name, model)
+            data_df = pd.DataFrame(
+                {
+                    "nhm_id": process.params.coords["nhm_id"],
+                    var_name: process[var_name],
+                }
+            ).set_index("nhm_id")
+
         else:
             if nhm_id is None:
-                nhm_id = model.control.params.parameters["nhm_id"]
+                nhm_id = model.parameters["nhm_id"]
             data_df = pd.DataFrame(
                 {
                     "nhm_id": nhm_id,
                     var_name: data,
                 }
             ).set_index("nhm_id")
 
@@ -243,14 +212,15 @@
             tiles=True,
             crs=ccrs.epsg(5070),
             frame_height=frame_height,
             c=var_name,
             line_width=0,
             alpha=0.75,
             # clim=stat_lims[stat],
+            hover_cols=["nhm_id"],
             title=title,
             clabel=clabel,
             xlabel="Longitude (degrees East)",
             ylabel="Latitude (degrees North)",
         )
         return plot
 
@@ -265,14 +235,16 @@
     vary_color=True,
     colors=None,
     alpha=1.0,
     linewidth=1.0,
     **kwargs,
 ):
     """Plot a collection of line geometries"""
+    shapely = import_optional_dependency("shapely")
+
     lines = []
     for geom in geoms:
         a = np.asarray(geom.coords)
 
         if geom.has_z:
             a = shapely.geometry.LineString(zip(*geom.xy))
 
@@ -312,14 +284,16 @@
     edgecolor=None,
     alpha=1.0,
     linewidth=1.0,
     **kwargs,
 ):
     """Plot a collection of Polygon geometries"""
     # from https://stackoverflow.com/questions/33714050/geopandas-plotting-any-way-to-speed-things-up
+    shapely = import_optional_dependency("shapely")
+
     patches = []
 
     for poly in geoms:
         a = np.asarray(poly.exterior)
         if poly.has_z:
             a = shapely.geometry.Polygon(zip(*poly.exterior.xy))
```

### Comparing `pywatershed-0.1.2/pywatershed/analysis/utils/colorbrewer.py` & `pywatershed-0.2.0/pywatershed/analysis/utils/colorbrewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # for updates to copyright information.
 
 # Translation to Python by David Schoonover and released under the MIT license.
 
 from typing import Union
 
 from ...base.model import Model
+from ...utils.optional_import import import_optional_dependency
 
 
 class ColorBrewer:
     def __init__(self):
         self.format = "hex"
         self._possible_formats = ["hex", "rgb"]
         self.palettes_by_cat = palettes_by_cat
@@ -2341,38 +2342,40 @@
         "PRMSSoilzone": palette[6],
         "PRMSGroundwater": palette[7],
         "PRMSChannel": palette[4],
     }
     if not model:
         return process_colors
     else:
-        model_processes = list(model.processes.keys())
+        model_proc_cls = {
+            key: val.__class__.__name__ for key, val in model.processes.items()
+        }
         model_process_colors = {
-            key: val
-            for key, val in process_colors.items()
-            if key in [cc for cc in model_processes]
+            name: process_colors[cls]
+            for name, cls in model_proc_cls.items()
+            if cls in model_proc_cls.values()
         }
         return model_process_colors
 
 
 def jupyter_palette(palette: Union[list, dict]):
-    from IPython.display import Markdown, display
+    ipdisplay = import_optional_dependency("IPython.display")
 
     if isinstance(palette, list):
-        display(
-            Markdown(
+        ipdisplay.display(
+            ipdisplay.Markdown(
                 "<br>".join(
                     f'<span style="font-family: monospace">{color} <span style="color: {color}">████████</span></span>'
                     for color in palette
                 )
             )
         )
     else:
-        display(
-            Markdown(
+        ipdisplay.display(
+            ipdisplay.Markdown(
                 "<br>".join(
                     f'<span style="font-family: monospace">{key} <span style="color: {color}">████████</span></span>'
                     for key, color in palette.items()
                 )
             )
         )
```

### Comparing `pywatershed-0.1.2/pywatershed/atmosphere/PRMSAtmosphere.py` & `pywatershed-0.2.0/pywatershed/atmosphere/prms_atmosphere.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import pathlib as pl
+from warnings import warn
 
 import numpy as np
 
-from pywatershed.base.storageUnit import StorageUnit
+from pywatershed.base.process import Process
 from pywatershed.utils.netcdf_utils import NetCdfWrite
 
-from ..base import meta
 from ..base.adapter import adaptable
 from ..base.control import Control
 from ..constants import epsilon, inch2cm, nan, one, zero
+from ..parameters import Parameters
 from ..utils.time_utils import datetime_doy, datetime_month
 from .solar_constants import solf
 
 
 # may not use this if they cant be called with jit
 # if it can, put it in a common utility.
 def tile_space_to_time(arr: np.ndarray, n_time) -> np.ndarray:
     return np.tile(arr, (n_time, 1))
 
 
 def tile_time_to_space(arr: np.ndarray, n_space) -> np.ndarray:
     return np.transpose(np.tile(arr, (n_space, 1)))
 
 
-class PRMSAtmosphere(StorageUnit):
+class PRMSAtmosphere(Process):
     """PRMS atmospheric boundary layer model.
 
     Implementation based on PRMS 5.2.1 with theoretical documentation based on
     PRMS-IV:
 
     Markstrom, S. L., Regan, R. S., Hay, L. E., Viger, R. J., Webb, R. M.,
     Payn, R. A., & LaFontaine, J. H. (2015). PRMS-IV, the
@@ -37,82 +38,76 @@
 
     This representation uses precipitation and temperature inputs. Relative
     humidity could be added as well.
 
     The boundary layer calculates and manages the following variables (given
     by PRMSAtmosphere.get_variables()):
 
-        tmaxf,
-        tminf,
-        prmx,
-        hru_ppt,
-        hru_rain,
-        hru_snow,
-        swrad,
-        potet,
-        transp_on,
+    *tmaxf, tminf, prmx, hru_ppt, hru_rain, hru_snow, swrad, potet, transp_on*
 
     PRMS adjustments to temperature and precipitation are applied here to
     the inputs. Shortwave radiation (using degree day method) and potential
     evapotranspiration (Jensen and Haise ,1963) and a temperature based
     transpiration flag (transp_on) are also calculated.
 
     Note that all variables are calculated for all time upon initialization and
     that all calculated variables are written to netcdf (when netcdf output is
     requested) prior to the first model advance. This is effectively a complete
     preprocessing of the input CBH files to the fields the model actually uses
     on initialization. If you just want to preprocess these variables, see
     `this notebook <https://github.com/EC-USGS/pywatershed/tree/main/examples/preprocess_cbh_adj.ipynb>`_.
 
-
     The full time version of a variable is given by the "private" version of
     the variable which is named with a single-leading underscore (eg tmaxf for
     all time is _tmaxf).
 
     This full-time initialization ma not be tractable for large domains and/or
     long periods of time and require changes to batch the processing of the
     variables. The benefits of full-time initialization are 1) the code is
     vectorized and fast for such a large calculation, 2) the initialization of
     this class effectively preprocess all the inputs to the rest of the model
     and can then be skipped in subsequent model calls (unless the parameters
     are changing).
 
     Args:
-        control: control object
-        prcp: precipitation cbh netcdf file
-        tmax: maximum daily temperature cbh netcdf file
-        tmin: minimum daily temperature cbh netcdf file
-        soltab_potsw: potential shortwave radiation special format file. Only
-            the versions of PRMS 5.2.1 shipped with pywatershed output soltab in this
-            format
-        soltab_horad_potsw: this is the potential shortwave on the horizontal
-            plane at each HRU. See soltab_potsw comment on file format.
-        budget_type: [None | "warn" |  "error"].
-        verbose: bool indicating amount of output to terminal.
-        netcdf_output_dir: an existing directory to which to write all
-            variables for all time.
-        netcdf_output_vars: a list or subset of variables to output to netcdf
-        n_time_chunk: int = -1,
-        load_n_time_batches: int = 1,
+        control: a Control object
+        discretization: a discretization of class Parameters
+        parameters: a parameter object of class Parameters
+
+        prcp: daily precipitation
+        tmax: daily maximum temperature
+        tmin: daily minimum temperature
+        soltab_potsw: the solar table of potential shortwave radiation
+        soltab_horad_potsw: the solar table of potential shortwave
+            radiation on a horizontal plane
+
+        verbose: Print extra information or not?
+        netcdf_output_dir: A directory to write netcdf outpuf files
+        netcdf_output_vars: A list of variables to output via netcdf.
+        netcdf_separate_files: Separate or a single netcdf output file
+        load_n_time_batches: How often to load from disk (not-implemented?)
+        n_time_chunk: the inverse of load_n_time_batches, the number of
+           times in a chunk/batch (implemented?)
 
     """
 
     def __init__(
         self,
         control: Control,
+        discretization: Parameters,
+        parameters: Parameters,
         prcp: [str, pl.Path],
         tmax: [str, pl.Path],
         tmin: [str, pl.Path],
         soltab_potsw: adaptable,
         soltab_horad_potsw: adaptable,
-        budget_type: str = None,
         verbose: bool = False,
         netcdf_output_dir: [str, pl.Path] = None,
         netcdf_output_vars: list = None,
-        netcdf_separate_files: bool = True,
+        netcdf_separate_files: bool = None,
         # from_file_dir: [str, pl.Path] = None,
         n_time_chunk: int = -1,
         load_n_time_batches: int = 1,
     ):
         # Defering handling batch handling of time chunks but self.n_time_chunk
         # is a dimension used in the metadata/variables dimensions.
         # TODO: make time chunking options work (esp with output)
@@ -126,38 +121,35 @@
 
         metadata_patches = {
             kk: {"dims": ("ntime", "nhru")} for kk in self.variables
         }
 
         super().__init__(
             control=control,
-            verbose=verbose,
-            load_n_time_batches=load_n_time_batches,
+            discretization=discretization,
+            parameters=parameters,
             metadata_patches=metadata_patches,
             metadata_patch_conflicts="left",
         )
-        # need to override the initailization of self variables
-        self._set_inputs(locals())
-
         self.name = "PRMSAtmosphere"
-        self.budget = None
+
+        self._set_inputs(locals())
+        self._set_options(locals())
 
         self._calculated = False
 
+        self._netcdf_initialized = False
         self.netcdf_output_dir = netcdf_output_dir
         if self.netcdf_output_dir:
             self.initialize_netcdf(
                 output_dir=pl.Path(netcdf_output_dir),
                 separate_variables=netcdf_separate_files,
                 output_vars=netcdf_output_vars,
             )
 
-        else:
-            self._output_netcdf = False
-
         return
 
     def _calculate_all_time(self):
         if self._calculated:
             return
 
         # Eventually refactor to work at specific chunks of time
@@ -185,40 +177,27 @@
 
         self.adjust_temperature()
         self.adjust_precip()
         self.calculate_sw_rad_degree_day()
         self.calculate_potential_et_jh()
         self.calculate_transp_tindex()
 
-        # Budget is not for all time
-        # self.set_budget(budget_type)
-        # This is a nonstandard budget.
-        self.budget = None
-        # self.budget = {
-        #     "inputs": {"potet": self.potet},
-        #     "outputs": {"hru_actet": self.hru_actet},
-        #     "storage_changes": {"available_potet": self.available_potet},
-        # }
-
         # JLM todo: delete large variables on self for memory management
         self._calculated = True
 
         return
 
     @staticmethod
     def get_dimensions():
-        return (
-            "nhru",
-            "nmonth",
-            "ntime",
-        )
+        return ("nhru", "nmonth", "ndoy", "ntime")
 
     @staticmethod
     def get_parameters():
         return (
+            "doy",
             "radadj_intcp",
             "radadj_slope",
             "tmax_index",
             "dday_slope",
             "dday_intcp",
             "radmax",
             "ppt_rad_adj",
@@ -311,38 +290,21 @@
             "orad_hru": nan,
         }
 
     def _set_initial_conditions(self):
         return
 
     def _advance_variables(self):
-        """Advance the PRMSAtmosphere
-
-        Returns:
-            None
-
-        """
         if not self._calculated:
             self._calculate_all_time()
         for vv in self.variables:
             self[vv].advance()
         return
 
     def _calculate(self, time_length):
-        """Calculate PRMSAtmosphere"
-
-        Sets the current value to the precalculated values.
-
-        Args:
-            time_length: time step length
-
-        Returns:
-            None
-
-        """
         return
 
     def adjust_temperature(self):
         """Input temperature adjustments using calibrated parameters."""
 
         # throw an error if these have different shapes
         if self["tmax_cbh_adj"].shape != self["tmin_cbh_adj"].shape:
@@ -374,14 +336,17 @@
         return
 
     def adjust_precip(self):
         """Input precipitation adjustments using calibrated parameters.
 
         Snow/rain partitioning of total precip depends on adjusted temperature
         in addition to depending on additonal parameters.
+
+        Returns:
+            None
         """
 
         ivd = self._input_variables_dict
 
         # throw an error shapes are inconsistent
         shape_list = np.array(
             [
@@ -472,15 +437,20 @@
             ivd["prcp"].data * self.rain_cbh_adj[month_ind]
         )[wh_all_rain]
         self.hru_rain.data[wh_all_rain] = self.hru_ppt.data[wh_all_rain]
         self.hru_snow.data[wh_all_rain] = zero
         return
 
     def calculate_sw_rad_degree_day(self) -> None:
-        """Calculate shortwave radiation using the degree day method."""
+        """Calculate shortwave radiation using the degree day method.
+
+        Returns:
+            None
+
+        """
 
         solar_params = {}
         solar_param_names = (
             "radadj_intcp",
             "radadj_slope",
             "tmax_index",
             "dday_slope",
@@ -660,16 +630,20 @@
         orad_hru = radadj * doy_to_daily(soltab_horad_potsw)
         return swrad, orad_hru
 
     # https://github.com/nhm-usgs/prms/blob/6.0.0_dev/src/prmslib/physics/sm_potet_jh.f90
 
     def calculate_potential_et_jh(self) -> None:
         """Calculate potential evapotranspiration following Jensen and Haise
-        (1963)."""
 
+        Jensen and Haise (1963)
+
+        Returns:
+            None
+        """
         self.potet.data[:] = self._potet_jh_run(
             dates=self._time,
             tavgc=self.tavgc.data,
             swrad=self.swrad.data,
             jh_coef=self.jh_coef,
             jh_coef_hru=self.jh_coef_hru,
             nmonth=self.nmonth,
@@ -715,15 +689,15 @@
     #     return et
 
     def calculate_transp_tindex(self):
         # INIT: Process_flag==INIT
         # transp_on inited to 0 everywhere above
 
         # candidate for worst code lines
-        if self.control.params.get_parameters("temp_units")["temp_units"] == 0:
+        if self.params.parameters["temp_units"] == 0:
             transp_tmax_f = self.transp_tmax
         else:
             transp_tmax_f = (self.transp_tmax * (9.0 / 5.0)) + 32.0
 
         transp_check = self.transp_on.current.copy()  # dim nhrus only
         tmax_sum = self.transp_on.current.copy().astype(
             "float64"
@@ -802,20 +776,20 @@
                         transp_check[hh] = 0
                         tmax_sum[hh] = 0.0
 
         # <<<
         return
 
     def _write_netcdf_timeseries(self) -> None:
-        if not self._output_netcdf:
+        if not self._netcdf_initialized:
             return
 
         if self.netcdf_separate_files:
             for var in self.variables:
-                if var not in self.netcdf_output_vars:
+                if var not in self._netcdf_output_vars:
                     continue
                 nc_path = self.netcdf_output_dir / f"{var}.nc"
 
                 nc = NetCdfWrite(
                     nc_path,
                     self.params.coords,
                     [var],
@@ -831,58 +805,69 @@
                 print(f"Wrote file: {nc_path}")
 
         else:
             nc_path = self.netcdf_output_dir / f"{self.name}.nc"
             nc = NetCdfWrite(
                 nc_path,
                 self.params.coords,
-                self.netcdf_output_vars,
+                self._netcdf_output_vars,
                 self.meta,
             )
             for var in self.variables:
-                if var not in self.netcdf_output_vars:
+                if var not in self._netcdf_output_vars:
                     continue
                 nc.add_all_data(
                     var,
                     self[var].data,
                     self._time,
                 )
 
             nc.close()
             assert nc_path.exists()
             print(f"Wrote file: {nc_path}")
 
-        self._output_netcdf = False
-        return
-
-    def _finalize_netcdf(self) -> None:
+        self._finalize_netcdf()
         return
 
     def initialize_netcdf(
         self,
         output_dir: [str, pl.Path],
         separate_files: bool = True,
         output_vars: list = None,
         **kwargs,
     ):
-        self._output_netcdf = True
+        if self._netcdf_initialized:
+            msg = (
+                f"{self.name} class previously initialized netcdf output "
+                f"in {self._netcdf_output_dir}"
+            )
+            warn(msg)
+            return
+
+        self._netcdf_initialized = True
         self.netcdf_separate_files = separate_files
         self.netcdf_output_dir = output_dir
         if output_vars is None:
-            self.netcdf_output_vars = self.variables
+            self._netcdf_output_vars = self.variables
         else:
-            self.netcdf_output_vars = output_vars
+            self._netcdf_output_vars = list(
+                set(output_vars).intersection(set(self.variables))
+            )
+
+        if self._netcdf_output_vars is None:
+            self._netcdf_initialized = False
 
         return
 
     def _finalize_netcdf(self) -> None:
+        self._netcdf_initialized = False
         return
 
     def output(self):
-        if self._output_netcdf:
-            if self.verbose:
+        if self._netcdf_initialized:
+            if self._verbose:
                 print(
                     f"Writing FULL timeseries output for: {self.name}",
                     flush=True,
                 )
             self._write_netcdf_timeseries()
         return
```

### Comparing `pywatershed-0.1.2/pywatershed/atmosphere/PRMSSolarGeometry.py` & `pywatershed-0.2.0/pywatershed/atmosphere/prms_solar_geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,122 @@
 import pathlib as pl
 import warnings
 from typing import Tuple
 
 import numpy as np
 
-# would like to not subclass storageUnit but it is much simpler to do so
-from pywatershed.base.storageUnit import StorageUnit
+from pywatershed.base.process import Process
 from pywatershed.utils.netcdf_utils import NetCdfWrite
 
 from ..base.control import Control
 from ..constants import epsilon32, nan, one, zero
+from ..parameters import Parameters
 from ..utils.prms5util import load_soltab_debug
 from .solar_constants import ndoy, pi, pi_12, r1, solar_declination, two_pi
 
 epsilon = epsilon32
 
 doy = np.arange(ndoy) + 1
 
-# The solar geometry model for NHM/PRMS
-# Primary reference
-# * Appendix E of Dingman, S. L., 1994,
-#   Physical Hydrology. Englewood Cliffs, NJ: Prentice Hall, 575 p.
-
 # Dimensions
 # The cyclic time dimension is ndoy (known apriori)
 # The spatial dimension n_hru (only known on init from parameters)
 
 
 def tile_space_to_time(arr: np.ndarray) -> np.ndarray:
     return np.tile(arr, (ndoy, 1))
 
 
 # def tile_time_to_space(arr: np.ndarray, n_hru) -> np.ndarray:
 #    return np.transpose(np.tile(arr, (n_hru, 1)))
 
 
-class PRMSSolarGeometry(StorageUnit):
-    """PRMS solar geometry."""
+class PRMSSolarGeometry(Process):
+    """PRMS solar geometry.
+
+    Swift's daily potential solar radiation and number of hours
+    of duration on a sloping surface in [cal/cm2/day].
+    Swift, 1976, equation 6.
+
+    Primary reference: Appendix E of Dingman, S. L., 1994, Physical Hydrology.
+    Englewood Cliffs, NJ: Prentice Hall, 575 p.
+
+    Args:
+        control: a Control object
+        discretization: a discretization of class Parameters
+        parameters: a parameter object of class Parameters
+        verbose: Print extra information or not?
+        from_prms_file: Load from a PRMS output file?
+        from_nc_files_dir: [str, pl.Path] = None,
+        load_n_time_batches: How often to load from disk (not-implemented?)
+        netcdf_output_dir: A directory to write netcdf outpuf files
+        netcdf_separate_files: Separate or a single netcdf output file
+        netcdf_output_vars: A list of variables to output via netcdf.
+
+    """
 
     def __init__(
         self,
         control: Control,
+        discretization: Parameters,
+        parameters: Parameters,
         verbose: bool = False,
         from_prms_file: [str, pl.Path] = None,
         from_nc_files_dir: [str, pl.Path] = None,
         load_n_time_batches: int = 1,
         netcdf_output_dir: [str, pl.Path] = None,
         netcdf_separate_files: bool = True,
         netcdf_output_vars: list = None,
     ):
-        # This is a singular case of having a constant parameter dimensions
-        self.ndoy = doy
-
-        budget_type = None
-        self._set_budget(budget_type)
         self.netcdf_output_dir = netcdf_output_dir
+
+        # self._time is needed by Process for timeseries arrays
+        # TODO: this is redundant because the parameter doy is set
+        #       on load of prms file. Could pass the name to use for
+        #       self._time to super or come up with some other work around.
         self._time = doy
 
         super().__init__(
             control=control,
-            verbose=verbose,
-            load_n_time_batches=load_n_time_batches,
+            discretization=discretization,
+            parameters=parameters,
         )
         self._set_inputs(locals())
+        self._set_options(locals())
         self.name = "PRMSSolarGeometry"
 
         if from_prms_file:
             (
                 self.soltab_potsw.data[:],
                 self.soltab_horad_potsw.data[:],
                 self.soltab_sunhrs.data[:],
             ) = load_soltab_debug(from_prms_file)
 
         elif from_nc_files_dir:
             raise NotImplementedError()
 
         self._calculated = False
 
+        self._netcdf_initialized = False
         if self.netcdf_output_dir:
             self._calculate_all_time()
             self.initialize_netcdf(
                 output_dir=pl.Path(netcdf_output_dir),
                 separate_variables=netcdf_separate_files,
                 output_vars=netcdf_output_vars,
             )
 
-        else:
-            self._output_netcdf = False
-
         return
 
     @staticmethod
     def get_inputs() -> tuple:
         return ()
 
     @staticmethod
     def get_variables():
-        """Get solar geometry variables
-
-        Returns:
-            variables: output variables
-
-        """
         return (
             "soltab_horad_potsw",
             "soltab_potsw",
             "soltab_sunhrs",
         )
 
     @staticmethod
@@ -119,14 +130,15 @@
     @staticmethod
     def get_dimensions() -> tuple:
         return ("nhru", "ndoy")
 
     @staticmethod
     def get_parameters() -> tuple:
         return (
+            "doy",
             "hru_slope",
             "radj_sppt",
             "radj_wppt",
             "hru_lat",
             "hru_area",
             "hru_aspect",
         )
@@ -157,61 +169,40 @@
             self.func3,
         )
 
         self._calculated = True
         return
 
     def _advance_variables(self):
-        """Advance solar geometry
-
-        Returns:
-            None
-
-        """
         if not self._calculated:
             self._calculate_all_time()
         for vv in self.variables:
             self[vv].advance()
         return
 
     def _calculate(self, time_length):
-        """Calculate solar_geom"
-
-        Sets the current value to the precalculated values.
-
-        Args:
-            time_length: time step length
-
-        Returns:
-            None
-
-        """
         return
 
     # @jit
     @staticmethod
     def compute_soltab(
         slopes: np.ndarray,
         aspects: np.ndarray,
         lats: np.ndarray,
         compute_t: callable,
         func3: callable,
     ) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        Swift's daily potential solar radiation and number of hours
-        of duration on a sloping surface in [cal/cm2/day].
-        Swift, 1976, equation 6.
-
-        Arguments:
+        """Calculate the solar table
+        Args:
           cossl: cos(atan(hru_slope)) [nhru] ?
           slope: slope [nhru]
           aspect: aspect [nhru]
           latitude: latitude [nhru]
 
-        Return Values: (solt, sunh)
+        Returns: (solt, sunh)
           solt: Swift's potential solar radiation on a sloping surface in
             [cal/cm2/day]. Swift, 1976, equation 6.
             Dimensions: [ndoy, nhru]
           sunh: The number of hours of direct sunlight
             Dimensions: [ndoy, nhru]
         """
         nhru = len(slopes)
@@ -337,32 +328,31 @@
 
         return solt, sunh
 
     @staticmethod
     def compute_t(
         lats: np.ndarray, solar_declination: np.ndarray
     ) -> np.ndarray:
-        # This function is
-        #   * named as in prms for historical purposes
-        #   * is for numba compilation
         # JLM: why is division by earth's angular velocity not done here?
-        """
-        The "sunrise" equation
-        lats - latitudes of the hrus
-        solar_declination: the declination of the sun on all julian days
-        result: the angle hour from the local meridian (local solar noon) to
+        """The "sunrise" equation
+
+        Args:
+            lats - latitudes of the hrus
+            solar_declination: the declination of the sun on all julian days
+        Returns:
+            The angle hour from the local meridian (local solar noon) to
             the sunrise (negative) or sunset (positive).  The Earth rotates at
             the angular speed of 15 degrees/hour (2 pi / 24 hour in radians)
             and, therefore, result*(24/(2pi) radians gives the time of sunrise
             as the number of hours before the local noon, or the time of sunset
             as the number of hours after the local noon. Here the term local
             noon indicates the local time when the sun is exactly to the
             south or north or exactly overhead.
 
-        https://github.com/nhm-usgs/prms/blob/6.0.0_dev/src/prmslib/physics/sm_solar_radiation.f90
+        See reference: https://github.com/nhm-usgs/prms/blob/6.0.0_dev/src/prmslib/physics/sm_solar_radiation.f90
         """
         nhru = len(lats)
         lats_mat = np.tile(-1 * np.tan(lats), (ndoy, 1))
         sol_dec_mat = np.transpose(
             np.tile(np.tan(solar_declination), (nhru, 1))
         )
         tx = lats_mat * sol_dec_mat
@@ -383,29 +373,36 @@
     @staticmethod
     def func3(
         v: np.ndarray,
         w: np.ndarray,
         x: np.ndarray,
         y: np.ndarray,
     ) -> np.ndarray:
-        """
-        This is the radian angle version of FUNC3 (eqn 6) from Swift, 1976
-        or Lee, 1963 equation 5.
-        result: (R4) is potential solar radiation on the surface cal/cm2/day [ndoy, nhru]
-        v: (L2) latitude angle hour offset between actual and equivalent slope [nhru]
-        w: (L1) latitude of the equivalent slope [nhru]
-        x: (T3) hour angle of sunset on equivalent slope [ndoy, nhru]
-        y: (T2) hour angle of sunrise on equivalent slope [ndoy, nhru]
-
-        # Constants
-        r1: solar constant for 60 minutes [ndoy]
-        solar_declination: declination of sun [ndoy]
+        """Potential solar radiation on the surface cal/cm2/day
 
-        https://github.com/nhm-usgs/prms/blob/6.0.0_dev/src/prmslib/physics/sm_solar_radiation.f90
+        Radian angle version of FUNC3 (eqn 6) from Swift, 1976
+        or Lee, 1963 equation 5. (Names in parens below from Swift?)
+
+        Args:
+            v: (L2) latitude angle hour offset between actual and equivalent
+               slope [nhru]
+            w: (L1) latitude of the equivalent slope [nhru]
+            x: (T3) hour angle of sunset on equivalent slope [ndoy, nhru]
+            y: (T2) hour angle of sunrise on equivalent slope [ndoy, nhru]
+
+        Returns:
+            (R4) is potential solar radiation on the surface cal/cm2/day [ndoy, nhru]
+
+        Constants
+            r1: solar constant for 60 minutes [ndoy]
+            solar_declination: declination of sun [ndoy]
+
+        See also: https://github.com/nhm-usgs/prms/blob/6.0.0_dev/src/prmslib/physics/sm_solar_radiation.f90
         """
+
         # Must alter the dimensions of the inputs to get the outputs.
         nhru = len(v)
         vv = np.tile(v, (ndoy, 1))
         ww = np.tile(w, (ndoy, 1))
         # These are known at init time, not sure they are worth saving in self
         # and passing
         rr = np.transpose(np.tile(r1, (nhru, 1)))
@@ -419,83 +416,97 @@
                 + np.cos(dd) * np.cos(ww) * (np.sin(x + vv) - np.sin(y + vv))
             )
         )
 
         return f3
 
     def _write_netcdf_timeseries(self) -> None:
-        if not self._output_netcdf:
+        if not self._netcdf_initialized:
             return
 
         if self.netcdf_separate_files:
             for var in self.variables:
-                if var not in self.netcdf_output_vars:
+                if var not in self._netcdf_output_vars:
                     continue
                 nc_path = self.netcdf_output_dir / f"{var}.nc"
 
                 nc = NetCdfWrite(
                     nc_path,
                     self.params.coords,
                     [var],
                     {var: self.meta[var]},
                 )
                 nc.add_all_data(
                     var,
                     self[var].data,
-                    self._time,
+                    self.doy,
                     time_coord="doy",
                 )
                 nc.close()
                 assert nc_path.exists()
                 print(f"Wrote file: {nc_path}")
 
         else:
             nc_path = self.netcdf_output_dir / f"{self.name}.nc"
             nc = NetCdfWrite(
                 nc_path,
                 self.params.coords,
-                self.netcdf_output_vars,
+                self._netcdf_output_vars,
                 self.meta,
             )
             for var in self.variables:
-                if var not in self.netcdf_output_vars:
+                if var not in self._netcdf_output_vars:
                     continue
                 nc.add_all_data(
                     var,
                     self[var].data,
-                    self._time,
+                    self.doy,
                     time_coord="doy",
                 )
 
             nc.close()
             assert nc_path.exists()
             print(f"Wrote file: {nc_path}")
 
-        self._output_netcdf = False
+        self._finalize_netcdf()
         return
 
     def _finalize_netcdf(self) -> None:
+        self._netcdf_initialized = False
         return
 
     def initialize_netcdf(
         self,
         output_dir: [str, pl.Path],
         separate_files: bool = True,
         output_vars: list = None,
         **kwargs,
     ):
-        self._output_netcdf = True
+        if self._netcdf_initialized:
+            msg = (
+                f"{self.name} class previously initialized netcdf output "
+                f"in {self._netcdf_output_dir}"
+            )
+            warnings.warn(msg)
+            return
+
+        self._netcdf_initialized = True
         self.netcdf_separate_files = separate_files
         self.netcdf_output_dir = output_dir
         if output_vars is None:
-            self.netcdf_output_vars = self.variables
+            self._netcdf_output_vars = self.variables
         else:
-            self.netcdf_output_vars = output_vars
+            self.netcdf__output_vars = list(
+                set(output_vars).intersection(set(self.variables))
+            )
+
+        if self._netcdf_output_vars is None:
+            self._netcdf_initialized = False
 
         return
 
     def output(self):
-        if self._output_netcdf:
-            if self.verbose:
+        if self._netcdf_initialized:
+            if self._verbose:
                 print(f"writing FULL timeseries output for: {self.name}")
             self._write_netcdf_timeseries()
         return
```

### Comparing `pywatershed-0.1.2/pywatershed/atmosphere/solar_constants.py` & `pywatershed-0.2.0/pywatershed/atmosphere/solar_constants.py`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/base/adapter.py` & `pywatershed-0.2.0/pywatershed/base/adapter.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,60 +6,88 @@
 from ..base.control import Control
 from ..base.timeseries import TimeseriesArray
 from ..constants import fileish
 from ..utils.netcdf_utils import NetCdfRead
 
 
 class Adapter:
-    """Adapter base class for getting data from a variety of sources."""
+    """Adapter base class for getting data from a variety of sources.
+
+    Args:
+        variable: string name ov variable
+    """
 
     def __init__(
         self,
         variable: str,
     ) -> None:
         self.name = "Adapter"
         self._variable = variable
         return None
 
     def advance(self):
+        "Advance the adapter in time"
         raise NotImplementedError("Must be overridden")
 
     @property
     def current(self):
         return self._current_value
 
 
 class AdapterNetcdf(Adapter):
+    """Adapter class for a netcdf file
+
+    Args:
+        fname: filename of netcdf as string or Path
+        variable: variable name string
+        dim_sizes: a tuple of dimension sizes
+        type: a variable dtype
+        control: a Control object
+        load_n_time_batches: number of times to read from file.
+
+    """
+
     def __init__(
         self,
         fname: fileish,
         variable: str,
+        dim_sizes: tuple,
+        type: str,
         control: Control,
         load_n_time_batches: int = 1,
     ) -> None:
         super().__init__(variable)
         self.name = "AdapterNetcdf"
 
+        self._dim_sizes = dim_sizes
+        self._type = type
         self._fname = fname
         self.control = control
         self._start_time = self.control.start_time
         self._end_time = self.control.end_time
 
         self._nc_read = NetCdfRead(
             fname,
             start_time=self._start_time,
             end_time=self._end_time,
             load_n_time_batches=load_n_time_batches,
         )
 
+        # would like to make this a check if dim_sizes and type are available
+        nc_type = self._nc_read.dataset[variable].dtype
+        nc_shape = list(self._nc_read.dataset[variable].shape)
+        nc_dims = list(self._nc_read.dataset[variable].dimensions)
+        for time_dim in ["time", "doy"]:
+            if time_dim in nc_dims:
+                _ = nc_shape.pop(nc_dims.index(time_dim))
+
         self.time = self._nc_read.times
+        # self._current_value = np.full(self._dim_sizes, np.nan, self._type)
+        self._current_value = np.full(nc_shape, np.nan, nc_type)
 
-        self._current_value = control.get_var_nans(
-            self._variable, drop_time_dim=True
-        )
         return
 
     def advance(self):
         if self._nc_read._itime_step[self._variable] > self.control.itime_step:
             return
         self._current_value[:] = self._nc_read.advance(
             self._variable, self.control.current_time
@@ -83,34 +111,38 @@
         self._current_value = data
         return
 
     def advance(self, *args):
         return None
 
 
-adaptable = Union[str, np.ndarray, Adapter]
+adaptable = Union[str, pl.Path, np.ndarray, Adapter]
 
 
 def adapter_factory(
     var: adaptable,
     variable_name: str = None,
     control: Control = None,
+    variable_dim_sizes: tuple = None,
+    variable_type: str = None,
     load_n_time_batches: int = 1,
 ):
     if isinstance(var, Adapter):
         """Adapt an adapter"""
         return var
 
     elif isinstance(var, (str, pl.Path)):
         """Paths and strings are considered paths to netcdf files"""
         if pl.Path(var).suffix == ".nc":
             return AdapterNetcdf(
                 var,
                 variable=variable_name,
                 control=control,
+                dim_sizes=variable_dim_sizes,
+                type=variable_type,
                 load_n_time_batches=load_n_time_batches,
             )
 
     elif isinstance(var, np.ndarray) and len(var.shape) == 1:
         """Adapt 1-D np.ndarrays"""
         return AdapterOnedarray(var, variable=variable_name)
```

### Comparing `pywatershed-0.1.2/pywatershed/base/budget.py` & `pywatershed-0.2.0/pywatershed/base/budget.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from pywatershed.base.control import Control
 
 from ..constants import zero
 from ..utils.formatting import pretty_print
 from ..utils.netcdf_utils import NetCdfWrite
 from .accessor import Accessor
+from .parameters import Parameters
 
 # Todo
 # * documentation
 # * get time_units / time_step from control
 # * decide on the fate of "from storage unit"
 # * terminology: "balance" just means "storage change"
 # * terminology: what is the term for the budget dosent close/zero?
@@ -484,26 +485,33 @@
                 self._storage_changes_sum,
                 stor_col_width,
                 stor_col_key_width,
             ),
         )
 
         def balance_line_col_wise():
+            # TODO(JLM): This is a hack until i have some time to sort this out
             bal_line = "Balance: "
             for oper, vals_sum, col_width, col_key_width in term_data:
+                if vals_sum.sum() > 0:
+                    sign_extra = 0
+                else:
+                    sign_extra = 1
+
                 bal_line += (
                     oper
                     + (" " * (col_key_width + col_extra_colon - len(oper)))
                     + pretty_print(
                         np.format_float_scientific(
                             vals_sum.sum(),
                             precision=col_width
                             - col_key_width
                             - col_extra_colon
-                            - 6,
+                            - 6
+                            - sign_extra,
                         ),
                         col_width - col_key_width - col_extra_colon,
                     )
                     + col_sep
                 )
             return bal_line
 
@@ -570,14 +578,15 @@
         """
         if self._output_netcdf:
             self.__output_netcdf()
         return
 
     def initialize_netcdf(
         self,
+        params: Parameters,
         output_dir: str,
         write_sum_vars: Union[list, bool] = True,
         write_individual_vars: bool = False,
     ) -> None:
         """Initialize NetCDF output
 
         Args:
@@ -632,26 +641,24 @@
                 f"pywatershed ({self.basis}) budget for {self.description}"
             ),
             "Budget basis": f"{self.basis} (unit or global)",
         }
         for key in self.terms.keys():
             global_attrs[key] = "[" + ", ".join(self.terms[key]) + "]"
 
-        coordinates = {"one": 0, **self.control.params.nhm_coordinates}
+        coordinates = {"one": 0, **params.coords}
 
         self._netcdf = NetCdfWrite(
             nc_path,
             coordinates,
             self._netcdf_output_var_dict,
             self.meta,
             global_attrs=global_attrs,
         )
-
         # todo jlm: put terms in to metadata
-
         return
 
     def __output_netcdf(self) -> None:
         """Output variable data for a time step
 
         Returns:
             None
```

### Comparing `pywatershed-0.1.2/pywatershed/base/data_model.py` & `pywatershed-0.2.0/pywatershed/base/data_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Iterable, Literal
 
 import cftime
 import netCDF4 as nc4
 import numpy as np
 import xarray as xr
 
-from ..constants import fill_values_dict, listish, np_type_to_netcdf_type_dict
+from ..constants import fileish, fill_values_dict, np_type_to_netcdf_type_dict
 from .accessor import Accessor
 
 # This file defines the data model for pywatershed. It is called a
 # "dataset_dict" and has a invertible mapping with non-hierarchical netcdf
 # or xarray datasets.
 
 # Show a basic example of how an xr_dd is changed to a dd.
@@ -38,30 +38,157 @@
     "dims": {},
     "coords": {},
     "data_vars": {},
     "encoding": {},
 }
 
 
+# Note: Methods do not deep copy by default, but not all references may be
+# preserved. use with caution and test.
+
+
 class DatasetDict(Accessor):
+    """DatasetDict class maps between netcdf conventions
+
+    This is the core class in the data model adopted by pywatershed.
+
+    Where typically metadata is stored on a variable, we maintain metadata
+    on a collocated dictionary. The data model is a DatasetDict with dims,
+    coords, data_vars, and metadata keys. The dims track the length of each
+    dimension. The coordinates are the discrete locations along dimensions or
+    sets of dimensions. The data_vars contain the data located on dims and
+    coordinates. The metadata describes the relationship between both coords
+    and data_vars and their dims. Together the coords and data_vars are the
+    variables of the DatasetDict. All keys in the variables must be present
+    in the metadata dictionary and each ke contains two more keys: dims and
+    attrs. The dims is a tuple of the variable's dimensions and attrs are
+    more general attributes.
+
+    When a netcdf file is read from disk, it has encoding properties that may
+    come along. Alternatively, encodings may be specified before writing to
+    file.
+
+    Args:
+        dims: A dictionary of pairs of `dim_names: dim_len` where `dim_len` is
+            an integer value.
+        coords: A dictionary of pairs of `coord_names: coord_data` where
+            `coord_data` is an np.ndarray.
+        data_vars: A dictionary of pairs of `var_names: var_data` where
+            `coord_data` is an np.ndarray.
+        metadata: For all names in `coords` and `data_vars`, metadata entries
+            with the required fields:
+
+            - dims: tuple of names in dim,
+            - attrs: dictionary whose values may be strings, ints, floats
+
+            The metadata argument may also contain a special `global` key
+            paired with a dictionary of global metadata of arbitrary name and
+            values of string, integer, or float types.
+        encoding: (to document)
+        validate: A bool that defaults to True, enforcing the consistency
+            of the supplied dictionaries
+
+
+    Examples:
+
+    ..
+        # This code is commented, copy and paste in to python, then paste the
+        # output below to keep it clean
+        from pprint import pprint
+        import pywatershed as pws
+        import numpy as np
+        coords = {
+            'time': np.arange('2005-02-01', '2005-02-03', dtype='datetime64[D]'),
+            'space': np.arange(3)
+        }
+        dims = {'ntime': len(coords['time']), 'nspace': len(coords['space'])}
+        data = {'precip': 10 * np.random.rand(dims['ntime'], dims['nspace'])}
+        metadata = {
+            "time": {"dims": ("ntime",), "attrs": {"description": "days"}},
+            "space": {
+                "dims": ("nspace",),
+                "attrs": {"description": "points of interest"},
+            },
+            "precip": {
+                "dims": (
+                    "ntime",
+                    "nspace",
+                ),
+                "attrs": {
+                    "description": "precipitation rate of all phases",
+                    "units": "mm/day",
+                },
+            },
+        }
+        dd = pws.base.DatasetDict(
+            dims=dims, coords=coords, data_vars=data, metadata=metadata
+        )
+        dd.dims.keys()
+        dd.variables.keys()
+        ds = dd.to_xr_ds()
+        print(ds)
+
+
+    >>> from pprint import pprint
+    >>> import pywatershed as pws
+    >>> import numpy as np
+    >>> coords = {
+    ...     "time": np.arange(
+    ...         "2005-02-01", "2005-02-03", dtype="datetime64[D]"
+    ...     ),
+    ...     "space": np.arange(3),
+    ... }
+    >>> dims = {"ntime": len(coords["time"]), "nspace": len(coords["space"])}
+    >>> data = {"precip": 10 * np.random.rand(dims["ntime"], dims["nspace"])}
+    >>> metadata = {
+    ...     "time": {"dims": ("ntime",), "attrs": {"description": "days"}},
+    ...     "space": {
+    ...         "dims": ("nspace",),
+    ...         "attrs": {"description": "points of interest"},
+    ...     },
+    ...     "precip": {
+    ...         "dims": (
+    ...             "ntime",
+    ...             "nspace",
+    ...         ),
+    ...         "attrs": {
+    ...             "description": "precipitation rate of all phases",
+    ...             "units": "mm/day",
+    ...         },
+    ...     },
+    ... }
+    >>> dd = pws.base.DatasetDict(
+    ...     dims=dims, coords=coords, data_vars=data, metadata=metadata
+    ... )
+    >>> dd.dims.keys()
+    dict_keys(['ntime', 'nspace'])
+    >>> dd.variables.keys()
+    dict_keys(['time', 'space', 'precip'])
+    >>> ds = dd.to_xr_ds()
+    >>> print(ds)
+    <xarray.Dataset>
+    Dimensions:  (ntime: 2, nspace: 3)
+    Coordinates:
+        time     (ntime) datetime64[ns] 2005-02-01 2005-02-02
+        space    (nspace) int64 0 1 2
+    Dimensions without coordinates: ntime, nspace
+    Data variables:
+        precip   (ntime, nspace) float64 8.835 5.667 9.593 7.239 3.92 0.4195
+
+    """
+
     def __init__(
         self,
-        dims: dict = None,
+        dims: dict[int] = None,
         coords: dict = None,
         data_vars: dict = None,
         metadata: dict = None,
         encoding: dict = None,
         validate: bool = True,
-    ) -> "DatasetDict":
-        """DatasetDict class which maps between netcdf conventions
-
-        Note: Methods do not deep copy by default, but not all
-              references may be preserved. use with caution
-        """
-
+    ) -> None:
         if dims is None:
             dims = {}
         if coords is None:
             coords = {}
         if data_vars is None:
             data_vars = {}
         if metadata is None:
@@ -124,14 +251,22 @@
         """Return the encoding"""
         if copy:
             return deepcopy(self._encoding)
         return self._encoding
 
     @property
     def data(self, copy=False) -> dict:
+        """Return a dict of dicts: dims, coords, data_vars, metadata, encoding
+
+        Args:
+            copy: boolean if a deepcopy is desired
+
+        Returns:
+            A dict of dicts containing all the data
+        """
         data = {
             "dims": self._dims,
             "coords": self._coords,
             "data_vars": self._data_vars,
             "metadata": self._metadata,
             "encoding": self._encoding,
         }
@@ -155,89 +290,110 @@
     #     )
 
     # def __str__(self):
     #     return
 
     @classmethod
     def from_dict(cls, dict_in, copy=False):
+        """Return this class from a passed dictionary.
+        Args:
+            dict_in: a dictionary from which to create an instance of this
+                class
+            copy: boolean if the passed dictionary should be deep copied
+        Returns:
+            A object of this class.
+        """
         if copy:
             return cls(**deepcopy(dict_in))
         return cls(**dict_in)
 
     @property
     def spatial_coord_names(self) -> dict:
-        """Return the spatial coordinate names."""
+        """Return the spatial coordinate names.
+        Args:
+           None
+        Returns:
+           Dictionary of spatial coordinates with names.
+        """
         attrs = self._metadata["global"]
         return {kk: vv for kk, vv in attrs.items() if "spatial" in kk}
 
     @classmethod
     def from_ds(cls, ds):
+        """Get this class from a dataset (nc4 or xarray)."""
         # detect typ as xr or nc4
         if isinstance(ds, xr.Dataset):
             return cls(**xr_ds_to_dd(ds))
         elif isinstance(ds, nc4.Dataset):
             return cls(**nc4_ds_to_dd(ds))
         else:
             raise ValueError("Passed dataset neither from xarray nor netCDF4")
 
     @classmethod
-    def from_netcdf(cls, nc_file, use_xr=False) -> "DatasetDict":
-        """Load from a netcdf file"""
+    def from_netcdf(
+        cls, nc_file: fileish, use_xr: bool = False, encoding=False
+    ) -> "DatasetDict":
+        """Load this class from a netcdf file."""
         # handle more than one file?
         if use_xr:
-            return cls(**xr_ds_to_dd(nc_file))
+            return cls(**xr_ds_to_dd(nc_file, encoding=encoding))
         else:
-            return cls(**nc4_ds_to_dd(nc_file))
+            return cls(**nc4_ds_to_dd(nc_file, use_xr_enc=encoding))
 
     def to_xr_ds(self) -> xr.Dataset:
+        """Export to an xarray Dataset"""
         return dd_to_xr_ds(self.data)
 
     def to_xr_dd(self) -> dict:
+        """Export to an xarray DatasetDict (xr.Dataset.to_dict())."""
         return dd_to_xr_dd(self.data)
 
     def to_nc4_ds(self, filename) -> None:
+        """Export to a netcdf file via netcdf4"""
         return dd_to_nc4_ds(self.data, filename)
 
     def to_netcdf(self, filename, use_xr=False) -> None:
         """Write parameters to a netcdf file"""
         if use_xr:
             self.to_xr_ds().to_netcdf(filename)
         else:
             self.to_nc4_ds(filename)
         return
 
     def rename_dim(self, name_maps: dict, in_place: bool = True):
+        """Rename dimensions."""
         if not in_place:
             raise NotImplementedError
         for old_name, new_name in name_maps.items():
             self.dims[new_name] = self.dims.pop(old_name)
             for mk, mv in self.metadata.items():
                 if "dims" in mv.keys() and old_name in mv["dims"]:
                     dim_list = list(mv["dims"])
                     dim_list[dim_list.index(old_name)] = new_name
                     mv["dims"] = tuple(dim_list)
 
         self.validate()
         return
 
     def rename_var(self, name_maps: dict, in_place=True):
+        """Rename variables."""
         if not in_place:
             raise NotImplementedError
         for old_name, new_name in name_maps.items():
             for cv in ["coords", "data_vars"]:
                 if old_name in self[cv].keys():
                     self[cv][new_name] = self[cv].pop(old_name)
                     for aa in ["metadata", "encoding"]:
                         self[aa][new_name] = self[aa].pop(old_name)
 
         self.validate()
         return
 
     def drop_var(self, var_names):
-        """Drop variables from the dd"""
+        """Drop variables"""
         if not isinstance(var_names, list):
             var_names = [var_names]
         for vv in var_names:
             for cv in ["coords", "data_vars"]:
                 if vv in self[cv].keys():
                     del self[cv][vv]
                     del self.metadata[vv]
@@ -291,29 +447,45 @@
 
         if copy:
             coord_data = deepcopy(coord_data)
         return coord_data
 
     def subset(
         self,
-        keys: listish = None,
-        copy=False,
+        keys: Iterable,
+        copy: bool = False,
         keep_global: bool = False,
         keep_global_metadata: bool = None,
         keep_global_encoding: bool = None,
+        strict: bool = False,
     ) -> "DatasetDict":
-        """Subset a DatasetDict to keys in data_vars or coordinates."""
+        """Subset a DatasetDict to keys in data_vars or coordinates
+
+        Args:
+            keys: Iterable to subset on
+            copy: bool to copy the input or edit it
+            keep_global: bool that sets both keep_global_metadata and
+                keep_global_encoding
+            keep_global_metadata: bool retain the global metadata in the subset
+            keep_global_encoding: bool retain the global encoding in the subset
+
+        Returns:
+          A subset Parameter object on the passed keys.
+
+        """
         # Instantiate the DatasetDict at end as deepcopy will be used
         # on the constructed subset dict (if requested)
 
         if not isinstance(keys, Iterable) or isinstance(keys, str):
             keys = [keys]
 
         for kk in keys:
             if kk not in self.variables.keys():
+                if not strict:
+                    continue
                 msg = f"key '{kk}' not in this {type(self).__name__} object"
                 raise KeyError(msg)
 
         if keep_global_metadata is None:
             keep_global_metadata = keep_global
         if keep_global_encoding is None:
             keep_global_encoding = keep_global
@@ -371,16 +543,25 @@
         result = type(self).from_dict(subset, copy=copy)
         return result
 
     def subset_on_coord(
         self,
         coord_name: str,
         where: np.ndarray,
-        in_place=True,
-    ):
+    ) -> None:
+        """Subset DatasetDict to a np.where along a named coordinate in-place
+
+        Args:
+            coord_name: string name of a coordinate
+            where: the result of an np.where along that coordinate (or likewise
+                constructed)
+
+        Returns:
+            None
+        """
         # only doing it in place for now
 
         # TODO: should almost work for 2+D? just linearizes np.where
         if len(where) > 1:
             raise NotImplementedError("at least not tested")
 
         # add the where to the data_vars
@@ -424,15 +605,21 @@
             else:
                 self["data_vars"][vk] = self.variables[vk][var_wh]
             self.metadata[vk]["attrs"]["subset_on_coord"] = coord_name
             self.metadata[vk]["attrs"]["subset_inds_on_orig"] = wh_data_name
 
         return
 
-    def validate(self):
+    def validate(self) -> None:
+        """Check that a DatasetDict is internally consistent.
+
+        Returns:
+            None
+        """
+
         # required keys
         assert sorted(self.data.keys()) == sorted(
             ["dims", "coords", "data_vars", "metadata", "encoding"]
         )
 
         # can not have same names in coords and data_vars
         common_keys = set(self.coords.keys()).intersection(
@@ -458,14 +645,25 @@
 
         # TODO: check dims lens equal data in the coordinates with those dims
 
         return
 
     @classmethod
     def merge(cls, *dd_list, copy=True, del_global_src=True):
+        """Merge a list of this class in to a single instance
+
+        Args:
+            dd_list: a list of object of this class
+            copy: boolean if a deep copy of inputs is desired
+            del_global_src: boolean to delete encodings' global source
+                attribute prior to merging (as these often conflict)
+
+        Returns:
+            An object of this class.
+        """
         if del_global_src or copy:
             dd_list = [deepcopy(dd.data) for dd in dd_list]
             if del_global_src:
                 for dd in dd_list:
                     if "source" in dd["encoding"]["global"]:
                         del dd["encoding"]["global"]["source"]
             merged_dict = _merge_dicts(dd_list)
@@ -479,15 +677,15 @@
 
 # DatasetDict
 # ---------------------------
 # module scope functions
 
 
 def _is_equal(aa, bb):
-    """How sketchy is this?"""
+    # How sketchy is this? (honest question)
     try:
         np.testing.assert_equal(aa, bb)
         return True
     except:  # noqa
         return False
 
 
@@ -524,15 +722,15 @@
                     raise ValueError(
                         f"Argument 'conflicts' can not be '{conflicts}'"
                     )
 
     return merged
 
 
-def xr_ds_to_dd(file_or_ds, schema_only=False) -> dict:
+def xr_ds_to_dd(file_or_ds, schema_only=False, encoding=True) -> dict:
     """Xarray dataset to a pywatershed dataset dict
 
     The pyws data model moves metadata off the variables to a separate
     var_metadata dictionary with the same keys found in the union of
     the keys of coords and data_vars.
     """
     if not isinstance(file_or_ds, xr.Dataset):
@@ -540,15 +738,16 @@
     else:
         xr_ds = file_or_ds
 
     if schema_only:
         data_arg = False
     else:
         data_arg = "array"
-    dd = xr_ds.to_dict(data=data_arg, encoding=True)
+
+    dd = xr_ds.to_dict(data=data_arg, encoding=encoding)
 
     dd = xr_dd_to_dd(dd)
 
     return dd
 
 
 def xr_dd_to_dd(xr_dd: dict) -> dict:
@@ -562,20 +761,26 @@
     coord_metadata = dd.pop("coords")
 
     # create empty data dicts and move the data out of the metadata
     # and move the encoding to encoding[var]
     dd["data_vars"] = {}
     for key, val in var_metadata.items():
         dd["data_vars"][key] = val.pop("data")
-        dd["encoding"][key] = val.pop("encoding")
+        if "encoding" in val.keys():
+            dd["encoding"][key] = val.pop("encoding")
+        else:
+            dd["encoding"][key] = {}
 
     dd["coords"] = {}
     for key, val in coord_metadata.items():
         dd["coords"][key] = val.pop("data")
-        dd["encoding"][key] = val.pop("encoding")
+        if "encoding" in val.keys():
+            dd["encoding"][key] = val.pop("encoding")
+        else:
+            dd["encoding"][key] = {}
 
     dd["metadata"] = {**coord_metadata, **var_metadata}
     dd["metadata"]["global"] = dd.pop("attrs")
 
     return dd
 
 
@@ -594,18 +799,21 @@
     for key, val in meta.items():
         cv = None
         if key in dd["data_vars"].keys():
             cv = "data_vars"
         elif key in dd["coords"].keys():
             cv = "coords"
 
+        key_enc = {}
+        if key in encoding.keys():
+            key_enc = encoding[key]
         dd[cv][key] = {
             **val,
             "data": dd[cv][key],
-            "encoding": encoding[key],
+            "encoding": key_enc,
         }
 
     return dd
 
 
 def dd_to_xr_ds(dd: dict) -> xr.Dataset:
     """pywatershed dataset dict to xarray dataset
@@ -769,15 +977,15 @@
     if not isinstance(nc4_file_ds, nc4.Dataset):
         if use_xr_enc:
             xr_enc = _get_xr_encoding(nc4_file_ds)
         nc4_file_ds = nc4.Dataset(nc4_file_ds)
     else:
         if use_xr_enc:
             raise ValueError(
-                "Must pass a file and not an nc4.Dataset to use_xr_enc argument"
+                "Pass a file and not an nc4.Dataset to use_xr_enc argument"
             )
 
     xr_dd = nc4_ds_to_xr_dd(nc4_file_ds, xr_enc=xr_enc)
     dd = xr_dd_to_dd(xr_dd)
     return dd
 
 
@@ -886,7 +1094,11 @@
                     coords += [c_name]
             if len(coords):
                 var.coordinates = " ".join(sorted(coords))
             if is_bool:
                 var.setncattr("dtype", "bool")
 
     return
+
+
+def open_datasetdict(nc_file: fileish, use_xr=True):
+    return DatasetDict.from_netcdf(nc_file, use_xr=use_xr)
```

### Comparing `pywatershed-0.1.2/pywatershed/base/meta.py` & `pywatershed-0.2.0/pywatershed/base/meta.py`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/base/storageUnit.py` & `pywatershed-0.2.0/pywatershed/base/process.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,40 @@
+import inspect
 import os
 import pathlib as pl
 from typing import Literal
 from warnings import warn
 
 import numpy as np
 
 from ..base import meta
 from ..base.adapter import Adapter, adapter_factory
-from ..base.budget import Budget
 from ..base.data_model import _merge_dicts
 from ..base.timeseries import TimeseriesArray
+from ..parameters import Parameters
 from ..utils.netcdf_utils import NetCdfWrite
 from .accessor import Accessor
 from .control import Control
 
 
-class StorageUnit(Accessor):
-    """StorageUnit base class
+class Process(Accessor):
+    """Process base class
 
-    The StorageUnit is a base class for conserving mass and energy.
+    Process is a base class for physical processes.
 
-    It has budgets that can optionally be established for mass an energy and
-    these can be enforced or simply diagnosed with the model run.
-
-    The  class aims to describe itself through it sstaticmethods and
+    The  class aims to describe itself through it staticmethods and
     properties.
 
     Conventions are adopted through the use of the following
     properties/methods:
 
         inputs/get_inputs():
             List the names of variables required from external sources.
-            Still working on conventions if these are to be modified but
-            the storageUnit. For an input to be successfully inicluded,
+            Still working on conventions if these are to be modified.
+            For an input to be successfully inicluded,
             that variable must be defined in the metadata
             (pywatershed/static/metadata/variables.yaml).
             Efforts should be made to not use diagnostic variables as input
             as much as possible.
         variables/get_variables():
             List the names of internal public variables. If not necessary,
             to be public, variables should be made private with a single,
@@ -44,30 +42,25 @@
             to be successfully inicluded, that variable must be defined in the
             metadata (pywatershed/static/metadata/variables.yaml).
             Efforts should be made not to track diagnostic variables in this
             public variable set, as much as possible.
         parameters/get_parameters():
             List the names of parameters used by the subclass.
         description:
-            Return a dictionary of with the storage unit cubclass name and its
+            Return a dictionary of with the process subclass name and its
             metadata for all variables for each of inputs, variables, and
             parameters.
         get_init_values:
             Return a dictionary of initialization values for variables.
             Note that these may be overridden by subclass initialization
             routines (e.g. using parameters) or by restart values. So these
             are not "initial values", they are initialization values that
             are set when the variable is declared from metadata in
             _initialize_var(). Initization values should be nan as much as
             possible.
-        mass_budget_terms/get_mass_budget_terms():
-            These terms must all in in the same units across all components of
-            the budget (inputs, outputs, storage_changes). Diagnostic variables
-            should not appear in the budget terms, only prognostic variables
-            should.
         _advance_variables():
             This advance should exactly specify the prognostic variables in
             setting previous values to current values. When/if necessary to
             keep previous diagnostic variables, those must not appear here but
             in _calculate().
         _calculate():
             This method is to be overridden by the subclass. Near the end of
@@ -76,41 +69,43 @@
             mass_budget_terms, storage changes should only be tracked for
             prognostic variables. (For example is snow_water_equiv = snow_ice +
             snow_liquid, then storage changes for snow_ice and snow_liquid
             should be tracked and not for snow_water_equiv).
 
         Args:
           control: a Control object
-          verbose: boolean controling the amount of information printed
-          load_n_time_batches: integer number of times the input data should
-            be loaded from file. Deafult is 1 or just once. If input data are
-            large in space, time, or total number of variables then increasing
-            this number can help reduce memory usage at the expense of reduced
-            performance due to more frequent IO.
 
     """
 
     def __init__(
         self,
         control: Control,
-        verbose: bool,
-        load_n_time_batches: int = 1,
+        discretization: Parameters,
+        parameters: Parameters,
         metadata_patches: dict[dict] = None,
         metadata_patch_conflicts: Literal["ignore", "warn", "error"] = "error",
     ):
-        self.name = "StorageUnit"
+        self.name = "Process"
         self.control = control
-        self.params = self.control.params.subset(self.get_parameters())
-        self.verbose = verbose
-        self._load_n_time_batches = load_n_time_batches
+
+        # params from dis and params: methodize this
+        missing_params = set(self.parameters).difference(
+            set(parameters.variables.keys())
+        )
+        if missing_params:
+            self.params = type(parameters).merge(parameters, discretization)
+        else:
+            self.params = parameters.subset(self.get_parameters())
 
         # netcdf output variables
-        self._output_netcdf = False
+        self._netcdf_initialized = False
+        self._netcdf_output_dir = None
         self._netcdf = None
         self._separate_netcdf = True
+
         self._itime_step = -1
 
         # TODO metadata patching.
         self._set_metadata()
         if metadata_patches is not None:
             self._patch_metadata(
                 metadata_patches,
@@ -120,96 +115,63 @@
         self._initialize_self_variables()
         self._set_initial_conditions()
 
         return None
 
     def output(self) -> None:
         """Output data to previously initialized output types.
-
-        Writes output for initalized output types.
-
         Returns:
             None
-
         """
-        if self._output_netcdf:
-            if self.verbose:
+        if self._netcdf_initialized:
+            if self._verbose:
                 print(f"writing output for: {self.name}")
-            self.__output_netcdf()
-
-        if self.budget is not None:
-            self.budget.output()
+            self._output_netcdf()
         return
 
     def finalize(self) -> None:
-        """Finalize storageUnit
-
-        Finalizes the object, including output methods.
-
+        """Finalizes the Process, including output methods.
         Returns:
             None
-
         """
-        if self.verbose:
+        if self._verbose:
             print(f"finalizing: {self.name}")
 
         self._finalize_netcdf()
-        if self.budget is not None:
-            self.budget._finalize_netcdf()
         return
 
     @staticmethod
     def get_dimensions() -> tuple:
-        """Get a tuple of parameter names."""
+        """Get a tuple of dimension names for this Process."""
         raise Exception("This must be overridden")
 
     @staticmethod
     def get_parameters() -> tuple:
-        """Get a tuple of parameter names."""
+        """Get a tuple of parameter names for this Process."""
         raise Exception("This must be overridden")
 
     @staticmethod
     def get_inputs() -> tuple:
-        """Get a tuple of input variable names."""
+        """Get a tuple of input variable names for this Process."""
         raise Exception("This must be overridden")
 
     @classmethod
     def get_variables(cls) -> tuple:
-        """Get a tuple of internal public variable names."""
+        """Get a tuple of (public) variable names for this Process."""
         return list(cls.get_init_values().keys())
 
     @classmethod
-    def get_mass_budget_terms(cls) -> dict:
-        """Get a dictionary of variable names for mass budget terms."""
-        mass_budget_terms = {
-            "inputs": list(
-                meta.filter_vars(
-                    cls.get_inputs(), "var_category", "mass flux"
-                ).keys()
-            ),
-            "outputs": list(
-                meta.filter_vars(
-                    cls.get_variables(), "var_category", "mass flux"
-                ).keys()
-            ),
-            "storage_changes": list(
-                meta.filter_vars(
-                    cls.get_variables(), "var_category", "mass storage change"
-                ).keys()
-            ),
-        }
-        return mass_budget_terms
-
-    @classmethod
     def description(cls) -> dict:
-        """A description (all metadata) for all variables in inputs, variables,
-        and parameters."""
+        """A dictionary description of this Process.
+
+        Returns:
+            All metadata for all variables in inputs, variables,
+            and parameters."""
         return {
             "class_name": cls.__name__,
-            "mass_budget_terms": cls.get_mass_budget_terms(),
             "inputs": meta.get_vars(cls.get_inputs()),
             "variables": meta.get_vars(cls.get_variables()),
             "parameters": meta.get_params(cls.get_parameters()),
         }
 
     @staticmethod
     def get_restart_variables() -> list:
@@ -248,32 +210,30 @@
         return self.get_restart_variables()
 
     @property
     def init_values(self) -> dict:
         """A dictionary of initial values for each public variable."""
         return self.get_init_values()
 
-    @property
-    def mass_budget_terms(self) -> dict:
-        """A dictionary of variable names for the mass budget terms."""
-        return self.get_mass_budget_terms()
-
     def _initialize_self_variables(self, restart: bool = False):
         # dims
         for name in self.dimensions:
-            setattr(self, name, self.control.params.dims[name])
+            if name == "ntime":
+                setattr(self, name, self.control.n_times)
+            else:
+                setattr(self, name, self.params.dims[name])
 
         # parameters
         for name in self.parameters:
             setattr(self, name, self.params.get_param_values(name))
 
         # inputs
         for name in self.inputs:
             # dims of internal variables never have time, so they are spatial
-            spatial_dims = self.control.params.get_dim_values(
+            spatial_dims = self.params.get_dim_values(
                 list(meta.find_variables(name)[name]["dims"])
             )
             spatial_dims = tuple(spatial_dims.values())
             setattr(self, name, np.zeros(spatial_dims, dtype=float) + np.nan)
 
         # variables
         # skip restart variables if restart (for speed) ?
@@ -290,15 +250,15 @@
         """Initialize a variable using get_init_values and metadata.
 
         Initialized variables can be for single time or they can be a timeries
         array object if they have a time dimension in metadata.
         """
         init_vals = self.get_init_values()
         if var_name not in init_vals.keys():
-            if self.verbose:
+            if self._verbose:
                 warn(
                     f"{var_name} not initialized (no initial value specified)"
                 )
             return
 
         dims = [self[vv] for vv in self.meta[var_name]["dims"]]
         init_type = self.meta[var_name]["type"]
@@ -328,113 +288,116 @@
             self[key][:] = value.current
 
         return
 
     def _set_inputs(self, args):
         self._input_variables_dict = {}
         for ii in self.inputs:
+            ii_dims = self.control.meta.get_dimensions(ii)[ii]
+            # This accomodates Timeseries like objects that need to init
+            # both full rank and reduced rank versions of their data
+            # this is pretty adhoc
+            check_list = ["time", "doy"]
+            if len([mm for mm in check_list if mm in ii_dims[0]]):
+                ii_dims = ii_dims[1:]
+
+            ii_dim_sizes = tuple(self.params.get_dim_values(ii_dims).values())
+            ii_type = self.control.meta.get_numpy_types(ii)[ii]
+
             self._input_variables_dict[ii] = adapter_factory(
                 args[ii],
-                ii,
-                args["control"],
-                load_n_time_batches=self._load_n_time_batches,
+                variable_name=ii,
+                control=args["control"],
+                variable_dim_sizes=ii_dim_sizes,
+                variable_type=ii_type,
             )
             if self._input_variables_dict[ii]:
                 self[ii] = self._input_variables_dict[ii].current
 
         return
 
+    def _set_options(self, init_locals):
+        """Set options options on self if supplied on init, else take
+        from control"""
+        # some self and Process introspection reveals the option names
+        init_arg_names = set(
+            inspect.signature(self.__init__).parameters.keys()
+        )
+        process_init_args = set(
+            inspect.signature(Process.__init__).parameters.keys()
+        )
+        inputs_args = self.inputs
+        non_option_args = process_init_args.union(inputs_args)
+        option_names = init_arg_names.difference(non_option_args)
+
+        for opt in option_names:
+            if opt in init_locals.keys() and init_locals[opt] is not None:
+                setattr(self, f"_{opt}", init_locals[opt])
+            elif opt in self.control.options.keys():
+                setattr(self, f"_{opt}", self.control.options[opt])
+            else:
+                setattr(self, f"_{opt}", None)
+
+        return
+
     def set_input_to_adapter(self, input_variable_name: str, adapter: Adapter):
+        # Todo: document
         self._input_variables_dict[input_variable_name] = adapter
         # can NOT use [:] on the LHS as we are relying on pointers between
         # boxes. [:] on the LHS here means it's not a pointer and then
         # requires that the calculation of the input happens before the
-        # advance of this storage unit. But that gives the incorrect budget
-        # for et.
+        # advance of this process.
         self[input_variable_name] = adapter.current
-
-        # Using a pointer between boxes means that the same pointer has to
-        # be used for the budget, so there's no way to have a preestablished
-        # pointer between storageUnit and its budget. So this stuff...
-        if self.budget is not None:
-            for comp in self.budget.components:
-                if input_variable_name in self.budget[comp].keys():
-                    # can not use [:] on the LHS?
-                    self.budget[comp][input_variable_name] = self[
-                        input_variable_name
-                    ]
-
-        return
-
-    def _set_budget(self, behavior, basis: str = "unit"):
-        if behavior is None:
-            self.budget = None
-        elif behavior in ["error", "warn"]:
-            self.budget = Budget.from_storage_unit(
-                self,
-                time_unit="D",
-                description=self.name,
-                imbalance_fatal=(behavior == "error"),
-                basis=basis,
-            )
-        else:
-            raise ValueError(f"Illegal behavior: {behavior}")
-
         return
 
     def advance(self):
         """
-        Advance the storage unit in time.
+        Advance the Process in time.
 
         Returns:
             None
         """
 
         if self._itime_step >= self.control.itime_step:
-            if self.verbose:
+            if self._verbose:
                 msg = (
                     f"{self.name} did not advance because "
                     f"it is not behind control time"
                 )
                 # warn(msg)
                 print(msg)  # can/howto make warn flush in real time?
                 # is a warning sufficient? an error
             return
 
-        if self.verbose:
+        if self._verbose:
             print(f"advancing: {self.name}")
 
         self._advance_variables()
         self._advance_inputs()
         self._itime_step += 1
         return
 
     def _calculate(self):
         raise Exception("This must be overridden")
 
     def calculate(self, time_length: float, **kwargs) -> None:
-        """Calculate storageUnit terms for a time step
+        """Calculate Process terms for a time step
 
         Args:
             simulation_time: current simulation time
 
         Returns:
             None
         """
-        if self.verbose:
+        if self._verbose:
             print(f"calculating: {self.name}")
 
         # self._calculate must be implemented by the subclass
         self._calculate(time_length, *kwargs)
 
-        # move to a timestep finalization method at some future date.
-        if self.budget is not None:
-            self.budget.advance()
-            self.budget.calculate()
-
         return
 
     def _set_metadata(self):
         """Set metadata on self for self's inputs, parameters, and variables"""
         meta_keys = (*self.variables, *self.inputs, *self.parameters)
         msg = (
             "Duplicate varible names amongst self's variables, "
@@ -472,85 +435,96 @@
             df.to_csv(fname)
         return
 
     def initialize_netcdf(
         self,
         output_dir: [str, pl.Path],
         separate_files: bool = True,
-        budget_args: dict = None,
         output_vars: list = None,
     ) -> None:
         """Initialize NetCDF output.
 
         Args:
-            output_dir: base directory path or NetCDF file path if separate_files
-                is True
+            output_dir: base directory path or NetCDF file path if
+                separate_files is True
             separate_files: boolean indicating if storage component output
                 variables should be written to a separate file for each
                 variable
-            budget_args: a dict of argument key: values to pass to
-                initialize_netcdf on this storage unit's budget. see budget
-                object for options.
+            output_vars: list of variable names to outuput.
 
         Returns:
             None
 
         """
-        if self.verbose:
+        if self._netcdf_initialized:
+            msg = (
+                f"{self.name} class previously initialized netcdf output "
+                f"in {self._netcdf_output_dir}"
+            )
+            warn(msg)
+            return
+
+        if self._verbose:
             print(f"initializing netcdf output for: {self.output_dir}")
 
-        self._output_netcdf = True
-        self._output_vars = output_vars
+        self._netcdf_initialized = True
+        self._netcdf_output_dir = pl.Path(output_dir)
+        if output_vars is None:
+            self._output_vars = self.variables
+        else:
+            self._output_vars = list(
+                set(output_vars).intersection(set(self.variables))
+            )
+
+        if self._output_vars is None:
+            self._netcdf_initialized = False
+            return
+
         self._netcdf = {}
+
         if separate_files:
             self._separate_netcdf = True
             # make working directory
-            output_dir = pl.Path(output_dir)
-            output_dir.mkdir(parents=True, exist_ok=True)
+            self._netcdf_output_dir.mkdir(parents=True, exist_ok=True)
             for variable_name in self.variables:
                 if (self._output_vars is not None) and (
                     variable_name not in self._output_vars
                 ):
                     continue
-                nc_path = pl.Path(output_dir) / f"{variable_name}.nc"
+                nc_path = self._netcdf_output_dir / f"{variable_name}.nc"
                 self._netcdf[variable_name] = NetCdfWrite(
                     nc_path,
                     self.params.coords,
                     [variable_name],
                     {variable_name: self.meta[variable_name]},
+                    {"process class": self.name},
                 )
         else:
             initial_variable = self.variables[0]
-            pl.Path(output_dir).mkdir(parents=True, exist_ok=True)
+            self._netcdf_output_dir.mkdir(parents=True, exist_ok=True)
             self._netcdf[initial_variable] = NetCdfWrite(
-                output_dir / f"{self.name}.nc",
-                self.params.nhm_coordinates,
+                self._netcdf_output_dir / f"{self.name}.nc",
+                self.params.coords,
                 self.variables,
                 self.meta,
+                {"process class": self.name},
             )
             for variable in self.variables[1:]:
                 self._netcdf[variable] = self._netcdf[initial_variable]
 
-        if self.budget is not None:
-            if budget_args is None:
-                budget_args = {}
-            budget_args["output_dir"] = output_dir
-
-            self.budget.initialize_netcdf(**budget_args)
-
         return
 
-    def __output_netcdf(self) -> None:
+    def _output_netcdf(self) -> None:
         """Output variable data to NetCDF for a time step.
 
         Returns:
             None
 
         """
-        if self._output_netcdf:
+        if self._netcdf_initialized:
             time_added = False
             for variable in self.variables:
                 if (self._output_vars is not None) and (
                     variable not in self._output_vars
                 ):
                     continue
                 if not time_added or self._separate_netcdf:
@@ -568,15 +542,15 @@
 
     def _finalize_netcdf(self) -> None:
         """Finalize NetCDF output to disk.
 
         Returns:
             None
         """
-        if self._output_netcdf:
+        if self._netcdf_initialized:
             for idx, variable in enumerate(self.variables):
                 if (self._output_vars is not None) and (
                     variable not in self._output_vars
                 ):
                     continue
 
                 self._netcdf[variable].close()
```

### Comparing `pywatershed-0.1.2/pywatershed/base/timeseries.py` & `pywatershed-0.2.0/pywatershed/base/timeseries.py`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/constants.py` & `pywatershed-0.2.0/pywatershed/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 if numba_num_threads is None:
     numba_num_threads = 0
 else:
     numba_num_threads = int(numba_num_threads)
 
 # Typing constants
 fileish = Union[str, pl.Path]
-listish = Union[str, list, tuple]
+listish = Union[str, list, tuple]  # Todo deprecate to Typing.Iterable
 
 # PRMS6 Constants module:
 # https://github.com/nhm-usgs/prms/blob/6.0.0_dev/src/prmslib/misc/m_constants.f90
 
 __pywatershed_root__ = pl.Path(__file__).parent
 
 zero = np.zeros([1])[0]
```

### Comparing `pywatershed-0.1.2/pywatershed/hydrology/PRMSCanopy.py` & `pywatershed-0.2.0/pywatershed/hydrology/prms_canopy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+from typing import Literal
+from warnings import warn
+
 import numpy as np
 from numba import prange
 
 from ..base.adapter import adaptable
+from ..base.conservative_process import ConservativeProcess
 from ..base.control import Control
-from ..base.storageUnit import StorageUnit
 from ..constants import CovType, HruType, numba_num_threads, zero
+from ..parameters import Parameters
 
 try:
-    from ..PRMSCanopy_f import canopy
+    from ..prms_canopy_f import canopy
 
     _calculate_fortran = canopy.calc_canopy
     has_prmscanopy_f = True
 except ImportError:
     has_prmscanopy_f = False
 
 # set constants (may need .value for enum to be used in > comparisons)
@@ -23,95 +27,96 @@
 LAKE = HruType.LAKE.value
 RAIN = 0
 SNOW = 1
 OFF = 0
 ACTIVE = 1
 
 
-class PRMSCanopy(StorageUnit):
-    """PRMS canopy."""
+class PRMSCanopy(ConservativeProcess):
+    """PRMS canopy class.
+
+    Args:
+        control: a Control object
+        discretization: a discretization of class Parameters
+        parameters: a parameter object of class Parameters
+        pkwater_ante: Previous snowpack water equivalent on each HRU
+        transp_on: Flag indicating whether transpiration is occurring
+            (0=no;1=yes)
+        hru_ppt: Precipitation on each HRU
+        hru_rain: Rain on each HRU
+        hru_snow: Snow on each HRU
+        budget_type: one of [None, "warn", "error"]
+        calc_method: one of ["fortran", "numba", "numpy"]. None defaults to
+            "numba".
+        verbose: Print extra information or not?
+        load_n_time_batches: not-implemented
+    """
 
     def __init__(
         self,
         control: Control,
+        discretization: Parameters,
+        parameters: Parameters,
         pkwater_ante: adaptable,
         transp_on: adaptable,
         hru_ppt: adaptable,
         hru_rain: adaptable,
         hru_snow: adaptable,
         potet: adaptable,
-        budget_type: str = None,
-        calc_method: str = None,
-        verbose: bool = False,
-        load_n_time_batches: int = 1,
-    ) -> "PRMSCanopy":
+        budget_type: Literal[None, "warn", "error"] = None,
+        calc_method: Literal["fortran", "numba", "numpy"] = None,
+        verbose: bool = None,
+    ):
         super().__init__(
             control=control,
-            verbose=verbose,
-            load_n_time_batches=load_n_time_batches,
+            discretization=discretization,
+            parameters=parameters,
         )
         self.name = "PRMSCanopy"
 
-        self._calc_method = str(calc_method)
+        # set hrutype to LAND as this is only type supported in NHM
+        self._hru_type = np.array(self.nhru * [LAND])
 
         self._set_inputs(locals())
-        self._set_budget(budget_type)
+        self._set_options(locals())
 
-        # set hrutype to LAND as this is only type supported in NHM
-        self._hru_type = np.array(self.nhru * [LAND])
+        self._set_budget()
+        self._init_calc_method()
 
         return
 
     @staticmethod
     def get_dimensions() -> tuple:
-        """
-        Return a tuple the dimension names
-        """
         return ("nhru",)
 
     @staticmethod
     def get_parameters() -> tuple:
-        """
-        Return a tuple of parameters names
-        """
         return (
             "cov_type",
             "covden_sum",
             "covden_win",
             "srain_intcp",
             "wrain_intcp",
             "snow_intcp",
             "potet_sublim",
         )
 
     @staticmethod
     def get_inputs() -> tuple:
-        """Get canopy reservoir input variables
-
-        Returns:
-            variables: input variables
-
-        """
         return (
             "pkwater_ante",
             "transp_on",
             "hru_ppt",
             "hru_rain",
             "hru_snow",
             "potet",
         )
 
     @staticmethod
     def get_init_values() -> dict:
-        """Get canopy initial values
-
-        Returns:
-            dict: initial values for named variables
-        """
-
         return {
             "net_ppt": zero,
             "net_rain": zero,
             "net_snow": zero,
             "intcp_changeover": zero,
             "intcp_evap": zero,
             "intcp_form": 0,  # could make boolean but would have to make the RAIN/SNOW match
@@ -135,14 +140,138 @@
             ],
             "storage_changes": ["hru_intcpstor_change"],
         }
 
     def _set_initial_conditions(self):
         return
 
+    def _init_calc_method(self):
+        if self._calc_method is None:
+            self._calc_method = "numba"
+
+        avail_methods = ["numpy", "numba", "fortran"]
+        fortran_msg = ""
+        if self._calc_method == "fortran" and not has_prmscanopy_f:
+            _ = avail_methods.remove("fortran")
+            fortran_msg = "\n(Fortran not available as installed)\n"
+
+        if self._calc_method.lower() not in avail_methods:
+            msg = (
+                f"Invalid calc_method={self._calc_method} for {self.name}. "
+                f"{fortran_msg}"
+                f"Setting calc_method to 'numba' for {self.name}"
+            )
+            warn(msg)
+            self._calc_method = "numba"
+
+        if self._calc_method.lower() in ["numba"]:
+            import numba as nb
+
+            numba_msg = f"{self.name} jit compiling with numba "
+            nb_parallel = (numba_num_threads is not None) and (
+                numba_num_threads > 1
+            )
+            if nb_parallel:
+                numba_msg += f"and using {numba_num_threads} threads"
+            print(numba_msg, flush=True)
+
+            # JLM: note. I gave up on specifying signatures because it
+            #      appears impossible/undocumented how to specify the type
+            #      of a passed function. The work is not in vain as then
+            #      types will be required for f90. The signatures remain
+            #      here commented for that reason and in case we can get it
+            #      to work in the future.
+
+            # self._intercept_numba = nb.njit(
+            #     nb.types.Tuple(
+            #         (
+            #             nb.float64[:],  # intcp_stor
+            #             nb.float64[:],  # net_precip
+            #         )
+            #     )(
+            #         nb.float64[:],  # precip
+            #         nb.float64[:],  # stor_max
+            #         nb.float64[:],  # cov
+            #         nb.float64[:],  # intcp_stor
+            #         nb.float64[:],  # net_precip
+            #     ),
+            #     fastmath=True,
+            # )(self._intercept)
+            self._intercept = nb.njit(fastmath=True)(self._intercept)
+
+            # self._calculate_numba = nb.njit(
+            #     nb.types.Tuple(
+            #         (
+            #             nb.float64[:],  # intcp_evap
+            #             nb.float64[:],  # intcp_stor
+            #             nb.float64[:],  # net_rain
+            #             nb.float64[:],  # net_snow
+            #             nb.float64[:],  # net_ppt
+            #             nb.float64[:],  # hru_intcpstor
+            #             nb.float64[:],  # hru_intcpevap
+            #             nb.float64[:],  # intcp_changeover
+            #             nb.int32[:],  # intcp_transp_on
+            #         )
+            #     )(
+            #         nb.int32,  # np.int32(self.nhru)
+            #         nb.int64[:],  # cov_type
+            #         nb.float64[:],  # covden_sum
+            #         nb.float64[:],  # covden_win
+            #         nb.float64[:],  # hru_intcpstor
+            #         nb.float64[:],  # hru_intcpevap
+            #         nb.float64[:],  # hru_ppt
+            #         nb.float64[:],  # hru_rain
+            #         nb.float64[:],  # hru_snow
+            #         nb.float64[:],  # intcp_changeover
+            #         nb.float64[:],  # intcp_evap
+            #         nb.int32[:],  # intcp_form
+            #         nb.float64[:],  # intcp_stor
+            #         nb.int32[:],  # intcp_transp_on
+            #         nb.float64[:],  # net_ppt
+            #         nb.float64[:],  # net_rain
+            #         nb.float64[:],  # net_snow
+            #         nb.float64[:],  # self.pkwater_ante
+            #         nb.float64[:],  # potet
+            #         nb.float64[:],  # potet_sublim
+            #         nb.float64[:],  # snow_intcp
+            #         nb.float64[:],  # srain_intcp
+            #         nb.float64[:],  # transp_on
+            #         nb.float64[:],  # wrain_intcp
+            #         nb.float64,  # np.float64(time_length),
+            #         nb.int64[:],  # self._hru_type
+            #         nb.float64,  # NEARZERO
+            #         nb.float64,  # DNEARZERO,
+            #         nb.int32,  # BARESOIL,
+            #         nb.int32,  # GRASSES,
+            #         nb.int32,  # LAND,
+            #         nb.int32,  # LAKE,
+            #         nb.int32,  # RAIN,
+            #         nb.int32,  # SNOW,
+            #         nb.int32,  # OFF,
+            #         nb.int32,  # ACTIVE,
+            #         nb.typeof(self._intercept_numba),  # function.
+            #     ),
+            #     fastmath=True,
+            # )(self._calculate_procedural)
+            self._calculate_canopy = nb.njit(
+                fastmath=True, parallel=nb_parallel
+            )(self._calculate_numpy)
+
+        elif self._calc_method.lower() == "fortran":
+            pass
+            # fortran has a different call signature in the last agument
+            # because the intercept function is not passed.
+            # so it is handled with an if statement at call time.
+            # self._calculate_gw = _calculate_fortran
+
+        else:
+            self._calculate_canopy = self._calculate_numpy
+
+        return
+
     def _advance_variables(self):
         """Advance canopy
         Returns:
             None
 
         """
         self.hru_intcpstor_old[:] = self.hru_intcpstor
@@ -154,171 +283,26 @@
         Args:
             simulation_time: current simulation time
 
         Returns:
             None
 
         """
-        if self._calc_method.lower() == "numba":
-            import numba as nb
-
-            if not hasattr(self, "_calculate_numba"):
-                numba_msg = f"{self.name} using numba "
-                nb_parallel = (numba_num_threads is not None) and (
-                    numba_num_threads > 1
-                )
-                if nb_parallel:
-                    numba_msg += f"with {numba_num_threads} threads"
-                print(numba_msg, flush=True)
-
-                # JLM: note. I gave up on specifying signatures because it
-                #      appears impossible/undocumented how to specify the type
-                #      of a passed function. The work is not in vain as then
-                #      types will be required for f90. The signatures remain
-                #      here commented for that reason and in case we can get it
-                #      to work in the future.
-
-                # self._intercept_numba = nb.njit(
-                #     nb.types.Tuple(
-                #         (
-                #             nb.float64[:],  # intcp_stor
-                #             nb.float64[:],  # net_precip
-                #         )
-                #     )(
-                #         nb.float64[:],  # precip
-                #         nb.float64[:],  # stor_max
-                #         nb.float64[:],  # cov
-                #         nb.float64[:],  # intcp_stor
-                #         nb.float64[:],  # net_precip
-                #     ),
-                #     fastmath=True,
-                # )(self._intercept)
-                self._intercept_numba = nb.njit(fastmath=True)(self._intercept)
-
-                # self._calculate_numba = nb.njit(
-                #     nb.types.Tuple(
-                #         (
-                #             nb.float64[:],  # intcp_evap
-                #             nb.float64[:],  # intcp_stor
-                #             nb.float64[:],  # net_rain
-                #             nb.float64[:],  # net_snow
-                #             nb.float64[:],  # net_ppt
-                #             nb.float64[:],  # hru_intcpstor
-                #             nb.float64[:],  # hru_intcpevap
-                #             nb.float64[:],  # intcp_changeover
-                #             nb.int32[:],  # intcp_transp_on
-                #         )
-                #     )(
-                #         nb.int32,  # np.int32(self.nhru)
-                #         nb.int64[:],  # cov_type
-                #         nb.float64[:],  # covden_sum
-                #         nb.float64[:],  # covden_win
-                #         nb.float64[:],  # hru_intcpstor
-                #         nb.float64[:],  # hru_intcpevap
-                #         nb.float64[:],  # hru_ppt
-                #         nb.float64[:],  # hru_rain
-                #         nb.float64[:],  # hru_snow
-                #         nb.float64[:],  # intcp_changeover
-                #         nb.float64[:],  # intcp_evap
-                #         nb.int32[:],  # intcp_form
-                #         nb.float64[:],  # intcp_stor
-                #         nb.int32[:],  # intcp_transp_on
-                #         nb.float64[:],  # net_ppt
-                #         nb.float64[:],  # net_rain
-                #         nb.float64[:],  # net_snow
-                #         nb.float64[:],  # self.pkwater_ante
-                #         nb.float64[:],  # potet
-                #         nb.float64[:],  # potet_sublim
-                #         nb.float64[:],  # snow_intcp
-                #         nb.float64[:],  # srain_intcp
-                #         nb.float64[:],  # transp_on
-                #         nb.float64[:],  # wrain_intcp
-                #         nb.float64,  # np.float64(time_length),
-                #         nb.int64[:],  # self._hru_type
-                #         nb.float64,  # NEARZERO
-                #         nb.float64,  # DNEARZERO,
-                #         nb.int32,  # BARESOIL,
-                #         nb.int32,  # GRASSES,
-                #         nb.int32,  # LAND,
-                #         nb.int32,  # LAKE,
-                #         nb.int32,  # RAIN,
-                #         nb.int32,  # SNOW,
-                #         nb.int32,  # OFF,
-                #         nb.int32,  # ACTIVE,
-                #         nb.typeof(self._intercept_numba),  # function.
-                #     ),
-                #     fastmath=True,
-                # )(self._calculate_procedural)
-                self._calculate_numba = nb.njit(
-                    fastmath=True, parallel=nb_parallel
-                )(self._calculate_procedural)
-
-            # <
+        if self._calc_method.lower() != "fortran":
             (
                 self.intcp_evap[:],
                 self.intcp_stor[:],
                 self.net_rain[:],
                 self.net_snow[:],
                 self.net_ppt[:],
                 self.hru_intcpstor[:],
                 self.hru_intcpevap[:],
                 self.intcp_changeover[:],
                 self.intcp_transp_on[:],
-            ) = self._calculate_numba(
-                nhru=np.int32(self.nhru),
-                cov_type=self.cov_type,
-                covden_sum=self.covden_sum,
-                covden_win=self.covden_win,
-                hru_intcpstor=self.hru_intcpstor,
-                hru_intcpevap=self.hru_intcpevap,
-                hru_ppt=self.hru_ppt,
-                hru_rain=self.hru_rain,
-                hru_snow=self.hru_snow,
-                intcp_changeover=self.intcp_changeover,
-                intcp_evap=self.intcp_evap,
-                intcp_form=self.intcp_form,
-                intcp_stor=self.intcp_stor,
-                intcp_transp_on=self.intcp_transp_on,
-                net_ppt=self.net_ppt,
-                net_rain=self.net_rain,
-                net_snow=self.net_snow,
-                pkwater_ante=self.pkwater_ante,
-                potet=self.potet,
-                potet_sublim=self.potet_sublim,
-                snow_intcp=self.snow_intcp,
-                srain_intcp=self.srain_intcp,
-                transp_on=self.transp_on,
-                wrain_intcp=self.wrain_intcp,
-                time_length=time_length,
-                hru_type=self._hru_type,
-                NEARZERO=np.float64(NEARZERO),
-                DNEARZERO=np.float64(DNEARZERO),
-                BARESOIL=np.int32(BARESOIL),
-                GRASSES=np.int32(GRASSES),
-                LAND=np.int32(LAND),
-                LAKE=np.int32(LAKE),
-                RAIN=np.int32(RAIN),
-                SNOW=np.int32(SNOW),
-                OFF=np.int32(OFF),
-                ACTIVE=np.int32(ACTIVE),
-                intercept=self._intercept_numba,
-            )
-
-        elif self._calc_method.lower() in ["none", "numpy"]:
-            (
-                self.intcp_evap[:],
-                self.intcp_stor[:],
-                self.net_rain[:],
-                self.net_snow[:],
-                self.net_ppt[:],
-                self.hru_intcpstor[:],
-                self.hru_intcpevap[:],
-                self.intcp_changeover[:],
-                self.intcp_transp_on[:],
-            ) = self._calculate_procedural(
+            ) = self._calculate_canopy(
                 nhru=np.int32(self.nhru),
                 cov_type=self.cov_type,
                 covden_sum=self.covden_sum,
                 covden_win=self.covden_win,
                 hru_intcpstor=self.hru_intcpstor,
                 hru_intcpevap=self.hru_intcpevap,
                 hru_ppt=self.hru_ppt,
@@ -350,15 +334,15 @@
                 RAIN=np.int32(RAIN),
                 SNOW=np.int32(SNOW),
                 OFF=np.int32(OFF),
                 ACTIVE=np.int32(ACTIVE),
                 intercept=self._intercept,
             )
 
-        elif self._calc_method.lower() == "fortran":
+        else:
             (
                 self.intcp_evap[:],
                 self.intcp_stor[:],
                 self.net_rain[:],
                 self.net_snow[:],
                 self.net_ppt[:],
                 self.hru_intcpstor[:],
@@ -399,27 +383,23 @@
                 np.int32(LAKE),
                 np.int32(RAIN),
                 np.int32(SNOW),
                 np.int32(OFF),
                 np.int32(ACTIVE),
             )
 
-        else:
-            msg = f"Invalid calc_method={self._calc_method} for {self.name}"
-            raise ValueError(msg)
-
         # <
         self.hru_intcpstor_change[:] = (
             self.hru_intcpstor - self.hru_intcpstor_old
         )
 
         return
 
     @staticmethod
-    def _calculate_procedural(
+    def _calculate_numpy(
         nhru,
         cov_type,
         covden_sum,
         covden_win,
         hru_intcpstor,
         hru_intcpevap,
         hru_ppt,
```

### Comparing `pywatershed-0.1.2/pywatershed/hydrology/PRMSChannel.py` & `pywatershed-0.2.0/pywatershed/hydrology/prms_channel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import platform
-from typing import Tuple
+from typing import Literal, Tuple
+from warnings import warn
 
 import networkx as nx
 import numpy as np
 
-from pywatershed.base.storageUnit import StorageUnit
-
 from ..base.adapter import adaptable
+from ..base.conservative_process import ConservativeProcess
 from ..base.control import Control
 from ..constants import SegmentType, nan, zero
+from ..parameters import Parameters
 
 try:
-    from ..PRMSChannel_f import calc_muskingum_mann as _calculate_fortran
+    from ..prms_channel_f import calc_muskingum_mann as _calculate_fortran
 
     has_prmschannel_f = True
 except ImportError:
     has_prmschannel_f = False
 
 
-class PRMSChannel(StorageUnit):
+class PRMSChannel(ConservativeProcess):
     """PRMS channel flow (muskingum_mann).
 
     The muskingum module was originally developed for the Precipitation Runoff
     Modeling System (PRMS) by Mastin and Vaccaro (2002) and developed further
     by Markstrom and others (2008). This module has been modified from past
     versions to make it more stable for stream network routing in watersheds
     with stream segments with varying travel times. Although this module runs
@@ -58,71 +58,62 @@
 
         K_coef = seg_length / (velocity * 60 * 60)
 
     K_coef values computed greater than 24.0 are set to 24.0, values computed
     less than 0.01 are set to 0.01, and the value for lake HRUs is set to 24.0.
 
     Args:
-        control: control object
-        sroff_vol: surface runoff adapter object
-        ssres_flow_vol: subsurface (gravity) reservoir lateral flow adapter
-            object
-        gwres_flow_vol: groundwater reservoir baseflow adapter object
-        verbose: verbose output boolean (default is False)
-
-
+        control: a Control object
+        discretization: a discretization of class Parameters
+        parameters: a parameter object of class Parameters
+        sroff_vol: Surface runoff to the stream network for each HRU
+        ssres_flow_vol: Interflow volume from gravity and preferential-flow
+            reservoirs to the stream network for each HRU
+        gwres_flow_vol: Groundwater discharge volume from each GWR to the
+            stream network
+        budget_type: one of [None, "warn", "error"]
+        calc_method: one of ["fortran", "numba", "numpy"]. None defaults to
+            "numba".
+        verbose: Print extra information or not?
     """
 
     def __init__(
         self,
         control: Control,
+        discretization: Parameters,
+        parameters: Parameters,
         sroff_vol: adaptable,
         ssres_flow_vol: adaptable,
         gwres_flow_vol: adaptable,
-        verbose: bool = False,
-        calc_method: str = None,
-        budget_type: str = None,
-        load_n_time_batches: int = 1,
-    ) -> "PRMSChannel":
+        budget_type: Literal[None, "warn", "error"] = None,
+        calc_method: Literal["fortran", "numba", "numpy"] = None,
+        verbose: bool = None,
+    ) -> None:
         super().__init__(
             control=control,
-            verbose=verbose,
-            load_n_time_batches=load_n_time_batches,
+            discretization=discretization,
+            parameters=parameters,
         )
         self.name = "PRMSChannel"
 
-        self._calc_method = str(calc_method)
-
         self._set_inputs(locals())
-        # override for now until the channel budget is sorted out
-        self._set_budget(budget_type, basis="global")
+        self._set_options(locals())
 
-        # process channel data
+        self._set_budget(basis="global")
         self._initialize_channel_data()
+        self._init_calc_method()
 
         return
 
     @staticmethod
     def get_dimensions() -> tuple:
-        """Get channel segment dimensions
-
-        Returns:
-            dimensions: input dimensions
-
-        """
-        return ("nhru", "nssr", "ngw", "nsegment")
+        return ("nhru", "nsegment")
 
     @staticmethod
     def get_parameters() -> tuple:
-        """Get channel segment parameters
-
-        Returns:
-            parameters: input parameters
-
-        """
         return (
             "hru_area",
             "hru_segment",
             "mann_n",
             "seg_depth",
             "seg_length",
             "seg_slope",
@@ -133,73 +124,70 @@
             "segment_flow_init",
             "obsin_segment",
             "obsout_segment",
         )
 
     @staticmethod
     def get_inputs() -> tuple:
-        """Get channel segment input variables
-
-        Returns:
-            variables: input variables
-
-        """
         return (
             "sroff_vol",
             "ssres_flow_vol",
             "gwres_flow_vol",
         )
 
     @staticmethod
     def get_init_values() -> dict:
-        """Get channel segment initial values
-
-        Returns:
-            dict: initial values for named variables
-        """
         return {
+            "channel_sroff_vol": nan,
+            "channel_ssres_flow_vol": nan,
+            "channel_gwres_flow_vol": nan,
             "channel_outflow_vol": nan,
             "seg_lateral_inflow": zero,
             "seg_upstream_inflow": zero,
             "seg_outflow": zero,
             "seg_stor_change": zero,
         }
 
     @staticmethod
     def get_mass_budget_terms():
         return {
-            "inputs": ["sroff_vol", "ssres_flow_vol", "gwres_flow_vol"],
+            "inputs": [
+                "channel_sroff_vol",
+                "channel_ssres_flow_vol",
+                "channel_gwres_flow_vol",
+            ],
             "outputs": ["channel_outflow_vol"],
             "storage_changes": ["seg_stor_change"],
         }
 
     def get_outflow_mask(self):
         return self._outflow_mask
 
     @property
     def outflow_mask(self):
         return self._outflow_mask
 
     def _set_initial_conditions(self) -> None:
         # initialize channel segment storage
-        self.seg_outflow = self.segment_flow_init
+        self.seg_outflow[:] = self.segment_flow_init
         return
 
     def _initialize_channel_data(self) -> None:
         """Initialize internal variables from raw channel data"""
 
         # convert prms data to zero-based
-        self.hru_segment -= 1
-        self.tosegment -= 1
+        self._hru_segment = self.hru_segment - 1
+        self._tosegment = self.tosegment - 1
+        self._tosegment = self._tosegment.astype("int64")
 
         # calculate connectivity
-        self._outflow_mask = np.full((len(self.tosegment)), False)
+        self._outflow_mask = np.full((len(self._tosegment)), False)
         connectivity = []
         for iseg in range(self.nsegment):
-            tosegment = self.tosegment[iseg]
+            tosegment = self._tosegment[iseg]
             if tosegment < 0:
                 self._outflow_mask[iseg] = True
                 continue
             connectivity.append(
                 (
                     iseg,
                     tosegment,
@@ -221,15 +209,15 @@
         seg_ord_set = set(segment_order)
         mask_not_seg_ord = list(wh_mask_set - seg_ord_set)
         if len(mask_not_seg_ord):
             segment_order = mask_not_seg_ord + segment_order
             # for pp in mask_not_seg_ord:
             #    assert (tosegment[pp] == -1) and (not pp in tosegment)
 
-        self._segment_order = np.array(segment_order, dtype=int)
+        self._segment_order = np.array(segment_order, dtype="int64")
 
         # calculate the Muskingum parameters
         velocity = (
             (
                 (1.0 / self.mann_n)
                 * np.sqrt(self.seg_slope)
                 * self.seg_depth ** (2.0 / 3.0)
@@ -256,15 +244,15 @@
         Kcoef = np.where(
             self.segment_type == SegmentType.LAKE.value, 24.0, Kcoef
         )
         Kcoef = np.where(Kcoef < 0.01, 0.01, Kcoef)
         self._Kcoef = np.where(Kcoef > 24.0, 24.0, Kcoef)
 
         self._ts = np.ones(self.nsegment, dtype=float)
-        self._tsi = np.ones(self.nsegment, dtype=int)
+        self._tsi = np.ones(self.nsegment, dtype="int64")
 
         # todo: vectorize this
         for iseg in range(self.nsegment):
             k = self._Kcoef[iseg]
             if k < 1.0:
                 self._tsi[iseg] = -1
             elif k < 2.0:
@@ -315,178 +303,131 @@
         self._seg_inflow0 = np.zeros(self.nsegment, dtype=float) * nan
         self._inflow_ts = np.zeros(self.nsegment, dtype=float)
         self._outflow_ts = np.zeros(self.nsegment, dtype=float)
         self._seg_current_sum = np.zeros(self.nsegment, dtype=float)
 
         # initialize internal self_inflow variable
         for iseg in range(self.nsegment):
-            jseg = self.tosegment[iseg]
+            jseg = self._tosegment[iseg]
             if jseg < 0:
                 continue
             self._seg_inflow[jseg] = self.seg_outflow[iseg]
 
         return
 
-    def _advance_variables(self) -> None:
-        """Advance the channel segment variables
-        Returns:
-            None
-        """
-        self._seg_inflow0[:] = self._seg_inflow
-        return
+    def _init_calc_method(self):
+        if self._calc_method is None:
+            self._calc_method = "numba"
+
+        avail_methods = ["numpy", "numba", "fortran"]
+        fortran_msg = ""
+        if self._calc_method == "fortran" and not has_prmschannel_f:
+            _ = avail_methods.remove("fortran")
+            fortran_msg = "\n(Fortran not available as installed)\n"
+
+        if self._calc_method.lower() not in avail_methods:
+            msg = (
+                f"Invalid calc_method={self._calc_method} for {self.name}. "
+                f"{fortran_msg}"
+                f"Setting calc_method to 'numba' for {self.name}"
+            )
+            warn(msg)
+            self._calc_method = "numba"
 
-    def _calculate(self, simulation_time: float) -> None:
-        """Calculate channel segment terms for a time step
+        if self._calc_method.lower() == "numba":
+            import numba as nb
 
-        Args:
-            simulation_time: current simulation time
+            numba_msg = f"{self.name} jit compiling with numba "
+            # this method can not be parallelized (? true?)
+            print(numba_msg, flush=True)
+
+            self._muskingum_mann = nb.njit(
+                nb.types.UniTuple(nb.float64[:], 7)(
+                    nb.int64[:],  # _segment_order
+                    nb.int64[:],  # _tosegment
+                    nb.float64[:],  # seg_lateral_inflow
+                    nb.float64[:],  # _seg_inflow0
+                    nb.float64[:],  # _outflow_ts
+                    nb.int64[:],  # _tsi
+                    nb.float64[:],  # _ts
+                    nb.float64[:],  # _c0
+                    nb.float64[:],  # _c1
+                    nb.float64[:],  # _c2
+                ),
+                fastmath=True,
+                parallel=False,
+            )(self._muskingum_mann_numpy)
 
-        Returns:
-            None
+        elif self._calc_method.lower() == "fortran":
+            self._muskingum_mann = _calculate_fortran
+
+        else:
+            self._muskingum_mann = self._muskingum_mann_numpy
 
-        """
+    def _advance_variables(self) -> None:
+        self._seg_inflow0[:] = self._seg_inflow
+        return
 
+    def _calculate(self, simulation_time: float) -> None:
         self._simulation_time = simulation_time
 
         # This could vary with timestep so leave here
         s_per_time = self.control.time_step_seconds
 
         # WRITE a function for this?
         # calculate lateral flow term
         self.seg_lateral_inflow[:] = 0.0
         for ihru in range(self.nhru):
-            iseg = self.hru_segment[ihru]
+            iseg = self._hru_segment[ihru]
             if iseg < 0:
                 # This is bad, selective handling of fluxes is not cool,
                 # mass is being discarded in a way that has to be coordinated
                 # with other parts of the code.
                 # This code shuold be removed evenutally.
-                self.sroff_vol[ihru] = zero
-                self.ssres_flow_vol[ihru] = zero
-                self.gwres_flow_vol[ihru] = zero
+                self.channel_sroff_vol[ihru] = zero
+                self.channel_ssres_flow_vol[ihru] = zero
+                self.channel_gwres_flow_vol[ihru] = zero
                 continue
 
+            else:
+                self.channel_sroff_vol[ihru] = self.sroff_vol[ihru]
+                self.channel_ssres_flow_vol[ihru] = self.ssres_flow_vol[ihru]
+                self.channel_gwres_flow_vol[ihru] = self.gwres_flow_vol[ihru]
+
             # cubicfeet to cfs
             lateral_inflow = (
-                self.sroff_vol[ihru]
-                + self.ssres_flow_vol[ihru]
-                + self.gwres_flow_vol[ihru]
+                self.channel_sroff_vol[ihru]
+                + self.channel_ssres_flow_vol[ihru]
+                + self.channel_gwres_flow_vol[ihru]
             ) / (s_per_time)
 
             self.seg_lateral_inflow[iseg] += lateral_inflow
 
         # solve muskingum_mann routing
-        if self._calc_method.lower() == "numba":
-            import numba as nb
-
-            if not hasattr(self, "_muskingum_mann_numba"):
-                # This is annoying that long integers on windows are 32bit
-                if platform.system() == "Windows":
-                    self._muskingum_mann_numba = nb.njit(
-                        nb.types.UniTuple(nb.float64[:], 7)(
-                            nb.int32[:],  # _segment_order
-                            nb.int32[:],  # tosegment
-                            nb.float64[:],  # seg_lateral_inflow
-                            nb.float64[:],  # _seg_inflow0
-                            nb.float64[:],  # _outflow_ts
-                            nb.int32[:],  # _tsi
-                            nb.float64[:],  # _ts
-                            nb.float64[:],  # _c0
-                            nb.float64[:],  # _c1
-                            nb.float64[:],  # _c2
-                        ),
-                        fastmath=True,
-                        parallel=False,
-                    )(self._muskingum_mann_numpy)
-
-                else:
-                    self._muskingum_mann_numba = nb.njit(
-                        nb.types.UniTuple(nb.float64[:], 7)(
-                            nb.int64[:],  # _segment_order
-                            nb.int64[:],  # tosegment
-                            nb.float64[:],  # seg_lateral_inflow
-                            nb.float64[:],  # _seg_inflow0
-                            nb.float64[:],  # _outflow_ts
-                            nb.int64[:],  # _tsi
-                            nb.float64[:],  # _ts
-                            nb.float64[:],  # _c0
-                            nb.float64[:],  # _c1
-                            nb.float64[:],  # _c2
-                        ),
-                        fastmath=True,
-                    )(self._muskingum_mann_numpy)
 
-            (
-                self.seg_upstream_inflow[:],
-                self._seg_inflow0[:],
-                self._seg_inflow[:],
-                self.seg_outflow[:],
-                self._inflow_ts[:],
-                self._outflow_ts[:],
-                self._seg_current_sum[:],
-            ) = self._muskingum_mann_numba(
-                self._segment_order,
-                self.tosegment,
-                self.seg_lateral_inflow,
-                self._seg_inflow0,
-                self._outflow_ts,
-                self._tsi,
-                self._ts,
-                self._c0,
-                self._c1,
-                self._c2,
-            )
-
-        elif self._calc_method.lower() in ["none", "numpy"]:
-            (
-                self.seg_upstream_inflow[:],
-                self._seg_inflow0[:],
-                self._seg_inflow[:],
-                self.seg_outflow[:],
-                self._inflow_ts[:],
-                self._outflow_ts[:],
-                self._seg_current_sum[:],
-            ) = self._muskingum_mann_numpy(
-                self._segment_order,
-                self.tosegment,
-                self.seg_lateral_inflow,
-                self._seg_inflow0,
-                self._outflow_ts,
-                self._tsi,
-                self._ts,
-                self._c0,
-                self._c1,
-                self._c2,
-            )
-
-        elif self._calc_method.lower() == "fortran":
-            (
-                self.seg_upstream_inflow[:],
-                self._seg_inflow0[:],
-                self._seg_inflow[:],
-                self.seg_outflow[:],
-                self._inflow_ts[:],
-                self._outflow_ts[:],
-                self._seg_current_sum[:],
-            ) = _calculate_fortran(
-                self._segment_order,
-                self.tosegment,
-                self.seg_lateral_inflow,
-                self._seg_inflow0,
-                self._outflow_ts,
-                self._tsi,
-                self._ts,
-                self._c0,
-                self._c1,
-                self._c2,
-            )
-
-        else:
-            msg = f"Invalid calc_method={self._calc_method} for {self.name}"
-            raise ValueError(msg)
+        (
+            self.seg_upstream_inflow[:],
+            self._seg_inflow0[:],
+            self._seg_inflow[:],
+            self.seg_outflow[:],
+            self._inflow_ts[:],
+            self._outflow_ts[:],
+            self._seg_current_sum[:],
+        ) = self._muskingum_mann(
+            self._segment_order,
+            self._tosegment,
+            self.seg_lateral_inflow,
+            self._seg_inflow0,
+            self._outflow_ts,
+            self._tsi,
+            self._ts,
+            self._c0,
+            self._c1,
+            self._c2,
+        )
 
         self.seg_stor_change[:] = (
             self._seg_inflow - self.seg_outflow
         ) * s_per_time
 
         self.channel_outflow_vol[:] = (
             np.where(self._outflow_mask, self.seg_outflow, zero)
```

### Comparing `pywatershed-0.1.2/pywatershed/hydrology/PRMSEt.py` & `pywatershed-0.2.0/pywatershed/hydrology/prms_et.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 import numpy as np
 
 from pywatershed.base.budget import Budget
-from pywatershed.base.storageUnit import StorageUnit
+from pywatershed.base.process import Process
 
 from ..base.adapter import adaptable
 from ..base.control import Control
 from ..constants import nan, one, zero
+from ..parameters import Parameters
 
 # THis class seems to be a sort of intermediate class that should
 # not exist in the future.
 # PRMS: solution is calculate hru_actet at the bottom of the chain, in
 #       soilzone.
 # pywatershed solution: potet and hru_actet are in atmosphere. potet is an "input"
 #       and avail_potet is passed around, resulting in hru_actet at the
 #       end of each time calculation.
 
 
-class PRMSEt(StorageUnit):
+class PRMSEt(Process):
     def __init__(
         self,
         control: Control,
+        discretization: Parameters,
+        parameters: Parameters,
         potet: adaptable,
         hru_impervevap: adaptable,
         hru_intcpevap: adaptable,
         snow_evap: adaptable,
         dprst_evap_hru: adaptable,
         perv_actet: adaptable,
         verbose: bool = False,
         budget_type: str = None,
     ) -> "PRMSEt":
         super().__init__(
             control=control,
-            verbose=verbose,
+            discretization=discretization,
+            parameters=parameters,
         )
         self.name = "PRMSEt"
 
         self._set_inputs(locals())
+        self._set_options(locals())
 
         # Cant set the default budget for ET
         # self.set_budget(budget_type)
         # because the input/output conventions dont match.
         # potet is an "input" but all the other inputs to
         # the class are actually outputs
```

### Comparing `pywatershed-0.1.2/pywatershed/hydrology/PRMSRunoff.py` & `pywatershed-0.2.0/pywatershed/hydrology/prms_runoff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from typing import Literal
+from warnings import warn
+
 import numpy as np
 from numba import prange
 
-from pywatershed.base.storageUnit import StorageUnit
-
 from ..base.adapter import adaptable
+from ..base.conservative_process import ConservativeProcess
 from ..base.control import Control
 from ..constants import HruType, nan, numba_num_threads, zero
+from ..parameters import Parameters
 
 NEARZERO = 1.0e-6
 DNEARZERO = np.finfo(float).eps  # EPSILON(0.0D0)
 
 RAIN = 0
 SNOW = 1
 
@@ -19,51 +22,81 @@
 OFF = 0
 ACTIVE = 1
 
 LAND = HruType.LAND.value
 LAKE = HruType.LAKE.value
 
 
-class PRMSRunoff(StorageUnit):
-    """PRMS surface runoff."""
+class PRMSRunoff(ConservativeProcess):
+    """PRMS surface runoff.
+
+    Args:
+        control: a Control object
+        discretization: a discretization of class Parameters
+        parameters: a parameter object of class Parameters
+        soil_moist_prev: Previous storage of capillary reservoir for each
+            HRU
+        net_ppt: Precipitation (rain and/or snow) that falls through the
+            canopy for each HRU
+        net_rain: Rain that falls through canopy for each HRU
+        net_snow: Snow that falls through canopy for each HRU
+        potet: Potential ET for each HRU
+        snowmelt: Snowmelt from snowpack on each HRU
+        snow_evap: Evaporation and sublimation from snowpack on each HRU
+        pkwater_equiv: Snowpack water equivalent on each HRU
+        pptmix_nopack: Flag indicating that a mixed precipitation event has
+            occurred with no snowpack
+        snowcov_area: Snow-covered area on each HRU prior to melt and
+            sublimation unless snowpack
+        through_rain: Rain that passes through snow when no snow present
+        hru_intcpevap: HRU area-weighted average evaporation from the
+            canopy for each HRU
+        intcp_changeover: Canopy throughfall caused by canopy density
+            change from winter to summer
+        budget_type: one of [None, "warn", "error"]
+        calc_method: one of ["fortran", "numba", "numpy"]. None defaults to
+            "numba".
+        verbose: Print extra information or not?
+    """
 
     def __init__(
         self,
         control: Control,
+        discretization: Parameters,
+        parameters: Parameters,
         soil_moist_prev: adaptable,
-        net_rain: adaptable,
         net_ppt: adaptable,
+        net_rain: adaptable,
         net_snow: adaptable,
         potet: adaptable,
         snowmelt: adaptable,
         snow_evap: adaptable,
         pkwater_equiv: adaptable,
         pptmix_nopack: adaptable,
         snowcov_area: adaptable,
         through_rain: adaptable,
         hru_intcpevap: adaptable,
         intcp_changeover: adaptable,
-        budget_type: str = None,
-        calc_method: str = None,
-        verbose: bool = False,
-        load_n_time_batches: int = 1,
-    ) -> "PRMSRunoff":
+        budget_type: Literal[None, "warn", "error"] = None,
+        calc_method: Literal["numba", "numpy"] = None,
+        verbose: bool = None,
+    ) -> None:
         super().__init__(
             control=control,
-            verbose=verbose,
-            load_n_time_batches=load_n_time_batches,
+            discretization=discretization,
+            parameters=parameters,
         )
-        self.name = "PRMSRunoff"
 
-        self._calc_method = str(calc_method)
+        self.name = "PRMSRunoff"
 
         self._set_inputs(locals())
+        self._set_options(locals())
 
-        self._set_budget(budget_type)
-
+        self._set_budget()
+        self._init_calc_method()
         return
 
     def _set_initial_conditions(self):
         # Where does the initial storage come from? Document here.
         # apparently it's just zero?
         # self.var1_stor[:] = np.zeros([1])[0]
         # self.var1_stor_old = None
@@ -84,29 +117,22 @@
         # call the depression storage init
         self.dprst_init()
 
         return
 
     @staticmethod
     def get_dimensions() -> tuple:
-        """
-        Return a list of the dimensions required for this process
-
-        """
         return ("nhru",)
 
     @staticmethod
     def get_parameters() -> tuple:
-        """
-        Return a list of the parameters required for this process
-
-        """
         return (
             "hru_type",
             "hru_area",
+            "hru_in_to_cf",
             "hru_percent_imperv",
             "imperv_stor_max",
             "dprst_frac",
             "carea_max",
             "smidx_coef",
             "smidx_exp",
             "soil_moist_max",
@@ -124,20 +150,14 @@
             "va_open_exp",
             "va_clos_exp",
             "op_flow_thres",
         )
 
     @staticmethod
     def get_inputs() -> tuple:
-        """Get input variables
-
-        Returns:
-            variables: input variables
-
-        """
         return (
             "soil_moist_prev",
             "net_rain",
             "net_ppt",
             "net_snow",
             "potet",
             "snowmelt",
@@ -148,19 +168,14 @@
             "through_rain",
             "hru_intcpevap",
             "intcp_changeover",
         )
 
     @staticmethod
     def get_init_values() -> dict:
-        """Get initial values
-
-        Returns:
-            dict: initial values for named variables
-        """
         return {
             "contrib_fraction": zero,
             "infil": zero,
             "infil_hru": zero,
             "sroff": zero,  # todo: privatize and only make vol public
             "sroff_vol": zero,
             "hru_sroffp": zero,
@@ -348,254 +363,159 @@
                     self.dprst_vol_frac[i] = (
                         self.dprst_vol_open[i] + self.dprst_vol_clos[i]
                     ) / (
                         self.dprst_vol_open_max[i] + self.dprst_vol_clos_max[i]
                     )
         return
 
-    def _advance_variables(self) -> None:
-        """Advance the variables
-        Returns:
-            None
-        """
-        self.hru_impervstor_old[:] = self.hru_impervstor
-        self.dprst_stor_hru_old[:] = self.dprst_stor_hru
-        return None
-
-    def _calculate(self, time_length, vectorized=False):
-        """Calculate terms for a time step
-
-        Args:
-            simulation_time: current simulation time
-
-        Returns:
-            None
+    def _init_calc_method(self):
+        if self._calc_method is None:
+            self._calc_method = "numba"
+
+        if self._calc_method.lower() not in ["numpy", "numba"]:
+            msg = (
+                f"Invalid calc_method={self._calc_method} for {self.name}. "
+                f"Setting calc_method to 'numba' for {self.name}"
+            )
+            warn(msg)
+            self._calc_method = "numba"
 
-        """
-        # perform the core calculations
         if self._calc_method.lower() == "numba":
             import numba as nb
 
-            if not hasattr(self, "_calculate_numba"):
-                numba_msg = f"{self.name} using numba "
-                nb_parallel = (numba_num_threads is not None) and (
-                    numba_num_threads > 1
-                )
-                if nb_parallel:
-                    numba_msg += f"with {numba_num_threads} threads"
-                print(numba_msg, flush=True)
-
-                self._calculate_numba = nb.njit(
-                    self._calculate_numpy, parallel=nb_parallel
-                )
-                self.check_capacity_numba = nb.jit(self.check_capacity)
-                self.perv_comp_numba = nb.jit(self.perv_comp)
-                self.compute_infil_numba = nb.jit(self.compute_infil)
-                self.dprst_comp_numba = nb.jit(self.dprst_comp)
-                self.imperv_et_numba = nb.jit(self.imperv_et)
-
-            # <
-            (
-                self.infil[:],
-                self.contrib_fraction[:],
-                self.hru_sroffp[:],
-                self.hru_sroffi[:],
-                self.imperv_evap[:],
-                self.hru_impervevap[:],
-                self.imperv_stor[:],
-                self.dprst_in[:],
-                self.dprst_vol_open[:],
-                self.dprst_vol_clos[:],
-                self.dprst_sroff_hru[:],
-                self.dprst_evap_hru[:],
-                self.dprst_seep_hru[:],
-                self.dprst_insroff_hru[:],
-                self.dprst_vol_open_frac[:],
-                self.dprst_vol_clos_frac[:],
-                self.dprst_vol_frac[:],
-                self.dprst_stor_hru[:],
-                self.sroff[:],
-            ) = self._calculate_numba(
-                infil=self.infil,
-                nhru=self.nhru,
-                hru_area=self.hru_area,
-                hru_perv=self.hru_perv,
-                hru_frac_perv=self.hru_frac_perv,
-                hru_sroffp=self.hru_sroffp,
-                contrib_fraction=self.contrib_fraction,
-                hru_percent_imperv=self.hru_percent_imperv,
-                hru_sroffi=self.hru_sroffi,
-                imperv_evap=self.imperv_evap,
-                hru_imperv=self.hru_imperv,
-                hru_impervevap=self.hru_impervevap,
-                potet=self.potet,
-                snow_evap=self.snow_evap,
-                hru_intcpevap=self.hru_intcpevap,
-                soil_moist_prev=self.soil_moist_prev,
-                soil_moist_max=self.soil_moist_max,
-                carea_max=self.carea_max,
-                smidx_coef=self.smidx_coef,
-                smidx_exp=self.smidx_exp,
-                pptmix_nopack=self.pptmix_nopack,
-                net_rain=self.net_rain,
-                net_ppt=self.net_ppt,
-                imperv_stor=self.imperv_stor,
-                imperv_stor_max=self.imperv_stor_max,
-                snowmelt=self.snowmelt,
-                snowinfil_max=self.snowinfil_max,
-                net_snow=self.net_snow,
-                pkwater_equiv=self.pkwater_equiv,
-                hru_type=self.hru_type,
-                intcp_changeover=self.intcp_changeover,
-                dprst_in=self.dprst_in,
-                dprst_seep_hru=self.dprst_seep_hru,
-                dprst_area_max=self.dprst_area_max,
-                dprst_vol_open=self.dprst_vol_open,
-                dprst_vol_clos=self.dprst_vol_clos,
-                dprst_sroff_hru=self.dprst_sroff_hru,
-                dprst_evap_hru=self.dprst_evap_hru,
-                dprst_insroff_hru=self.dprst_insroff_hru,
-                dprst_vol_open_frac=self.dprst_vol_open_frac,
-                dprst_vol_clos_frac=self.dprst_vol_clos_frac,
-                dprst_vol_frac=self.dprst_vol_frac,
-                dprst_stor_hru=self.dprst_stor_hru,
-                dprst_area_clos_max=self.dprst_area_clos_max,
-                dprst_area_clos=self.dprst_area_clos,
-                dprst_vol_open_max=self.dprst_vol_open_max,
-                dprst_area_open_max=self.dprst_area_open_max,
-                dprst_area_open=self.dprst_area_open,
-                sro_to_dprst_perv=self.sro_to_dprst_perv,
-                sro_to_dprst_imperv=self.sro_to_dprst_imperv,
-                dprst_frac_open=self.dprst_frac_open,
-                dprst_frac_clos=self.dprst_frac_clos,
-                va_open_exp=self.va_open_exp,
-                dprst_vol_clos_max=self.dprst_vol_clos_max,
-                va_clos_exp=self.va_clos_exp,
-                snowcov_area=self.snowcov_area,
-                dprst_et_coef=self.dprst_et_coef,
-                dprst_seep_rate_open=self.dprst_seep_rate_open,
-                dprst_vol_thres_open=self.dprst_vol_thres_open,
-                dprst_flow_coef=self.dprst_flow_coef,
-                dprst_seep_rate_clos=self.dprst_seep_rate_clos,
-                sroff=self.sroff,
-                hru_impervstor=self.hru_impervstor,
-                check_capacity=self.check_capacity_numba,
-                perv_comp=self.perv_comp_numba,
-                compute_infil=self.compute_infil_numba,
-                dprst_comp=self.dprst_comp_numba,
-                imperv_et=self.imperv_et_numba,
+            numba_msg = f"{self.name} jit compiling with numba "
+            nb_parallel = (numba_num_threads is not None) and (
+                numba_num_threads > 1
             )
+            if nb_parallel:
+                numba_msg += f"and using {numba_num_threads} threads"
+            print(numba_msg, flush=True)
 
-        elif self._calc_method.lower() in ["none", "numpy"]:
-            (
-                self.infil[:],
-                self.contrib_fraction[:],
-                self.hru_sroffp[:],
-                self.hru_sroffi[:],
-                self.imperv_evap[:],
-                self.hru_impervevap[:],
-                self.imperv_stor[:],
-                self.dprst_in[:],
-                self.dprst_vol_open[:],
-                self.dprst_vol_clos[:],
-                self.dprst_sroff_hru[:],
-                self.dprst_evap_hru[:],
-                self.dprst_seep_hru[:],
-                self.dprst_insroff_hru[:],
-                self.dprst_vol_open_frac[:],
-                self.dprst_vol_clos_frac[:],
-                self.dprst_vol_frac[:],
-                self.dprst_stor_hru[:],
-                self.sroff[:],
-            ) = self._calculate_numpy(
-                infil=self.infil,
-                nhru=self.nhru,
-                hru_area=self.hru_area,
-                hru_perv=self.hru_perv,
-                hru_frac_perv=self.hru_frac_perv,
-                hru_sroffp=self.hru_sroffp,
-                contrib_fraction=self.contrib_fraction,
-                hru_percent_imperv=self.hru_percent_imperv,
-                hru_sroffi=self.hru_sroffi,
-                imperv_evap=self.imperv_evap,
-                hru_imperv=self.hru_imperv,
-                hru_impervevap=self.hru_impervevap,
-                potet=self.potet,
-                snow_evap=self.snow_evap,
-                hru_intcpevap=self.hru_intcpevap,
-                soil_moist_prev=self.soil_moist_prev,
-                soil_moist_max=self.soil_moist_max,
-                carea_max=self.carea_max,
-                smidx_coef=self.smidx_coef,
-                smidx_exp=self.smidx_exp,
-                pptmix_nopack=self.pptmix_nopack,
-                net_rain=self.net_rain,
-                net_ppt=self.net_ppt,
-                imperv_stor=self.imperv_stor,
-                imperv_stor_max=self.imperv_stor_max,
-                snowmelt=self.snowmelt,
-                snowinfil_max=self.snowinfil_max,
-                net_snow=self.net_snow,
-                pkwater_equiv=self.pkwater_equiv,
-                hru_type=self.hru_type,
-                intcp_changeover=self.intcp_changeover,
-                dprst_in=self.dprst_in,
-                dprst_seep_hru=self.dprst_seep_hru,
-                dprst_area_max=self.dprst_area_max,
-                dprst_vol_open=self.dprst_vol_open,
-                dprst_vol_clos=self.dprst_vol_clos,
-                dprst_sroff_hru=self.dprst_sroff_hru,
-                dprst_evap_hru=self.dprst_evap_hru,
-                dprst_insroff_hru=self.dprst_insroff_hru,
-                dprst_vol_open_frac=self.dprst_vol_open_frac,
-                dprst_vol_clos_frac=self.dprst_vol_clos_frac,
-                dprst_vol_frac=self.dprst_vol_frac,
-                dprst_stor_hru=self.dprst_stor_hru,
-                dprst_area_clos_max=self.dprst_area_clos_max,
-                dprst_area_clos=self.dprst_area_clos,
-                dprst_vol_open_max=self.dprst_vol_open_max,
-                dprst_area_open_max=self.dprst_area_open_max,
-                dprst_area_open=self.dprst_area_open,
-                sro_to_dprst_perv=self.sro_to_dprst_perv,
-                sro_to_dprst_imperv=self.sro_to_dprst_imperv,
-                dprst_frac_open=self.dprst_frac_open,
-                dprst_frac_clos=self.dprst_frac_clos,
-                va_open_exp=self.va_open_exp,
-                dprst_vol_clos_max=self.dprst_vol_clos_max,
-                va_clos_exp=self.va_clos_exp,
-                snowcov_area=self.snowcov_area,
-                dprst_et_coef=self.dprst_et_coef,
-                dprst_seep_rate_open=self.dprst_seep_rate_open,
-                dprst_vol_thres_open=self.dprst_vol_thres_open,
-                dprst_flow_coef=self.dprst_flow_coef,
-                dprst_seep_rate_clos=self.dprst_seep_rate_clos,
-                sroff=self.sroff,
-                hru_impervstor=self.hru_impervstor,
-                check_capacity=self.check_capacity,
-                perv_comp=self.perv_comp,
-                compute_infil=self.compute_infil,
-                dprst_comp=self.dprst_comp,
-                imperv_et=self.imperv_et,
+            self._calculate_runoff = nb.njit(
+                self._calculate_numpy, parallel=nb_parallel
             )
+            self.check_capacity = nb.njit(self.check_capacity)
+            self.perv_comp = nb.njit(self.perv_comp)
+            self.compute_infil = nb.njit(self.compute_infil)
+            self.dprst_comp = nb.njit(self.dprst_comp)
+            self.imperv_et = nb.njit(self.imperv_et)
 
         else:
-            msg = f"Invalid calc_method={self._calc_method} for {self.name}"
-            raise ValueError(msg)
+            self._calculate_runoff = self._calculate_numpy
+
+        return
+
+    def _advance_variables(self) -> None:
+        self.hru_impervstor_old[:] = self.hru_impervstor
+        self.dprst_stor_hru_old[:] = self.dprst_stor_hru
+        return None
+
+    def _calculate(self, time_length, vectorized=False):
+        """Perform the core calculations"""
+        (
+            self.infil[:],
+            self.contrib_fraction[:],
+            self.hru_sroffp[:],
+            self.hru_sroffi[:],
+            self.imperv_evap[:],
+            self.hru_impervevap[:],
+            self.imperv_stor[:],
+            self.dprst_in[:],
+            self.dprst_vol_open[:],
+            self.dprst_vol_clos[:],
+            self.dprst_sroff_hru[:],
+            self.dprst_evap_hru[:],
+            self.dprst_seep_hru[:],
+            self.dprst_insroff_hru[:],
+            self.dprst_vol_open_frac[:],
+            self.dprst_vol_clos_frac[:],
+            self.dprst_vol_frac[:],
+            self.dprst_stor_hru[:],
+            self.sroff[:],
+        ) = self._calculate_runoff(
+            infil=self.infil,
+            nhru=self.nhru,
+            hru_area=self.hru_area,
+            hru_perv=self.hru_perv,
+            hru_frac_perv=self.hru_frac_perv,
+            hru_sroffp=self.hru_sroffp,
+            contrib_fraction=self.contrib_fraction,
+            hru_percent_imperv=self.hru_percent_imperv,
+            hru_sroffi=self.hru_sroffi,
+            imperv_evap=self.imperv_evap,
+            hru_imperv=self.hru_imperv,
+            hru_impervevap=self.hru_impervevap,
+            potet=self.potet,
+            snow_evap=self.snow_evap,
+            hru_intcpevap=self.hru_intcpevap,
+            soil_moist_prev=self.soil_moist_prev,
+            soil_moist_max=self.soil_moist_max,
+            carea_max=self.carea_max,
+            smidx_coef=self.smidx_coef,
+            smidx_exp=self.smidx_exp,
+            pptmix_nopack=self.pptmix_nopack,
+            net_rain=self.net_rain,
+            net_ppt=self.net_ppt,
+            imperv_stor=self.imperv_stor,
+            imperv_stor_max=self.imperv_stor_max,
+            snowmelt=self.snowmelt,
+            snowinfil_max=self.snowinfil_max,
+            net_snow=self.net_snow,
+            pkwater_equiv=self.pkwater_equiv,
+            hru_type=self.hru_type,
+            intcp_changeover=self.intcp_changeover,
+            dprst_in=self.dprst_in,
+            dprst_seep_hru=self.dprst_seep_hru,
+            dprst_area_max=self.dprst_area_max,
+            dprst_vol_open=self.dprst_vol_open,
+            dprst_vol_clos=self.dprst_vol_clos,
+            dprst_sroff_hru=self.dprst_sroff_hru,
+            dprst_evap_hru=self.dprst_evap_hru,
+            dprst_insroff_hru=self.dprst_insroff_hru,
+            dprst_vol_open_frac=self.dprst_vol_open_frac,
+            dprst_vol_clos_frac=self.dprst_vol_clos_frac,
+            dprst_vol_frac=self.dprst_vol_frac,
+            dprst_stor_hru=self.dprst_stor_hru,
+            dprst_area_clos_max=self.dprst_area_clos_max,
+            dprst_area_clos=self.dprst_area_clos,
+            dprst_vol_open_max=self.dprst_vol_open_max,
+            dprst_area_open_max=self.dprst_area_open_max,
+            dprst_area_open=self.dprst_area_open,
+            sro_to_dprst_perv=self.sro_to_dprst_perv,
+            sro_to_dprst_imperv=self.sro_to_dprst_imperv,
+            dprst_frac_open=self.dprst_frac_open,
+            dprst_frac_clos=self.dprst_frac_clos,
+            va_open_exp=self.va_open_exp,
+            dprst_vol_clos_max=self.dprst_vol_clos_max,
+            va_clos_exp=self.va_clos_exp,
+            snowcov_area=self.snowcov_area,
+            dprst_et_coef=self.dprst_et_coef,
+            dprst_seep_rate_open=self.dprst_seep_rate_open,
+            dprst_vol_thres_open=self.dprst_vol_thres_open,
+            dprst_flow_coef=self.dprst_flow_coef,
+            dprst_seep_rate_clos=self.dprst_seep_rate_clos,
+            sroff=self.sroff,
+            hru_impervstor=self.hru_impervstor,
+            check_capacity=self.check_capacity,
+            perv_comp=self.perv_comp,
+            compute_infil=self.compute_infil,
+            dprst_comp=self.dprst_comp,
+            imperv_et=self.imperv_et,
+        )
 
-        # <
         self.infil_hru[:] = self.infil * self.hru_frac_perv
 
         self.hru_impervstor_change[:] = (
             self.hru_impervstor - self.hru_impervstor_old
         )
         self.dprst_stor_hru_change[:] = (
             self.dprst_stor_hru - self.dprst_stor_hru_old
         )
 
-        self.sroff_vol = self.sroff * self.control.params.hru_in_to_cf
+        self.sroff_vol[:] = self.sroff * self.hru_in_to_cf
 
         return
 
     @staticmethod
     def _calculate_numpy(
         infil,
         nhru,
@@ -1272,14 +1192,15 @@
             else:
                 ca_fraction = smidx_coef * 10.0 ** (smidx_exp * smidx)
         else:
             raise Exception("you did a bad thing...")
 
         if ca_fraction > carea_max:
             ca_fraction = carea_max
+
         srpp = ca_fraction * pptp
         infil = infil - srpp
         srp = srp + srpp
 
         return infil, srp, ca_fraction
 
     @staticmethod
@@ -1291,14 +1212,15 @@
         infiltration by snowinfil_max, with excess added to runoff
         """
         capacity = soil_moist_max - soil_moist_prev
         excess = infil - capacity
         if excess > snowinfil_max:
             srp = srp + excess - snowinfil_max
             infil = snowinfil_max + capacity
+
         return infil, srp
 
     @staticmethod
     def imperv_et(imperv_stor, potet, imperv_evap, sca, avail_et, imperv_frac):
         if sca < 1.0:
             if potet < imperv_stor:
                 imperv_evap = potet * (1.0 - sca)
```

### Comparing `pywatershed-0.1.2/pywatershed/hydrology/PRMSSnow.py` & `pywatershed-0.2.0/pywatershed/hydrology/prms_snow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+from typing import Literal
+from warnings import warn
+
 import numpy as np
 from numba import prange
 
-from pywatershed.base.storageUnit import StorageUnit
-
 from ..base.adapter import adaptable
+from ..base.conservative_process import ConservativeProcess
 from ..base.control import Control
 from ..constants import (
     HruType,
     epsilon32,
     epsilon64,
     inch2cm,
     nan,
     numba_num_threads,
     one,
     zero,
 )
+from ..parameters import Parameters
 
 # These are constants used like variables (on self) in PRMS6
 # They dont appear on any LHS, so it seems they are constants
 # These should probably be in the parameters?
 acum_init = np.array(
     [
         0.80,
@@ -63,20 +66,52 @@
 ONETHIRD = 1.0 / 3.0
 
 tcind = 0
 
 dbgind = 434
 
 
-class PRMSSnow(StorageUnit):
-    """PRMS snow pack."""
+class PRMSSnow(ConservativeProcess):
+    """PRMS snow pack.
+
+    Args:
+        control: a Control object
+        discretization: a discretization of class Parameters
+        parameters: a parameter object of class Parameters
+        orad_hru: Solar radiation on a horizontal surface for each HRU
+        soltab_horad_potsw: Potential solar radiation on a horizontal plane
+            for each Julian Day for each
+        swrad: Shortwave radiation distributed to each HRU
+        hru_intcpevap: HRU area-weighted average evaporation from the
+            canopy for each HRU
+        hru_ppt: Precipitation distributed to each HRU
+        potet: Potential ET for each HRU
+        pptmix: Flag to indicate if precipitation is a mixture of rain and
+            snow for each HRU
+        prmx: Fraction of rain in a mixed precipitation event for each HRU
+        tavgc: Average air temperature distributed to each HRU
+        tmaxc: Maximum air temperature distributed to each HRU
+        tminc: Minimum air temperature distributed to each HRU
+        net_ppt: Precipitation (rain and/or snow) that falls through the
+            canopy for each HRU
+        net_rain: Rain that falls through canopy for each HRU
+        net_snow: Snow that falls through canopy for each HRU
+        transp_on: Flag indicating whether transpiration is occurring
+            (0=no;1=yes)
+        budget_type: one of [None, "warn", "error"]
+        calc_method: one of ["fortran", "numba", "numpy"]. None defaults to
+            "numba".
+        verbose: Print extra information or not?
+    """
 
     def __init__(
         self,
         control: Control,
+        discretization: Parameters,
+        parameters: Parameters,
         orad_hru: adaptable,
         soltab_horad_potsw: adaptable,
         swrad: adaptable,
         hru_intcpevap: adaptable,
         hru_ppt: adaptable,
         potet: adaptable,
         pptmix: adaptable,
@@ -84,52 +119,41 @@
         tavgc: adaptable,
         tmaxc: adaptable,
         tminc: adaptable,
         net_ppt: adaptable,
         net_rain: adaptable,
         net_snow: adaptable,
         transp_on: adaptable,
-        budget_type: str = None,
-        calc_method: str = None,
-        verbose: bool = False,
-        load_n_time_batches: int = 1,
+        budget_type: Literal[None, "warn", "error"] = None,
+        calc_method: Literal["numba", "numpy"] = None,
+        verbose: bool = None,
     ) -> "PRMSSnow":
         super().__init__(
             control=control,
-            verbose=verbose,
-            load_n_time_batches=load_n_time_batches,
+            discretization=discretization,
+            parameters=parameters,
         )
         self.name = "PRMSSnow"
 
-        self._calc_method = str(calc_method)
-
         self._set_inputs(locals())
-        self._set_budget(budget_type)
+        self._set_options(locals())
+
+        self._set_budget()
+        self._init_calc_method()
 
         return
 
     @staticmethod
     def get_dimensions() -> tuple:
-        """Get snow pack dimensions
-
-        Returns:
-            dimensions: input dimensions
-
-        """
-        return ("nhru", "nmonth", "ndeplval")
+        return ("nhru", "nmonth", "ndoy", "ndeplval")
 
     @staticmethod
     def get_parameters() -> tuple:
-        """Get snow pack parameters
-
-        Returns:
-            parameters: input parameters
-
-        """
         return (
+            "doy",
             "cov_type",
             "covden_win",
             "covden_sum",
             "hru_type",
             "albset_rna",
             "albset_rnm",
             "albset_sna",
@@ -150,20 +174,14 @@
             "tmax_allsnow",
             "cecn_coef",
             "tstorm_mo",
         )
 
     @staticmethod
     def get_inputs() -> tuple:
-        """Get snow pack input variables
-
-        Returns:
-            variables: input variables
-
-        """
         return (
             "hru_ppt",
             "hru_intcpevap",
             "net_ppt",
             "net_rain",
             "net_snow",
             "orad_hru",
@@ -176,20 +194,14 @@
             "tmaxc",
             "tminc",
             "transp_on",
         )
 
     @staticmethod
     def get_init_values() -> dict:
-        """Get snow pack initial values
-
-        Returns:
-            dict: initial values for named variables
-        """
-
         return {
             "ai": zero,
             "albedo": zero,
             "frac_swe": zero,
             "freeh2o": zero,
             "freeh2o_change": nan,
             "freeh2o_prev": nan,
@@ -245,20 +257,14 @@
                 # pkwater_equiv
                 # "pkwater_equiv_change",
             ],
         }
 
     @staticmethod
     def get_restart_variables() -> tuple:
-        """Get snow pack restart variables
-
-        Returns:
-            variables: restart variables
-        """
-
         return (
             "albedo",
             "freeh2o",
             "iasw",
             "int_alb",
             "iso",
             "lso",
@@ -277,16 +283,14 @@
             "slst",
             "snowcov_area",
             "snowcov_areasv",
             "snsv",
         )
 
     def _set_initial_conditions(self):
-        """Initialize PRMSSnow snowpack variables."""
-
         # Derived parameters
         self.tmax_allsnow_c = (self.tmax_allsnow - 32.0) / 1.8
         del self.tmax_allsnow
 
         # Deninv and denmaxinv not in variables nor in metadata but we can set
         # them on self for convenience
         if (self.den_init.shape == ()) or (
@@ -310,15 +314,15 @@
         self.denmaxinv = one / self.den_max
 
         self.pkwater_equiv[:] = self.snowpack_init.copy()
 
         sd = int(self.ndeplval / 11)
         self.snarea_curve_2d = np.reshape(self.snarea_curve, (sd, 11))
 
-        if self.control.config["init_vars_from_file"] in [0, 2, 3]:
+        if self.control.options["init_vars_from_file"] in [0, 2, 3]:
             # The super().__init__ already set_initial_conditions using its
             # set_initial_conditions
             # Below Im just following PRMS6, will reconcile later with the
             # super (may be redundant).
             vars_init = [
                 "albedo",
                 "iasw",
@@ -383,336 +387,204 @@
             raise RuntimeError("Snow restart capability not implemented")
             # JLM: a list of restart variables dosent shed light on what states
             # actually have memory.
             # JLM: could there be a diagnostic part of the advance?
 
         return
 
-    def _advance_variables(self) -> None:
-        self.pkwater_ante[:] = self.pkwater_equiv
-        self.freeh2o_prev[:] = self.freeh2o
-        self.pk_ice_prev[:] = self.pk_ice
-        return
-
-    def _calculate(self, simulation_time):
-        """Calculate canopy terms for a time step
-
-        Args:
-            simulation_time: current simulation time
-
-        Returns:
-            None
+    def _init_calc_method(self):
+        if self._calc_method is None:
+            self._calc_method = "numba"
+
+        if self._calc_method.lower() not in ["numpy", "numba"]:
+            msg = (
+                f"Invalid calc_method={self._calc_method} for {self.name}. "
+                f"Setting calc_method to 'numba' for {self.name}"
+            )
+            warn(msg)
+            self._calc_method = "numba"
 
-        """
         if self._calc_method.lower() == "numba":
             import numba as nb
 
-            if not hasattr(self, "_calculate_numba"):
-                numba_msg = f"{self.name} using numba "
-                nb_parallel = (numba_num_threads is not None) and (
-                    numba_num_threads > 1
-                )
-                if nb_parallel:
-                    numba_msg += f"with {numba_num_threads} threads"
-                print(numba_msg, flush=True)
-
-                self._calculate_numba = nb.njit(
-                    fastmath=True, parallel=nb_parallel
-                )(self._calculate_numpy)
-                fns = [
-                    "_calc_calin",
-                    "_calc_caloss",
-                    "_calc_ppt_to_pack",
-                    "_calc_sca_deplcrv",
-                    "_calc_snalbedo",
-                    "_calc_snowbal",
-                    "_calc_snowcov",
-                    "_calc_snowevap",
-                    "_calc_step_4",
-                ]
-                for fn in fns:
-                    setattr(
-                        self,
-                        f"{fn}_numba",
-                        nb.njit(fastmath=True)(getattr(self, fn)),
-                    )
-
-            # <
-            (
-                self.ai[:],
-                self.albedo[:],
-                self.frac_swe[:],
-                self.freeh2o[:],
-                self.freeh2o_change[:],
-                self.iasw[:],
-                self.int_alb[:],
-                self.iso[:],
-                self.lso[:],
-                self.lst[:],
-                self.mso[:],
-                self.newsnow[:],
-                self.pk_def[:],
-                self.pk_den[:],
-                self.pk_depth[:],
-                self.pk_ice[:],
-                self.pk_ice_change[:],
-                self.pk_precip[:],
-                self.pk_temp[:],
-                self.pksv[:],
-                self.pkwater_equiv[:],
-                self.pkwater_equiv_change[:],
-                self.pptmix_nopack[:],
-                self.pss[:],
-                self.pst[:],
-                self.salb[:],
-                self.scrv[:],
-                self.slst[:],
-                self.snow_evap[:],
-                self.snowcov_area[:],
-                self.snowcov_areasv[:],
-                self.snowmelt[:],
-                self.snsv[:],
-                self.tcal[:],
-                self.through_rain[:],
-            ) = self._calculate_numba(
-                acum_init=acum_init,
-                ai=self.ai,
-                albedo=self.albedo,
-                albset_rna=self.albset_rna,
-                albset_rnm=self.albset_rnm,
-                albset_sna=self.albset_sna,
-                albset_snm=self.albset_snm,
-                amlt_init=amlt_init,
-                calc_calin=self._calc_calin_numba,
-                calc_caloss=self._calc_caloss_numba,
-                calc_ppt_to_pack=self._calc_ppt_to_pack_numba,
-                calc_sca_deplcrv=self._calc_sca_deplcrv_numba,
-                calc_snalbedo=self._calc_snalbedo_numba,
-                calc_snowbal=self._calc_snowbal_numba,
-                calc_snowcov=self._calc_snowcov_numba,
-                calc_snowevap=self._calc_snowevap_numba,
-                calc_step_4=self._calc_step_4_numba,
-                cecn_coef=self.cecn_coef,
-                cov_type=self.cov_type,
-                covden_sum=self.covden_sum,
-                covden_win=self.covden_win,
-                current_dowy=self.control.current_dowy,
-                current_doy=self.control.current_doy,
-                current_month=self.control.current_month,
-                den_max=self.den_max,
-                deninv=self.deninv,
-                denmaxinv=self.denmaxinv,
-                emis_noppt=self.emis_noppt,
-                frac_swe=self.frac_swe,
-                freeh2o=self.freeh2o,
-                freeh2o_cap=self.freeh2o_cap,
-                freeh2o_change=self.freeh2o_change,
-                freeh2o_prev=self.freeh2o_prev,
-                hru_deplcrv=self.hru_deplcrv,
-                hru_intcpevap=self.hru_intcpevap,
-                hru_ppt=self.hru_ppt,
-                hru_type=self.hru_type,
-                iasw=self.iasw,
-                int_alb=self.int_alb,
-                iso=self.iso,
-                itime_step=self.control.itime_step,
-                lso=self.lso,
-                lst=self.lst,
-                melt_force=self.melt_force,
-                melt_look=self.melt_look,
-                mso=self.mso,
-                net_ppt=self.net_ppt,
-                net_rain=self.net_rain,
-                net_snow=self.net_snow,
-                newsnow=self.newsnow,
-                nhru=self.nhru,
-                orad_hru=self.orad_hru,
-                pk_def=self.pk_def,
-                pk_den=self.pk_den,
-                pk_depth=self.pk_depth,
-                pk_ice=self.pk_ice,
-                pk_ice_change=self.pk_ice_change,
-                pk_ice_prev=self.pk_ice_prev,
-                pk_precip=self.pk_precip,
-                pk_temp=self.pk_temp,
-                pksv=self.pksv,
-                pkwater_ante=self.pkwater_ante,
-                pkwater_equiv=self.pkwater_equiv,
-                pkwater_equiv_change=self.pkwater_equiv_change,
-                potet=self.potet,
-                potet_sublim=self.potet_sublim,
-                pptmix=self.pptmix,
-                pptmix_nopack=self.pptmix_nopack,
-                prmx=self.prmx,
-                pss=self.pss,
-                pst=self.pst,
-                rad_trncf=self.rad_trncf,
-                salb=self.salb,
-                scrv=self.scrv,
-                settle_const=self.settle_const,
-                simulation_time=simulation_time,
-                slst=self.slst,
-                snarea_curve_2d=self.snarea_curve_2d,
-                snarea_thresh=self.snarea_thresh,
-                snow_evap=self.snow_evap,
-                snowcov_area=self.snowcov_area,
-                snowcov_areasv=self.snowcov_areasv,
-                snowmelt=self.snowmelt,
-                snsv=self.snsv,
-                soltab_horad_potsw=self.soltab_horad_potsw,
-                swrad=self.swrad,
-                tavgc=self.tavgc,
-                tcal=self.tcal,
-                through_rain=self.through_rain,
-                tmax_allsnow_c=self.tmax_allsnow_c,
-                tmaxc=self.tmaxc,
-                tminc=self.tminc,
-                transp_on=self.transp_on,
-                tstorm_mo=self.tstorm_mo,
-                verbose=self.verbose,
-            )
-
-        elif self._calc_method.lower() in ["none", "numpy"]:
-            (
-                self.ai[:],
-                self.albedo[:],
-                self.frac_swe[:],
-                self.freeh2o[:],
-                self.freeh2o_change[:],
-                self.iasw[:],
-                self.int_alb[:],
-                self.iso[:],
-                self.lso[:],
-                self.lst[:],
-                self.mso[:],
-                self.newsnow[:],
-                self.pk_def[:],
-                self.pk_den[:],
-                self.pk_depth[:],
-                self.pk_ice[:],
-                self.pk_ice_change[:],
-                self.pk_precip[:],
-                self.pk_temp[:],
-                self.pksv[:],
-                self.pkwater_equiv[:],
-                self.pkwater_equiv_change[:],
-                self.pptmix_nopack[:],
-                self.pss[:],
-                self.pst[:],
-                self.salb[:],
-                self.scrv[:],
-                self.slst[:],
-                self.snow_evap[:],
-                self.snowcov_area[:],
-                self.snowcov_areasv[:],
-                self.snowmelt[:],
-                self.snsv[:],
-                self.tcal[:],
-                self.through_rain[:],
-            ) = self._calculate_numpy(
-                acum_init=acum_init,
-                ai=self.ai,
-                albedo=self.albedo,
-                albset_rna=self.albset_rna,
-                albset_rnm=self.albset_rnm,
-                albset_sna=self.albset_sna,
-                albset_snm=self.albset_snm,
-                amlt_init=amlt_init,
-                calc_calin=self._calc_calin,
-                calc_caloss=self._calc_caloss,
-                calc_ppt_to_pack=self._calc_ppt_to_pack,
-                calc_sca_deplcrv=self._calc_sca_deplcrv,
-                calc_snalbedo=self._calc_snalbedo,
-                calc_snowbal=self._calc_snowbal,
-                calc_snowcov=self._calc_snowcov,
-                calc_snowevap=self._calc_snowevap,
-                calc_step_4=self._calc_step_4,
-                cecn_coef=self.cecn_coef,
-                cov_type=self.cov_type,
-                covden_sum=self.covden_sum,
-                covden_win=self.covden_win,
-                current_dowy=self.control.current_dowy,
-                current_doy=self.control.current_doy,
-                current_month=self.control.current_month,
-                den_max=self.den_max,
-                deninv=self.deninv,
-                denmaxinv=self.denmaxinv,
-                emis_noppt=self.emis_noppt,
-                frac_swe=self.frac_swe,
-                freeh2o=self.freeh2o,
-                freeh2o_cap=self.freeh2o_cap,
-                freeh2o_change=self.freeh2o_change,
-                freeh2o_prev=self.freeh2o_prev,
-                hru_deplcrv=self.hru_deplcrv,
-                hru_intcpevap=self.hru_intcpevap,
-                hru_ppt=self.hru_ppt,
-                hru_type=self.hru_type,
-                iasw=self.iasw,
-                int_alb=self.int_alb,
-                iso=self.iso,
-                itime_step=self.control.itime_step,
-                lso=self.lso,
-                lst=self.lst,
-                melt_force=self.melt_force,
-                melt_look=self.melt_look,
-                mso=self.mso,
-                net_ppt=self.net_ppt,
-                net_rain=self.net_rain,
-                net_snow=self.net_snow,
-                newsnow=self.newsnow,
-                nhru=self.nhru,
-                orad_hru=self.orad_hru,
-                pk_def=self.pk_def,
-                pk_den=self.pk_den,
-                pk_depth=self.pk_depth,
-                pk_ice=self.pk_ice,
-                pk_ice_change=self.pk_ice_change,
-                pk_ice_prev=self.pk_ice_prev,
-                pk_precip=self.pk_precip,
-                pk_temp=self.pk_temp,
-                pksv=self.pksv,
-                pkwater_ante=self.pkwater_ante,
-                pkwater_equiv=self.pkwater_equiv,
-                pkwater_equiv_change=self.pkwater_equiv_change,
-                potet=self.potet,
-                potet_sublim=self.potet_sublim,
-                pptmix=self.pptmix,
-                pptmix_nopack=self.pptmix_nopack,
-                prmx=self.prmx,
-                pss=self.pss,
-                pst=self.pst,
-                rad_trncf=self.rad_trncf,
-                salb=self.salb,
-                scrv=self.scrv,
-                settle_const=self.settle_const,
-                simulation_time=simulation_time,
-                slst=self.slst,
-                snarea_curve_2d=self.snarea_curve_2d,
-                snarea_thresh=self.snarea_thresh,
-                snow_evap=self.snow_evap,
-                snowcov_area=self.snowcov_area,
-                snowcov_areasv=self.snowcov_areasv,
-                snowmelt=self.snowmelt,
-                snsv=self.snsv,
-                soltab_horad_potsw=self.soltab_horad_potsw,
-                swrad=self.swrad,
-                tavgc=self.tavgc,
-                tcal=self.tcal,
-                through_rain=self.through_rain,
-                tmax_allsnow_c=self.tmax_allsnow_c,
-                tmaxc=self.tmaxc,
-                tminc=self.tminc,
-                transp_on=self.transp_on,
-                tstorm_mo=self.tstorm_mo,
-                verbose=self.verbose,
+            numba_msg = f"{self.name} jit compiling with numba "
+            nb_parallel = (numba_num_threads is not None) and (
+                numba_num_threads > 1
             )
+            if nb_parallel:
+                numba_msg += f"and using {numba_num_threads} threads"
+            print(numba_msg, flush=True)
+
+            self._calculate_snow = nb.njit(
+                fastmath=True, parallel=nb_parallel
+            )(self._calculate_numpy)
+
+            fns = [
+                "_calc_calin",
+                "_calc_caloss",
+                "_calc_ppt_to_pack",
+                "_calc_sca_deplcrv",
+                "_calc_snalbedo",
+                "_calc_snowbal",
+                "_calc_snowcov",
+                "_calc_snowevap",
+                "_calc_step_4",
+            ]
+            for fn in fns:
+                setattr(
+                    self,
+                    fn,
+                    nb.njit(fastmath=True)(getattr(self, fn)),
+                )
 
         else:
-            msg = f"Invalid calc_method={self._calc_method} for {self.name}"
-            raise ValueError(msg)
+            self._calculate_snow = self._calculate_numpy
+
+        return
+
+    def _advance_variables(self) -> None:
+        self.pkwater_ante[:] = self.pkwater_equiv
+        self.freeh2o_prev[:] = self.freeh2o
+        self.pk_ice_prev[:] = self.pk_ice
+        return
+
+    def _calculate(self, simulation_time):
+        (
+            self.ai[:],
+            self.albedo[:],
+            self.frac_swe[:],
+            self.freeh2o[:],
+            self.freeh2o_change[:],
+            self.iasw[:],
+            self.int_alb[:],
+            self.iso[:],
+            self.lso[:],
+            self.lst[:],
+            self.mso[:],
+            self.newsnow[:],
+            self.pk_def[:],
+            self.pk_den[:],
+            self.pk_depth[:],
+            self.pk_ice[:],
+            self.pk_ice_change[:],
+            self.pk_precip[:],
+            self.pk_temp[:],
+            self.pksv[:],
+            self.pkwater_equiv[:],
+            self.pkwater_equiv_change[:],
+            self.pptmix_nopack[:],
+            self.pss[:],
+            self.pst[:],
+            self.salb[:],
+            self.scrv[:],
+            self.slst[:],
+            self.snow_evap[:],
+            self.snowcov_area[:],
+            self.snowcov_areasv[:],
+            self.snowmelt[:],
+            self.snsv[:],
+            self.tcal[:],
+            self.through_rain[:],
+        ) = self._calculate_snow(
+            acum_init=acum_init,
+            ai=self.ai,
+            albedo=self.albedo,
+            albset_rna=self.albset_rna,
+            albset_rnm=self.albset_rnm,
+            albset_sna=self.albset_sna,
+            albset_snm=self.albset_snm,
+            amlt_init=amlt_init,
+            calc_calin=self._calc_calin,
+            calc_caloss=self._calc_caloss,
+            calc_ppt_to_pack=self._calc_ppt_to_pack,
+            calc_sca_deplcrv=self._calc_sca_deplcrv,
+            calc_snalbedo=self._calc_snalbedo,
+            calc_snowbal=self._calc_snowbal,
+            calc_snowcov=self._calc_snowcov,
+            calc_snowevap=self._calc_snowevap,
+            calc_step_4=self._calc_step_4,
+            cecn_coef=self.cecn_coef,
+            cov_type=self.cov_type,
+            covden_sum=self.covden_sum,
+            covden_win=self.covden_win,
+            current_dowy=self.control.current_dowy,
+            current_doy=self.control.current_doy,
+            current_month=self.control.current_month,
+            den_max=self.den_max,
+            deninv=self.deninv,
+            denmaxinv=self.denmaxinv,
+            emis_noppt=self.emis_noppt,
+            frac_swe=self.frac_swe,
+            freeh2o=self.freeh2o,
+            freeh2o_cap=self.freeh2o_cap,
+            freeh2o_change=self.freeh2o_change,
+            freeh2o_prev=self.freeh2o_prev,
+            hru_deplcrv=self.hru_deplcrv,
+            hru_intcpevap=self.hru_intcpevap,
+            hru_ppt=self.hru_ppt,
+            hru_type=self.hru_type,
+            iasw=self.iasw,
+            int_alb=self.int_alb,
+            iso=self.iso,
+            itime_step=self.control.itime_step,
+            lso=self.lso,
+            lst=self.lst,
+            melt_force=self.melt_force,
+            melt_look=self.melt_look,
+            mso=self.mso,
+            net_ppt=self.net_ppt,
+            net_rain=self.net_rain,
+            net_snow=self.net_snow,
+            newsnow=self.newsnow,
+            nhru=self.nhru,
+            orad_hru=self.orad_hru,
+            pk_def=self.pk_def,
+            pk_den=self.pk_den,
+            pk_depth=self.pk_depth,
+            pk_ice=self.pk_ice,
+            pk_ice_change=self.pk_ice_change,
+            pk_ice_prev=self.pk_ice_prev,
+            pk_precip=self.pk_precip,
+            pk_temp=self.pk_temp,
+            pksv=self.pksv,
+            pkwater_ante=self.pkwater_ante,
+            pkwater_equiv=self.pkwater_equiv,
+            pkwater_equiv_change=self.pkwater_equiv_change,
+            potet=self.potet,
+            potet_sublim=self.potet_sublim,
+            pptmix=self.pptmix,
+            pptmix_nopack=self.pptmix_nopack,
+            prmx=self.prmx,
+            pss=self.pss,
+            pst=self.pst,
+            rad_trncf=self.rad_trncf,
+            salb=self.salb,
+            scrv=self.scrv,
+            settle_const=self.settle_const,
+            simulation_time=simulation_time,
+            slst=self.slst,
+            snarea_curve_2d=self.snarea_curve_2d,
+            snarea_thresh=self.snarea_thresh,
+            snow_evap=self.snow_evap,
+            snowcov_area=self.snowcov_area,
+            snowcov_areasv=self.snowcov_areasv,
+            snowmelt=self.snowmelt,
+            snsv=self.snsv,
+            soltab_horad_potsw=self.soltab_horad_potsw,
+            swrad=self.swrad,
+            tavgc=self.tavgc,
+            tcal=self.tcal,
+            through_rain=self.through_rain,
+            tmax_allsnow_c=self.tmax_allsnow_c,
+            tmaxc=self.tmaxc,
+            tminc=self.tminc,
+            transp_on=self.transp_on,
+            tstorm_mo=self.tstorm_mo,
+            verbose=self._verbose,
+        )
 
         return
 
     @staticmethod
     def _calculate_numpy(
         acum_init,
         ai,
@@ -815,15 +687,15 @@
         Args:
             simulation_time: current simulation time
 
         Returns:
             None
         """
 
-        canopy_covden = covden_win
+        canopy_covden = covden_win.copy()
         wh_transp_on = np.where(transp_on)
         canopy_covden[wh_transp_on] = covden_sum[wh_transp_on]
 
         # cals = zero  # JLM this is unnecessary.
 
         # newsnow
         newsnow[:] = False
```

### Comparing `pywatershed-0.1.2/pywatershed/hydrology/PRMSSoilzone.py` & `pywatershed-0.2.0/pywatershed/hydrology/prms_soilzone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,91 +1,109 @@
+from typing import Literal
+from warnings import warn
+
 import numpy as np
 from numba import prange
 
-from pywatershed.base.storageUnit import StorageUnit
-
 from ..base.adapter import adaptable
+from ..base.conservative_process import ConservativeProcess
 from ..base.control import Control
 from ..constants import (
     ETType,
     HruType,
     SoilType,
     epsilon,
     nan,
     numba_num_threads,
     one,
     zero,
 )
+from ..parameters import Parameters
 
 ONETHIRD = 1 / 3
 TWOTHIRDS = 2 / 3
 
 
-class PRMSSoilzone(StorageUnit):
+class PRMSSoilzone(ConservativeProcess):
     """PRMS soil zone.
 
     Args:
+        control: a Control object
+        discretization: a discretization of class Parameters
+        parameters: a parameter object of class Parameters
+        dprst_evap_hru: Evaporation from surface-depression storage for each
+            HRU
+        dprst_seep_hru: Seepage from surface-depression storage to associated
+            GWR for each HRU
+        hru_impervevap: HRU area-weighted average evaporation from impervious
+            area for each HRU
+        hru_intcpevap: HRU area-weighted average evaporation from the
+            canopy for each HRU
+        infil_hru: Infiltration to the capillary and preferential-flow
+            reservoirs, depth on HRU area
+        sroff: Surface runoff to the stream network for each HRU
+        potet: Potential ET for each HRU
+        transp_on: Flag indicating whether transpiration is occurring
+            (0=no;1=yes)
+        snow_evap: Evaporation and sublimation from snowpack on each HRU
+        snowcov_area: Snow-covered area on each HRU prior to melt and
+            sublimation unless snowpack
+        budget_type: one of [None, "warn", "error"]
+        calc_method: one of ["fortran", "numba", "numpy"]. None defaults to
+            "numba".
+        verbose: Print extra information or not?
     """
 
     def __init__(
         self,
         control: Control,
+        discretization: Parameters,
+        parameters: Parameters,
         dprst_evap_hru: adaptable,
         dprst_seep_hru: adaptable,
         hru_impervevap: adaptable,
         hru_intcpevap: adaptable,
         infil_hru: adaptable,  # file by /pywatershed/analysis/budget_soilzone.py
         sroff: adaptable,
         potet: adaptable,
         transp_on: adaptable,
         snow_evap: adaptable,
         snowcov_area: adaptable,
-        budget_type: str = None,
-        calc_method: str = None,
-        verbose: bool = False,
-        load_n_time_batches: int = 1,
+        budget_type: Literal[None, "warn", "error"] = None,
+        calc_method: Literal["numba", "numpy"] = None,
+        verbose: bool = None,
     ) -> "PRMSSoilzone":
         super().__init__(
             control=control,
-            verbose=verbose,
-            load_n_time_batches=load_n_time_batches,
+            discretization=discretization,
+            parameters=parameters,
         )
         self.name = "PRMSSoilzone"
 
-        self._calc_method = str(calc_method)
-
         self._set_inputs(locals())
-        self._set_budget(budget_type)
+        self._set_options(locals())
+
+        self._set_budget()
+        self._init_calc_method()
 
         return
 
     @staticmethod
     def get_dimensions() -> tuple:
-        """Get soil zone dimensions
-
-        Returns:
-            dimensions: input dimensions
-
-        """
-        return ("nhru", "nssr")
+        return ("nhru",)
 
     @staticmethod
     def get_parameters() -> tuple:
-        """Get soil zone parameters
-
-        Returns:
-            parameters: input parameters
-
-        """
         return (
             "dprst_frac",
             "cov_type",
             "fastcoef_lin",
             "fastcoef_sq",
             "hru_area",
+            "hru_in_to_cf",
             "hru_percent_imperv",
             "hru_type",
             "pref_flow_den",
             "sat_threshold",
             "slowcoef_lin",
             "slowcoef_sq",
             "soil_moist_max",
@@ -97,20 +115,14 @@
             "ssr2gw_exp",
             "ssr2gw_rate",
             "ssstor_init_frac",
         )
 
     @staticmethod
     def get_inputs() -> tuple:
-        """Get soil zone input variables
-
-        Returns:
-            variables: input variables
-
-        """
         return (
             "dprst_evap_hru",  # JLM ?? needs this stuff to calculate evap?
             "dprst_seep_hru",
             "hru_impervevap",  # JLM ??
             "hru_intcpevap",  # JLM ???
             "infil_hru",
             "sroff",
@@ -119,30 +131,18 @@
             "transp_on",
             "snow_evap",
             "snowcov_area",
         )
 
     @staticmethod
     def get_restart_variables() -> tuple:
-        """Get soil zone restart variables
-
-        Returns:
-            variables: restart variables
-        """
-
         return ()
 
     @staticmethod
     def get_init_values() -> dict:
-        """Get soil zone inital values
-
-        Returns:
-            dict: inital values for named variables
-        """
-
         return {
             "cap_infil_tot": zero,
             "cap_waterin": zero,
             "dunnian_flow": zero,
             "hru_actet": zero,
             "perv_actet": zero,
             "perv_actet_hru": zero,
@@ -164,15 +164,15 @@
             "soil_lower": nan,  # completely set later
             "soil_lower_change": nan,
             "soil_lower_change_hru": nan,
             "soil_lower_prev": nan,
             "soil_lower_ratio": zero,
             "soil_lower_max": nan,  # completely set later
             "soil_moist": nan,  # sm_climateflow
-            "soil_moist_prev": nan,  # sm_climateflow
+            "soil_moist_prev": zero,  # sm_climateflow
             "soil_moist_tot": nan,  # completely set later
             "soil_rechr": nan,  # sm_climateflow
             "soil_rechr_change": nan,  # sm_climateflow
             "soil_rechr_change_hru": nan,  # sm_climateflow
             "soil_rechr_prev": nan,  # sm_climateflow
             "soil_to_gw": zero,
             "soil_to_ssr": zero,
@@ -204,16 +204,14 @@
                 "soil_lower_change_hru",
                 "slow_stor_change",
                 # "pref_flow_stor_change",
             ],
         }
 
     def _set_initial_conditions(self):
-        """Initialize PRMSSoilzone variables."""
-
         # Derived parameters
         # JLM: is this awkward here?
         # JLM: it's definitely awkward to edit a parameter. maybe
         #      changes/checks on params should throw errors so
         #      parameter values remain the responsibility of the users
         #      and their deficiencies are transparent?
         self.hru_area_imperv = self.hru_percent_imperv * self.hru_area
@@ -239,21 +237,23 @@
 
         self._snow_free = one - self.snowcov_area
         # edit a param
         wh_inactive_or_lake = np.where(
             (self.hru_type == HruType.INACTIVE.value)
             | (self.hru_type == HruType.LAKE.value)
         )
-        self.sat_threshold[wh_inactive_or_lake] = zero
+        self._sat_threshold = self.sat_threshold.copy()
+        self._sat_threshold[wh_inactive_or_lake] = zero
         # edit a param
         wh_not_land = np.where(self.hru_type != HruType.LAND.value)
-        self.pref_flow_den[wh_not_land] = zero
+        self._pref_flow_den = self.pref_flow_den.copy()
+        self._pref_flow_den[wh_not_land] = zero
 
         # variables
-        if self.control.config["init_vars_from_file"] in [0, 2, 5]:
+        if self.control.options["init_vars_from_file"] in [0, 2, 5]:
             # these are set in sm_climateflow
             self.soil_moist[:] = (
                 self.soil_moist_init_frac * self.soil_moist_max
             )
             self.soil_rechr[:] = (
                 self.soil_rechr_init_frac * self.soil_rechr_max
             )
@@ -265,16 +265,16 @@
             raise RuntimeError("Soilzone restart capability not implemented")
 
         # Note that the following is often editing a copy of the parameters,
         # which is a bit odd in that it might be contrary to the users
         # expectations. Move this parameter business to __init__
 
         # ssres_stor
-        if self.control.config["init_vars_from_file"] in [0, 2, 5]:
-            self.ssres_stor = self.ssstor_init_frac * self.sat_threshold
+        if self.control.options["init_vars_from_file"] in [0, 2, 5]:
+            self.ssres_stor = self.ssstor_init_frac * self._sat_threshold
             wh_inactive_or_lake = np.where(
                 (self.hru_type == HruType.INACTIVE.value)
                 | (self.hru_type == HruType.LAKE.value)
             )
             self.ssres_stor[wh_inactive_or_lake] = zero
             del self.ssstor_init_frac
 
@@ -308,43 +308,44 @@
             self.soil_moist_max,
             self.soil_moist,
         )
         self.soil_rechr = np.where(
             self.soil_rechr > self.soil_moist, self.soil_moist, self.soil_rechr
         )
         self.ssres_stor = np.where(
-            self.ssres_stor > self.sat_threshold,
-            self.sat_threshold,
+            self.ssres_stor > self._sat_threshold,
+            self._sat_threshold,
             self.ssres_stor,
         )
 
         # <
         # need to set on swale_limit self? move to variables?
         self._swale_limit = np.full(self.nhru, zero, "float64")
         wh_swale = np.where(self.hru_type == HruType.SWALE.value)
-        self._swale_limit[wh_swale] = 3.0 * self.sat_threshold[wh_swale]
+        self._swale_limit[wh_swale] = 3.0 * self._sat_threshold[wh_swale]
 
-        self.pref_flow_thrsh[wh_swale] = self.sat_threshold[wh_swale]
+        self.pref_flow_thrsh[wh_swale] = self._sat_threshold[wh_swale]
         wh_land = np.where(self.hru_type == HruType.LAND.value)
-        self.pref_flow_thrsh[wh_land] = self.sat_threshold[wh_land] * (
-            one - self.pref_flow_den[wh_land]
+        self.pref_flow_thrsh[wh_land] = self._sat_threshold[wh_land] * (
+            one - self._pref_flow_den[wh_land]
         )
         self.pref_flow_max[wh_land] = (
-            self.sat_threshold[wh_land] - self.pref_flow_thrsh[wh_land]
+            self._sat_threshold[wh_land] - self.pref_flow_thrsh[wh_land]
         )
 
         # Need to set pref_flow_flag on self? or add to variables?
         wh_land_and_prf_den = np.where(
-            (self.hru_type == HruType.LAND.value) & (self.pref_flow_den > zero)
+            (self.hru_type == HruType.LAND.value)
+            & (self._pref_flow_den > zero)
         )
         self._pref_flow_flag = np.full(self.nhru, False, dtype=int)
         self._pref_flow_flag[wh_land_and_prf_den] = True
 
         # can this one be combined with the restart read logic above?
-        if self.control.config["init_vars_from_file"] in [0, 2, 5]:
+        if self.control.options["init_vars_from_file"] in [0, 2, 5]:
             wh_land_or_swale = np.where(
                 (self.hru_type == HruType.LAND.value)
                 | (self.hru_type == HruType.SWALE.value)
             )
             # JLM: to verify this
             self.slow_stor[wh_land_or_swale] = np.minimum(
                 self.ssres_stor[wh_land_or_swale],
@@ -364,15 +365,15 @@
         # <
         # need to set soil2gw_flag on self? move to variables?
         self._soil2gw_flag = np.full(self.nhru, False, dtype=bool)
         wh_soil2gwmax = np.where(self.soil2gw_max > zero)
         self._soil2gw_flag[wh_soil2gwmax] = True
 
         self.soil_zone_max = (
-            self.sat_threshold + self.soil_moist_max * self.hru_frac_perv
+            self._sat_threshold + self.soil_moist_max * self.hru_frac_perv
         )
         self.soil_moist_tot = (
             self.ssres_stor + self.soil_moist * self.hru_frac_perv
         )
 
         self.soil_lower = self.soil_moist - self.soil_rechr
         self.soil_lower_max = self.soil_moist_max - self.soil_rechr_max
@@ -381,293 +382,183 @@
         self.soil_lower_ratio[wh_soil_lower_stor] = (
             self.soil_lower[wh_soil_lower_stor]
             / self.soil_lower_max[wh_soil_lower_stor]
         )
 
         return
 
-    def _advance_variables(self) -> None:
-        self.pref_flow_stor_prev[:] = self.pref_flow_stor
-        self.soil_rechr_prev[:] = self.soil_rechr
-        self.soil_lower_prev[:] = self.soil_lower
-        self.slow_stor_prev[:] = self.slow_stor
-        return
+    def _init_calc_method(self):
+        if self._calc_method is None:
+            self._calc_method = "numba"
+
+        if self._calc_method.lower() not in ["numpy", "numba"]:
+            msg = (
+                f"Invalid calc_method={self._calc_method} for {self.name}. "
+                f"Setting calc_method to 'numba' for {self.name}"
+            )
+            warn(msg)
+            self._calc_method = "numba"
 
-    def _calculate(self, simulation_time):
         if self._calc_method.lower() == "numba":
             import numba as nb
 
-            if not hasattr(self, "_calculate_numba"):
-                numba_msg = f"{self.name} using numba "
-                nb_parallel = (numba_num_threads is not None) and (
-                    numba_num_threads > 1
-                )
-                if nb_parallel:
-                    numba_msg += f"with {numba_num_threads} threads"
-                print(numba_msg, flush=True)
-
-                self._calculate_numba = nb.njit(
-                    fastmath=True, parallel=nb_parallel
-                )(self._calculate_numpy)
-                self._compute_gwflow_numba = nb.njit(fastmath=True)(
-                    self._compute_gwflow
-                )
-                self._compute_interflow_numba = nb.njit(fastmath=True)(
-                    self._compute_interflow
-                )
-                self._compute_soilmoist_numba = nb.njit(fastmath=True)(
-                    self._compute_soilmoist
-                )
-                self._compute_szactet_numba = nb.njit(fastmath=True)(
-                    self._compute_szactet
-                )
-
-            # <
-            (
-                self.soil_to_gw[:],
-                self.soil_to_ssr[:],
-                self.ssr_to_gw[:],
-                self.slow_flow[:],
-                self.ssres_flow[:],
-                self.potet_rechr[:],
-                self.potet_lower[:],
-                self.cap_waterin[:],
-                self.soil_moist[:],
-                self.soil_rechr[:],
-                self.soil_moist_prev[:],
-                self.hru_actet[:],
-                self.cap_infil_tot[:],
-                self.slow_stor[:],
-                self.pref_flow_in[:],
-                self.pref_flow_stor[:],
-                self.perv_actet[:],
-                self.soil_lower[:],
-                self.dunnian_flow[:],
-                self.perv_actet_hru[:],
-                self.pref_flow[:],
-                self.pref_flow_stor_change[:],
-                self.recharge[:],
-                self.slow_stor_change[:],
-                self.soil_lower_change[:],
-                self.soil_lower_change_hru[:],
-                self.soil_lower_ratio[:],
-                self.soil_moist_tot[:],
-                self.soil_rechr_change[:],
-                self.soil_rechr_change_hru[:],
-                self.sroff[:],
-                self.ssres_flow_vol[:],
-                self.ssres_in[:],
-                self.ssres_stor[:],
-                self.swale_actet[:],
-                self.unused_potet[:],
-            ) = self._calculate_numba(
-                _pref_flow_flag=self._pref_flow_flag,
-                _snow_free=self._snow_free,
-                _soil2gw_flag=self._soil2gw_flag,
-                cap_infil_tot=self.cap_infil_tot,
-                cap_waterin=self.cap_waterin,
-                cov_type=self.cov_type,
-                current_time=self.control.current_time,
-                dprst_evap_hru=self.dprst_evap_hru,
-                dprst_flag=self.control.config["dprst_flag"],
-                dprst_seep_hru=self.dprst_seep_hru,
-                dunnian_flow=self.dunnian_flow,
-                fastcoef_lin=self.fastcoef_lin,
-                fastcoef_sq=self.fastcoef_sq,
-                hru_actet=self.hru_actet,
-                hru_frac_perv=self.hru_frac_perv,
-                hru_impervevap=self.hru_impervevap,
-                hru_in_to_cf=self.control.params.hru_in_to_cf,
-                hru_intcpevap=self.hru_intcpevap,
-                hru_type=self.hru_type,
-                infil_hru=self.infil_hru,
-                nhru=self.nhru,
-                perv_actet=self.perv_actet,
-                perv_actet_hru=self.perv_actet_hru,
-                potet=self.potet,
-                potet_lower=self.potet_lower,
-                potet_rechr=self.potet_rechr,
-                pref_flow=self.pref_flow,
-                pref_flow_in=self.pref_flow_in,
-                pref_flow_infil=self.pref_flow_infil,
-                pref_flow_max=self.pref_flow_max,
-                pref_flow_stor=self.pref_flow_stor,
-                pref_flow_stor_change=self.pref_flow_stor_change,
-                pref_flow_stor_prev=self.pref_flow_stor_prev,
-                pref_flow_thrsh=self.pref_flow_thrsh,
-                recharge=self.recharge,
-                sat_threshold=self.sat_threshold,
-                slow_flow=self.slow_flow,
-                slow_stor=self.slow_stor,
-                slow_stor_change=self.slow_stor_change,
-                slow_stor_prev=self.slow_stor_prev,
-                slowcoef_lin=self.slowcoef_lin,
-                slowcoef_sq=self.slowcoef_sq,
-                snow_evap=self.snow_evap,
-                snowcov_area=self.snowcov_area,
-                soil2gw_max=self.soil2gw_max,
-                soil_lower=self.soil_lower,
-                soil_lower_change=self.soil_lower_change,
-                soil_lower_change_hru=self.soil_lower_change_hru,
-                soil_lower_max=self.soil_lower_max,
-                soil_lower_prev=self.soil_lower_prev,
-                soil_lower_ratio=self.soil_lower_ratio,
-                soil_moist=self.soil_moist,
-                soil_moist_max=self.soil_moist_max,
-                soil_moist_prev=self.soil_moist_prev,
-                soil_moist_tot=self.soil_moist_tot,
-                soil_rechr=self.soil_rechr,
-                soil_rechr_change=self.soil_rechr_change,
-                soil_rechr_change_hru=self.soil_rechr_change_hru,
-                soil_rechr_max=self.soil_rechr_max,
-                soil_rechr_prev=self.soil_rechr_prev,
-                soil_to_gw=self.soil_to_gw,
-                soil_to_ssr=self.soil_to_ssr,
-                soil_type=self.soil_type,
-                sroff=self.sroff,
-                ssr2gw_exp=self.ssr2gw_exp,
-                ssr2gw_rate=self.ssr2gw_rate,
-                ssr_to_gw=self.ssr_to_gw,
-                ssres_flow=self.ssres_flow,
-                ssres_flow_vol=self.ssres_flow_vol,
-                ssres_in=self.ssres_in,
-                ssres_stor=self.ssres_stor,
-                swale_actet=self.swale_actet,
-                transp_on=self.transp_on,
-                unused_potet=self.unused_potet,
-                compute_gwflow=self._compute_gwflow_numba,
-                compute_interflow=self._compute_interflow_numba,
-                compute_soilmoist=self._compute_soilmoist_numba,
-                compute_szactet=self._compute_szactet_numba,
+            numba_msg = f"{self.name} jit compiling with numba "
+            nb_parallel = (numba_num_threads is not None) and (
+                numba_num_threads > 1
             )
-
-        elif self._calc_method.lower() in ["none", "numpy"]:
-            (
-                self.soil_to_gw[:],
-                self.soil_to_ssr[:],
-                self.ssr_to_gw[:],
-                self.slow_flow[:],
-                self.ssres_flow[:],
-                self.potet_rechr[:],
-                self.potet_lower[:],
-                self.cap_waterin[:],
-                self.soil_moist[:],
-                self.soil_rechr[:],
-                self.soil_moist_prev[:],
-                self.hru_actet[:],
-                self.cap_infil_tot[:],
-                self.slow_stor[:],
-                self.pref_flow_in[:],
-                self.pref_flow_stor[:],
-                self.perv_actet[:],
-                self.soil_lower[:],
-                self.dunnian_flow[:],
-                self.perv_actet_hru[:],
-                self.pref_flow[:],
-                self.pref_flow_stor_change[:],
-                self.recharge[:],
-                self.slow_stor_change[:],
-                self.soil_lower_change[:],
-                self.soil_lower_change_hru[:],
-                self.soil_lower_ratio[:],
-                self.soil_moist_tot[:],
-                self.soil_rechr_change[:],
-                self.soil_rechr_change_hru[:],
-                self.sroff[:],
-                self.ssres_flow_vol[:],
-                self.ssres_in[:],
-                self.ssres_stor[:],
-                self.swale_actet[:],
-                self.unused_potet[:],
-            ) = self._calculate_numpy(
-                _pref_flow_flag=self._pref_flow_flag,
-                _snow_free=self._snow_free,
-                _soil2gw_flag=self._soil2gw_flag,
-                cap_infil_tot=self.cap_infil_tot,
-                cap_waterin=self.cap_waterin,
-                compute_gwflow=self._compute_gwflow,
-                compute_interflow=self._compute_interflow,
-                compute_soilmoist=self._compute_soilmoist,
-                compute_szactet=self._compute_szactet,
-                cov_type=self.cov_type,
-                current_time=self.control.current_time,
-                dprst_evap_hru=self.dprst_evap_hru,
-                dprst_flag=self.control.config["dprst_flag"],
-                dprst_seep_hru=self.dprst_seep_hru,
-                dunnian_flow=self.dunnian_flow,
-                fastcoef_lin=self.fastcoef_lin,
-                fastcoef_sq=self.fastcoef_sq,
-                hru_actet=self.hru_actet,
-                hru_frac_perv=self.hru_frac_perv,
-                hru_impervevap=self.hru_impervevap,
-                hru_in_to_cf=self.control.params.hru_in_to_cf,
-                hru_intcpevap=self.hru_intcpevap,
-                hru_type=self.hru_type,
-                infil_hru=self.infil_hru,
-                nhru=self.nhru,
-                perv_actet=self.perv_actet,
-                perv_actet_hru=self.perv_actet_hru,
-                potet=self.potet,
-                potet_lower=self.potet_lower,
-                potet_rechr=self.potet_rechr,
-                pref_flow=self.pref_flow,
-                pref_flow_in=self.pref_flow_in,
-                pref_flow_infil=self.pref_flow_infil,
-                pref_flow_max=self.pref_flow_max,
-                pref_flow_stor=self.pref_flow_stor,
-                pref_flow_stor_change=self.pref_flow_stor_change,
-                pref_flow_stor_prev=self.pref_flow_stor_prev,
-                pref_flow_thrsh=self.pref_flow_thrsh,
-                recharge=self.recharge,
-                sat_threshold=self.sat_threshold,
-                slow_flow=self.slow_flow,
-                slow_stor=self.slow_stor,
-                slow_stor_change=self.slow_stor_change,
-                slow_stor_prev=self.slow_stor_prev,
-                slowcoef_lin=self.slowcoef_lin,
-                slowcoef_sq=self.slowcoef_sq,
-                snow_evap=self.snow_evap,
-                snowcov_area=self.snowcov_area,
-                soil2gw_max=self.soil2gw_max,
-                soil_lower=self.soil_lower,
-                soil_lower_change=self.soil_lower_change,
-                soil_lower_change_hru=self.soil_lower_change_hru,
-                soil_lower_max=self.soil_lower_max,
-                soil_lower_prev=self.soil_lower_prev,
-                soil_lower_ratio=self.soil_lower_ratio,
-                soil_moist=self.soil_moist,
-                soil_moist_max=self.soil_moist_max,
-                soil_moist_prev=self.soil_moist_prev,
-                soil_moist_tot=self.soil_moist_tot,
-                soil_rechr=self.soil_rechr,
-                soil_rechr_change=self.soil_rechr_change,
-                soil_rechr_change_hru=self.soil_rechr_change_hru,
-                soil_rechr_max=self.soil_rechr_max,
-                soil_rechr_prev=self.soil_rechr_prev,
-                soil_to_gw=self.soil_to_gw,
-                soil_to_ssr=self.soil_to_ssr,
-                soil_type=self.soil_type,
-                sroff=self.sroff,
-                ssr2gw_exp=self.ssr2gw_exp,
-                ssr2gw_rate=self.ssr2gw_rate,
-                ssr_to_gw=self.ssr_to_gw,
-                ssres_flow=self.ssres_flow,
-                ssres_flow_vol=self.ssres_flow_vol,
-                ssres_in=self.ssres_in,
-                ssres_stor=self.ssres_stor,
-                swale_actet=self.swale_actet,
-                transp_on=self.transp_on,
-                unused_potet=self.unused_potet,
+            if nb_parallel:
+                numba_msg += f"and using {numba_num_threads} threads"
+            print(numba_msg, flush=True)
+
+            self._calculate_soilzone = nb.njit(
+                fastmath=True, parallel=nb_parallel
+            )(self._calculate_numpy)
+
+            self._compute_gwflow = nb.njit(fastmath=True)(self._compute_gwflow)
+            self._compute_interflow = nb.njit(fastmath=True)(
+                self._compute_interflow
+            )
+            self._compute_soilmoist = nb.njit(fastmath=True)(
+                self._compute_soilmoist
+            )
+            self._compute_szactet = nb.njit(fastmath=True)(
+                self._compute_szactet
             )
 
         else:
-            msg = f"Invalid calc_method={self._calc_method} for {self.name}"
-            raise ValueError(msg)
+            self._calculate_soilzone = self._calculate_numpy
+
+        return
+
+    def _advance_variables(self) -> None:
+        self.pref_flow_stor_prev[:] = self.pref_flow_stor
+        self.soil_rechr_prev[:] = self.soil_rechr
+        self.soil_lower_prev[:] = self.soil_lower
+        self.slow_stor_prev[:] = self.slow_stor
+        return
+
+    def _calculate(self, simulation_time):
+        (
+            self.soil_to_gw[:],
+            self.soil_to_ssr[:],
+            self.ssr_to_gw[:],
+            self.slow_flow[:],
+            self.ssres_flow[:],
+            self.potet_rechr[:],
+            self.potet_lower[:],
+            self.cap_waterin[:],
+            self.soil_moist[:],
+            self.soil_rechr[:],
+            self.soil_moist_prev[:],
+            self.hru_actet[:],
+            self.cap_infil_tot[:],
+            self.slow_stor[:],
+            self.pref_flow_in[:],
+            self.pref_flow_stor[:],
+            self.perv_actet[:],
+            self.soil_lower[:],
+            self.dunnian_flow[:],
+            self.perv_actet_hru[:],
+            self.pref_flow[:],
+            self.pref_flow_stor_change[:],
+            self.recharge[:],
+            self.slow_stor_change[:],
+            self.soil_lower_change[:],
+            self.soil_lower_change_hru[:],
+            self.soil_lower_ratio[:],
+            self.soil_moist_tot[:],
+            self.soil_rechr_change[:],
+            self.soil_rechr_change_hru[:],
+            self.sroff[:],
+            self.ssres_flow_vol[:],
+            self.ssres_in[:],
+            self.ssres_stor[:],
+            self.swale_actet[:],
+            self.unused_potet[:],
+        ) = self._calculate_soilzone(
+            _pref_flow_flag=self._pref_flow_flag,
+            _snow_free=self._snow_free,
+            _soil2gw_flag=self._soil2gw_flag,
+            cap_infil_tot=self.cap_infil_tot,
+            cap_waterin=self.cap_waterin,
+            compute_gwflow=self._compute_gwflow,
+            compute_interflow=self._compute_interflow,
+            compute_soilmoist=self._compute_soilmoist,
+            compute_szactet=self._compute_szactet,
+            cov_type=self.cov_type,
+            current_time=self.control.current_time,
+            dprst_evap_hru=self.dprst_evap_hru,
+            dprst_flag=self.control.options["dprst_flag"],
+            dprst_seep_hru=self.dprst_seep_hru,
+            dunnian_flow=self.dunnian_flow,
+            fastcoef_lin=self.fastcoef_lin,
+            fastcoef_sq=self.fastcoef_sq,
+            hru_actet=self.hru_actet,
+            hru_frac_perv=self.hru_frac_perv,
+            hru_impervevap=self.hru_impervevap,
+            hru_in_to_cf=self.hru_in_to_cf,
+            hru_intcpevap=self.hru_intcpevap,
+            hru_type=self.hru_type,
+            infil_hru=self.infil_hru,
+            nhru=self.nhru,
+            perv_actet=self.perv_actet,
+            perv_actet_hru=self.perv_actet_hru,
+            potet=self.potet,
+            potet_lower=self.potet_lower,
+            potet_rechr=self.potet_rechr,
+            pref_flow=self.pref_flow,
+            pref_flow_in=self.pref_flow_in,
+            pref_flow_infil=self.pref_flow_infil,
+            pref_flow_max=self.pref_flow_max,
+            pref_flow_stor=self.pref_flow_stor,
+            pref_flow_stor_change=self.pref_flow_stor_change,
+            pref_flow_stor_prev=self.pref_flow_stor_prev,
+            pref_flow_thrsh=self.pref_flow_thrsh,
+            recharge=self.recharge,
+            sat_threshold=self._sat_threshold,
+            slow_flow=self.slow_flow,
+            slow_stor=self.slow_stor,
+            slow_stor_change=self.slow_stor_change,
+            slow_stor_prev=self.slow_stor_prev,
+            slowcoef_lin=self.slowcoef_lin,
+            slowcoef_sq=self.slowcoef_sq,
+            snow_evap=self.snow_evap,
+            snowcov_area=self.snowcov_area,
+            soil2gw_max=self.soil2gw_max,
+            soil_lower=self.soil_lower,
+            soil_lower_change=self.soil_lower_change,
+            soil_lower_change_hru=self.soil_lower_change_hru,
+            soil_lower_max=self.soil_lower_max,
+            soil_lower_prev=self.soil_lower_prev,
+            soil_lower_ratio=self.soil_lower_ratio,
+            soil_moist=self.soil_moist,
+            soil_moist_max=self.soil_moist_max,
+            soil_moist_prev=self.soil_moist_prev,
+            soil_moist_tot=self.soil_moist_tot,
+            soil_rechr=self.soil_rechr,
+            soil_rechr_change=self.soil_rechr_change,
+            soil_rechr_change_hru=self.soil_rechr_change_hru,
+            soil_rechr_max=self.soil_rechr_max,
+            soil_rechr_prev=self.soil_rechr_prev,
+            soil_to_gw=self.soil_to_gw,
+            soil_to_ssr=self.soil_to_ssr,
+            soil_type=self.soil_type,
+            sroff=self.sroff,
+            ssr2gw_exp=self.ssr2gw_exp,
+            ssr2gw_rate=self.ssr2gw_rate,
+            ssr_to_gw=self.ssr_to_gw,
+            ssres_flow=self.ssres_flow,
+            ssres_flow_vol=self.ssres_flow_vol,
+            ssres_in=self.ssres_in,
+            ssres_stor=self.ssres_stor,
+            swale_actet=self.swale_actet,
+            transp_on=self.transp_on,
+            unused_potet=self.unused_potet,
+        )
 
-        # <
         return
 
     @staticmethod
     def _calculate_numpy(
         _pref_flow_flag,
         _snow_free,
         _soil2gw_flag,
@@ -774,15 +665,15 @@
         soil_moist_prev[:] = soil_moist
 
         # JLM: ET calculations to be removed from soilzone.
         hru_actet = hru_impervevap + hru_intcpevap + snow_evap
 
         # This is obnoxious. i guess this should be an
         # optional input? should default to zero?
-        if dprst_flag == 1:
+        if dprst_flag:
             hru_actet = hru_actet + dprst_evap_hru
 
         # <
         for hh in prange(nhru):
             dunnianflw = zero
             dunnianflw_pfr = zero
             dunnianflw_gvr = zero
@@ -932,29 +823,35 @@
 
                 # JLM: the order of the PRMSIV theory is not maintained here
                 # This skips over 8 to step 9
 
                 # PRMSIV Step 9
                 # Compute slow contribution to interflow, if any
                 if slow_stor[hh] > epsilon:
-                    (slow_stor[hh], slow_flow[hh],) = compute_interflow(
+                    (
+                        slow_stor[hh],
+                        slow_flow[hh],
+                    ) = compute_interflow(
                         slowcoef_lin[hh],
                         slowcoef_sq[hh],
                         ssresin,
                         slow_stor[hh],
                         slow_flow[hh],
                     )
 
                 # <
             elif hru_type[hh] == HruType.SWALE.value:
                 slow_stor[hh] = availh2o
 
             # <
             if (slow_stor[hh] > epsilon) and (ssr2gw_rate[hh] > zero):
-                (ssr_to_gw[hh], slow_stor[hh],) = compute_gwflow(
+                (
+                    ssr_to_gw[hh],
+                    slow_stor[hh],
+                ) = compute_gwflow(
                     ssr2gw_rate[hh],
                     ssr2gw_exp[hh],
                     slow_stor[hh],
                 )
 
             # <
             # JLM: right about here the code gets difficult to follow
@@ -1075,15 +972,15 @@
         )
         # if current_time == np.datetime64("1979-03-18T00:00:00"):
         # asdf
 
         soil_moist_tot = ssres_stor + soil_moist * hru_frac_perv
         recharge = soil_to_gw + ssr_to_gw
 
-        if dprst_flag == 1:
+        if dprst_flag:
             recharge = recharge + dprst_seep_hru
 
         pref_flow_stor_change[:] = pref_flow_stor - pref_flow_stor_prev
         soil_lower_change[:] = soil_lower - soil_lower_prev
         soil_rechr_change[:] = soil_rechr - soil_rechr_prev
         slow_stor_change[:] = slow_stor - slow_stor_prev
         # Apparently the following are sums of the above and not actual
```

### Comparing `pywatershed-0.1.2/pywatershed/hydrology/Starfit.py` & `pywatershed-0.2.0/pywatershed/hydrology/starfit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from typing import Literal
+
 import numpy as np
 
-from pywatershed.base.storageUnit import StorageUnit
+from pywatershed.base.conservative_process import ConservativeProcess
 
 from ..base.adapter import adaptable
 from ..base.control import Control
 from ..constants import nan, one, zero
+from ..parameters import Parameters
 
 
-class Starfit(StorageUnit):
+class Starfit(ConservativeProcess):
     """starfit: Storage Targets And Release Function Inference Tool
 
     Sean W.D. Turner, Jennie Clarice Steyaert, Laura Condon, Nathalie Voisin,
     Water storage and release policies for all large reservoirs of conterminous
     United States, Journal of Hydrology, Volume 603, Part A, 2021, 126843,
     ISSN 0022-1694, https://doi.org/10.1016/j.jhydrol.2021.126843.
 
@@ -19,50 +22,53 @@
 
     Adapted from STARFIT implementation in the MOSART-WM model:
     https://github.com/IMMM-SFA/mosartwmpy/blob/main/mosartwmpy/reservoirs/istarf.py
 
     Noah Knowles (USGS) and James McCreight (UCAR/USGS)
 
     Args:
+        control: a Control object
+        discretization: a discretization of class Parameters
+        parameters: a parameter object of class Parameters
+        lake_inflow: Daily lake inflow
+        budget_type: one of [None, "warn", "error"]
+        verbose: Print extra information or not?
+        load_n_time_batches: not-implemented
+
     """
 
     def __init__(
         self,
         control: Control,
+        discretization: Parameters,
+        parameters: Parameters,
         lake_inflow: adaptable,
-        budget_type: str = None,
-        calc_method: str = None,
+        budget_type: Literal[None, "warn", "error"] = None,
         verbose: bool = False,
         load_n_time_batches: int = 1,
-    ) -> "Starfit":
+    ) -> None:
         super().__init__(
             control=control,
-            verbose=verbose,
-            load_n_time_batches=load_n_time_batches,
+            discretization=discretization,
+            parameters=parameters,
         )
         self.name = "Starfit"
 
-        self._calc_method = str(calc_method)
-
         self._set_inputs(locals())
+        self._set_options(locals())
+
         self._set_budget(budget_type)
         return
 
     @staticmethod
     def get_dimensions() -> dict:
         return ("nreservoirs",)
 
     @staticmethod
     def get_parameters() -> tuple:
-        """Get starfit parameters
-
-        Returns:
-            parameters: input parameters
-
-        """
         return (
             "grand_id",
             "initial_storage",
             "start_time",
             "end_time",
             "inflow_mean",
             "NORhi_min",
@@ -86,20 +92,14 @@
             "Release_c",
             "GRanD_CAP_MCM",
             "Obs_MEANFLOW_CUMECS",
         )
 
     @staticmethod
     def get_inputs() -> tuple:
-        """Get starfit input variables
-
-        Returns:
-            variables: input variables
-
-        """
         return ("lake_inflow",)
 
     @staticmethod
     def get_mass_budget_terms():
         return {
             "inputs": [
                 "lake_inflow",
@@ -111,19 +111,14 @@
             "storage_changes": [
                 "lake_storage_change",
             ],
         }
 
     @staticmethod
     def get_init_values() -> dict:
-        """Get starfit initial values
-
-        Returns:
-            dict: initial values for named variables
-        """
         return {
             "lake_storage": nan,
             "lake_storage_old": nan,
             "lake_storage_change": nan,
             "lake_inflow": nan,
             "lake_release": nan,
             "lake_spill": nan,
```

### Comparing `pywatershed-0.1.2/pywatershed/parameters/prms_parameters.py` & `pywatershed-0.2.0/pywatershed/parameters/prms_parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
+from copy import deepcopy
 
-import netCDF4 as nc4
 import numpy as np
 
 from ..base import meta
 from ..base.parameters import Parameters
-from ..constants import fileish, ft2_per_acre, inches_per_foot, listish, ndoy
+from ..constants import fileish, ft2_per_acre, inches_per_foot, ndoy
 from ..utils.prms5_file_util import PrmsFile
 
 prms_dim_names = (
     "nhru",
     "nsegment",
     "nssr",
     "ngw",
@@ -48,42 +48,40 @@
     return pars
 
 
 class PrmsParameters(Parameters):
     """
     PRMS parameter class
 
-    Parameters
-    ----------
-    parameter_dict : dict
-        parameters dictionary: either structure
-          * param: value
-          * process: {param: value ... }
-        where the later is a parameter dictionary grouped by process.
-        The keys for process should be either the class itself, class.name, or
-        type(class.__name__).
-    parameter_dimensions_dict : dict
-        parameters dimensions dictionary with a structure mirring the parameter
-        dict as described above but with shape tuples in place of parameter
-        value data.
-
-    Returns:
-        PrmsParameter object
+    Args:
+        parameter_dict : dict
+            parameters dictionary: either structure
+
+            * param: value
+            * process: {param: value ... }
+
+            where the later is a parameter dictionary grouped by process.
+            The keys for process should be either the class itself, class.name,
+            or type(class.__name__).
+        parameter_dimensions_dict : dict
+            parameters dimensions dictionary with a structure mirring the
+            parameter dict as described above but with shape tuples in place
+            of parameter value data.
 
     """
 
     def __init__(
         self,
         dims: dict = None,
         coords: dict = None,
         data_vars: dict = None,
         metadata: dict = None,
         encoding: dict = None,
         validate: bool = True,
-    ) -> "PrmsParameters":
+    ) -> None:
         if dims is None:
             dims = {}
         if coords is None:
             coords = {}
         if data_vars is None:
             data_vars = {}
         if metadata is None:
@@ -98,127 +96,57 @@
             metadata=metadata,
             encoding=encoding,
             validate=validate,
         )
 
         return
 
-    def get_parameters(self, keys: listish, dims: bool = False) -> dict:
-        """Get a subset of keys in the parameter dictionary
-
-        Args:
-            keys: keys to retrieve from the full PRMS parameter object
-            process: return a single process (all keys)
-            dims: return dims instead of values (default is False)
-
-        Returns:
-            dict: containing requested key:val pairs
-
-        """
-        if isinstance(keys, str):
-            keys = [keys]
-
-        if dims:
-            return {
-                key: self.parameter_dimensions.get(key)
-                for key in keys
-                if key in self.parameter_dimensions.keys()
-            }
-        else:
-            return {
-                key: self.parameters.get(key)
-                for key in keys
-                if key in self.parameters.keys()
-            }
-
     @property
     def dimensions(self) -> dict:
         """Get the dimensions from the parameters
 
         Returns:
             dimensions in the PRMS parameter dictionary
 
         """
         dimensions = {}
         for key, value in self.dims.items():
             if isinstance(value, int):
                 dimensions[key] = value
         return dimensions
 
-    @property
-    def nhm_hru_coordinate(self) -> np.ndarray:
-        """Get the nhm hru coordinate
-
-        Returns:
-            id: nhm coordinate for each hru
-
-        """
-        if "nhru" not in self.dims.keys():
-            return None
-
-        if "nhm_id" in self.parameters.keys():
-            nhm_id = self.parameters["nhm_id"]
-        else:
-            nhm_id = np.arange(1, self.dims["nhru"] + 1)
-        return nhm_id
-
-    @property
-    def nhm_segment_coordinate(self) -> np.ndarray:
-        """Get the nhm segment coordinate
-
-        Returns:
-            id: nhm coordinate for each segment
-
-        """
-        if "nsegment" not in self.dims.keys():
-            return None
-
-        if "nhm_seg" in self.parameters.keys():
-            nhm_seg = self.parameters["nhm_seg"]
-        else:
-            nhm_seg = np.arange(1, self.dims["nsegment"] + 1)
-        return nhm_seg
-
-    @property
-    def nhm_coordinates(self) -> dict:
-        """Get the nhm coordinates
-
-        Returns:
-            id: nhm coordinates
-
-        """
-        return {
-            "nhm_id": self.nhm_hru_coordinate,
-            "nhm_seg": self.nhm_segment_coordinate,
-        }
-
     def parameters_to_json(self, json_filename):
         """write the parameters dictionary out to a json file"""
         json.dump(
             {**self.dims, **self.parameters},
             open(json_filename, "w"),
             indent=4,
             cls=JSONParameterEncoder,
         )
 
         return
 
     @staticmethod
+    def _from_dict(param_dict: dict) -> "PrmsParameters":
+        """Load parameters from a dictionary of just parameters"""
+        return PrmsParameters._after_load(param_dict)
+
+    @staticmethod
     def load_from_json(json_filename: fileish) -> "PrmsParameters":
         """Load parameters from a json file
 
         Args:
             : json file path
 
         Returns:
             PrmsParameters: full PRMS parameter dictionary
 
         """
         pars = _json_load(json_filename)
-        params = PrmsParameters._after_load(pars)
+        params = PrmsParameters._process_file_input(pars)
 
         return params
 
     @staticmethod
     def load(parameter_file: fileish) -> "PrmsParameters":
         """Load parameters from a PRMS parameter file
 
@@ -226,22 +154,31 @@
             parameter_file: parameter file path
 
         Returns:
             PrmsParameters: full PRMS parameter dictionary
 
         """
         data = PrmsFile(parameter_file, "parameter").get_data()
-        params = PrmsParameters._after_load(
+        params = PrmsParameters._process_file_input(
             data["parameter"]["parameters"],
             # data["parameter"]["parameter_dimensions"],
         )
 
         return params
 
-    def _after_load(
+    def to_netcdf(self, filename, use_xr=False) -> None:
+        """Write PrmsParameters to a netcdf file"""
+        self.data_vars
+        if use_xr:
+            self.to_xr_ds().to_netcdf(filename)
+        else:
+            self.to_nc4_ds(filename)
+        return
+
+    def _process_file_input(
         parameter_dict: dict,
         parameter_dimensions_dict: dict = None,
     ) -> "PrmsParameters":
         # move dims from params to dims
         if parameter_dimensions_dict is None:
             parameter_dimensions_dict = {}
 
@@ -258,23 +195,14 @@
 
         # build dimension metadata from data
         if len(parameter_dimensions_dict) == 0:
             for key, value in parameter_dict.items():
                 param_dim_names = meta.get_params(key)[key]["dims"]
                 parameter_dimensions_dict[key] = {"dims": param_dim_names}
 
-                # need below?
-                # this was original code before above
-                # if len(param_dim_names):
-                #     param_dim_names = list(
-                #         param_dimensions_dict[key]["dims"].values()
-                #     )
-                # else:
-                #     param_dim_names = [key]
-
                 common_params = set(param_dim_names) & set(dims)
                 if not len(common_params):
                     parameter_dimensions_dict[key] = {
                         "dims": tuple(["unknown"])
                     }
                     continue
 
@@ -297,19 +225,27 @@
                             found_dim = True
                             temp_dims.append("scalar")
 
                 parameter_dimensions_dict[key] = {"dims": tuple(temp_dims)}
 
         # build coords, only some dims have coords that are not indexes
         coords = {}
-        for cc in ["nhm_id", "nhm_seg", "poi_gage_id"]:
+        # edge case of dims that have only index or implied coords
+        # this is justified, as this data should probably be in the parameter
+        # files. netcdf neccisitates this to even carry the dimension data.
+        # alternative would be to have a scalar, but in fact this is a
+        # dimension of the data.
+        coords["doy"] = np.arange(dims["ndoy"], dtype="int32") + 1
+
+        for cc in ["nhm_id", "nhm_seg", "poi_gage_id", "doy"]:
             coord_to_dim = {
                 "nhm_id": "nhru",
                 "nhm_seg": "nsegment",
                 "poi_gage_id": "npoigages",
+                "doy": "ndoy",
             }
             dim_name = coord_to_dim[cc]
             if dim_name not in dims:
                 continue
 
             dim_val = dims[dim_name]
 
@@ -317,58 +253,31 @@
                 coords[cc] = parameter_dict.pop(cc)
             else:
                 coord_to_dim = {"nhm_id": "nhru", "nhm_seg": "nsegment"}
                 coords[cc] = np.arange(1, dim_val + 1)
 
             parameter_dimensions_dict[cc] = {"dims": (dim_name,)}
 
-        parameter_dimensions_dict["global"] = {}
+        # Derived parameter converting inches to cubic feet on hrus.
+        parameter_dict["hru_in_to_cf"] = (
+            parameter_dict["hru_area"] * ft2_per_acre / (inches_per_foot)
+        )
+        parameter_dimensions_dict["hru_in_to_cf"] = {"dims": ("nhru",)}
+
+        for key, value in parameter_dimensions_dict.items():
+            key_meta = deepcopy(meta.get_params(key)[key])
+            _ = key_meta.pop("dims")
+            parameter_dimensions_dict[key]["attrs"] = key_meta
+
+        parameter_dimensions_dict["global"] = {
+            "Description": "Parameter data for PRMS"
+        }
 
         prms_params = PrmsParameters(
             dims=dims,
             coords=coords,
             data_vars=parameter_dict,
             metadata=parameter_dimensions_dict,
             validate=True,
         )
-        return prms_params
-
-    @staticmethod
-    def from_nc_files(
-        proc_param_nc_file_dict: dict,
-        use_xr: bool = False,
-        merge: bool = False,
-    ) -> "PrmsParameters":
-        # TODO: this method could be in the super: DatasetDict?
-        """Load parameters from a PRMS parameter file
-
-        Args:
-            proc_param_nc_file_dict: dict of proc: param_nc_file pairs
-            for all processes in the model
-
-        Returns:
-            param_dict: A dictionary containing PRMSParameters objects for
-            each process.
-
-        """
-        params = {
-            proc: PrmsParameters.from_netcdf(file)
-            for proc, file in proc_param_nc_file_dict.items()
-        }
-        if merge:
-            params = PrmsParameters.merge(list(prams.values()))
-
-        return params
 
-    def hru_in_to_cfs(self, time_step: np.timedelta64) -> np.ndarray:
-        "Derived parameter converting inches to cfs on hrus."
-        time_step_seconds = time_step / np.timedelta64(1, "s")
-        return self.hru_in_to_cf / time_step_seconds
-
-    @property
-    def hru_in_to_cf(self) -> np.ndarray:
-        "Derived parameter converting inches to cubic feet on hrus."
-        return (
-            self.get_parameters("hru_area")["hru_area"]
-            * ft2_per_acre
-            / (inches_per_foot)
-        )
+        return prms_params
```

### Comparing `pywatershed-0.1.2/pywatershed/parameters/starfit_parameters.py` & `pywatershed-0.2.0/pywatershed/parameters/starfit_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+from ..base.data_model import DatasetDict
 from ..base.parameters import Parameters
 from ..constants import fileish
 
 
 class StarfitParameters(Parameters):
     """
     Starfit parameter class
@@ -62,16 +63,16 @@
     def from_netcdf(
         resops_domain: fileish,
         istarf_conus: fileish,
         grand_dams: fileish,
         grand_ids: fileish = None,
         param_names: list = None,
     ) -> dict:
-        resops_dd = Parameters.from_netcdf(resops_domain)
-        istarf_conus_dd = Parameters.from_netcdf(istarf_conus)
+        resops_dd = DatasetDict.from_netcdf(resops_domain)
+        istarf_conus_dd = DatasetDict.from_netcdf(istarf_conus)
         istarf_rename = {"GRanD_ID": "grand_id"}
         istarf_conus_dd.rename_dim(istarf_rename)
         istarf_conus_dd.rename_var(istarf_rename)
         wh_subset = np.where(
             np.isin(
                 istarf_conus_dd.coords["grand_id"],
                 resops_dd.coords["grand_id"],
@@ -80,15 +81,15 @@
         istarf_conus_dd.subset_on_coord("grand_id", wh_subset)
         # these attributes make merging fail
         # relax merging with a dict of nested keys?, or jst on encoding/meta?
         del istarf_conus_dd.encoding["grand_id"]["source"]
         del istarf_conus_dd.encoding["grand_id"]["original_shape"]
         # params_dd = DatasetDict.merge(istarf_conus_dd, resops_dd)
 
-        grand_dams_dd = Parameters.from_netcdf(grand_dams)
+        grand_dams_dd = DatasetDict.from_netcdf(grand_dams)
         grand_rename = {"GRAND_ID": "grand_id"}
         grand_dams_dd.rename_dim(grand_rename)
         grand_dams_dd.rename_var(grand_rename)
         wh_subset = np.where(
             np.isin(
                 grand_dams_dd.coords["grand_id"],
                 resops_dd.coords["grand_id"],
@@ -99,13 +100,15 @@
         # relax merging with a dict of nested keys?, or jst on encoding/meta?
         del grand_dams_dd.encoding["grand_id"]["source"]
         del grand_dams_dd.encoding["grand_id"]["original_shape"]
 
         istarf_conus_dd.drop_var("subset_inds")
         grand_dams_dd.drop_var("subset_inds")
 
-        params_dd = Parameters.merge(resops_dd, istarf_conus_dd, grand_dams_dd)
+        params_dd = DatasetDict.merge(
+            resops_dd, istarf_conus_dd, grand_dams_dd
+        )
         # probably should have named the spatial dim nreservoirs when
         # I created the netcdf file
         _ = params_dd.rename_dim({"grand_id": "nreservoirs"})
 
         return StarfitParameters.from_dict(params_dd.data)
```

### Comparing `pywatershed-0.1.2/pywatershed/static/metadata/control.yaml` & `pywatershed-0.2.0/pywatershed/static/metadata/control.yaml`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/static/metadata/dimensions.yaml` & `pywatershed-0.2.0/pywatershed/static/metadata/dimensions.yaml`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/static/metadata/parameters.yaml` & `pywatershed-0.2.0/pywatershed/static/metadata/parameters.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -402,14 +402,20 @@
   maximum: 1.0E9
   minimum: 0.0
   modules:
   - precip_dist2
   - temp_dist2
   type: F
   units: feet
+doy:
+  desc: Day of year (1-366)
+  dims:
+    0: ndoy
+  type: I
+  units: day index  # using 'days' will trigger an undesired xarray encoding
 dprst_depth_avg:
   default: 132.0
   desc: Average depth of surface depressions at maximum storage capacity
   dims:
     0: nhru
   help: Average depth of surface depressions at maximum storage capacity
   maximum: 500.0
@@ -775,53 +781,53 @@
   - cascade
   type: I
   units: none
 gwflow_coef:
   default: 0.015
   desc: Groundwater routing coefficient
   dims:
-    0: ngw
+    0: nhru
   help: Linear coefficient in the equation to compute groundwater discharge for each
     GWR
   maximum: 0.5
   minimum: 0.0
   modules:
   - gwflow
   type: F
   units: fraction/day
 gwsink_coef:
   default: 0.0
   desc: Groundwater sink coefficient
   dims:
-    0: ngw
+    0: nhru
   help: Linear coefficient in the equation to compute outflow to the groundwater sink
     for each GWR
   maximum: 1.0
   minimum: 0.0
   modules:
   - gwflow
   type: F
   units: fraction/day
 gwstor_init:
   default: 2.0
   desc: Initial storage in each GWR
   dims:
-    0: ngw
+    0: nhru
   help: Storage in each GWR at the beginning of a simulation
   maximum: 50.0
   minimum: 0.0
   modules:
   - gwflow
   type: F
   units: inches
 gwstor_min:
   default: 0.0
   desc: Minimum storage in each GWR
   dims:
-    0: ngw
+    0: nhru
   help: Minimum storage in each GWR to ensure storage is greater than specified value
     to account for inflow from deep aquifers or injection wells with the water source
     outside the basin
   maximum: 1.0
   minimum: 0.0
   modules:
   - gwflow
@@ -910,14 +916,24 @@
   help: Index of humidity measurement station for each HRU
   maximum: nhumid
   minimum: bounded
   modules:
   - potet_pm_sta
   type: I
   units: none
+hru_in_to_cf:
+  default: None
+  desc: Conversion of inches of depth to cubic feet for each HRU
+  dims:
+    0: nhru
+  help: Conversion of inches of depth to cubic feet for each HRU
+  maximum: Large
+  minimum: zero
+  type: F
+  units: cubic feet
 hru_lat:
   default: 40.0
   desc: HRU latitude
   dims:
     0: nhru
   help: Latitude of each HRU
   maximum: 90.0
@@ -2458,19 +2474,20 @@
   type: F
   units: inches
 seg_cum_area:
   default: NaN
   desc: Segment cumulative area
   dims:
     0: nsegment
-  help: Ssegment cumulative area
+  help: Segment cumulative area
   maximum: NaN
   minimum: 0.00
   model: PRMS
   modules:
+    - none
   type: F
   units: unknown
 seg_depth:
   default: 1.0
   desc: Depth of bankfull water in segment
   dims:
     0: nsegment
@@ -2991,42 +3008,42 @@
   - stream_temp
   type: I
   units: days
 ssr2gw_exp:
   default: 1.0
   desc: Coefficient to route water from subsurface to groundwater
   dims:
-    0: nssr
+    0: nhru
   help: Non-linear coefficient in equation used to route water from the gravity reservoir
     to the GWR for each HRU
   maximum: 3.0
   minimum: 0.0
   modules:
   - soilzone
   type: F
   units: none
 ssr2gw_rate:
   default: 0.1
   desc: Coefficient to route water from gravity reservoir to GWR
   dims:
-    0: nssr
+    0: nhru
   help: Linear coefficient in equation used to route water from the gravity reservoir
     to the GWR for each HRU
   maximum: 1.0
   minimum: 0.0001
   modules:
   - soilzone
   type: F
   units: fraction/day
 ssstor_init_frac:
   default: 0.0
   desc: Initial fraction of available water in the gravity plus preferential-flow
     reservoirs
   dims:
-    0: nssr
+    0: nhru
   help: Initial fraction of available water in the gravity plus preferential-flow
     reservoirs (fraction of sat_threshold) for each HRU
   maximum: 1.0
   minimum: 0.0
   modules:
   - soilzone
   - convert_params
```

### Comparing `pywatershed-0.1.2/pywatershed/static/metadata/variables.yaml` & `pywatershed-0.2.0/pywatershed/static/metadata/variables.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1005,14 +1005,35 @@
   units: inches
 cascade_interflow:
   desc: Cascading interflow for each HRU
   dims:
     0: nhru
   type: float64
   units: inches
+channel_sroff_vol:
+  desc: Runoff volume entering the stream channel from each HRU
+  dims:
+    0: nhru
+  type: float64
+  units: cubicfeet
+  var_category: mass flux
+channel_ssres_flow_vol:
+  desc: Subsurface reservoir discharge volume entering the stream channel from each HRU
+  dims:
+    0: nhru
+  type: float64
+  units: cubicfeet
+  var_category: mass flux
+channel_gwres_flow_vol:
+  desc: Groundwater reservoir discharge volume entering the stream channel from each HRU
+  dims:
+    0: nhru
+  type: float64
+  units: cubicfeet
+  var_category: mass flux
 channel_outflow_vol:
   desc: Streamflow volume leaving the stream channel model
   dims:
     0: nsegment
   type: float64
   units: cubicfeet
   var_category: mass flux
@@ -1371,33 +1392,33 @@
   dims:
     0: nhrucell
   type: float64
   units: inches
 gw_in_soil:
   desc: Drainage from capillary reservoir excess water for each GWR
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: acre-inches
 gw_in_ssr:
   desc: Drainage from gravity reservoir excess water for each GWR
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: acre-inches
 gw_seep_lakein:
   desc: Groundwater discharge to any associated lake for each GWR
   dims:
     0: nlake
   type: float64
   units: acre-feet
 gw_upslope:
   desc: Groundwater flow received from upslope GWRs for each GWR
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: acre-inches
 gwr_gain:
   desc: Transfer gain to the groundwater reservoir of each HRU for each time step
   dims:
     0: nhru
   type: float64
@@ -1420,58 +1441,58 @@
   dims:
     0: nhru
   type: float64
   units: cfs
 gwres_flow:
   desc: Groundwater discharge from each GWR to the stream network
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: inches
   var_category: mass flux
 gwres_flow_vol:
   desc: Groundwater discharge volume from each GWR to the stream network
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: cubicfeet
   var_category: mass flux
 gwres_sink:
   desc: Outflow from GWRs to the groundwater sink; water is considered underflow or
     flow to deep aquifers and does not flow to the stream network
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: inches
   var_category: mass flux
 gwres_stor:
   desc: Storage in each GWR
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: inches
   var_category: mass storage
 gwres_stor_change:
   desc: Change is storage in each GWR
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: inches
   var_category: mass storage change
 gwres_stor_old:
   desc: Previous storage in each GWR
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: inches
   var_category: mass storage
 gwstor_minarea_wb:
   desc: Storage added to each GWR when storage is less than gwstor_min
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: inches
 hortonian_flow:
   desc: Hortonian surface runoff reaching stream network for each HRU
   dims:
     0: nhru
   type: float64
@@ -1499,15 +1520,15 @@
   dims:
     0: nhru
   type: float64
   units: decimal fraction
 hru_gw_cascadeflow:
   desc: Cascading groundwater flow from each GWR
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: inches
 hru_hortn_cascflow:
   desc: Cascading Hortonian surface runoff leaving each HRU
   dims:
     0: nhru
   type: float64
@@ -1873,15 +1894,15 @@
   dims:
     0: nlake
   type: float64
   units: acre-feet
 lake_seepage_gwr:
   desc: Net lake-bed seepage to associated GWRs
   dims:
-    0: ngw
+    0: nhru
   type: float64
   units: inches
 lake_spill:
   desc: Spill from each lake
   dims:
     0: nreservoirs
   type: float64
@@ -2806,42 +2827,42 @@
     0: nhru
   type: float64
   units: cubicfeet
   var_category: mass flux
 ssr_to_gw:
   desc: Drainage from the gravity-reservoir to the associated GWR for each HRU
   dims:
-    0: nssr
+    0: nhru
   type: float64
   units: inches
   var_category: mass flux
 ssres_flow:
   desc: Interflow from gravity and preferential-flow reservoirs to the stream network
     for each HRU
   dims:
-    0: nssr
+    0: nhru
   type: float64
   units: inches
 ssres_flow_vol:
   desc: Interflow volume from gravity and preferential-flow reservoirs to the stream network
     for each HRU
   dims:
-    0: nssr
+    0: nhru
   type: float64
   units: cubicfeet
 ssres_in:
   desc: Inflow to the gravity and preferential-flow reservoirs for each HRU
   dims:
-    0: nssr
+    0: nhru
   type: float64
   units: inches
 ssres_stor:
   desc: Storage in the gravity and preferential-flow reservoirs for each HRU
   dims:
-    0: nssr
+    0: nhru
   type: float64
   units: inches
 streamflow_cfs:
   desc: Streamflow at each measurement station
   dims:
     0: nobs
   type: float64
```

### Comparing `pywatershed-0.1.2/pywatershed/static/metadata/xml_to_yaml.py` & `pywatershed-0.2.0/pywatershed/static/metadata/xml_to_yaml.py`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/utils/cbh_utils.py` & `pywatershed-0.2.0/pywatershed/utils/cbh_utils.py`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/utils/control.py` & `pywatershed-0.2.0/pywatershed/utils/control.py`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/utils/csv_utils.py` & `pywatershed-0.2.0/pywatershed/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/utils/dis_hru.py` & `pywatershed-0.2.0/pywatershed/utils/dis_hru.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 import numpy as np
 
 from ..constants import fileish
 from .mf6_file_writer import mf6_file_writer
 from .parameters import PrmsParameters
 
-# try:
-#     import geopandas as gpd
-
-#     has_geopandas = True
-# except ModuleNotFoundError:
-#     has_geopandas = False
-
-
 acres_to_m2 = 4046.8564224
 
 required = [
     "nodes",
     "nja",
     "top",
     "bot",
@@ -113,15 +105,14 @@
         param_file: fileish = None,
         params: PrmsParameters = None,
         hru_shapefile: fileish = None,
         length_units: str = "meters",
         disu_file: fileish = None,
         **kwargs,
     ):
-
         # read the parameter file: currently just for HRU areas
         self._param_file = param_file
         self.params = params
         if (param_file is not None) and (params is not None):
             msg = "Can only specify one of param_file or params"
             raise ValueError(msg)
         elif (param_file is None) and (params is None):
```

### Comparing `pywatershed-0.1.2/pywatershed/utils/netcdf_utils.py` & `pywatershed-0.2.0/pywatershed/utils/netcdf_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
         var_meta: dict,
         global_attrs: dict = {},
         time_units: str = "days since 1970-01-01 00:00:00",
         clobber: bool = True,
         zlib: bool = True,
         complevel: int = 4,
         chunk_sizes: dict = {"time": 30, "hruid": 0},
-    ) -> "NetCdfWrite":
+    ):
         if isinstance(variables, dict):
             group_variables = []
             for group, vars in variables.items():
                 for var_name in vars:
                     if group is None:
                         group_variables += [var_name]
                     else:
```

### Comparing `pywatershed-0.1.2/pywatershed/utils/prms5_file_util.py` & `pywatershed-0.2.0/pywatershed/utils/prms5_file_util.py`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/utils/prms5util.py` & `pywatershed-0.2.0/pywatershed/utils/prms5util.py`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed/utils/prms_to_mf6.py` & `pywatershed-0.2.0/pywatershed/utils/prms_to_mf6.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import pint
 import xarray as xr
 
 from pywatershed import Control, meta
 
 from ..constants import SegmentType, fileish, zero
-from .parameters import PrmsParameters
+from ..parameters import PrmsParameters
 
 # try:
 #     import geopandas as gpd
 
 #     has_geopandas = True
 # except ModuleNotFoundError:
 #     has_geopandas = False
@@ -203,15 +203,15 @@
         # ]
 
         # nvert turns off requirement of vertices and cell2d
         nvert = None  # len(vertices)
         vertices = None
         cell2d = None
 
-        nsegment = parameters["nsegment"]
+        nsegment = self.params.dims["nsegment"]
         hru_segment = parameters["hru_segment"] - 1
         tosegment = parameters["tosegment"] - 1
 
         # united quantities
 
         segment_units = self.units(meta.parameters["seg_length"]["units"])
         segment_length = parameters["seg_length"]
@@ -275,28 +275,29 @@
         # meta.get_units could be defined
         vel_units = {
             key: self.units(val)
             for key, val in meta.get_units(
                 ["mann_n", "seg_slope", "seg_depth"], to_pint=True
             ).items()
         }
+        vel_terms = {}
         for var in vel_units:
-            parameters[var] *= vel_units[var]
+            vel_terms[var] = parameters[var] * vel_units[var]
 
         velocity = (
-            (1.0 / parameters["mann_n"])
-            * np.sqrt(parameters["seg_slope"])
-            * parameters["seg_depth"] ** (2.0 / 3.0)
+            (1.0 / vel_terms["mann_n"])
+            * np.sqrt(vel_terms["seg_slope"])
+            * vel_terms["seg_depth"] ** (2.0 / 3.0)
             * (3600.0 * self.units("seconds/hour"))
         )
 
         # JLM: This is a bad idea and should throw an error rather than edit
         # inputs in place during run
         # Shouldnt this ALSO BE ABOVE the velocity calculation?
-        parameters["seg_slope"] = np.where(
+        seg_slope = np.where(
             parameters["seg_slope"] < 1e-7, 0.0001, parameters["seg_slope"]
         )  # this is from prms5.2.1, it is not in prms6
 
         # Kcoef
         # initialize Kcoef to 24.0 for segments with zero velocities
         # this is different from PRMS, which relied on divide by zero resulting
         # in a value of infinity that when evaluated relative to a maximum
@@ -387,15 +388,15 @@
             inflows[flow_name] /= timestep_s.to("seconds")
 
             new_inflow_unit = inflows[flow_name].units
 
             # calculate lateral flow term to the REACH/segment from HRUs
             lat_inflow = np.zeros((self.nper, nsegment)) * new_inflow_unit
 
-            for ihru in range(parameters["nhru"]):
+            for ihru in range(self.params.dims["nhru"]):
                 iseg = hru_segment[ihru]
                 if iseg < 0:
                     # This is bad, selective handling of fluxes is not cool,
                     # mass is being discarded in a way that has to be
                     # coordinated
                     # with other parts of the code.
                     # This code shuold be removed evenutally.
```

### Comparing `pywatershed-0.1.2/pywatershed/utils/time_utils.py` & `pywatershed-0.2.0/pywatershed/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pywatershed-0.1.2/pywatershed.egg-info/PKG-INFO` & `pywatershed-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,232 +1,171 @@
-Metadata-Version: 2.1
-Name: pywatershed
-Version: 0.1.2
-Summary: pywatershed is a Python package for hydrologic modeling
-Author-email: USGS Enterprise Capacity Team <modflow@usgs.gov>
-Maintainer-email: "James L. McCreight" <jmccreight@usgs.gov>, "Joseph D. Hughes" <jdhughes@usgs.gov>
-License: CC0
-Project-URL: Documentation, https://pywatershed.readthedocs.io
-Project-URL: Bug Tracker, https://github.com/EC-USGS/pywatershed/issues
-Project-URL: Source Code, https://github.com/EC-USGS/pywatershed
-Keywords: hydrology,PRMS
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: lint
-Provides-Extra: test
-License-File: LICENSE
-
 # pywatershed
-[![ci-badge](https://github.com/ec-usgs/pywatershed/workflows/CI/badge.svg?branch=main)](https://github.com/ec-usgs/pywatershed/actions?query=workflow%3ACI)
+
+[![ci-badge](https://github.com/ec-usgs/pywatershed/workflows/CI/badge.svg?branch=develop)](https://github.com/ec-usgs/pywatershed/actions?query=workflow%3ACI)
 [![codecov-badge](https://codecov.io/gh/ec-usgs/pywatershed/branch/main/graph/badge.svg)](https://codecov.io/gh/ec-usgs/pywatershed)
 [![Documentation Status](https://readthedocs.org/projects/pywatershed/badge/?version=latest)](https://pywatershed.readthedocs.io/en/latest/?badge=latest)
+[![asv](http://img.shields.io/badge/benchmarked%20by-asv-green.svg?style=flat)](https://github.com/ec-usgs/pywatershed)
+[![Formatted with black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+
+[![Available on pypi](https://img.shields.io/pypi/v/pywatershed.svg)](https://pypi.python.org/pypi/pywatershed)
+[![PyPI Status](https://img.shields.io/pypi/status/pywatershed.svg)](https://pypi.python.org/pypi/pywatershed)
+[![PyPI Versions](https://img.shields.io/pypi/pyversions/pywatershed.svg)](https://pypi.python.org/pypi/pywatershed)
+
+[![WholeTale](https://raw.githubusercontent.com/whole-tale/wt-design-docs/master/badges/wholetale-explore.svg)](https://dashboard.wholetale.org/run/64ae29e8a887f48b9f173678?tab=metadata)
 
-[![PyPI Version](https://img.shields.io/pypi/v/pywatershed.png)](https://pypi.python.org/pypi/pywatershed)
-[![PyPI Status](https://img.shields.io/pypi/status/pywatershed.png)](https://pypi.python.org/pypi/pywatershed)
-[![PyPI Versions](https://img.shields.io/pypi/pyversions/pywatershed.png)](https://pypi.python.org/pypi/pywatershed)
 
-[//]: # (<img src="https://raw.githubusercontent.com/ec-usgs/pywatershed/main/resources/images/prms_flow.png" alt="prms_flow" style="width:50;height:20">)
+<!-- START doctoc generated TOC please keep comment here to allow auto update -->
+<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
+**Table of Contents**
+
+- [Purpose](#purpose)
+- [Installation](#installation)
+- [Contributing](#contributing)
+- [Example Notebooks](#example-notebooks)
+- [Overview of Repository Contents](#overview-of-repository-contents)
+- [Disclaimer](#disclaimer)
+
+<!-- END doctoc generated TOC please keep comment here to allow auto update -->
+
+## Purpose
 
-Purpose
-=========
 The purpose of this repository is to refactor and redesign the [PRMS modeling
 system](https://www.usgs.gov/software/precipitation-runoff-modeling-system-prms)
 while maintaining its functionality. Code modernization is a step towards
 unification with [MODFLOW 6 (MF6)](https://github.com/MODFLOW-USGS/modflow6).
 
-The following motivations are taken from our
-[AGU poster from December 2022](https://agu2022fallmeeting-agu.ipostersessions.com/default.aspx?s=05-E1-C6-40-DF-0D-4D-C7-4E-DE-D2-61-02-05-8F-0A)
+The following motivations are taken from our [AGU poster from December
+2022](https://agu2022fallmeeting-agu.ipostersessions.com/default.aspx?s=05-E1-C6-40-DF-0D-4D-C7-4E-DE-D2-61-02-05-8F-0A)
 which provides additional details on motivations, project status, and current
 directions of this project as of approximately January 2023.
 
-Goals of the USGS Enterprise Capacity (EC) project include:
-  * A sustainable integrated, hydrologic modeling framework for the U.S. Geological Survey (USGS)
-  * Interoperable modeling across the USGS, partner agencies, and academia
-
-Goals for EC Watershed Modeling:
-  * Couple the Precipitation-Runoff Modeling System (PRMS, e.g. Regan et al, 2018)  with MODFLOW 6 (MF6, e.g. Langevin et al, 2017) in a sustainable way
-  * Redesign PRMS to be more modern and flexible
-  * Prioritize process representations in the current National Hydrological Model (NHM) based on PRMS 5.2.1
-
-Prototype an EC watershed model: "pywatershed"
-  * Redesign PRMS quickly in python
-  * Couple to MF6 via BMI/XMI interface (Hughes et al, 2021; Hutton et al, 2020)
-  * Establish a prototyping ground for EC codes that couples to the compiled framework: low cost proof of concepts (at the price of potentially less computational performance)
-  * Enable process representation hypothesis testing
-  * Use cutting-edge techniques and technologies to improve models
-  * Machine learning, automatic differentiation
-  * Address challenges of modeling across space and time scales
-  * Transition prototype watershed model to compiled EC code
-
-
-Installation and Python Environments
-=====================================
-This installation assumes you do not need to run automated tests locally. See
-the following "Developer Installation" section for complete installation
-instructions.
-
-To install the software you will need Python >= 3.8. We recommend installing
-the python package dependencies using anaconda or miniconda. Most users will
-likely want to create the `pyws_nb` conda environment by running
-
-```conda env create -f examples/examples_env.yml```.
-
-One could also do
-
-```pip install -r examples/exampes_env.txt```
-
-but this is not guaranteed.
-
-Once the environment is established, activate the environment and install
-pywatershed
-
-`conda activate pyws_nb; cd pywatershed; pip install .`
-
-If you would like to compile the fortran computational kernels for
-certain physical process representations (not required), you'll need a fortran
-compiler and you will run
-
-`export PYWS_FORTRAN=true; cd pywatershed;  pip install .`
-
-See Developer Requirements below for more details.
-
-
-Developer Installation
-=======================
-Git is required if you plan to contribute code back to the repository.
-
-C and Fortran compilers are required. We are currently using gnu (gcc, gfortran)
-11 and 12 as well as intel (icc, ifort) 2021 on Windows, Linux, and MacOS
-(including Apple Silicon). Both of these are freely obtainable but the installation
-process varies widely. We are looking for a conda-based approach to obtaining
-compilers, but currently do not have a solution. Compilers are needed for
-two applications:
-
-  1. Compiling and running C/Fortran PRMS code to generate testing/verification data
-  2. Compiling (installing) and running fortran backends/kernels for some hydrological
-     process representations in pywatershed
-
-On Apple Silicon, the PRMS source code is only currently known to compile with intel while
-the fortran kernels in pywatershed only compile with gnu.
-
-Python >= 3.8 is required. Three different python environments are specified within the repository.
-These are:
-
-* Minimal (for developing/testing), 'pyws': ci/requirements/environment.yml
-* Notebooks (~= minimal + jupyter), 'pyws_nb': examples/examples_env.yml
-* Documentation (only if you want to build the documentation), 'pyws-docs': ci/requirements/doc.yml
-
-We recommend (because we test it in CI) using anacoda or miniconda to establish these environments
-with the following commands
-
-```conda env create -f path/to/env_of_choice.yml```
-
-which will create the environment with "name" specified on the first line of the file, given before the path
-to the file above.
-
-More detailed python environment installation instructions using conda can be found in
-`examples/00_python_virtual_env.ipynb`.
-
-There are also .txt equivalents that can be used for installing from pip, like so:
-
-```pip install -r env_of_choice.txt```
-
-though these are not comprehensive installs as with conda and not tested.
-
-Once the python environment and dependencies are established and activated (`conda activate env_of_choice`),
-pywatershed is installed for development into that environment with the following command
-
-`cd pywatershed; pip install -e .`
-
-The numpy extension F2PY is used to provide fortran compiled kernels of core calculations to boost
-performance. F2PY is documented [within numpy](https://numpy.org/doc/stable/f2py/index.html). This
-repository is configured NOT to compile on install by default. Currently, we have not established
-this compilation procedure for Windows. On linux and MacOS, compilation of fortran kernels on package
-installation is achieved by the following code:
-
-```
-export SETUPTOOLS_ENABLE_FEATURES="legacy-editable"
-export CC=path/to/gcc  # for example
-export FC=path/to/gfortran  # for example
-export PYWS_FORTRAN=true
-cd path/to/pywatershed
-pip install -e .
-```
-
-Once the dependencies are available, we want to verify the software by running its test suite. The
-following testing procedures are also covered in the notebook `examples/01_automated_testing.ipynb`.
-To run the tests, we first need to generate the test data. This consists of running PRMS
-and then converting the output to netcdf:
-
-```
-cd path/to/pywatershed/test_data/scripts
-pytest -v -n=4 test_run_domains.py
-pytest -v -n=8 test_nc_domains.py
-```
-
-Finally, run the tests themselves,
-
-```
-cd path/to/pywatershed/autotest
-pytest -v -n=8
-```
-
-All tests should pass, XPASS, or XFAIL. XFAIL is an expected failure.
-
-
-Contributing
-============
-We welcome community development! Please file Issues and/or Pull Requests in the appropriate places on github. The continuous
-integration (CI) procedure is the first gate keeper for new code contribution. The CI procedure is defined by
-`.github/workflows/ci.yaml`. This includes running the formatting and linting packages `isort`, `black`, and
-`flake8` in addition to generating the test data and running the tests in `autotest/`. New codes need new tests so they can
-be verified moving ahead in time.
-
-
-Example Notebooks
-==================
-Jupyter notebooks containing examples are found in the
-[examples/](https://github.com/EC-USGS/pywatershed/tree/main/examples) directory. Numbered notebooks are tested.
-Notebooks 00 and 01 walk the user through the setting the python environment and running the software tests.
-Notebook 02 demonstrates modeling with pywatershed. Non-numbered notebooks cover additional topics. These notebooks
-are note yet covered by testing and so may be expected to have some issues until they are added to testing.
-
-
-Overview of Repository Contents
-==========
-The contents of directories at this level is described. Therein you may discover another README.md for more information.
-
-```
-.github/    Github actions for deploying continuous integration (CI)
-autotest/   pywatershed package testing using pytest
-bin/        PRMS executables distributed
-ci/         Python environments for CI
-doc/        Package/code documentation source code
-examples/   How to use the package, mostly jupyter notebooks
-prms_src/   PRMS source used for generating executables in bin/
-pywatershed/      Package source
-reference/  Ancillary materials for development
-resources/  Static stuff like images
-test_data/  Data used for automated testing
-```
-
-
-Disclaimer
-==========
-
-This information is preliminary or provisional and is subject to revision. It is being provided to meet the need for timely best science. The information has not received final approval by the U.S. Geological Survey (USGS) and is provided on the condition that neither the USGS nor the U.S. Government shall be held liable for any damages resulting from the authorized or unauthorized use of the information.
+Goals of the USGS Enterprise Capacity (EC) project include: * A sustainable
+integrated, hydrologic modeling framework for the U.S. Geological Survey (USGS)
+* Interoperable modeling across the USGS, partner agencies, and academia
+
+Goals for EC Watershed Modeling: * Couple the Precipitation-Runoff Modeling
+System (PRMS, e.g. Regan et al, 2018)  with MODFLOW 6 (MF6, e.g. Langevin et al,
+2017) in a sustainable way * Redesign PRMS to be more modern and flexible *
+Prioritize process representations in the current National Hydrological Model
+(NHM) based on PRMS 5.2.1
+
+Prototype an EC watershed model: "pywatershed" * Redesign PRMS quickly in python
+* Couple to MF6 via BMI/XMI interface (Hughes et al, 2021; Hutton et al, 2020) *
+Establish a prototyping ground for EC codes that couples to the compiled
+framework: low cost proof of concepts (at the price of potentially less
+computational performance) * Enable process representation hypothesis testing *
+Use cutting-edge techniques and technologies to improve models * Machine
+learning, automatic differentiation * Address challenges of modeling across
+space and time scales * Transition prototype watershed model to compiled EC code
+
+## Installation
+
+To install the software you will need Python 3.9 or 3.10.
+
+We currently recommend dependencies be installed with
+[Mamba](https://mamba.readthedocs.io/en/latest/) which will be much faster than
+Ananconda (but the conda command can also be used). An environment containing
+all core and optional dependencies can be created from the project root with:
+
+```mamba env create -f environment_w_jupyter.yml```
+
+(The environment `environment.yml` does not contain jupyter or jupyterlab
+in order to not interfere with installation in WholeTale, see Example
+Notebooks seection below.)
+
+The `pywatershed` package is [available on
+PyPI](https://pypi.org/project/pywatershed/). At the moment, the installation
+may not be reliable on all platforms and we are working to fix this.
+
+Using PyPI (with the above caveat), `pywatershed` can be installed with:
+
+``` pip install pywatershed ```
+
+A number of extra dependencies are needed to run the example notebooks. These
+can be installed with pip with
+
+``` pip install "pywatershed[optional]" ```
+
+These installation steps are suitable for `pywatershed` end users. See the
+[developer documentation](./DEVELOPER.md) for detailed instructions on
+configuring a development environment.
+
+## Contributing
+
+See the [developer documentation](./DEVELOPER.md) for instructions on setting up
+a development environment. See the [contribution guide](./CONTRIBUTING.md) to
+contribute to this project.
+
+## Example Notebooks
+
+For introductory example notebooks, look in the
+[`examples/`](https://github.com/EC-USGS/pywatershed/tree/main/examples>)
+directory in the repository. Numbered starting at 00, these are meant to be
+completed in order. Non-numbered notebooks coveradditional topics. These
+notebooks are note yet covered by testing and so may be expected to have some
+issues until they are added to testing. In `examples/developer/` there are
+notebooks of interest to developers who may want to learn about running the
+software tests.
+
+Though no notebook outputs are saved in Github, these notebooks can easily
+navigated to and run in WholeTale containers (free but sign-up or log-in
+required). This is a very easy and quick way to get started without needing to
+install pywatershed requirements yourself. WholeTale is an NSF funded project
+and supports logins from many institutions, e.g. the USGS, and you may not need
+to register.
+
+There are containers for both the `main` and `develop` branches.
+
+[![WholeTale](https://raw.githubusercontent.com/whole-tale/wt-design-docs/master/badges/wholetale-explore.svg)](https://dashboard.wholetale.org)
+* [WholeTale container for latest release (main
+  branch)](https://dashboard.wholetale.org/run/64ae29e8a887f48b9f173678?tab=metadata)
+* [WholeTale container for develop
+  branch](https://dashboard.wholetale.org/run/64ae25c3a887f48b9f1735c8?tab=metadata)
+
+WholeTale will give you a jupyter-lab running in the root of this
+repository. You can navigate to `examples/` and then open and run the notebooks
+of your choice.  The develop container may require the user to update the
+repository (`git pull origin`) to stay current with development.
+
+## Overview of Repository Contents
+
+The contents of directories at this level is described. Therein you may discover
+another README.md for more information.
+
+```
+.github/: Github actions, scripts and Python environments for continuous integration (CI) and releasing,
+asv_benchmarks/: preformance benchmarking by ASV
+autotest/: pywatershed package testing using pytest
+autotest_exs/: pywatershed example notebook testing using pytest
+bin/:PRMS executables distributed
+doc/:Package/code documentation source code
+evaluation/: tools for evaluation of pywatershed
+examples/:How to use the package, mostly jupyter notebooks
+prms_src/:PRMS source used for generating executables in bin/
+pywatershed/:Package source
+reference/:Ancillary materials for development
+resources/:Static stuff like images
+test_data/:Data used for automated testing
+```
+
+## Disclaimer
+
+This information is preliminary or provisional and is subject to revision. It is
+being provided to meet the need for timely best science. The information has not
+received final approval by the U.S. Geological Survey (USGS) and is provided on
+the condition that neither the USGS nor the U.S. Government shall be held liable
+for any damages resulting from the authorized or unauthorized use of the
+information.
 
 From: https://www2.usgs.gov/fsp/fsp_disclaimers.asp#5
 
-This software is in the public domain because it contains materials that originally came from the U.S. Geological Survey, an agency of the United States Department of Interior. For more information, see the [official USGS copyright policy](https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits "official USGS copyright policy")
-
-Although this software program has been used by the USGS, no warranty, expressed or implied, is made by the USGS or the U.S. Government as to the accuracy and functioning of the program and related program material nor shall the fact of distribution constitute any such warranty, and no responsibility is assumed by the USGS in connection therewith.
-This software is provided "AS IS."
+This software is in the public domain because it contains materials that
+originally came from the U.S. Geological Survey, an agency of the United States
+Department of Interior. For more information, see the [official USGS copyright
+policy](https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits
+"official USGS copyright policy")
+
+Although this software program has been used by the USGS, no warranty, expressed
+or implied, is made by the USGS or the U.S. Government as to the accuracy and
+functioning of the program and related program material nor shall the fact of
+distribution constitute any such warranty, and no responsibility is assumed by
+the USGS in connection therewith.  This software is provided "AS IS."
```

### Comparing `pywatershed-0.1.2/pywatershed.egg-info/SOURCES.txt` & `pywatershed-0.2.0/pywatershed.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,51 @@
-.gitignore
-.mf6_ci_ref_remote
-DISCLAIMER.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-readthedocs.yml
 setup.py
-pywatershed/MANIFEST.in
 pywatershed/__init__.py
 pywatershed/constants.py
 pywatershed/version.py
 pywatershed.egg-info/PKG-INFO
 pywatershed.egg-info/SOURCES.txt
 pywatershed.egg-info/dependency_links.txt
 pywatershed.egg-info/not-zip-safe
 pywatershed.egg-info/requires.txt
 pywatershed.egg-info/top_level.txt
 pywatershed/analysis/__init__.py
 pywatershed/analysis/model_graph.py
 pywatershed/analysis/process_plot.py
 pywatershed/analysis/utils/__init__.py
 pywatershed/analysis/utils/colorbrewer.py
-pywatershed/atmosphere/PRMSAtmosphere.py
-pywatershed/atmosphere/PRMSSolarGeometry.py
 pywatershed/atmosphere/__init__.py
+pywatershed/atmosphere/prms_atmosphere.py
+pywatershed/atmosphere/prms_solar_geometry.py
 pywatershed/atmosphere/solar_constants.py
 pywatershed/base/__init__.py
 pywatershed/base/accessor.py
 pywatershed/base/adapter.py
 pywatershed/base/budget.py
+pywatershed/base/conservative_process.py
 pywatershed/base/control.py
 pywatershed/base/data_model.py
 pywatershed/base/meta.py
 pywatershed/base/model.py
 pywatershed/base/parameters.py
-pywatershed/base/storageUnit.py
+pywatershed/base/process.py
 pywatershed/base/timeseries.py
-pywatershed/hydrology/PRMSCanopy.f90
-pywatershed/hydrology/PRMSCanopy.py
-pywatershed/hydrology/PRMSCanopy.pyf
-pywatershed/hydrology/PRMSChannel.f90
-pywatershed/hydrology/PRMSChannel.py
-pywatershed/hydrology/PRMSChannel.pyf
-pywatershed/hydrology/PRMSEt.py
-pywatershed/hydrology/PRMSGroundwater.f90
-pywatershed/hydrology/PRMSGroundwater.py
-pywatershed/hydrology/PRMSGroundwater.pyf
-pywatershed/hydrology/PRMSRunoff.py
-pywatershed/hydrology/PRMSSnow.py
-pywatershed/hydrology/PRMSSoilzone.py
-pywatershed/hydrology/Starfit.py
 pywatershed/hydrology/__init__.py
+pywatershed/hydrology/prms_canopy.py
+pywatershed/hydrology/prms_channel.py
+pywatershed/hydrology/prms_et.py
+pywatershed/hydrology/prms_groundwater.py
+pywatershed/hydrology/prms_runoff.py
+pywatershed/hydrology/prms_snow.py
+pywatershed/hydrology/prms_soilzone.py
+pywatershed/hydrology/starfit.py
 pywatershed/parameters/__init__.py
 pywatershed/parameters/prms_parameters.py
 pywatershed/parameters/starfit_parameters.py
 pywatershed/static/metadata/control.yaml
 pywatershed/static/metadata/dimensions.yaml
 pywatershed/static/metadata/parameters.yaml
 pywatershed/static/metadata/variables.yaml
@@ -63,14 +53,16 @@
 pywatershed/utils/__init__.py
 pywatershed/utils/cbh_utils.py
 pywatershed/utils/control.py
 pywatershed/utils/csv_utils.py
 pywatershed/utils/dis_hru.py
 pywatershed/utils/formatting.py
 pywatershed/utils/netcdf_utils.py
-pywatershed/utils/parameters.py
+pywatershed/utils/optional_import.py
+pywatershed/utils/parse_version.py
+pywatershed/utils/path.py
 pywatershed/utils/prms5_file_util.py
 pywatershed/utils/prms5util.py
 pywatershed/utils/prms_to_mf6.py
 pywatershed/utils/separate_nhm_params.py
 pywatershed/utils/time_utils.py
 pywatershed/utils/utils.py
```

### Comparing `pywatershed-0.1.2/setup.py` & `pywatershed-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import platform
-import setuptools
 import warnings
 
-from numpy.distutils.misc_util import Configuration
+import setuptools  # noqa
 from numpy.distutils.core import setup
+from numpy.distutils.misc_util import Configuration
 
 pyws_fortran = str(os.getenv("PYWS_FORTRAN"))
+
 if pyws_fortran.lower() == "true":
     pyws_fortran = True
     if platform.system() == "Windows":
         pyws_fortran = False
         warnings.warn(
             "Fortran source compilation not enabled on Windows", Warning
         )
@@ -19,21 +20,20 @@
     pyws_fortran = False
 
 
 config = Configuration("pywatershed")
 
 if pyws_fortran:
     source_dir_names = {
-        "hydrology": ["PRMSGroundwater", "PRMSCanopy", "PRMSChannel"]
+        "hydrology": ["prms_groundwater", "prms_canopy", "prms_channel"]
     }
-    for dir, names in source_dir_names.items():
+    for dir_name, names in source_dir_names.items():
         for name in names:
             config.add_extension(
                 f"{name}_f",
                 sources=[
-                    f"pywatershed/{dir}/{name}.pyf",
-                    f"pywatershed/{dir}/{name}.f90",
+                    f"pywatershed/{dir_name}/{name}.pyf",
+                    f"pywatershed/{dir_name}/{name}.f90",
                 ],
             )
 
-
-setup(name="pywatershed")
+setup(**config.todict(), packages=setuptools.find_packages())
```

