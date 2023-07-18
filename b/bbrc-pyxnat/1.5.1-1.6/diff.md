# Comparing `tmp/bbrc-pyxnat-1.5.1.tar.gz` & `tmp/bbrc-pyxnat-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrc-pyxnat-1.5.1.tar", last modified: Thu Nov 10 15:04:11 2022, max compression
+gzip compressed data, was "bbrc-pyxnat-1.6.tar", last modified: Tue Jul 18 10:22:32 2023, max compression
```

## Comparing `bbrc-pyxnat-1.5.1.tar` & `bbrc-pyxnat-1.6.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxrwxrwx   0        0        0        0 2022-11-10 15:04:11.926551 bbrc-pyxnat-1.5.1/
--rw-rw-rw-   0        0        0     1663 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     5217 2022-11-10 15:04:11.926551 bbrc-pyxnat-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4390 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-10 15:04:11.879633 bbrc-pyxnat-1.5.1/bbrc_pyxnat.egg-info/
--rw-rw-rw-   0        0        0     5217 2022-11-10 15:04:11.000000 bbrc-pyxnat-1.5.1/bbrc_pyxnat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2166 2022-11-10 15:04:11.000000 bbrc-pyxnat-1.5.1/bbrc_pyxnat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-10 15:04:11.000000 bbrc-pyxnat-1.5.1/bbrc_pyxnat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2022-11-10 15:04:11.000000 bbrc-pyxnat-1.5.1/bbrc_pyxnat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-11-10 15:04:11.000000 bbrc-pyxnat-1.5.1/bbrc_pyxnat.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-10 15:04:11.879633 bbrc-pyxnat-1.5.1/bin/
--rw-rw-rw-   0        0        0    25200 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/bin/sessionmirror.py
-drwxrwxrwx   0        0        0        0 2022-11-10 15:04:11.879633 bbrc-pyxnat-1.5.1/pyxnat/
--rw-rw-rw-   0        0        0      695 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-10 15:04:11.895301 bbrc-pyxnat-1.5.1/pyxnat/core/
--rw-rw-rw-   0        0        0      153 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/__init__.py
--rw-rw-rw-   0        0        0     9938 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/array.py
--rw-rw-rw-   0        0        0     6374 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/attributes.py
-drwxrwxrwx   0        0        0        0 2022-11-10 15:04:11.910934 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/
--rw-rw-rw-   0        0        0     1758 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/__init__.py
--rw-rw-rw-   0        0        0     1026 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/ashs.py
--rw-rw-rw-   0        0        0     7798 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/bamos.py
--rw-rw-rw-   0        0        0     2649 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/basil.py
--rw-rw-rw-   0        0        0     1195 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/cat12.py
--rw-rw-rw-   0        0        0      587 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/dicom.py
--rw-rw-rw-   0        0        0      194 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/donsurf.py
--rw-rw-rw-   0        0        0      614 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/dtifit.py
--rw-rw-rw-   0        0        0     6651 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/freesurfer.py
--rw-rw-rw-   0        0        0     2159 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/freesurfer7_extras.py
--rw-rw-rw-   0        0        0     1065 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/pet_fdg.py
--rw-rw-rw-   0        0        0      488 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/pet_ftm.py
--rw-rw-rw-   0        0        0      953 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/qsxmt.py
--rw-rw-rw-   0        0        0     1136 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/spm12.py
--rw-rw-rw-   0        0        0     3386 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/validator.py
--rw-rw-rw-   0        0        0     7954 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/downloadutils.py
--rw-rw-rw-   0        0        0     3572 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/errors.py
--rw-rw-rw-   0        0        0    22552 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/help.py
--rw-rw-rw-   0        0        0      597 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/httputil.py
--rw-rw-rw-   0        0        0    20220 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/interfaces.py
--rw-rw-rw-   0        0        0    10299 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/jsonutil.py
--rw-rw-rw-   0        0        0    10873 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/manage.py
--rw-rw-rw-   0        0        0      775 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/pathutil.py
--rw-rw-rw-   0        0        0    14888 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/pipelines.py
--rw-rw-rw-   0        0        0    10017 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/provenance.py
--rw-rw-rw-   0        0        0    89440 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/core/resources.py
--rw-rw-rw-   0        0        0     5338 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/schema.py
--rw-rw-rw-   0        0        0    26770 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/search.py
--rw-rw-rw-   0        0        0    11899 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/select.py
--rw-rw-rw-   0        0        0     3633 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/tags.py
--rw-rw-rw-   0        0        0     4272 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/uriutil.py
--rw-rw-rw-   0        0        0     2506 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/users.py
--rw-rw-rw-   0        0        0     2094 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/xpass.py
--rw-rw-rw-   0        0        0     5038 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/core/xpath_store.py
-drwxrwxrwx   0        0        0        0 2022-11-10 15:04:11.926551 bbrc-pyxnat-1.5.1/pyxnat/tests/
--rw-rw-rw-   0        0        0      695 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/__init__.py
--rw-rw-rw-   0        0        0     2745 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/array_test.py
--rw-rw-rw-   0        0        0     3655 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/attributes_test.py
--rw-rw-rw-   0        0        0     1167 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/custom_variables_test.py
--rw-rw-rw-   0        0        0      525 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/downloadutils_test.py
--rw-rw-rw-   0        0        0      482 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/experiments_tests.py
--rw-rw-rw-   0        0        0      557 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/graphdata_test.py
--rw-rw-rw-   0        0        0      321 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/inspector_test.py
--rw-rw-rw-   0        0        0     1917 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/interfaces_test.py
--rw-rw-rw-   0        0        0     1437 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/jsonutil_test.py
--rw-rw-rw-   0        0        0      822 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/manage_test.py
--rw-rw-rw-   0        0        0      123 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/pathutil_test.py
--rw-rw-rw-   0        0        0     1854 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/pipelines_test.py
--rw-rw-rw-   0        0        0      570 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/prearchive_test.py
--rw-rw-rw-   0        0        0      237 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/project_manager_tests.py
--rw-rw-rw-   0        0        0     1142 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/provenance_test.py
--rw-rw-rw-   0        0        0     4779 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/repr_tests.py
--rw-rw-rw-   0        0        0    11788 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/resources_test.py
--rw-rw-rw-   0        0        0      520 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/scans_tests.py
--rw-rw-rw-   0        0        0     3002 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/search_test.py
--rw-rw-rw-   0        0        0     3263 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/select_test.py
--rw-rw-rw-   0        0        0     1730 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/sessionmirror_test.py
--rw-rw-rw-   0        0        0     5935 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/test_resource_functions.py
--rw-rw-rw-   0        0        0     1782 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/uriutil_test.py
--rw-rw-rw-   0        0        0     7437 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/user_and_project_management_test.py
--rw-rw-rw-   0        0        0     1462 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/xpass_test.py
--rw-rw-rw-   0        0        0     1021 2022-11-10 14:48:40.000000 bbrc-pyxnat-1.5.1/pyxnat/tests/xpath_test.py
--rw-rw-rw-   0        0        0       19 2022-11-10 15:04:07.000000 bbrc-pyxnat-1.5.1/pyxnat/version.py
--rw-rw-rw-   0        0        0      136 2022-11-10 15:04:11.926551 bbrc-pyxnat-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2521 2022-11-10 14:48:51.000000 bbrc-pyxnat-1.5.1/setup.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 10:22:32.320997 bbrc-pyxnat-1.6/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6070 2023-07-18 10:22:32.320997 bbrc-pyxnat-1.6/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4302 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/README.rst
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 10:22:32.310997 bbrc-pyxnat-1.6/bbrc_pyxnat.egg-info/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6070 2023-07-18 10:22:32.000000 bbrc-pyxnat-1.6/bbrc_pyxnat.egg-info/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2222 2023-07-18 10:22:32.000000 bbrc-pyxnat-1.6/bbrc_pyxnat.egg-info/SOURCES.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2023-07-18 10:22:32.000000 bbrc-pyxnat-1.6/bbrc_pyxnat.egg-info/dependency_links.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      109 2023-07-18 10:22:32.000000 bbrc-pyxnat-1.6/bbrc_pyxnat.egg-info/requires.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        7 2023-07-18 10:22:32.000000 bbrc-pyxnat-1.6/bbrc_pyxnat.egg-info/top_level.txt
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 10:22:32.310997 bbrc-pyxnat-1.6/bin/
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)    24499 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/bin/sessionmirror.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 10:22:32.310997 bbrc-pyxnat-1.6/pyxnat/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      666 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/__init__.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 10:22:32.310997 bbrc-pyxnat-1.6/pyxnat/core/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      148 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/__init__.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     9682 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/array.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6184 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/attributes.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 10:22:32.320997 bbrc-pyxnat-1.6/pyxnat/core/derivatives/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1718 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/__init__.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      991 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/ashs.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     7574 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/bamos.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2567 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/basil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1157 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/cat12.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      562 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/dicom.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      186 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/donsurf.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      601 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/dtifit.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6465 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/freesurfer.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2090 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/freesurfer7_extras.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1055 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/mrtrix3.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1028 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/pet_fdg.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      471 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/pet_ftm.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      903 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/qsxmt.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1099 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/spm12.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3269 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/validator.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      778 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/derivatives/xcp_d.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     7751 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/downloadutils.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3431 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/errors.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21861 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/help.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      576 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/httputil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19614 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/interfaces.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     9953 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/jsonutil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    10565 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/manage.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      745 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/pathutil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14510 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/pipelines.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     9708 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/provenance.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    86916 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/core/resources.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5191 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/schema.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26029 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/search.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    11517 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/select.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3509 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/tags.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4113 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/uriutil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2424 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/users.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2018 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/xpass.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4876 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/core/xpath_store.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 10:22:32.320997 bbrc-pyxnat-1.6/pyxnat/tests/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      583 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/__init__.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2699 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/array_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3556 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/attributes_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1129 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/custom_variables_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      519 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/downloadutils_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      478 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/experiments_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      543 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/graphdata_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      308 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/tests/inspector_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1860 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/interfaces_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1384 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/tests/jsonutil_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      799 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/manage_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      119 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/tests/pathutil_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1785 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/tests/pipelines_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      559 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/prearchive_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      228 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/project_manager_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1109 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/provenance_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4638 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/repr_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    11394 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/resources_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      514 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/scans_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2911 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/tests/search_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3199 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/tests/select_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1691 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/sessionmirror_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     7361 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/tests/test_resource_functions.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1731 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/tests/uriutil_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     7087 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/pyxnat/tests/user_and_project_management_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1425 2022-11-10 14:41:27.000000 bbrc-pyxnat-1.6/pyxnat/tests/xpass_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      993 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/tests/xpath_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       16 2023-07-18 10:19:03.000000 bbrc-pyxnat-1.6/pyxnat/version.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      276 2023-07-18 10:22:32.320997 bbrc-pyxnat-1.6/setup.cfg
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2458 2023-07-18 10:21:43.000000 bbrc-pyxnat-1.6/setup.py
```

### Comparing `bbrc-pyxnat-1.5.1/PKG-INFO` & `bbrc-pyxnat-1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,145 @@
-Metadata-Version: 2.1
-Name: bbrc-pyxnat
-Version: 1.5.1
-Summary: XNAT in Python
-Home-page: https://github.com/pyxnat/pyxnat
-Author: Yannick Schwartz
-Author-email: yannick.schwartz@cea.fr
-License: BSD
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Utilities
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-=======
-pyxnat
-=======
-
-..  image:: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml/badge.svg
-     :target: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml
-.. image:: https://coveralls.io/repos/github/pyxnat/pyxnat/badge.svg?branch=master
-    :target: https://coveralls.io/github/pyxnat/pyxnat?branch=master
-.. image:: https://img.shields.io/pypi/dm/pyxnat.svg
-    :target: https://pypi.org/project/pyxnat/
-.. image:: https://img.shields.io/pypi/pyversions/pyxnat.svg
-    :target: https://pypi.org/project/pyxnat
-.. image:: https://img.shields.io/pypi/v/pyxnat.svg
-    :target: https://pypi.org/project/pyxnat
-
-.. image:: https://gitlab.com/xgrg/tweetit/-/raw/master/resources/008-pyxnat-v1.4.gif?inline=false
-
-Where to get it
-===============
-
-The source code is currently hosted on GitHub at:
-https://github.com/pyxnat/pyxnat
-
-Binary installers for the latest released version are available at the `Python
-package index <https://pypi.org/project/pyxnat>`_. **pyxnat** can be installed
-using ``pip`` with the following command::
-
-    pip install pyxnat
-
-Dependencies
-============
-
-- `requests <https://2.python-requests.org/en/master/>`_ v2.20 or higher
-- `python-lxml <https://lxml.de/>`_ v4.3.2 or higher recommended, earlier versions may work.
-
-For development purposes:
-
-- *python-nose* v1.2.1 or higher
-- *coverage* v3.6 or higher
-
-See the `full installation instructions <https://pyxnat.github.io/pyxnat/installing.html>`_
-for recommended and optional dependencies.
-
-Installation from sources
-=========================
-
-To install **pyxnat** from source, from the ``pyxnat`` directory (same one
-where you found this file after cloning the git repo), execute::
-
-    python setup.py install
-
-
-Documentation
-=============
-
-The official documentation is hosted at: https://pyxnat.github.io/pyxnat
-
-Running the test suite
-=========================
-
-Until v1.1 tests were exclusively performed on `XNAT Central <http://central.xnat.org>`_
-using a dedicated user account (``nosetests``). Yet some tests were not allowed to
-run due to restricted permissions.
-In v1.1, tests were restructured and were directed to two independent XNAT
-instances based on permission level. Hence `XNAT Central <http://central.xnat.org>`_
-is still used for most tests with read access whereas other tests requiring
-write permissions are run on a local XNAT instance in a Docker container.
-
-Consequently, running the test suite now requires the following:
-
-  - *python-nose* v1.2.1+
-  - *coverage* v3.6+
-  - *docker* v18+
-
-Setting up a local Docker-powered XNAT instance may be achieved easily using
-``docker-compose`` and any available recipe. We recommend the one from the
-`following repository <https://github.com/NrgXnat/xnat-docker-compose>`_
-(maintained by the XNAT team). Once the repository cloned, run the following
-command (possibly as ``sudo``) ::
-
-  docker-compose up -d
-
-After a couple of minutes, the XNAT instance should be up and running locally.
-You may check it out visiting http://localhost.
-
-The script ``tests/setup_xnat.py`` may then be executed to populate the local
-instance before running the tests.
-
-Finally run the tests with the following command (from the root of the project)::
-
-    nosetests pyxnat/tests
-
-The file ``.github/workflows/ci.yml`` (used for CI) features these described
-steps and may be referred to for further information.
-
-
-Building the documentation
-==========================
-
-Building the docs requires to have `setuptools <https://pypi.org/project/setuptools/>`_
-and `sphinx <http://www.sphinx-doc.org/en/master/>`_ (v2.0+) installed.
-Then run the command::
-
-    python setup.py build_sphinx
-
-The docs are built in the ``build/sphinx/html`` folder.
-
-Contribute to **pyxnat**
-=========================
-
-To contribute to **pyxnat**, first create an account on `GitHub
-<http://github.com/>`_. Once this is done, fork the `pyxnat repository
-<http://github.com/pyxnat/pyxnat>`_ to have you own repository,
-clone it using ``git clone`` on the computers where you want to work. Make
-changes in your clone, push them to your GitHub fork, test them
-on several computers and when you are happy with them, send a `pull
-request <https://github.com/pyxnat/pyxnat/issues>`_ to the main repository.
-
-License
-=======
-
-`BSD 3 <LICENSE>`_
+Metadata-Version: 2.1
+Name: bbrc-pyxnat
+Version: 1.6
+Summary: XNAT in Python
+Home-page: https://github.com/pyxnat/pyxnat
+Author: Yannick Schwartz
+Author-email: yannick.schwartz@cea.fr
+License: BSD
+Description: =======
+        pyxnat
+        =======
+        
+        ..  image:: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml/badge.svg
+             :target: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml
+        .. image:: https://coveralls.io/repos/github/pyxnat/pyxnat/badge.svg?branch=master
+            :target: https://coveralls.io/github/pyxnat/pyxnat?branch=master
+        .. image:: https://img.shields.io/pypi/dm/pyxnat.svg
+            :target: https://pypi.org/project/pyxnat/
+        .. image:: https://img.shields.io/pypi/pyversions/pyxnat.svg
+            :target: https://pypi.org/project/pyxnat
+        .. image:: https://img.shields.io/pypi/v/pyxnat.svg
+            :target: https://pypi.org/project/pyxnat
+        
+        .. image:: https://gitlab.com/xgrg/tweetit/-/raw/master/resources/008-pyxnat-v1.4.gif?inline=false
+        
+        Where to get it
+        ===============
+        
+        The source code is currently hosted on GitHub at:
+        https://github.com/pyxnat/pyxnat
+        
+        Binary installers for the latest released version are available at the `Python
+        package index <https://pypi.org/project/pyxnat>`_. **pyxnat** can be installed
+        using ``pip`` with the following command::
+        
+            pip install pyxnat
+        
+        Dependencies
+        ============
+        
+        - `requests <https://requests.readthedocs.io/>`_ v2.20 or higher
+        - `python-lxml <https://lxml.de/>`_ v4.3.2 or higher recommended, earlier versions may work.
+        
+        For development purposes:
+        
+        - `pytest <https://pytest.org/>`_ v7.1 or higher
+        - `coverage <https://coverage.readthedocs.io/>`_ v3.6 or higher
+        
+        See the `full installation instructions <https://pyxnat.github.io/pyxnat/installing.html>`_
+        for recommended and optional dependencies.
+        
+        Installation from sources
+        =========================
+        
+        To install **pyxnat** from source, from the ``pyxnat`` directory (same one
+        where you found this file after cloning the git repo), execute::
+        
+            python setup.py install
+        
+        
+        Documentation
+        =============
+        
+        The official documentation is hosted at: https://pyxnat.github.io/pyxnat
+        
+        Running the test suite
+        =========================
+        
+        Until v1.1 tests were exclusively performed on `XNAT Central <http://central.xnat.org>`_
+        using a dedicated user account (``nosetests``). Yet some tests were not allowed to
+        run due to restricted permissions.
+        In v1.1, tests were restructured and were directed to two independent XNAT
+        instances based on permission level. Hence `XNAT Central <http://central.xnat.org>`_
+        is still used for most tests with read access whereas other tests requiring
+        write permissions are run on a local XNAT instance in a Docker container.
+        
+        Consequently, running the test suite now requires the following:
+        
+          - *pytest* v7.1+
+          - *coverage* v3.6+
+          - *docker* v18+
+        
+        Setting up a local Docker-powered XNAT instance may be achieved easily using
+        ``docker-compose`` and any available recipe. We recommend the one from the
+        `following repository <https://github.com/NrgXnat/xnat-docker-compose>`_
+        (maintained by the XNAT team). Once the repository cloned, run the following
+        command (possibly as ``sudo``) ::
+        
+          docker-compose up -d
+        
+        After a couple of minutes, the XNAT instance should be up and running locally.
+        You may check it out visiting http://localhost.
+        
+        The script ``tests/setup_xnat.py`` may then be executed to populate the local
+        instance before running the tests.
+        
+        Finally run the tests with the following command (from the root of the project)::
+        
+            pytest --cov pyxnat
+        
+        The file ``.github/workflows/ci.yml`` (used for CI) features these described
+        steps and may be referred to for further information.
+        
+        
+        Building the documentation
+        ==========================
+        
+        Building the docs requires to have `setuptools <https://pypi.org/project/setuptools/>`_
+        and `sphinx <http://www.sphinx-doc.org/en/master/>`_ (v2.0+) installed.
+        Then run the command::
+        
+            python setup.py build_sphinx
+        
+        The docs are built in the ``build/sphinx/html`` folder.
+        
+        Contribute to **pyxnat**
+        =========================
+        
+        To contribute to **pyxnat**, first create an account on `GitHub
+        <http://github.com/>`_. Once this is done, fork the `pyxnat repository
+        <http://github.com/pyxnat/pyxnat>`_ to have you own repository,
+        clone it using ``git clone`` on the computers where you want to work. Make
+        changes in your clone, push them to your GitHub fork, test them
+        on several computers and when you are happy with them, send a `pull
+        request <https://github.com/pyxnat/pyxnat/issues>`_ to the main repository.
+        
+        License
+        =======
+        
+        `BSD 3 <LICENSE>`_
+        
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Utilities
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/x-rst
```

### Comparing `bbrc-pyxnat-1.5.1/README.rst` & `bbrc-pyxnat-1.6/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-=======
-pyxnat
-=======
-
-..  image:: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml/badge.svg
-     :target: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml
-.. image:: https://coveralls.io/repos/github/pyxnat/pyxnat/badge.svg?branch=master
-    :target: https://coveralls.io/github/pyxnat/pyxnat?branch=master
-.. image:: https://img.shields.io/pypi/dm/pyxnat.svg
-    :target: https://pypi.org/project/pyxnat/
-.. image:: https://img.shields.io/pypi/pyversions/pyxnat.svg
-    :target: https://pypi.org/project/pyxnat
-.. image:: https://img.shields.io/pypi/v/pyxnat.svg
-    :target: https://pypi.org/project/pyxnat
-
-.. image:: https://gitlab.com/xgrg/tweetit/-/raw/master/resources/008-pyxnat-v1.4.gif?inline=false
-
-Where to get it
-===============
-
-The source code is currently hosted on GitHub at:
-https://github.com/pyxnat/pyxnat
-
-Binary installers for the latest released version are available at the `Python
-package index <https://pypi.org/project/pyxnat>`_. **pyxnat** can be installed
-using ``pip`` with the following command::
-
-    pip install pyxnat
-
-Dependencies
-============
-
-- `requests <https://2.python-requests.org/en/master/>`_ v2.20 or higher
-- `python-lxml <https://lxml.de/>`_ v4.3.2 or higher recommended, earlier versions may work.
-
-For development purposes:
-
-- *python-nose* v1.2.1 or higher
-- *coverage* v3.6 or higher
-
-See the `full installation instructions <https://pyxnat.github.io/pyxnat/installing.html>`_
-for recommended and optional dependencies.
-
-Installation from sources
-=========================
-
-To install **pyxnat** from source, from the ``pyxnat`` directory (same one
-where you found this file after cloning the git repo), execute::
-
-    python setup.py install
-
-
-Documentation
-=============
-
-The official documentation is hosted at: https://pyxnat.github.io/pyxnat
-
-Running the test suite
-=========================
-
-Until v1.1 tests were exclusively performed on `XNAT Central <http://central.xnat.org>`_
-using a dedicated user account (``nosetests``). Yet some tests were not allowed to
-run due to restricted permissions.
-In v1.1, tests were restructured and were directed to two independent XNAT
-instances based on permission level. Hence `XNAT Central <http://central.xnat.org>`_
-is still used for most tests with read access whereas other tests requiring
-write permissions are run on a local XNAT instance in a Docker container.
-
-Consequently, running the test suite now requires the following:
-
-  - *python-nose* v1.2.1+
-  - *coverage* v3.6+
-  - *docker* v18+
-
-Setting up a local Docker-powered XNAT instance may be achieved easily using
-``docker-compose`` and any available recipe. We recommend the one from the
-`following repository <https://github.com/NrgXnat/xnat-docker-compose>`_
-(maintained by the XNAT team). Once the repository cloned, run the following
-command (possibly as ``sudo``) ::
-
-  docker-compose up -d
-
-After a couple of minutes, the XNAT instance should be up and running locally.
-You may check it out visiting http://localhost.
-
-The script ``tests/setup_xnat.py`` may then be executed to populate the local
-instance before running the tests.
-
-Finally run the tests with the following command (from the root of the project)::
-
-    nosetests pyxnat/tests
-
-The file ``.github/workflows/ci.yml`` (used for CI) features these described
-steps and may be referred to for further information.
-
-
-Building the documentation
-==========================
-
-Building the docs requires to have `setuptools <https://pypi.org/project/setuptools/>`_
-and `sphinx <http://www.sphinx-doc.org/en/master/>`_ (v2.0+) installed.
-Then run the command::
-
-    python setup.py build_sphinx
-
-The docs are built in the ``build/sphinx/html`` folder.
-
-Contribute to **pyxnat**
-=========================
-
-To contribute to **pyxnat**, first create an account on `GitHub
-<http://github.com/>`_. Once this is done, fork the `pyxnat repository
-<http://github.com/pyxnat/pyxnat>`_ to have you own repository,
-clone it using ``git clone`` on the computers where you want to work. Make
-changes in your clone, push them to your GitHub fork, test them
-on several computers and when you are happy with them, send a `pull
-request <https://github.com/pyxnat/pyxnat/issues>`_ to the main repository.
-
-License
-=======
-
-`BSD 3 <LICENSE>`_
+=======
+pyxnat
+=======
+
+..  image:: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml/badge.svg
+     :target: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml
+.. image:: https://coveralls.io/repos/github/pyxnat/pyxnat/badge.svg?branch=master
+    :target: https://coveralls.io/github/pyxnat/pyxnat?branch=master
+.. image:: https://img.shields.io/pypi/dm/pyxnat.svg
+    :target: https://pypi.org/project/pyxnat/
+.. image:: https://img.shields.io/pypi/pyversions/pyxnat.svg
+    :target: https://pypi.org/project/pyxnat
+.. image:: https://img.shields.io/pypi/v/pyxnat.svg
+    :target: https://pypi.org/project/pyxnat
+
+.. image:: https://gitlab.com/xgrg/tweetit/-/raw/master/resources/008-pyxnat-v1.4.gif?inline=false
+
+Where to get it
+===============
+
+The source code is currently hosted on GitHub at:
+https://github.com/pyxnat/pyxnat
+
+Binary installers for the latest released version are available at the `Python
+package index <https://pypi.org/project/pyxnat>`_. **pyxnat** can be installed
+using ``pip`` with the following command::
+
+    pip install pyxnat
+
+Dependencies
+============
+
+- `requests <https://requests.readthedocs.io/>`_ v2.20 or higher
+- `python-lxml <https://lxml.de/>`_ v4.3.2 or higher recommended, earlier versions may work.
+
+For development purposes:
+
+- `pytest <https://pytest.org/>`_ v7.1 or higher
+- `coverage <https://coverage.readthedocs.io/>`_ v3.6 or higher
+
+See the `full installation instructions <https://pyxnat.github.io/pyxnat/installing.html>`_
+for recommended and optional dependencies.
+
+Installation from sources
+=========================
+
+To install **pyxnat** from source, from the ``pyxnat`` directory (same one
+where you found this file after cloning the git repo), execute::
+
+    python setup.py install
+
+
+Documentation
+=============
+
+The official documentation is hosted at: https://pyxnat.github.io/pyxnat
+
+Running the test suite
+=========================
+
+Until v1.1 tests were exclusively performed on `XNAT Central <http://central.xnat.org>`_
+using a dedicated user account (``nosetests``). Yet some tests were not allowed to
+run due to restricted permissions.
+In v1.1, tests were restructured and were directed to two independent XNAT
+instances based on permission level. Hence `XNAT Central <http://central.xnat.org>`_
+is still used for most tests with read access whereas other tests requiring
+write permissions are run on a local XNAT instance in a Docker container.
+
+Consequently, running the test suite now requires the following:
+
+  - *pytest* v7.1+
+  - *coverage* v3.6+
+  - *docker* v18+
+
+Setting up a local Docker-powered XNAT instance may be achieved easily using
+``docker-compose`` and any available recipe. We recommend the one from the
+`following repository <https://github.com/NrgXnat/xnat-docker-compose>`_
+(maintained by the XNAT team). Once the repository cloned, run the following
+command (possibly as ``sudo``) ::
+
+  docker-compose up -d
+
+After a couple of minutes, the XNAT instance should be up and running locally.
+You may check it out visiting http://localhost.
+
+The script ``tests/setup_xnat.py`` may then be executed to populate the local
+instance before running the tests.
+
+Finally run the tests with the following command (from the root of the project)::
+
+    pytest --cov pyxnat
+
+The file ``.github/workflows/ci.yml`` (used for CI) features these described
+steps and may be referred to for further information.
+
+
+Building the documentation
+==========================
+
+Building the docs requires to have `setuptools <https://pypi.org/project/setuptools/>`_
+and `sphinx <http://www.sphinx-doc.org/en/master/>`_ (v2.0+) installed.
+Then run the command::
+
+    python setup.py build_sphinx
+
+The docs are built in the ``build/sphinx/html`` folder.
+
+Contribute to **pyxnat**
+=========================
+
+To contribute to **pyxnat**, first create an account on `GitHub
+<http://github.com/>`_. Once this is done, fork the `pyxnat repository
+<http://github.com/pyxnat/pyxnat>`_ to have you own repository,
+clone it using ``git clone`` on the computers where you want to work. Make
+changes in your clone, push them to your GitHub fork, test them
+on several computers and when you are happy with them, send a `pull
+request <https://github.com/pyxnat/pyxnat/issues>`_ to the main repository.
+
+License
+=======
+
+`BSD 3 <LICENSE>`_
```

### Comparing `bbrc-pyxnat-1.5.1/bbrc_pyxnat.egg-info/PKG-INFO` & `bbrc-pyxnat-1.6/bbrc_pyxnat.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,145 @@
-Metadata-Version: 2.1
-Name: bbrc-pyxnat
-Version: 1.5.1
-Summary: XNAT in Python
-Home-page: https://github.com/pyxnat/pyxnat
-Author: Yannick Schwartz
-Author-email: yannick.schwartz@cea.fr
-License: BSD
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Utilities
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-=======
-pyxnat
-=======
-
-..  image:: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml/badge.svg
-     :target: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml
-.. image:: https://coveralls.io/repos/github/pyxnat/pyxnat/badge.svg?branch=master
-    :target: https://coveralls.io/github/pyxnat/pyxnat?branch=master
-.. image:: https://img.shields.io/pypi/dm/pyxnat.svg
-    :target: https://pypi.org/project/pyxnat/
-.. image:: https://img.shields.io/pypi/pyversions/pyxnat.svg
-    :target: https://pypi.org/project/pyxnat
-.. image:: https://img.shields.io/pypi/v/pyxnat.svg
-    :target: https://pypi.org/project/pyxnat
-
-.. image:: https://gitlab.com/xgrg/tweetit/-/raw/master/resources/008-pyxnat-v1.4.gif?inline=false
-
-Where to get it
-===============
-
-The source code is currently hosted on GitHub at:
-https://github.com/pyxnat/pyxnat
-
-Binary installers for the latest released version are available at the `Python
-package index <https://pypi.org/project/pyxnat>`_. **pyxnat** can be installed
-using ``pip`` with the following command::
-
-    pip install pyxnat
-
-Dependencies
-============
-
-- `requests <https://2.python-requests.org/en/master/>`_ v2.20 or higher
-- `python-lxml <https://lxml.de/>`_ v4.3.2 or higher recommended, earlier versions may work.
-
-For development purposes:
-
-- *python-nose* v1.2.1 or higher
-- *coverage* v3.6 or higher
-
-See the `full installation instructions <https://pyxnat.github.io/pyxnat/installing.html>`_
-for recommended and optional dependencies.
-
-Installation from sources
-=========================
-
-To install **pyxnat** from source, from the ``pyxnat`` directory (same one
-where you found this file after cloning the git repo), execute::
-
-    python setup.py install
-
-
-Documentation
-=============
-
-The official documentation is hosted at: https://pyxnat.github.io/pyxnat
-
-Running the test suite
-=========================
-
-Until v1.1 tests were exclusively performed on `XNAT Central <http://central.xnat.org>`_
-using a dedicated user account (``nosetests``). Yet some tests were not allowed to
-run due to restricted permissions.
-In v1.1, tests were restructured and were directed to two independent XNAT
-instances based on permission level. Hence `XNAT Central <http://central.xnat.org>`_
-is still used for most tests with read access whereas other tests requiring
-write permissions are run on a local XNAT instance in a Docker container.
-
-Consequently, running the test suite now requires the following:
-
-  - *python-nose* v1.2.1+
-  - *coverage* v3.6+
-  - *docker* v18+
-
-Setting up a local Docker-powered XNAT instance may be achieved easily using
-``docker-compose`` and any available recipe. We recommend the one from the
-`following repository <https://github.com/NrgXnat/xnat-docker-compose>`_
-(maintained by the XNAT team). Once the repository cloned, run the following
-command (possibly as ``sudo``) ::
-
-  docker-compose up -d
-
-After a couple of minutes, the XNAT instance should be up and running locally.
-You may check it out visiting http://localhost.
-
-The script ``tests/setup_xnat.py`` may then be executed to populate the local
-instance before running the tests.
-
-Finally run the tests with the following command (from the root of the project)::
-
-    nosetests pyxnat/tests
-
-The file ``.github/workflows/ci.yml`` (used for CI) features these described
-steps and may be referred to for further information.
-
-
-Building the documentation
-==========================
-
-Building the docs requires to have `setuptools <https://pypi.org/project/setuptools/>`_
-and `sphinx <http://www.sphinx-doc.org/en/master/>`_ (v2.0+) installed.
-Then run the command::
-
-    python setup.py build_sphinx
-
-The docs are built in the ``build/sphinx/html`` folder.
-
-Contribute to **pyxnat**
-=========================
-
-To contribute to **pyxnat**, first create an account on `GitHub
-<http://github.com/>`_. Once this is done, fork the `pyxnat repository
-<http://github.com/pyxnat/pyxnat>`_ to have you own repository,
-clone it using ``git clone`` on the computers where you want to work. Make
-changes in your clone, push them to your GitHub fork, test them
-on several computers and when you are happy with them, send a `pull
-request <https://github.com/pyxnat/pyxnat/issues>`_ to the main repository.
-
-License
-=======
-
-`BSD 3 <LICENSE>`_
+Metadata-Version: 2.1
+Name: bbrc-pyxnat
+Version: 1.6
+Summary: XNAT in Python
+Home-page: https://github.com/pyxnat/pyxnat
+Author: Yannick Schwartz
+Author-email: yannick.schwartz@cea.fr
+License: BSD
+Description: =======
+        pyxnat
+        =======
+        
+        ..  image:: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml/badge.svg
+             :target: https://github.com/pyxnat/pyxnat/actions/workflows/ci.yml
+        .. image:: https://coveralls.io/repos/github/pyxnat/pyxnat/badge.svg?branch=master
+            :target: https://coveralls.io/github/pyxnat/pyxnat?branch=master
+        .. image:: https://img.shields.io/pypi/dm/pyxnat.svg
+            :target: https://pypi.org/project/pyxnat/
+        .. image:: https://img.shields.io/pypi/pyversions/pyxnat.svg
+            :target: https://pypi.org/project/pyxnat
+        .. image:: https://img.shields.io/pypi/v/pyxnat.svg
+            :target: https://pypi.org/project/pyxnat
+        
+        .. image:: https://gitlab.com/xgrg/tweetit/-/raw/master/resources/008-pyxnat-v1.4.gif?inline=false
+        
+        Where to get it
+        ===============
+        
+        The source code is currently hosted on GitHub at:
+        https://github.com/pyxnat/pyxnat
+        
+        Binary installers for the latest released version are available at the `Python
+        package index <https://pypi.org/project/pyxnat>`_. **pyxnat** can be installed
+        using ``pip`` with the following command::
+        
+            pip install pyxnat
+        
+        Dependencies
+        ============
+        
+        - `requests <https://requests.readthedocs.io/>`_ v2.20 or higher
+        - `python-lxml <https://lxml.de/>`_ v4.3.2 or higher recommended, earlier versions may work.
+        
+        For development purposes:
+        
+        - `pytest <https://pytest.org/>`_ v7.1 or higher
+        - `coverage <https://coverage.readthedocs.io/>`_ v3.6 or higher
+        
+        See the `full installation instructions <https://pyxnat.github.io/pyxnat/installing.html>`_
+        for recommended and optional dependencies.
+        
+        Installation from sources
+        =========================
+        
+        To install **pyxnat** from source, from the ``pyxnat`` directory (same one
+        where you found this file after cloning the git repo), execute::
+        
+            python setup.py install
+        
+        
+        Documentation
+        =============
+        
+        The official documentation is hosted at: https://pyxnat.github.io/pyxnat
+        
+        Running the test suite
+        =========================
+        
+        Until v1.1 tests were exclusively performed on `XNAT Central <http://central.xnat.org>`_
+        using a dedicated user account (``nosetests``). Yet some tests were not allowed to
+        run due to restricted permissions.
+        In v1.1, tests were restructured and were directed to two independent XNAT
+        instances based on permission level. Hence `XNAT Central <http://central.xnat.org>`_
+        is still used for most tests with read access whereas other tests requiring
+        write permissions are run on a local XNAT instance in a Docker container.
+        
+        Consequently, running the test suite now requires the following:
+        
+          - *pytest* v7.1+
+          - *coverage* v3.6+
+          - *docker* v18+
+        
+        Setting up a local Docker-powered XNAT instance may be achieved easily using
+        ``docker-compose`` and any available recipe. We recommend the one from the
+        `following repository <https://github.com/NrgXnat/xnat-docker-compose>`_
+        (maintained by the XNAT team). Once the repository cloned, run the following
+        command (possibly as ``sudo``) ::
+        
+          docker-compose up -d
+        
+        After a couple of minutes, the XNAT instance should be up and running locally.
+        You may check it out visiting http://localhost.
+        
+        The script ``tests/setup_xnat.py`` may then be executed to populate the local
+        instance before running the tests.
+        
+        Finally run the tests with the following command (from the root of the project)::
+        
+            pytest --cov pyxnat
+        
+        The file ``.github/workflows/ci.yml`` (used for CI) features these described
+        steps and may be referred to for further information.
+        
+        
+        Building the documentation
+        ==========================
+        
+        Building the docs requires to have `setuptools <https://pypi.org/project/setuptools/>`_
+        and `sphinx <http://www.sphinx-doc.org/en/master/>`_ (v2.0+) installed.
+        Then run the command::
+        
+            python setup.py build_sphinx
+        
+        The docs are built in the ``build/sphinx/html`` folder.
+        
+        Contribute to **pyxnat**
+        =========================
+        
+        To contribute to **pyxnat**, first create an account on `GitHub
+        <http://github.com/>`_. Once this is done, fork the `pyxnat repository
+        <http://github.com/pyxnat/pyxnat>`_ to have you own repository,
+        clone it using ``git clone`` on the computers where you want to work. Make
+        changes in your clone, push them to your GitHub fork, test them
+        on several computers and when you are happy with them, send a `pull
+        request <https://github.com/pyxnat/pyxnat/issues>`_ to the main repository.
+        
+        License
+        =======
+        
+        `BSD 3 <LICENSE>`_
+        
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Utilities
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/x-rst
```

### Comparing `bbrc-pyxnat-1.5.1/bbrc_pyxnat.egg-info/SOURCES.txt` & `bbrc-pyxnat-1.6/bbrc_pyxnat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.rst
 setup.cfg
 setup.py
 bbrc_pyxnat.egg-info/PKG-INFO
 bbrc_pyxnat.egg-info/SOURCES.txt
 bbrc_pyxnat.egg-info/dependency_links.txt
 bbrc_pyxnat.egg-info/requires.txt
@@ -38,38 +37,40 @@
 pyxnat/core/derivatives/basil.py
 pyxnat/core/derivatives/cat12.py
 pyxnat/core/derivatives/dicom.py
 pyxnat/core/derivatives/donsurf.py
 pyxnat/core/derivatives/dtifit.py
 pyxnat/core/derivatives/freesurfer.py
 pyxnat/core/derivatives/freesurfer7_extras.py
+pyxnat/core/derivatives/mrtrix3.py
 pyxnat/core/derivatives/pet_fdg.py
 pyxnat/core/derivatives/pet_ftm.py
 pyxnat/core/derivatives/qsxmt.py
 pyxnat/core/derivatives/spm12.py
 pyxnat/core/derivatives/validator.py
+pyxnat/core/derivatives/xcp_d.py
 pyxnat/tests/__init__.py
 pyxnat/tests/array_test.py
 pyxnat/tests/attributes_test.py
 pyxnat/tests/custom_variables_test.py
 pyxnat/tests/downloadutils_test.py
-pyxnat/tests/experiments_tests.py
+pyxnat/tests/experiments_test.py
 pyxnat/tests/graphdata_test.py
 pyxnat/tests/inspector_test.py
 pyxnat/tests/interfaces_test.py
 pyxnat/tests/jsonutil_test.py
 pyxnat/tests/manage_test.py
 pyxnat/tests/pathutil_test.py
 pyxnat/tests/pipelines_test.py
 pyxnat/tests/prearchive_test.py
-pyxnat/tests/project_manager_tests.py
+pyxnat/tests/project_manager_test.py
 pyxnat/tests/provenance_test.py
-pyxnat/tests/repr_tests.py
+pyxnat/tests/repr_test.py
 pyxnat/tests/resources_test.py
-pyxnat/tests/scans_tests.py
+pyxnat/tests/scans_test.py
 pyxnat/tests/search_test.py
 pyxnat/tests/select_test.py
 pyxnat/tests/sessionmirror_test.py
 pyxnat/tests/test_resource_functions.py
 pyxnat/tests/uriutil_test.py
 pyxnat/tests/user_and_project_management_test.py
 pyxnat/tests/xpass_test.py
```

### Comparing `bbrc-pyxnat-1.5.1/bin/sessionmirror.py` & `bbrc-pyxnat-1.6/bin/sessionmirror.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,699 +1,699 @@
-#!/usr/bin/env python
-'''
-The MIT License (MIT)
-
-Copyright (c) 2014 VUIIS
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-'''
-
-'''
-Adapted from xnatmirror (https://github.com/VUIIS/dax/blob/master/bin/Xnat_tools/Xnatmirror)
-'''
-
-def cmp(a, b):
-    return (a > b) - (a < b)
-
-from builtins import zip
-from builtins import str
-
-import os
-import os.path as op
-import sys
-
-from xml.etree import cElementTree as ET
-import pyxnat
-
-PROJ_ATTRS = [
-    'xnat:projectData/name',
-    'xnat:projectData/description',
-    'xnat:projectData/keywords',
-]
-
-SUBJ_ATTRS = [
-    'xnat:subjectData/group',
-    'xnat:subjectData/src',
-    'xnat:subjectData/investigator/firstname',
-    'xnat:subjectData/investigator/lastname',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/dob',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/yob',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/age',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/gender',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/handedness',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/ses',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/education',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/\
-educationDesc',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/race',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/ethnicity',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/weight',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/height',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/\
-gestational_age',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/\
-post_menstrual_age',
-    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/\
-birth_weight'
-]
-
-MR_EXP_ATTRS = [
-    'xnat:experimentData/date',
-    'xnat:experimentData/visit_id',
-    'xnat:experimentData/time',
-    'xnat:experimentData/note',
-    'xnat:experimentData/investigator/firstname',
-    'xnat:experimentData/investigator/lastname',
-    'xnat:imageSessionData/scanner/manufacturer',
-    'xnat:imageSessionData/scanner/model',
-    'xnat:imageSessionData/operator',
-    'xnat:imageSessionData/dcmAccessionNumber',
-    'xnat:imageSessionData/dcmPatientId',
-    'xnat:imageSessionData/dcmPatientName',
-    'xnat:imageSessionData/session_type',
-    'xnat:imageSessionData/modality',
-    'xnat:imageSessionData/UID',
-    'xnat:mrSessionData/coil',
-    'xnat:mrSessionData/fieldStrength',
-    'xnat:mrSessionData/marker',
-    'xnat:mrSessionData/stabilization'
-]
-
-OTHER_DICOM_SCAN_ATTRS = [
-    'xnat:imageScanData/type',
-    'xnat:imageScanData/UID',
-    'xnat:imageScanData/note',
-    'xnat:imageScanData/quality',
-    'xnat:imageScanData/condition',
-    'xnat:imageScanData/series_description',
-    'xnat:imageScanData/documentation',
-    'xnat:imageScanData/frames',
-    'xnat:imageScanData/startTime',
-    'xnat:imageScanData/scanner/manufacturer',
-    'xnat:imageScanData/scanner/model'
-]
-
-MR_SCAN_ATTRS = [
-    'xnat:imageScanData/type',
-    'xnat:imageScanData/UID',
-    'xnat:imageScanData/note',
-    'xnat:imageScanData/quality',
-    'xnat:imageScanData/condition',
-    'xnat:imageScanData/series_description',
-    'xnat:imageScanData/documentation',
-    'xnat:imageScanData/frames',
-    'xnat:imageScanData/startTime',
-    'xnat:imageScanData/scanner/manufacturer',
-    'xnat:imageScanData/scanner/model',
-    'xnat:mrScanData/parameters/flip',
-    'xnat:mrScanData/parameters/orientation',
-    'xnat:mrScanData/parameters/tr',
-    'xnat:mrScanData/parameters/ti',
-    'xnat:mrScanData/parameters/te',
-    'xnat:mrScanData/parameters/sequence',
-    'xnat:mrScanData/parameters/imageType',
-    'xnat:mrScanData/parameters/scanSequence',
-    'xnat:mrScanData/parameters/seqVariant',
-    'xnat:mrScanData/parameters/scanOptions',
-    'xnat:mrScanData/parameters/acqType',
-    'xnat:mrScanData/parameters/pixelBandwidth',
-    'xnat:mrScanData/parameters/voxelRes/x',
-    'xnat:mrScanData/parameters/voxelRes/y',
-    'xnat:mrScanData/parameters/voxelRes/z',
-    'xnat:mrScanData/parameters/fov/x',
-    'xnat:mrScanData/parameters/fov/y',
-    'xnat:mrScanData/parameters/matrix/x',
-    'xnat:mrScanData/parameters/matrix/y',
-    'xnat:mrScanData/parameters/partitions',
-    'xnat:mrScanData/fieldStrength',
-    'xnat:mrScanData/marker',
-    'xnat:mrScanData/stabilization',
-    'xnat:mrScanData/coil'
-]
-
-SC_SCAN_ATTRS = [
-    'xnat:imageScanData/type',
-    'xnat:imageScanData/UID',
-    'xnat:imageScanData/note',
-    'xnat:imageScanData/quality',
-    'xnat:imageScanData/condition',
-    'xnat:imageScanData/series_description',
-    'xnat:imageScanData/documentation',
-    'xnat:imageScanData/frames',
-    'xnat:imageScanData/scanner/manufacturer',
-    'xnat:imageScanData/scanner/model'
-]
-
-PET_EXP_ATTRS = [
-    'xnat:experimentData/date',
-    'xnat:experimentData/visit_id',
-    'xnat:experimentData/time',
-    'xnat:experimentData/note',
-    'xnat:experimentData/investigator/firstname',
-    'xnat:experimentData/investigator/lastname',
-    'xnat:imageSessionData/scanner/manufacturer',
-    'xnat:imageSessionData/scanner/model',
-    'xnat:imageSessionData/operator',
-    'xnat:imageSessionData/dcmAccessionNumber',
-    'xnat:imageSessionData/dcmPatientId',
-    'xnat:imageSessionData/dcmPatientName',
-    'xnat:imageSessionData/session_type',
-    'xnat:imageSessionData/modality',
-    'xnat:imageSessionData/UID',
-    'xnat:petSessionData/studyType',
-    'xnat:petSessionData/patientID',
-    'xnat:petSessionData/patientName',
-    'xnat:petSessionData/stabilization',
-    'xnat:petSessionData/start_time_scan',
-    'xnat:petSessionData/start_time_injection',
-    'xnat:petSessionData/tracer/name',
-    'xnat:petSessionData/tracer/startTime',
-    'xnat:petSessionData/tracer/dose',
-    'xnat:petSessionData/tracer/specificActivity',
-    'xnat:petSessionData/tracer/totalMass',
-    'xnat:petSessionData/tracer/intermediate',
-    'xnat:petSessionData/tracer/isotope',
-    'xnat:petSessionData/tracer/isotope/half-life',
-    'xnat:petSessionData/tracer/transmissions',
-    'xnat:petSessionData/tracer/transmissions_starttime'
-]
-
-CT_EXP_ATTRS = [
-    'xnat:experimentData/date',
-    'xnat:experimentData/visit_id',
-    'xnat:experimentData/time',
-    'xnat:experimentData/note',
-    'xnat:experimentData/investigator/firstname',
-    'xnat:experimentData/investigator/lastname',
-    'xnat:imageSessionData/scanner/manufacturer',
-    'xnat:imageSessionData/scanner/model',
-    'xnat:imageSessionData/operator',
-    'xnat:imageSessionData/dcmAccessionNumber',
-    'xnat:imageSessionData/dcmPatientId',
-    'xnat:imageSessionData/dcmPatientName',
-    'xnat:imageSessionData/session_type',
-    'xnat:imageSessionData/modality',
-    'xnat:imageSessionData/UID'
-]
-
-PET_SCAN_ATTRS = [
-    'xnat:imageScanData/type',
-    'xnat:imageScanData/UID',
-    'xnat:imageScanData/note',
-    'xnat:imageScanData/quality',
-    'xnat:imageScanData/condition',
-    'xnat:imageScanData/series_description',
-    'xnat:imageScanData/documentation',
-    'xnat:imageScanData/frames',
-    'xnat:imageScanData/scanner/manufacturer',
-    'xnat:imageScanData/scanner/model',
-    'xnat:imageScanData/startTime',
-    'xnat:petScanData/parameters/orientation',
-    'xnat:petScanData/parameters/originalFileName',
-    'xnat:petScanData/parameters/systemType',
-    'xnat:petScanData/parameters/fileType',
-    'xnat:petScanData/parameters/transaxialFOV',
-    'xnat:petScanData/parameters/acqType',
-    'xnat:petScanData/parameters/facility',
-    'xnat:petScanData/parameters/numPlanes',
-    'xnat:petScanData/parameters/frames/numFrames',
-    'xnat:petScanData/parameters/numGates',
-    'xnat:petScanData/parameters/planeSeparation',
-    'xnat:petScanData/parameters/binSize',
-    'xnat:petScanData/parameters/dataType'
-]
-
-CT_SCAN_ATTRS = [
-    'xnat:imageScanData/type',
-    'xnat:imageScanData/UID',
-    'xnat:imageScanData/note',
-    'xnat:imageScanData/quality',
-    'xnat:imageScanData/condition',
-    'xnat:imageScanData/series_description',
-    'xnat:imageScanData/documentation',
-    'xnat:imageScanData/frames',
-    'xnat:imageScanData/scanner/manufacturer',
-    'xnat:imageScanData/scanner/model'
-]
-
-PROC_ATTRS = [
-    'proc:genProcData/validation/status',
-    'proc:genProcData/procstatus',
-    'proc:genProcData/proctype',
-    'proc:genProcData/procversion',
-    'proc:genProcData/walltimeused',
-    'proc:genProcData/memused'
-]
-
-
-def copy_attrs(src_obj, dest_obj, attr_list):
-    """ Copies list of attributes form source to destination"""
-    src_attrs = src_obj.attrs.mget(attr_list)
-    src_list = dict(list(zip(attr_list, src_attrs)))
-
-    # NOTE: For some reason need to set te again b/c a bug somewhere sets te
-    # to sequence name
-    te_key = 'xnat:mrScanData/parameters/te'
-    if te_key in src_list:
-        src_list[te_key] = src_obj.attrs.get(te_key)
-
-    dest_obj.attrs.mset(src_list)
-    return 0
-
-
-def copy_attributes(src_obj, dest_obj):
-    '''Copy attributes from src to dest'''
-    src_type = src_obj.datatype()
-    types = {'xnat:projectData': PROJ_ATTRS,
-             'xnat:subjectData': SUBJ_ATTRS,
-             'xnat:mrSessionData': MR_EXP_ATTRS,
-             'xnat:petSessionData': PET_EXP_ATTRS,
-             'xnat:ctSessionData': CT_EXP_ATTRS,
-             'xnat:mrScanData': MR_SCAN_ATTRS,
-             'xnat:petScanData': PET_SCAN_ATTRS,
-             'xnat:ctScanData': CT_SCAN_ATTRS,
-             'xnat:scScanData': SC_SCAN_ATTRS,
-             'proc:genProcData': PROC_ATTRS,
-             'xnat:otherDicomScanData': OTHER_DICOM_SCAN_ATTRS}
-
-    try:
-        copy_attrs(src_obj, dest_obj, types[src_type])
-    except KeyError:
-        print('ERROR:cannot copy attributes, unsupported datatype:' + src_type)
-
-
-def subj_compare(item1, item2):
-    '''Compare sort of items'''
-    return cmp(item1.label(), item2.label())
-
-
-def copy_file(src_f, dest_r, cache_d):
-    '''
-    Copy file from XNAT file source to XNAT resource destination,
-    using local cache in between'''
-    f_label = src_f.label()
-    loc_f = cache_d + '/' + f_label
-
-    # Make subdirectories
-    loc_d = op.dirname(loc_f)
-    if not op.exists(loc_d):
-        os.makedirs(loc_d)
-
-    try:
-        # Download file
-        if op.exists(loc_f) is False:
-            src_f.get(loc_f)
-
-        # Get File Attributes
-        f_in_attrs = src_f.attributes()
-        f_content = f_in_attrs.get('file_content')
-        f_format = f_in_attrs.get('file_format')
-        f_tags = f_in_attrs.get('file_tags')
-
-        # Upload File
-        if f_format and f_content and not f_tags:         # format & content
-            dest_r.file(f_label).put(loc_f, f_format, f_content)
-        elif f_format and not f_content and not f_tags:   # format only
-            dest_r.file(f_label).put(loc_f, f_format)
-        elif f_format and f_content and f_tags:   # format, content, & tags
-            dest_r.file(f_label).put(loc_f, f_format, f_content)
-        else:                                             # none
-            dest_r.file(f_label).put(loc_f)
-
-        # Delete local copy
-        os.remove(loc_f)
-    except Exception:
-        print("ERROR:failed to copy file:%s, error=%s"
-              % (f_label, sys.exc_info()[0]))
-
-
-def copy_res_zip(src_r, dest_r, cache_d):
-    '''
-    Copy a resource from XNAT source to XNAT destination using local cache
-    in between
-    '''
-    try:
-        # Download zip of resource
-        print('INFO:Downloading resource as zip...')
-        cache_z = src_r.get(cache_d, extract=False)
-
-        # Upload zip of resource
-        print('INFO:Uploading resource as zip...')
-        dest_r.put_zip(cache_z, extract=True)
-
-        # Delete cached zip
-        os.remove(cache_z)
-
-    except IndexError:
-        print('ERROR:failed to copy:%s:%s' % (cache_z, sys.exc_info()[0]))
-        raise
-
-
-def is_empty_resource(_res):
-    '''Check if resource contains any files'''
-    f_count = 0
-    for f_in in _res.files().fetchall('obj'):
-        f_count += 1
-        break
-
-    return f_count == 0
-
-# copy_project and copy_subject are untested
-
-# def copy_project(src_proj, dst_proj, proj_cache_dir):
-#     '''Copy XNAT project from source to destination'''
-#
-#     if not dst_proj.exists():
-#         try:
-#             dst_proj.create()
-#         except Exception as e:
-#             msg = 'ERROR: can not create project on destination '\
-#                 'xnat. Check your user rights. %s' % e
-#             raise Exception(msg)
-#         copy_attributes(src_proj, dst_proj)
-#     print('INFO:loading and sorting subject list...')
-#
-#     proj_label = src_proj.label()
-#     subj_list = src_xnat.get_subjects(proj_label)
-#     subj_list = [x for x in subj_list if x['label'] not in SUBJECTS_MIRRORED]
-#     subj_i = 0
-#     for subj in subj_list:
-#         subj_i += 1
-#         subject_label = subj['label']
-#
-#         print("INFO:Processing subject %s (%d)..." % (subject_label, subj_i))
-#         src_subj = src_proj.subject(subject_label)
-#         dst_subj = dst_proj.subject(subject_label)
-#         subj_cache_dir = op.join(proj_cache_dir, subject_label)
-#         copy_subject(src_subj, dst_subj, subj_cache_dir)
-
-
-# def copy_subject(src_subj, dst_subj, subj_cache_dir):
-#     '''Copy subject from XNAT src to XNAT dst'''
-#
-#     if not dst_subj.exists():
-#         print('INFO:uploading subject attributes as xml')
-#
-#         # Create dirs
-#         if not op.exists(subj_cache_dir):
-#             os.makedirs(subj_cache_dir)
-#
-#         # Write xml to file
-#         subj_xml = src_subj.get()
-#         xml_path = op.join(subj_cache_dir, 'subj.xml')
-#         write_xml(subj_xml, xml_path)
-#         dst_subj.create(xml=xml_path, allowDataDeletion=False)
-#
-#     # Process each experiment of subject
-#     for src_sess in src_subj.experiments().fetchall('obj'):
-#         sess_label = src_sess.label()
-#         sess_type = src_sess.datatype()
-#         if sess_type != 'xnat:mrSessionData' and \
-#            sess_type != 'xnat:petSessionData' and \
-#            sess_type != 'xnat:ctSessionData':
-#             print('WARN:Skipping, session is not MR, CT, or PET Session')
-#             continue
-#
-#         print("INFO:Processing session:%s..." % (sess_label))
-#
-#         dst_sess = dst_subj.experiment(sess_label)
-#         sess_cache_dir = op.join(subj_cache_dir, sess_label)
-#         copy_session(src_sess, dst_sess, sess_cache_dir)
-
-
-def copy_session(src_sess, dst_sess, sess_cache_dir):
-    '''Copy XNAT session from source to destination'''
-
-    print('INFO:uploading session attributes as xml')
-    # Write xml to file
-    if not op.exists(sess_cache_dir):
-        os.makedirs(sess_cache_dir)
-    sess_xml = src_sess.get()
-    xml_path = op.join(sess_cache_dir, 'sess.xml')
-    write_xml(sess_xml, xml_path)
-
-    sess_type = src_sess.datatype()
-    dst_sess.create(experiments=sess_type)
-    copy_attributes(src_sess, dst_sess)
-
-    # Process each scan of session
-    for src_scan in src_sess.scans().fetchall('obj'):
-        scan_label = src_scan.label()
-
-        print('INFO:Processing scan:%s...' % scan_label)
-        dst_scan = dst_sess.scan(scan_label)
-        scan_cache_dir = op.join(sess_cache_dir, scan_label)
-        copy_scan(src_scan, dst_scan, scan_cache_dir)
-
-    # Process each assessor of session
-    for src_assr in src_sess.assessors():
-        assr_label = src_assr.label()
-        print('INFO:Processing assessor:%s:...' % assr_label)
-        # dst_assr = dst_sess.assessor(assr_label)
-        # assr_cache_dir = op.join(sess_cache_dir, assr_label)
-        # copy_assr(src_assr, dst_assr, assr_cache_dir)
-
-    for src_res in src_sess.resources().fetchall('obj'):
-        res_label = src_res.label()
-
-        print('INFO:Processing resource:%s...' % (res_label))
-
-        dst_res = dst_sess.resource(res_label)
-
-        res_cache_dir = op.join(scan_cache_dir, res_label)
-
-        copy_res(src_res, dst_res, res_cache_dir, use_zip=True)
-
-
-def copy_scan(src_scan, dst_scan, scan_cache_dir):
-    '''Copy scan from source XNAT to destination XNAT'''
-
-    scan_type = src_scan.datatype()
-    if scan_type == '':
-        scan_type = 'xnat:otherDicomScanData'
-    dst_scan.create(scans=scan_type)
-    copy_attributes(src_scan, dst_scan)
-
-    # Process each resource of scan
-    for src_res in src_scan.resources().fetchall('obj'):
-        res_label = src_res.label()
-
-        print('INFO:Processing resource:%s...' % res_label)
-
-        dst_res = dst_scan.resource(res_label)
-
-        res_cache_dir = op.join(scan_cache_dir, res_label)
-        if res_label == 'SNAPSHOTS':
-            copy_res(src_res, dst_res, res_cache_dir)
-        else:
-            copy_res(src_res, dst_res, res_cache_dir, use_zip=True)
-
-
-def copy_res(src_res, dst_res, res_cache_dir, use_zip=False):
-    '''Copy resource from source XNAT to destination XNAT'''
-    # Create cache dir
-    if not op.exists(res_cache_dir):
-        os.makedirs(res_cache_dir)
-
-    # Prepare resource and check for empty
-    is_empty = False
-    print(dst_res._uri)
-    if not dst_res.exists():
-        dst_res.create()
-        is_empty = True
-    elif is_empty_resource(dst_res):
-        is_empty = True
-
-    # Check for empty source
-    if is_empty_resource(src_res):
-        print('WARN:empty resource, nothing to copy')
-        return
-
-    if is_empty:
-        if use_zip:
-            # Try to copy as zip
-            try:
-                print('INFO:Copying resource as zip: %s...' % src_res.label())
-                copy_res_zip(src_res, dst_res, res_cache_dir)
-                return
-            except Exception:
-                try:
-                    print('INFO: second attempt to copy resource as zip: %s...'
-                          % src_res.label())
-                    copy_res_zip(src_res, dst_res, res_cache_dir)
-                    return
-                except Exception:
-                    msg = 'ERROR:failed twice to copy resource as zip, will'\
-                        'copy individual files'
-                    print(msg)
-
-        copy_count = 0
-        for f in src_res.files():
-            print('INFO:Copying file: %s...' % f.label())
-            copy_count += 1
-            copy_file(f, dst_res, res_cache_dir)
-        print('INFO:Finished copying resource, %d files copied' % copy_count)
-
-
-# def copy_assr(src_assr, dst_assr, assr_cache_dir):
-#     '''Copy assessor from source XNAT to destination XNAT'''
-#
-#     # Check type
-#     assr_type = src_assr.datatype()
-#     if assr_type != 'proc:genProcData' and assr_type != 'fs:fsData':
-#         print('WARN:skipping unsupported assessor type: {}'.format(assr_type))
-#         return
-#
-#     if not dst_assr.exists():
-#         print('INFO:uploading assessor attributes as xml')
-#         # Write xml to file
-#         if not op.exists(assr_cache_dir):
-#             os.makedirs(assr_cache_dir)
-#         assr_xml = src_assr.get()
-#         xml_path = op.join(assr_cache_dir, 'assr.xml')
-#         write_xml(assr_xml, xml_path)
-#         dst_assr.create(xml=xml_path, allowDataDeletion=False)
-#
-#     # Process each resource of assr
-#     for src_res in src_assr.out_resources():
-#         res_label = src_res.label()
-#         print('INFO:Processing resource:%s...' % res_label)
-#         dst_res = dst_assr.out_resource(res_label)
-#         res_cache_dir = op.join(assr_cache_dir, res_label)
-#
-#         if res_label == 'SNAPSHOTS':
-#             copy_res(src_res, dst_res, res_cache_dir)
-#         else:
-#             copy_res(src_res, dst_res, res_cache_dir, use_zip=True)
-
-
-def write_xml(xml_str, file_path, clean_tags=True):
-    """Writing XML."""
-    root = ET.fromstring(xml_str)
-
-    # We only want the tags and attributes relevant to root, no children
-    if clean_tags:
-        # Remove ID
-        if 'ID' in root.attrib:
-            del root.attrib['ID']
-
-        # Remove sharing tags
-        tag = '{http://nrg.wustl.edu/xnat}sharing'
-        for child in root.findall(tag):
-            root.remove(child)
-
-        # Remove out
-        for child in root.findall('{http://nrg.wustl.edu/xnat}out'):
-            root.remove(child)
-            break
-
-        # Remove session ID
-        tag = '{http://nrg.wustl.edu/xnat}imageSession_ID'
-        for child in root.findall(tag):
-            root.remove(child)
-
-        # Remove subject ID
-        for child in root.findall('{http://nrg.wustl.edu/xnat}subject_ID'):
-            root.remove(child)
-
-        # Remove _session ID
-        tag = '{http://nrg.wustl.edu/xnat}image_session_ID'
-        for child in root.findall(tag):
-            root.remove(child)
-
-        # Remove scans
-        for child in root.findall('{http://nrg.wustl.edu/xnat}scans'):
-            root.remove(child)
-            break
-
-        # Remove assessors
-        for child in root.findall('{http://nrg.wustl.edu/xnat}assessors'):
-            root.remove(child)
-            break
-
-        # Remove resources
-        for child in root.findall('{http://nrg.wustl.edu/xnat}resources'):
-            root.remove(child)
-            break
-
-        # Remove experiments
-        for child in root.findall('{http://nrg.wustl.edu/xnat}experiments'):
-            root.remove(child)
-            break
-
-    try:
-        # Write to file
-        ET.register_namespace('xnat', 'http://nrg.wustl.edu/xnat')
-        ET.register_namespace('proc', 'http://nrg.wustl.edu/proc')
-        ET.register_namespace('prov', 'http://www.nbirn.net/prov')
-        ET.register_namespace('fs', 'http://nrg.wustl.edu/fs')
-        ET.ElementTree(root).write(file_path)
-    except IOError as error:
-        print('ERROR:writing xml file: {}: {}'.format(file_path, str(error)))
-
-
-def create_parser():
-    import argparse
-    """Parse commandline arguments."""
-    arg_parser = argparse.ArgumentParser(
-        description='Downloads a given experiment/session from an XNAT instance '
-                    'and uploads it to an independent one. Only DICOM resources '
-                    'will be imported.',
-        formatter_class=argparse.RawTextHelpFormatter)
-    arg_parser.add_argument(
-        '--h1', '--source_config', dest='source_config',
-        help='Source XNAT configuration file', required=True)
-    arg_parser.add_argument(
-        '--h2', '--dest_config', dest='dest_config', required=True,
-        help='Destination XNAT configuration file')
-    arg_parser.add_argument(
-        '-e', '--experiment_id', required=True,
-        help='Which resource to download? (Entity name/identifier)')
-    arg_parser.add_argument(
-        '-p', '--project_id', dest='project_id', required=True,
-        help='Which project to store the resource in')
-    arg_parser.add_argument(
-        '-v', '--verbose', dest='verbose', action='store_true', default=False,
-        help='Display verbosal information (optional)', required=False)
-
-    return arg_parser
-
-
-def main(args):
-    x1 = pyxnat.Interface(config=args.source_config)
-    x2 = pyxnat.Interface(config=args.dest_config)
-
-    columns = ['subject_label', 'label']
-    e1 = x1.array.experiments(experiment_id=args.experiment_id,
-                              columns=columns).data[0]
-    p = x2.select.project(args.project_id)
-    s = p.subject(e1['subject_label'])
-    if not s.exists():
-        s.create()
-    e = s.experiment(e1['label'])
-
-    src_sess = x1.select.project(e1['project']).subject(e1['subject_ID']).experiment(e1['ID'])
-    dst_sess = e
-
-    copy_session(src_sess, dst_sess, '/tmp')
-
-
-if __name__ == '__main__':
-    parser = create_parser()
-    arguments = parser.parse_args()
-    main(arguments)
+#!/usr/bin/env python
+'''
+The MIT License (MIT)
+
+Copyright (c) 2014 VUIIS
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+'''
+
+'''
+Adapted from xnatmirror (https://github.com/VUIIS/dax/blob/master/bin/Xnat_tools/Xnatmirror)
+'''
+
+def cmp(a, b):
+    return (a > b) - (a < b)
+
+from builtins import zip
+from builtins import str
+
+import os
+import os.path as op
+import sys
+
+from xml.etree import cElementTree as ET
+import pyxnat
+
+PROJ_ATTRS = [
+    'xnat:projectData/name',
+    'xnat:projectData/description',
+    'xnat:projectData/keywords',
+]
+
+SUBJ_ATTRS = [
+    'xnat:subjectData/group',
+    'xnat:subjectData/src',
+    'xnat:subjectData/investigator/firstname',
+    'xnat:subjectData/investigator/lastname',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/dob',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/yob',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/age',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/gender',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/handedness',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/ses',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/education',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/\
+educationDesc',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/race',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/ethnicity',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/weight',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/height',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/\
+gestational_age',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/\
+post_menstrual_age',
+    'xnat:subjectData/demographics[@xsi:type=xnat:demographicData]/\
+birth_weight'
+]
+
+MR_EXP_ATTRS = [
+    'xnat:experimentData/date',
+    'xnat:experimentData/visit_id',
+    'xnat:experimentData/time',
+    'xnat:experimentData/note',
+    'xnat:experimentData/investigator/firstname',
+    'xnat:experimentData/investigator/lastname',
+    'xnat:imageSessionData/scanner/manufacturer',
+    'xnat:imageSessionData/scanner/model',
+    'xnat:imageSessionData/operator',
+    'xnat:imageSessionData/dcmAccessionNumber',
+    'xnat:imageSessionData/dcmPatientId',
+    'xnat:imageSessionData/dcmPatientName',
+    'xnat:imageSessionData/session_type',
+    'xnat:imageSessionData/modality',
+    'xnat:imageSessionData/UID',
+    'xnat:mrSessionData/coil',
+    'xnat:mrSessionData/fieldStrength',
+    'xnat:mrSessionData/marker',
+    'xnat:mrSessionData/stabilization'
+]
+
+OTHER_DICOM_SCAN_ATTRS = [
+    'xnat:imageScanData/type',
+    'xnat:imageScanData/UID',
+    'xnat:imageScanData/note',
+    'xnat:imageScanData/quality',
+    'xnat:imageScanData/condition',
+    'xnat:imageScanData/series_description',
+    'xnat:imageScanData/documentation',
+    'xnat:imageScanData/frames',
+    'xnat:imageScanData/startTime',
+    'xnat:imageScanData/scanner/manufacturer',
+    'xnat:imageScanData/scanner/model'
+]
+
+MR_SCAN_ATTRS = [
+    'xnat:imageScanData/type',
+    'xnat:imageScanData/UID',
+    'xnat:imageScanData/note',
+    'xnat:imageScanData/quality',
+    'xnat:imageScanData/condition',
+    'xnat:imageScanData/series_description',
+    'xnat:imageScanData/documentation',
+    'xnat:imageScanData/frames',
+    'xnat:imageScanData/startTime',
+    'xnat:imageScanData/scanner/manufacturer',
+    'xnat:imageScanData/scanner/model',
+    'xnat:mrScanData/parameters/flip',
+    'xnat:mrScanData/parameters/orientation',
+    'xnat:mrScanData/parameters/tr',
+    'xnat:mrScanData/parameters/ti',
+    'xnat:mrScanData/parameters/te',
+    'xnat:mrScanData/parameters/sequence',
+    'xnat:mrScanData/parameters/imageType',
+    'xnat:mrScanData/parameters/scanSequence',
+    'xnat:mrScanData/parameters/seqVariant',
+    'xnat:mrScanData/parameters/scanOptions',
+    'xnat:mrScanData/parameters/acqType',
+    'xnat:mrScanData/parameters/pixelBandwidth',
+    'xnat:mrScanData/parameters/voxelRes/x',
+    'xnat:mrScanData/parameters/voxelRes/y',
+    'xnat:mrScanData/parameters/voxelRes/z',
+    'xnat:mrScanData/parameters/fov/x',
+    'xnat:mrScanData/parameters/fov/y',
+    'xnat:mrScanData/parameters/matrix/x',
+    'xnat:mrScanData/parameters/matrix/y',
+    'xnat:mrScanData/parameters/partitions',
+    'xnat:mrScanData/fieldStrength',
+    'xnat:mrScanData/marker',
+    'xnat:mrScanData/stabilization',
+    'xnat:mrScanData/coil'
+]
+
+SC_SCAN_ATTRS = [
+    'xnat:imageScanData/type',
+    'xnat:imageScanData/UID',
+    'xnat:imageScanData/note',
+    'xnat:imageScanData/quality',
+    'xnat:imageScanData/condition',
+    'xnat:imageScanData/series_description',
+    'xnat:imageScanData/documentation',
+    'xnat:imageScanData/frames',
+    'xnat:imageScanData/scanner/manufacturer',
+    'xnat:imageScanData/scanner/model'
+]
+
+PET_EXP_ATTRS = [
+    'xnat:experimentData/date',
+    'xnat:experimentData/visit_id',
+    'xnat:experimentData/time',
+    'xnat:experimentData/note',
+    'xnat:experimentData/investigator/firstname',
+    'xnat:experimentData/investigator/lastname',
+    'xnat:imageSessionData/scanner/manufacturer',
+    'xnat:imageSessionData/scanner/model',
+    'xnat:imageSessionData/operator',
+    'xnat:imageSessionData/dcmAccessionNumber',
+    'xnat:imageSessionData/dcmPatientId',
+    'xnat:imageSessionData/dcmPatientName',
+    'xnat:imageSessionData/session_type',
+    'xnat:imageSessionData/modality',
+    'xnat:imageSessionData/UID',
+    'xnat:petSessionData/studyType',
+    'xnat:petSessionData/patientID',
+    'xnat:petSessionData/patientName',
+    'xnat:petSessionData/stabilization',
+    'xnat:petSessionData/start_time_scan',
+    'xnat:petSessionData/start_time_injection',
+    'xnat:petSessionData/tracer/name',
+    'xnat:petSessionData/tracer/startTime',
+    'xnat:petSessionData/tracer/dose',
+    'xnat:petSessionData/tracer/specificActivity',
+    'xnat:petSessionData/tracer/totalMass',
+    'xnat:petSessionData/tracer/intermediate',
+    'xnat:petSessionData/tracer/isotope',
+    'xnat:petSessionData/tracer/isotope/half-life',
+    'xnat:petSessionData/tracer/transmissions',
+    'xnat:petSessionData/tracer/transmissions_starttime'
+]
+
+CT_EXP_ATTRS = [
+    'xnat:experimentData/date',
+    'xnat:experimentData/visit_id',
+    'xnat:experimentData/time',
+    'xnat:experimentData/note',
+    'xnat:experimentData/investigator/firstname',
+    'xnat:experimentData/investigator/lastname',
+    'xnat:imageSessionData/scanner/manufacturer',
+    'xnat:imageSessionData/scanner/model',
+    'xnat:imageSessionData/operator',
+    'xnat:imageSessionData/dcmAccessionNumber',
+    'xnat:imageSessionData/dcmPatientId',
+    'xnat:imageSessionData/dcmPatientName',
+    'xnat:imageSessionData/session_type',
+    'xnat:imageSessionData/modality',
+    'xnat:imageSessionData/UID'
+]
+
+PET_SCAN_ATTRS = [
+    'xnat:imageScanData/type',
+    'xnat:imageScanData/UID',
+    'xnat:imageScanData/note',
+    'xnat:imageScanData/quality',
+    'xnat:imageScanData/condition',
+    'xnat:imageScanData/series_description',
+    'xnat:imageScanData/documentation',
+    'xnat:imageScanData/frames',
+    'xnat:imageScanData/scanner/manufacturer',
+    'xnat:imageScanData/scanner/model',
+    'xnat:imageScanData/startTime',
+    'xnat:petScanData/parameters/orientation',
+    'xnat:petScanData/parameters/originalFileName',
+    'xnat:petScanData/parameters/systemType',
+    'xnat:petScanData/parameters/fileType',
+    'xnat:petScanData/parameters/transaxialFOV',
+    'xnat:petScanData/parameters/acqType',
+    'xnat:petScanData/parameters/facility',
+    'xnat:petScanData/parameters/numPlanes',
+    'xnat:petScanData/parameters/frames/numFrames',
+    'xnat:petScanData/parameters/numGates',
+    'xnat:petScanData/parameters/planeSeparation',
+    'xnat:petScanData/parameters/binSize',
+    'xnat:petScanData/parameters/dataType'
+]
+
+CT_SCAN_ATTRS = [
+    'xnat:imageScanData/type',
+    'xnat:imageScanData/UID',
+    'xnat:imageScanData/note',
+    'xnat:imageScanData/quality',
+    'xnat:imageScanData/condition',
+    'xnat:imageScanData/series_description',
+    'xnat:imageScanData/documentation',
+    'xnat:imageScanData/frames',
+    'xnat:imageScanData/scanner/manufacturer',
+    'xnat:imageScanData/scanner/model'
+]
+
+PROC_ATTRS = [
+    'proc:genProcData/validation/status',
+    'proc:genProcData/procstatus',
+    'proc:genProcData/proctype',
+    'proc:genProcData/procversion',
+    'proc:genProcData/walltimeused',
+    'proc:genProcData/memused'
+]
+
+
+def copy_attrs(src_obj, dest_obj, attr_list):
+    """ Copies list of attributes form source to destination"""
+    src_attrs = src_obj.attrs.mget(attr_list)
+    src_list = dict(list(zip(attr_list, src_attrs)))
+
+    # NOTE: For some reason need to set te again b/c a bug somewhere sets te
+    # to sequence name
+    te_key = 'xnat:mrScanData/parameters/te'
+    if te_key in src_list:
+        src_list[te_key] = src_obj.attrs.get(te_key)
+
+    dest_obj.attrs.mset(src_list)
+    return 0
+
+
+def copy_attributes(src_obj, dest_obj):
+    '''Copy attributes from src to dest'''
+    src_type = src_obj.datatype()
+    types = {'xnat:projectData': PROJ_ATTRS,
+             'xnat:subjectData': SUBJ_ATTRS,
+             'xnat:mrSessionData': MR_EXP_ATTRS,
+             'xnat:petSessionData': PET_EXP_ATTRS,
+             'xnat:ctSessionData': CT_EXP_ATTRS,
+             'xnat:mrScanData': MR_SCAN_ATTRS,
+             'xnat:petScanData': PET_SCAN_ATTRS,
+             'xnat:ctScanData': CT_SCAN_ATTRS,
+             'xnat:scScanData': SC_SCAN_ATTRS,
+             'proc:genProcData': PROC_ATTRS,
+             'xnat:otherDicomScanData': OTHER_DICOM_SCAN_ATTRS}
+
+    try:
+        copy_attrs(src_obj, dest_obj, types[src_type])
+    except KeyError:
+        print('ERROR:cannot copy attributes, unsupported datatype:' + src_type)
+
+
+def subj_compare(item1, item2):
+    '''Compare sort of items'''
+    return cmp(item1.label(), item2.label())
+
+
+def copy_file(src_f, dest_r, cache_d):
+    '''
+    Copy file from XNAT file source to XNAT resource destination,
+    using local cache in between'''
+    f_label = src_f.label()
+    loc_f = cache_d + '/' + f_label
+
+    # Make subdirectories
+    loc_d = op.dirname(loc_f)
+    if not op.exists(loc_d):
+        os.makedirs(loc_d)
+
+    try:
+        # Download file
+        if op.exists(loc_f) is False:
+            src_f.get(loc_f)
+
+        # Get File Attributes
+        f_in_attrs = src_f.attributes()
+        f_content = f_in_attrs.get('file_content')
+        f_format = f_in_attrs.get('file_format')
+        f_tags = f_in_attrs.get('file_tags')
+
+        # Upload File
+        if f_format and f_content and not f_tags:         # format & content
+            dest_r.file(f_label).put(loc_f, f_format, f_content)
+        elif f_format and not f_content and not f_tags:   # format only
+            dest_r.file(f_label).put(loc_f, f_format)
+        elif f_format and f_content and f_tags:   # format, content, & tags
+            dest_r.file(f_label).put(loc_f, f_format, f_content)
+        else:                                             # none
+            dest_r.file(f_label).put(loc_f)
+
+        # Delete local copy
+        os.remove(loc_f)
+    except Exception:
+        print("ERROR:failed to copy file:%s, error=%s"
+              % (f_label, sys.exc_info()[0]))
+
+
+def copy_res_zip(src_r, dest_r, cache_d):
+    '''
+    Copy a resource from XNAT source to XNAT destination using local cache
+    in between
+    '''
+    try:
+        # Download zip of resource
+        print('INFO:Downloading resource as zip...')
+        cache_z = src_r.get(cache_d, extract=False)
+
+        # Upload zip of resource
+        print('INFO:Uploading resource as zip...')
+        dest_r.put_zip(cache_z, extract=True)
+
+        # Delete cached zip
+        os.remove(cache_z)
+
+    except IndexError:
+        print('ERROR:failed to copy:%s:%s' % (cache_z, sys.exc_info()[0]))
+        raise
+
+
+def is_empty_resource(_res):
+    '''Check if resource contains any files'''
+    f_count = 0
+    for f_in in _res.files().fetchall('obj'):
+        f_count += 1
+        break
+
+    return f_count == 0
+
+# copy_project and copy_subject are untested
+
+# def copy_project(src_proj, dst_proj, proj_cache_dir):
+#     '''Copy XNAT project from source to destination'''
+#
+#     if not dst_proj.exists():
+#         try:
+#             dst_proj.create()
+#         except Exception as e:
+#             msg = 'ERROR: can not create project on destination '\
+#                 'xnat. Check your user rights. %s' % e
+#             raise Exception(msg)
+#         copy_attributes(src_proj, dst_proj)
+#     print('INFO:loading and sorting subject list...')
+#
+#     proj_label = src_proj.label()
+#     subj_list = src_xnat.get_subjects(proj_label)
+#     subj_list = [x for x in subj_list if x['label'] not in SUBJECTS_MIRRORED]
+#     subj_i = 0
+#     for subj in subj_list:
+#         subj_i += 1
+#         subject_label = subj['label']
+#
+#         print("INFO:Processing subject %s (%d)..." % (subject_label, subj_i))
+#         src_subj = src_proj.subject(subject_label)
+#         dst_subj = dst_proj.subject(subject_label)
+#         subj_cache_dir = op.join(proj_cache_dir, subject_label)
+#         copy_subject(src_subj, dst_subj, subj_cache_dir)
+
+
+# def copy_subject(src_subj, dst_subj, subj_cache_dir):
+#     '''Copy subject from XNAT src to XNAT dst'''
+#
+#     if not dst_subj.exists():
+#         print('INFO:uploading subject attributes as xml')
+#
+#         # Create dirs
+#         if not op.exists(subj_cache_dir):
+#             os.makedirs(subj_cache_dir)
+#
+#         # Write xml to file
+#         subj_xml = src_subj.get()
+#         xml_path = op.join(subj_cache_dir, 'subj.xml')
+#         write_xml(subj_xml, xml_path)
+#         dst_subj.create(xml=xml_path, allowDataDeletion=False)
+#
+#     # Process each experiment of subject
+#     for src_sess in src_subj.experiments().fetchall('obj'):
+#         sess_label = src_sess.label()
+#         sess_type = src_sess.datatype()
+#         if sess_type != 'xnat:mrSessionData' and \
+#            sess_type != 'xnat:petSessionData' and \
+#            sess_type != 'xnat:ctSessionData':
+#             print('WARN:Skipping, session is not MR, CT, or PET Session')
+#             continue
+#
+#         print("INFO:Processing session:%s..." % (sess_label))
+#
+#         dst_sess = dst_subj.experiment(sess_label)
+#         sess_cache_dir = op.join(subj_cache_dir, sess_label)
+#         copy_session(src_sess, dst_sess, sess_cache_dir)
+
+
+def copy_session(src_sess, dst_sess, sess_cache_dir):
+    '''Copy XNAT session from source to destination'''
+
+    print('INFO:uploading session attributes as xml')
+    # Write xml to file
+    if not op.exists(sess_cache_dir):
+        os.makedirs(sess_cache_dir)
+    sess_xml = src_sess.get()
+    xml_path = op.join(sess_cache_dir, 'sess.xml')
+    write_xml(sess_xml, xml_path)
+
+    sess_type = src_sess.datatype()
+    dst_sess.create(experiments=sess_type)
+    copy_attributes(src_sess, dst_sess)
+
+    # Process each scan of session
+    for src_scan in src_sess.scans().fetchall('obj'):
+        scan_label = src_scan.label()
+
+        print('INFO:Processing scan:%s...' % scan_label)
+        dst_scan = dst_sess.scan(scan_label)
+        scan_cache_dir = op.join(sess_cache_dir, scan_label)
+        copy_scan(src_scan, dst_scan, scan_cache_dir)
+
+    # Process each assessor of session
+    for src_assr in src_sess.assessors():
+        assr_label = src_assr.label()
+        print('INFO:Processing assessor:%s:...' % assr_label)
+        # dst_assr = dst_sess.assessor(assr_label)
+        # assr_cache_dir = op.join(sess_cache_dir, assr_label)
+        # copy_assr(src_assr, dst_assr, assr_cache_dir)
+
+    for src_res in src_sess.resources().fetchall('obj'):
+        res_label = src_res.label()
+
+        print('INFO:Processing resource:%s...' % res_label)
+
+        dst_res = dst_sess.resource(res_label)
+
+        res_cache_dir = op.join(sess_cache_dir, res_label)
+
+        copy_res(src_res, dst_res, res_cache_dir, use_zip=True)
+
+
+def copy_scan(src_scan, dst_scan, scan_cache_dir):
+    '''Copy scan from source XNAT to destination XNAT'''
+
+    scan_type = src_scan.datatype()
+    if scan_type == '':
+        scan_type = 'xnat:otherDicomScanData'
+    dst_scan.create(scans=scan_type)
+    copy_attributes(src_scan, dst_scan)
+
+    # Process each resource of scan
+    for src_res in src_scan.resources().fetchall('obj'):
+        res_label = src_res.label()
+
+        print('INFO:Processing resource:%s...' % res_label)
+
+        dst_res = dst_scan.resource(res_label)
+
+        res_cache_dir = op.join(scan_cache_dir, res_label)
+        if res_label == 'SNAPSHOTS':
+            copy_res(src_res, dst_res, res_cache_dir)
+        else:
+            copy_res(src_res, dst_res, res_cache_dir, use_zip=True)
+
+
+def copy_res(src_res, dst_res, res_cache_dir, use_zip=False):
+    '''Copy resource from source XNAT to destination XNAT'''
+    # Create cache dir
+    if not op.exists(res_cache_dir):
+        os.makedirs(res_cache_dir)
+
+    # Prepare resource and check for empty
+    is_empty = False
+    print(dst_res._uri)
+    if not dst_res.exists():
+        dst_res.create()
+        is_empty = True
+    elif is_empty_resource(dst_res):
+        is_empty = True
+
+    # Check for empty source
+    if is_empty_resource(src_res):
+        print('WARN:empty resource, nothing to copy')
+        return
+
+    if is_empty:
+        if use_zip:
+            # Try to copy as zip
+            try:
+                print('INFO:Copying resource as zip: %s...' % src_res.label())
+                copy_res_zip(src_res, dst_res, res_cache_dir)
+                return
+            except Exception:
+                try:
+                    print('INFO: second attempt to copy resource as zip: %s...'
+                          % src_res.label())
+                    copy_res_zip(src_res, dst_res, res_cache_dir)
+                    return
+                except Exception:
+                    msg = 'ERROR:failed twice to copy resource as zip, will'\
+                        'copy individual files'
+                    print(msg)
+
+        copy_count = 0
+        for f in src_res.files():
+            print('INFO:Copying file: %s...' % f.label())
+            copy_count += 1
+            copy_file(f, dst_res, res_cache_dir)
+        print('INFO:Finished copying resource, %d files copied' % copy_count)
+
+
+# def copy_assr(src_assr, dst_assr, assr_cache_dir):
+#     '''Copy assessor from source XNAT to destination XNAT'''
+#
+#     # Check type
+#     assr_type = src_assr.datatype()
+#     if assr_type != 'proc:genProcData' and assr_type != 'fs:fsData':
+#         print('WARN:skipping unsupported assessor type: {}'.format(assr_type))
+#         return
+#
+#     if not dst_assr.exists():
+#         print('INFO:uploading assessor attributes as xml')
+#         # Write xml to file
+#         if not op.exists(assr_cache_dir):
+#             os.makedirs(assr_cache_dir)
+#         assr_xml = src_assr.get()
+#         xml_path = op.join(assr_cache_dir, 'assr.xml')
+#         write_xml(assr_xml, xml_path)
+#         dst_assr.create(xml=xml_path, allowDataDeletion=False)
+#
+#     # Process each resource of assr
+#     for src_res in src_assr.out_resources():
+#         res_label = src_res.label()
+#         print('INFO:Processing resource:%s...' % res_label)
+#         dst_res = dst_assr.out_resource(res_label)
+#         res_cache_dir = op.join(assr_cache_dir, res_label)
+#
+#         if res_label == 'SNAPSHOTS':
+#             copy_res(src_res, dst_res, res_cache_dir)
+#         else:
+#             copy_res(src_res, dst_res, res_cache_dir, use_zip=True)
+
+
+def write_xml(xml_str, file_path, clean_tags=True):
+    """Writing XML."""
+    root = ET.fromstring(xml_str)
+
+    # We only want the tags and attributes relevant to root, no children
+    if clean_tags:
+        # Remove ID
+        if 'ID' in root.attrib:
+            del root.attrib['ID']
+
+        # Remove sharing tags
+        tag = '{http://nrg.wustl.edu/xnat}sharing'
+        for child in root.findall(tag):
+            root.remove(child)
+
+        # Remove out
+        for child in root.findall('{http://nrg.wustl.edu/xnat}out'):
+            root.remove(child)
+            break
+
+        # Remove session ID
+        tag = '{http://nrg.wustl.edu/xnat}imageSession_ID'
+        for child in root.findall(tag):
+            root.remove(child)
+
+        # Remove subject ID
+        for child in root.findall('{http://nrg.wustl.edu/xnat}subject_ID'):
+            root.remove(child)
+
+        # Remove _session ID
+        tag = '{http://nrg.wustl.edu/xnat}image_session_ID'
+        for child in root.findall(tag):
+            root.remove(child)
+
+        # Remove scans
+        for child in root.findall('{http://nrg.wustl.edu/xnat}scans'):
+            root.remove(child)
+            break
+
+        # Remove assessors
+        for child in root.findall('{http://nrg.wustl.edu/xnat}assessors'):
+            root.remove(child)
+            break
+
+        # Remove resources
+        for child in root.findall('{http://nrg.wustl.edu/xnat}resources'):
+            root.remove(child)
+            break
+
+        # Remove experiments
+        for child in root.findall('{http://nrg.wustl.edu/xnat}experiments'):
+            root.remove(child)
+            break
+
+    try:
+        # Write to file
+        ET.register_namespace('xnat', 'http://nrg.wustl.edu/xnat')
+        ET.register_namespace('proc', 'http://nrg.wustl.edu/proc')
+        ET.register_namespace('prov', 'http://www.nbirn.net/prov')
+        ET.register_namespace('fs', 'http://nrg.wustl.edu/fs')
+        ET.ElementTree(root).write(file_path)
+    except IOError as error:
+        print('ERROR:writing xml file: {}: {}'.format(file_path, str(error)))
+
+
+def create_parser():
+    import argparse
+    """Parse commandline arguments."""
+    arg_parser = argparse.ArgumentParser(
+        description='Downloads a given experiment/session from an XNAT instance '
+                    'and uploads it to an independent one. Only DICOM resources '
+                    'will be imported.',
+        formatter_class=argparse.RawTextHelpFormatter)
+    arg_parser.add_argument(
+        '--h1', '--source_config', dest='source_config',
+        help='Source XNAT configuration file', required=True)
+    arg_parser.add_argument(
+        '--h2', '--dest_config', dest='dest_config', required=True,
+        help='Destination XNAT configuration file')
+    arg_parser.add_argument(
+        '-e', '--experiment_id', required=True,
+        help='Which resource to download? (Entity name/identifier)')
+    arg_parser.add_argument(
+        '-p', '--project_id', dest='project_id', required=True,
+        help='Which project to store the resource in')
+    arg_parser.add_argument(
+        '-v', '--verbose', dest='verbose', action='store_true', default=False,
+        help='Display verbosal information (optional)', required=False)
+
+    return arg_parser
+
+
+def main(args):
+    x1 = pyxnat.Interface(config=args.source_config)
+    x2 = pyxnat.Interface(config=args.dest_config)
+
+    columns = ['subject_label', 'label']
+    e1 = x1.array.experiments(experiment_id=args.experiment_id,
+                              columns=columns).data[0]
+    p = x2.select.project(args.project_id)
+    s = p.subject(e1['subject_label'])
+    if not s.exists():
+        s.create()
+    e = s.experiment(e1['label'])
+
+    src_sess = x1.select.project(e1['project']).subject(e1['subject_ID']).experiment(e1['ID'])
+    dst_sess = e
+
+    copy_session(src_sess, dst_sess, '/tmp')
+
+
+if __name__ == '__main__':
+    parser = create_parser()
+    arguments = parser.parse_args()
+    main(arguments)
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/__init__.py` & `bbrc-pyxnat-1.6/pyxnat/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""
-PyXNAT
-======
-
-:mod:`pyxnat` provides an API to access data on XNAT servers
-(see http://xnat.org).
-
-Visit https://pyxnat.github.io/pyxnat for more information.
-"""
-
-from .version import VERSION as __version__
-
-from .core import Interface
-from .core import SearchManager
-from .core import Select
-from .core import Inspector
-from .core import Users
-from .core import attributes
-from .core import help
-from .core import interfaces
-from .core import resources
-from .core import manage
-from .core import schema
-from .core import select
-from .core import users
-from .core import jsonutil
-from .core import uriutil
-from .core import xpass
-from .core import xpath_store
+"""
+PyXNAT
+======
+
+:mod:`pyxnat` provides an API to access data on XNAT servers
+(see http://xnat.org).
+
+Visit https://pyxnat.github.io/pyxnat for more information.
+"""
+
+from .version import VERSION as __version__
+
+from .core import Interface
+from .core import SearchManager
+from .core import Select
+from .core import Inspector
+from .core import Users
+from .core import attributes
+from .core import help
+from .core import interfaces
+from .core import resources
+from .core import manage
+from .core import schema
+from .core import select
+from .core import users
+from .core import jsonutil
+from .core import uriutil
+from .core import xpass
+from .core import xpath_store
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/array.py` & `bbrc-pyxnat-1.6/pyxnat/core/array.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-from .jsonutil import JsonTable
-
-
-class ArrayData(object):
-
-    def __init__(self, interface):
-        self._intf = interface
-
-    def _get_array(self, query_string, project_id=None,
-                   subject_id=None, subject_label=None,
-                   experiment_id=None, experiment_label=None,
-                   experiment_type='xnat:subjectAssessorData',
-                   columns=None, constraints=None
-                   ):
-
-        if constraints is None:
-            constraints = {}
-
-        uri = '%s/experiments?xsiType=%s' % (self._intf._get_entry_point(),
-                                             experiment_type)
-
-        if project_id is not None:
-            uri += '&project=%s' % project_id
-
-        if subject_id is not None:
-            uri += '&%s/subject_id=%s' % (experiment_type, subject_id)
-
-        # Subject Label is only held in the xnat:subjectData so look for it
-        # there. This should join against whatever the experiment type is.
-        if subject_label is not None:
-            uri += '&xnat:subjectData/label=%s' % (subject_label)
-
-        if experiment_id is not None:
-            uri += '&ID=%s' % experiment_id
-
-        if experiment_label is not None:
-            uri += '&label=%s' % experiment_label
-
-        uri += query_string
-
-        if constraints != {}:
-            uri += ',' + ','.join(constraints.keys())
-
-        if columns is not None:
-            uri += ',' + ','.join(columns)
-
-        c = {}
-
-        [c.setdefault(key.lower(), value)
-         for key, value in constraints.items()
-         ]
-
-        return JsonTable(self._intf._get_json(uri)).where(**c)
-
-    def experiments(self, project_id=None, subject_id=None, subject_label=None,
-                    experiment_id=None, experiment_label=None,
-                    experiment_type='xnat:subjectAssessorData',
-                    columns=None,
-                    constraints=None):
-
-        """ Returns a list of all visible experiment IDs of the specified
-            type, filtered by optional constraints.
-
-            Parameters
-            ----------
-            project_id: string
-                Name pattern to filter by project ID.
-            subject_id: string
-                Name pattern to filter by subject ID.
-            subject_label: string
-                Name pattern to filter by subject ID.
-            experiment_id: string
-                Name pattern to filter by experiment ID.
-            experiment_label: string
-                Name pattern to filter by experiment ID.
-            experiment_type: string
-                xsi path type; e.g. 'xnat:mrSessionData'
-            columns: list
-                Values to return.
-            constraints: dict
-                Dictionary of xsi_type (key--) and parameter (--value)
-                pairs by which to filter.
-            """
-
-        query_string = '&columns=ID,project,%s/subject_id' % experiment_type
-
-        return self._get_array(query_string, project_id,
-                               subject_id, subject_label,
-                               experiment_id, experiment_label,
-                               experiment_type, columns, constraints
-                               )
-
-    def mrsessions(self, project_id=None, subject_id=None, subject_label=None,
-                   experiment_id=None, experiment_label=None,
-                   columns=None,
-                   constraints=None):
-
-        """ Returns a list of all MR sessions, filtered by optional constraints.
-
-            Parameters
-            ----------
-            project_id: string
-                Name pattern to filter by project ID.
-            subject_id: string
-                Name pattern to filter by subject ID.
-            subject_label: string
-                Name pattern to filter by subject ID.
-            experiment_id: string
-                Name pattern to filter by experiment ID.
-            experiment_label: string
-                Name pattern to filter by experiment ID.
-            columns: list
-                Values to return.
-            constraints: dict
-                Dictionary of xsi_type (key--) and parameter (--value)
-                pairs by which to filter.
-            """
-
-        return self.experiments(project_id, subject_id, subject_label,
-                                experiment_id, experiment_label,
-                                'xnat:mrSessionData', columns, constraints
-                                )
-
-    def scans(self, project_id=None, subject_id=None, subject_label=None,
-              experiment_id=None, experiment_label=None,
-              experiment_type='xnat:imageSessionData',
-              scan_type='xnat:imageScanData',
-              columns=None,
-              constraints=None
-              ):
-
-        """ Returns a list of all visible scan IDs of the specified type,
-            filtered by optional constraints.
-
-            Parameters
-            ----------
-            project_id: string
-                Name pattern to filter by project ID.
-            subject_id: string
-                Name pattern to filter by subject ID.
-            subject_label: string
-                Name pattern to filter by subject ID.
-            experiment_id: string
-                Name pattern to filter by experiment ID.
-            experiment_label: string
-                Name pattern to filter by experiment ID.
-            experiment_type: string
-                xsi path type; e.g. 'xnat:mrSessionData'
-            scan_type: string
-                xsi path type; e.g. 'xnat:mrScanData', etc.
-            columns: list
-                Values to return.
-            constraints: dict
-                Dictionary of xsi_type (key--) and parameter (--value)
-                pairs by which to filter.
-            """
-
-        query_string = '&columns=ID,project,%s/subject_id,%s/ID' % (
-            experiment_type, scan_type)
-
-        array = self._get_array(query_string, project_id,
-                                subject_id, subject_label,
-                                experiment_id, experiment_label,
-                                experiment_type, columns, constraints)
-        id_key = ('%s/ID' % scan_type).lower()
-        return JsonTable([i for i in array if i[id_key]])
-
-    def mrscans(self, project_id=None, subject_id=None, subject_label=None,
-                experiment_id=None, experiment_label=None,
-                columns=None,
-                constraints=None):
-
-        """ Returns a list of all MR scans, filtered by optional constraints.
-
-            Parameters
-            ----------
-            project_id: string
-                Name pattern to filter by project ID.
-            subject_id: string
-                Name pattern to filter by subject ID.
-            subject_label: string
-                Name pattern to filter by subject ID.
-            experiment_id: string
-                Name pattern to filter by experiment ID.
-            experiment_label: string
-                Name pattern to filter by experiment ID.
-            columns: list
-                Values to return.
-            constraints: dict
-                Dictionary of xsi_type (key--) and parameter (--value)
-                pairs by which to filter.
-            """
-
-        return self.scans(project_id, subject_id, subject_label,
-                          experiment_id, experiment_label,
-                          'xnat:mrSessionData', 'xnat:mrScanData',
-                          columns, constraints
-                          )
-
-    def search_experiments(self,
-                           project_id=None,
-                           subject_id=None,
-                           subject_label=None,
-                           experiment_type='xnat:subjectAssessorData',
-                           columns=None,
-                           constraints=None
-                           ):
-
-        """ Returns a list of all visible experiment IDs of the
-            specified type, filtered by optional constraints. This
-            function is a shortcut using the search engine.
-
-            Parameters
-            ----------
-            project_id: string
-                Name pattern to filter by project ID.
-            subject_id: string
-                Name pattern to filter by subject ID.
-            subject_label: string
-                Name pattern to filter by subject ID.
-            experiment_type: string
-                xsi path type must be a leaf session type.
-                defaults to 'xnat:mrSessionData'
-            columns: List[string]
-                list of xsi paths for names of columns to return.
-            constraints: list[(tupple)]
-                List of tupples for comparison in the form (key, comparison,
-                value) valid comparisons are: =, <, <=,>,>=, LIKE
-            """
-
-        if columns is None:
-            columns = []
-
-        where_clause = []
-
-        if project_id is not None:
-            item = ('%s/project' % experiment_type, "=", project_id)
-            where_clause.append(item)
-        if subject_id is not None:
-            where_clause.append(('xnat:subjectData/ID', "=", subject_id))
-        if subject_label is not None:
-            where_clause.append(('xnat:subjectData/LABEL', "=", subject_label))
-
-        if constraints is not None:
-            where_clause.extend(constraints)
-
-        if where_clause != []:
-            where_clause.append('AND')
-
-        if where_clause != []:
-            sel = self._intf.select(experiment_type, columns=columns)
-            table = sel.where(where_clause)
-            return table
-        else:
-            table = self._intf.select(experiment_type, columns=columns)
-            return table.all()
+from .jsonutil import JsonTable
+
+
+class ArrayData(object):
+
+    def __init__(self, interface):
+        self._intf = interface
+
+    def _get_array(self, query_string, project_id=None,
+                   subject_id=None, subject_label=None,
+                   experiment_id=None, experiment_label=None,
+                   experiment_type='xnat:subjectAssessorData',
+                   columns=None, constraints=None
+                   ):
+
+        if constraints is None:
+            constraints = {}
+
+        uri = '%s/experiments?xsiType=%s' % (self._intf._get_entry_point(),
+                                             experiment_type)
+
+        if project_id is not None:
+            uri += '&project=%s' % project_id
+
+        if subject_id is not None:
+            uri += '&%s/subject_id=%s' % (experiment_type, subject_id)
+
+        # Subject Label is only held in the xnat:subjectData so look for it
+        # there. This should join against whatever the experiment type is.
+        if subject_label is not None:
+            uri += '&xnat:subjectData/label=%s' % (subject_label)
+
+        if experiment_id is not None:
+            uri += '&ID=%s' % experiment_id
+
+        if experiment_label is not None:
+            uri += '&label=%s' % experiment_label
+
+        uri += query_string
+
+        if constraints != {}:
+            uri += ',' + ','.join(constraints.keys())
+
+        if columns is not None:
+            uri += ',' + ','.join(columns)
+
+        c = {}
+
+        [c.setdefault(key.lower(), value)
+         for key, value in constraints.items()
+         ]
+
+        return JsonTable(self._intf._get_json(uri)).where(**c)
+
+    def experiments(self, project_id=None, subject_id=None, subject_label=None,
+                    experiment_id=None, experiment_label=None,
+                    experiment_type='xnat:subjectAssessorData',
+                    columns=None,
+                    constraints=None):
+
+        """ Returns a list of all visible experiment IDs of the specified
+            type, filtered by optional constraints.
+
+            Parameters
+            ----------
+            project_id: string
+                Name pattern to filter by project ID.
+            subject_id: string
+                Name pattern to filter by subject ID.
+            subject_label: string
+                Name pattern to filter by subject ID.
+            experiment_id: string
+                Name pattern to filter by experiment ID.
+            experiment_label: string
+                Name pattern to filter by experiment ID.
+            experiment_type: string
+                xsi path type; e.g. 'xnat:mrSessionData'
+            columns: list
+                Values to return.
+            constraints: dict
+                Dictionary of xsi_type (key--) and parameter (--value)
+                pairs by which to filter.
+            """
+
+        query_string = '&columns=ID,project,%s/subject_id' % experiment_type
+
+        return self._get_array(query_string, project_id,
+                               subject_id, subject_label,
+                               experiment_id, experiment_label,
+                               experiment_type, columns, constraints
+                               )
+
+    def mrsessions(self, project_id=None, subject_id=None, subject_label=None,
+                   experiment_id=None, experiment_label=None,
+                   columns=None,
+                   constraints=None):
+
+        """ Returns a list of all MR sessions, filtered by optional constraints.
+
+            Parameters
+            ----------
+            project_id: string
+                Name pattern to filter by project ID.
+            subject_id: string
+                Name pattern to filter by subject ID.
+            subject_label: string
+                Name pattern to filter by subject ID.
+            experiment_id: string
+                Name pattern to filter by experiment ID.
+            experiment_label: string
+                Name pattern to filter by experiment ID.
+            columns: list
+                Values to return.
+            constraints: dict
+                Dictionary of xsi_type (key--) and parameter (--value)
+                pairs by which to filter.
+            """
+
+        return self.experiments(project_id, subject_id, subject_label,
+                                experiment_id, experiment_label,
+                                'xnat:mrSessionData', columns, constraints
+                                )
+
+    def scans(self, project_id=None, subject_id=None, subject_label=None,
+              experiment_id=None, experiment_label=None,
+              experiment_type='xnat:imageSessionData',
+              scan_type='xnat:imageScanData',
+              columns=None,
+              constraints=None
+              ):
+
+        """ Returns a list of all visible scan IDs of the specified type,
+            filtered by optional constraints.
+
+            Parameters
+            ----------
+            project_id: string
+                Name pattern to filter by project ID.
+            subject_id: string
+                Name pattern to filter by subject ID.
+            subject_label: string
+                Name pattern to filter by subject ID.
+            experiment_id: string
+                Name pattern to filter by experiment ID.
+            experiment_label: string
+                Name pattern to filter by experiment ID.
+            experiment_type: string
+                xsi path type; e.g. 'xnat:mrSessionData'
+            scan_type: string
+                xsi path type; e.g. 'xnat:mrScanData', etc.
+            columns: list
+                Values to return.
+            constraints: dict
+                Dictionary of xsi_type (key--) and parameter (--value)
+                pairs by which to filter.
+            """
+
+        query_string = '&columns=ID,project,%s/subject_id,%s/ID' % (
+            experiment_type, scan_type)
+
+        array = self._get_array(query_string, project_id,
+                                subject_id, subject_label,
+                                experiment_id, experiment_label,
+                                experiment_type, columns, constraints)
+        id_key = ('%s/ID' % scan_type).lower()
+        return JsonTable([i for i in array if i[id_key]])
+
+    def mrscans(self, project_id=None, subject_id=None, subject_label=None,
+                experiment_id=None, experiment_label=None,
+                columns=None,
+                constraints=None):
+
+        """ Returns a list of all MR scans, filtered by optional constraints.
+
+            Parameters
+            ----------
+            project_id: string
+                Name pattern to filter by project ID.
+            subject_id: string
+                Name pattern to filter by subject ID.
+            subject_label: string
+                Name pattern to filter by subject ID.
+            experiment_id: string
+                Name pattern to filter by experiment ID.
+            experiment_label: string
+                Name pattern to filter by experiment ID.
+            columns: list
+                Values to return.
+            constraints: dict
+                Dictionary of xsi_type (key--) and parameter (--value)
+                pairs by which to filter.
+            """
+
+        return self.scans(project_id, subject_id, subject_label,
+                          experiment_id, experiment_label,
+                          'xnat:mrSessionData', 'xnat:mrScanData',
+                          columns, constraints
+                          )
+
+    def search_experiments(self,
+                           project_id=None,
+                           subject_id=None,
+                           subject_label=None,
+                           experiment_type='xnat:subjectAssessorData',
+                           columns=None,
+                           constraints=None
+                           ):
+
+        """ Returns a list of all visible experiment IDs of the
+            specified type, filtered by optional constraints. This
+            function is a shortcut using the search engine.
+
+            Parameters
+            ----------
+            project_id: string
+                Name pattern to filter by project ID.
+            subject_id: string
+                Name pattern to filter by subject ID.
+            subject_label: string
+                Name pattern to filter by subject ID.
+            experiment_type: string
+                xsi path type must be a leaf session type.
+                defaults to 'xnat:mrSessionData'
+            columns: List[string]
+                list of xsi paths for names of columns to return.
+            constraints: list[(tupple)]
+                List of tupples for comparison in the form (key, comparison,
+                value) valid comparisons are: =, <, <=,>,>=, LIKE
+            """
+
+        if columns is None:
+            columns = []
+
+        where_clause = []
+
+        if project_id is not None:
+            item = ('%s/project' % experiment_type, "=", project_id)
+            where_clause.append(item)
+        if subject_id is not None:
+            where_clause.append(('xnat:subjectData/ID', "=", subject_id))
+        if subject_label is not None:
+            where_clause.append(('xnat:subjectData/LABEL', "=", subject_label))
+
+        if constraints is not None:
+            where_clause.extend(constraints)
+
+        if where_clause != []:
+            where_clause.append('AND')
+
+        if where_clause != []:
+            sel = self._intf.select(experiment_type, columns=columns)
+            table = sel.where(where_clause)
+            return table
+        else:
+            table = self._intf.select(experiment_type, columns=columns)
+            return table.all()
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/__init__.py` & `bbrc-pyxnat-1.6/pyxnat/core/derivatives/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Since pyxnat v1.2.1.0.post3, we introduced a mechanism to tune these objects
-# and allow adding custom functions for specific types of resources.
-#
-# For instance, one could now directly write:
-#
-# resource = experiment.resource('FREESURFER6')
-# aparc = resource.aparc()
-# aseg = resource.aseg()
-# and thus get access to FreeSurfer measurements.
-#
-# Another example, with the ASHS pipeline for hippocampal subfield
-# segmentation:
-#
-# resource = experiment.resource('ASHS')
-# volumes = resource.volumes()
-#
-# Again, this would only work provided that corresponding resources respect a
-# certain naming and structure on XNAT. Here in this present example,
-# FreeSurfer results are stored in resources called FREESURFER6 and the whole
-# FreeSurfer folder (named after the subject) is stored in the resource.
-# Having access to such additional functions would be conditioned by the
-# existence of these resources with proper matching structure.
-#
-# Nevertheless, this mechanism has been implemented so as to get easily adapted
-# to local configurations, by editing/adding this very same folder.
-#
-# Adding a custom function can be done simply as follows.
-#
-# In this same folder (pyxnat/core/derivatives/), edit any existing file or add
-# a new one (filename does not matter):
-#
-# Define XNAT_RESOURCE_NAME. This variable names the XNAT resource which needs
-# a custom function.
-# Write the custom function with self as first parameter (self will be the
-# pyxnat Resource object).
-# If the resources which the custom function should be added has multiple names
-# instead of a single one, their list may be provided under the variable
-# XNAT_RESOURCE_NAMES.
-#
-# An example is provided in pyxnat/core/derivatives/ashs.py
+# Since pyxnat v1.2.1.0.post3, we introduced a mechanism to tune these objects
+# and allow adding custom functions for specific types of resources.
+#
+# For instance, one could now directly write:
+#
+# resource = experiment.resource('FREESURFER6')
+# aparc = resource.aparc()
+# aseg = resource.aseg()
+# and thus get access to FreeSurfer measurements.
+#
+# Another example, with the ASHS pipeline for hippocampal subfield
+# segmentation:
+#
+# resource = experiment.resource('ASHS')
+# volumes = resource.volumes()
+#
+# Again, this would only work provided that corresponding resources respect a
+# certain naming and structure on XNAT. Here in this present example,
+# FreeSurfer results are stored in resources called FREESURFER6 and the whole
+# FreeSurfer folder (named after the subject) is stored in the resource.
+# Having access to such additional functions would be conditioned by the
+# existence of these resources with proper matching structure.
+#
+# Nevertheless, this mechanism has been implemented so as to get easily adapted
+# to local configurations, by editing/adding this very same folder.
+#
+# Adding a custom function can be done simply as follows.
+#
+# In this same folder (pyxnat/core/derivatives/), edit any existing file or add
+# a new one (filename does not matter):
+#
+# Define XNAT_RESOURCE_NAME. This variable names the XNAT resource which needs
+# a custom function.
+# Write the custom function with self as first parameter (self will be the
+# pyxnat Resource object).
+# If the resources which the custom function should be added has multiple names
+# instead of a single one, their list may be provided under the variable
+# XNAT_RESOURCE_NAMES.
+#
+# An example is provided in pyxnat/core/derivatives/ashs.py
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/bamos.py` & `bbrc-pyxnat-1.6/pyxnat/core/derivatives/bamos.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,224 +1,224 @@
-import os
-import nibabel as nib
-import tempfile
-import numpy as np
-import pandas as pd
-
-XNAT_RESOURCE_NAME = 'BAMOS'
-
-BAMOS_LABELS = {0: 'background',
-                1: 'left frontal',
-                2: 'right frontal',
-                3: 'left parietal',
-                4: 'right parietal',
-                5: 'left occipital',
-                6: 'right occipital',
-                7: 'left temporal',
-                8: 'right temporal',
-                9: 'basal ganglia',
-                10: 'infratentorial'}
-
-
-def volume(self):
-    """ Returns the estimated volume of the identified lesions (i.e. voxels
-    with a value higher than 0.5."""
-
-    fd, fp = tempfile.mkstemp(suffix='.nii.gz')
-    os.close(fd)
-
-    f = list(self.files('CorrectLesion_*nii.gz'))[0]
-    f.get(fp)
-    d = nib.load(fp)
-    size = np.prod(d.header['pixdim'].tolist()[:4])
-    n = np.array(d.dataobj)
-    v = np.sum(n[n >= 0.5]) * size
-    os.remove(fp)
-    return v
-
-
-def n_lesions(self):
-    """ Returns the estimated number of lesions i.e. the # of found connected
-    components in Connect_WS3WT3WC1Lesion*_corr.nii.gz. """
-
-    fd, fp = tempfile.mkstemp(suffix='.nii.gz')
-    os.close(fd)
-
-    f = list(self.files('Connect_WS3WT3WC1Lesion_*_corr.nii.gz'))[0]
-    f.get(fp)
-    d = nib.load(fp)
-    n = len(np.unique(d.dataobj))
-
-    os.remove(fp)
-    return n
-
-
-def stats(self):
-    """ Collects descriptive statistics based on the segmented lesions of the
-    white matter, including volumes and number of lesions. A voxel is
-    considered as a part of a lesion if it has a value higher than 0.5."""
-    def _download_data_(self):
-        fd, fp = tempfile.mkstemp(suffix='.nii.gz')
-        os.close(fd)
-
-        f = list(self.files('Connect_WS3WT3WC1Lesion_*_corr.nii.gz'))[0]
-        f.get(fp)
-        cc = np.array(nib.load(fp).dataobj)
-        f = list(self.files('CorrectLesion_*nii.gz'))[0]
-        f.get(fp)
-        d = nib.load(fp)
-        size = np.prod(d.header['pixdim'].tolist()[:4])
-        les = np.array(d.dataobj)
-
-        f = list(self.files('Layers_*.nii.gz'))[0]
-        f.get(fp)
-        d1 = np.array(nib.load(fp).dataobj)
-
-        f = list(self.files('Lobes_*.nii.gz'))[0]
-        f.get(fp)
-        d2 = np.array(nib.load(fp).dataobj)
-        os.remove(fp)
-        return cc, d1, d2, les, size
-
-    def _roistats_from_map(m, atlas1, atlas2, func=np.mean):
-        import itertools
-        assert(m.shape == atlas1.shape)
-        assert(m.shape == atlas2.shape)
-        labels1 = list(np.unique(atlas1))
-        labels2 = list(np.unique(atlas2))
-
-        combinations = list(itertools.product(labels1, labels2))
-
-        mask = lambda i1, i2: (atlas1 == i1) & (atlas2 == i2)
-        label_values = dict([((i1, BAMOS_LABELS[i2]), func(m[mask(i1, i2)]))
-                             for (i1, i2) in combinations])
-        return label_values
-
-
-    cc, d1, d2, les, size = _download_data_(self)
-    d1[d1 == 5] = 4  # Merging layer 5 with layer 4
-
-    stats1 = _roistats_from_map(cc, d1, d2, func=lambda d: len(np.unique(d)))
-    stats2 = _roistats_from_map(les, d1, d2, func=lambda d: np.sum(d[d >= 0.5]))
-
-    df = [(d, r, val, stats2[(d, r)] * size) for (d, r), val in stats1.items()]
-    df = pd.DataFrame(df, columns=['depth', 'region', 'n', 'volume'])
-
-    return df
-
-
-def bullseye_plot(self, ax=None, figsize=(12, 8), segBold=[],
-                  measurement='volume', stats=None, cm=None):
-    """
-    Bullseye's representation of cerebral white matter hyperintensities
-    (adapted from https://matplotlib.org/stable/gallery/specialty_plots/leftventricle_bulleye.html)
-
-    Args:
-    `ax`          If None then a new Matplotlib figure is created
-    `figsize`     Figure size
-    `segBold`     Highlight some sections (if an integer is passed then will
-                   highlight the regions over the given nth percentile)
-    `measurement` Measurement to plot (default: `volume`)
-    `stats`       Can be used to plot precalculated stats. (default: None -
-                   stats will be calculated for the current resource)
-    `cm`          Color map (default: `matplotlib.pyplot.cm.YlOrRd`)
-
-    Reference:
-    C. Sudre et al., J Neuroradiol, 2018
-    """
-    from matplotlib import pyplot as plt
-    import matplotlib as mpl
-
-    num = 80   # sampling parameter
-    nreg = 10  # how many regions
-    ndep = 4   # how many layers
-    offset = 18 * np.pi/180  # in radians
-    ordered_labels = [3, 1, 2, 4, 8, 6, 10, 9, 5, 7]
-
-    def _ravel_stats_(stats, measurement='n'):
-        data = []
-        for d in range(1, ndep+1):
-            for label in ordered_labels:
-                q = 'depth == %s & region == "%s"' % (d, BAMOS_LABELS[label])
-                v = float(stats.query(q)[measurement])
-                data.append(v)
-        return data
-
-    if stats is None:
-        stats = self.stats()
-
-    layers = [int(e) for e in set(stats['depth'])][1:]  # remove 0 (background)
-
-    # Highlight regions > nth percentile
-    if isinstance(segBold, int):
-        pc = stats[measurement].quantile(q=segBold/100.0)
-        segBold = []
-        for _, r in stats.query('%s > @pc' % measurement).iterrows():
-            label = [k for (k, v) in BAMOS_LABELS.items() if v == r.region][0]
-            idx = ordered_labels.index(label)
-            segBold.append((int(r.depth)-1, idx))
-
-    data = _ravel_stats_(stats, measurement=measurement)
-
-    # Start plotting
-    data = np.array(data).ravel()
-    vlim = [data.min(), data.max()]
-    if cm is None:
-        cm = plt.cm.YlOrRd
-
-    axnone = ax is None
-    if axnone:
-        fig, ax = plt.subplots(subplot_kw=dict(projection='polar'),
-                               figsize=figsize)
-
-    theta = np.linspace(0, 2*np.pi, num*nreg)
-    r = np.linspace(0.2, 1, ndep+1)
-
-    # Draw circles
-    linewidth = 1
-    for i in range(r.shape[0]):
-        ax.plot(theta, np.repeat(r[i], theta.shape), '-k', lw=linewidth)
-
-    # Draw lines
-    for i in range(nreg):
-        theta_i = (i * 360.0/nreg) * np.pi/180 + offset
-        ax.plot([theta_i, theta_i], [r[0], 1], '-k', lw=linewidth)
-
-    # Paint areas
-    for depth in range(ndep):
-        r0 = r[depth:depth+2]
-        r0 = np.repeat(r0[:, np.newaxis], num, axis=1).T
-        for i in range(nreg):
-            theta0 = theta[i*num:(i+1)*num] + offset
-            theta0 = np.repeat(theta0[:, np.newaxis], 2, axis=1)
-            z = np.ones((num, 2)) * data[depth*nreg + i]
-            ax.pcolormesh(theta0, r0, z, vmin=vlim[0], vmax=vlim[1], cmap=cm)
-
-            # Highlight some regions
-            if (depth, i) in segBold:
-                ax.plot(theta0, r0, '-k', lw=linewidth+2)
-                ax.plot(theta0[0], [r[depth], r[depth+1]], '-k', lw=linewidth+1)
-                ax.plot(theta0[-1], [r[depth], r[depth+1]], '-k', lw=linewidth+1)
-
-    ax.set_ylim([0, 1])
-    ax.set_yticklabels(layers)
-
-    thetaticks = np.arange(0, 360, 36)
-    ordered_labels = [7, 3, 1, 2, 4, 8, 6, 10, 9, 5]
-
-    labels = [BAMOS_LABELS[e] for e in ordered_labels]
-    ax.set_thetagrids(thetaticks, labels=labels)
-    ax.tick_params(pad=12, labelsize=14, axis='both')
-    bbox = dict(boxstyle="round", ec="white", fc="white", alpha=0.5)
-    plt.setp(ax.get_xticklabels(), bbox=bbox)
-
-    if axnone:  # Add legend
-        cNorm = mpl.colors.Normalize(vmin=vlim[0], vmax=vlim[1])
-
-        ax = fig.add_axes([0.3, 0.04, 0.45, 0.05])
-        ticks = [vlim[0], 0, vlim[1]]
-        cb = mpl.colorbar.ColorbarBase(ax, cmap=cm, norm=cNorm,
-                                       orientation='horizontal', ticks=ticks)
-    plt.show()
-
-    if axnone:
-        return fig, ax
+import os
+import nibabel as nib
+import tempfile
+import numpy as np
+import pandas as pd
+
+XNAT_RESOURCE_NAME = 'BAMOS'
+
+BAMOS_LABELS = {0: 'background',
+                1: 'left frontal',
+                2: 'right frontal',
+                3: 'left parietal',
+                4: 'right parietal',
+                5: 'left occipital',
+                6: 'right occipital',
+                7: 'left temporal',
+                8: 'right temporal',
+                9: 'basal ganglia',
+                10: 'infratentorial'}
+
+
+def volume(self):
+    """ Returns the estimated volume of the identified lesions (i.e. voxels
+    with a value higher than 0.5."""
+
+    fd, fp = tempfile.mkstemp(suffix='.nii.gz')
+    os.close(fd)
+
+    f = list(self.files('CorrectLesion_*nii.gz'))[0]
+    f.get(fp)
+    d = nib.load(fp)
+    size = np.prod(d.header['pixdim'].tolist()[:4])
+    n = np.array(d.dataobj)
+    v = np.sum(n[n >= 0.5]) * size
+    os.remove(fp)
+    return v
+
+
+def n_lesions(self):
+    """ Returns the estimated number of lesions i.e. the # of found connected
+    components in Connect_WS3WT3WC1Lesion*_corr.nii.gz. """
+
+    fd, fp = tempfile.mkstemp(suffix='.nii.gz')
+    os.close(fd)
+
+    f = list(self.files('Connect_WS3WT3WC1Lesion_*_corr.nii.gz'))[0]
+    f.get(fp)
+    d = nib.load(fp)
+    n = len(np.unique(d.dataobj))
+
+    os.remove(fp)
+    return n
+
+
+def stats(self):
+    """ Collects descriptive statistics based on the segmented lesions of the
+    white matter, including volumes and number of lesions. A voxel is
+    considered as a part of a lesion if it has a value higher than 0.5."""
+    def _download_data_(self):
+        fd, fp = tempfile.mkstemp(suffix='.nii.gz')
+        os.close(fd)
+
+        f = list(self.files('Connect_WS3WT3WC1Lesion_*_corr.nii.gz'))[0]
+        f.get(fp)
+        cc = np.array(nib.load(fp).dataobj)
+        f = list(self.files('CorrectLesion_*nii.gz'))[0]
+        f.get(fp)
+        d = nib.load(fp)
+        size = np.prod(d.header['pixdim'].tolist()[:4])
+        les = np.array(d.dataobj)
+
+        f = list(self.files('Layers_*.nii.gz'))[0]
+        f.get(fp)
+        d1 = np.array(nib.load(fp).dataobj)
+
+        f = list(self.files('Lobes_*.nii.gz'))[0]
+        f.get(fp)
+        d2 = np.array(nib.load(fp).dataobj)
+        os.remove(fp)
+        return cc, d1, d2, les, size
+
+    def _roistats_from_map(m, atlas1, atlas2, func=np.mean):
+        import itertools
+        assert(m.shape == atlas1.shape)
+        assert(m.shape == atlas2.shape)
+        labels1 = list(np.unique(atlas1))
+        labels2 = list(np.unique(atlas2))
+
+        combinations = list(itertools.product(labels1, labels2))
+
+        mask = lambda i1, i2: (atlas1 == i1) & (atlas2 == i2)
+        label_values = dict([((i1, BAMOS_LABELS[i2]), func(m[mask(i1, i2)]))
+                             for (i1, i2) in combinations])
+        return label_values
+
+
+    cc, d1, d2, les, size = _download_data_(self)
+    d1[d1 == 5] = 4  # Merging layer 5 with layer 4
+
+    stats1 = _roistats_from_map(cc, d1, d2, func=lambda d: len(np.unique(d)))
+    stats2 = _roistats_from_map(les, d1, d2, func=lambda d: np.sum(d[d >= 0.5]))
+
+    df = [(d, r, val, stats2[(d, r)] * size) for (d, r), val in stats1.items()]
+    df = pd.DataFrame(df, columns=['depth', 'region', 'n', 'volume'])
+
+    return df
+
+
+def bullseye_plot(self, ax=None, figsize=(12, 8), segBold=[],
+                  measurement='volume', stats=None, cm=None):
+    """
+    Bullseye's representation of cerebral white matter hyperintensities
+    (adapted from https://matplotlib.org/stable/gallery/specialty_plots/leftventricle_bulleye.html)
+
+    Args:
+    `ax`          If None then a new Matplotlib figure is created
+    `figsize`     Figure size
+    `segBold`     Highlight some sections (if an integer is passed then will
+                   highlight the regions over the given nth percentile)
+    `measurement` Measurement to plot (default: `volume`)
+    `stats`       Can be used to plot precalculated stats. (default: None -
+                   stats will be calculated for the current resource)
+    `cm`          Color map (default: `matplotlib.pyplot.cm.YlOrRd`)
+
+    Reference:
+    C. Sudre et al., J Neuroradiol, 2018
+    """
+    from matplotlib import pyplot as plt
+    import matplotlib as mpl
+
+    num = 80   # sampling parameter
+    nreg = 10  # how many regions
+    ndep = 4   # how many layers
+    offset = 18 * np.pi/180  # in radians
+    ordered_labels = [3, 1, 2, 4, 8, 6, 10, 9, 5, 7]
+
+    def _ravel_stats_(stats, measurement='n'):
+        data = []
+        for d in range(1, ndep+1):
+            for label in ordered_labels:
+                q = 'depth == %s & region == "%s"' % (d, BAMOS_LABELS[label])
+                v = float(stats.query(q)[measurement])
+                data.append(v)
+        return data
+
+    if stats is None:
+        stats = self.stats()
+
+    layers = [int(e) for e in set(stats['depth'])][1:]  # remove 0 (background)
+
+    # Highlight regions > nth percentile
+    if isinstance(segBold, int):
+        pc = stats[measurement].quantile(q=segBold/100.0)
+        segBold = []
+        for _, r in stats.query('%s > @pc' % measurement).iterrows():
+            label = [k for (k, v) in BAMOS_LABELS.items() if v == r.region][0]
+            idx = ordered_labels.index(label)
+            segBold.append((int(r.depth)-1, idx))
+
+    data = _ravel_stats_(stats, measurement=measurement)
+
+    # Start plotting
+    data = np.array(data).ravel()
+    vlim = [data.min(), data.max()]
+    if cm is None:
+        cm = plt.cm.YlOrRd
+
+    axnone = ax is None
+    if axnone:
+        fig, ax = plt.subplots(subplot_kw=dict(projection='polar'),
+                               figsize=figsize)
+
+    theta = np.linspace(0, 2*np.pi, num*nreg)
+    r = np.linspace(0.2, 1, ndep+1)
+
+    # Draw circles
+    linewidth = 1
+    for i in range(r.shape[0]):
+        ax.plot(theta, np.repeat(r[i], theta.shape), '-k', lw=linewidth)
+
+    # Draw lines
+    for i in range(nreg):
+        theta_i = (i * 360.0/nreg) * np.pi/180 + offset
+        ax.plot([theta_i, theta_i], [r[0], 1], '-k', lw=linewidth)
+
+    # Paint areas
+    for depth in range(ndep):
+        r0 = r[depth:depth+2]
+        r0 = np.repeat(r0[:, np.newaxis], num, axis=1).T
+        for i in range(nreg):
+            theta0 = theta[i*num:(i+1)*num] + offset
+            theta0 = np.repeat(theta0[:, np.newaxis], 2, axis=1)
+            z = np.ones((num, 2)) * data[depth*nreg + i]
+            ax.pcolormesh(theta0, r0, z, vmin=vlim[0], vmax=vlim[1], cmap=cm)
+
+            # Highlight some regions
+            if (depth, i) in segBold:
+                ax.plot(theta0, r0, '-k', lw=linewidth+2)
+                ax.plot(theta0[0], [r[depth], r[depth+1]], '-k', lw=linewidth+1)
+                ax.plot(theta0[-1], [r[depth], r[depth+1]], '-k', lw=linewidth+1)
+
+    ax.set_ylim([0, 1])
+    ax.set_yticklabels(layers)
+
+    thetaticks = np.arange(0, 360, 36)
+    ordered_labels = [7, 3, 1, 2, 4, 8, 6, 10, 9, 5]
+
+    labels = [BAMOS_LABELS[e] for e in ordered_labels]
+    ax.set_thetagrids(thetaticks, labels=labels)
+    ax.tick_params(pad=12, labelsize=14, axis='both')
+    bbox = dict(boxstyle="round", ec="white", fc="white", alpha=0.5)
+    plt.setp(ax.get_xticklabels(), bbox=bbox)
+
+    if axnone:  # Add legend
+        cNorm = mpl.colors.Normalize(vmin=vlim[0], vmax=vlim[1])
+
+        ax = fig.add_axes([0.3, 0.04, 0.45, 0.05])
+        ticks = [vlim[0], 0, vlim[1]]
+        cb = mpl.colorbar.ColorbarBase(ax, cmap=cm, norm=cNorm,
+                                       orientation='horizontal', ticks=ticks)
+    plt.show()
+
+    if axnone:
+        return fig, ax
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/basil.py` & `bbrc-pyxnat-1.6/pyxnat/core/derivatives/basil.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-XNAT_RESOURCE_NAMES = ['BASIL']
-
-
-def volumes(self):
-    """Partial volume segmentations for CSF, GM, WM (fsl_anat)"""
-    import os
-    import tempfile
-    import nibabel as nib
-    import numpy as np
-
-    vols = []
-    fd, fp = tempfile.mkstemp(suffix='.nii.gz')
-    os.close(fd)
-
-    names = ['T1_fast_pve_0', 'T1_fast_pve_1', 'T1_fast_pve_2']
-    for kls in names:
-        f = self.files('*{}*'.format(kls))[0]
-        f.get(fp)
-        d = nib.load(fp)
-        size = np.prod(d.header['pixdim'].tolist()[:4])
-        v = np.sum(d.dataobj) * size
-        vols.append((kls, v))
-
-    os.remove(fp)
-    return dict(vols)
-
-
-def perfusion(self):
-    """Perfusion and arrival-time mean values"""
-    import pandas as pd
-
-    def _fix_label(label):
-        """Some BASIL mean files have typos in their names. This helper
-        fixes them so they are consistent with the measurement represented."""
-
-        d = {'arrival_wm_wm_mean': 'arrival_wm_mean',
-             'perfusion_wm_wm_mean': 'perfusion_wm_mean',
-             'perfusion_wm_calib_wm_mean': 'perfusion_calib_wm_mean'}
-
-        return d.get(label, label)
-
-    data = []
-
-    mean_files = [f for f in list(self.files('native_space/*.txt'))]
-    for f in mean_files:
-        fp = f.attributes()['path']
-        key = _fix_label(f.attributes()['Name'].split('.txt')[0])
-        pvcorr = ('pvcorr' in fp)
-        value = float(self._intf.get(f.attributes()['URI']).text.strip())
-
-        data.append([key, pvcorr, value, fp])
-
-    return pd.DataFrame(data, columns=['measurement', 'pvcorr', 'value', 'filepath'])
-
-
-def stats(self):
-    """Summary statistics for the perfusion values within each region
-    in the Harvard-Oxford cortical and subcortical atlases"""
-    import csv
-    import pandas as pd
-    import os.path as op
-
-    region_stats = []
-
-    stats_files = {'whole_brain': 'region_analysis.csv',
-                   'GM': 'region_analysis_gm.csv',
-                   'WM': 'region_analysis_wm.csv'}
-    for roi, fn in stats_files.items():
-        f = self.files('*{}'.format(fn))[0]
-        content = self._intf.get(f.attributes()['URI']).text.splitlines()
-        for idx, ln in enumerate(csv.reader(content)):
-            if idx == 0:
-                cols = ['region_analysis'] + ln
-            elif idx > 0:
-                region_stats.append([roi] + ln)
-
-    df = pd.DataFrame(region_stats, columns=cols)
-    num_cols = ['Nvoxels', 'Mean', 'Std', 'Median',
-                'IQR', 'Precision-weighted mean', 'I2']
-    for col in num_cols:
-        df[col] = pd.to_numeric(df[col])
-    return df
+XNAT_RESOURCE_NAMES = ['BASIL']
+
+
+def volumes(self):
+    """Partial volume segmentations for CSF, GM, WM (fsl_anat)"""
+    import os
+    import tempfile
+    import nibabel as nib
+    import numpy as np
+
+    vols = []
+    fd, fp = tempfile.mkstemp(suffix='.nii.gz')
+    os.close(fd)
+
+    names = ['T1_fast_pve_0', 'T1_fast_pve_1', 'T1_fast_pve_2']
+    for kls in names:
+        f = self.files('*{}*'.format(kls))[0]
+        f.get(fp)
+        d = nib.load(fp)
+        size = np.prod(d.header['pixdim'].tolist()[:4])
+        v = np.sum(d.dataobj) * size
+        vols.append((kls, v))
+
+    os.remove(fp)
+    return dict(vols)
+
+
+def perfusion(self):
+    """Perfusion and arrival-time mean values"""
+    import pandas as pd
+
+    def _fix_label(label):
+        """Some BASIL mean files have typos in their names. This helper
+        fixes them so they are consistent with the measurement represented."""
+
+        d = {'arrival_wm_wm_mean': 'arrival_wm_mean',
+             'perfusion_wm_wm_mean': 'perfusion_wm_mean',
+             'perfusion_wm_calib_wm_mean': 'perfusion_calib_wm_mean'}
+
+        return d.get(label, label)
+
+    data = []
+
+    mean_files = [f for f in list(self.files('native_space/*.txt'))]
+    for f in mean_files:
+        fp = f.attributes()['path']
+        key = _fix_label(f.attributes()['Name'].split('.txt')[0])
+        pvcorr = ('pvcorr' in fp)
+        value = float(self._intf.get(f.attributes()['URI']).text.strip())
+
+        data.append([key, pvcorr, value, fp])
+
+    return pd.DataFrame(data, columns=['measurement', 'pvcorr', 'value', 'filepath'])
+
+
+def stats(self):
+    """Summary statistics for the perfusion values within each region
+    in the Harvard-Oxford cortical and subcortical atlases"""
+    import csv
+    import pandas as pd
+    import os.path as op
+
+    region_stats = []
+
+    stats_files = {'whole_brain': 'region_analysis.csv',
+                   'GM': 'region_analysis_gm.csv',
+                   'WM': 'region_analysis_wm.csv'}
+    for roi, fn in stats_files.items():
+        f = self.files('*{}'.format(fn))[0]
+        content = self._intf.get(f.attributes()['URI']).text.splitlines()
+        for idx, ln in enumerate(csv.reader(content)):
+            if idx == 0:
+                cols = ['region_analysis'] + ln
+            elif idx > 0:
+                region_stats.append([roi] + ln)
+
+    df = pd.DataFrame(region_stats, columns=cols)
+    num_cols = ['Nvoxels', 'Mean', 'Std', 'Median',
+                'IQR', 'Precision-weighted mean', 'I2']
+    for col in num_cols:
+        df[col] = pd.to_numeric(df[col])
+    return df
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/cat12.py` & `bbrc-pyxnat-1.6/pyxnat/core/derivatives/spm12.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-XNAT_RESOURCE_NAME = 'CAT12_SEGMENT'
-
-
-def volumes(self):
-    import os
-    import tempfile
-    import nibabel as nib
-    import numpy as np
-
-    vols = []
-    fd, fp = tempfile.mkstemp(suffix='.nii.gz')
-    os.close(fd)
-
-    names = ['mri/p1', 'mri/p2', 'mri/p3']
-    for kls in names:
-        f = [each for each in self.files() if each.id().startswith(kls)][0]
-        f.get(fp)
-        d = nib.load(fp)
-        size = np.prod(d.header['pixdim'].tolist()[:4])
-        v = np.sum(d.dataobj) * size
-        vols.append((kls, v))
-
-    os.remove(fp)
-    return dict(vols)
-
-
-def download_rc(self, path):
-    '''Downloads a local copy of DARTEL imports. (Keep in mind that in CAT12
-    images are named rp*, not rc*.'''
-    import os.path as op
-    rc_files = ['mri/rp1', 'mri/rp2']
-    for each in rc_files:
-        res = self._intf.array.experiments(experiment_id=self.parent().id(),
-                                           columns=['subject_label']).data[0]
-        subject_label = res['subject_label']
-        id = res['ID']
-        fp = '%s_%s_%s.nii.gz' % (each[-3:], subject_label, id)
-        list(self.files('%s*' % each))[0].get(op.join(path, fp))
+XNAT_RESOURCE_NAMES = ['SPM12_SEGMENT', 'SPM12_SEGMENT_T1T2']
+
+
+def volumes(self):
+    import os
+    import tempfile
+    import nibabel as nib
+    import numpy as np
+
+    vols = []
+    fd, fp = tempfile.mkstemp(suffix='.nii.gz')
+    os.close(fd)
+
+    names = ['c1', 'c2', 'c3']
+    for kls in names:
+        f = [each for each in self.files() if each.id().startswith(kls)][0]
+        f.get(fp)
+        d = nib.load(fp)
+        size = np.prod(d.header['pixdim'].tolist()[:4])
+        v = np.sum(d.dataobj) * size
+        vols.append((kls, v))
+
+    os.remove(fp)
+    return dict(vols)
+
+
+def download_rc(self, path):
+    """Downloads a local copy of DARTEL imports."""
+    import os.path as op
+    rc_files = ['rc1', 'rc2']
+    for each in rc_files:
+        res = self._intf.array.experiments(experiment_id=self.parent().id(),
+                                           columns=['subject_label']).data[0]
+        subject_label = res['subject_label']
+        id = res['ID']
+        fp = '%s_%s_%s.nii.gz' % (each[-3:], subject_label, id)
+        list(self.files('%s*' % each))[0].get(op.join(path, fp))
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/dicom.py` & `bbrc-pyxnat-1.6/pyxnat/core/derivatives/dicom.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-XNAT_RESOURCE_NAME = 'DICOM'
-
-
-def scandate(self):
-    import os.path as op
-    import os
-    import tempfile
-    import pydicom
-    from datetime import datetime
-
-    f = list(self.files())[0]
-
-    fd, fp = tempfile.mkstemp(suffix='.dcm')
-    os.close(fd)
-    f.get(dest=fp)
-    d = pydicom.read_file(fp)
-
-    if hasattr(d, 'AcquisitionDate'):
-        acquisition_date = d.AcquisitionDate
-    else:
-        acquisition_date = d.AcquisitionDateTime[:8]
-
-    os.remove(fp)
-    ad = datetime.strptime(acquisition_date, '%Y%m%d').strftime('%Y-%m-%d')
-    return ad
+XNAT_RESOURCE_NAME = 'DICOM'
+
+
+def scandate(self):
+    import os.path as op
+    import os
+    import tempfile
+    import pydicom
+    from datetime import datetime
+
+    f = list(self.files())[0]
+
+    fd, fp = tempfile.mkstemp(suffix='.dcm')
+    os.close(fd)
+    f.get(dest=fp)
+    d = pydicom.read_file(fp)
+
+    if hasattr(d, 'AcquisitionDate'):
+        acquisition_date = d.AcquisitionDate
+    else:
+        acquisition_date = d.AcquisitionDateTime[:8]
+
+    os.remove(fp)
+    ad = datetime.strptime(acquisition_date, '%Y%m%d').strftime('%Y-%m-%d')
+    return ad
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/freesurfer.py` & `bbrc-pyxnat-1.6/pyxnat/core/derivatives/freesurfer.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-XNAT_RESOURCE_NAMES = ['FREESURFER6', 'FREESURFER6_HIRES', 'FREESURFER7']
-
-
-def amygNucVolumes(self, mode='T1'):
-    """Returns amygdala nuclei volumetry as estimated by FreeSurfer
-    `recon-all`."""
-    import pandas as pd
-
-    if self.label().startswith('FREESURFER6'):
-        raise NotImplementedError('Not available in FreeSurfer 6')
-
-    table = []
-    files = list(self.files('*h.amygNucVolumes-%s.v*.txt' % mode))
-    for f in files:
-        uri = f._uri
-
-        res = self._intf.get(uri).text.split('\n')
-        d1 = dict([each.split(' ') for each in res[:-1]])
-        d2 = dict([('%s' % k, float(v))
-                  for k, v in d1.items()])
-
-        side = {'l': 'left', 'r': 'right'}[uri.split('/')[-1][0]]
-        for region, value in d2.items():
-            row = [side, region, value]
-            table.append(row)
-
-    columns = ['side', 'region', 'value']
-    return pd.DataFrame(table, columns=columns)
-
-
-def hippoSfVolumes(self, mode='T1'):
-    """Returns hippocampal subfield volumetry as estimated by FreeSurfer
-    `recon-all`."""
-    import pandas as pd
-
-    table = []
-    files = list(self.files('*h.hippoSfVolumes-%s.v*.txt' % mode))
-    for f in files:
-        uri = f._uri
-
-        res = self._intf.get(uri).text.split('\n')
-        d1 = dict([each.split(' ') for each in res[:-1]])
-        d2 = dict([('%s' % k, float(v))
-                  for k, v in d1.items()])
-
-        side = {'l': 'left', 'r': 'right'}[uri.split('/')[-1][0]]
-        for region, value in d2.items():
-            row = [side, region, value]
-            table.append(row)
-
-    columns = ['side', 'region', 'value']
-    return pd.DataFrame(table, columns=columns)
-
-
-def aparc(self, atlas='desikan-killiany'):
-    """Returns cortical features as estimated by FreeSurfer `recon-all`."""
-
-    import pandas as pd
-
-    volumes = ['BrainSegVol', 'BrainSegVolNotVent', 'BrainSegVolNotVentSurf',
-               'CortexVol', 'SupraTentorialVol', 'SupraTentorialVolNotVent',
-               'eTIV']
-
-    unitless = ['NumVert']
-
-    surfaces = ['WhiteSurfArea']
-
-    thickness = ['MeanThickness']
-
-    columns = ['StructName', 'NumVert', 'SurfArea', 'GrayVol', 'ThickAvg',
-               'ThickStd', 'MeanCurv', 'GausCurv', 'FoldInd', 'CurvInd']
-
-    table = []
-    if atlas == 'desikan-killiany':
-        ft = 'aparc'
-    elif atlas == 'destrieux':
-        ft = 'aparc.a2009s'
-    else:
-        raise Exception('Invalid atlas "%s". Should be either '
-                        'desikan-killiany or destrieux.' % atlas)
-
-    files = list(self.files('*h.%s.stats' % ft))
-    for f in files:
-
-        uri = f._uri
-        side = {'l': 'left', 'r': 'right'}[uri.split('/')[-1][0]]
-
-        res = self._intf.get(uri).text.split('\n')
-
-        res2 = [e for e in res if e.startswith('# Measure ')]
-
-        measurements = {'Volume_mm3': volumes,
-                        'Thickness_mm': thickness,
-                        'SurfArea_mm2': surfaces,
-                        'unitless': unitless}
-
-        for unit, data in measurements.items():
-            for each in data:
-                m = [e for e in res2 if each == e.split(', ')[1]]
-                if len(m) == 1:
-                    m = float(m[0].split(', ')[-2])
-                    table.append([None, unit, each, m])        
-
-        res2 = [e for e in res if not e.startswith('#')]
-        d2 = [[each for each in e.split(' ') if each != ''] for e in res2]
-        d2 = pd.DataFrame(d2, columns=columns).dropna()
-        d3 = d2.set_index('StructName').to_dict()
-
-        for m, aparc in d3.items():
-            for region, value in aparc.items():
-                row = [side, m, region, value]
-                table.append(row)
-
-    columns = ['side', 'measurement', 'region', 'value']
-    return pd.DataFrame(table, columns=columns)
-
-
-def aseg(self):
-    import pandas as pd
-    columns = ['Index', 'SegId', 'NVoxels', 'Volume_mm3', 'StructName',
-               'normMean', 'normStdDev', 'normMin', 'normMax', 'normRange']
-
-    f = list(self.files('*aseg.stats'))[0]
-
-    uri = f._uri
-
-    res = self._intf.get(uri).text.split('\n')
-
-    volumes = ['BrainSegVol', 'BrainSegVolNotVent', 'BrainSegVolNotVentSurf',
-               'VentricleChoroidVol', 'lhCortexVol', 'rhCortexVol',  # 'Cortex'
-               'lhCerebralWhiteMatterVol', 'rhCerebralWhiteMatterVol',
-               'CerebralWhiteMatterVol', 'SubCortGrayVol', 'TotalGrayVol',
-               'SupraTentorialVol', 'SupraTentorialVolNotVent',
-               'SupraTentorialVolNotVentVox', 'MaskVol', 'eTIV']
-    if self.label() == 'FREESURFER7':
-        deprecated = ['BrainSegVolNotVentSurf', 'SupraTentorialVolNotVentVox']
-        volumes = [v for v in volumes if v not in deprecated]
-
-    unitless = ['BrainSegVol-to-eTIV', 'MaskVol-to-eTIV', 'lhSurfaceHoles',
-                'rhSurfaceHoles', 'SurfaceHoles']
-
-    table = []
-    res2 = [e for e in res if e.startswith('# Measure ')]
-    for each in volumes:
-        # [e for e in res2 if each == e.split(', ')[1]]
-        m = float([e for e in res2
-                   if each == e.split(', ')[1]][0].split(', ')[-2])
-        table.append(['Volume_mm3', each, m])
-
-    for each in unitless:
-        m = float([e for e in res2
-                   if each == e.split(', ')[1]][0].split(', ')[-2])
-        table.append(['unitless', each, m])
-
-    res2 = [e for e in res if not e.startswith('#')]
-    d2 = [[each for each in e.split(' ') if each != ''] for e in res2]
-    d2 = pd.DataFrame(d2, columns=columns).dropna()
-    d3 = d2.set_index('StructName').to_dict()
-
-    for m, aseg in d3.items():
-        for region, value in aseg.items():
-            row = [m, region, value]
-            table.append(row)
-
-    columns = ['measurement', 'region', 'value']
-    return pd.DataFrame(table, columns=columns)
-
-
-def normMean(self):
-
-    from roistats import collect
-    import pandas as pd
-    f1 = list(self.files('*mri/aparc.a2009s+aseg.mgz'))[0]
-    f2 = list(self.files('*mri/norm.mgz'))[0]
-    s_label = f2._uri.split('/')[-3]
-    e_id = f2._uri.split('/')[-7]
-    f1.get('/tmp/aparc.mgz')
-    f2.get('/tmp/T1.mgz')
-    import json
-    lut = dict([(int(e), v)
-               for e, v in json.load(open('/tmp/d.json')).items()])
-    roi_values = collect.roistats_from_maps(['/tmp/norm.mgz'],
-                                            '/tmp/aparc.mgz',
-                                            subjects=[(e_id, s_label)])
-    df = pd.DataFrame(roi_values, columns=lut)
-    return df.rename(columns=lut)
+XNAT_RESOURCE_NAMES = ['FREESURFER6', 'FREESURFER6_HIRES', 'FREESURFER7']
+
+
+def amygNucVolumes(self, mode='T1'):
+    """Returns amygdala nuclei volumetry as estimated by FreeSurfer
+    `recon-all`."""
+    import pandas as pd
+
+    if self.label().startswith('FREESURFER6'):
+        raise NotImplementedError('Not available in FreeSurfer 6')
+
+    table = []
+    files = list(self.files('*h.amygNucVolumes-%s.v*.txt' % mode))
+    for f in files:
+        uri = f._uri
+
+        res = self._intf.get(uri).text.split('\n')
+        d1 = dict([each.split(' ') for each in res[:-1]])
+        d2 = dict([('%s' % k, float(v))
+                  for k, v in d1.items()])
+
+        side = {'l': 'left', 'r': 'right'}[uri.split('/')[-1][0]]
+        for region, value in d2.items():
+            row = [side, region, value]
+            table.append(row)
+
+    columns = ['side', 'region', 'value']
+    return pd.DataFrame(table, columns=columns)
+
+
+def hippoSfVolumes(self, mode='T1'):
+    """Returns hippocampal subfield volumetry as estimated by FreeSurfer
+    `recon-all`."""
+    import pandas as pd
+
+    table = []
+    files = list(self.files('*h.hippoSfVolumes-%s.v*.txt' % mode))
+    for f in files:
+        uri = f._uri
+
+        res = self._intf.get(uri).text.split('\n')
+        d1 = dict([each.split(' ') for each in res[:-1]])
+        d2 = dict([('%s' % k, float(v))
+                  for k, v in d1.items()])
+
+        side = {'l': 'left', 'r': 'right'}[uri.split('/')[-1][0]]
+        for region, value in d2.items():
+            row = [side, region, value]
+            table.append(row)
+
+    columns = ['side', 'region', 'value']
+    return pd.DataFrame(table, columns=columns)
+
+
+def aparc(self, atlas='desikan-killiany'):
+    """Returns cortical features as estimated by FreeSurfer `recon-all`."""
+
+    import pandas as pd
+
+    volumes = ['BrainSegVol', 'BrainSegVolNotVent', 'BrainSegVolNotVentSurf',
+               'CortexVol', 'SupraTentorialVol', 'SupraTentorialVolNotVent',
+               'eTIV']
+
+    unitless = ['NumVert']
+
+    surfaces = ['WhiteSurfArea']
+
+    thickness = ['MeanThickness']
+
+    columns = ['StructName', 'NumVert', 'SurfArea', 'GrayVol', 'ThickAvg',
+               'ThickStd', 'MeanCurv', 'GausCurv', 'FoldInd', 'CurvInd']
+
+    table = []
+    if atlas == 'desikan-killiany':
+        ft = 'aparc'
+    elif atlas == 'destrieux':
+        ft = 'aparc.a2009s'
+    else:
+        raise Exception('Invalid atlas "%s". Should be either '
+                        'desikan-killiany or destrieux.' % atlas)
+
+    files = list(self.files('*h.%s.stats' % ft))
+    for f in files:
+
+        uri = f._uri
+        side = {'l': 'left', 'r': 'right'}[uri.split('/')[-1][0]]
+
+        res = self._intf.get(uri).text.split('\n')
+
+        res2 = [e for e in res if e.startswith('# Measure ')]
+
+        measurements = {'Volume_mm3': volumes,
+                        'Thickness_mm': thickness,
+                        'SurfArea_mm2': surfaces,
+                        'unitless': unitless}
+
+        for unit, data in measurements.items():
+            for each in data:
+                m = [e for e in res2 if each == e.split(', ')[1]]
+                if len(m) == 1:
+                    m = float(m[0].split(', ')[-2])
+                    table.append([None, unit, each, m])        
+
+        res2 = [e for e in res if not e.startswith('#')]
+        d2 = [[each for each in e.split(' ') if each != ''] for e in res2]
+        d2 = pd.DataFrame(d2, columns=columns).dropna()
+        d3 = d2.set_index('StructName').to_dict()
+
+        for m, aparc in d3.items():
+            for region, value in aparc.items():
+                row = [side, m, region, value]
+                table.append(row)
+
+    columns = ['side', 'measurement', 'region', 'value']
+    return pd.DataFrame(table, columns=columns)
+
+
+def aseg(self):
+    import pandas as pd
+    columns = ['Index', 'SegId', 'NVoxels', 'Volume_mm3', 'StructName',
+               'normMean', 'normStdDev', 'normMin', 'normMax', 'normRange']
+
+    f = list(self.files('*aseg.stats'))[0]
+
+    uri = f._uri
+
+    res = self._intf.get(uri).text.split('\n')
+
+    volumes = ['BrainSegVol', 'BrainSegVolNotVent', 'BrainSegVolNotVentSurf',
+               'VentricleChoroidVol', 'lhCortexVol', 'rhCortexVol',  # 'Cortex'
+               'lhCerebralWhiteMatterVol', 'rhCerebralWhiteMatterVol',
+               'CerebralWhiteMatterVol', 'SubCortGrayVol', 'TotalGrayVol',
+               'SupraTentorialVol', 'SupraTentorialVolNotVent',
+               'SupraTentorialVolNotVentVox', 'MaskVol', 'eTIV']
+    if self.label() == 'FREESURFER7':
+        deprecated = ['BrainSegVolNotVentSurf', 'SupraTentorialVolNotVentVox']
+        volumes = [v for v in volumes if v not in deprecated]
+
+    unitless = ['BrainSegVol-to-eTIV', 'MaskVol-to-eTIV', 'lhSurfaceHoles',
+                'rhSurfaceHoles', 'SurfaceHoles']
+
+    table = []
+    res2 = [e for e in res if e.startswith('# Measure ')]
+    for each in volumes:
+        # [e for e in res2 if each == e.split(', ')[1]]
+        m = float([e for e in res2
+                   if each == e.split(', ')[1]][0].split(', ')[-2])
+        table.append(['Volume_mm3', each, m])
+
+    for each in unitless:
+        m = float([e for e in res2
+                   if each == e.split(', ')[1]][0].split(', ')[-2])
+        table.append(['unitless', each, m])
+
+    res2 = [e for e in res if not e.startswith('#')]
+    d2 = [[each for each in e.split(' ') if each != ''] for e in res2]
+    d2 = pd.DataFrame(d2, columns=columns).dropna()
+    d3 = d2.set_index('StructName').to_dict()
+
+    for m, aseg in d3.items():
+        for region, value in aseg.items():
+            row = [m, region, value]
+            table.append(row)
+
+    columns = ['measurement', 'region', 'value']
+    return pd.DataFrame(table, columns=columns)
+
+
+def normMean(self):
+
+    from roistats import collect
+    import pandas as pd
+    f1 = list(self.files('*mri/aparc.a2009s+aseg.mgz'))[0]
+    f2 = list(self.files('*mri/norm.mgz'))[0]
+    s_label = f2._uri.split('/')[-3]
+    e_id = f2._uri.split('/')[-7]
+    f1.get('/tmp/aparc.mgz')
+    f2.get('/tmp/T1.mgz')
+    import json
+    lut = dict([(int(e), v)
+               for e, v in json.load(open('/tmp/d.json')).items()])
+    roi_values = collect.roistats_from_maps(['/tmp/norm.mgz'],
+                                            '/tmp/aparc.mgz',
+                                            subjects=[(e_id, s_label)])
+    df = pd.DataFrame(roi_values, columns=lut)
+    return df.rename(columns=lut)
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/freesurfer7_extras.py` & `bbrc-pyxnat-1.6/pyxnat/core/derivatives/freesurfer7_extras.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-XNAT_RESOURCE_NAMES = ['FREESURFER7_EXTRAS']
-
-
-def __extract_volumes(self, filename):
-    f = list(self.files(filename))[0]
-    uri = f._uri
-
-    res = self._intf.get(uri).text.split('\n')
-    if filename.endswith('.csv'):
-        import csv
-        csv_content = list(csv.reader(res, delimiter=','))
-        d1 = dict(zip(csv_content[0], csv_content[1]))
-    else:
-        d1 = dict([each.split(' ') for each in res[:-1]])
-
-    return dict([('%s' % k, float(v))
-                 for k, v in d1.items()
-                 if k != 'subject'])
-
-
-def brainstem_substructures_volumes(self):
-    """Returns brainstem substructures volumetry as estimated by the FreeSurfer
-    brainstem segmentation module."""
-    import pandas as pd
-
-    table = []
-    data = __extract_volumes(self, '*brainstemSsVolumes.v*.txt')
-    for region, value in data.items():
-        row = [region, value]
-        table.append(row)
-
-    columns = ['region', 'value']
-    return pd.DataFrame(table, columns=columns)
-
-
-def thalamic_nuclei_volumes(self):
-    """Returns thalamic nuclei volumetry as estimated by the FreeSurfer thalamus
-    segmentation  module."""
-    import pandas as pd
-
-    table = []
-    data = __extract_volumes(self, '*ThalamicNuclei.v*.T1.volumes.txt')
-    for label, value in data.items():
-        side, region = label.split('-', 1)
-        row = [side.lower(), region, value]
-        table.append(row)
-
-    columns = ['side', 'region', 'value']
-    return pd.DataFrame(table, columns=columns)
-
-
-def hypothalamic_subunits_volumes(self):
-    """Returns hypothalamic subunits volumetry as estimated by the FreeSurfer
-    hypothalamus segmentation module."""
-    import pandas as pd
-    import csv
-
-    table = []
-    data = __extract_volumes(self, '*hypothalamic_subunits_volumes.v*.csv')
-    for label, value in data.items():
-        side, region = label.split(' ', 1)
-        if side == 'whole':
-            region, side = label.split(' ', 1)
-
-        row = [side, region, value]
-        table.append(row)
-
-    columns = ['side', 'region', 'value']
-    return pd.DataFrame(table, columns=columns)
+XNAT_RESOURCE_NAMES = ['FREESURFER7_EXTRAS']
+
+
+def __extract_volumes(self, filename):
+    f = list(self.files(filename))[0]
+    uri = f._uri
+
+    res = self._intf.get(uri).text.split('\n')
+    if filename.endswith('.csv'):
+        import csv
+        csv_content = list(csv.reader(res, delimiter=','))
+        d1 = dict(zip(csv_content[0], csv_content[1]))
+    else:
+        d1 = dict([each.split(' ') for each in res[:-1]])
+
+    return dict([('%s' % k, float(v))
+                 for k, v in d1.items()
+                 if k != 'subject'])
+
+
+def brainstem_substructures_volumes(self):
+    """Returns brainstem substructures volumetry as estimated by the FreeSurfer
+    brainstem segmentation module."""
+    import pandas as pd
+
+    table = []
+    data = __extract_volumes(self, '*brainstemSsVolumes.v*.txt')
+    for region, value in data.items():
+        row = [region, value]
+        table.append(row)
+
+    columns = ['region', 'value']
+    return pd.DataFrame(table, columns=columns)
+
+
+def thalamic_nuclei_volumes(self):
+    """Returns thalamic nuclei volumetry as estimated by the FreeSurfer thalamus
+    segmentation  module."""
+    import pandas as pd
+
+    table = []
+    data = __extract_volumes(self, '*ThalamicNuclei.v*.T1.volumes.txt')
+    for label, value in data.items():
+        side, region = label.split('-', 1)
+        row = [side.lower(), region, value]
+        table.append(row)
+
+    columns = ['side', 'region', 'value']
+    return pd.DataFrame(table, columns=columns)
+
+
+def hypothalamic_subunits_volumes(self):
+    """Returns hypothalamic subunits volumetry as estimated by the FreeSurfer
+    hypothalamus segmentation module."""
+    import pandas as pd
+    import csv
+
+    table = []
+    data = __extract_volumes(self, '*hypothalamic_subunits_volumes.v*.csv')
+    for label, value in data.items():
+        side, region = label.split(' ', 1)
+        if side == 'whole':
+            region, side = label.split(' ', 1)
+
+        row = [side, region, value]
+        table.append(row)
+
+    columns = ['side', 'region', 'value']
+    return pd.DataFrame(table, columns=columns)
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/pet_fdg.py` & `bbrc-pyxnat-1.6/pyxnat/core/derivatives/pet_fdg.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-XNAT_RESOURCE_NAME = 'FDG_QUANTIFICATION'
-
-
-def quantification_results(self):
-    import pandas as pd
-    import sys
-    if sys.version_info[0] < 3:
-        from StringIO import StringIO
-    else:
-        from io import StringIO
-
-    f = self.file('quantification_results.csv')
-    uri = f._uri
-    res = self._intf.get(uri).text
-    text = StringIO(res)
-    df = pd.read_csv(text)
-    return df
-
-
-def landau_signature(self, optimized=True, reference_region='vermis'):
-    """Returns the AD signature obtained from FDG as described in
-    Landau et al., Ann Neurol., 2012."""
-
-    df = self.quantification_results()
-
-    q = 'reference_region == "{reference_region}" &'\
-        ' measurement == "suvr"'.format(reference_region=reference_region)
-
-    q += ' & %soptimized_pet' % {True: '', False: '~'}[optimized]
-    df = df.query(q)
-    df = df.query('region.str.contains("landau")', engine='python')
-    
-    assert(len(set(df['atlas'])) == 1)
-    del df['atlas']
-    assert(len(set(df['optimized_pet'])) == 1)
-
-    return df
+XNAT_RESOURCE_NAME = 'FDG_QUANTIFICATION'
+
+
+def quantification_results(self):
+    import pandas as pd
+    import sys
+    if sys.version_info[0] < 3:
+        from StringIO import StringIO
+    else:
+        from io import StringIO
+
+    f = self.file('quantification_results.csv')
+    uri = f._uri
+    res = self._intf.get(uri).text
+    text = StringIO(res)
+    df = pd.read_csv(text)
+    return df
+
+
+def landau_signature(self, optimized=True, reference_region='vermis'):
+    """Returns the AD signature obtained from FDG as described in
+    Landau et al., Ann Neurol., 2012."""
+
+    df = self.quantification_results()
+
+    q = 'reference_region == "{reference_region}" &'\
+        ' measurement == "suvr"'.format(reference_region=reference_region)
+
+    q += ' & %soptimized_pet' % {True: '', False: '~'}[optimized]
+    df = df.query(q)
+    df = df.query('region.str.contains("landau")', engine='python')
+    
+    assert(len(set(df['atlas'])) == 1)
+    del df['atlas']
+    assert(len(set(df['optimized_pet'])) == 1)
+
+    return df
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/qsxmt.py` & `bbrc-pyxnat-1.6/pyxnat/core/derivatives/qsxmt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-XNAT_RESOURCE_NAMES = ['QSMXT']
-
-
-def stats(self):
-    """Summary statistics for the regional QSM values within each region
-    in the Harvard-Oxford cortical and subcortical atlases"""
-    import csv
-    import pandas as pd
-
-    region_stats = []
-    cols = []
-
-    f = self.files('region_analysis/*.csv')[0]
-    content = self._intf.get(f.attributes()['URI']).text.splitlines()
-    for idx, ln in enumerate(csv.reader(content)):
-        if idx == 0:
-            cols = ln
-        else:
-            region_stats.append(ln)
-
-    df = pd.DataFrame(region_stats, columns=cols).dropna()
-    df['subject_id'] = df['subject'].str.split('_', expand=True)[0].str[4:]
-    df['session_id'] = df['subject'].str.split('_', expand=True)[1].str[4:]
-    df = df.reindex(['subject_id', 'session_id'] + cols, axis=1)
-    for col in ['num_voxels', 'min', 'max', 'median', 'mean', 'std']:
-        df[col] = pd.to_numeric(df[col])
-    return df
+XNAT_RESOURCE_NAMES = ['QSMXT']
+
+
+def stats(self):
+    """Summary statistics for the regional QSM values within each structure
+    in the FreeSurfer aseg atlas"""
+    import csv
+    import pandas as pd
+
+    region_stats = []
+    cols = []
+
+    f = self.files('region_analysis/*.csv')[0]
+    content = self._intf.get(f.attributes()['URI']).text.splitlines()
+    for idx, ln in enumerate(csv.reader(content)):
+        if idx == 0:
+            cols = ln
+        else:
+            region_stats.append(ln)
+
+    df = pd.DataFrame(region_stats, columns=cols).dropna()
+    df['subject_id'] = df['subject'].str.split('_', expand=True)[0].str[4:]
+    df['session_id'] = df['subject'].str.split('_', expand=True)[1].str[4:]
+    df = df.reindex(['subject_id', 'session_id'] + cols, axis=1)
+    for col in ['num_voxels', 'min', 'max', 'median', 'mean', 'std']:
+        df[col] = pd.to_numeric(df[col])
+    return df
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/derivatives/validator.py` & `bbrc-pyxnat-1.6/pyxnat/core/derivatives/validator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-XNAT_RESOURCE_NAMES = ['BBRC_VALIDATOR']
-
-
-def tests(self, name, key=None):
-    """
-    Looks up a validation test based on the validator name and returns its
-    result. If no test name is provided, then a dictionary is returned with
-    all the tests from the validation report.
-
-    Args:
-        name (String): Root found in the name of the report
-            (ex: FreeSurferValidator)
-        key (String): Name of the test.
-    Returns:
-        A `pyxnat` File of the report.
-
-    """
-    import json
-    j = [e for e in list(self.files('{}*.json'.format(name)))][0]
-    j = json.loads(self._intf.get(j._uri).text)
-    if key is None:
-        return j
-    else:
-        return j[key]
-
-
-def pdf(self, name):
-    """
-    Returns a validator report based on its name. Raises exception if
-    multiple reports are found.
-
-    Args:
-        name (String): Root found in the name of the report
-            (ex: FreeSurferValidator)
-    Returns:
-        A `pyxnat` File of the report.
-
-    """
-    files = list(self.files())
-    pdf_file = {each._uri.split('/')[-1]: each for each in files
-                if name in each._uri.split('/')[-1] and
-                each._uri.split('/')[-1].endswith('.pdf')}
-
-    if len(pdf_file.items()) == 0:
-        raise Exception('No %s found' % name)
-
-    keys = list(pdf_file.keys())
-    if len(keys) != 1:
-        raise Exception('Multiple matching reports found (%s)' % keys)
-
-    f = pdf_file[list(pdf_file.keys())[0]]
-    return f
-
-
-def download_snapshot(self, name, fp):
-    """
-    Extract snapshot(s) from a validation report given its name.
-
-    Args:
-        name (String): Root found in the name of the report
-            (ex: FreeSurferValidator)
-        fp (String): Path to the file where the snapshot(s) will be saved.
-    """
-
-    import os
-    import os.path as op
-    import tempfile
-
-    def extract_snapshots(fp):
-        import fitz
-        doc = fitz.open(fp)
-        dn = op.dirname(fp)
-        bn = op.splitext(op.basename(fp))[0]
-        images = []
-        xrefs = []
-        for page in range(len(doc)):
-            xrefs.extend([img[0] for img in doc.getPageImageList(page)])
-        xrefs = sorted(set(xrefs))
-        for k, xref in enumerate(xrefs[1:]):
-            pix = fitz.Pixmap(doc, xref)
-            fp_snap = op.join(dn, "{}_{}.png".format(bn, k))
-            if pix.n >= 5:    # CMYK: convert to RGB first
-                pix = fitz.Pixmap(fitz.csRGB, pix)
-            pix.writePNG(fp_snap)
-            images.append(fp_snap)
-        return images
-
-    pdf_file = self.pdf(name)
-
-    f, fp1 = tempfile.mkstemp(suffix='.pdf')
-    os.close(f)
-    pdf_file.get(dest=fp1)
-
-    snaps = extract_snapshots(fp1)
-
-    if len(snaps) == 0:
-        raise Exception('No snapshot found in report. %s %s' % (name, fp1))
-
-    files = []  # Will store the snapshots in their final folder
-    for i, each in enumerate(snaps):
-        bn, _ = op.splitext(fp)
-        _, ext = op.splitext(each)
-        interm = ''
-        if len(snaps) > 1:  # if multiple snapshots then add # in filename
-            interm = '_%s' % i
-        fp2 = '%s%s%s' % (bn, interm, ext)  # create destination filepath
-        cmd = 'mv %s %s' % (each, fp2)
-        os.system(cmd)
-        files.append(fp2)
-
-    os.remove(fp1)
-    return files
+XNAT_RESOURCE_NAMES = ['BBRC_VALIDATOR']
+
+
+def tests(self, name, key=None):
+    """
+    Looks up a validation test based on the validator name and returns its
+    result. If no test name is provided, then a dictionary is returned with
+    all the tests from the validation report.
+
+    Args:
+        name (String): Root found in the name of the report
+            (ex: FreeSurferValidator)
+        key (String): Name of the test.
+    Returns:
+        A `pyxnat` File of the report.
+
+    """
+    import json
+    j = [e for e in list(self.files('{}*.json'.format(name)))][0]
+    j = json.loads(self._intf.get(j._uri).text)
+    if key is None:
+        return j
+    else:
+        return j[key]
+
+
+def pdf(self, name):
+    """
+    Returns a validator report based on its name. Raises exception if
+    multiple reports are found.
+
+    Args:
+        name (String): Root found in the name of the report
+            (ex: FreeSurferValidator)
+    Returns:
+        A `pyxnat` File of the report.
+
+    """
+    files = list(self.files())
+    pdf_file = {each._uri.split('/')[-1]: each for each in files
+                if name in each._uri.split('/')[-1] and
+                each._uri.split('/')[-1].endswith('.pdf')}
+
+    if len(pdf_file.items()) == 0:
+        raise Exception('No %s found' % name)
+
+    keys = list(pdf_file.keys())
+    if len(keys) != 1:
+        raise Exception('Multiple matching reports found (%s)' % keys)
+
+    f = pdf_file[list(pdf_file.keys())[0]]
+    return f
+
+
+def download_snapshot(self, name, fp):
+    """
+    Extract snapshot(s) from a validation report given its name.
+
+    Args:
+        name (String): Root found in the name of the report
+            (ex: FreeSurferValidator)
+        fp (String): Path to the file where the snapshot(s) will be saved.
+    """
+
+    import os
+    import os.path as op
+    import tempfile
+
+    def extract_snapshots(fp):
+        import fitz
+        doc = fitz.open(fp)
+        dn = op.dirname(fp)
+        bn = op.splitext(op.basename(fp))[0]
+        images = []
+        xrefs = []
+        for page in range(len(doc)):
+            xrefs.extend([img[0] for img in doc.get_page_images(page)])
+        xrefs = sorted(set(xrefs))
+        for k, xref in enumerate(xrefs[1:]):
+            pix = fitz.Pixmap(doc, xref)
+            fp_snap = op.join(dn, "{}_{}.png".format(bn, k))
+            if pix.n >= 5:    # CMYK: convert to RGB first
+                pix = fitz.Pixmap(fitz.csRGB, pix)
+            pix.save(fp_snap)
+            images.append(fp_snap)
+        return images
+
+    pdf_file = self.pdf(name)
+
+    f, fp1 = tempfile.mkstemp(suffix='.pdf')
+    os.close(f)
+    pdf_file.get(dest=fp1)
+
+    snaps = extract_snapshots(fp1)
+
+    if len(snaps) == 0:
+        raise Exception('No snapshot found in report. %s %s' % (name, fp1))
+
+    files = []  # Will store the snapshots in their final folder
+    for i, each in enumerate(snaps):
+        bn, _ = op.splitext(fp)
+        _, ext = op.splitext(each)
+        interm = ''
+        if len(snaps) > 1:  # if multiple snapshots then add # in filename
+            interm = '_%s' % i
+        fp2 = '%s%s%s' % (bn, interm, ext)  # create destination filepath
+        cmd = 'mv %s %s' % (each, fp2)
+        os.system(cmd)
+        files.append(fp2)
+
+    os.remove(fp1)
+    return files
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/downloadutils.py` & `bbrc-pyxnat-1.6/pyxnat/core/downloadutils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-import os.path as op
-import zipfile
-import sys
-
-from .schema import class_name
-from . import uriutil
-
-DEBUG = False
-
-
-def unzip(fzip,
-          dest_dir,
-          check={'run': lambda z, d: True, 'desc': ""}):
-    """
-    Extracts the given zip file to the given directory, but only if all members
-    of the archive pass the given check.
-
-        Parameters
-        ----------
-        src: fzip
-            zipfile
-        dest_dir: string
-            directory into which to extract the archive
-        check: dict
-            An dictionary that has the keys:
-                 'run' : A function that takes a filename and parent directory
-                     and returns Bool. By default this function always returns
-                     True.
-                 'dest' : A string description of this test. By default this
-                     is empty.
-
-        Returns a tuple of type (bool,[string]) where if the extraction ran
-        successfully the first is true and the second is a list of files that
-        were extracted, and if not the first is false and the second is the
-        name of the failing member.
-    """
-    for member in fzip.namelist():
-        if not check['run'](member, dest_dir):
-            return (False, member)
-
-    fzip.extractall(path=dest_dir)
-    return (True, map(lambda f: op.join(dest_dir, f), fzip.namelist()))
-
-
-def download(dest_dir, instance=None, type="ALL", name=None, extract=False,
-             safe=False, removeZip=False):
-    """
-    Download all the files at this level that match the given constraint as a
-    zip archive. Should not be called directly but from a instance of class
-    that supports bulk downloading eg. "Scans"
-
-        Parameters
-        ----------
-        instance : 'object
-             The instance that contains local values needed by this function
-             eg. instance._cbase stores the URI.
-        dest_dir : string
-             directory into which to place the downloaded archive.
-        type: string
-             a comma separated list of file types, eg. "T1,T2". Default is
-             "ALL".
-        name: string
-             the name of the zip archive. Defaults to None. See below for the
-             default naming scheme.
-        extract: bool
-             If True, the files are left extracted in the parent directory.
-             Default is False.
-        safe: bool
-             If true, run safety checks on the files before extracting,
-             eg. check that the file doesn't exist in the parent directory
-             before overwriting it. Default is False.
-
-        Default Zip Name
-        ----------------
-        Given the project "p", subject "s" and experiment "e", and that the
-        "Scans" (as opposed to "Assessors" or "Reconstructions") are being
-        downloaded, and the scan types are constrained to "T1,T2", the name of
-        the zip file defaults to:
-          "p_s_e_scans_T1_T2.zip"
-
-        Exceptions
-        ----------
-        A generic Exception will be raised if any of the following happen:
-         - This function is called directly and not from an instance of a
-            class that supports bulk downloading eg."Scans"
-         - The destination directory is unspecified
-        A LookupError is raised if there are no resources to download
-        A ValueError is raised if any of the following happen:
-         - The project, subject and experiment names could not be extracted
-            from the URI
-         - The type constraint "ALL" is used with other constraints.
-            eg. "ALL,T1,T2"
-         - The URI associated with this class contains wildcards
-            eg. /projects/proj/subjects/*/experiments/scans
-        An EnvironmentError is raised if any of the following happen:
-         - If "safe" is true, and (a) a zip file with the same name exists in
-            given destination directory or
-           (b) extracting the archive overrides an existing file. In the second
-            case the downloaded archive
-           is left in the parent directory.
-
-        Return
-        ------
-        A path to the zip archive if "extract" is False, and a list of
-        extracted files if True.
-    """
-
-    if instance is None:
-        raise Exception('This function should be called directly but from an'
-                        'instance of a class that supports bulk downloading, '
-                        'eg. "Scans"')
-    if dest_dir is None:
-        raise Exception('Destination directory is unspecified')
-
-    # the URI must be fully qualified with a project,subject and experiment
-    if '%2A' in instance._cbase:
-        raise ValueError('URI contains wildcards :' + instance._cbase)
-
-    # Check that there are resources at this level
-    available = instance.get()
-    if len(available) == 0:
-        raise LookupError(
-            'There are no %s to download' % class_name(instance).lower())
-
-    pse = uriutil.extract_uri(instance._cbase)
-    if pse is None:
-        raise ValueError("Could not extract project, subject and experiment "
-                         "from the uri: " + instance._cbase)
-
-    # Extract the desired scan types. Clean up whitespace and remove dupes
-    types = {}
-    for t in type.split(','):
-        cleaned = t.strip()
-        if cleaned != "":
-            types[cleaned] = cleaned
-
-    # Make sure the user hasn't asked us to download ALL the scans and then
-    # asked for them to be constrained to a type.
-    if len(types) > 1 and 'ALL' in types:
-        raise ValueError('The \"ALL\" scan type constraint cannot be used with'
-                         ' any other constraint')
-
-    (p, s, e) = pse
-
-    # Make the name of the zip file
-    default_zip_name = lambda: '%s_%s_%s_%s_%s' % (
-        p, s, e, class_name(instance).lower(), '_'.join(types.values()))
-
-    zip_name = name if name is not None else default_zip_name()
-    zip_location = op.join(dest_dir, zip_name + '.zip')
-
-    if safe:
-        if op.exists(zip_location):
-            raise EnvironmentError("Unable to download to " + zip_location +
-                                   " because this file already exists.")
-
-    # Download from the server
-    with open(zip_location, 'wb') as f:
-        response = instance._intf.get(uriutil.join_uri(
-            instance._cbase, ','.join(types.values())) + '/files?format=zip',
-            stream=True)
-        try:
-            count = 0
-            for chunk in response.iter_content(chunk_size=1024):
-                if chunk:  # filter out keep-alive new chunks
-                    f.write(chunk)
-                    count += 1
-                    if count % 10 == 0:
-                        # flush the buffer every once in a while.
-                        f.flush()
-            f.flush()  # and one last flush.
-        except Exception as e:
-            sys.stderr.write(e)
-        finally:
-            response.close()
-
-    if DEBUG:
-        print(zip_location)
-
-    ##
-
-    # Extract the archive
-    fzip = zipfile.ZipFile(zip_location, 'r')
-    if extract:
-        check = {'run': lambda f, d: not op.exists(op.join(dest_dir, f)),
-                 'desc': 'File does not exist in the parent directory'}
-        safeUnzip = lambda: unzip(fzip, dest_dir, check) \
-            if safe else lambda: unzip(fzip, dest_dir)
-        (unzipped, paths) = safeUnzip()()
-        if not unzipped:
-            fzip.close()
-            msg = "Unable to extract " + zip_location + " because file " +\
-                paths + " failed the following test: " + check['desc']
-            raise EnvironmentError(msg)
-        else:
-            if removeZip:
-                fzip.close()
-                import os
-                os.remove(zip_location)
-            return paths
-    else:
-        fzip.close()
-        return zip_location
+import os.path as op
+import zipfile
+import sys
+
+from .schema import class_name
+from . import uriutil
+
+DEBUG = False
+
+
+def unzip(fzip,
+          dest_dir,
+          check={'run': lambda z, d: True, 'desc': ""}):
+    """
+    Extracts the given zip file to the given directory, but only if all members
+    of the archive pass the given check.
+
+        Parameters
+        ----------
+        src: fzip
+            zipfile
+        dest_dir: string
+            directory into which to extract the archive
+        check: dict
+            An dictionary that has the keys:
+                 'run' : A function that takes a filename and parent directory
+                     and returns Bool. By default this function always returns
+                     True.
+                 'dest' : A string description of this test. By default this
+                     is empty.
+
+        Returns a tuple of type (bool,[string]) where if the extraction ran
+        successfully the first is true and the second is a list of files that
+        were extracted, and if not the first is false and the second is the
+        name of the failing member.
+    """
+    for member in fzip.namelist():
+        if not check['run'](member, dest_dir):
+            return (False, member)
+
+    fzip.extractall(path=dest_dir)
+    return (True, map(lambda f: op.join(dest_dir, f), fzip.namelist()))
+
+
+def download(dest_dir, instance=None, type="ALL", name=None, extract=False,
+             safe=False, removeZip=False):
+    """
+    Download all the files at this level that match the given constraint as a
+    zip archive. Should not be called directly but from a instance of class
+    that supports bulk downloading eg. "Scans"
+
+        Parameters
+        ----------
+        instance : 'object
+             The instance that contains local values needed by this function
+             eg. instance._cbase stores the URI.
+        dest_dir : string
+             directory into which to place the downloaded archive.
+        type: string
+             a comma separated list of file types, eg. "T1,T2". Default is
+             "ALL".
+        name: string
+             the name of the zip archive. Defaults to None. See below for the
+             default naming scheme.
+        extract: bool
+             If True, the files are left extracted in the parent directory.
+             Default is False.
+        safe: bool
+             If true, run safety checks on the files before extracting,
+             eg. check that the file doesn't exist in the parent directory
+             before overwriting it. Default is False.
+
+        Default Zip Name
+        ----------------
+        Given the project "p", subject "s" and experiment "e", and that the
+        "Scans" (as opposed to "Assessors" or "Reconstructions") are being
+        downloaded, and the scan types are constrained to "T1,T2", the name of
+        the zip file defaults to:
+          "p_s_e_scans_T1_T2.zip"
+
+        Exceptions
+        ----------
+        A generic Exception will be raised if any of the following happen:
+         - This function is called directly and not from an instance of a
+            class that supports bulk downloading eg."Scans"
+         - The destination directory is unspecified
+        A LookupError is raised if there are no resources to download
+        A ValueError is raised if any of the following happen:
+         - The project, subject and experiment names could not be extracted
+            from the URI
+         - The type constraint "ALL" is used with other constraints.
+            eg. "ALL,T1,T2"
+         - The URI associated with this class contains wildcards
+            eg. /projects/proj/subjects/*/experiments/scans
+        An EnvironmentError is raised if any of the following happen:
+         - If "safe" is true, and (a) a zip file with the same name exists in
+            given destination directory or
+           (b) extracting the archive overrides an existing file. In the second
+            case the downloaded archive
+           is left in the parent directory.
+
+        Return
+        ------
+        A path to the zip archive if "extract" is False, and a list of
+        extracted files if True.
+    """
+
+    if instance is None:
+        raise Exception('This function should be called directly but from an'
+                        'instance of a class that supports bulk downloading, '
+                        'eg. "Scans"')
+    if dest_dir is None:
+        raise Exception('Destination directory is unspecified')
+
+    # the URI must be fully qualified with a project,subject and experiment
+    if '%2A' in instance._cbase:
+        raise ValueError('URI contains wildcards :' + instance._cbase)
+
+    # Check that there are resources at this level
+    available = instance.get()
+    if len(available) == 0:
+        raise LookupError(
+            'There are no %s to download' % class_name(instance).lower())
+
+    pse = uriutil.extract_uri(instance._cbase)
+    if pse is None:
+        raise ValueError("Could not extract project, subject and experiment "
+                         "from the uri: " + instance._cbase)
+
+    # Extract the desired scan types. Clean up whitespace and remove dupes
+    types = {}
+    for t in type.split(','):
+        cleaned = t.strip()
+        if cleaned != "":
+            types[cleaned] = cleaned
+
+    # Make sure the user hasn't asked us to download ALL the scans and then
+    # asked for them to be constrained to a type.
+    if len(types) > 1 and 'ALL' in types:
+        raise ValueError('The \"ALL\" scan type constraint cannot be used with'
+                         ' any other constraint')
+
+    (p, s, e) = pse
+
+    # Make the name of the zip file
+    default_zip_name = lambda: '%s_%s_%s_%s_%s' % (
+        p, s, e, class_name(instance).lower(), '_'.join(types.values()))
+
+    zip_name = name if name is not None else default_zip_name()
+    zip_location = op.join(dest_dir, zip_name + '.zip')
+
+    if safe:
+        if op.exists(zip_location):
+            raise EnvironmentError("Unable to download to " + zip_location +
+                                   " because this file already exists.")
+
+    # Download from the server
+    with open(zip_location, 'wb') as f:
+        response = instance._intf.get(uriutil.join_uri(
+            instance._cbase, ','.join(types.values())) + '/files?format=zip',
+            stream=True)
+        try:
+            count = 0
+            for chunk in response.iter_content(chunk_size=1024):
+                if chunk:  # filter out keep-alive new chunks
+                    f.write(chunk)
+                    count += 1
+                    if count % 10 == 0:
+                        # flush the buffer every once in a while.
+                        f.flush()
+            f.flush()  # and one last flush.
+        except Exception as e:
+            sys.stderr.write(e)
+        finally:
+            response.close()
+
+    if DEBUG:
+        print(zip_location)
+
+    ##
+
+    # Extract the archive
+    fzip = zipfile.ZipFile(zip_location, 'r')
+    if extract:
+        check = {'run': lambda f, d: not op.exists(op.join(dest_dir, f)),
+                 'desc': 'File does not exist in the parent directory'}
+        safeUnzip = lambda: unzip(fzip, dest_dir, check) \
+            if safe else lambda: unzip(fzip, dest_dir)
+        (unzipped, paths) = safeUnzip()()
+        if not unzipped:
+            fzip.close()
+            msg = "Unable to extract " + zip_location + " because file " +\
+                paths + " failed the following test: " + check['desc']
+            raise EnvironmentError(msg)
+        else:
+            if removeZip:
+                fzip.close()
+                import os
+                os.remove(zip_location)
+            return paths
+    else:
+        fzip.close()
+        return zip_location
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/help.py` & `bbrc-pyxnat-1.6/pyxnat/core/help.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,691 +1,691 @@
-try:
-    import networkx as nx
-    from networkx.drawing.nx_agraph import graphviz_layout
-    import matplotlib.pyplot as plt
-    _DRAW_GRAPHS = True
-except Exception:
-    _DRAW_GRAPHS = False
-
-from . import schema
-from .jsonutil import get_column
-from .search import Search
-
-
-class Inspector(object):
-    """ Database introspection interface.
-    """
-
-    def __init__(self, interface):
-        """
-            Parameters
-            ----------
-            interface:
-                :class:`Interface` Object
-        """
-        self._intf = interface
-        self._get_json = interface._get_json
-        self._auto = True
-        self._tick = 30
-
-        self.schemas = SchemasInspector(interface)
-
-    def __call__(self):
-        for name in ['experiment', 'assessor', 'scan', 'reconstruction']:
-            self._resource_struct(name)
-
-    def set_autolearn(self, auto=None, tick=None):
-        """ Once in a while queries will persist additional
-            information on the server. This information is available
-            through the following methods of this class:
-
-                - experiment_types
-                - assessor_types
-                - scan_types
-                - reconstruction_types
-
-            It is also transparently used in insert operations.
-
-            Parameters
-            ----------
-            auto: boolean
-                True to enable auto learn. False to disable.
-            tick: int
-                Every 'tick' seconds, if a query is issued, additional
-                information will be persisted.
-
-            See Also
-            --------
-            :func:`EObject.insert`
-        """
-        if auto is not None:
-            self._auto = auto
-        if tick is not None:
-            self._tick = tick
-
-    def datatypes(self, pattern='*', fields_pattern=None):
-        """ Discovers the datatypes and datafields of the database.
-
-            Parameters
-            ----------
-            pattern: string
-                Pattern for the datatype. May include wildcards.
-            fields_pattern: string
-                - Pattern for the datafields -- may include wildcards.
-                - If specified, datafields will be returned instead of
-                  datatypes.
-
-            Returns
-            -------
-            list : datatypes or datafields depending on the argument usage.
-        """
-        self._intf._get_entry_point()
-
-        search_els = self._get_json('%s/search/elements?format=json' %
-                                    self._intf._get_entry_point())
-
-        if not fields_pattern and ('*' in pattern or '?' in pattern):
-            return get_column(search_els, 'ELEMENT_NAME', pattern)
-
-        else:
-            fields = []
-            for datatype in get_column(search_els, 'ELEMENT_NAME', pattern):
-                df = self._datafields(datatype, fields_pattern or '*', True)
-                fields.extend(df)
-
-            return fields
-
-    def _datafields(self, datatype, pattern='*', prepend_type=True):
-        self._intf._get_entry_point()
-
-        search_fds = self._get_json('%s/search/elements/%s?format=json' %
-                                    (self._intf._get_entry_point(),
-                                        datatype))
-
-        fields = get_column(search_fds, 'FIELD_ID', pattern)
-
-        return ['%s/%s' % (datatype, field)
-                if prepend_type else field
-                for field in fields
-                if '=' not in field and 'SHARINGSHAREPROJECT' not in field
-                ]
-
-    def experiment_types(self):
-        """ Returns the datatypes used at the experiment level in this
-            database.
-
-            See Also
-            --------
-            :func:`Inspector.set_autolearn`
-        """
-        return self._resource_types('experiment')
-
-    def assessor_types(self):
-        """ Returns the datatypes used at the assessor level in this
-            database.
-
-            See Also
-            --------
-            :func:`Inspector.set_autolearn`
-        """
-        return self._resource_types('assessor')
-
-    def reconstruction_types(self):
-        """ Returns the datatypes used at the reconstruction level in this
-            database.
-
-            See Also
-            --------
-            :func:`Inspector.set_autolearn`
-        """
-        return self._resource_types('reconstruction')
-
-    def scan_types(self):
-        """ Returns the datatypes used at the scan level in this
-            database.
-
-            See Also
-            --------
-            :func:`Inspector.set_autolearn`
-        """
-        return self._resource_types('scan')
-
-    def field_values(self, field_name):
-        """ Look for the values a specific datafield takes in the database.
-        """
-        self._intf._get_entry_point()
-
-        search_tbl = Search(field_name.split('/')[0],
-                            [field_name], self._intf
-                            )
-
-        criteria = [('%s/ID' % field_name.split('/')[0], 'LIKE', '%'), 'AND']
-
-        return list(set([val
-                         for entry in search_tbl.where(criteria)
-                         for val in entry.values()
-                         ])
-                    )
-
-    def project_values(self):
-        """ Look for the values a the project level in the database.
-
-            .. note::
-                Is equivalent to interface.select.projects().get()
-        """
-        self._intf._get_entry_point()
-
-        return get_column(self._get_json(
-                '%s/projects' % self._intf._entry), 'ID')
-
-    def subject_values(self, project=None):
-        """ Look for the values a the subject level in the database.
-
-            .. note::
-                Is equivalent to interface.select('//subjects').get()
-        """
-        self._intf._get_entry_point()
-
-        uri = '%s/subjects?columns=ID' % self._intf._entry
-
-        if project is not None:
-            uri += '&project=%s' % project
-
-        return get_column(self._get_json(uri), 'ID')
-
-    def experiment_values(self, datatype, project=None):
-        """ Look for the values a the experiment level for a given datatype
-            in the database.
-
-            .. note::
-                The  datatype should be one of Inspector.experiment_types()
-
-            Parameters
-            ----------
-            datatype: string
-                An experiment type. eg: xnat:mrsessiondata
-            project: string
-                Optional. Restrict operation to a project.
-        """
-        self._intf._get_entry_point()
-
-        uri = '%s/experiments?columns=ID' % self._intf._entry
-        if datatype is not None:
-            uri += '&xsiType=%s' % datatype
-        if project is not None:
-            uri += '&project=%s' % project
-
-        return get_column(self._get_json(uri), 'ID')
-
-    def assessor_values(self, experiment_type, project=None):
-        """ Look for the values at the assessor level for a given experiment
-            type in the database.
-
-            .. note::
-               The experiment type should be one of
-               Inspector.experiment_types()
-
-            .. warning::
-                Depending on the number of elements the operation may
-                take a while.
-
-            Parameters
-            ----------
-            datatype: string
-                An experiment type. eg: xnat:mrsessiondata
-            project: string
-                Optional. Restrict operation to a project.
-        """
-        return self._sub_experiment_values('assessor',
-                                           project, experiment_type)
-
-    def scan_values(self, experiment_type, project=None):
-        """ Look for the values at the scan level for a given experiment
-            type in the database.
-
-            .. note::
-               The experiment type should be one of
-               Inspector.experiment_types()
-
-            .. warning::
-                Depending on the number of elements the operation may
-                take a while.
-
-            Parameters
-            ----------
-            datatype: string
-                An experiment type.
-            project: string
-                Optional. Restrict operation to a project.
-        """
-        return self._sub_experiment_values('scan', project, experiment_type)
-
-    def reconstruction_values(self, experiment_type, project=None):
-        """ Look for the values at the reconstruction level for a given
-            experiment type in the database.
-
-            .. note::
-               The experiment type should be one of
-               Inspector.experiment_types()
-
-            .. warning::
-                Depending on the number of elements the operation may
-                take a while.
-
-            Parameters
-            ----------
-            datatype: string
-                An experiment type.
-            project: string
-                Optional. Restrict operation to a project.
-        """
-        return self._sub_experiment_values('reconstruction',
-                                           project, experiment_type)
-
-    def structure(self):
-        """ Displays the keywords structure used in XNAT REST API.
-        """
-        def traverse(coll, lvl):
-            for key in schema.resources_tree[coll]:
-                print('%s+%s' % (' ' * lvl, key.upper()))
-
-                datatypes = set([
-                        self._intf._struct[uri]
-                        for uri in self._intf._struct.keys()
-                        if uri.split('/')[-2] == key
-                        ])
-
-                if datatypes != set():
-                    print('%s  %s' % (' ' * lvl, '-' * len(key)))
-
-                for datatype in datatypes:
-                    print('%s- %s' % (' ' * lvl, datatype))
-
-                if key in schema.resources_tree.keys():
-                    traverse(key, lvl + 4)
-
-        print('- %s' % 'PROJECTS')
-        traverse('projects', 4)
-
-    def _sub_experiment_values(self, sub_exp, project, experiment_type):
-        self._intf._get_entry_point()
-
-        values = []
-
-        column = '%s/%ss/%s/id' % \
-            (experiment_type.lower(), sub_exp, sub_exp)
-
-        sub_exps = '%s/experiments?columns=ID,%s' % (self._intf._entry,
-                                                     column
-                                                     )
-
-        if project is not None:
-            sub_exps += '&project=%s' % project
-
-        values = get_column(self._get_json(sub_exps), column)
-
-        return list(set(values))
-
-    def _resource_struct(self, name):
-
-        return self._intf._struct
-
-    def _resource_types(self, name):
-        return list(set(self._resource_struct(name).values()))
-
-
-class GraphData(object):
-    def __init__(self, interface):
-        self._intf = interface
-        self._struct = interface._struct
-
-    # def link(self, subjects, fields):
-
-    #     criteria = [('xnat:subjectData/SUBJECT_ID', '=', _id)
-    #                 for _id in subjects
-    #                 ]
-    #     criteria += ['OR']
-    #     # variables = ['xnat:subjectData/SUBJECT_ID'] + fields
-
-    #     subject_id = 'xnat:subjectData/SUBJECT_ID'
-
-    #     for field in fields:
-
-    #         field_tbl = self._intf.select('xnat:subjectData',
-    #                                       [subject_id, field]
-    #                                       ).where(criteria)
-    #         head = field_tbl.headers()
-    #         head.remove('subject_id')
-    #         head = head[0]
-    #         possible = set(field_tbl.get(head))
-
-    #         groups = {}
-
-    #         for val in possible:
-    #             groups[val] = field_tbl.where(**{head:val}
-    #                                             ).select('subject_id')
-
-    #     return groups
-
-    def datatypes(self, pattern='*'):
-        graph = nx.DiGraph()
-        graph.add_node('datatypes')
-        graph.labels = {'datatypes': 'datatypes'}
-        graph.weights = {'datatypes': 100.0}
-
-        datatypes = self._intf.inspect.datatypes(pattern)
-        namespaces = set([dat.split(':')[0] for dat in datatypes])
-
-        for ns in namespaces:
-            graph.add_edge('datatypes', ns)
-            graph.weights[ns] = 70.0
-
-            for dat in datatypes:
-                if dat.startswith(ns):
-                    graph.add_edge(ns, dat)
-                    graph.weights[dat] = 40.0
-
-        return graph
-
-    def rest_resource(self, name):
-        resource_types = self._intf.inspect._resource_types(name)
-
-        graph = nx.DiGraph()
-        graph.add_node(name)
-        graph.labels = {name: name}
-        graph.weights = {name: 100.0}
-
-        namespaces = set([exp.split(':')[0] for exp in resource_types])
-
-        for ns in namespaces:
-            graph.add_edge(name, ns)
-            graph.weights[ns] = 70.0
-
-            for exp in resource_types:
-                if exp.startswith(ns):
-                    graph.add_edge(ns, exp)
-                    graph.weights[exp] = 40.0
-
-        return graph
-
-    def field_values(self, field_name):
-
-        search_tbl = Search(field_name.split('/')[0],
-                            [field_name], self._intf
-                            )
-
-        criteria = [('%s/ID' % field_name.split('/')[0], 'LIKE', '%'), 'AND']
-
-        dist = {}
-
-        for entry in search_tbl.where(criteria):
-            for val in entry.values():
-                dist.setdefault(val, 1.0)
-                dist[val] += 1
-
-        graph = nx.Graph()
-        graph.add_node(field_name)
-        graph.weights = dist
-        graph.weights[field_name] = 100.0
-
-        for val in dist.keys():
-            graph.add_edge(field_name, val)
-
-        return graph
-
-    def architecture(self, with_datatypes=True):
-        graph = nx.DiGraph()
-        graph.add_node('projects')
-        graph.labels = {'projects': 'projects'}
-        graph.weights = {'projects': 100.0}
-
-        def traverse(lkw, as_lkw):
-
-            for key in schema.resources_tree[lkw]:
-                as_key = '%s_%s' % (as_lkw, key)
-                weight = (1 - len(as_key*2)/100.0) * 100
-                graph.add_edge(as_lkw, as_key)
-                graph.labels[as_key] = key
-                graph.weights[as_key] = weight
-
-                if with_datatypes:
-                    for uri in self._struct.keys():
-                        if uri.split('/')[-2] == key:
-                            datatype = self._struct[uri]
-                            graph.add_edge(as_key, datatype)
-                            graph.weights[datatype] = 10
-                            graph.labels[datatype] = datatype
-
-                traverse(key, as_key)
-
-        traverse('projects', 'projects')
-
-        return graph
-
-
-class PaintGraph(object):
-    def __init__(self, interface):
-        self._intf = interface
-        self.get_graph = interface._get_graph
-
-    def architecture(self, with_datatypes=True, save=None):
-        graph = self.get_graph.architecture(with_datatypes)
-
-        plt.figure(figsize=(8, 8))
-        pos = graphviz_layout(graph, prog='twopi', args='')
-
-        # node_size = [(float(graph.degree(v)) * 5)**3 for v in graph]
-        # node_size = [graph.weights[v] ** 2 for v in graph]
-        # node_color = [float(graph.degree(v)) for v in graph]
-        # node_color = [graph.weights[v] ** 2 for v in graph]
-
-        cost = lambda v: float(graph.degree(v)) ** 3 + \
-            graph.weights[v] ** 2
-
-        costs = norm_costs([cost(v) for v in graph], 10000)
-
-        nx.draw(graph, pos, labels=graph.labels,
-                node_size=costs, node_color=costs,
-                font_size=13, font_color='orange',
-                font_weight='bold', with_labels=True
-                )
-
-        plt.axis('off')
-
-        if save is not None:
-            plt.savefig(save)
-
-        plt.show()
-
-    def experiments(self, save=None):
-        graph = self.get_graph.rest_resource('experiments')
-        self._draw_rest_resource(graph, save=None)
-
-    def assessors(self, save=None):
-        graph = self.get_graph.rest_resource('assessors')
-        self._draw_rest_resource(graph, save=None)
-
-    def reconstructions(self, save=None):
-        graph = self.get_graph.rest_resource('reconstructions')
-        self._draw_rest_resource(graph, save=None)
-
-    def scans(self):
-        graph = self.get_graph.rest_resource('scans')
-        self._draw_rest_resource(graph)
-
-    def _draw_rest_resource(self, graph, save=None):
-        plt.figure(figsize=(8, 8))
-        pos = graphviz_layout(graph, prog='twopi', args='')
-
-        cost = lambda v: float(graph.degree(v)) ** 3 + \
-            graph.weights[v] ** 2
-
-        node_size = [cost(v) for v in graph]
-        # node_size = [graph.weights[v] ** 2 for v in graph]
-        # node_color = [float(graph.degree(v)) for v in graph]
-        node_color = [cost(v) for v in graph]
-
-        nx.draw(graph, pos,
-                node_size=node_size, node_color=node_color,
-                font_size=13, font_color='green', font_weight='bold'
-                )
-
-        plt.axis('off')
-
-        if save is not None:
-            plt.savefig(save)
-
-        plt.show()
-
-    def datatypes(self, pattern='*', save=None):
-        graph = self.get_graph.datatypes(pattern)
-
-        plt.figure(figsize=(8, 8))
-        pos = graphviz_layout(graph, prog='twopi', args='')
-
-        cost = lambda v: float(graph.degree(v)) ** 3 + \
-            graph.weights[v] ** 2
-
-        node_size = [cost(v) for v in graph]
-        # node_size = [graph.weights[v] ** 2 for v in graph]
-        # node_color = [float(graph.degree(v)) for v in graph]
-        node_color = [cost(v) for v in graph]
-
-        nx.draw(graph, pos,
-                node_size=node_size, node_color=node_color,
-                font_size=13, font_color='green', font_weight='bold',
-                with_labels=True
-                )
-
-        plt.axis('off')
-
-        if save is not None:
-            plt.savefig(save)
-
-        plt.show()
-
-    def field_values(self, field_name, save=None):
-        graph = self.get_graph.field_values(field_name)
-
-        plt.figure(figsize=(8, 8))
-        pos = graphviz_layout(graph, prog='twopi', args='')
-
-        cost = lambda v: graph.weights[v]
-
-        graph.weights[field_name] = max([cost(v) for v in graph]) / 2.0
-
-        costs = norm_costs([cost(v) for v in graph], 10000)
-
-        nx.draw(graph, pos,
-                node_size=costs, node_color=costs,
-                font_size=13, font_color='black',
-                font_weight='bold', with_labels=True
-                )
-
-        plt.axis('off')
-
-        if save is not None:
-            plt.savefig(save)
-
-        plt.show()
-
-
-def norm_costs(costs, norm=1000):
-    max_cost = max(costs)
-
-    return [(cost / max_cost) * norm for cost in costs]
-
-
-# class GraphDrawer(object):
-#     def __init__(self, interface):
-#         self._intf = interface
-
-#     def datatypes(self, project):
-#         self._intf.connection.set_strategy('offline')
-
-#         experiments_types = self._intf.inspect.datatypes.experiments(project)
-
-#         labels = {project:project, 'Experiments':'Experiments'}
-
-#         g = nx.Graph()
-
-#         g.add_edge(project, 'Experiments', {'weight':1})
-
-#         for exp_type in experiments_types:
-#             g.add_edge('Experiments', exp_type, {'weight':8})
-#             labels[exp_type] = exp_type
-
-#         pos = nx.graphviz_layout(g, prog='twopi', args='')
-
-#         nx.draw_networkx_nodes(g, pos,
-#                                nodelist=[project],
-#                                node_color='green', alpha=0.7,
-#                                node_size=2500, node_shape='s')
-
-#         nx.draw_networkx_nodes(g, pos,
-#                                nodelist=['Experiments'],
-#                                node_color='blue', alpha=0.7,
-#                                node_size=2000, node_shape='p')
-
-#         nx.draw_networkx_nodes(g, pos,
-#                                nodelist=experiments_types,
-#                                node_color='red', alpha=0.7,
-#                                node_size=1500, node_shape='o')
-
-#         nx.draw_networkx_edges(g, pos, width=2, alpha=0.5,
-#                                edge_color='black')
-
-#         nx.draw_networkx_labels(g, pos, labels,
-#                                 alpha=0.9, font_size=8,
-#                                 font_color='black', font_weight='bold')
-
-#         plt.axis('off')
-#         plt.show()
-
-#         self._intf.connection.revert_strategy()
-
-class SchemasInspector(object):
-    def __init__(self, interface):
-        self._intf = interface
-
-    def __call__(self):
-        self._intf.manage.schemas()
-
-        for xsd in self._intf.manage.schemas():
-            print('-'*40)
-            print(xsd.upper())
-            print('-'*40)
-            print()
-
-            trees = self._intf.manage.schemas._trees[xsd]
-            for datatype in schema.datatypes(trees):
-                print('[%s]' % datatype)
-                print()
-
-                for path in schema.datatype_attributes(trees, datatype):
-                    print(path)
-
-                print()
-
-    def look_for(self, element_name, datatype_name=None):
-        paths = []
-        self._intf.manage.schemas._init()
-
-        if ':' in element_name:
-            for root in self._intf.manage.schemas._trees.values():
-                paths.extend(schema.datatype_attributes(root, element_name))
-            return paths
-
-        for xsd in self._intf.manage.schemas():
-            # nsmap = self._intf.manage.schemas._trees[xsd].nsmap
-            trees = self._intf.manage.schemas._trees[xsd]
-            if datatype_name is not None:
-                datatypes = [datatype_name]
-            else:
-                datatypes = schema.datatypes(trees)
-
-            for datatype in datatypes:
-                for path in schema.datatype_attributes(trees, datatype):
-                    if element_name in path:
-                        paths.append(path)
-
-        return paths
+try:
+    import networkx as nx
+    from networkx.drawing.nx_agraph import graphviz_layout
+    import matplotlib.pyplot as plt
+    _DRAW_GRAPHS = True
+except Exception:
+    _DRAW_GRAPHS = False
+
+from . import schema
+from .jsonutil import get_column
+from .search import Search
+
+
+class Inspector(object):
+    """ Database introspection interface.
+    """
+
+    def __init__(self, interface):
+        """
+            Parameters
+            ----------
+            interface:
+                :class:`Interface` Object
+        """
+        self._intf = interface
+        self._get_json = interface._get_json
+        self._auto = True
+        self._tick = 30
+
+        self.schemas = SchemasInspector(interface)
+
+    def __call__(self):
+        for name in ['experiment', 'assessor', 'scan', 'reconstruction']:
+            self._resource_struct(name)
+
+    def set_autolearn(self, auto=None, tick=None):
+        """ Once in a while queries will persist additional
+            information on the server. This information is available
+            through the following methods of this class:
+
+                - experiment_types
+                - assessor_types
+                - scan_types
+                - reconstruction_types
+
+            It is also transparently used in insert operations.
+
+            Parameters
+            ----------
+            auto: boolean
+                True to enable auto learn. False to disable.
+            tick: int
+                Every 'tick' seconds, if a query is issued, additional
+                information will be persisted.
+
+            See Also
+            --------
+            :func:`EObject.insert`
+        """
+        if auto is not None:
+            self._auto = auto
+        if tick is not None:
+            self._tick = tick
+
+    def datatypes(self, pattern='*', fields_pattern=None):
+        """ Discovers the datatypes and datafields of the database.
+
+            Parameters
+            ----------
+            pattern: string
+                Pattern for the datatype. May include wildcards.
+            fields_pattern: string
+                - Pattern for the datafields -- may include wildcards.
+                - If specified, datafields will be returned instead of
+                  datatypes.
+
+            Returns
+            -------
+            list : datatypes or datafields depending on the argument usage.
+        """
+        self._intf._get_entry_point()
+
+        search_els = self._get_json('%s/search/elements?format=json' %
+                                    self._intf._get_entry_point())
+
+        if not fields_pattern and ('*' in pattern or '?' in pattern):
+            return get_column(search_els, 'ELEMENT_NAME', pattern)
+
+        else:
+            fields = []
+            for datatype in get_column(search_els, 'ELEMENT_NAME', pattern):
+                df = self._datafields(datatype, fields_pattern or '*', True)
+                fields.extend(df)
+
+            return fields
+
+    def _datafields(self, datatype, pattern='*', prepend_type=True):
+        self._intf._get_entry_point()
+
+        search_fds = self._get_json('%s/search/elements/%s?format=json' %
+                                    (self._intf._get_entry_point(),
+                                        datatype))
+
+        fields = get_column(search_fds, 'FIELD_ID', pattern)
+
+        return ['%s/%s' % (datatype, field)
+                if prepend_type else field
+                for field in fields
+                if '=' not in field and 'SHARINGSHAREPROJECT' not in field
+                ]
+
+    def experiment_types(self):
+        """ Returns the datatypes used at the experiment level in this
+            database.
+
+            See Also
+            --------
+            :func:`Inspector.set_autolearn`
+        """
+        return self._resource_types('experiment')
+
+    def assessor_types(self):
+        """ Returns the datatypes used at the assessor level in this
+            database.
+
+            See Also
+            --------
+            :func:`Inspector.set_autolearn`
+        """
+        return self._resource_types('assessor')
+
+    def reconstruction_types(self):
+        """ Returns the datatypes used at the reconstruction level in this
+            database.
+
+            See Also
+            --------
+            :func:`Inspector.set_autolearn`
+        """
+        return self._resource_types('reconstruction')
+
+    def scan_types(self):
+        """ Returns the datatypes used at the scan level in this
+            database.
+
+            See Also
+            --------
+            :func:`Inspector.set_autolearn`
+        """
+        return self._resource_types('scan')
+
+    def field_values(self, field_name):
+        """ Look for the values a specific datafield takes in the database.
+        """
+        self._intf._get_entry_point()
+
+        search_tbl = Search(field_name.split('/')[0],
+                            [field_name], self._intf
+                            )
+
+        criteria = [('%s/ID' % field_name.split('/')[0], 'LIKE', '%'), 'AND']
+
+        return list(set([val
+                         for entry in search_tbl.where(criteria)
+                         for val in entry.values()
+                         ])
+                    )
+
+    def project_values(self):
+        """ Look for the values a the project level in the database.
+
+            .. note::
+                Is equivalent to interface.select.projects().get()
+        """
+        self._intf._get_entry_point()
+
+        return get_column(self._get_json(
+                '%s/projects' % self._intf._entry), 'ID')
+
+    def subject_values(self, project=None):
+        """ Look for the values a the subject level in the database.
+
+            .. note::
+                Is equivalent to interface.select('//subjects').get()
+        """
+        self._intf._get_entry_point()
+
+        uri = '%s/subjects?columns=ID' % self._intf._entry
+
+        if project is not None:
+            uri += '&project=%s' % project
+
+        return get_column(self._get_json(uri), 'ID')
+
+    def experiment_values(self, datatype, project=None):
+        """ Look for the values a the experiment level for a given datatype
+            in the database.
+
+            .. note::
+                The  datatype should be one of Inspector.experiment_types()
+
+            Parameters
+            ----------
+            datatype: string
+                An experiment type. eg: xnat:mrsessiondata
+            project: string
+                Optional. Restrict operation to a project.
+        """
+        self._intf._get_entry_point()
+
+        uri = '%s/experiments?columns=ID' % self._intf._entry
+        if datatype is not None:
+            uri += '&xsiType=%s' % datatype
+        if project is not None:
+            uri += '&project=%s' % project
+
+        return get_column(self._get_json(uri), 'ID')
+
+    def assessor_values(self, experiment_type, project=None):
+        """ Look for the values at the assessor level for a given experiment
+            type in the database.
+
+            .. note::
+               The experiment type should be one of
+               Inspector.experiment_types()
+
+            .. warning::
+                Depending on the number of elements the operation may
+                take a while.
+
+            Parameters
+            ----------
+            datatype: string
+                An experiment type. eg: xnat:mrsessiondata
+            project: string
+                Optional. Restrict operation to a project.
+        """
+        return self._sub_experiment_values('assessor',
+                                           project, experiment_type)
+
+    def scan_values(self, experiment_type, project=None):
+        """ Look for the values at the scan level for a given experiment
+            type in the database.
+
+            .. note::
+               The experiment type should be one of
+               Inspector.experiment_types()
+
+            .. warning::
+                Depending on the number of elements the operation may
+                take a while.
+
+            Parameters
+            ----------
+            datatype: string
+                An experiment type.
+            project: string
+                Optional. Restrict operation to a project.
+        """
+        return self._sub_experiment_values('scan', project, experiment_type)
+
+    def reconstruction_values(self, experiment_type, project=None):
+        """ Look for the values at the reconstruction level for a given
+            experiment type in the database.
+
+            .. note::
+               The experiment type should be one of
+               Inspector.experiment_types()
+
+            .. warning::
+                Depending on the number of elements the operation may
+                take a while.
+
+            Parameters
+            ----------
+            datatype: string
+                An experiment type.
+            project: string
+                Optional. Restrict operation to a project.
+        """
+        return self._sub_experiment_values('reconstruction',
+                                           project, experiment_type)
+
+    def structure(self):
+        """ Displays the keywords structure used in XNAT REST API.
+        """
+        def traverse(coll, lvl):
+            for key in schema.resources_tree[coll]:
+                print('%s+%s' % (' ' * lvl, key.upper()))
+
+                datatypes = set([
+                        self._intf._struct[uri]
+                        for uri in self._intf._struct.keys()
+                        if uri.split('/')[-2] == key
+                        ])
+
+                if datatypes != set():
+                    print('%s  %s' % (' ' * lvl, '-' * len(key)))
+
+                for datatype in datatypes:
+                    print('%s- %s' % (' ' * lvl, datatype))
+
+                if key in schema.resources_tree.keys():
+                    traverse(key, lvl + 4)
+
+        print('- %s' % 'PROJECTS')
+        traverse('projects', 4)
+
+    def _sub_experiment_values(self, sub_exp, project, experiment_type):
+        self._intf._get_entry_point()
+
+        values = []
+
+        column = '%s/%ss/%s/id' % \
+            (experiment_type.lower(), sub_exp, sub_exp)
+
+        sub_exps = '%s/experiments?columns=ID,%s' % (self._intf._entry,
+                                                     column
+                                                     )
+
+        if project is not None:
+            sub_exps += '&project=%s' % project
+
+        values = get_column(self._get_json(sub_exps), column)
+
+        return list(set(values))
+
+    def _resource_struct(self, name):
+
+        return self._intf._struct
+
+    def _resource_types(self, name):
+        return list(set(self._resource_struct(name).values()))
+
+
+class GraphData(object):
+    def __init__(self, interface):
+        self._intf = interface
+        self._struct = interface._struct
+
+    # def link(self, subjects, fields):
+
+    #     criteria = [('xnat:subjectData/SUBJECT_ID', '=', _id)
+    #                 for _id in subjects
+    #                 ]
+    #     criteria += ['OR']
+    #     # variables = ['xnat:subjectData/SUBJECT_ID'] + fields
+
+    #     subject_id = 'xnat:subjectData/SUBJECT_ID'
+
+    #     for field in fields:
+
+    #         field_tbl = self._intf.select('xnat:subjectData',
+    #                                       [subject_id, field]
+    #                                       ).where(criteria)
+    #         head = field_tbl.headers()
+    #         head.remove('subject_id')
+    #         head = head[0]
+    #         possible = set(field_tbl.get(head))
+
+    #         groups = {}
+
+    #         for val in possible:
+    #             groups[val] = field_tbl.where(**{head:val}
+    #                                             ).select('subject_id')
+
+    #     return groups
+
+    def datatypes(self, pattern='*'):
+        graph = nx.DiGraph()
+        graph.add_node('datatypes')
+        graph.labels = {'datatypes': 'datatypes'}
+        graph.weights = {'datatypes': 100.0}
+
+        datatypes = self._intf.inspect.datatypes(pattern)
+        namespaces = set([dat.split(':')[0] for dat in datatypes])
+
+        for ns in namespaces:
+            graph.add_edge('datatypes', ns)
+            graph.weights[ns] = 70.0
+
+            for dat in datatypes:
+                if dat.startswith(ns):
+                    graph.add_edge(ns, dat)
+                    graph.weights[dat] = 40.0
+
+        return graph
+
+    def rest_resource(self, name):
+        resource_types = self._intf.inspect._resource_types(name)
+
+        graph = nx.DiGraph()
+        graph.add_node(name)
+        graph.labels = {name: name}
+        graph.weights = {name: 100.0}
+
+        namespaces = set([exp.split(':')[0] for exp in resource_types])
+
+        for ns in namespaces:
+            graph.add_edge(name, ns)
+            graph.weights[ns] = 70.0
+
+            for exp in resource_types:
+                if exp.startswith(ns):
+                    graph.add_edge(ns, exp)
+                    graph.weights[exp] = 40.0
+
+        return graph
+
+    def field_values(self, field_name):
+
+        search_tbl = Search(field_name.split('/')[0],
+                            [field_name], self._intf
+                            )
+
+        criteria = [('%s/ID' % field_name.split('/')[0], 'LIKE', '%'), 'AND']
+
+        dist = {}
+
+        for entry in search_tbl.where(criteria):
+            for val in entry.values():
+                dist.setdefault(val, 1.0)
+                dist[val] += 1
+
+        graph = nx.Graph()
+        graph.add_node(field_name)
+        graph.weights = dist
+        graph.weights[field_name] = 100.0
+
+        for val in dist.keys():
+            graph.add_edge(field_name, val)
+
+        return graph
+
+    def architecture(self, with_datatypes=True):
+        graph = nx.DiGraph()
+        graph.add_node('projects')
+        graph.labels = {'projects': 'projects'}
+        graph.weights = {'projects': 100.0}
+
+        def traverse(lkw, as_lkw):
+
+            for key in schema.resources_tree[lkw]:
+                as_key = '%s_%s' % (as_lkw, key)
+                weight = (1 - len(as_key*2)/100.0) * 100
+                graph.add_edge(as_lkw, as_key)
+                graph.labels[as_key] = key
+                graph.weights[as_key] = weight
+
+                if with_datatypes:
+                    for uri in self._struct.keys():
+                        if uri.split('/')[-2] == key:
+                            datatype = self._struct[uri]
+                            graph.add_edge(as_key, datatype)
+                            graph.weights[datatype] = 10
+                            graph.labels[datatype] = datatype
+
+                traverse(key, as_key)
+
+        traverse('projects', 'projects')
+
+        return graph
+
+
+class PaintGraph(object):
+    def __init__(self, interface):
+        self._intf = interface
+        self.get_graph = interface._get_graph
+
+    def architecture(self, with_datatypes=True, save=None):
+        graph = self.get_graph.architecture(with_datatypes)
+
+        plt.figure(figsize=(8, 8))
+        pos = graphviz_layout(graph, prog='twopi', args='')
+
+        # node_size = [(float(graph.degree(v)) * 5)**3 for v in graph]
+        # node_size = [graph.weights[v] ** 2 for v in graph]
+        # node_color = [float(graph.degree(v)) for v in graph]
+        # node_color = [graph.weights[v] ** 2 for v in graph]
+
+        cost = lambda v: float(graph.degree(v)) ** 3 + \
+            graph.weights[v] ** 2
+
+        costs = norm_costs([cost(v) for v in graph], 10000)
+
+        nx.draw(graph, pos, labels=graph.labels,
+                node_size=costs, node_color=costs,
+                font_size=13, font_color='orange',
+                font_weight='bold', with_labels=True
+                )
+
+        plt.axis('off')
+
+        if save is not None:
+            plt.savefig(save)
+
+        plt.show()
+
+    def experiments(self, save=None):
+        graph = self.get_graph.rest_resource('experiments')
+        self._draw_rest_resource(graph, save=None)
+
+    def assessors(self, save=None):
+        graph = self.get_graph.rest_resource('assessors')
+        self._draw_rest_resource(graph, save=None)
+
+    def reconstructions(self, save=None):
+        graph = self.get_graph.rest_resource('reconstructions')
+        self._draw_rest_resource(graph, save=None)
+
+    def scans(self):
+        graph = self.get_graph.rest_resource('scans')
+        self._draw_rest_resource(graph)
+
+    def _draw_rest_resource(self, graph, save=None):
+        plt.figure(figsize=(8, 8))
+        pos = graphviz_layout(graph, prog='twopi', args='')
+
+        cost = lambda v: float(graph.degree(v)) ** 3 + \
+            graph.weights[v] ** 2
+
+        node_size = [cost(v) for v in graph]
+        # node_size = [graph.weights[v] ** 2 for v in graph]
+        # node_color = [float(graph.degree(v)) for v in graph]
+        node_color = [cost(v) for v in graph]
+
+        nx.draw(graph, pos,
+                node_size=node_size, node_color=node_color,
+                font_size=13, font_color='green', font_weight='bold'
+                )
+
+        plt.axis('off')
+
+        if save is not None:
+            plt.savefig(save)
+
+        plt.show()
+
+    def datatypes(self, pattern='*', save=None):
+        graph = self.get_graph.datatypes(pattern)
+
+        plt.figure(figsize=(8, 8))
+        pos = graphviz_layout(graph, prog='twopi', args='')
+
+        cost = lambda v: float(graph.degree(v)) ** 3 + \
+            graph.weights[v] ** 2
+
+        node_size = [cost(v) for v in graph]
+        # node_size = [graph.weights[v] ** 2 for v in graph]
+        # node_color = [float(graph.degree(v)) for v in graph]
+        node_color = [cost(v) for v in graph]
+
+        nx.draw(graph, pos,
+                node_size=node_size, node_color=node_color,
+                font_size=13, font_color='green', font_weight='bold',
+                with_labels=True
+                )
+
+        plt.axis('off')
+
+        if save is not None:
+            plt.savefig(save)
+
+        plt.show()
+
+    def field_values(self, field_name, save=None):
+        graph = self.get_graph.field_values(field_name)
+
+        plt.figure(figsize=(8, 8))
+        pos = graphviz_layout(graph, prog='twopi', args='')
+
+        cost = lambda v: graph.weights[v]
+
+        graph.weights[field_name] = max([cost(v) for v in graph]) / 2.0
+
+        costs = norm_costs([cost(v) for v in graph], 10000)
+
+        nx.draw(graph, pos,
+                node_size=costs, node_color=costs,
+                font_size=13, font_color='black',
+                font_weight='bold', with_labels=True
+                )
+
+        plt.axis('off')
+
+        if save is not None:
+            plt.savefig(save)
+
+        plt.show()
+
+
+def norm_costs(costs, norm=1000):
+    max_cost = max(costs)
+
+    return [(cost / max_cost) * norm for cost in costs]
+
+
+# class GraphDrawer(object):
+#     def __init__(self, interface):
+#         self._intf = interface
+
+#     def datatypes(self, project):
+#         self._intf.connection.set_strategy('offline')
+
+#         experiments_types = self._intf.inspect.datatypes.experiments(project)
+
+#         labels = {project:project, 'Experiments':'Experiments'}
+
+#         g = nx.Graph()
+
+#         g.add_edge(project, 'Experiments', {'weight':1})
+
+#         for exp_type in experiments_types:
+#             g.add_edge('Experiments', exp_type, {'weight':8})
+#             labels[exp_type] = exp_type
+
+#         pos = nx.graphviz_layout(g, prog='twopi', args='')
+
+#         nx.draw_networkx_nodes(g, pos,
+#                                nodelist=[project],
+#                                node_color='green', alpha=0.7,
+#                                node_size=2500, node_shape='s')
+
+#         nx.draw_networkx_nodes(g, pos,
+#                                nodelist=['Experiments'],
+#                                node_color='blue', alpha=0.7,
+#                                node_size=2000, node_shape='p')
+
+#         nx.draw_networkx_nodes(g, pos,
+#                                nodelist=experiments_types,
+#                                node_color='red', alpha=0.7,
+#                                node_size=1500, node_shape='o')
+
+#         nx.draw_networkx_edges(g, pos, width=2, alpha=0.5,
+#                                edge_color='black')
+
+#         nx.draw_networkx_labels(g, pos, labels,
+#                                 alpha=0.9, font_size=8,
+#                                 font_color='black', font_weight='bold')
+
+#         plt.axis('off')
+#         plt.show()
+
+#         self._intf.connection.revert_strategy()
+
+class SchemasInspector(object):
+    def __init__(self, interface):
+        self._intf = interface
+
+    def __call__(self):
+        self._intf.manage.schemas()
+
+        for xsd in self._intf.manage.schemas():
+            print('-'*40)
+            print(xsd.upper())
+            print('-'*40)
+            print()
+
+            trees = self._intf.manage.schemas._trees[xsd]
+            for datatype in schema.datatypes(trees):
+                print('[%s]' % datatype)
+                print()
+
+                for path in schema.datatype_attributes(trees, datatype):
+                    print(path)
+
+                print()
+
+    def look_for(self, element_name, datatype_name=None):
+        paths = []
+        self._intf.manage.schemas._init()
+
+        if ':' in element_name:
+            for root in self._intf.manage.schemas._trees.values():
+                paths.extend(schema.datatype_attributes(root, element_name))
+            return paths
+
+        for xsd in self._intf.manage.schemas():
+            # nsmap = self._intf.manage.schemas._trees[xsd].nsmap
+            trees = self._intf.manage.schemas._trees[xsd]
+            if datatype_name is not None:
+                datatypes = [datatype_name]
+            else:
+                datatypes = schema.datatypes(trees)
+
+            for datatype in datatypes:
+                for path in schema.datatype_attributes(trees, datatype):
+                    if element_name in path:
+                        paths.append(path)
+
+        return paths
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/httputil.py` & `bbrc-pyxnat-1.6/pyxnat/core/httputil.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
-_boundary = '----------ThIs_Is_tHe_bouNdaRY_$'
-_crlf = '\r\n'
-
-
-def file_message(content, content_type, path, name):
-    body = []
-    body.append('--' + _boundary)
-    body.append('Content-Disposition: form-data; '
-                'name="%s"; filename="%s"' % (path, name)
-                )
-    body.append('Content-Type: %s' % content_type)
-    body.append('')
-
-    body.append(content)
-    body.append('--' + _boundary + '--')
-    body.append('')
-    body = _crlf.join(body)
-    content_type = 'multipart/form-data; boundary=%s' % _boundary
-
-    return body, content_type
+
+_boundary = '----------ThIs_Is_tHe_bouNdaRY_$'
+_crlf = '\r\n'
+
+
+def file_message(content, content_type, path, name):
+    body = []
+    body.append('--' + _boundary)
+    body.append('Content-Disposition: form-data; '
+                'name="%s"; filename="%s"' % (path, name)
+                )
+    body.append('Content-Type: %s' % content_type)
+    body.append('')
+
+    body.append(content)
+    body.append('--' + _boundary + '--')
+    body.append('')
+    body = _crlf.join(body)
+    content_type = 'multipart/form-data; boundary=%s' % _boundary
+
+    return body, content_type
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/interfaces.py` & `bbrc-pyxnat-1.6/pyxnat/core/interfaces.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,606 +1,606 @@
-import os
-import time
-import getpass
-import json
-import requests
-
-try:
-    import socks
-except ImportError:
-    socks = None
-
-import six
-if six.PY2:
-    from urlparse import urlparse
-    input = raw_input
-elif six.PY3:
-    from urllib.parse import urlparse
-
-from .select import Select
-from .help import Inspector, GraphData, PaintGraph, _DRAW_GRAPHS
-from .manage import GlobalManager
-from .uriutil import join_uri, file_path, uri_last
-from .jsonutil import csv_to_json
-from .errors import is_xnat_error
-from .errors import catch_error
-from .array import ArrayData
-from .xpath_store import XpathStore
-from . import xpass
-from . import derivatives
-
-
-DEBUG = False
-STUBBORN = False
-
-
-# generic classes
-def __get_modules__(m):
-    import pkgutil
-    modules = []
-    prefix = m.__name__ + '.'
-    for importer, modname, ispkg in pkgutil.iter_modules(m.__path__, prefix):
-        module = __import__(modname, fromlist='dummy')
-        if not ispkg:
-            modules.append(module)
-        else:
-            modules.extend(__get_modules__(module))
-    return modules
-
-
-def __find_all_functions__(m):
-    import inspect
-    functions = {}
-    modules = __get_modules__(m)
-    for m in modules:
-        for name, obj in inspect.getmembers(m):
-            if inspect.isfunction(obj):
-                functions.setdefault(m, []).append(obj)
-    return functions
-
-
-# main entry point
-class Interface(object):
-    """ Main entry point to access an XNAT server.
-
-        >>> central = Interface(server='http://central.xnat.org:8080',
-                                user='login',
-                                password='pwd')
-
-        Or with config file:
-
-        >>> central = Interface(config='/home/me/.xnat.cfg')
-
-        Or for interactive use:
-
-        >>> central = Interface('http://central.xnat.org')
-
-        .. note::
-            The interactive mode is triggered whenever an argument (between
-            server, user or password) is missing. In interactive mode pyxnat
-            will check that connection settings are valid.
-
-        .. note::
-            Proxy support requires the socks module be installed. This can be
-            installed via pip::
-
-            `pip install SocksiPy-branch`
-
-        Or anonymously (unauthenticated):
-
-        >>> central = Interface('http://central.xnat.org', anonymous=True)
-    """
-
-    def __init__(self, server=None, user=None, password=None, config=None,
-                 anonymous=False, proxy=None, verify=None):
-        """
-            Parameters
-            ----------
-            server: string | None
-                The server's full URL (including port and XNAT instance name
-                if necessary) e.g. http://central.xnat.org,
-                http://localhost:8080/xnat_db
-                If None the user will be prompted for it.
-            user: string | None
-                A valid login registered through the XNAT web interface.
-                If None the user will be prompted for it.
-            password: string | None
-                The user's password.
-                If None the user will be prompted for it.
-
-            config: string
-                Reads a config file in json to get the connection parameters.
-                If a config file is specified, it will be used regardless of
-                other parameters that might have been given.
-            anonymous: boolean
-                Indicates an unauthenticated connection.  If True, user
-                and password are ignored and a session is started with
-                no credentials.
-            proxy: string | None
-                Indicates the full URL for an HTTP proxy server to be used for
-                transactions with the specified XNAT server. If you need to
-                specify a username and password for proxy access, prepend them
-                to the hostname:
-                http://user:pass@hostname:port
-
-            verify: True, False, or path to file containing certificate for
-              your site. Added to the requests Session, as documented here:
-              http://docs.python-requests.org/en/latest/user/advanced/#ssl-cert-verification
-              Simplifies handling self-certified sites, or sites where there
-              is an issue with certification
-
-        """
-
-        self._interactive = False
-        self._anonymous = anonymous
-        self._verify = verify
-
-        if self._anonymous:
-
-            if server is None:
-                self._server = input('Server: ')
-                self._interactive = True
-            else:
-                self._server = server
-                self._interactive = False
-
-            self.__set_proxy(proxy)
-
-            self._user = None
-            self._pwd = None
-
-        else:
-
-            if not all([server, user, password]) and not config:
-                self._interactive = True
-
-            if all(arg is None
-                    for arg in [server, user, password, config]) \
-                    and os.path.exists(xpass.path()):
-
-                connection_args = xpass.read_xnat_pass(xpass.path())
-
-                if connection_args is None:
-                    raise Exception('XNAT configuration file not found '
-                                    'or formatted incorrectly.')
-
-                self._server = connection_args['host']
-                self._user = connection_args['u']
-                self._pwd = connection_args['p']
-
-                if 'proxy' in connection_args:
-                    self.__set_proxy(connection_args['proxy'])
-                else:
-                    self.__set_proxy(None)
-
-            elif config is not None:
-                self.load_config(config)
-
-            else:
-                if server is None:
-                    self._server = input('Server: ')
-                else:
-                    self._server = server
-
-                if user is None:
-                    user = input('User: ')
-
-                if password is None:
-                    password = getpass.getpass()
-
-                self._user = user
-                self._pwd = password
-
-                self.__set_proxy(proxy)
-
-        self._callback = None
-
-        self._struct = {}
-        self._entry = None
-        self._jsession = None  # 'authentication_by_credentials'
-        self._connect_extras = {}
-        self._connect()
-
-        self.inspect = Inspector(self)
-        self.select = Select(self)
-        self.array = ArrayData(self)
-        self.manage = GlobalManager(self)
-        self.xpath = XpathStore(self)
-
-        functions = __find_all_functions__(derivatives)
-        d = {}
-        for m, mod_functions in functions.items():
-            if hasattr(m, 'XNAT_RESOURCE_NAME'):
-                d[m.XNAT_RESOURCE_NAME] = mod_functions
-            elif hasattr(m, 'XNAT_RESOURCE_NAMES'):
-                for each in m.XNAT_RESOURCE_NAMES:
-                    d[each] = mod_functions
-        self._mod_functions = d
-
-        if _DRAW_GRAPHS:
-            self._get_graph = GraphData(self)
-            self.draw = PaintGraph(self)
-
-        if self._interactive:
-            self._get_entry_point()
-
-        self.inspect()
-
-    def __getstate__(self):
-        return {
-            '_server': self._server,
-            '_user': self._user,
-            '_pwd': self._pwd,
-            '_anonymous': self._anonymous,
-        }
-
-    def __setstate__(self, dictionary):
-        self.__dict__ = dictionary
-        if self._anonymous:
-            self.__init__(self._server, anonymous=True)
-        else:
-            self.__init__(self._server, self._user, self._pwd)
-
-    def __set_proxy(self, proxy=None):
-        if proxy is None:
-            proxy = os.environ.get("http_proxy")
-        if proxy is None:
-            self._proxy_url = None
-        else:
-            self._proxy_url = urlparse(proxy)
-
-    def _get_entry_point(self):
-        if self._entry is None:
-            # /REST for XNAT 1.4, /data if >=1.5
-            self._entry = '/REST'
-            try:
-                ans = self._exec('/data/JSESSION', force_preemptive_auth=True)
-                self._jsession = 'JSESSIONID=' + str(ans)
-                self._entry = '/data'
-
-                if is_xnat_error(self._jsession):
-                    catch_error(self._jsession)
-            except Exception as e:
-                if '/data/JSESSION' not in str(e):
-                    raise e
-
-        return self._entry
-
-    def _connect(self, **kwargs):
-        """ Sets up the connection with the XNAT server.
-
-            Parameters
-            ----------
-            kwargs: dict
-                Can be used to pass additional arguments to
-                the Http constructor. See the httplib2 documentation
-                for details. http://code.google.com/p/httplib2/
-        """
-
-        if kwargs != {}:
-            self._connect_extras = kwargs
-        else:
-            kwargs = self._connect_extras
-
-        self._http = requests.Session()
-
-        # requests verify defaults to True, but can be set from environment
-        # variables Leave as-is unless user has explicitly overridden it
-        if self._verify is not None:
-            self._http.verify = self._verify
-
-        if not self._anonymous:
-            self._http.auth = (self._user, self._pwd)
-
-        if self._proxy_url:
-            self._http.proxies = {'http': self._proxy_url.geturl()}
-
-        # Turns out this doesn't work any more: XNAT doesn't do the 401
-        # response that forces httplib2 to re-submit the request with
-        # credentials. See where the Authorization header is added manually in
-        # the _exec function.
-        # if not self._anonymous:
-        #    self._http.add_credentials(self._user, self._pwd)
-
-    def _exec(self, uri, method='GET', body=None, headers=None,
-              force_preemptive_auth=False, **kwargs):
-        """ A wrapper around a simple httplib2.request call that:
-                - avoids repeating the server url in the request
-                - deals with custom caching mechanisms :: Depricated
-                - manages a user session with cookies
-                - catches and broadcast specific XNAT errors
-
-            Parameters
-            ----------
-            uri: string
-                URI of the resource to be accessed. e.g. /REST/projects
-            method: GET | PUT | POST | DELETE | HEAD
-                HTTP method.
-            body: string | dict
-                HTTP message body
-            headers: dict
-                Additional headers for the HTTP request.
-            force_preemptive_auth: boolean
-                .. note:: Depricated as of 1.0.0.0
-                Indicates whether the request should include an Authorization
-                header with basic auth credentials.
-            **kwargs: dictionary
-                Additional parameters to pass directly to the Requests HTTP
-                call.
-
-            HTTP:GET
-            ----------
-                When calling with GET as method, the body parameter can be a
-                key:value dictionary containing request parameters or a string
-                of parameters. They will be url encoded and appended to the
-                url.
-
-            HTTP:POST
-            ----------
-                When calling with POST as method, the body parameter can be a
-                key:value dictionary containing request parameters they will
-                be url encoded and appended to the url.
-
-        """
-
-        if headers is None:
-            headers = {}
-
-        self._get_entry_point()
-
-        uri = join_uri(self._server, uri)
-
-        if DEBUG:
-            print(uri)
-
-        response = None
-
-        def request(method, uri, headers, body, kwargs):
-            if method == 'PUT':
-                response = self._http.put(uri, headers=headers, data=body,
-                                          **kwargs)
-            elif method == 'GET':
-                response = self._http.get(uri, headers=headers, params=body,
-                                          **kwargs)
-            elif method == 'POST':
-                response = self._http.post(uri, headers=headers, data=body,
-                                           **kwargs)
-            elif method == 'DELETE':
-                response = self._http.delete(uri, headers=headers, data=body,
-                                             **kwargs)
-            elif method == 'HEAD':
-                response = self._http.head(uri, headers=headers, data=body,
-                                           **kwargs)
-            else:
-                print('Unsupported HTTP method (%s)' % method)
-                return
-            return response
-
-        response = request(method, uri, headers, body, kwargs)
-        if response is None:
-            return
-
-        # Dirty trick to help Travis CI tests on CENTRAL: consider fixing it
-        if STUBBORN:
-            if (response is not None and response.status_code == 500):
-                print('Retrying request... %s' % uri)
-                response = request(method, uri, headers, body, kwargs)
-
-        if (response is not None and not response.ok) or \
-           is_xnat_error(response.content):
-            if DEBUG:
-                print(response.content)
-                print(response.status_code)
-
-            catch_error(response.content, '''pyxnat._exec failure:
-                    URI: {response.url}
-                    status code: {response.status_code}
-                    headers: {response.headers}
-                    content: {response.content}
-                '''.format(response=response))
-
-        return response.content
-
-    def _get_json(self, uri):
-        """ Specific Interface._exec method to retrieve data.
-            It forces the data format to csv and then puts it back to a
-            json-like format.
-
-            Parameters
-            ----------
-            uri: string
-                URI of the resource to be accessed. e.g. /REST/projects
-
-            Returns
-            -------
-            List of dicts containing the results
-        """
-        if 'format=json' in uri:
-            uri = uri.replace('format=json', 'format=csv')
-        else:
-            if '?' in uri:
-                uri += '&format=csv'
-            else:
-                uri += '?format=csv'
-
-        content = self._exec(uri, 'GET')
-
-        if is_xnat_error(content):
-            catch_error(content)
-
-        json_content = csv_to_json(content)
-
-        # add the (relative) path field for files
-        base_uri = uri.split('?')[0]
-        if uri_last(base_uri) == 'files':
-            for element in json_content:
-                element['path'] = file_path(element['URI'])
-        return json_content
-
-    def _get_head(self, uri):
-        if DEBUG:
-            print('GET HEAD')
-
-        response = self._http.head('{server}{uri}'.format(server=self._server,
-                                                          uri=uri))
-
-        if not response.ok:
-            time.sleep(1)
-            self._http.head('{server}{uri}'.format(server=self._server,
-                                                   uri=uri))
-
-        return response.headers
-
-    def save_config(self, location):
-        """ Saves current configuration - including password - in a file.
-
-            .. warning::
-                Since the password is saved as well, make sure the file
-                is saved at a safe location with appropriate permissions.
-
-            .. note::
-                This method raises NotImplementedError for an anonymous
-                interface.
-
-            Parameters
-            ----------
-            location: string
-                Destination config file.
-        """
-        if self._anonymous:
-            raise NotImplementedError(
-                'no save_config() for anonymous interfaces')
-
-        if not os.path.exists(os.path.dirname(location)):
-            os.makedirs(os.path.dirname(location))
-
-        config = {'server': self._server,
-                  'user': self._user,
-                  'password': self._pwd,
-                  }
-        if self._verify:
-            config['verify'] = self._verify
-
-        if self._proxy_url:
-            config['proxy'] = self._proxy_url.geturl()
-
-        with open(location, 'w') as fp:
-            json.dump(config, fp)
-
-    def load_config(self, location):
-        """ Loads a configuration file and replaces current connection
-            parameters.
-
-            .. note::
-                This method raises NotImplementedError for an anonymous
-                interface.
-
-            Parameters
-            ----------
-            location: string
-                Configuration file path.
-        """
-        if self._anonymous:
-            raise NotImplementedError(
-                'no load_config() for anonymous interfaces')
-
-        if os.path.exists(location):
-            with open(location, 'rb') as fp:
-                config = json.load(fp)
-
-            self._server = str(config['server'])
-            self._user = str(config['user'])
-            self._pwd = str(config['password'])
-
-            self._verify = bool(config.get('verify', True))
-            if 'proxy' in config:
-                self.__set_proxy(str(config['proxy']))
-            else:
-                self.__set_proxy(None)
-
-        else:
-            raise Exception('Configuration file does not exist.')
-
-    def version(self):
-        """
-            Get version of the currently running XNAT instance.
-        """
-        from pyxnat.core.errors import DatabaseError
-        try:
-            return self._exec('/data/version')
-        except DatabaseError:
-            j = self._exec('/xapi/siteConfig/buildInfo').decode()
-            return json.loads(j)
-
-    def set_logging(self, level=0):
-        pass
-
-    def disconnect(self):
-        """
-            Tell XNAT to disconnect this session
-        """
-        self._exec('/data/JSESSION', method='DELETE')
-        self._http.close()
-
-    def get(self, uri, **kwargs):
-        '''
-        Wrapper around requests.get()
-        returns rquests.response object
-        '''
-        uri = join_uri(self._server, uri)
-        response = self._http.get(uri, **kwargs)
-        return response
-
-    def put(self, uri, **kwargs):
-        '''
-        Wrapper around requests.put()
-        returns rquests.response object
-        '''
-        uri = join_uri(self._server, uri)
-        response = self._http.put(uri, **kwargs)
-        return response
-
-    def post(self, uri, **kwargs):
-        '''
-        Wrapper around requests.post()
-        returns rquests.response object
-        '''
-        uri = join_uri(self._server, uri)
-        response = self._http.post(uri, **kwargs)
-        return response
-
-    def delete(self, uri, **kwargs):
-        '''
-        Wrapper around requests.delete()
-        returns rquests.response object
-        '''
-        uri = join_uri(self._server, uri)
-        response = self._http.delete(uri, **kwargs)
-        return response
-
-    def head(self, uri, **kwargs):
-        '''
-        Wrapper around requests.head()
-        returns rquests.response object
-        '''
-        uri = join_uri(self._server, uri)
-        response = self._http.head(uri, **kwargs)
-        return response
-
-    def __enter__(self):
-
-        return self
-
-    def close_jsession(self):
-        '''
-        Closes the session with XNAT server and consumes the JSESSIONID token.
-        '''
-        uri = '/data/JSESSION'
-        response = self.delete(uri)
-        response.raise_for_status()
-        self._jsession = None
-
-    def __exit__(self, type, value, traceback):
-
-        if self._jsession:
-            self.close_jsession()
-        self._http.close()
+import os
+import time
+import getpass
+import json
+import requests
+
+try:
+    import socks
+except ImportError:
+    socks = None
+
+import six
+if six.PY2:
+    from urlparse import urlparse
+    input = raw_input
+elif six.PY3:
+    from urllib.parse import urlparse
+
+from .select import Select
+from .help import Inspector, GraphData, PaintGraph, _DRAW_GRAPHS
+from .manage import GlobalManager
+from .uriutil import join_uri, file_path, uri_last
+from .jsonutil import csv_to_json
+from .errors import is_xnat_error
+from .errors import catch_error
+from .array import ArrayData
+from .xpath_store import XpathStore
+from . import xpass
+from . import derivatives
+
+
+DEBUG = False
+STUBBORN = False
+
+
+# generic classes
+def __get_modules__(m):
+    import pkgutil
+    modules = []
+    prefix = m.__name__ + '.'
+    for importer, modname, ispkg in pkgutil.iter_modules(m.__path__, prefix):
+        module = __import__(modname, fromlist='dummy')
+        if not ispkg:
+            modules.append(module)
+        else:
+            modules.extend(__get_modules__(module))
+    return modules
+
+
+def __find_all_functions__(m):
+    import inspect
+    functions = {}
+    modules = __get_modules__(m)
+    for m in modules:
+        for name, obj in inspect.getmembers(m):
+            if inspect.isfunction(obj):
+                functions.setdefault(m, []).append(obj)
+    return functions
+
+
+# main entry point
+class Interface(object):
+    """ Main entry point to access an XNAT server.
+
+        >>> central = Interface(server='http://central.xnat.org:8080',
+                                user='login',
+                                password='pwd')
+
+        Or with config file:
+
+        >>> central = Interface(config='/home/me/.xnat.cfg')
+
+        Or for interactive use:
+
+        >>> central = Interface('http://central.xnat.org')
+
+        .. note::
+            The interactive mode is triggered whenever an argument (between
+            server, user or password) is missing. In interactive mode pyxnat
+            will check that connection settings are valid.
+
+        .. note::
+            Proxy support requires the socks module be installed. This can be
+            installed via pip::
+
+            `pip install SocksiPy-branch`
+
+        Or anonymously (unauthenticated):
+
+        >>> central = Interface('http://central.xnat.org', anonymous=True)
+    """
+
+    def __init__(self, server=None, user=None, password=None, config=None,
+                 anonymous=False, proxy=None, verify=None):
+        """
+            Parameters
+            ----------
+            server: string | None
+                The server's full URL (including port and XNAT instance name
+                if necessary) e.g. http://central.xnat.org,
+                http://localhost:8080/xnat_db
+                If None the user will be prompted for it.
+            user: string | None
+                A valid login registered through the XNAT web interface.
+                If None the user will be prompted for it.
+            password: string | None
+                The user's password.
+                If None the user will be prompted for it.
+
+            config: string
+                Reads a config file in json to get the connection parameters.
+                If a config file is specified, it will be used regardless of
+                other parameters that might have been given.
+            anonymous: boolean
+                Indicates an unauthenticated connection.  If True, user
+                and password are ignored and a session is started with
+                no credentials.
+            proxy: string | None
+                Indicates the full URL for an HTTP proxy server to be used for
+                transactions with the specified XNAT server. If you need to
+                specify a username and password for proxy access, prepend them
+                to the hostname:
+                http://user:pass@hostname:port
+
+            verify: True, False, or path to file containing certificate for
+              your site. Added to the requests Session, as documented here:
+              http://docs.python-requests.org/en/latest/user/advanced/#ssl-cert-verification
+              Simplifies handling self-certified sites, or sites where there
+              is an issue with certification
+
+        """
+
+        self._interactive = False
+        self._anonymous = anonymous
+        self._verify = verify
+
+        if self._anonymous:
+
+            if server is None:
+                self._server = input('Server: ')
+                self._interactive = True
+            else:
+                self._server = server
+                self._interactive = False
+
+            self.__set_proxy(proxy)
+
+            self._user = None
+            self._pwd = None
+
+        else:
+
+            if not all([server, user, password]) and not config:
+                self._interactive = True
+
+            if all(arg is None
+                    for arg in [server, user, password, config]) \
+                    and os.path.exists(xpass.path()):
+
+                connection_args = xpass.read_xnat_pass(xpass.path())
+
+                if connection_args is None:
+                    raise Exception('XNAT configuration file not found '
+                                    'or formatted incorrectly.')
+
+                self._server = connection_args['host']
+                self._user = connection_args['u']
+                self._pwd = connection_args['p']
+
+                if 'proxy' in connection_args:
+                    self.__set_proxy(connection_args['proxy'])
+                else:
+                    self.__set_proxy(None)
+
+            elif config is not None:
+                self.load_config(config)
+
+            else:
+                if server is None:
+                    self._server = input('Server: ')
+                else:
+                    self._server = server
+
+                if user is None:
+                    user = input('User: ')
+
+                if password is None:
+                    password = getpass.getpass()
+
+                self._user = user
+                self._pwd = password
+
+                self.__set_proxy(proxy)
+
+        self._callback = None
+
+        self._struct = {}
+        self._entry = None
+        self._jsession = None  # 'authentication_by_credentials'
+        self._connect_extras = {}
+        self._connect()
+
+        self.inspect = Inspector(self)
+        self.select = Select(self)
+        self.array = ArrayData(self)
+        self.manage = GlobalManager(self)
+        self.xpath = XpathStore(self)
+
+        functions = __find_all_functions__(derivatives)
+        d = {}
+        for m, mod_functions in functions.items():
+            if hasattr(m, 'XNAT_RESOURCE_NAME'):
+                d[m.XNAT_RESOURCE_NAME] = mod_functions
+            elif hasattr(m, 'XNAT_RESOURCE_NAMES'):
+                for each in m.XNAT_RESOURCE_NAMES:
+                    d[each] = mod_functions
+        self._mod_functions = d
+
+        if _DRAW_GRAPHS:
+            self._get_graph = GraphData(self)
+            self.draw = PaintGraph(self)
+
+        if self._interactive:
+            self._get_entry_point()
+
+        self.inspect()
+
+    def __getstate__(self):
+        return {
+            '_server': self._server,
+            '_user': self._user,
+            '_pwd': self._pwd,
+            '_anonymous': self._anonymous,
+        }
+
+    def __setstate__(self, dictionary):
+        self.__dict__ = dictionary
+        if self._anonymous:
+            self.__init__(self._server, anonymous=True)
+        else:
+            self.__init__(self._server, self._user, self._pwd)
+
+    def __set_proxy(self, proxy=None):
+        if proxy is None:
+            proxy = os.environ.get("http_proxy")
+        if proxy is None:
+            self._proxy_url = None
+        else:
+            self._proxy_url = urlparse(proxy)
+
+    def _get_entry_point(self):
+        if self._entry is None:
+            # /REST for XNAT 1.4, /data if >=1.5
+            self._entry = '/REST'
+            try:
+                ans = self._exec('/data/JSESSION', force_preemptive_auth=True)
+                self._jsession = 'JSESSIONID=' + str(ans)
+                self._entry = '/data'
+
+                if is_xnat_error(self._jsession):
+                    catch_error(self._jsession)
+            except Exception as e:
+                if '/data/JSESSION' not in str(e):
+                    raise e
+
+        return self._entry
+
+    def _connect(self, **kwargs):
+        """ Sets up the connection with the XNAT server.
+
+            Parameters
+            ----------
+            kwargs: dict
+                Can be used to pass additional arguments to
+                the Http constructor. See the httplib2 documentation
+                for details. http://code.google.com/p/httplib2/
+        """
+
+        if kwargs != {}:
+            self._connect_extras = kwargs
+        else:
+            kwargs = self._connect_extras
+
+        self._http = requests.Session()
+
+        # requests verify defaults to True, but can be set from environment
+        # variables Leave as-is unless user has explicitly overridden it
+        if self._verify is not None:
+            self._http.verify = self._verify
+
+        if not self._anonymous:
+            self._http.auth = (self._user, self._pwd)
+
+        if self._proxy_url:
+            self._http.proxies = {'http': self._proxy_url.geturl()}
+
+        # Turns out this doesn't work any more: XNAT doesn't do the 401
+        # response that forces httplib2 to re-submit the request with
+        # credentials. See where the Authorization header is added manually in
+        # the _exec function.
+        # if not self._anonymous:
+        #    self._http.add_credentials(self._user, self._pwd)
+
+    def _exec(self, uri, method='GET', body=None, headers=None,
+              force_preemptive_auth=False, **kwargs):
+        """ A wrapper around a simple httplib2.request call that:
+                - avoids repeating the server url in the request
+                - deals with custom caching mechanisms :: Depricated
+                - manages a user session with cookies
+                - catches and broadcast specific XNAT errors
+
+            Parameters
+            ----------
+            uri: string
+                URI of the resource to be accessed. e.g. /REST/projects
+            method: GET | PUT | POST | DELETE | HEAD
+                HTTP method.
+            body: string | dict
+                HTTP message body
+            headers: dict
+                Additional headers for the HTTP request.
+            force_preemptive_auth: boolean
+                .. note:: Depricated as of 1.0.0.0
+                Indicates whether the request should include an Authorization
+                header with basic auth credentials.
+            **kwargs: dictionary
+                Additional parameters to pass directly to the Requests HTTP
+                call.
+
+            HTTP:GET
+            ----------
+                When calling with GET as method, the body parameter can be a
+                key:value dictionary containing request parameters or a string
+                of parameters. They will be url encoded and appended to the
+                url.
+
+            HTTP:POST
+            ----------
+                When calling with POST as method, the body parameter can be a
+                key:value dictionary containing request parameters they will
+                be url encoded and appended to the url.
+
+        """
+
+        if headers is None:
+            headers = {}
+
+        self._get_entry_point()
+
+        uri = join_uri(self._server, uri)
+
+        if DEBUG:
+            print(uri)
+
+        response = None
+
+        def request(method, uri, headers, body, kwargs):
+            if method == 'PUT':
+                response = self._http.put(uri, headers=headers, data=body,
+                                          **kwargs)
+            elif method == 'GET':
+                response = self._http.get(uri, headers=headers, params=body,
+                                          **kwargs)
+            elif method == 'POST':
+                response = self._http.post(uri, headers=headers, data=body,
+                                           **kwargs)
+            elif method == 'DELETE':
+                response = self._http.delete(uri, headers=headers, data=body,
+                                             **kwargs)
+            elif method == 'HEAD':
+                response = self._http.head(uri, headers=headers, data=body,
+                                           **kwargs)
+            else:
+                print('Unsupported HTTP method (%s)' % method)
+                return
+            return response
+
+        response = request(method, uri, headers, body, kwargs)
+        if response is None:
+            return
+
+        # Dirty trick to help Travis CI tests on CENTRAL: consider fixing it
+        if STUBBORN:
+            if (response is not None and response.status_code == 500):
+                print('Retrying request... %s' % uri)
+                response = request(method, uri, headers, body, kwargs)
+
+        if (response is not None and not response.ok) or \
+           is_xnat_error(response.content):
+            if DEBUG:
+                print(response.content)
+                print(response.status_code)
+
+            catch_error(response.content, '''pyxnat._exec failure:
+                    URI: {response.url}
+                    status code: {response.status_code}
+                    headers: {response.headers}
+                    content: {response.content}
+                '''.format(response=response))
+
+        return response.content
+
+    def _get_json(self, uri):
+        """ Specific Interface._exec method to retrieve data.
+            It forces the data format to csv and then puts it back to a
+            json-like format.
+
+            Parameters
+            ----------
+            uri: string
+                URI of the resource to be accessed. e.g. /REST/projects
+
+            Returns
+            -------
+            List of dicts containing the results
+        """
+        if 'format=json' in uri:
+            uri = uri.replace('format=json', 'format=csv')
+        else:
+            if '?' in uri:
+                uri += '&format=csv'
+            else:
+                uri += '?format=csv'
+
+        content = self._exec(uri, 'GET')
+
+        if is_xnat_error(content):
+            catch_error(content)
+
+        json_content = csv_to_json(content)
+
+        # add the (relative) path field for files
+        base_uri = uri.split('?')[0]
+        if uri_last(base_uri) == 'files':
+            for element in json_content:
+                element['path'] = file_path(element['URI'])
+        return json_content
+
+    def _get_head(self, uri):
+        if DEBUG:
+            print('GET HEAD')
+
+        response = self._http.head('{server}{uri}'.format(server=self._server,
+                                                          uri=uri))
+
+        if not response.ok:
+            time.sleep(1)
+            self._http.head('{server}{uri}'.format(server=self._server,
+                                                   uri=uri))
+
+        return response.headers
+
+    def save_config(self, location):
+        """ Saves current configuration - including password - in a file.
+
+            .. warning::
+                Since the password is saved as well, make sure the file
+                is saved at a safe location with appropriate permissions.
+
+            .. note::
+                This method raises NotImplementedError for an anonymous
+                interface.
+
+            Parameters
+            ----------
+            location: string
+                Destination config file.
+        """
+        if self._anonymous:
+            raise NotImplementedError(
+                'no save_config() for anonymous interfaces')
+
+        if not os.path.exists(os.path.dirname(location)):
+            os.makedirs(os.path.dirname(location))
+
+        config = {'server': self._server,
+                  'user': self._user,
+                  'password': self._pwd,
+                  }
+        if self._verify:
+            config['verify'] = self._verify
+
+        if self._proxy_url:
+            config['proxy'] = self._proxy_url.geturl()
+
+        with open(location, 'w') as fp:
+            json.dump(config, fp)
+
+    def load_config(self, location):
+        """ Loads a configuration file and replaces current connection
+            parameters.
+
+            .. note::
+                This method raises NotImplementedError for an anonymous
+                interface.
+
+            Parameters
+            ----------
+            location: string
+                Configuration file path.
+        """
+        if self._anonymous:
+            raise NotImplementedError(
+                'no load_config() for anonymous interfaces')
+
+        if os.path.exists(location):
+            with open(location, 'rb') as fp:
+                config = json.load(fp)
+
+            self._server = str(config['server'])
+            self._user = str(config['user'])
+            self._pwd = str(config['password'])
+
+            self._verify = bool(config.get('verify', True))
+            if 'proxy' in config:
+                self.__set_proxy(str(config['proxy']))
+            else:
+                self.__set_proxy(None)
+
+        else:
+            raise Exception('Configuration file does not exist.')
+
+    def version(self):
+        """
+            Get version of the currently running XNAT instance.
+        """
+        from pyxnat.core.errors import DatabaseError
+        try:
+            return self._exec('/data/version')
+        except DatabaseError:
+            j = self._exec('/xapi/siteConfig/buildInfo').decode()
+            return json.loads(j)
+
+    def set_logging(self, level=0):
+        pass
+
+    def disconnect(self):
+        """
+            Tell XNAT to disconnect this session
+        """
+        self._exec('/data/JSESSION', method='DELETE')
+        self._http.close()
+
+    def get(self, uri, **kwargs):
+        '''
+        Wrapper around requests.get()
+        returns rquests.response object
+        '''
+        uri = join_uri(self._server, uri)
+        response = self._http.get(uri, **kwargs)
+        return response
+
+    def put(self, uri, **kwargs):
+        '''
+        Wrapper around requests.put()
+        returns rquests.response object
+        '''
+        uri = join_uri(self._server, uri)
+        response = self._http.put(uri, **kwargs)
+        return response
+
+    def post(self, uri, **kwargs):
+        '''
+        Wrapper around requests.post()
+        returns rquests.response object
+        '''
+        uri = join_uri(self._server, uri)
+        response = self._http.post(uri, **kwargs)
+        return response
+
+    def delete(self, uri, **kwargs):
+        '''
+        Wrapper around requests.delete()
+        returns rquests.response object
+        '''
+        uri = join_uri(self._server, uri)
+        response = self._http.delete(uri, **kwargs)
+        return response
+
+    def head(self, uri, **kwargs):
+        '''
+        Wrapper around requests.head()
+        returns rquests.response object
+        '''
+        uri = join_uri(self._server, uri)
+        response = self._http.head(uri, **kwargs)
+        return response
+
+    def __enter__(self):
+
+        return self
+
+    def close_jsession(self):
+        '''
+        Closes the session with XNAT server and consumes the JSESSIONID token.
+        '''
+        uri = '/data/JSESSION'
+        response = self.delete(uri)
+        response.raise_for_status()
+        self._jsession = None
+
+    def __exit__(self, type, value, traceback):
+
+        if self._jsession:
+            self.close_jsession()
+        self._http.close()
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/jsonutil.py` & `bbrc-pyxnat-1.6/pyxnat/core/jsonutil.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,346 +1,346 @@
-import csv
-import copy
-from fnmatch import fnmatch
-import json
-
-import six
-if six.PY2:
-    from StringIO import StringIO
-elif six.PY3:
-    unicode = str
-    from io import StringIO
-
-# jdata is a list of dicts
-
-
-def join_tables(join_column, jdata, *jtables):
-    indexes = []
-
-    for jtable in [jdata]+list(jtables):
-        if isinstance(jtable, dict):
-            jtable = [jtable]
-        index = {}
-        [index.setdefault(entry[join_column], entry) for entry in jtable]
-        indexes.append(index)
-
-    merged_jdata = []
-    for join_id in indexes[0].keys():
-        for index in indexes[1:]:
-            indexes[0][join_id].update(index[join_id])
-            merged_jdata.append(indexes[0][join_id])
-
-    return merged_jdata
-
-
-def get_column(jdata, col, val_pattern='*'):
-    if isinstance(jdata, dict):
-        jdata = [jdata]
-
-    if val_pattern == '*':
-        return [entry[col] for entry in jdata if col in entry]
-    else:
-        return [entry[col] for entry in jdata
-                if fnmatch(entry.get(col), val_pattern)
-                ]
-
-
-def get_where(jdata, *args, **kwargs):
-    if isinstance(jdata, dict):
-        jdata = [jdata]
-
-    match = []
-
-    for entry in jdata:
-        match_args = all([arg in entry.keys() or arg in entry.values()
-                          for arg in args
-                          ])
-
-        match_kwargs = all([entry[key] == kwargs[key]
-                            for key in kwargs.keys()
-                            ])
-
-        if match_args and match_kwargs:
-            match.append(entry)
-
-    return match
-
-
-def get_where_not(jdata, *args, **kwargs):
-    if isinstance(jdata, dict):
-        jdata = [jdata]
-
-    match = []
-
-    for entry in jdata:
-        match_args = all([arg in entry.keys() or arg in entry.values()
-                          for arg in args
-                          ])
-
-        match_kwargs = all([entry[key] == kwargs[key]
-                            for key in kwargs.keys()
-                            ])
-
-        if not match_args and not match_kwargs:
-            match.append(entry)
-
-    return match
-
-
-def get_headers(jdata):
-    if isinstance(jdata, dict):
-        jdata = [jdata]
-    return [] if jdata == [] else jdata[0].keys()
-
-
-def get_selection(jdata, columns):
-    if isinstance(jdata, dict):
-        jdata = [jdata]
-
-    sub_table = copy.deepcopy(jdata)
-
-    rmcols = set(get_headers(jdata)).difference(columns)
-
-    for entry in sub_table:
-        for col in rmcols:
-            if col in entry.keys():
-                del entry[col]
-
-    return sub_table
-
-
-def csv_to_json(csv_str):
-
-    import csv
-    import six
-    if six.PY2:
-        csv_reader = csv.reader(StringIO(csv_str), delimiter=',',
-                                quotechar='"')
-    elif six.PY3:
-        try:
-            csv_reader = csv.reader(StringIO(csv_str), delimiter=',',
-                                    quotechar='"')
-        except TypeError:
-            csv_reader = csv.reader(StringIO(csv_str.decode('utf-8')),
-                                    delimiter=',', quotechar='"')
-    headers = next(csv_reader)
-    ans = [dict(zip(headers, entry)) for entry in csv_reader]
-    return ans
-
-
-class JsonTable(object):
-    """ Wrapper around a list of dictionnaries to provide utility functions.
-    """
-    def __init__(self, jdata, order_by=[]):
-        self.data = jdata
-        self.order_by = order_by
-
-    def __repr__(self):
-        # if len(self.data) == 0:
-        #     return '[]'
-        # elif len(self.data) == 1:
-        #     return str(self.data[0])
-
-        if len(self.headers()) <= 5:
-            _headers = self.headers()
-        else:
-            _headers = '%s ... %s' % (','.join(list(self.headers())[:2]),
-                                      ','.join(list(self.headers())[-2:])
-                                      )
-
-        return '<JsonTable %s:%s> %s' % (
-            len(self.data), len(self.headers()), _headers
-            )
-
-        # return ('[%s\n .\n .\n . \n%s]\n\n'
-        #         '------------\n'
-        #         '%s rows\n'
-        #         '%s columns\n'
-        #         '%s characters') % (str(self.data[0]),
-        #                             str(self.data[-1]),
-        #                             len(self),
-        #                             len(self.headers()),
-        #                             len(self.dumps_csv())
-        #                             )
-
-    def __str__(self):
-        return self.dumps_csv()
-
-    def __len__(self):
-        return len(self.data)
-
-    def __iter__(self):
-        return iter(self.data)
-
-    def __getitem__(self, name):
-        if isinstance(name, (str, unicode)):
-            return self.get(name)
-        elif isinstance(name, int):
-            return self.__class__([self.data[name]], self.order_by)
-        elif isinstance(name, list):
-            return self.select(name)
-
-    def __getslice__(self, i, j):
-        return self.__class__(self.data[i:j], self.order_by)
-
-    def join(self, join_column, *jtables):
-        """ Join jsontables with a common column.
-
-            Parameters
-            ----------
-            join_column: string
-                The name or header of the join column.
-            jtables: *args
-                Other  jtables.
-        """
-        return self.__class__(
-            join_tables(join_column, self.data,
-                        *[jtable.data for jtable in jtables]),
-            self.order_by
-            )
-
-    def has_header(self, name):
-        return name in self.headers()
-
-    def headers(self):
-        """ Returns the headers of the object.
-        """
-        return get_headers(self.data)
-
-    def get(self, col, val_pattern='*', always_list=False):
-        """ Gets a single column value.
-
-            Parameters
-            ----------
-            col: string
-                The column name
-            val_pattern: string
-                Enable a filter on the values to be returned.
-            always_list: boolean
-                If only a single value is to be returned - i.e. there
-                is only on element in the list of dicts or there is only
-                one match against the value filter - is can be returned
-                within a list (with True) or not (default).
-        """
-        res = get_column(self.data, col, val_pattern)
-        if always_list:
-            return res
-        if len(self.data) == 1:
-            return res[0]
-        return res
-
-    def where(self, *args, **kwargs):
-        """ Filters the object.
-
-            Paramaters
-            ----------
-            args:
-                Value must be matched in the key or the value of an entry.
-            kwargs:
-                Value for a specific key must be matched in an entry.
-
-            Returns
-            -------
-            A :class:`JsonTable` containing the matches.
-        """
-        return self.__class__(get_where(self.data, *args, **kwargs),
-                              self.order_by
-                              )
-
-    def where_not(self, *args, **kwargs):
-        """ Filters the object. Conditions must not be matched.
-
-            Paramaters
-            ----------
-            args:
-                Value must not be matched in the key or the value of an
-                entry.
-            kwargs:
-                Value for a specific key must not be matched in an entry.
-
-            Returns
-            -------
-            A :class:`JsonTable` containing the not matches.
-        """
-        return self.__class__(get_where_not(self.data, *args, **kwargs),
-                              self.order_by
-                              )
-
-    def select(self, columns):
-        """ Select only some columns of interest.
-
-            Returns
-            -------
-            A :class:`JsonTable` with the selected columns.
-        """
-        return self.__class__(get_selection(self.data, columns),
-                              self.order_by
-                              )
-
-    def dump_csv(self, dest, delimiter=','):
-        """ Dumps the object content in a csv file format.
-
-            Parameters
-            ----------
-            dest: string
-                Destination file path.
-            delimiter: char
-                Character to separate values in the csv file.
-        """
-        fd = open(dest, 'w')
-        fd.write(self.dumps_csv(delimiter))
-        fd.close()
-
-    def dumps_csv(self, delimiter=','):
-        str_buffer = StringIO()
-        csv_writer = csv.writer(str_buffer, delimiter=delimiter,
-                                quotechar='"', quoting=csv.QUOTE_MINIMAL)
-
-        for entry in self.as_list():
-            csv_writer.writerow(unicode(entry))
-
-        return str_buffer.getvalue()
-
-    def dump_json(self, dest):
-        fd = open(dest, 'w')
-        fd.write(self.dumps_json())
-        fd.close()
-
-    def dumps_json(self):
-        return json.dumps(self.data)
-
-    def as_list(self):
-        table = [[]]
-
-        for header in self.order_by:
-            if header in self.headers():
-                table[0].append(header)
-        for header in self.headers():
-            if header not in self.order_by:
-                table[0].append(header)
-
-        for entry in self.data:
-            row = []
-            for header in self.order_by:
-                if header in entry.keys():
-                    row.append(entry.get(header))
-            for header in self.headers():
-                if header not in self.order_by:
-                    row.append(entry.get(header))
-            table.append(row)
-
-        return table
-
-    def items(self):
-        table = []
-
-        for entry in self.data:
-            row = ()
-            for header in self.order_by:
-                if header in entry.keys():
-                    row += (entry.get(header), )
-            for header in self.headers():
-                if header not in self.order_by:
-                    row += (entry.get(header), )
-            table.append(row)
-
-        return table
+import csv
+import copy
+from fnmatch import fnmatch
+import json
+
+import six
+if six.PY2:
+    from StringIO import StringIO
+elif six.PY3:
+    unicode = str
+    from io import StringIO
+
+# jdata is a list of dicts
+
+
+def join_tables(join_column, jdata, *jtables):
+    indexes = []
+
+    for jtable in [jdata]+list(jtables):
+        if isinstance(jtable, dict):
+            jtable = [jtable]
+        index = {}
+        [index.setdefault(entry[join_column], entry) for entry in jtable]
+        indexes.append(index)
+
+    merged_jdata = []
+    for join_id in indexes[0].keys():
+        for index in indexes[1:]:
+            indexes[0][join_id].update(index[join_id])
+            merged_jdata.append(indexes[0][join_id])
+
+    return merged_jdata
+
+
+def get_column(jdata, col, val_pattern='*'):
+    if isinstance(jdata, dict):
+        jdata = [jdata]
+
+    if val_pattern == '*':
+        return [entry[col] for entry in jdata if col in entry]
+    else:
+        return [entry[col] for entry in jdata
+                if fnmatch(entry.get(col), val_pattern)
+                ]
+
+
+def get_where(jdata, *args, **kwargs):
+    if isinstance(jdata, dict):
+        jdata = [jdata]
+
+    match = []
+
+    for entry in jdata:
+        match_args = all([arg in entry.keys() or arg in entry.values()
+                          for arg in args
+                          ])
+
+        match_kwargs = all([entry[key] == kwargs[key]
+                            for key in kwargs.keys()
+                            ])
+
+        if match_args and match_kwargs:
+            match.append(entry)
+
+    return match
+
+
+def get_where_not(jdata, *args, **kwargs):
+    if isinstance(jdata, dict):
+        jdata = [jdata]
+
+    match = []
+
+    for entry in jdata:
+        match_args = all([arg in entry.keys() or arg in entry.values()
+                          for arg in args
+                          ])
+
+        match_kwargs = all([entry[key] == kwargs[key]
+                            for key in kwargs.keys()
+                            ])
+
+        if not match_args and not match_kwargs:
+            match.append(entry)
+
+    return match
+
+
+def get_headers(jdata):
+    if isinstance(jdata, dict):
+        jdata = [jdata]
+    return [] if jdata == [] else jdata[0].keys()
+
+
+def get_selection(jdata, columns):
+    if isinstance(jdata, dict):
+        jdata = [jdata]
+
+    sub_table = copy.deepcopy(jdata)
+
+    rmcols = set(get_headers(jdata)).difference(columns)
+
+    for entry in sub_table:
+        for col in rmcols:
+            if col in entry.keys():
+                del entry[col]
+
+    return sub_table
+
+
+def csv_to_json(csv_str):
+
+    import csv
+    import six
+    if six.PY2:
+        csv_reader = csv.reader(StringIO(csv_str), delimiter=',',
+                                quotechar='"')
+    elif six.PY3:
+        try:
+            csv_reader = csv.reader(StringIO(csv_str), delimiter=',',
+                                    quotechar='"')
+        except TypeError:
+            csv_reader = csv.reader(StringIO(csv_str.decode('utf-8')),
+                                    delimiter=',', quotechar='"')
+    headers = next(csv_reader)
+    ans = [dict(zip(headers, entry)) for entry in csv_reader]
+    return ans
+
+
+class JsonTable(object):
+    """ Wrapper around a list of dictionnaries to provide utility functions.
+    """
+    def __init__(self, jdata, order_by=[]):
+        self.data = jdata
+        self.order_by = order_by
+
+    def __repr__(self):
+        # if len(self.data) == 0:
+        #     return '[]'
+        # elif len(self.data) == 1:
+        #     return str(self.data[0])
+
+        if len(self.headers()) <= 5:
+            _headers = self.headers()
+        else:
+            _headers = '%s ... %s' % (','.join(list(self.headers())[:2]),
+                                      ','.join(list(self.headers())[-2:])
+                                      )
+
+        return '<JsonTable %s:%s> %s' % (
+            len(self.data), len(self.headers()), _headers
+            )
+
+        # return ('[%s\n .\n .\n . \n%s]\n\n'
+        #         '------------\n'
+        #         '%s rows\n'
+        #         '%s columns\n'
+        #         '%s characters') % (str(self.data[0]),
+        #                             str(self.data[-1]),
+        #                             len(self),
+        #                             len(self.headers()),
+        #                             len(self.dumps_csv())
+        #                             )
+
+    def __str__(self):
+        return self.dumps_csv()
+
+    def __len__(self):
+        return len(self.data)
+
+    def __iter__(self):
+        return iter(self.data)
+
+    def __getitem__(self, name):
+        if isinstance(name, (str, unicode)):
+            return self.get(name)
+        elif isinstance(name, int):
+            return self.__class__([self.data[name]], self.order_by)
+        elif isinstance(name, list):
+            return self.select(name)
+
+    def __getslice__(self, i, j):
+        return self.__class__(self.data[i:j], self.order_by)
+
+    def join(self, join_column, *jtables):
+        """ Join jsontables with a common column.
+
+            Parameters
+            ----------
+            join_column: string
+                The name or header of the join column.
+            jtables: *args
+                Other  jtables.
+        """
+        return self.__class__(
+            join_tables(join_column, self.data,
+                        *[jtable.data for jtable in jtables]),
+            self.order_by
+            )
+
+    def has_header(self, name):
+        return name in self.headers()
+
+    def headers(self):
+        """ Returns the headers of the object.
+        """
+        return get_headers(self.data)
+
+    def get(self, col, val_pattern='*', always_list=False):
+        """ Gets a single column value.
+
+            Parameters
+            ----------
+            col: string
+                The column name
+            val_pattern: string
+                Enable a filter on the values to be returned.
+            always_list: boolean
+                If only a single value is to be returned - i.e. there
+                is only on element in the list of dicts or there is only
+                one match against the value filter - is can be returned
+                within a list (with True) or not (default).
+        """
+        res = get_column(self.data, col, val_pattern)
+        if always_list:
+            return res
+        if len(self.data) == 1:
+            return res[0]
+        return res
+
+    def where(self, *args, **kwargs):
+        """ Filters the object.
+
+            Paramaters
+            ----------
+            args:
+                Value must be matched in the key or the value of an entry.
+            kwargs:
+                Value for a specific key must be matched in an entry.
+
+            Returns
+            -------
+            A :class:`JsonTable` containing the matches.
+        """
+        return self.__class__(get_where(self.data, *args, **kwargs),
+                              self.order_by
+                              )
+
+    def where_not(self, *args, **kwargs):
+        """ Filters the object. Conditions must not be matched.
+
+            Paramaters
+            ----------
+            args:
+                Value must not be matched in the key or the value of an
+                entry.
+            kwargs:
+                Value for a specific key must not be matched in an entry.
+
+            Returns
+            -------
+            A :class:`JsonTable` containing the not matches.
+        """
+        return self.__class__(get_where_not(self.data, *args, **kwargs),
+                              self.order_by
+                              )
+
+    def select(self, columns):
+        """ Select only some columns of interest.
+
+            Returns
+            -------
+            A :class:`JsonTable` with the selected columns.
+        """
+        return self.__class__(get_selection(self.data, columns),
+                              self.order_by
+                              )
+
+    def dump_csv(self, dest, delimiter=','):
+        """ Dumps the object content in a csv file format.
+
+            Parameters
+            ----------
+            dest: string
+                Destination file path.
+            delimiter: char
+                Character to separate values in the csv file.
+        """
+        fd = open(dest, 'w')
+        fd.write(self.dumps_csv(delimiter))
+        fd.close()
+
+    def dumps_csv(self, delimiter=','):
+        str_buffer = StringIO()
+        csv_writer = csv.writer(str_buffer, delimiter=delimiter,
+                                quotechar='"', quoting=csv.QUOTE_MINIMAL)
+
+        for entry in self.as_list():
+            csv_writer.writerow(unicode(entry))
+
+        return str_buffer.getvalue()
+
+    def dump_json(self, dest):
+        fd = open(dest, 'w')
+        fd.write(self.dumps_json())
+        fd.close()
+
+    def dumps_json(self):
+        return json.dumps(self.data)
+
+    def as_list(self):
+        table = [[]]
+
+        for header in self.order_by:
+            if header in self.headers():
+                table[0].append(header)
+        for header in self.headers():
+            if header not in self.order_by:
+                table[0].append(header)
+
+        for entry in self.data:
+            row = []
+            for header in self.order_by:
+                if header in entry.keys():
+                    row.append(entry.get(header))
+            for header in self.headers():
+                if header not in self.order_by:
+                    row.append(entry.get(header))
+            table.append(row)
+
+        return table
+
+    def items(self):
+        table = []
+
+        for entry in self.data:
+            row = ()
+            for header in self.order_by:
+                if header in entry.keys():
+                    row += (entry.get(header), )
+            for header in self.headers():
+                if header not in self.order_by:
+                    row += (entry.get(header), )
+            table.append(row)
+
+        return table
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/manage.py` & `bbrc-pyxnat-1.6/pyxnat/core/manage.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,308 +1,308 @@
-from lxml import etree
-import urllib
-from .search import SearchManager
-from .users import Users
-from .resources import Project
-from .tags import Tags
-from .jsonutil import JsonTable
-
-
-class GlobalManager(object):
-    """ Mainly a container class to provide a clean interface for all
-        management classes.
-    """
-
-    def __init__(self, interface):
-        self._intf = interface
-
-        self.search = SearchManager(self._intf)
-        self.users = Users(self._intf)
-        self.tags = Tags(self._intf)
-        self.schemas = SchemaManager(self._intf)
-        self.prearchive = PreArchive(self._intf)
-
-    def register_callback(self, func):
-        """ Defines a callback to execute when collections of resources are
-            accessed.
-
-            Parameters
-            ----------
-            func: callable
-                A callable that takes the current collection object as first
-                argument and the current element object as second argument.
-
-            Examples
-            --------
-            >>> def notify(cobj, eobj):
-            >>>    print eobj._uri
-            >>> interface.manage.register_callback(notify)
-        """
-        self._intf._callback = func
-
-    def unregister_callback(self):
-        """ Unregisters the callback.
-        """
-        self._intf._callback = None
-
-    def project(self, project_id):
-        """ Returns a project manager.
-        """
-        return ProjectManager(project_id, self._intf)
-
-
-class ProjectManager(object):
-    """ Management interface for projects.
-
-        This functionalities are also available through `Project` objects.
-    """
-
-    def __init__(self, project_id, interface):
-
-        self._intf = interface
-        self._intf._get_entry_point()
-
-        project = Project('%s/projects/%s' % (self._intf._entry,
-                                              project_id
-                                              ),
-                          self._intf
-                          )
-
-        self.prearchive_code = project.prearchive_code
-        self.set_prearchive_code = project.set_prearchive_code
-        self.quarantine_code = project.quarantine_code
-        self.set_quarantine_code = project.set_quarantine_code
-        self.current_arc = project.current_arc
-        self.set_subfolder_in_current_arc = \
-            project.set_subfolder_in_current_arc
-        self.accessibility = project.accessibility
-        self.users = project.users
-        self.owners = project.owners
-        self.members = project.members
-        self.collaborators = project.collaborators
-        self.user_role = project.user_role
-        self.add_user = project.add_user
-        self.remove_user = project.remove_user
-
-
-class SchemaManager(object):
-    """ Management interface for XNAT schemas.
-
-        The aim is to provide a minimal set of functionalities to parse
-        and look at XNAT schemas.
-    """
-
-    def __init__(self, interface):
-        self._intf = interface
-        self._trees = {}
-
-    def __call__(self):
-        return self._trees.keys()
-
-    def add(self, url):
-        """ Loads an additional schema.
-
-            Parameters
-            ----------
-            url: str
-                url of the schema relative to the server.
-                    e.g. for
-                    http://central.xnat.org/xapi/schemas/xnat give
-                    ``/xapi/schemas/xnat``
-
-        """
-
-        # if not re.match('/?schemas/.*/.*\.xsd', url):
-        #    if not 'schemas' in url and re.match('/?\w+/\w+[.]xsd', url):
-        #        url = join_uri('/schemas', url)
-        #
-        #    elif not re.match('^[^/].xsd', url):
-        #        url = '/schemas/%s/%s'%(url.split('.xsd')[0], url)
-        #    else:
-        #        raise NotImplementedError
-
-        self._trees[url.split('/')[-1]] = \
-            etree.fromstring(self._intf._exec(url))
-
-    def remove(self, name):
-        """ Removes a schema.
-        """
-        if name in self._trees.keys():
-            del self._trees[name]
-
-
-"""
-   Fields Of the Prearchive
-   ------------------------
-   Each session in the prearchive
-    has the following fields:
-       "project" - The name of the project. "Unassigned" if the session is
-            unassigned.
-       "timestamp" - The time (down to millisecond) that this session was
-            received by XNAT. "20110603_124835868" for example.
-       "lastmod" - The time this session as last modified. Moving, resetting
-            etc. updates this time
-       "uploaded" - The time this session was uploaded to XNAT. Usually the
-            same as "timestamp"
-       "scan_date" - The date this session was scanned.
-       "scan_time" - The time this session was scanned.
-       "subject" - The name of the subject
-       "folderName" - The id of this session. Corresponds to XNAT's session id,
-       "name" - The name of this session. Corresponds to XNAT's session label.
-       "tag" - This session's unique DICOM identifier. Usually the SOP
-            instance UID.
-       "status" - The current status of this session
-       "url" - The unique uri of this session.
-       "autoarchive" - Whether this session should be auto-archived.
-    For more in-depth information about the prearchive see:
-    http://docs.xnat.org/Using+the+Prearchive#XNAT%201.5:%20Managing%20Data%20with%20the%20Prearchive-Operations-Session%20Status
-
-    Uniquely identifying a session
-    ------------------------------
-    Every session in the prearchive uniquely is identified by "project",
-    "timestamp" and "folderName".
-    (13/7/2011) - Each session could have been uniquely identified by the "url"
-                  field or the "tag" field. These are arguably more elegant
-                  identifiers but for now the "project", "timestamp",
-                  "folderName" triple is used.
-
-"""
-
-
-class PreArchive(object):
-    def __init__(self, interface):
-        self._intf = interface
-
-    """
-    Retrieve the status of a session
-    Parameters
-    ----------
-       triple - A list containing the project, timestamp and session id, in
-       that order.
-    """
-    def status(self, triple):
-        return JsonTable(
-            self._intf._get_json('/data/prearchive/projects')
-            ).where(
-            project=triple[0], timestamp=triple[1], folderName=triple[2]
-            ).get('status')
-
-    """
-    Retrieve the contents of the prearchive.
-    """
-    def get(self):
-        return JsonTable(self._intf._get_json('/data/prearchive/projects'),
-                         ['project', 'timestamp', 'folderName']
-                         ).select(['project', 'timestamp', 'folderName']
-                                  ).as_list()[1:]
-
-    """
-    Retrieve the scans of a give session triple
-    Parameters
-    ----------
-       triple - A list containing the project, timestamp and session id, in
-       that order.
-    """
-    def get_scans(self, triple):
-        return JsonTable(self._intf._get_json(
-                '/data/prearchive/projects/%s/scans'
-                % '/'.join(triple))).get('ID')
-
-    """
-    Retrieve the resource of a session triple
-    Parameters
-    ----------
-       triple - A list containing the project, timestamp and session id, in
-       that order.
-       scan_id - id of the scan
-    """
-    def get_resources(self, triple, scan_id):
-        return JsonTable(self._intf._get_json(
-                '/data/prearchive/projects/%s'
-                '/scans/%s/resources' % ('/'.join(triple), scan_id)
-                )).get('label')
-
-    """
-    Retrieve a list of files in a given session triple
-    Parameters
-    ----------
-       triple - A list containing the project, timestamp and session id, in
-       that order.
-       scan_id - id of the scan
-       resource_id - id of the resource
-    """
-    def get_files(self, triple, scan_id, resource_id):
-        return JsonTable(self._intf._get_json(
-                '/data/prearchive/projects/%s'
-                '/scans/%s/resources/%s/files' % ('/'.join(triple),
-                                                  scan_id,
-                                                  resource_id)
-                )).get('Name')
-
-    """
-    Move multiple sessions to a project in the prearchive asynchronously.
-    If only one session is it is done now.
-
-    This does *not* archive a session.
-
-    Parameters
-    ----------
-       uris - a list of session uris
-       new_project - The name of the project to which to move the sessions.
-    """
-
-    def move(self, uris, new_project):
-        add_src = lambda u: urllib.urlencode({'src': u})
-
-        async_ = len(uris) > 1 and 'true' or 'false'
-        print(async_)
-
-        post_body = '&'.join((map(add_src, uris)) +
-                             [urllib.urlencode({'newProject': new_project})] +
-                             [urllib.urlencode({'async': async_})])
-
-        request_uri = '/data/services/prearchive/move?format=csv'
-        ct = {'content-type': 'application/x-www-form-urlencoded'}
-        return self._intf._exec(request_uri, 'POST', post_body, ct)
-
-    """
-    Reinspect the file on the filesystem on the XNAT server and recreate the
-    parameters of the file. Essentially a refresh of the file.
-
-    Be warned that if this session has been scheduled for an operation, that
-    operation is cancelled.
-    Parameters
-    ----------
-       uris - a list of session uris
-       new_project - The name of the project to which to move the sessions.
-    """
-
-    def reset(self, triple):
-        post_body = "action=build"
-        request_uri = '/data/prearchive/projects/%s?format=single' \
-                      % '/'.join(triple)
-        ct = {'content-type': 'application/x-www-form-urlencoded'}
-        return self._intf._exec(request_uri, 'POST', post_body, ct)
-
-    """
-    Delete  a session from the prearchive
-    Parameters
-    ----------
-       uri - The uri of the session to delete
-    """
-
-    def delete(self, uri):
-        post_body = "src=" + uri + "&" + "async=false"
-        request_uri = "/data/services/prearchive/delete?format=csv"
-        ct = {'content-type': 'application/x-www-form-urlencoded'}
-        return self._intf._exec(request_uri, 'POST', post_body, ct)
-    """
-    Get the uri of the given session.
-    Parameters
-    ----------
-       triple - A list containing the project, timestamp and session id, in
-       that order.
-    """
-    def get_uri(self, triple):
-        j = JsonTable(self._intf._get_json('/data/prearchive/projects'))
-        return j.where(project=triple[0], timestamp=triple[1],
-                       folderName=triple[2]).get('url')
+from lxml import etree
+import urllib
+from .search import SearchManager
+from .users import Users
+from .resources import Project
+from .tags import Tags
+from .jsonutil import JsonTable
+
+
+class GlobalManager(object):
+    """ Mainly a container class to provide a clean interface for all
+        management classes.
+    """
+
+    def __init__(self, interface):
+        self._intf = interface
+
+        self.search = SearchManager(self._intf)
+        self.users = Users(self._intf)
+        self.tags = Tags(self._intf)
+        self.schemas = SchemaManager(self._intf)
+        self.prearchive = PreArchive(self._intf)
+
+    def register_callback(self, func):
+        """ Defines a callback to execute when collections of resources are
+            accessed.
+
+            Parameters
+            ----------
+            func: callable
+                A callable that takes the current collection object as first
+                argument and the current element object as second argument.
+
+            Examples
+            --------
+            >>> def notify(cobj, eobj):
+            >>>    print eobj._uri
+            >>> interface.manage.register_callback(notify)
+        """
+        self._intf._callback = func
+
+    def unregister_callback(self):
+        """ Unregisters the callback.
+        """
+        self._intf._callback = None
+
+    def project(self, project_id):
+        """ Returns a project manager.
+        """
+        return ProjectManager(project_id, self._intf)
+
+
+class ProjectManager(object):
+    """ Management interface for projects.
+
+        This functionalities are also available through `Project` objects.
+    """
+
+    def __init__(self, project_id, interface):
+
+        self._intf = interface
+        self._intf._get_entry_point()
+
+        project = Project('%s/projects/%s' % (self._intf._entry,
+                                              project_id
+                                              ),
+                          self._intf
+                          )
+
+        self.prearchive_code = project.prearchive_code
+        self.set_prearchive_code = project.set_prearchive_code
+        self.quarantine_code = project.quarantine_code
+        self.set_quarantine_code = project.set_quarantine_code
+        self.current_arc = project.current_arc
+        self.set_subfolder_in_current_arc = \
+            project.set_subfolder_in_current_arc
+        self.accessibility = project.accessibility
+        self.users = project.users
+        self.owners = project.owners
+        self.members = project.members
+        self.collaborators = project.collaborators
+        self.user_role = project.user_role
+        self.add_user = project.add_user
+        self.remove_user = project.remove_user
+
+
+class SchemaManager(object):
+    """ Management interface for XNAT schemas.
+
+        The aim is to provide a minimal set of functionalities to parse
+        and look at XNAT schemas.
+    """
+
+    def __init__(self, interface):
+        self._intf = interface
+        self._trees = {}
+
+    def __call__(self):
+        return self._trees.keys()
+
+    def add(self, url):
+        """ Loads an additional schema.
+
+            Parameters
+            ----------
+            url: str
+                url of the schema relative to the server.
+                    e.g. for
+                    http://central.xnat.org/xapi/schemas/xnat give
+                    ``/xapi/schemas/xnat``
+
+        """
+
+        # if not re.match('/?schemas/.*/.*\.xsd', url):
+        #    if not 'schemas' in url and re.match('/?\w+/\w+[.]xsd', url):
+        #        url = join_uri('/schemas', url)
+        #
+        #    elif not re.match('^[^/].xsd', url):
+        #        url = '/schemas/%s/%s'%(url.split('.xsd')[0], url)
+        #    else:
+        #        raise NotImplementedError
+
+        self._trees[url.split('/')[-1]] = \
+            etree.fromstring(self._intf._exec(url))
+
+    def remove(self, name):
+        """ Removes a schema.
+        """
+        if name in self._trees.keys():
+            del self._trees[name]
+
+
+"""
+   Fields Of the Prearchive
+   ------------------------
+   Each session in the prearchive
+    has the following fields:
+       "project" - The name of the project. "Unassigned" if the session is
+            unassigned.
+       "timestamp" - The time (down to millisecond) that this session was
+            received by XNAT. "20110603_124835868" for example.
+       "lastmod" - The time this session as last modified. Moving, resetting
+            etc. updates this time
+       "uploaded" - The time this session was uploaded to XNAT. Usually the
+            same as "timestamp"
+       "scan_date" - The date this session was scanned.
+       "scan_time" - The time this session was scanned.
+       "subject" - The name of the subject
+       "folderName" - The id of this session. Corresponds to XNAT's session id,
+       "name" - The name of this session. Corresponds to XNAT's session label.
+       "tag" - This session's unique DICOM identifier. Usually the SOP
+            instance UID.
+       "status" - The current status of this session
+       "url" - The unique uri of this session.
+       "autoarchive" - Whether this session should be auto-archived.
+    For more in-depth information about the prearchive see:
+    http://docs.xnat.org/Using+the+Prearchive#XNAT%201.5:%20Managing%20Data%20with%20the%20Prearchive-Operations-Session%20Status
+
+    Uniquely identifying a session
+    ------------------------------
+    Every session in the prearchive uniquely is identified by "project",
+    "timestamp" and "folderName".
+    (13/7/2011) - Each session could have been uniquely identified by the "url"
+                  field or the "tag" field. These are arguably more elegant
+                  identifiers but for now the "project", "timestamp",
+                  "folderName" triple is used.
+
+"""
+
+
+class PreArchive(object):
+    def __init__(self, interface):
+        self._intf = interface
+
+    """
+    Retrieve the status of a session
+    Parameters
+    ----------
+       triple - A list containing the project, timestamp and session id, in
+       that order.
+    """
+    def status(self, triple):
+        return JsonTable(
+            self._intf._get_json('/data/prearchive/projects')
+            ).where(
+            project=triple[0], timestamp=triple[1], folderName=triple[2]
+            ).get('status')
+
+    """
+    Retrieve the contents of the prearchive.
+    """
+    def get(self):
+        return JsonTable(self._intf._get_json('/data/prearchive/projects'),
+                         ['project', 'timestamp', 'folderName']
+                         ).select(['project', 'timestamp', 'folderName']
+                                  ).as_list()[1:]
+
+    """
+    Retrieve the scans of a give session triple
+    Parameters
+    ----------
+       triple - A list containing the project, timestamp and session id, in
+       that order.
+    """
+    def get_scans(self, triple):
+        return JsonTable(self._intf._get_json(
+                '/data/prearchive/projects/%s/scans'
+                % '/'.join(triple))).get('ID')
+
+    """
+    Retrieve the resource of a session triple
+    Parameters
+    ----------
+       triple - A list containing the project, timestamp and session id, in
+       that order.
+       scan_id - id of the scan
+    """
+    def get_resources(self, triple, scan_id):
+        return JsonTable(self._intf._get_json(
+                '/data/prearchive/projects/%s'
+                '/scans/%s/resources' % ('/'.join(triple), scan_id)
+                )).get('label')
+
+    """
+    Retrieve a list of files in a given session triple
+    Parameters
+    ----------
+       triple - A list containing the project, timestamp and session id, in
+       that order.
+       scan_id - id of the scan
+       resource_id - id of the resource
+    """
+    def get_files(self, triple, scan_id, resource_id):
+        return JsonTable(self._intf._get_json(
+                '/data/prearchive/projects/%s'
+                '/scans/%s/resources/%s/files' % ('/'.join(triple),
+                                                  scan_id,
+                                                  resource_id)
+                )).get('Name')
+
+    """
+    Move multiple sessions to a project in the prearchive asynchronously.
+    If only one session is it is done now.
+
+    This does *not* archive a session.
+
+    Parameters
+    ----------
+       uris - a list of session uris
+       new_project - The name of the project to which to move the sessions.
+    """
+
+    def move(self, uris, new_project):
+        add_src = lambda u: urllib.urlencode({'src': u})
+
+        async_ = len(uris) > 1 and 'true' or 'false'
+        print(async_)
+
+        post_body = '&'.join((map(add_src, uris)) +
+                             [urllib.urlencode({'newProject': new_project})] +
+                             [urllib.urlencode({'async': async_})])
+
+        request_uri = '/data/services/prearchive/move?format=csv'
+        ct = {'content-type': 'application/x-www-form-urlencoded'}
+        return self._intf._exec(request_uri, 'POST', post_body, ct)
+
+    """
+    Reinspect the file on the filesystem on the XNAT server and recreate the
+    parameters of the file. Essentially a refresh of the file.
+
+    Be warned that if this session has been scheduled for an operation, that
+    operation is cancelled.
+    Parameters
+    ----------
+       uris - a list of session uris
+       new_project - The name of the project to which to move the sessions.
+    """
+
+    def reset(self, triple):
+        post_body = "action=build"
+        request_uri = '/data/prearchive/projects/%s?format=single' \
+                      % '/'.join(triple)
+        ct = {'content-type': 'application/x-www-form-urlencoded'}
+        return self._intf._exec(request_uri, 'POST', post_body, ct)
+
+    """
+    Delete  a session from the prearchive
+    Parameters
+    ----------
+       uri - The uri of the session to delete
+    """
+
+    def delete(self, uri):
+        post_body = "src=" + uri + "&" + "async=false"
+        request_uri = "/data/services/prearchive/delete?format=csv"
+        ct = {'content-type': 'application/x-www-form-urlencoded'}
+        return self._intf._exec(request_uri, 'POST', post_body, ct)
+    """
+    Get the uri of the given session.
+    Parameters
+    ----------
+       triple - A list containing the project, timestamp and session id, in
+       that order.
+    """
+    def get_uri(self, triple):
+        j = JsonTable(self._intf._get_json('/data/prearchive/projects'))
+        return j.where(project=triple[0], timestamp=triple[1],
+                       folderName=triple[2]).get('url')
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/pathutil.py` & `bbrc-pyxnat-1.6/pyxnat/core/pathutil.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import os
-
-
-def find_files(src):
-    names = os.listdir(src)
-
-    errors = []
-    files = []
-
-    for name in names:
-        srcname = os.path.join(src, name)
-        try:
-            if os.path.islink(srcname):
-                linkto = os.readlink(srcname)
-                files.extend(find_files(linkto))
-                # os.symlink(linkto, dstname)
-            elif os.path.isdir(srcname):
-                files.extend(find_files(srcname))
-            else:
-                files.append(srcname)
-        except (IOError, os.error) as why:
-            errors.append((srcname, str(why)))
-
-    return files
-
-
-def ensure_dir_exists(dir_path):
-    if not os.path.exists(dir_path):
-        os.makedirs(dir_path)
-    return os.path.isdir(dir_path)
+import os
+
+
+def find_files(src):
+    names = os.listdir(src)
+
+    errors = []
+    files = []
+
+    for name in names:
+        srcname = os.path.join(src, name)
+        try:
+            if os.path.islink(srcname):
+                linkto = os.readlink(srcname)
+                files.extend(find_files(linkto))
+                # os.symlink(linkto, dstname)
+            elif os.path.isdir(srcname):
+                files.extend(find_files(srcname))
+            else:
+                files.append(srcname)
+        except (IOError, os.error) as why:
+            errors.append((srcname, str(why)))
+
+    return files
+
+
+def ensure_dir_exists(dir_path):
+    if not os.path.exists(dir_path):
+        os.makedirs(dir_path)
+    return os.path.isdir(dir_path)
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/pipelines.py` & `bbrc-pyxnat-1.6/pyxnat/core/pipelines.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,378 +1,378 @@
-import os.path as op
-
-# import six
-# if six.PY2:
-#     from urllib2 import urlopen
-# elif six.PY3:
-#     from urllib.request import urlopen
-
-# import smtplib
-# from copy import deepcopy
-# import email.mime.text
-# import xml.dom.minidom
-
-# import suds.client
-# import suds.xsd.doctor
-
-# from . import httputil
-
-
-class PipelineNotFoundError(Exception):
-    """workflow not found"""
-
-
-class Pipelines(object):
-
-    def __init__(self, project, interface):
-        self._intf = interface
-        self._project = project
-
-    def aliases(self):
-        """
-        Fetch the alias ID (stepId) of each available pipeline.
-        :return: Dictionary including pipeline IDs and aliases of all
-        available pipelines as keys and values respectively.
-        """
-        import xml.etree.ElementTree as eTree
-
-        namespace = {'archive': 'http://nrg.wustl.edu/arc'}
-
-        uri = '{}/archive_spec'.format(self._project.attrs.get('URI'))
-        data = self._intf.get(uri).content
-
-        # traverse XML sub-elements named 'pipeline' and get stepId attribute,
-        # Pipeline Engine uses stepID as actual ID for scheduling the pipeline
-        proj_specs = eTree.fromstring(data)
-        pipes_info = proj_specs.findall('archive:pipelines/archive:descendants/archive:'
-                                        'descendant/archive:pipeline', namespace)
-        aliases = {item.find('archive:name', namespace).text: item.attrib['stepId']
-                   for item in pipes_info}
-
-        return aliases
-
-    def info(self, pipeline_id=None):
-        """ Get information about the available pipelines.
-        """
-        response = self._intf.get('{}/pipelines'.format(self._project.attrs.get('URI')))
-        result = response.json()['ResultSet']['Result']
-        if pipeline_id:
-            result = [item for item in result if item['Name'] == pipeline_id]
-        return result
-
-    def pipeline(self, pipeline_id):
-        """ Return a pipeline object.
-        """
-        return Pipeline(pipeline_id, self._project, self._intf)
-
-    def add(self, location):
-        raise NotImplementedError
-        # f = open(location, 'rb')
-        # pip_doc = f.read()
-        # f.close()
-        #
-        # body, content_type = httputil.file_message(
-        #     pip_doc, 'text/xml', location, op.split(location)[1])
-        #
-        # pipeline_uri = '%s/projects/%s/pipelines/%s' % (
-        #     self._intf._get_entry_point(),
-        #     self._project,
-        #     op.split(location)[1]
-        #     )
-        #
-        # self._intf._exec(pipeline_uri,
-        #                  method='PUT',
-        #                  body=body,
-        #                  headers={'content-type': content_type}
-        #                  )
-
-    def delete(self, pipeline_id):
-        raise NotImplementedError
-
-
-class Pipeline(object):
-
-    def __init__(self, pipeline_id, project, interface):
-        self._intf = interface
-        self._project = project
-        self.id = pipeline_id
-        self.uri = '{}/pipelines/{}'.format(self._project.attrs.get('URI'), self.id)
-        # self.datatype = self._datatype()
-        # self.alias = self._alias()
-
-    def _alias(self):
-        """Fetch the alias ID of the pipeline (stepId) asserting its uniqueness.
-        """
-        proj_pipes = Pipelines(self._project, self._intf)
-        proj_aliases = proj_pipes.aliases()
-
-        alias = proj_aliases[self.id]
-        if list(proj_aliases.values()).count(alias) > 1:
-            raise ValueError('Pipeline {} alias ({}) is not unique in project {}.'
-                             .format(self.id, alias, self._project.id()))
-        return alias
-
-    def _datatype(self):
-        """Fetch the experiment datatype the pipeline applies to. If the
-        pipeline does not cope with an specific datatype, function returns
-        'All Datatypes'.
-        """
-        proj_pipes = Pipelines(self._project, self._intf)
-        info = proj_pipes.info(self.id).pop()
-
-        return info['Datatype']
-
-    def exists(self):
-        """ Test whether a pipeline exists in the given context.
-        """
-        response = self._intf.head(self.uri)
-        return response.ok
-
-    def info(self):
-        """ Get pipeline details.
-        """
-        if not self.exists():
-            raise PipelineNotFoundError('Pipeline {} not found in project {}.'
-                                        .format(self.id, self._project.id()))
-
-        response = self._intf.get(self.uri)
-        return response.json()
-
-    def run(self, experiment_id, params=None):
-        """ Run the pipeline on an experiment.
-        """
-        if not self.exists():
-            raise PipelineNotFoundError('Pipeline {} not found in project {}.'
-                                        .format(self.id, self._project.id()))
-
-        e = self._project.experiment(experiment_id)
-        if not e.exists():
-            raise ValueError('Experiment {} not found in project {}.'
-                             .format(experiment_id, self._project.id()))
-
-        datatype = self._datatype()
-        if datatype != 'All Datatypes' and datatype != e.datatype():
-            raise TypeError('Experiment {} does not match the pipeline\'s '
-                            'expected datatype ({}).'.format(experiment_id,
-                                                             datatype))
-
-        uri = '{}/experiments/{}'.format(self.uri.replace(self.id, self._alias()),
-                                         experiment_id)
-
-        response = self._intf.post(uri, params=params)
-        return response.raise_for_status()
-
-    def status(self, experiment_id):
-        """ Fetch latest pipeline execution status for the given experiment.
-        """
-        if not self.exists():
-            raise PipelineNotFoundError('Pipeline {} not found in project {}.'
-                                        .format(self.id, self._project.id()))
-
-        e = self._project.experiment(experiment_id)
-        if not e.exists():
-            raise ValueError('Experiment {} not found in project {}.'
-                             .format(experiment_id, self._project.id()))
-
-        uri = '/data/services/workflows/{}'.format(self.id)
-        options = {'project': self._project.id(),
-                   'experiment': experiment_id,
-                   'display': 'ALL',
-                   'format': 'json'}
-
-        response = self._intf.get(uri, params=options)
-        data = response.json()['ResultSet']['Result']
-        data = [item for item in data
-                if self.id == op.basename(op.splitext(item['pipeline_name'])[0])]
-
-        if not data:
-            status = None
-        else:
-            from operator import itemgetter
-            status = sorted(data, key=lambda x: int(x['wrk_workflowData_id'])).pop(-1)
-        return status
-
-    def stop(self):
-        pass
-
-    def update(self):
-        pass
-
-    def complete(self):
-        pass
-
-    def fail(self):
-        pass
-
-# class Pipeline(object):
-
-#     """class for mirroring workflow information (XML) in XNAT"""
-
-#     def __init__(self, base_url, username, password, workflow_id):
-#         self._base_url = base_url
-#         self._username = username
-#         self._password = password
-#         self._cookiejar = None
-#         res = self._call('CreateServiceSession.jws',
-#                          'execute',
-#                          (),
-#                          authenticated=True)
-#         self._session = str(res)
-#         args = (('ns1:string', self._session),
-#                 ('ns1:string', 'wrk:workflowData.ID'),
-#                 ('ns1:string', '='),
-#                 ('ns1:string', workflow_id),
-#                 ('ns1:string', 'wrk:workflowData'))
-#         workflow_ids = self._call('GetIdentifiers.jws', 'search', args)
-#         self._doc = None
-#         for w_id in workflow_ids:
-#             url = '%s/app/template/XMLSearch.vm/id/%s/data_type/wrk:workflowData' % (self._base_url, str(w_id))
-#             r = urllib2.Request(url)
-#             self._cookiejar.add_cookie_header(r)
-#             data = urllib2.urlopen(r).read()
-#             doc = xml.dom.minidom.parseString(data)
-#             workflow_node = doc.getElementsByTagName('wrk:Workflow')[0]
-#             status = workflow_node.getAttribute('status').lower()
-#             if status in ('queued', 'awaiting action', 'hold'):
-#                 self._doc = doc
-#                 break
-#         if self._doc is None:
-#             raise PipelineNotFoundError
-#         return
-
-#     def _call(self,
-#               jws,
-#               operation,
-#               inputs,
-#               authenticated=False,
-#               fix_import=False):
-#         """perform a SOAP call"""
-#         url = '%s/axis/%s' % (self._base_url, jws)
-#         if authenticated:
-#             t = suds.transport.http.HttpAuthenticated(username=self._username,
-#                                                       password=self._password)
-#         else:
-#             t = suds.transport.http.HttpTransport()
-#         if self._cookiejar is not None:
-#             t.cookiejar = self._cookiejar
-#         if fix_import:
-#             xsd_url = 'http://schemas.xmlsoap.org/soap/encoding/'
-#             imp = suds.xsd.doctor.Import(xsd_url)
-#             doctor = suds.xsd.doctor.ImportDoctor(imp)
-#             client = suds.client.Client('%s?wsdl' % url,
-#                                         transport=t,
-#                                         doctor=doctor)
-#         else:
-#             client = suds.client.Client('%s?wsdl' % url, transport=t)
-#         typed_inputs = []
-#         for (dtype, val) in inputs:
-#             ti = client.factory.create(dtype)
-#             ti.value = val
-#             typed_inputs.append(ti)
-#         # the WSDL returns the local IP address in the URLs; these need
-#         # to be corrected if XNAT is behind a proxy
-#         client.set_options(location=url)
-#         f = getattr(client.service, operation)
-#         result = f(*typed_inputs)
-#         if self._cookiejar is None:
-#             self._cookiejar = t.cookiejar
-#         return result
-
-
-#     def _close(self):
-#         """close the XNAT session (log out)"""
-#         self._call('CloseServiceSession.jws', 'execute', ())
-#         return
-
-#     def _update_xnat(self):
-#         """update XNAT with the current state of this (WorkflowInfo) object"""
-#         inputs = (('ns0:string', self._session),
-#                   ('ns0:string', self._doc.toxml()),
-#                   ('ns0:boolean', False),
-#                   ('ns0:boolean', True))
-#         self._call('StoreXML.jws',
-#                    'store',
-#                    inputs,
-#                    authenticated=True,
-#                    fix_import=True)
-#         return
-
-#     def _append_node(self, root, name, value):
-#         """add a simple text node with tag "name" and data "value" under
-#         the node "root"
-#         """
-#         node = self._doc.createElement(name)
-#         node.appendChild(self._doc.createTextNode(value))
-#         root.appendChild(node)
-#         return
-
-#     def set_environment(self, arguments, parameters):
-#         """set the execution environment
-
-#         should be run only once before update() is called
-#         """
-#         # order is important
-#         workflow_node = self._doc.getElementsByTagName('wrk:Workflow')[0]
-#         ee_node = self._doc.createElement('wrk:executionEnvironment')
-#         ee_node.setAttribute('xsi:type', 'wrk:xnatExecutionEnvironment')
-#         workflow_node.appendChild(ee_node)
-#         self._append_node(ee_node, 'wrk:pipeline', arguments['pipeline'])
-#         self._append_node(ee_node, 'wrk:xnatuser', arguments['u'])
-#         self._append_node(ee_node, 'wrk:host', arguments['host'])
-#         params_node = self._doc.createElement('wrk:parameters')
-#         ee_node.appendChild(params_node)
-#         for key in parameters:
-#             param_node = self._doc.createElement('wrk:parameter')
-#             param_node.setAttribute('name', key)
-#             for val in parameters[key]:
-#                 param_node.appendChild(self._doc.createTextNode(val))
-#             params_node.appendChild(param_node)
-#         for email in arguments['notify_emails']:
-#             self._append_node(ee_node, 'wrk:notify', email)
-#         self._append_node(ee_node, 'wrk:dataType', arguments['dataType'])
-#         self._append_node(ee_node, 'wrk:id', arguments['id'])
-#         if arguments['notify_flag']:
-#             self._append_node(ee_node, 'wrk:supressNotification', '0')
-#         else:
-#             self._append_node(ee_node, 'wrk:supressNotification', '1')
-#         return
-
-#     def update(self, step_id, step_description, percent_complete):
-#         """update the workflow in XNAT"""
-#         workflow_node = self._doc.getElementsByTagName('wrk:Workflow')[0]
-#         workflow_node.setAttribute('status', 'Running')
-#         t = datetime.datetime.now().strftime('%Y-%m-%dT%H:%M:%S')
-#         workflow_node.setAttribute('current_step_launch_time', t)
-#         workflow_node.setAttribute('current_step_id', step_id)
-#         workflow_node.setAttribute('step_description', step_description)
-#         workflow_node.setAttribute('percentageComplete', percent_complete)
-#         self._update_xnat()
-#         return
-
-#     def complete(self):
-#         """mark the workflow comleted in XNAT and close the session"""
-#         workflow_node = self._doc.getElementsByTagName('wrk:Workflow')[0]
-#         workflow_node.setAttribute('status', 'Complete')
-#         t = datetime.datetime.now().strftime('%Y-%m-%dT%H:%M:%S')
-#         workflow_node.setAttribute('current_step_launch_time', t)
-#         workflow_node.setAttribute('percentageComplete', '100.0')
-#         try:
-#             workflow_node.removeAttribute('current_step_id')
-#         except xml.dom.NotFoundErr:
-#             pass
-#         try:
-#             workflow_node.removeAttribute('step_description')
-#         except xml.dom.NotFoundErr:
-#             pass
-#         self._update_xnat()
-#         self._close()
-#         return
-
-#     def fail(self, description=None):
-#         """mark the workflow failed in XNAT and close the session"""
-#         workflow_node = self._doc.getElementsByTagName('wrk:Workflow')[0]
-#         workflow_node.setAttribute('status', 'Failed')
-#         if description is not None:
-#             workflow_node.setAttribute('step_description', description)
-#         self._update_xnat()
-#         self._close()
-#         return
+import os.path as op
+
+# import six
+# if six.PY2:
+#     from urllib2 import urlopen
+# elif six.PY3:
+#     from urllib.request import urlopen
+
+# import smtplib
+# from copy import deepcopy
+# import email.mime.text
+# import xml.dom.minidom
+
+# import suds.client
+# import suds.xsd.doctor
+
+# from . import httputil
+
+
+class PipelineNotFoundError(Exception):
+    """workflow not found"""
+
+
+class Pipelines(object):
+
+    def __init__(self, project, interface):
+        self._intf = interface
+        self._project = project
+
+    def aliases(self):
+        """
+        Fetch the alias ID (stepId) of each available pipeline.
+        :return: Dictionary including pipeline IDs and aliases of all
+        available pipelines as keys and values respectively.
+        """
+        import xml.etree.ElementTree as eTree
+
+        namespace = {'archive': 'http://nrg.wustl.edu/arc'}
+
+        uri = '{}/archive_spec'.format(self._project.attrs.get('URI'))
+        data = self._intf.get(uri).content
+
+        # traverse XML sub-elements named 'pipeline' and get stepId attribute,
+        # Pipeline Engine uses stepID as actual ID for scheduling the pipeline
+        proj_specs = eTree.fromstring(data)
+        pipes_info = proj_specs.findall('archive:pipelines/archive:descendants/archive:'
+                                        'descendant/archive:pipeline', namespace)
+        aliases = {item.find('archive:name', namespace).text: item.attrib['stepId']
+                   for item in pipes_info}
+
+        return aliases
+
+    def info(self, pipeline_id=None):
+        """ Get information about the available pipelines.
+        """
+        response = self._intf.get('{}/pipelines'.format(self._project.attrs.get('URI')))
+        result = response.json()['ResultSet']['Result']
+        if pipeline_id:
+            result = [item for item in result if item['Name'] == pipeline_id]
+        return result
+
+    def pipeline(self, pipeline_id):
+        """ Return a pipeline object.
+        """
+        return Pipeline(pipeline_id, self._project, self._intf)
+
+    def add(self, location):
+        raise NotImplementedError
+        # f = open(location, 'rb')
+        # pip_doc = f.read()
+        # f.close()
+        #
+        # body, content_type = httputil.file_message(
+        #     pip_doc, 'text/xml', location, op.split(location)[1])
+        #
+        # pipeline_uri = '%s/projects/%s/pipelines/%s' % (
+        #     self._intf._get_entry_point(),
+        #     self._project,
+        #     op.split(location)[1]
+        #     )
+        #
+        # self._intf._exec(pipeline_uri,
+        #                  method='PUT',
+        #                  body=body,
+        #                  headers={'content-type': content_type}
+        #                  )
+
+    def delete(self, pipeline_id):
+        raise NotImplementedError
+
+
+class Pipeline(object):
+
+    def __init__(self, pipeline_id, project, interface):
+        self._intf = interface
+        self._project = project
+        self.id = pipeline_id
+        self.uri = '{}/pipelines/{}'.format(self._project.attrs.get('URI'), self.id)
+        # self.datatype = self._datatype()
+        # self.alias = self._alias()
+
+    def _alias(self):
+        """Fetch the alias ID of the pipeline (stepId) asserting its uniqueness.
+        """
+        proj_pipes = Pipelines(self._project, self._intf)
+        proj_aliases = proj_pipes.aliases()
+
+        alias = proj_aliases[self.id]
+        if list(proj_aliases.values()).count(alias) > 1:
+            raise ValueError('Pipeline {} alias ({}) is not unique in project {}.'
+                             .format(self.id, alias, self._project.id()))
+        return alias
+
+    def _datatype(self):
+        """Fetch the experiment datatype the pipeline applies to. If the
+        pipeline does not cope with an specific datatype, function returns
+        'All Datatypes'.
+        """
+        proj_pipes = Pipelines(self._project, self._intf)
+        info = proj_pipes.info(self.id).pop()
+
+        return info['Datatype']
+
+    def exists(self):
+        """ Test whether a pipeline exists in the given context.
+        """
+        response = self._intf.head(self.uri)
+        return response.ok
+
+    def info(self):
+        """ Get pipeline details.
+        """
+        if not self.exists():
+            raise PipelineNotFoundError('Pipeline {} not found in project {}.'
+                                        .format(self.id, self._project.id()))
+
+        response = self._intf.get(self.uri)
+        return response.json()
+
+    def run(self, experiment_id, params=None):
+        """ Run the pipeline on an experiment.
+        """
+        if not self.exists():
+            raise PipelineNotFoundError('Pipeline {} not found in project {}.'
+                                        .format(self.id, self._project.id()))
+
+        e = self._project.experiment(experiment_id)
+        if not e.exists():
+            raise ValueError('Experiment {} not found in project {}.'
+                             .format(experiment_id, self._project.id()))
+
+        datatype = self._datatype()
+        if datatype != 'All Datatypes' and datatype != e.datatype():
+            raise TypeError('Experiment {} does not match the pipeline\'s '
+                            'expected datatype ({}).'.format(experiment_id,
+                                                             datatype))
+
+        uri = '{}/experiments/{}'.format(self.uri.replace(self.id, self._alias()),
+                                         experiment_id)
+
+        response = self._intf.post(uri, params=params)
+        return response.raise_for_status()
+
+    def status(self, experiment_id):
+        """ Fetch latest pipeline execution status for the given experiment.
+        """
+        if not self.exists():
+            raise PipelineNotFoundError('Pipeline {} not found in project {}.'
+                                        .format(self.id, self._project.id()))
+
+        e = self._project.experiment(experiment_id)
+        if not e.exists():
+            raise ValueError('Experiment {} not found in project {}.'
+                             .format(experiment_id, self._project.id()))
+
+        uri = '/data/services/workflows/{}'.format(self.id)
+        options = {'project': self._project.id(),
+                   'experiment': experiment_id,
+                   'display': 'ALL',
+                   'format': 'json'}
+
+        response = self._intf.get(uri, params=options)
+        data = response.json()['ResultSet']['Result']
+        data = [item for item in data
+                if self.id == op.basename(op.splitext(item['pipeline_name'])[0])]
+
+        if not data:
+            status = None
+        else:
+            from operator import itemgetter
+            status = sorted(data, key=lambda x: int(x['wrk_workflowData_id'])).pop(-1)
+        return status
+
+    def stop(self):
+        pass
+
+    def update(self):
+        pass
+
+    def complete(self):
+        pass
+
+    def fail(self):
+        pass
+
+# class Pipeline(object):
+
+#     """class for mirroring workflow information (XML) in XNAT"""
+
+#     def __init__(self, base_url, username, password, workflow_id):
+#         self._base_url = base_url
+#         self._username = username
+#         self._password = password
+#         self._cookiejar = None
+#         res = self._call('CreateServiceSession.jws',
+#                          'execute',
+#                          (),
+#                          authenticated=True)
+#         self._session = str(res)
+#         args = (('ns1:string', self._session),
+#                 ('ns1:string', 'wrk:workflowData.ID'),
+#                 ('ns1:string', '='),
+#                 ('ns1:string', workflow_id),
+#                 ('ns1:string', 'wrk:workflowData'))
+#         workflow_ids = self._call('GetIdentifiers.jws', 'search', args)
+#         self._doc = None
+#         for w_id in workflow_ids:
+#             url = '%s/app/template/XMLSearch.vm/id/%s/data_type/wrk:workflowData' % (self._base_url, str(w_id))
+#             r = urllib2.Request(url)
+#             self._cookiejar.add_cookie_header(r)
+#             data = urllib2.urlopen(r).read()
+#             doc = xml.dom.minidom.parseString(data)
+#             workflow_node = doc.getElementsByTagName('wrk:Workflow')[0]
+#             status = workflow_node.getAttribute('status').lower()
+#             if status in ('queued', 'awaiting action', 'hold'):
+#                 self._doc = doc
+#                 break
+#         if self._doc is None:
+#             raise PipelineNotFoundError
+#         return
+
+#     def _call(self,
+#               jws,
+#               operation,
+#               inputs,
+#               authenticated=False,
+#               fix_import=False):
+#         """perform a SOAP call"""
+#         url = '%s/axis/%s' % (self._base_url, jws)
+#         if authenticated:
+#             t = suds.transport.http.HttpAuthenticated(username=self._username,
+#                                                       password=self._password)
+#         else:
+#             t = suds.transport.http.HttpTransport()
+#         if self._cookiejar is not None:
+#             t.cookiejar = self._cookiejar
+#         if fix_import:
+#             xsd_url = 'http://schemas.xmlsoap.org/soap/encoding/'
+#             imp = suds.xsd.doctor.Import(xsd_url)
+#             doctor = suds.xsd.doctor.ImportDoctor(imp)
+#             client = suds.client.Client('%s?wsdl' % url,
+#                                         transport=t,
+#                                         doctor=doctor)
+#         else:
+#             client = suds.client.Client('%s?wsdl' % url, transport=t)
+#         typed_inputs = []
+#         for (dtype, val) in inputs:
+#             ti = client.factory.create(dtype)
+#             ti.value = val
+#             typed_inputs.append(ti)
+#         # the WSDL returns the local IP address in the URLs; these need
+#         # to be corrected if XNAT is behind a proxy
+#         client.set_options(location=url)
+#         f = getattr(client.service, operation)
+#         result = f(*typed_inputs)
+#         if self._cookiejar is None:
+#             self._cookiejar = t.cookiejar
+#         return result
+
+
+#     def _close(self):
+#         """close the XNAT session (log out)"""
+#         self._call('CloseServiceSession.jws', 'execute', ())
+#         return
+
+#     def _update_xnat(self):
+#         """update XNAT with the current state of this (WorkflowInfo) object"""
+#         inputs = (('ns0:string', self._session),
+#                   ('ns0:string', self._doc.toxml()),
+#                   ('ns0:boolean', False),
+#                   ('ns0:boolean', True))
+#         self._call('StoreXML.jws',
+#                    'store',
+#                    inputs,
+#                    authenticated=True,
+#                    fix_import=True)
+#         return
+
+#     def _append_node(self, root, name, value):
+#         """add a simple text node with tag "name" and data "value" under
+#         the node "root"
+#         """
+#         node = self._doc.createElement(name)
+#         node.appendChild(self._doc.createTextNode(value))
+#         root.appendChild(node)
+#         return
+
+#     def set_environment(self, arguments, parameters):
+#         """set the execution environment
+
+#         should be run only once before update() is called
+#         """
+#         # order is important
+#         workflow_node = self._doc.getElementsByTagName('wrk:Workflow')[0]
+#         ee_node = self._doc.createElement('wrk:executionEnvironment')
+#         ee_node.setAttribute('xsi:type', 'wrk:xnatExecutionEnvironment')
+#         workflow_node.appendChild(ee_node)
+#         self._append_node(ee_node, 'wrk:pipeline', arguments['pipeline'])
+#         self._append_node(ee_node, 'wrk:xnatuser', arguments['u'])
+#         self._append_node(ee_node, 'wrk:host', arguments['host'])
+#         params_node = self._doc.createElement('wrk:parameters')
+#         ee_node.appendChild(params_node)
+#         for key in parameters:
+#             param_node = self._doc.createElement('wrk:parameter')
+#             param_node.setAttribute('name', key)
+#             for val in parameters[key]:
+#                 param_node.appendChild(self._doc.createTextNode(val))
+#             params_node.appendChild(param_node)
+#         for email in arguments['notify_emails']:
+#             self._append_node(ee_node, 'wrk:notify', email)
+#         self._append_node(ee_node, 'wrk:dataType', arguments['dataType'])
+#         self._append_node(ee_node, 'wrk:id', arguments['id'])
+#         if arguments['notify_flag']:
+#             self._append_node(ee_node, 'wrk:supressNotification', '0')
+#         else:
+#             self._append_node(ee_node, 'wrk:supressNotification', '1')
+#         return
+
+#     def update(self, step_id, step_description, percent_complete):
+#         """update the workflow in XNAT"""
+#         workflow_node = self._doc.getElementsByTagName('wrk:Workflow')[0]
+#         workflow_node.setAttribute('status', 'Running')
+#         t = datetime.datetime.now().strftime('%Y-%m-%dT%H:%M:%S')
+#         workflow_node.setAttribute('current_step_launch_time', t)
+#         workflow_node.setAttribute('current_step_id', step_id)
+#         workflow_node.setAttribute('step_description', step_description)
+#         workflow_node.setAttribute('percentageComplete', percent_complete)
+#         self._update_xnat()
+#         return
+
+#     def complete(self):
+#         """mark the workflow comleted in XNAT and close the session"""
+#         workflow_node = self._doc.getElementsByTagName('wrk:Workflow')[0]
+#         workflow_node.setAttribute('status', 'Complete')
+#         t = datetime.datetime.now().strftime('%Y-%m-%dT%H:%M:%S')
+#         workflow_node.setAttribute('current_step_launch_time', t)
+#         workflow_node.setAttribute('percentageComplete', '100.0')
+#         try:
+#             workflow_node.removeAttribute('current_step_id')
+#         except xml.dom.NotFoundErr:
+#             pass
+#         try:
+#             workflow_node.removeAttribute('step_description')
+#         except xml.dom.NotFoundErr:
+#             pass
+#         self._update_xnat()
+#         self._close()
+#         return
+
+#     def fail(self, description=None):
+#         """mark the workflow failed in XNAT and close the session"""
+#         workflow_node = self._doc.getElementsByTagName('wrk:Workflow')[0]
+#         workflow_node.setAttribute('status', 'Failed')
+#         if description is not None:
+#             workflow_node.setAttribute('step_description', description)
+#         self._update_xnat()
+#         self._close()
+#         return
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/provenance.py` & `bbrc-pyxnat-1.6/pyxnat/core/provenance.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,309 +1,309 @@
-import time
-import platform
-import socket
-
-from lxml import etree
-from lxml.etree import Element, QName
-
-from .uriutil import uri_parent
-from .jsonutil import JsonTable
-from . import httputil
-
-_nsmap = {'xnat': 'http://nrg.wustl.edu/xnat',
-          'prov': 'http://www.nbirn.net/prov',
-          'xsi': 'http://www.w3.org/2001/XMLSchema-instance'}
-
-_required = ['program', 'timestamp', 'user', 'machine', 'platform']
-_optional = ['program_version', 'program_arguments',
-             'cvs',
-             'platform_version',
-             'compiler', 'compiler_version',
-             'library', 'library_version'
-             ]
-
-_all = ['program', 'program_version', 'program_arguments',
-        'timestamp',
-        'cvs',
-        'user',
-        'machine',
-        'platform', 'platform_version',
-        'compiler', 'compiler_version',
-        # 'library', 'library_version'
-        ]
-
-_platform_name, _hostname, \
-    _platform_version, _platform_version2,\
-    _machine, _machine2 = platform.uname()
-_machine = socket.gethostname()
-
-
-def provenance_document(eobj, process_steps, overwrite):
-    root_node = etree.fromstring(eobj.get())
-
-    existing_prov = None
-    for child in root_node.getchildren():
-        if str(child.tag).endswith('provenance'):
-            existing_prov = child
-            break
-
-    if existing_prov is not None and not overwrite:
-        prov_node = existing_prov
-    else:
-        if existing_prov is not None and overwrite:
-            root_node.remove(existing_prov)
-
-        prov_node = Element(QName(_nsmap['xnat'], 'provenance'),
-                            nsmap=_nsmap
-                            )
-        root_node.insert(0, prov_node)
-
-    prov_node.extend(provenance_parameters(process_steps))
-
-    return etree.tostring(root_node.getroottree())
-
-
-def provenance_parameters(process_steps):
-    prov = []
-
-    for step in process_steps:
-
-        if not set(_required).issubset(step.keys()):
-            missing = list(set(_required).difference(step.keys()))
-
-            raise Exception(('Following attributes are '
-                             'required to define provenance: %s' % missing
-                             )
-                            )
-
-        prov.append(process_step_xml(**step))
-
-    return prov
-
-
-def process_step_xml(**kwargs):
-
-    step_node = Element(QName(_nsmap['prov'], 'processStep'), nsmap=_nsmap)
-
-    program_node = Element(QName(_nsmap['prov'], 'program'), nsmap=_nsmap)
-    program_node.text = kwargs['program']
-
-    if 'program_version' in kwargs.keys():
-        program_node.set('version', kwargs['program_version'])
-
-    if 'program_arguments' in kwargs.keys():
-        program_node.set('arguments', kwargs['program_arguments'])
-
-    step_node.append(program_node)
-
-    timestamp_node = Element(QName(_nsmap['prov'], 'timestamp'),
-                             nsmap=_nsmap
-                             )
-    timestamp_node.text = kwargs['timestamp']
-
-    step_node.append(timestamp_node)
-
-    if 'cvs' in kwargs.keys():
-        cvs_node = Element(QName(_nsmap['prov'], 'cvs'), nsmap=_nsmap)
-        cvs_node.text = kwargs['cvs']
-
-        step_node.append(cvs_node)
-
-    user_node = Element(QName(_nsmap['prov'], 'user'), nsmap=_nsmap)
-    user_node.text = kwargs['user']
-
-    step_node.append(user_node)
-
-    machine_node = Element(QName(_nsmap['prov'], 'machine'), nsmap=_nsmap)
-    machine_node.text = kwargs['machine']
-
-    step_node.append(machine_node)
-
-    platform_node = Element(QName(_nsmap['prov'], 'platform'), nsmap=_nsmap)
-    platform_node.text = kwargs['platform']
-
-    if 'platform_version' in kwargs.keys():
-        platform_node.set('version', kwargs['platform_version'])
-
-    step_node.append(platform_node)
-
-    if 'compiler' in kwargs.keys():
-        compiler_node = Element(QName(_nsmap['prov'], 'compiler'),
-                                nsmap=_nsmap
-                                )
-        compiler_node.text = kwargs['compiler']
-
-        if 'compiler_version' in kwargs.keys():
-            compiler_node.set('version', kwargs['compiler_version'])
-
-        step_node.append(compiler_node)
-
-    if 'library' in kwargs.keys():
-        library_node = Element(QName(_nsmap['prov'], 'library'),
-                               nsmap=_nsmap)
-        library_node.text = kwargs['library']
-
-        if 'library_version' in kwargs.keys():
-            library_node.set('version', kwargs['library_version'])
-
-        step_node.append(library_node)
-
-    return step_node
-
-
-class Provenance(object):
-    """ Class to annotate processed data with provenance information.
-        The following parameters are available:
-
-            - program
-            - program_version
-            - program_arguments
-            - timestamp
-            - cvs
-            - user
-            - machine
-            - platform
-            - platform_version
-            - compiler
-            - compiler_version
-
-        Examples
-        --------
-            >>> prov = {'program':'young',
-                        'timestamp':'2011-03-01T12:01:01.897987',
-                        'user':'angus',
-                        'machine':'war',
-                        'platform':'linux',
-                        }
-            >>> element.provenance.set(prov)
-            >>> element.provenance.get()
-            >>> element.delete()
-    """
-
-    def __init__(self, eobject):
-        self._intf = eobject._intf
-        self._eobject = eobject
-
-    def set(self, process_steps, overwrite=False):
-        """ Set provenance information for the data within this element.
-
-            .. note::
-
-                If some required parameters are not provided, theses
-                parameters will be extracted from the current machine
-                and set automatically. Those parameters are:
-                    - machine
-                    - platform
-                    - timestamp
-                    - user
-
-            .. warning::
-                overwrite option doesn't work because of a bug with the
-                allowDataDeletion flag in XNAT
-
-            Parameters
-            ----------
-            process_steps: list or dict
-                dict or list of dicts to define the processing steps
-                of the data. The minimum set of information to give
-                is: program, timestamp, user, machine and platform. More
-                keywords in the class documentation.
-            overwrite: boolean
-                If False the process_steps are added to the existing ones.
-                Else the processing steps overwrite any existing provenance.
-        """
-        if isinstance(process_steps, dict):
-            process_steps = [process_steps]
-
-        for process_step in process_steps:
-            _timestamp = time.strftime('%Y-%m-%dT%H:%M:%S',
-                                       time.localtime()
-                                       )
-
-            if 'machine' not in process_step.keys():
-                process_step['machine'] = _machine
-            if 'platform' not in process_step.keys():
-                process_step['platform'] = _platform_name
-                process_step['platform_version'] = _platform_version
-            if 'timestamp' not in process_step.keys():
-                process_step['timestamp'] = _timestamp
-            if 'user' not in process_step.keys():
-                process_step['user'] = self._intf._user
-
-        doc = provenance_document(self._eobject, process_steps, overwrite)
-        doc = doc.decode('utf-8')
-
-        body, content_type = httputil.file_message(
-            doc, 'text/xml', 'prov.xml', 'prov.xml')
-
-        prov_uri = self._eobject._uri
-
-        if overwrite:
-            prov_uri += '?allowDataDeletion=true'
-
-        self._intf._exec(prov_uri,
-                         method='PUT',
-                         body=body,
-                         headers={'content-type': content_type})
-
-    def get(self):
-        """ Gets all the provenance information for that object.
-
-            Returns
-            -------
-            A list of dicts.
-        """
-        datatype = self._eobject.datatype()
-
-        columns = ['%s/ID' % datatype] + [
-            '%s/provenance/processStep/%s' % (datatype, field)
-            for field in _all
-            ]
-
-        prov_uri = uri_parent(self._eobject._uri)
-        prov_uri += '?columns='
-        prov_uri += ','.join(columns)
-
-        steps = []
-
-        table = JsonTable(self._intf._get_json(prov_uri))
-
-        id_header = 'ID' if table.has_header('ID') \
-            else '%s/id' % datatype.lower()
-
-        for step in table.where(**{id_header: self._eobject.id()}):
-            step_dict = {}
-            for key in step.keys():
-                if 'processstep' in key:
-                    step_dict[key.split('processstep/')[1]] = step[key]
-
-            steps.append(step_dict)
-
-        return steps
-
-    def delete(self):
-        """ Removes the provenance attached to this object.
-
-            .. warning::
-                doesn't work because of a bug with the allowDataDeletion
-                flag in XNAT
-        """
-
-        provenance_node = self._eobject.xpath('//xnat:provenance')
-
-        if provenance_node != []:
-            provenance_node = provenance_node[0]
-
-            parent_node = provenance_node.getparent()
-            parent_node.remove(provenance_node)
-
-            doc = etree.tostring(parent_node.getroottree())
-
-            body, content_type = httputil.file_message(
-                doc, 'text/xml', 'prov.xml', 'prov.xml')
-
-            self._intf._exec(
-                '%s?allowDataDeletion=true' % self._eobject._uri,
-                method='PUT',
-                body=body,
-                headers={'content-type': content_type}
-                )
+import time
+import platform
+import socket
+
+from lxml import etree
+from lxml.etree import Element, QName
+
+from .uriutil import uri_parent
+from .jsonutil import JsonTable
+from . import httputil
+
+_nsmap = {'xnat': 'http://nrg.wustl.edu/xnat',
+          'prov': 'http://www.nbirn.net/prov',
+          'xsi': 'http://www.w3.org/2001/XMLSchema-instance'}
+
+_required = ['program', 'timestamp', 'user', 'machine', 'platform']
+_optional = ['program_version', 'program_arguments',
+             'cvs',
+             'platform_version',
+             'compiler', 'compiler_version',
+             'library', 'library_version'
+             ]
+
+_all = ['program', 'program_version', 'program_arguments',
+        'timestamp',
+        'cvs',
+        'user',
+        'machine',
+        'platform', 'platform_version',
+        'compiler', 'compiler_version',
+        # 'library', 'library_version'
+        ]
+
+_platform_name, _hostname, \
+    _platform_version, _platform_version2,\
+    _machine, _machine2 = platform.uname()
+_machine = socket.gethostname()
+
+
+def provenance_document(eobj, process_steps, overwrite):
+    root_node = etree.fromstring(eobj.get())
+
+    existing_prov = None
+    for child in root_node.getchildren():
+        if str(child.tag).endswith('provenance'):
+            existing_prov = child
+            break
+
+    if existing_prov is not None and not overwrite:
+        prov_node = existing_prov
+    else:
+        if existing_prov is not None and overwrite:
+            root_node.remove(existing_prov)
+
+        prov_node = Element(QName(_nsmap['xnat'], 'provenance'),
+                            nsmap=_nsmap
+                            )
+        root_node.insert(0, prov_node)
+
+    prov_node.extend(provenance_parameters(process_steps))
+
+    return etree.tostring(root_node.getroottree())
+
+
+def provenance_parameters(process_steps):
+    prov = []
+
+    for step in process_steps:
+
+        if not set(_required).issubset(step.keys()):
+            missing = list(set(_required).difference(step.keys()))
+
+            raise Exception(('Following attributes are '
+                             'required to define provenance: %s' % missing
+                             )
+                            )
+
+        prov.append(process_step_xml(**step))
+
+    return prov
+
+
+def process_step_xml(**kwargs):
+
+    step_node = Element(QName(_nsmap['prov'], 'processStep'), nsmap=_nsmap)
+
+    program_node = Element(QName(_nsmap['prov'], 'program'), nsmap=_nsmap)
+    program_node.text = kwargs['program']
+
+    if 'program_version' in kwargs.keys():
+        program_node.set('version', kwargs['program_version'])
+
+    if 'program_arguments' in kwargs.keys():
+        program_node.set('arguments', kwargs['program_arguments'])
+
+    step_node.append(program_node)
+
+    timestamp_node = Element(QName(_nsmap['prov'], 'timestamp'),
+                             nsmap=_nsmap
+                             )
+    timestamp_node.text = kwargs['timestamp']
+
+    step_node.append(timestamp_node)
+
+    if 'cvs' in kwargs.keys():
+        cvs_node = Element(QName(_nsmap['prov'], 'cvs'), nsmap=_nsmap)
+        cvs_node.text = kwargs['cvs']
+
+        step_node.append(cvs_node)
+
+    user_node = Element(QName(_nsmap['prov'], 'user'), nsmap=_nsmap)
+    user_node.text = kwargs['user']
+
+    step_node.append(user_node)
+
+    machine_node = Element(QName(_nsmap['prov'], 'machine'), nsmap=_nsmap)
+    machine_node.text = kwargs['machine']
+
+    step_node.append(machine_node)
+
+    platform_node = Element(QName(_nsmap['prov'], 'platform'), nsmap=_nsmap)
+    platform_node.text = kwargs['platform']
+
+    if 'platform_version' in kwargs.keys():
+        platform_node.set('version', kwargs['platform_version'])
+
+    step_node.append(platform_node)
+
+    if 'compiler' in kwargs.keys():
+        compiler_node = Element(QName(_nsmap['prov'], 'compiler'),
+                                nsmap=_nsmap
+                                )
+        compiler_node.text = kwargs['compiler']
+
+        if 'compiler_version' in kwargs.keys():
+            compiler_node.set('version', kwargs['compiler_version'])
+
+        step_node.append(compiler_node)
+
+    if 'library' in kwargs.keys():
+        library_node = Element(QName(_nsmap['prov'], 'library'),
+                               nsmap=_nsmap)
+        library_node.text = kwargs['library']
+
+        if 'library_version' in kwargs.keys():
+            library_node.set('version', kwargs['library_version'])
+
+        step_node.append(library_node)
+
+    return step_node
+
+
+class Provenance(object):
+    """ Class to annotate processed data with provenance information.
+        The following parameters are available:
+
+            - program
+            - program_version
+            - program_arguments
+            - timestamp
+            - cvs
+            - user
+            - machine
+            - platform
+            - platform_version
+            - compiler
+            - compiler_version
+
+        Examples
+        --------
+            >>> prov = {'program':'young',
+                        'timestamp':'2011-03-01T12:01:01.897987',
+                        'user':'angus',
+                        'machine':'war',
+                        'platform':'linux',
+                        }
+            >>> element.provenance.set(prov)
+            >>> element.provenance.get()
+            >>> element.delete()
+    """
+
+    def __init__(self, eobject):
+        self._intf = eobject._intf
+        self._eobject = eobject
+
+    def set(self, process_steps, overwrite=False):
+        """ Set provenance information for the data within this element.
+
+            .. note::
+
+                If some required parameters are not provided, theses
+                parameters will be extracted from the current machine
+                and set automatically. Those parameters are:
+                    - machine
+                    - platform
+                    - timestamp
+                    - user
+
+            .. warning::
+                overwrite option doesn't work because of a bug with the
+                allowDataDeletion flag in XNAT
+
+            Parameters
+            ----------
+            process_steps: list or dict
+                dict or list of dicts to define the processing steps
+                of the data. The minimum set of information to give
+                is: program, timestamp, user, machine and platform. More
+                keywords in the class documentation.
+            overwrite: boolean
+                If False the process_steps are added to the existing ones.
+                Else the processing steps overwrite any existing provenance.
+        """
+        if isinstance(process_steps, dict):
+            process_steps = [process_steps]
+
+        for process_step in process_steps:
+            _timestamp = time.strftime('%Y-%m-%dT%H:%M:%S',
+                                       time.localtime()
+                                       )
+
+            if 'machine' not in process_step.keys():
+                process_step['machine'] = _machine
+            if 'platform' not in process_step.keys():
+                process_step['platform'] = _platform_name
+                process_step['platform_version'] = _platform_version
+            if 'timestamp' not in process_step.keys():
+                process_step['timestamp'] = _timestamp
+            if 'user' not in process_step.keys():
+                process_step['user'] = self._intf._user
+
+        doc = provenance_document(self._eobject, process_steps, overwrite)
+        doc = doc.decode('utf-8')
+
+        body, content_type = httputil.file_message(
+            doc, 'text/xml', 'prov.xml', 'prov.xml')
+
+        prov_uri = self._eobject._uri
+
+        if overwrite:
+            prov_uri += '?allowDataDeletion=true'
+
+        self._intf._exec(prov_uri,
+                         method='PUT',
+                         body=body,
+                         headers={'content-type': content_type})
+
+    def get(self):
+        """ Gets all the provenance information for that object.
+
+            Returns
+            -------
+            A list of dicts.
+        """
+        datatype = self._eobject.datatype()
+
+        columns = ['%s/ID' % datatype] + [
+            '%s/provenance/processStep/%s' % (datatype, field)
+            for field in _all
+            ]
+
+        prov_uri = uri_parent(self._eobject._uri)
+        prov_uri += '?columns='
+        prov_uri += ','.join(columns)
+
+        steps = []
+
+        table = JsonTable(self._intf._get_json(prov_uri))
+
+        id_header = 'ID' if table.has_header('ID') \
+            else '%s/id' % datatype.lower()
+
+        for step in table.where(**{id_header: self._eobject.id()}):
+            step_dict = {}
+            for key in step.keys():
+                if 'processstep' in key:
+                    step_dict[key.split('processstep/')[1]] = step[key]
+
+            steps.append(step_dict)
+
+        return steps
+
+    def delete(self):
+        """ Removes the provenance attached to this object.
+
+            .. warning::
+                doesn't work because of a bug with the allowDataDeletion
+                flag in XNAT
+        """
+
+        provenance_node = self._eobject.xpath('//xnat:provenance')
+
+        if provenance_node != []:
+            provenance_node = provenance_node[0]
+
+            parent_node = provenance_node.getparent()
+            parent_node.remove(provenance_node)
+
+            doc = etree.tostring(parent_node.getroottree())
+
+            body, content_type = httputil.file_message(
+                doc, 'text/xml', 'prov.xml', 'prov.xml')
+
+            self._intf._exec(
+                '%s?allowDataDeletion=true' % self._eobject._uri,
+                method='PUT',
+                body=body,
+                headers={'content-type': content_type}
+                )
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/resources.py` & `bbrc-pyxnat-1.6/pyxnat/core/resources.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,2523 +1,2523 @@
-import lxml
-import os
-import os.path as op
-import sys
-import re
-import shutil
-import tempfile
-import zipfile
-# import time
-import codecs
-from fnmatch import fnmatch
-from itertools import islice
-from lxml import etree
-from pathlib import Path
-
-
-from .uriutil import join_uri, translate_uri, uri_segment
-from .uriutil import uri_last, uri_nextlast
-from .uriutil import uri_parent, uri_grandparent
-from .uriutil import uri_shape
-from .uriutil import file_path
-from .jsonutil import JsonTable, get_selection
-from .pathutil import find_files, ensure_dir_exists
-from .attributes import EAttrs
-from .search import rpn_contraints, query_from_xml
-from .errors import is_xnat_error, parse_put_error_message
-from .errors import DataError, ProgrammingError, catch_error
-from .provenance import Provenance
-from .pipelines import Pipelines
-from . import schema
-from . import httputil
-from . import downloadutils
-import types
-import six
-from six import string_types, add_metaclass
-if six.PY2:
-    from urllib import quote, unquote  # Python 2.X
-elif six.PY3:
-    from urllib.parse import quote, unquote
-    unicode = str
-
-DEBUG = False
-SHOW_URL = True
-# metaclasses
-
-
-def get_element_from_element(rsc_name):
-
-    def getter(self, ID):
-        Element = globals()[rsc_name.title()]
-
-        return Element(join_uri(self._uri, rsc_name + 's', ID), self._intf)
-
-    return getter
-
-
-def get_element_from_collection(rsc_name):
-
-    def getter(self, ID):
-        Element = globals()[rsc_name.title()]
-        Collection = globals()[rsc_name.title() + 's']
-
-        return Collection([Element(join_uri(eobj._uri, rsc_name + 's', ID),
-                                   self._intf)
-                           for eobj in self],
-                          self._intf)
-    return getter
-
-
-def get_collection_from_element(rsc_name):
-
-    def getter(self, id_filter='*'):
-        Collection = globals()[rsc_name.title()]
-        return Collection(join_uri(self._uri, rsc_name),
-                          self._intf, id_filter
-                          )
-
-    return getter
-
-
-def get_collection_from_collection(rsc_name):
-
-    def getter(self, id_filter='*'):
-        Collection = globals()[rsc_name.title()]
-
-        return Collection(self, self._intf, id_filter,
-                          rsc_name, self._id_header, self._columns)
-
-    return getter
-
-
-class ElementType(type):
-    def __new__(cls, name, bases, dct):
-
-        rsc_name = name.lower() + 's' \
-            if name.lower() in schema.resources_singular \
-            else name.lower()
-
-        for child_rsc in schema.resources_tree[rsc_name]:
-            dct[child_rsc] = get_collection_from_element(child_rsc)
-            dct[child_rsc.rstrip('s')] = \
-                get_element_from_element(child_rsc.rstrip('s'))
-
-        return type.__new__(cls, name, bases, dct)
-
-    def __init__(cls, name, bases, dct):
-        super(ElementType, cls).__init__(name, bases, dct)
-
-
-class CollectionType(type):
-    def __new__(cls, name, bases, dct):
-        rsc_name = name.lower() + 's' \
-            if name.lower() in schema.resources_singular \
-            else name.lower()
-
-        for child_rsc in schema.resources_tree[rsc_name]:
-            dct[child_rsc] = get_collection_from_collection(child_rsc)
-            dct[child_rsc.rstrip('s')] = \
-                get_element_from_collection(child_rsc.rstrip('s'))
-
-        return type.__new__(cls, name, bases, dct)
-
-    def __init__(cls, name, bases, dct):
-        super(CollectionType, cls).__init__(name, bases, dct)
-
-
-class EObject(object):
-    """ Generic Object for an element URI.
-    """
-    def __init__(self, uri, interface):
-        """
-            Parameters
-            ----------
-            uri: string
-                URI for an element resource.
-                e.g. /REST/projects/my_project
-
-            interface: :class:`Interface`
-                Main interface reference.
-        """
-
-        self._uri = quote(translate_uri(uri))
-        self._urn = unquote(uri_last(self._uri))
-        self._urt = uri_nextlast(self._uri)
-        self._intf = interface
-        self.attrs = EAttrs(self)
-
-    def __getstate__(self):
-        return {'uri': self._uri,
-                'interface': self._intf}
-
-    def __setstate__(self, dict):
-        self.__init__(dict['uri'], dict['interface'])
-
-    def __repr__(self):
-        return '<%s Object> %s' % (self.__class__.__name__,
-                                   unquote(uri_last(self._uri)))
-
-    def _getcell(self, col):
-        """ Gets a single property of the element resource.
-        """
-        return self._getcells([col])
-
-    def _getcells(self, cols):
-        """ Gets multiple properties of the element resource.
-        """
-        p_uri = uri_parent(self._uri)
-        id_head = schema.json[self._urt][0]
-        lbl_head = schema.json[self._urt][1]
-        filters = {}
-
-        columns = set([col for col in cols
-                       if col not in schema.json[self._urt]
-                       or col != 'URI'] + schema.json[self._urt])
-        get_id = p_uri + '?format=json&columns=%s' % ','.join(columns)
-
-        for pattern in self._intf._struct.keys():
-            if fnmatch(uri_segment(
-                    self._uri.split(
-                        self._intf._get_entry_point(), 1)[1], -2), pattern):
-
-                reg_pat = self._intf._struct[pattern]
-                filters.setdefault('xsiType', set()).add(reg_pat)
-
-        if filters:
-            get_id += '&' + \
-                '&'.join('%s=%s' % (item[0], item[1])
-                         if isinstance(item[1], string_types)
-                         else '%s=%s' % (item[0],
-                                         ','.join([val for val in item[1]]))
-                         for item in filters.items())
-
-        for res in self._intf._get_json(get_id):
-            if self._urn in [res.get(id_head), res.get(lbl_head)]:
-                if len(cols) == 1:
-                    return res.get(cols[0])
-                else:
-                    return get_selection(res, cols)[0]
-
-    def exists(self, consistent=False):
-        """ Test whether an element resource exists.
-        """
-        try:
-            return self.id() is not None
-        except Exception as e:
-            if DEBUG:
-                print(e)
-            return False
-
-    def id(self):
-        """ Returns the element resource id.
-        """
-        return self._getcell(schema.json[self._urt][0])
-
-    def label(self):
-        """ Returns the element resource label.
-        """
-        return self._getcell(schema.json[self._urt][1])
-
-    def datatype(self):
-        """ Returns the type defined in the XNAT schema for this element
-        resource.
-
-            +----------------+-----------------------+
-            | EObject        | possible xsi types    |
-            +================+=======================+
-            | Project        | xnat:projectData      |
-            +----------------+-----------------------+
-            | Subject        | xnat:subjectData      |
-            +----------------+-----------------------+
-            | Experiment     | xnat:mrSessionData    |
-            |                | xnat:petSessionData   |
-            +----------------+-----------------------+
-        """
-        return self._getcell('xsiType')
-
-    def create(self, **params):
-        """ Creates the element if it does not exists.
-            Any non-existing ancestor will be created as well.
-
-            .. warning::
-                An element resource both have an ID and a label that
-                can be used to access it. At the moment, XNAT REST API
-                defines the label when creating an element, but not
-                the ID, which is generated. It means that the `name`
-                given to a resource may not appear when listing the
-                resources because the IDs will appear, not the labels.
-
-            .. note::
-               To set up additional variables for the element at its
-               creation it is possible to use shortcuts defined in the
-               XNAT REST documentation or xpath in the schema:
-
-                   - `element.create(ID='theid')`
-                   - `subject.create(**{'xnat:subjectData/ID':'theid'})`
-
-
-            Parameters
-            ----------
-            params: keywords
-
-                - Specify the datatype of the element resource and of
-                  any ancestor that may need to be created. The
-                  keywords correspond to the levels in the REST
-                  hierarchy, see Interface.inspect.architecture()
-
-                - If an element is created with no specified type:
-
-                      - if its name matches a naming convention, this type
-                        will be used
-                      - else a default type is defined in the schema module
-
-                - To give the ID the same value as the label use
-                  use_label=True e.g element.create(use_label=True)
-
-            Examples
-            --------
-
-                >>> interface.select('/project/PROJECT/subject'
-                                     '/SUBJECT/experiment/EXP/scan/SCAN'
-                            ).create(experiments='xnat:mrSessionData',
-                                     scans='xnat:mrScanData'
-                                     )
-
-            See Also
-            --------
-            :func:`EObject.id`
-            :func:`EObject.label`
-            :func:`EObject.datatype`
-        """
-        if 'xml' in params and op.exists(params.get('xml')):
-
-            f = codecs.open(params.get('xml'))
-            doc = f.read()
-            f.close()
-
-            try:
-                doc_tree = etree.fromstring(doc)
-                doc_tree.xpath('//*')[0].set('label', uri_last(self._uri))
-                doc = etree.tostring(doc_tree)
-            except Exception:
-                pass
-
-            body, content_type = httputil.file_message(
-                doc.decode(), 'text/xml', 'data.xml', 'data.xml')
-
-            _uri = self._uri
-            if ('allowDataDeletion' in params and
-                    params.get('allowDataDeletion') is False):
-                _uri += '?allowDataDeletion=false'
-            else:
-                _uri += '?allowDataDeletion=true'
-
-            self._intf._exec(_uri,
-                             method='PUT',
-                             body=body,
-                             headers={'content-type': content_type})
-
-            return self
-
-        datatype = params.get(uri_nextlast(self._uri))
-        struct = self._intf._struct
-
-        if datatype is None:
-            for uri_pattern in struct.keys():
-                if fnmatch(
-                    self._uri.split(
-                        self._intf._get_entry_point(), 1)[1], uri_pattern):
-                    datatype = struct.get(uri_pattern)
-                    break
-            else:
-                datatype = schema.default_datatypes.get(
-                    uri_nextlast(self._uri))
-
-        if datatype is None:
-            create_uri = self._uri
-        else:
-            local_params = \
-                [param for param in params
-                 if param not in schema.resources_types + ['use_label']
-                    and (param.startswith(datatype) or '/' not in param)
-                 ]
-
-            create_uri = '%s?xsiType=%s' % (self._uri, datatype)
-
-            if 'ID' not in local_params \
-                    and '%s/ID' % datatype not in local_params \
-                    and params.get('use_label'):
-
-                create_uri += '&%s/ID=%s' % (datatype, uri_last(self._uri))
-
-            if local_params:
-                create_uri += '&' + '&'.join('%s=%s' % (key,
-                                                        params.get(key)
-                                                        )
-                                             for key in local_params
-                                             )
-
-            # avoid to reuse relative parameters
-            for key in local_params:
-                del params[key]
-
-        parent_element = self._intf.select(uri_grandparent(self._uri))
-
-        if not uri_nextlast(self._uri) == 'projects' \
-                and not parent_element.exists():
-
-            parent_datatype = params.get(uri_nextlast(parent_element._uri))
-            if DEBUG:
-                print('CREATE', parent_element, parent_datatype)
-            parent_element.create(**params)
-
-        if DEBUG:
-            print('PUT', create_uri)
-
-        if 'params' in params and 'event_reason' in params['params']:
-            if DEBUG:
-                print('Found event_reason')
-            output = self._intf._exec(create_uri, 'PUT', **params)
-        else:
-            if DEBUG:
-                print('event_reason not found')
-            output = self._intf._exec(create_uri, 'PUT')
-
-        if is_xnat_error(output):
-            paths = []
-            for datatype_name, element_name \
-                    in parse_put_error_message(output):
-
-                path = self._intf.inspect.schemas.look_for(
-                    element_name, datatype_name)
-
-                paths.extend(path)
-
-                if DEBUG:
-                    print(path, 'is required')
-
-            return paths
-
-        return self
-
-    insert = create
-
-    def delete(self, delete_files=True):
-        """ Deletes an element resource.
-
-            Parameters
-            ----------
-            delete_files: boolean
-                Tells if files attached to the element resources are
-                removed as well from the server filesystem.
-        """
-        delete_uri = self._uri if not delete_files \
-            else self._uri + '?removeFiles=true'
-
-        out = self._intf._exec(delete_uri, 'DELETE')
-
-        if is_xnat_error(out):
-            catch_error(out)
-
-    def get(self):
-        """ Retrieves the XML document corresponding to this element.
-        """
-        return self._intf._exec(self._uri + '?format=xml', 'GET')
-
-    def xpath(self, xpath):
-        root = etree.fromstring(self.get())
-
-        return root.xpath(xpath, namespaces=root.nsmap)
-
-    def namespaces(self):
-        pass
-
-    def parent(self):
-        uri = uri_grandparent(self._uri)
-        klass = uri_nextlast(uri).title().rsplit('s', 1)[0]
-        if klass:
-            Klass = globals()[klass]
-            return Klass(uri, self._intf)
-        else:
-            return None
-
-    def children(self, show_names=True):
-        """ Returns the children levels of this element.
-
-            Parameters
-            ----------
-            show_name: boolean
-                If True returns a list of strings. If False returns a
-                collection object referencing all child objects of
-                this elements.
-
-            Examples
-            --------
-            >>> subject_object.children()
-            ['experiments', 'resources']
-            >>> subject_object.children(False)
-            <Collection Object> 170976556
-        """
-        children = schema.resources_tree.get(uri_nextlast(self._uri))
-
-        if show_names:
-            return children
-
-        return CObject([getattr(self, child)() for child in children],
-                       self._intf
-                       )
-
-    def tag(self, name):
-        """ Tag the element.
-        """
-        tag = self._intf.manage.tags.get(name)
-        if not tag.exists():
-            tag.create()
-
-        tag.reference(self._uri)
-        return tag
-
-    def untag(self, name):
-        """ Remove a tag for the element.
-        """
-        tag = self._intf.manage.tags.get(name)
-        tag.dereference(self._uri)
-        if not tag.references().get():
-            tag.delete()
-
-
-class CObject(object):
-    """ Generic Object for a collection resource.
-
-        A collection resource is a list of element resources. There is
-        however several ways to obtain such a list:
-
-            - a collection URI e.g. /REST/projects
-            - a list of element URIs
-            - a list of collections
-               e.g. /REST/projects/ONE/subjects **AND**
-               /REST/projects/TWO/subjects
-            - a list of element objects
-            - a list a collection objects
-
-        Collections objects built in different ways share the same behavior:
-
-            - they behave as iterators, which enables a lazy access to
-              the data
-            - they always yield EObjects
-            - they can be nested with any other collection
-
-        Examples
-        --------
-        No access to the data:
-            >>> interface.select.projects()
-            <Collection Object> 173667084
-
-        Lazy access to the data:
-            >>> for project in interface.select.projects():
-            >>>     print project
-
-        Nesting:
-            >>> for subject in interface.select.projects().subjects():
-            >>>     print subject
-    """
-    def __init__(self, cbase, interface, pattern='*', nested=None,
-                 id_header='ID', columns=[], filters={}):
-
-        """
-            Parameters
-            ----------
-            cbase: string | list | CObject
-                Object from which the collection is built.
-            interface: :class:`Interface`
-                Main interface reference.
-            pattern: string
-                Only resource element whose ID match the pattern are
-                returned.
-            nested: None | string
-                Parameter used to nest collections.
-            id_header: ID | label
-                Defines whether the element label or ID is returned as the
-                identifier.
-            columns: list
-                Defines additional columns to be returned.
-            filters: dict
-                Defines additional filters for the query, typically options
-                for the query string.
-        """
-
-        self._intf = interface
-        self._cbase = cbase
-        self._id_header = id_header
-        self._pattern = pattern
-        self._columns = columns
-        self._filters = filters
-        self._nested = nested
-
-        if isinstance(cbase, string_types):
-            self._ctype = 'cobjectcuri'
-        elif isinstance(cbase, CObject):
-            self._ctype = 'cobjectcobject'
-        elif isinstance(cbase, list) and cbase:
-            if isinstance(cbase[0], string_types):
-                self._ctype = 'cobjecteuris'
-            if isinstance(cbase[0], EObject):
-                self._ctype = 'cobjecteobjects'
-            if isinstance(cbase[0], CObject):
-                self._ctype = 'cobjectcobjects'
-        elif isinstance(cbase, list) and not cbase:
-            self._ctype = 'cobjectempty'
-        else:
-            raise Exception('Invalid collection accessor type: %s' % cbase)
-
-    def __repr__(self):
-        return '<Collection Object> %s' % id(self)
-
-    def _call(self, columns):
-        try:
-            uri = translate_uri(self._cbase)
-            uri = quote(uri)
-
-            # request_shape = uri_shape(
-            #    '%s/0' % uri.split(self._intf._get_entry_point(), 1)[1])
-
-            # gather = uri.split('/')[-1] in ['experiments', 'assessors',
-            #                                'scans', 'reconstructions']
-
-            # tick = time.gmtime(time.time())[5] % \
-            #    self._intf.inspect._tick == 0 and\
-            #    self._intf.inspect._auto
-
-            columns += ['xsiType']
-
-            query_string = '?format=json&columns=%s' % ','.join(columns)
-
-            if self._filters:
-                query_string += '&' + '&'.join(
-                    '%s=%s' % (item[0], item[1])
-                    if isinstance(item[1], (str, unicode))
-                    else '%s=%s' % (
-                        item[0], ','.join([val for val in item[1]]))
-                    for item in self._filters.items()
-                    )
-
-            if DEBUG:
-                print(uri + query_string)
-            jtable = self._intf._get_json(uri + query_string)
-
-            _type = uri.split('/')[-1]
-            self._learn_from_table(_type, jtable, None)
-
-            return jtable
-        except Exception as e:
-            if DEBUG:
-                raise e
-            return []
-
-    def _learn_from_table(self, _type, jtable, reqcache):
-        request_knowledge = {}
-
-        for element in jtable:
-            xsitype = element.get('xsiType')
-            if xsitype:
-                # Only some of the xnat elements return xsiType like we asked
-                # them to.Projects and Subjects are two known offenders so we
-                #  cannot update our knowledge of them.
-                uri = element.get('URI').split(self._intf._get_entry_point(),
-                                               1)[1]
-                uri = uri.replace(uri.split('/')[-2], _type)
-                shape = uri_shape(uri)
-                request_knowledge[shape] = xsitype
-
-        self._intf._struct.update(request_knowledge)
-
-    def __iter__(self):
-        if self._ctype == 'cobjectcuri':
-            if self._id_header == 'ID':
-                id_header = schema.json[uri_last(self._cbase)][0]
-            elif self._id_header == 'label':
-                id_header = schema.json[uri_last(self._cbase)][1]
-            else:
-                id_header = self._id_header
-
-            for res in self._call([id_header] + self._columns):
-                try:
-                    eid = unquote(res[id_header])
-                    if fnmatch(eid, self._pattern):
-                        klass_name = uri_last(self._cbase
-                                              ).rstrip('s').title()
-                        Klass = globals().get(klass_name, self._intf.__class__)
-                        eobj = Klass(join_uri(self._cbase, eid), self._intf)
-                        if self._nested is None:
-                            self._run_callback(self, eobj)
-                            yield eobj
-                        else:
-                            Klass = globals().get(self._nested.title(),
-                                                  self._intf.__class__)
-                            for subeobj in Klass(
-                                    cbase=join_uri(eobj._uri, self._nested),
-                                    interface=self._intf,
-                                    pattern=self._pattern,
-                                    id_header=self._id_header,
-                                    columns=self._columns):
-
-                                try:
-                                    self._run_callback(self, subeobj)
-                                    yield subeobj
-                                except RuntimeError:
-                                    pass
-
-                except KeyboardInterrupt:
-                    self._intf._connect()
-                    raise StopIteration
-
-        elif self._ctype == 'cobjecteuris':
-            for uri in self._cbase:
-                try:
-                    title = uri_nextlast(uri).rstrip('s').title()
-                    Klass = globals().get(title, self._intf.__class__)
-                    eobj = Klass(uri, self._intf)
-                    if self._nested is None:
-                        self._run_callback(self, eobj)
-                        yield eobj
-                    else:
-                        Klass = globals().get(self._nested.title(),
-                                              self._intf.__class__)
-                        for subeobj in Klass(
-                                cbase=join_uri(eobj._uri, self._nested),
-                                interface=self._intf,
-                                pattern=self._pattern,
-                                id_header=self._id_header,
-                                columns=self._columns):
-
-                            try:
-                                self._run_callback(self, subeobj)
-                                yield subeobj
-                            except RuntimeError:
-                                pass
-
-                except KeyboardInterrupt:
-                    self._intf._connect()
-                    raise StopIteration
-
-        elif self._ctype == 'cobjecteobjects':
-            for eobj in self._cbase:
-                try:
-                    if self._nested is None:
-                        self._run_callback(self, eobj)
-                        yield eobj
-                    else:
-                        Klass = globals().get(self._nested.rstrip('s').title(),
-                                              self._intf.__class__)
-                        for subeobj in Klass(
-                                cbase=join_uri(eobj._uri, self._nested),
-                                interface=self._intf,
-                                pattern=self._pattern,
-                                id_header=self._id_header,
-                                columns=self._columns):
-
-                            try:
-                                self._run_callback(self, subeobj)
-                                yield subeobj
-                            except RuntimeError:
-                                pass
-
-                except KeyboardInterrupt:
-                    self._intf._connect()
-                    raise StopIteration
-
-        elif self._ctype == 'cobjectcobject':
-            for eobj in self._cbase:
-                try:
-                    if self._nested is None:
-                        self._run_callback(self, eobj)
-                        yield eobj
-                    else:
-                        Klass = globals().get(self._nested.title(),
-                                              self._intf.__class__)
-                        for subeobj in Klass(
-                                cbase=join_uri(eobj._uri, self._nested),
-                                interface=self._intf,
-                                pattern=self._pattern,
-                                id_header=self._id_header,
-                                columns=self._columns):
-
-                            try:
-                                self._run_callback(self, eobj)
-                                yield subeobj
-                            except RuntimeError:
-                                pass
-
-                except KeyboardInterrupt:
-                    self._intf._connect()
-                    raise StopIteration
-
-        elif self._ctype == 'cobjectcobjects':
-            for cobj in self._cbase:
-                try:
-                    for eobj in cobj:
-                        if self._nested is None:
-                            self._run_callback(self, eobj)
-                            yield eobj
-                        else:
-                            Klass = globals().get(cobj._nested.title(),
-                                                  self._intf.__class__)
-
-                            for subeobj in Klass(
-                                    cbase=join_uri(eobj._uri, cobj._nested),
-                                    interface=cobj._intf,
-                                    pattern=cobj._pattern,
-                                    id_header=cobj._id_header,
-                                    columns=cobj._columns):
-
-                                try:
-                                    self._run_callback(self, eobj)
-                                    yield subeobj
-                                except RuntimeError:
-                                    pass
-
-                except KeyboardInterrupt:
-                    self._intf._connect()
-                    raise StopIteration
-
-        elif self._ctype == 'cobjectempty':
-            for empty in []:
-                yield empty
-
-    def _run_callback(self, cobj, eobj):
-        if self._intf._callback is not None:
-            self._intf._callback(cobj, eobj)
-
-    def first(self):
-        """ Returns the first element of the collection.
-        """
-        for eobj in self:
-            return eobj
-
-    fetchone = first
-
-    def __getitem__(self, k):
-        """ Use itertools.islice() to support indexed access and slicing.
-        """
-        if isinstance(k, slice):
-            return islice(self, k.start, k.stop, k.step)
-        else:
-            return next(islice(self, k, k+1))
-
-    def get(self, *args):
-        """ Returns every element.
-
-            .. warning::
-                If a collection needs to issue thousands of queries it may
-                be better to access the resources within a `for-loop`.
-
-            Parameters
-            ----------
-            args: strings
-                - Specify the information to return for the elements
-                  within ID, label and Object.
-                - Any combination of ID, label and obj is valid, if
-                  more than one is given, a list of tuple is returned
-                  instead of a list.
-        """
-        if not args:
-            return [unquote(uri_last(eobj._uri)) for eobj in self]
-        else:
-            entries = []
-
-            for eobj in self:
-                entry = ()
-                for arg in args:
-                    if arg == 'id':
-                        self._id_header = 'ID'
-                        entry += (unquote(uri_last(eobj._uri)),)
-                    elif arg == 'label':
-                        self._id_header = 'label'
-                        entry += (unquote(uri_last(eobj._uri)),)
-                    else:
-                        entry += (eobj,)
-
-                entries.append(entry)
-
-            if len(args) != 1:
-                return entries
-            else:
-                return [e[0] for e in entries]
-
-    fetchall = get
-
-    def __nonzero__(self):
-        try:
-            self.__iter__().next()
-        except StopIteration:
-            return False
-        else:
-            return True
-
-    def tag(self, name):
-        """ Tag the collection.
-        """
-        tag = self._intf.manage.tags.get(name)
-        if not tag.exists():
-            tag.create()
-
-        tag.reference_many([eobj._uri for eobj in self])
-        return tag
-
-    def untag(self, name):
-        """ Remove the tag from the collection.
-        """
-        tag = self._intf.manage.tags.get(name)
-        tag.dereference_many([eobj._uri for eobj in self])
-        if not tag.references().get():
-            tag.delete()
-
-    def where(self, constraints=None, template=None, query=None):
-        """ Only the element objects whose subject that are matching the
-            constraints will be returned. It means that it is not possible
-            to use this method on an element that is not linked to a
-            subject, such as a project.
-
-            Examples
-            --------
-            The ``where`` clause should be on the first select:
-                >>> for experiment in interface.select('//experiments'
-                         ).where([('atest/FIELD', '=', 'value'), 'AND']):
-                >>>      print experiment
-
-            Do **NOT** do this:
-                >>> for experiment in interface.select('//experiments'):
-                        for assessor in experiment.assessors(
-                            ).where([('atest/FIELD', '=', 'value'), 'AND']):
-                >>>         print assessor
-
-            Or this:
-                >>> for project in interface.select('//projects'
-                        ).where([('atest/FIELD', '=', 'value'), 'AND']):
-                >>>     print project
-
-            See Also
-            --------
-            :func:`search.Search`
-        """
-
-        if isinstance(constraints, (str, unicode)):
-            constraints = rpn_contraints(constraints)
-        elif isinstance(template, (tuple)):
-            tmp_bundle = self._intf.manage.search.get_template(
-                template[0], True)
-            tmp_bundle = tmp_bundle % template[1]
-            constraints = query_from_xml(tmp_bundle)['constraints']
-        elif isinstance(query, (str, unicode)):
-            tmp_bundle = self._intf.manage.search.get(query, 'xml')
-            constraints = query_from_xml(tmp_bundle)['constraints']
-        elif isinstance(constraints, list):
-            pass
-        else:
-            raise ProgrammingError('One in [contraints, template and '
-                                   'query] parameters must be correctly '
-                                   'set.')
-
-        # _columns = [
-        #     'xnat:subjectData/PROJECT',
-        #     'xnat:subjectData/SUBJECT_ID',
-        #     ] + ['%s/ID' %qtype for qtype in _queried_types]
-
-        # bundle = build_search_document(
-        #     'xnat:imageSessionData', _columns, constraints)
-
-        # content = self._intf._exec(
-        #     "%s/search?format=json" % self._intf._entry,
-        #     'POST', bundle)
-
-        # if content.startswith('<html>'):
-        #     raise Exception(content.split('<h3>')[1].split('</h3>')[0])
-
-        # results = JsonTable(json.loads(content)['ResultSet']['Result'])
-
-        # return results
-
-        results = query_with(
-            interface=self._intf,
-            join_field='xnat:subjectData/SUBJECT_ID',
-            common_field='SUBJECT_ID',
-            return_values=['xnat:subjectData/PROJECT',
-                           'xnat:subjectData/SUBJECT_ID'],
-            _filter=constraints
-            )
-
-        searchpop = ['%s/projects/' % self._intf._get_entry_point() +
-                     '%(project)s/subjects/%(subject_id)s' % res
-                     for res in results
-                     ]
-
-        cobj = self
-        while cobj:
-            first = cobj.first()
-            if not first:
-                break
-
-            if uri_nextlast(first._uri) == 'subjects':
-                break
-
-            else:
-                cobj = getattr(cobj, '_cbase')
-
-        backup_header = cobj._id_header
-
-        if cobj._pattern != '*':
-            cobj._id_header = 'ID'
-            poi = set(searchpop).intersection([eobj._uri for eobj in cobj])
-        else:
-            poi = searchpop
-
-        cobj._cbase = list(poi)
-        cobj._ctype = 'cobjecteuris'
-        cobj._nested = None
-        cobj._id_header = backup_header
-
-        return self
-
-# specialized classes
-
-
-@add_metaclass(ElementType)
-class Project(EObject):
-
-    def __init__(self, uri, interface):
-        """
-            Parameters
-            ----------
-            uri: string
-                The file resource URI
-            interface: Interface Object
-        """
-
-        EObject.__init__(self, uri, interface)
-        self.pipelines = Pipelines(self, self._intf)
-
-    def __repr__(self):
-        interface = self._intf
-
-        # Check if project exists
-        if self.exists():
-            project_id = self.id()
-
-            data = interface.select('xnat:projectData').all().data
-            data = [e for e in data if e['id'] == project_id][0]
-
-            # Collecting project details
-            name = data['name']
-
-            n_subjects = len(list(self.subjects()))
-
-            # Listing experiments
-            exp = []
-            for e in ['mr', 'ct', 'pet', 'ut']:
-                field = 'proj_%s_count' % e
-                if data[field]:
-                    item = '{f} {e} experiment{s}'
-                    final_s = {True: 's', False: ''}[int(data[field]) > 1]
-                    item = item.format(f=data[field],
-                                       e=e.upper(),
-                                       s=final_s)
-                    exp.append(item)
-
-            owners = [e.strip(' ')
-                      for e in data['project_owners'].split(' <br/> ')]
-            # Creating the output string to be returned
-            output = '<{cl} Object> {id} `{label}` ({access}) {n_subjects}'\
-                ' subject{s} {exp} (owner: {owner}) (created on {insert_date}'\
-                ')'
-            output = output.format(cl=self.__class__.__name__,
-                                   id=project_id,
-                                   label=name,
-                                   s={True: 's', False: ''}[n_subjects > 1],
-                                   n_subjects=n_subjects,
-                                   owner='/'.join(owners),
-                                   insert_date=data['insert_date'],
-                                   access=data['project_access'],
-                                   exp=' '.join(exp))
-
-            if SHOW_URL:
-                url = interface._server + self._uri + '?format=html'
-                output += ' ' + url
-
-            return output
-        else:
-            return '<%s Object> %s' % (self.__class__.__name__,
-                                       self._urn)
-
-    def prearchive_code(self):
-        """ Gets project prearchive code.
-        """
-        return int(self._intf._exec(join_uri(self._uri, 'prearchive_code')))
-
-    def set_prearchive_code(self, code):
-        """ Sets project prearchive code.
-
-            Parameters
-            ----------
-            code: 0 to 4
-        """
-        self._intf._exec(join_uri(self._uri, 'prearchive_code', code),
-                         'PUT')
-
-    def quarantine_code(self):
-        """ Gets project quarantine code.
-        """
-        return int(self._intf._exec(join_uri(self._uri, 'quarantine_code')))
-
-    def set_quarantine_code(self, code):
-        """ Sets project quarantine code.
-
-            Parameters
-            ----------
-            code: 0 to 1
-        """
-        self._intf._exec(join_uri(self._uri, 'quarantine_code', code),
-                         'PUT')
-
-    def current_arc(self):
-        """ Gets project current archive folder on the server.
-        """
-        return self._intf._exec(join_uri(self._uri, 'current_arc'))
-
-    def set_subfolder_in_current_arc(self, subfolder):
-        """ Changes project current archive subfolder on the server.
-        """
-        current_arc = self._intf._exec(join_uri(self._uri, 'current_arc'))
-
-        self._intf._exec(join_uri(self._uri, 'current_arc',
-                                  current_arc, subfolder),
-                         'PUT')
-
-    def accessibility(self):
-        """ Gets project accessibility.
-        """
-        return self._intf._exec(join_uri(self._uri, 'accessibility'), 'GET')
-
-    def set_accessibility(self, accessibility='protected'):
-        """ Sets project accessibility.
-
-            .. note::
-                Write access is given or not by the user level for a
-                specific project.
-
-            Parameters
-            ----------
-            accessibility: public | protected | private
-                Sets the project accessibility:
-                    - public: the project is visible and provides read
-                      access for anyone.
-                    - protected: the project is visible by anyone but the
-                      data is accessible for allowed users only.
-                    - private: the project is visible by allowed users only.
-
-        """
-        return self._intf._exec(join_uri(self._uri, 'accessibility',
-                                         accessibility), 'PUT')
-
-    def users(self):
-        """ Gets all registered users for this project.
-        """
-        return JsonTable(self._intf._get_json(join_uri(self._uri, 'users'))
-                         ).get('login', always_list=True)
-
-    def owners(self):
-        """ Gets owners of this project.
-        """
-        return JsonTable(self._intf._get_json(join_uri(self._uri, 'users'))
-                         ).where(displayname='Owners'
-                                 ).get('login', always_list=True)
-
-    def members(self):
-        """ Gets members of this project.
-        """
-        return JsonTable(self._intf._get_json(join_uri(self._uri, 'users'))
-                         ).where(displayname='Members'
-                                 ).get('login', always_list=True)
-
-    def collaborators(self):
-        """ Gets collaborator of this project.
-        """
-        return JsonTable(self._intf._get_json(join_uri(self._uri, 'users'))
-                         ).where(displayname='Collaborators'
-                                 ).get('login', always_list=True)
-
-    def user_role(self, login):
-        """ Gets the user level of the user for this project.
-
-            Parameters
-            ----------
-            login: string
-                A user of the project.
-
-            Returns
-            -------
-            string : owner | member | collaborator
-
-        """
-        j = JsonTable(self._intf._get_json(join_uri(self._uri, 'users')))
-        return ''.join(j.where(login=login)['displayname']).lower().rstrip('s')
-
-    def add_user(self, login, role='member'):
-        """ Adds a user to the project. The user must already exist on
-            the server.
-
-            Parameters
-            ----------
-            login: string
-                Valid username for the XNAT database.
-            role: owner | member | collaborator
-                The user level for this project:
-                    - owner: read and write access, as well as
-                      administrative privileges such as adding and removing
-                      users.
-                    - member: read access and can create new resources but
-                      not remove them.
-                    - collaborator: read access only.
-        """
-        self._intf._exec(join_uri(self._uri, 'users',
-                                  role.lstrip('s').title() + 's',
-                                  login
-                                  ),
-                         'PUT')
-
-    def remove_user(self, login):
-        """ Removes a user from the project.
-
-            Parameters
-            ----------
-            login: string
-                Valid username for the XNAT database.
-        """
-        self._intf._exec(join_uri(self._uri, 'users',
-                                  self.user_role(login).title() + 's',
-                                  login
-                                  ),
-                         'DELETE')
-
-    def datatype(self):
-        return 'xnat:projectData'
-
-    def experiments(self, id_filter='*'):
-        datapath = '%s/projects/%s/experiments'
-        dp = datapath % (self._intf._get_entry_point(), self.id())
-        return Experiments(dp, self._intf, id_filter)
-
-    def experiment(self, ID):
-        datapath = '%s/projects/%s/experiments/%s'
-        dp = datapath % (self._intf._get_entry_point(), self.id(), ID)
-
-        tmp = Experiment(dp, self._intf)
-        if tmp.id() == ID:
-            return tmp
-        else:
-            # if id id not mach given id (which may have been a label
-            # re-select with the ID of the matching experiment.
-            return Experiment(datapath % (
-                self._intf._get_entry_point(), self.id(), tmp.id()),
-                self._intf
-                )
-
-    def last_modified(self):
-        """ Gets the last modified dates for all the project subjects.
-
-            If any element related to a subject changes, experiment,
-            variable, scan, image etc... the date will be changed.
-        """
-        uri = '%s/subjects?columns=last_modified' % self._uri
-
-        return dict(JsonTable(self._intf._get_json(uri),
-                              order_by=['ID', 'last_modified']
-                              ).select(['ID', 'last_modified']
-                                       ).items()
-                    )
-
-    def add_custom_variables(self, custom_variables,
-                             allow_data_deletion=False):
-        """Adds a custom variable to a specified group
-
-        Parameters
-        ----------
-
-        custom_variables: a dictionary
-        allow_data_deletion : a boolean
-
-        Examples
-        --------
-
-        >>> variables = {'Subjects' : {'newgroup' : {'foo' : 'string',
-            'bar': 'int'}}}
-        >>> project.add_custom_variables(variables)
-
-        """
-        tree = lxml.etree.fromstring(self.get())
-
-        update = False
-
-        for protocol, value in custom_variables.items():
-            try:
-                protocol_element = tree.xpath(
-                    "//xnat:studyProtocol[@name='%s']" % protocol,
-                    namespaces=tree.nsmap).pop()
-
-            except IndexError:
-                raise ValueError(
-                    'Protocol %s not in current schema' % protocol
-                    )
-
-            try:
-                definitions_element = protocol_element.xpath(
-                    'xnat:definitions', namespaces=tree.nsmap).pop()
-            except IndexError:
-                update = True
-                definitions_element = lxml.etree.Element(
-                    lxml.etree.QName(tree.nsmap['xnat'], 'definitions'),
-                    nsmap=tree.nsmap
-                    )
-                protocol_element.append(definitions_element)
-
-            for group, fields in value.items():
-                try:
-                    group_element = definitions_element.xpath(
-                        "xnat:definition[@ID='%s']" % group,
-                        namespaces=tree.nsmap).pop()
-
-                    fields_element = group_element.xpath(
-                        "xnat:fields",
-                        namespaces=tree.nsmap).pop()
-
-                except IndexError:
-                    update = True
-
-                    group_element = lxml.etree.Element(
-                        lxml.etree.QName(tree.nsmap['xnat'], 'definition'),
-                        nsmap=tree.nsmap)
-                    group_element.set('ID', group)
-                    group_element.set(
-                        'data-type', protocol_element.get('data-type'))
-                    group_element.set('description', '')
-                    group_element.set('project-specific', '1')
-                    definitions_element.append(group_element)
-                    fields_element = lxml.etree.Element(
-                        lxml.etree.QName(tree.nsmap['xnat'], 'fields'),
-                        nsmap=tree.nsmap)
-                    group_element.append(fields_element)
-
-                for field, datatype in fields.items():
-                    try:
-                        field_element = fields_element.xpath(
-                            "xnat:field[@name='%s']" % field,
-                            namespaces=tree.nsmap).pop()
-                    except IndexError:
-                        field_element = lxml.etree.Element(
-                            lxml.etree.QName(tree.nsmap['xnat'], 'field'),
-                            nsmap=tree.nsmap)
-                        field_element.set('name', field)
-                        field_element.set('datatype', datatype)
-                        field_element.set('type', 'custom')
-                        field_element.set('required', '0')
-                        field_element.set(
-                            'xmlPath',
-                            "xnat:%s/fields/field[name=%s]/field" % (
-                                protocol_element.get(
-                                    'data-type').split(':')[-1], field))
-                        fields_element.append(field_element)
-                        update = True
-        if update:
-            body, content_type = httputil.file_message(
-                lxml.etree.tostring(tree).decode('utf-8'),
-                'text/xml',
-                'cust.xml',
-                'cust.xml')
-
-            uri = self._uri
-            if allow_data_deletion:
-                uri = self._uri + '?allowDataDeletion=true'
-            self._intf._exec(uri, method='PUT', body=str(body),
-                             headers={'content-type': content_type})
-
-    def get_custom_variables(self):
-        """Retrieves custom variables as a dictionary
-
-        It has the format {studyProtocol: { setname : {field: type, ...}}}
-
-        """
-        tree = lxml.etree.fromstring(self.get())
-        nsmap = tree.nsmap
-        custom_variables = {}
-        for studyprotocols in tree.xpath('//xnat:studyProtocol',
-                                         namespaces=nsmap):
-
-            protocol_name = studyprotocols.get('name')
-            custom_variables[protocol_name] = {}
-
-            for definition in studyprotocols.xpath(('xnat:definitions'
-                                                    '/xnat:definition'),
-                                                   namespaces=nsmap):
-
-                definition_id = definition.get('ID')
-                custom_variables[protocol_name][definition_id] = {}
-                for field in definition.xpath('xnat:fields/xnat:field',
-                                              namespaces=nsmap):
-
-                    field_name = field.get('name')
-                    if field.get('type') == 'custom':
-                        custom_variables[protocol_name][definition_id][
-                            field_name] = field.get('datatype')
-
-        return custom_variables
-
-    def aliases(self):
-        """Returns the aliases for this project.
-
-           Returns
-           -------
-           List of aliases
-        """
-
-        uri = '/data/projects'
-        options = {'columns': 'alias', 'format': 'csv'}
-        data = self._intf.get(uri, params=options).text
-        from .jsonutil import csv_to_json
-        data = csv_to_json(data)
-
-        # parse the results
-        return [item['alias'] for item in data
-                if item['alias'] and item['ID'] == self._urn]
-
-    def description(self):
-        """Returns the description for this project.
-
-        Returns
-        -------
-        Description (string) of the project.
-        """
-        return self.attrs.get('description')
-
-
-@add_metaclass(ElementType)
-class Subject(EObject):
-
-    def datatype(self):
-        return 'xnat:subjectData'
-
-    def __repr__(self):
-        interface = self._intf
-
-        # Check if subject exists
-        if self.exists():
-            subject_id = self.id()
-            columns = ['xnat:subjectData/PROJECT',
-                       'xnat:subjectData/SUBJECT_ID',
-                       'xnat:subjectData/INSERT_DATE',
-                       'xnat:subjectData/INSERT_USER',
-                       'xnat:subjectData/GENDER_TEXT',
-                       'xnat:subjectData/HANDEDNESS_TEXT',
-                       'xnat:subjectData/SES',
-                       'xnat:subjectData/ADD_IDS',
-                       'xnat:subjectData/RACE',
-                       'xnat:subjectData/ETHNICITY',
-                       'xnat:subjectData/SUBJECT_LABEL']
-
-            dt = 'xnat:subjectData'
-            data = interface.select(dt, columns=columns).all().data
-            interface._subjectData = data
-            data = [e for e in data if e['subject_id'] == subject_id][0]
-
-            # Collecting subject details
-            project_id = data['project']
-            age = self.attrs.get('age')
-            gender = data['gender_text']
-            handedness = data['handedness_text']
-            label = data['subject_label']
-            n_expes = len(list(self.experiments()))
-
-            ag = ''
-            if [age, gender, handedness] != ['', '', '']:
-                ag = []
-                if age != '':
-                    ag.append('Age: %s' % age)
-                if gender != '':
-                    ag.append('Gender: %s' % gender)
-                if handedness != '':
-                    ag.append('Handedness: %s' % handedness)
-                ag = '(%s)' % ' - '.join(ag)
-
-            # Creating the output string to be returned
-            output = '<{cl} Object> {id} `{label}` (project: {project}) {ag}'\
-                ' {n_expes} experiment{final_s}'
-            output = output.format(cl=self.__class__.__name__,
-                                   label=label,
-                                   id=subject_id,
-                                   project=project_id,
-                                   ag=ag,
-                                   n_expes=n_expes,
-                                   final_s={True: 's', False: ''}[n_expes > 1])
-
-            if SHOW_URL:
-                url = interface._server + self._uri + '?format=html'
-                output += ' ' + url
-
-            return output
-        else:
-            return '<%s Object> %s' % (self.__class__.__name__,
-                                       unquote(uri_last(self._uri))
-                                       )
-
-    def shares(self, id_filter='*'):
-        """ Returns the projects sharing this subject.
-
-            Returns
-            -------
-            Collection object.
-        """
-        return Projects(join_uri(self._uri, 'projects'),
-                        self._intf, id_filter)
-
-    def share(self, project, label=None, primary=False):
-        """ Share the subject with another project.
-
-            Parameters
-            ----------
-                project: string
-                    Target project name.
-                label: string
-                    Subject label as shared resource. By default, the original
-                    subject label is used.
-                primary: boolean
-                    If True, the ownership of the subject will be transferred to
-                    the target project. User must be owner of both projects to
-                    perform this operation.
-        """
-        owner_project = self.attrs.get('project')
-        aliases = self._intf.select.project(owner_project).aliases()
-        if project in [owner_project] + aliases:
-            raise ValueError("Cannot share a subject with its owner project.")
-
-        options = []
-        if label:
-            options.append('label=%s' % label)
-        else:
-            options.append('label=%s' % self.label())
-        if primary:
-            options.append('primary=true')
-
-        options = '?' + '&'.join(options)
-
-        self._intf._exec(join_uri(self._uri, 'projects', project) + options, 'PUT')
-
-    def unshare(self, project):
-        """ Unlink subject from a project it was shared with. Subject cannot be
-            unshared from the project that owns it.
-
-            Parameters
-            ----------
-                project: string
-                    Target project name.
-        """
-        owner_project = self.attrs.get('project')
-        aliases = self._intf.select.project(owner_project).aliases()
-        if project in [owner_project] + aliases:
-            raise ValueError("Cannot unlink a subject from its owner project.")
-
-        self._intf._exec(join_uri(self._uri, 'projects', project), 'DELETE')
-
-
-@add_metaclass(ElementType)
-class Experiment(EObject):
-
-    def __init__(self, cbase, interface):
-        items = cbase.split('/')
-        e = []
-        if 'subjects' not in items \
-                and 'projects' in items and 'experiments' in items:
-            ID = uri_last(cbase)
-            e = interface.array.experiments(experiment_id=ID).data
-
-        if len(e) == 1:
-            subject_id = e[0]['subject_ID']
-            project_id = e[0]['project']
-
-            cbase = '%s/projects/%s/subjects/%s/experiments/%s'
-            cbase = cbase % (interface._get_entry_point(),
-                             project_id,
-                             subject_id,
-                             ID)
-            return super(Experiment, self).__init__(cbase, interface)
-
-        return super(Experiment, self).__init__(cbase, interface)
-
-    def __repr__(self):
-        intf = self._intf
-
-        # Check if experiment exists
-        if self.exists():
-            eid = self.id()
-
-            e = intf.array.experiments(experiment_id=eid).data[0]
-            filter = [('{}/{}'.format(e['xsiType'], 'ID'), '=', eid)]
-            data = intf.select(e['xsiType']).where(filter).data[0]
-
-            # Collecting experiment details
-            project_id = data['project']
-            label = self.label()
-            subject_id = data['subject_id']
-            e = intf.array.experiments(experiment_id=eid,
-                                       columns=['subject_label']).data[0]
-            subject_label = e['subject_label']
-            insert_date = data['insert_date']
-            n_res = len(list(self.resources()))
-
-            n_scans = len(list(self.scans()))
-
-            # Creating the output string
-            output = '<{cl} Object> {id} `{label}` (subject: {subject_id} '\
-                     '`{subject_label}`) (project: {project}) {n_scans} '\
-                     'scan{final_s1} {n_res} resource{final_s2} (created on '\
-                     '{insert_date})'
-
-            fs = {True: 's', False: ''}
-            output = output.format(cl=self.__class__.__name__,
-                                   id=eid,
-                                   label=label,
-                                   subject_id=subject_id,
-                                   subject_label=subject_label,
-                                   project=project_id,
-                                   n_res=n_res,
-                                   insert_date=insert_date,
-                                   n_scans=n_scans,
-                                   final_s1=fs[n_scans > 1],
-                                   final_s2=fs[n_res > 1])
-            if SHOW_URL:
-                url = intf._server + self._uri + '?format=html'
-                output += ' ' + url
-            return output
-        else:
-            return '<%s Object> %s' % (self.__class__.__name__,
-                                       unquote(uri_last(self._uri)))
-
-    def shares(self, id_filter='*'):
-        """ Returns the projects sharing this experiment.
-
-            Returns
-            -------
-            Collection object.
-        """
-        return Projects(join_uri(self._uri, 'projects'),
-                        self._intf, id_filter)
-
-    def share(self, project, label=None, primary=False):
-        """ Share the experiment with another project.
-
-            Parameters
-            ----------
-                project: string
-                    Target project name.
-                label: string
-                    Experiment label as shared resource. By default, the original
-                    experiment label is used.
-                primary: boolean
-                    If True, the ownership of the subject will be transferred to
-                    the target project. User must be owner of both projects to
-                    perform this operation.
-        """
-        owner_project = self.attrs.get('project')
-        aliases = self._intf.select.project(owner_project).aliases()
-        if project in [owner_project] + aliases:
-            raise ValueError("Cannot share an experiment with its owner project.")
-
-        options = []
-        if label:
-            options.append('label=%s' % label)
-        else:
-            options.append('label=%s' % self.label())
-        if primary:
-            options.append('primary=true')
-
-        options = '?' + '&'.join(options)
-
-        self._intf._exec(join_uri(self._uri, 'projects', project) + options, 'PUT')
-
-    def unshare(self, project):
-        """ Unlink experiment from a project it was shared with. Experiment cannot
-            be unshared from the project that owns it.
-
-            Parameters
-            ----------
-                project: string
-                    Target project name.
-        """
-        owner_project = self.attrs.get('project')
-        aliases = self._intf.select.project(owner_project).aliases()
-        if project in [owner_project] + aliases:
-            raise ValueError("Cannot unlink an experiment from its owner project.")
-
-        self._intf._exec(join_uri(self._uri, 'projects', project), 'DELETE')
-
-    def trigger_pipelines(self):
-        """ Triggers the AutoRun pipeline.
-        """
-        self._intf._exec(self._uri + '?triggerPipelines=true', 'PUT')
-
-    def fix_scan_types(self):
-        """ Populate empty scan TYPE attributes based on how similar
-            scans were populated.
-        """
-        self._intf._exec(self._uri + '?fixScanTypes=true', 'PUT')
-
-    def pull_data_from_headers(self):
-        """ Pull DICOM header values into the session.
-        """
-        self._intf._exec(self._uri + '?pullDataFromHeaders=true', 'PUT')
-
-    def trigger(self, pipelines=True, fix_types=True, scan_headers=True):
-        """ Run several triggers in a single call.
-
-            Parameters
-            ----------
-            pipelines: boolean
-                Same as trigger_pipelines.
-            fix_types: boolean
-                Same as fix_scan_types.
-            scan_headers: boolean
-                Same as pull_data_from headers.
-        """
-        if not all([not pipelines, not fix_types, not scan_headers]):
-            options = []
-            if pipelines:
-                options.append('triggerPipelines=true')
-            if fix_types:
-                options.append('fixScanTypes=true')
-            if scan_headers:
-                options.append('pullDataFromHeaders=true')
-
-            options = '?' + '&'.join(options)
-
-            self._intf._exec(self._uri + options, 'PUT', body=[])
-
-
-@add_metaclass(ElementType)
-class Assessor(EObject):
-
-    def __init__(self, uri, interface):
-        EObject.__init__(self, uri, interface)
-
-        self.provenance = Provenance(self)
-
-    def set_param(self, key, value):
-        self.attrs.set('%s/parameters/addParam[name=%s]/addField'
-                       % (self.datatype(), key),
-                       value
-                       )
-
-    def get_param(self, key):
-        return self.xpath(
-            "//xnat:addParam[@name='%s']/child::text()" % key)[-1]
-
-    def get_params(self):
-        return self.xpath("//xnat:addParam/child::text()")[1::2]
-
-    def params(self):
-        return self.xpath('//xnat:addParam/attribute::*')
-
-
-@add_metaclass(ElementType)
-class Reconstruction(EObject):
-
-    def __init__(self, uri, interface):
-        EObject.__init__(self, uri, interface)
-
-        self.provenance = Provenance(self)
-
-    def datatype(self):
-        return (super(Reconstruction, self).datatype()
-                or 'xnat:reconstructedImageData'
-                )
-
-
-@add_metaclass(ElementType)
-class Scan(EObject):
-
-    def __repr__(self):
-        interface = self._intf
-
-        # Check if scan exists
-        if self.exists():
-            scan_id = self.id()
-
-            # Collect scan details
-            attrs = ['ID', 'type', 'frames', 'quality']
-            base_url = uri_parent(self._uri)
-            scans = self._intf._get_json('{}?columns={}'.format(base_url,
-                                                                ','.join(attrs)))
-            scan_info = [r for r in scans if r['ID'] == scan_id][0]
-
-            # Creating the output string
-            output = '<{cl} Object> {id} (`{type}` {n_frames} frames) {quality}'
-            output = output.format(cl=self.__class__.__name__,
-                                   id=scan_id,
-                                   type=scan_info['type'],
-                                   n_frames=scan_info['frames'],
-                                   quality=scan_info['quality'])
-            if SHOW_URL:
-                url = interface._server + self._uri + '?format=html'
-                output += ' ' + url
-            return output
-        else:
-            return '<%s Object> %s' % (self.__class__.__name__,
-                                       unquote(uri_last(self._uri)))
-
-    def set_param(self, key, value):
-        self.attrs.set('%s/parameters/addParam[name=%s]/addField'
-                       % (self.datatype(), key),
-                       value)
-
-    def get_param(self, key):
-        return self.xpath(
-            "//xnat:addParam[@name='%s']/child::text()" % key)[-1]
-
-    def get_params(self):
-        return self.xpath("//xnat:addParam/child::text()")[1::2]
-
-    def params(self):
-        return self.xpath('//xnat:addParam/attribute::*')
-
-
-@add_metaclass(ElementType)
-class Resource(EObject):
-
-    def __init__(self, cbase, interface):
-        from pyxnat.core.errors import DatabaseError
-        super(Resource, self).__init__(cbase, interface)
-
-        mf = interface._mod_functions.get(self._urn, [])
-        if len(mf) == 0:
-            uri = uri_parent(self._uri)
-            try:
-                d = self._intf._get_json(uri)
-                r = [e for e in d if e['xnat_abstractresource_id'] == self._urn]
-                if len(r) == 1:
-                    label = r[0]['label']
-                    mf = interface._mod_functions.get(label, [])
-            except DatabaseError:
-                print('Warning:', self._uri, 'raising DatabaseError')
-
-        for f in mf:
-            setattr(self, f.__name__, types.MethodType(f, self))
-
-        return None
-
-    def __repr__(self):
-
-        def sizeof_fmt(num, suffix='B'):
-            for unit in ['', 'K', 'M', 'G', 'T', 'P', 'E', 'Z']:
-                if abs(num) < 1024.0:
-                    return "%3.2f %s%s" % (num, unit, suffix)
-                num /= 1024.0
-            return "%.2f %s%s" % (num, 'Y', suffix)
-
-        # Check if resource exists
-        if self.exists():
-            resource_id = self.id()
-            base_url = uri_parent(self._uri)
-            resources = self._intf._get_json(base_url)
-            res_info = [r for r in resources
-                        if r['xnat_abstractresource_id'] == resource_id][0]
-            fs = '0.0 B'
-            if res_info['file_size'] != '':
-                fs = sizeof_fmt(float(res_info['file_size']))
-
-            # Creating the output string
-            output = '<{cl} Object> {id} `{label}` ({fc} files {fs})'
-            output = output.format(label=self.label(),
-                                   cl=self.__class__.__name__,
-                                   id=resource_id,
-                                   fc=res_info['file_count'],
-                                   fs=fs)
-            return output
-        else:
-            return '<%s Object> %s' % (self.__class__.__name__,
-                                       unquote(uri_last(self._uri)))
-
-    def get(self, dest_dir, extract=False):
-        """ Downloads all the files within a resource.
-
-            ..warning::
-                Currently XNAT adds parent folders in the zip file that
-                is downloaded to avoid name clashes if several resources
-                are downloaded in the same folder. In order to be able to
-                download the data uploaded previously with the same
-                structure, pyxnat extracts the zip file, removes the extra
-                paths and if necessary re-zips it. Careful, it may take
-                time, and there is the problem of name clashes.
-
-            Parameters
-            ----------
-            dest_dir: string
-                Destination directory for the resource data.
-                if dest_dir is None, then the user's Downloads directory is
-                used as the default download location.
-            extract: boolean
-                If True, the downloaded zip file is extracted.
-                If False, not extracted.
-
-            Returns
-            -------
-            If extract is False, the zip file path.
-            If extract is True, the list of file paths previously in
-            the zip.
-        """
-        zip_location = op.join(dest_dir, uri_last(self._uri) + '.zip')
-
-        with open(zip_location, 'wb') as f:
-            response = self._intf.get(join_uri(self._uri, 'files') +
-                                      '?format=zip', stream=True)
-            try:
-                count = 0
-                for chunk in response.iter_content(chunk_size=1024):
-                    if chunk:  # filter out keep-alive new chunks
-                        f.write(chunk)
-                        count += 1
-                        if count % 10 == 0:
-                            # flush the buffer every once in a while.
-                            f.flush()
-                f.flush()  # and one last flush.
-            except Exception as e:
-                sys.stderr.write(e)
-            finally:
-                response.close()
-
-        if DEBUG:
-            print(zip_location)
-
-        fzip = zipfile.ZipFile(zip_location, 'r')
-        fzip.extractall(path=dest_dir)
-        fzip.close()
-
-        members = []
-        fzip_namelist = [str(Path(item)) for item in fzip.namelist()]
-        for member in fzip_namelist:
-            old_path = op.join(dest_dir, member)
-            if DEBUG:
-                print(member)
-                print(member.split('files', 1))
-            new_path = op.join(
-                dest_dir,
-                uri_last(self._uri),
-                member.split('files', 1)[1].split(os.sep, 1)[1]
-                )
-
-            if not op.exists(op.dirname(new_path)):
-                os.makedirs(op.dirname(new_path))
-
-            shutil.move(old_path, new_path)
-
-            members.append(new_path)
-
-        # TODO: cache.delete(...)
-        for extracted in fzip_namelist:
-            pth = op.join(dest_dir, extracted.split(os.sep, 1)[0])
-
-            if op.isdir(pth):
-                shutil.rmtree(pth)
-
-        os.remove(zip_location)
-
-        if not extract:
-            fzip = zipfile.ZipFile(zip_location, 'w')
-            arcprefix = op.commonprefix(members).rpartition(os.sep)[0]
-            arcroot = '/%s' % op.split(arcprefix.rstrip(os.sep))[1]
-            for member in members:
-                opj = op.join(arcroot, member.split(arcprefix)[1])
-                fzip.write(member, opj)
-            fzip.close()
-            unzippedTree = op.join(dest_dir, uri_last(self._uri))
-            if op.exists(unzippedTree):
-                if op.isdir(unzippedTree):
-                    shutil.rmtree(op.join(dest_dir, uri_last(self._uri)))
-                else:
-                    os.remove(unzippedTree)
-
-        return zip_location if op.exists(zip_location) else members
-
-    def put(self, sources, overwrite=False, extract=True, **datatypes):
-        """ Insert a list of files in a single resource element.
-
-            This method takes all the files an creates a zip with them
-            which will be the element to be uploaded and then extracted on
-            the server.
-            If the files have a common prefix directory, that directory name
-            will be used.  If not, then "files" will be used as the zip name.
-
-            If avaiable, compression will be used on the zip file.
-
-            Parameters
-            ----------
-            sources: List of paths of files to upload.
-
-            overwrite: boolean
-                If True, overwrite the files that already exist under the
-                    given id.
-                If False, do not overwrite (Default)
-
-            extract: boolean
-                If True, the uploaded zip file is extracted. (Default)
-                If False, the file is not extracted.
-
-        """
-        zip_location = tempfile.mkdtemp(suffix='pyxnat')
-
-        # get the largest common directory.
-        arcprefix, _, _ = op.commonprefix(sources).rpartition(op.sep)
-        # get just the name of the largest common directory.
-        zip_name = op.split(arcprefix.rstrip(op.sep))[1]
-        arcroot = '/%s' % zip_name
-
-        if not zip_name:
-            # if no common prefix, then use "files" as the zip file name.
-            # inside, each file will be directly under the zip root.
-            zip_name = "files"
-
-        zip_name = op.join(zip_location, zip_name + ".zip")
-        fzip = None
-        try:
-            # use compression if avaiable.
-            fzip = zipfile.ZipFile(zip_name, 'w', zipfile.ZIP_DEFLATED)
-        except RuntimeError:
-            print("Zip compression not supported for uploading files.")
-            fzip = zipfile.ZipFile(zip_name, 'w')
-
-        for src in sources:
-            fzip.write(src, op.join(arcroot, src.split(arcprefix)[1]))
-
-        fzip.close()
-
-        self.put_zip(zip_name, overwrite=overwrite, extract=extract,
-                     **datatypes)
-        os.remove(zip_name)
-        os.rmdir(zip_location)
-
-    def put_zip(self, zip_location, overwrite=False, extract=True,
-                **datatypes):
-        """ Uploads a zip or tgz file an then extracts it on the server.
-
-            After the compressed file is extracted the individual
-            files are accessible separately, or as a whole using get_zip.
-
-            Parameters
-            ----------
-            zip_location: Path to zip file for upload.
-
-            overwrite: boolean
-                If True, overwrite the files that already exist under the
-                    given id.
-                If False, do not overwrite (Default)
-
-            extract: boolean
-                If True, the uploaded zip file is extracted. (Default)
-                If False, the file is not extracted.
-        """
-        if not self.exists():
-            self.create(**datatypes)
-
-        if extract:
-            do_extract = '?extract=true'
-        else:
-            do_extract = ''
-
-        self.file(op.split(zip_location)[1] + do_extract
-                  ).put(zip_location, overwrite=overwrite, **datatypes)
-
-    def put_dir(self, src_dir, overwrite=False, extract=True, **datatypes):
-        """ Finds recursively all the files in a folder and uploads
-            them using `insert`. Uses put_zip internally.
-
-            Parameters
-            ----------
-            src_dir: Path to directory to upload.
-
-            overwrite: boolean
-                If True, overwrite the files that already exist under the
-                    given id.
-                If False, do not overwrite (Default)
-
-            extract: boolean
-                If True, the uploaded zip file is extracted. (Default)
-                If False, the file is not extracted.
-        """
-        self.put(find_files(src_dir), overwrite=overwrite, extract=extract,
-                 **datatypes)
-
-    batch_insert = put
-    zip_insert = put_zip
-    dir_insert = put_dir
-
-    def datatype(self):
-        return (super(Resource, self).datatype()
-                or 'xnat:abstractResource'
-                )
-
-    def attributes(self):
-        """ Files attributes include:
-                - URI
-                - Name
-                - Size in bytes
-                - path (relative to the parent resource)
-                - tags
-                - format
-                - content
-            Returns
-            -------
-            dict : a dictionary with the resource attributes
-        """
-
-        return self._getcells(['URI', 'Name', 'Size', 'path',
-                               'tags', 'format', 'content'])
-
-
-class In_Resource(Resource):
-
-    def parent(self):
-        uri = uri_grandparent(self._uri)
-        Klass = globals()[uri.split('/')[-3].title().rsplit('s', 1)[0]]
-        return Klass(uri_parent(uri), self._intf)
-
-
-@add_metaclass(ElementType)
-class Out_Resource(Resource):
-
-    def parent(self):
-        uri = uri_grandparent(self._uri)
-        Klass = globals()[uri.split('/')[-3].title().rsplit('s', 1)[0]]
-        return Klass(uri_parent(uri), self._intf)
-
-
-@add_metaclass(ElementType)
-class File(EObject):
-    """ EObject for files stored in XNAT.
-    """
-
-    def __init__(self, uri, interface):
-        """
-            Parameters
-            ----------
-            uri: string
-                The file resource URI
-            interface: Interface Object
-        """
-
-        EObject.__init__(self, uri, interface)
-        self._urn = file_path(uri)
-        self._absuri = None
-
-    def __repr__(self):
-        return '<%s Object> %s' % (self.__class__.__name__,
-                                   self._urn)
-
-    def attributes(self):
-        """ Files attributes include:
-                - URI
-                - Name
-                - Size in bytes
-                - path (relative to the parent resource)
-                - file_tags
-                - file_format
-                - file_content
-
-            Returns
-            -------
-            dict : a dictionary with the file attributes
-        """
-
-        return self._getcells(['URI', 'Name', 'Size', 'path',
-                               'file_tags', 'file_format', 'file_content'])
-
-    def get(self, dest=None):
-        """ Downloads the file.
-
-            Parameters
-            ----------
-            dest: string | None
-
-                - If dest is None, then the user's Downloads directory is used
-                    as the default download location.
-                - Else the file is downloaded at the requested location.
-                    Path should include the file name.
-                    eg: /path/to/file.txt
-
-            Returns
-            -------
-            string : the file location.
-        """
-        if not self._absuri:
-            self._absuri = self._getcell('URI')
-
-        if self._absuri is None:
-            raise DataError('Cannot get file: does not exists')
-
-        if not dest:
-            dest = op.join(op.expanduser("~"), 'Downloads', self.id())
-            if not ensure_dir_exists(op.dirname(dest)):
-                if DEBUG:
-                    print("File.get: failed to create dir")
-                raise DataError('Cannot create dir for file: %s' % (dest))
-
-        if DEBUG:
-            print(("get_file:", dest))
-
-        with open(dest, 'wb') as f:
-            response = self._intf.get(self._uri, stream=True)
-            try:
-                count = 0
-                for chunk in response.iter_content(chunk_size=1024):
-                    if chunk:  # filter out keep-alive new chunks
-                        f.write(chunk)
-                        count += 1
-                        if count % 10 == 0:
-                            # flush the buffer every once in a while.
-                            f.flush()
-                f.flush()  # and one last flush.
-            except Exception as e:
-                sys.stderr.write(e)
-            finally:
-                response.close()
-        return dest
-
-    def get_copy(self, dest=None):
-        """ Downloads the file to the cache directory but creates a copy at
-            the specified location.
-
-            Parameters
-            ----------
-            dest: string | None
-                - file path for the copy
-                - if None a copy is created at a default location based
-                  on the file URI on the server
-
-            Returns
-            -------
-            string : the copy location.
-        """
-
-        return self.get(dest)
-
-    def put(self, src, format='U', content='U', tags='U', overwrite=False,
-            **datatypes):
-        """ Uploads a file to XNAT.
-
-            Parameters
-            ----------
-            src: string
-                Location of the local file to upload or the actual content
-                to upload.
-            format: string
-                Optional parameter to specify the file format.
-                Defaults to 'U'.
-            content: string
-                Optional parameter to specify the file content.
-                Defaults to 'U'.
-            tags: string
-                Optional parameter to specify tags for the file.
-                Defaults to 'U'.
-            overwrite: boolean
-                Optional parameter to specify if the file should be
-                overwritten. Defaults to False.
-        """
-
-        # First make sure parents and grandparents exist.
-
-        # URI is in the form of data/.../something/files/me so
-        # guri = data/.../something
-        guri = uri_grandparent(self._uri)
-
-        if not self._intf.select(guri).exists():
-            self._intf.select(guri).insert(**datatypes)
-
-        resource_id = self._intf.select(guri).id()
-        isFile = False
-
-        # Cleanup the src and make sure it exists.
-        try:
-            if op.exists(src):
-                isFile = True
-                # path = src
-                # name = op.basename(path).split('?')[0]
-            # else:
-                # path = self._uri.split('/')[-1]
-                # name = path
-        except Exception:
-            pass  # FIXME
-            # path = self._uri.split('/')[-1]
-            # name = path
-
-        self._absuri = unquote(
-            re.sub('resources/.*?/',
-                   'resources/%s/' % resource_id, self._uri)
-            )
-
-        query_args = {
-            'format': format,
-            'content': content,
-            'tags': tags,
-            'overwrite': 'true' if overwrite else 'false',
-            'inbody': 'true'
-            }
-
-        if 'params' in datatypes:
-            query_args.update(datatypes['params'])
-            # Pass on params such as event_reason
-
-        if '?' in self._absuri:
-            k, v = self._absuri.split('?')[1].split('=')
-            query_args[k] = v
-            self._absuri = self._absuri.split('?')[0]
-
-        if DEBUG:
-            print(('INSERT FILE', op.exists(src)))
-            print("URI is: " + self._absuri)
-
-        response = None
-        if isFile:
-            # If src was a file, use inbody streaming to send the file
-            with open(src, 'rb') as f:
-                response = self._intf.post(self._absuri, params=query_args,
-                                           data=f)
-        else:
-            # If it wasn't a file we can just dump the src as data directly.
-            response = self._intf.post(self._absuri, params=query_args,
-                                       data=src)
-
-        # default error handling.
-        if (response is not None and not response.ok) or \
-           is_xnat_error(response.content):
-            if DEBUG:
-                print(response.keys())
-                print(response.get("status"))
-            msg = '''pyxnat.file.put failure:
-                        URI: {response.url}
-                        status code: {response.status_code}
-                        headers: {response.headers}
-                        content: {response.content}
-                    '''.format(response=response)
-            catch_error(response.content, msg)
-
-    insert = put
-    create = put
-
-    def delete(self):
-        """ Deletes the file on the server.
-        """
-        if not self._absuri:
-            self._absuri = self._getcell('URI')
-
-        if self._absuri is None:
-            raise DataError('Cannot delete file: does not exists')
-
-        return self._intf._exec(self._absuri, 'DELETE')
-
-    def size(self):
-        """ Gets the file size.
-        """
-        return self._getcell('Size')
-
-    def labels(self):
-        """ Gets the file labels.
-        """
-        return self._getcell('file_tags')
-
-    def format(self):
-        """ Gets the file format.
-        """
-        return self._getcell('file_format')
-
-    def content(self):
-        """ Gets the file content description.
-        """
-        return self._getcell('file_content')
-
-    def last_modified(self):
-        """ Gets the file last-modified date.
-        """
-
-        if not self._absuri:
-            self._absuri = self._getcell('URI')
-
-        if self._absuri is None:
-            raise DataError('Cannot get file: does not exists')
-
-        info = self._intf._get_head(self._absuri)
-        return info['last-modified']
-
-
-@add_metaclass(ElementType)
-class In_File(File):
-    pass
-
-
-@add_metaclass(ElementType)
-class Out_File(File):
-    pass
-
-
-@add_metaclass(CollectionType)
-class Projects(CObject):
-    pass
-
-
-@add_metaclass(CollectionType)
-class Subjects(CObject):
-
-    def sharing(self, projects=[]):
-        return Subjects([eobj for eobj in self
-                         if set(projects).issubset(eobj.shares().get())],
-                        self._intf)
-
-    def share(self, project):
-        for eobj in self:
-            eobj.share(project)
-
-    def unshare(self, project):
-        for eobj in self:
-            eobj.unshare(project)
-
-
-@add_metaclass(CollectionType)
-class Experiments(CObject):
-
-    def sharing(self, projects=[]):
-        return Experiments([eobj for eobj in self
-                            if set(projects).issubset(eobj.shares().get())],
-                           self._intf)
-
-    def share(self, project):
-        for eobj in self:
-            eobj.share(project)
-
-    def unshare(self, project):
-        for eobj in self:
-            eobj.unshare(project)
-
-
-@add_metaclass(CollectionType)
-class Assessors(CObject):
-
-    def download(self, dest_dir, type="ALL",
-                 name=None, extract=False, safe=False, removeZip=False):
-        """
-        A wrapper around :func:`downloadutils.download`
-        """
-        return downloadutils.download(dest_dir, self, type, name,
-                                      extract, safe, removeZip)
-
-
-@add_metaclass(CollectionType)
-class Reconstructions(CObject):
-
-    def download(self, dest_dir, type="ALL",
-                 name=None, extract=False, safe=False, removeZip=False):
-        """
-        A wrapper around :func:`downloadutils.download`
-        """
-        return downloadutils.download(dest_dir, self, type, name,
-                                      extract, safe, removeZip)
-
-
-@add_metaclass(CollectionType)
-class Scans(CObject):
-
-    def download(self, dest_dir, type="ALL",
-                 name=None, extract=False, safe=False, removeZip=False):
-        """
-        A wrapper around :func:`downloadutils.download`
-
-        """
-        return downloadutils.download(dest_dir, self, type, name,
-                                      extract, safe, removeZip)
-
-
-@add_metaclass(CollectionType)
-class Resources(CObject):
-    pass
-
-
-@add_metaclass(CollectionType)
-class In_Resources(Resources):
-    pass
-
-
-@add_metaclass(CollectionType)
-class Out_Resources(Resources):
-    pass
-
-
-@add_metaclass(CollectionType)
-class Files(CObject):
-    pass
-
-
-@add_metaclass(CollectionType)
-class In_Files(Files):
-    pass
-
-
-@add_metaclass(CollectionType)
-class Out_Files(Files):
-    pass
-
-# Utility functions for downloading and extracting zip archives
-
-
-def _datatypes_from_query(query):
-    datatypes = []
-
-    for constraint in query:
-        if isinstance(constraint, list):
-            datatypes.extend(_datatypes_from_query(constraint))
-        elif isinstance(constraint, tuple):
-            datatypes.append(constraint[0].split('/')[0])
-
-    return datatypes
-
-
-def query_with(interface, join_field,
-               common_field, return_values, _filter):
-
-    _stm = (join_field.split('/')[0], return_values)
-    _cls = rewrite_query(interface, join_field,
-                         common_field, _filter)
-
-    return interface.select(*_stm).where(_cls)
-
-
-def rewrite_query(interface, join_field,
-                  common_field, _filter):
-
-    _new_filter = []
-
-    for _f in _filter:
-        if isinstance(_f, list):
-            _new_filter.append(rewrite_query(
-                interface, join_field, common_field, _f))
-
-        elif isinstance(_f, tuple):
-            _datatype = _f[0].split('/')[0]
-            _res = interface.select(
-                _datatype, ['%s/%s' % (_datatype, common_field)]
-                ).where([_f, 'AND'])
-
-            _new_f = [(join_field, '=', '%s' % sid)
-                      for sid in _res['subject_id']
-                      ]
-
-            _new_f.append('OR')
-            _new_filter.append(_new_f)
-
-        elif isinstance(_f, (str, unicode)):
-            _new_filter.append(_f)
-
-        else:
-            raise Exception('Invalid filter')
-
-    return _new_filter
+import lxml
+import os
+import os.path as op
+import sys
+import re
+import shutil
+import tempfile
+import zipfile
+# import time
+import codecs
+from fnmatch import fnmatch
+from itertools import islice
+from lxml import etree
+from pathlib import Path
+
+
+from .uriutil import join_uri, translate_uri, uri_segment
+from .uriutil import uri_last, uri_nextlast
+from .uriutil import uri_parent, uri_grandparent
+from .uriutil import uri_shape
+from .uriutil import file_path
+from .jsonutil import JsonTable, get_selection
+from .pathutil import find_files, ensure_dir_exists
+from .attributes import EAttrs
+from .search import rpn_contraints, query_from_xml
+from .errors import is_xnat_error, parse_put_error_message
+from .errors import DataError, ProgrammingError, catch_error
+from .provenance import Provenance
+from .pipelines import Pipelines
+from . import schema
+from . import httputil
+from . import downloadutils
+import types
+import six
+from six import string_types, add_metaclass
+if six.PY2:
+    from urllib import quote, unquote  # Python 2.X
+elif six.PY3:
+    from urllib.parse import quote, unquote
+    unicode = str
+
+DEBUG = False
+SHOW_URL = True
+# metaclasses
+
+
+def get_element_from_element(rsc_name):
+
+    def getter(self, ID):
+        Element = globals()[rsc_name.title()]
+
+        return Element(join_uri(self._uri, rsc_name + 's', ID), self._intf)
+
+    return getter
+
+
+def get_element_from_collection(rsc_name):
+
+    def getter(self, ID):
+        Element = globals()[rsc_name.title()]
+        Collection = globals()[rsc_name.title() + 's']
+
+        return Collection([Element(join_uri(eobj._uri, rsc_name + 's', ID),
+                                   self._intf)
+                           for eobj in self],
+                          self._intf)
+    return getter
+
+
+def get_collection_from_element(rsc_name):
+
+    def getter(self, id_filter='*'):
+        Collection = globals()[rsc_name.title()]
+        return Collection(join_uri(self._uri, rsc_name),
+                          self._intf, id_filter
+                          )
+
+    return getter
+
+
+def get_collection_from_collection(rsc_name):
+
+    def getter(self, id_filter='*'):
+        Collection = globals()[rsc_name.title()]
+
+        return Collection(self, self._intf, id_filter,
+                          rsc_name, self._id_header, self._columns)
+
+    return getter
+
+
+class ElementType(type):
+    def __new__(cls, name, bases, dct):
+
+        rsc_name = name.lower() + 's' \
+            if name.lower() in schema.resources_singular \
+            else name.lower()
+
+        for child_rsc in schema.resources_tree[rsc_name]:
+            dct[child_rsc] = get_collection_from_element(child_rsc)
+            dct[child_rsc.rstrip('s')] = \
+                get_element_from_element(child_rsc.rstrip('s'))
+
+        return type.__new__(cls, name, bases, dct)
+
+    def __init__(cls, name, bases, dct):
+        super(ElementType, cls).__init__(name, bases, dct)
+
+
+class CollectionType(type):
+    def __new__(cls, name, bases, dct):
+        rsc_name = name.lower() + 's' \
+            if name.lower() in schema.resources_singular \
+            else name.lower()
+
+        for child_rsc in schema.resources_tree[rsc_name]:
+            dct[child_rsc] = get_collection_from_collection(child_rsc)
+            dct[child_rsc.rstrip('s')] = \
+                get_element_from_collection(child_rsc.rstrip('s'))
+
+        return type.__new__(cls, name, bases, dct)
+
+    def __init__(cls, name, bases, dct):
+        super(CollectionType, cls).__init__(name, bases, dct)
+
+
+class EObject(object):
+    """ Generic Object for an element URI.
+    """
+    def __init__(self, uri, interface):
+        """
+            Parameters
+            ----------
+            uri: string
+                URI for an element resource.
+                e.g. /REST/projects/my_project
+
+            interface: :class:`Interface`
+                Main interface reference.
+        """
+
+        self._uri = quote(translate_uri(uri))
+        self._urn = unquote(uri_last(self._uri))
+        self._urt = uri_nextlast(self._uri)
+        self._intf = interface
+        self.attrs = EAttrs(self)
+
+    def __getstate__(self):
+        return {'uri': self._uri,
+                'interface': self._intf}
+
+    def __setstate__(self, dict):
+        self.__init__(dict['uri'], dict['interface'])
+
+    def __repr__(self):
+        return '<%s Object> %s' % (self.__class__.__name__,
+                                   unquote(uri_last(self._uri)))
+
+    def _getcell(self, col):
+        """ Gets a single property of the element resource.
+        """
+        return self._getcells([col])
+
+    def _getcells(self, cols):
+        """ Gets multiple properties of the element resource.
+        """
+        p_uri = uri_parent(self._uri)
+        id_head = schema.json[self._urt][0]
+        lbl_head = schema.json[self._urt][1]
+        filters = {}
+
+        columns = set([col for col in cols
+                       if col not in schema.json[self._urt]
+                       or col != 'URI'] + schema.json[self._urt])
+        get_id = p_uri + '?format=json&columns=%s' % ','.join(columns)
+
+        for pattern in self._intf._struct.keys():
+            if fnmatch(uri_segment(
+                    self._uri.split(
+                        self._intf._get_entry_point(), 1)[1], -2), pattern):
+
+                reg_pat = self._intf._struct[pattern]
+                filters.setdefault('xsiType', set()).add(reg_pat)
+
+        if filters:
+            get_id += '&' + \
+                '&'.join('%s=%s' % (item[0], item[1])
+                         if isinstance(item[1], string_types)
+                         else '%s=%s' % (item[0],
+                                         ','.join([val for val in item[1]]))
+                         for item in filters.items())
+
+        for res in self._intf._get_json(get_id):
+            if self._urn in [res.get(id_head), res.get(lbl_head)]:
+                if len(cols) == 1:
+                    return res.get(cols[0])
+                else:
+                    return get_selection(res, cols)[0]
+
+    def exists(self, consistent=False):
+        """ Test whether an element resource exists.
+        """
+        try:
+            return self.id() is not None
+        except Exception as e:
+            if DEBUG:
+                print(e)
+            return False
+
+    def id(self):
+        """ Returns the element resource id.
+        """
+        return self._getcell(schema.json[self._urt][0])
+
+    def label(self):
+        """ Returns the element resource label.
+        """
+        return self._getcell(schema.json[self._urt][1])
+
+    def datatype(self):
+        """ Returns the type defined in the XNAT schema for this element
+        resource.
+
+            +----------------+-----------------------+
+            | EObject        | possible xsi types    |
+            +================+=======================+
+            | Project        | xnat:projectData      |
+            +----------------+-----------------------+
+            | Subject        | xnat:subjectData      |
+            +----------------+-----------------------+
+            | Experiment     | xnat:mrSessionData    |
+            |                | xnat:petSessionData   |
+            +----------------+-----------------------+
+        """
+        return self._getcell('xsiType')
+
+    def create(self, **params):
+        """ Creates the element if it does not exists.
+            Any non-existing ancestor will be created as well.
+
+            .. warning::
+                An element resource both have an ID and a label that
+                can be used to access it. At the moment, XNAT REST API
+                defines the label when creating an element, but not
+                the ID, which is generated. It means that the `name`
+                given to a resource may not appear when listing the
+                resources because the IDs will appear, not the labels.
+
+            .. note::
+               To set up additional variables for the element at its
+               creation it is possible to use shortcuts defined in the
+               XNAT REST documentation or xpath in the schema:
+
+                   - `element.create(ID='theid')`
+                   - `subject.create(**{'xnat:subjectData/ID':'theid'})`
+
+
+            Parameters
+            ----------
+            params: keywords
+
+                - Specify the datatype of the element resource and of
+                  any ancestor that may need to be created. The
+                  keywords correspond to the levels in the REST
+                  hierarchy, see Interface.inspect.architecture()
+
+                - If an element is created with no specified type:
+
+                      - if its name matches a naming convention, this type
+                        will be used
+                      - else a default type is defined in the schema module
+
+                - To give the ID the same value as the label use
+                  use_label=True e.g element.create(use_label=True)
+
+            Examples
+            --------
+
+                >>> interface.select('/project/PROJECT/subject'
+                                     '/SUBJECT/experiment/EXP/scan/SCAN'
+                            ).create(experiments='xnat:mrSessionData',
+                                     scans='xnat:mrScanData'
+                                     )
+
+            See Also
+            --------
+            :func:`EObject.id`
+            :func:`EObject.label`
+            :func:`EObject.datatype`
+        """
+        if 'xml' in params and op.exists(params.get('xml')):
+
+            f = codecs.open(params.get('xml'))
+            doc = f.read()
+            f.close()
+
+            try:
+                doc_tree = etree.fromstring(doc)
+                doc_tree.xpath('//*')[0].set('label', uri_last(self._uri))
+                doc = etree.tostring(doc_tree)
+            except Exception:
+                pass
+
+            body, content_type = httputil.file_message(
+                doc.decode(), 'text/xml', 'data.xml', 'data.xml')
+
+            _uri = self._uri
+            if ('allowDataDeletion' in params and
+                    params.get('allowDataDeletion') is False):
+                _uri += '?allowDataDeletion=false'
+            else:
+                _uri += '?allowDataDeletion=true'
+
+            self._intf._exec(_uri,
+                             method='PUT',
+                             body=body,
+                             headers={'content-type': content_type})
+
+            return self
+
+        datatype = params.get(uri_nextlast(self._uri))
+        struct = self._intf._struct
+
+        if datatype is None:
+            for uri_pattern in struct.keys():
+                if fnmatch(
+                    self._uri.split(
+                        self._intf._get_entry_point(), 1)[1], uri_pattern):
+                    datatype = struct.get(uri_pattern)
+                    break
+            else:
+                datatype = schema.default_datatypes.get(
+                    uri_nextlast(self._uri))
+
+        if datatype is None:
+            create_uri = self._uri
+        else:
+            local_params = \
+                [param for param in params
+                 if param not in schema.resources_types + ['use_label']
+                    and (param.startswith(datatype) or '/' not in param)
+                 ]
+
+            create_uri = '%s?xsiType=%s' % (self._uri, datatype)
+
+            if 'ID' not in local_params \
+                    and '%s/ID' % datatype not in local_params \
+                    and params.get('use_label'):
+
+                create_uri += '&%s/ID=%s' % (datatype, uri_last(self._uri))
+
+            if local_params:
+                create_uri += '&' + '&'.join('%s=%s' % (key,
+                                                        params.get(key)
+                                                        )
+                                             for key in local_params
+                                             )
+
+            # avoid to reuse relative parameters
+            for key in local_params:
+                del params[key]
+
+        parent_element = self._intf.select(uri_grandparent(self._uri))
+
+        if not uri_nextlast(self._uri) == 'projects' \
+                and not parent_element.exists():
+
+            parent_datatype = params.get(uri_nextlast(parent_element._uri))
+            if DEBUG:
+                print('CREATE', parent_element, parent_datatype)
+            parent_element.create(**params)
+
+        if DEBUG:
+            print('PUT', create_uri)
+
+        if 'params' in params and 'event_reason' in params['params']:
+            if DEBUG:
+                print('Found event_reason')
+            output = self._intf._exec(create_uri, 'PUT', **params)
+        else:
+            if DEBUG:
+                print('event_reason not found')
+            output = self._intf._exec(create_uri, 'PUT')
+
+        if is_xnat_error(output):
+            paths = []
+            for datatype_name, element_name \
+                    in parse_put_error_message(output):
+
+                path = self._intf.inspect.schemas.look_for(
+                    element_name, datatype_name)
+
+                paths.extend(path)
+
+                if DEBUG:
+                    print(path, 'is required')
+
+            return paths
+
+        return self
+
+    insert = create
+
+    def delete(self, delete_files=True):
+        """ Deletes an element resource.
+
+            Parameters
+            ----------
+            delete_files: boolean
+                Tells if files attached to the element resources are
+                removed as well from the server filesystem.
+        """
+        delete_uri = self._uri if not delete_files \
+            else self._uri + '?removeFiles=true'
+
+        out = self._intf._exec(delete_uri, 'DELETE')
+
+        if is_xnat_error(out):
+            catch_error(out)
+
+    def get(self):
+        """ Retrieves the XML document corresponding to this element.
+        """
+        return self._intf._exec(self._uri + '?format=xml', 'GET')
+
+    def xpath(self, xpath):
+        root = etree.fromstring(self.get())
+
+        return root.xpath(xpath, namespaces=root.nsmap)
+
+    def namespaces(self):
+        pass
+
+    def parent(self):
+        uri = uri_grandparent(self._uri)
+        klass = uri_nextlast(uri).title().rsplit('s', 1)[0]
+        if klass:
+            Klass = globals()[klass]
+            return Klass(uri, self._intf)
+        else:
+            return None
+
+    def children(self, show_names=True):
+        """ Returns the children levels of this element.
+
+            Parameters
+            ----------
+            show_name: boolean
+                If True returns a list of strings. If False returns a
+                collection object referencing all child objects of
+                this elements.
+
+            Examples
+            --------
+            >>> subject_object.children()
+            ['experiments', 'resources']
+            >>> subject_object.children(False)
+            <Collection Object> 170976556
+        """
+        children = schema.resources_tree.get(uri_nextlast(self._uri))
+
+        if show_names:
+            return children
+
+        return CObject([getattr(self, child)() for child in children],
+                       self._intf
+                       )
+
+    def tag(self, name):
+        """ Tag the element.
+        """
+        tag = self._intf.manage.tags.get(name)
+        if not tag.exists():
+            tag.create()
+
+        tag.reference(self._uri)
+        return tag
+
+    def untag(self, name):
+        """ Remove a tag for the element.
+        """
+        tag = self._intf.manage.tags.get(name)
+        tag.dereference(self._uri)
+        if not tag.references().get():
+            tag.delete()
+
+
+class CObject(object):
+    """ Generic Object for a collection resource.
+
+        A collection resource is a list of element resources. There is
+        however several ways to obtain such a list:
+
+            - a collection URI e.g. /REST/projects
+            - a list of element URIs
+            - a list of collections
+               e.g. /REST/projects/ONE/subjects **AND**
+               /REST/projects/TWO/subjects
+            - a list of element objects
+            - a list a collection objects
+
+        Collections objects built in different ways share the same behavior:
+
+            - they behave as iterators, which enables a lazy access to
+              the data
+            - they always yield EObjects
+            - they can be nested with any other collection
+
+        Examples
+        --------
+        No access to the data:
+            >>> interface.select.projects()
+            <Collection Object> 173667084
+
+        Lazy access to the data:
+            >>> for project in interface.select.projects():
+            >>>     print project
+
+        Nesting:
+            >>> for subject in interface.select.projects().subjects():
+            >>>     print subject
+    """
+    def __init__(self, cbase, interface, pattern='*', nested=None,
+                 id_header='ID', columns=[], filters={}):
+
+        """
+            Parameters
+            ----------
+            cbase: string | list | CObject
+                Object from which the collection is built.
+            interface: :class:`Interface`
+                Main interface reference.
+            pattern: string
+                Only resource element whose ID match the pattern are
+                returned.
+            nested: None | string
+                Parameter used to nest collections.
+            id_header: ID | label
+                Defines whether the element label or ID is returned as the
+                identifier.
+            columns: list
+                Defines additional columns to be returned.
+            filters: dict
+                Defines additional filters for the query, typically options
+                for the query string.
+        """
+
+        self._intf = interface
+        self._cbase = cbase
+        self._id_header = id_header
+        self._pattern = pattern
+        self._columns = columns
+        self._filters = filters
+        self._nested = nested
+
+        if isinstance(cbase, string_types):
+            self._ctype = 'cobjectcuri'
+        elif isinstance(cbase, CObject):
+            self._ctype = 'cobjectcobject'
+        elif isinstance(cbase, list) and cbase:
+            if isinstance(cbase[0], string_types):
+                self._ctype = 'cobjecteuris'
+            if isinstance(cbase[0], EObject):
+                self._ctype = 'cobjecteobjects'
+            if isinstance(cbase[0], CObject):
+                self._ctype = 'cobjectcobjects'
+        elif isinstance(cbase, list) and not cbase:
+            self._ctype = 'cobjectempty'
+        else:
+            raise Exception('Invalid collection accessor type: %s' % cbase)
+
+    def __repr__(self):
+        return '<Collection Object> %s' % id(self)
+
+    def _call(self, columns):
+        try:
+            uri = translate_uri(self._cbase)
+            uri = quote(uri)
+
+            # request_shape = uri_shape(
+            #    '%s/0' % uri.split(self._intf._get_entry_point(), 1)[1])
+
+            # gather = uri.split('/')[-1] in ['experiments', 'assessors',
+            #                                'scans', 'reconstructions']
+
+            # tick = time.gmtime(time.time())[5] % \
+            #    self._intf.inspect._tick == 0 and\
+            #    self._intf.inspect._auto
+
+            columns += ['xsiType']
+
+            query_string = '?format=json&columns=%s' % ','.join(columns)
+
+            if self._filters:
+                query_string += '&' + '&'.join(
+                    '%s=%s' % (item[0], item[1])
+                    if isinstance(item[1], (str, unicode))
+                    else '%s=%s' % (
+                        item[0], ','.join([val for val in item[1]]))
+                    for item in self._filters.items()
+                    )
+
+            if DEBUG:
+                print(uri + query_string)
+            jtable = self._intf._get_json(uri + query_string)
+
+            _type = uri.split('/')[-1]
+            self._learn_from_table(_type, jtable, None)
+
+            return jtable
+        except Exception as e:
+            if DEBUG:
+                raise e
+            return []
+
+    def _learn_from_table(self, _type, jtable, reqcache):
+        request_knowledge = {}
+
+        for element in jtable:
+            xsitype = element.get('xsiType')
+            if xsitype:
+                # Only some of the xnat elements return xsiType like we asked
+                # them to.Projects and Subjects are two known offenders so we
+                #  cannot update our knowledge of them.
+                uri = element.get('URI').split(self._intf._get_entry_point(),
+                                               1)[1]
+                uri = uri.replace(uri.split('/')[-2], _type)
+                shape = uri_shape(uri)
+                request_knowledge[shape] = xsitype
+
+        self._intf._struct.update(request_knowledge)
+
+    def __iter__(self):
+        if self._ctype == 'cobjectcuri':
+            if self._id_header == 'ID':
+                id_header = schema.json[uri_last(self._cbase)][0]
+            elif self._id_header == 'label':
+                id_header = schema.json[uri_last(self._cbase)][1]
+            else:
+                id_header = self._id_header
+
+            for res in self._call([id_header] + self._columns):
+                try:
+                    eid = unquote(res[id_header])
+                    if fnmatch(eid, self._pattern):
+                        klass_name = uri_last(self._cbase
+                                              ).rstrip('s').title()
+                        Klass = globals().get(klass_name, self._intf.__class__)
+                        eobj = Klass(join_uri(self._cbase, eid), self._intf)
+                        if self._nested is None:
+                            self._run_callback(self, eobj)
+                            yield eobj
+                        else:
+                            Klass = globals().get(self._nested.title(),
+                                                  self._intf.__class__)
+                            for subeobj in Klass(
+                                    cbase=join_uri(eobj._uri, self._nested),
+                                    interface=self._intf,
+                                    pattern=self._pattern,
+                                    id_header=self._id_header,
+                                    columns=self._columns):
+
+                                try:
+                                    self._run_callback(self, subeobj)
+                                    yield subeobj
+                                except RuntimeError:
+                                    pass
+
+                except KeyboardInterrupt:
+                    self._intf._connect()
+                    raise StopIteration
+
+        elif self._ctype == 'cobjecteuris':
+            for uri in self._cbase:
+                try:
+                    title = uri_nextlast(uri).rstrip('s').title()
+                    Klass = globals().get(title, self._intf.__class__)
+                    eobj = Klass(uri, self._intf)
+                    if self._nested is None:
+                        self._run_callback(self, eobj)
+                        yield eobj
+                    else:
+                        Klass = globals().get(self._nested.title(),
+                                              self._intf.__class__)
+                        for subeobj in Klass(
+                                cbase=join_uri(eobj._uri, self._nested),
+                                interface=self._intf,
+                                pattern=self._pattern,
+                                id_header=self._id_header,
+                                columns=self._columns):
+
+                            try:
+                                self._run_callback(self, subeobj)
+                                yield subeobj
+                            except RuntimeError:
+                                pass
+
+                except KeyboardInterrupt:
+                    self._intf._connect()
+                    raise StopIteration
+
+        elif self._ctype == 'cobjecteobjects':
+            for eobj in self._cbase:
+                try:
+                    if self._nested is None:
+                        self._run_callback(self, eobj)
+                        yield eobj
+                    else:
+                        Klass = globals().get(self._nested.rstrip('s').title(),
+                                              self._intf.__class__)
+                        for subeobj in Klass(
+                                cbase=join_uri(eobj._uri, self._nested),
+                                interface=self._intf,
+                                pattern=self._pattern,
+                                id_header=self._id_header,
+                                columns=self._columns):
+
+                            try:
+                                self._run_callback(self, subeobj)
+                                yield subeobj
+                            except RuntimeError:
+                                pass
+
+                except KeyboardInterrupt:
+                    self._intf._connect()
+                    raise StopIteration
+
+        elif self._ctype == 'cobjectcobject':
+            for eobj in self._cbase:
+                try:
+                    if self._nested is None:
+                        self._run_callback(self, eobj)
+                        yield eobj
+                    else:
+                        Klass = globals().get(self._nested.title(),
+                                              self._intf.__class__)
+                        for subeobj in Klass(
+                                cbase=join_uri(eobj._uri, self._nested),
+                                interface=self._intf,
+                                pattern=self._pattern,
+                                id_header=self._id_header,
+                                columns=self._columns):
+
+                            try:
+                                self._run_callback(self, eobj)
+                                yield subeobj
+                            except RuntimeError:
+                                pass
+
+                except KeyboardInterrupt:
+                    self._intf._connect()
+                    raise StopIteration
+
+        elif self._ctype == 'cobjectcobjects':
+            for cobj in self._cbase:
+                try:
+                    for eobj in cobj:
+                        if self._nested is None:
+                            self._run_callback(self, eobj)
+                            yield eobj
+                        else:
+                            Klass = globals().get(cobj._nested.title(),
+                                                  self._intf.__class__)
+
+                            for subeobj in Klass(
+                                    cbase=join_uri(eobj._uri, cobj._nested),
+                                    interface=cobj._intf,
+                                    pattern=cobj._pattern,
+                                    id_header=cobj._id_header,
+                                    columns=cobj._columns):
+
+                                try:
+                                    self._run_callback(self, eobj)
+                                    yield subeobj
+                                except RuntimeError:
+                                    pass
+
+                except KeyboardInterrupt:
+                    self._intf._connect()
+                    raise StopIteration
+
+        elif self._ctype == 'cobjectempty':
+            for empty in []:
+                yield empty
+
+    def _run_callback(self, cobj, eobj):
+        if self._intf._callback is not None:
+            self._intf._callback(cobj, eobj)
+
+    def first(self):
+        """ Returns the first element of the collection.
+        """
+        for eobj in self:
+            return eobj
+
+    fetchone = first
+
+    def __getitem__(self, k):
+        """ Use itertools.islice() to support indexed access and slicing.
+        """
+        if isinstance(k, slice):
+            return islice(self, k.start, k.stop, k.step)
+        else:
+            return next(islice(self, k, k+1))
+
+    def get(self, *args):
+        """ Returns every element.
+
+            .. warning::
+                If a collection needs to issue thousands of queries it may
+                be better to access the resources within a `for-loop`.
+
+            Parameters
+            ----------
+            args: strings
+                - Specify the information to return for the elements
+                  within ID, label and Object.
+                - Any combination of ID, label and obj is valid, if
+                  more than one is given, a list of tuple is returned
+                  instead of a list.
+        """
+        if not args:
+            return [unquote(uri_last(eobj._uri)) for eobj in self]
+        else:
+            entries = []
+
+            for eobj in self:
+                entry = ()
+                for arg in args:
+                    if arg == 'id':
+                        self._id_header = 'ID'
+                        entry += (unquote(uri_last(eobj._uri)),)
+                    elif arg == 'label':
+                        self._id_header = 'label'
+                        entry += (unquote(uri_last(eobj._uri)),)
+                    else:
+                        entry += (eobj,)
+
+                entries.append(entry)
+
+            if len(args) != 1:
+                return entries
+            else:
+                return [e[0] for e in entries]
+
+    fetchall = get
+
+    def __nonzero__(self):
+        try:
+            self.__iter__().next()
+        except StopIteration:
+            return False
+        else:
+            return True
+
+    def tag(self, name):
+        """ Tag the collection.
+        """
+        tag = self._intf.manage.tags.get(name)
+        if not tag.exists():
+            tag.create()
+
+        tag.reference_many([eobj._uri for eobj in self])
+        return tag
+
+    def untag(self, name):
+        """ Remove the tag from the collection.
+        """
+        tag = self._intf.manage.tags.get(name)
+        tag.dereference_many([eobj._uri for eobj in self])
+        if not tag.references().get():
+            tag.delete()
+
+    def where(self, constraints=None, template=None, query=None):
+        """ Only the element objects whose subject that are matching the
+            constraints will be returned. It means that it is not possible
+            to use this method on an element that is not linked to a
+            subject, such as a project.
+
+            Examples
+            --------
+            The ``where`` clause should be on the first select:
+                >>> for experiment in interface.select('//experiments'
+                         ).where([('atest/FIELD', '=', 'value'), 'AND']):
+                >>>      print experiment
+
+            Do **NOT** do this:
+                >>> for experiment in interface.select('//experiments'):
+                        for assessor in experiment.assessors(
+                            ).where([('atest/FIELD', '=', 'value'), 'AND']):
+                >>>         print assessor
+
+            Or this:
+                >>> for project in interface.select('//projects'
+                        ).where([('atest/FIELD', '=', 'value'), 'AND']):
+                >>>     print project
+
+            See Also
+            --------
+            :func:`search.Search`
+        """
+
+        if isinstance(constraints, (str, unicode)):
+            constraints = rpn_contraints(constraints)
+        elif isinstance(template, (tuple)):
+            tmp_bundle = self._intf.manage.search.get_template(
+                template[0], True)
+            tmp_bundle = tmp_bundle % template[1]
+            constraints = query_from_xml(tmp_bundle)['constraints']
+        elif isinstance(query, (str, unicode)):
+            tmp_bundle = self._intf.manage.search.get(query, 'xml')
+            constraints = query_from_xml(tmp_bundle)['constraints']
+        elif isinstance(constraints, list):
+            pass
+        else:
+            raise ProgrammingError('One in [contraints, template and '
+                                   'query] parameters must be correctly '
+                                   'set.')
+
+        # _columns = [
+        #     'xnat:subjectData/PROJECT',
+        #     'xnat:subjectData/SUBJECT_ID',
+        #     ] + ['%s/ID' %qtype for qtype in _queried_types]
+
+        # bundle = build_search_document(
+        #     'xnat:imageSessionData', _columns, constraints)
+
+        # content = self._intf._exec(
+        #     "%s/search?format=json" % self._intf._entry,
+        #     'POST', bundle)
+
+        # if content.startswith('<html>'):
+        #     raise Exception(content.split('<h3>')[1].split('</h3>')[0])
+
+        # results = JsonTable(json.loads(content)['ResultSet']['Result'])
+
+        # return results
+
+        results = query_with(
+            interface=self._intf,
+            join_field='xnat:subjectData/SUBJECT_ID',
+            common_field='SUBJECT_ID',
+            return_values=['xnat:subjectData/PROJECT',
+                           'xnat:subjectData/SUBJECT_ID'],
+            _filter=constraints
+            )
+
+        searchpop = ['%s/projects/' % self._intf._get_entry_point() +
+                     '%(project)s/subjects/%(subject_id)s' % res
+                     for res in results
+                     ]
+
+        cobj = self
+        while cobj:
+            first = cobj.first()
+            if not first:
+                break
+
+            if uri_nextlast(first._uri) == 'subjects':
+                break
+
+            else:
+                cobj = getattr(cobj, '_cbase')
+
+        backup_header = cobj._id_header
+
+        if cobj._pattern != '*':
+            cobj._id_header = 'ID'
+            poi = set(searchpop).intersection([eobj._uri for eobj in cobj])
+        else:
+            poi = searchpop
+
+        cobj._cbase = list(poi)
+        cobj._ctype = 'cobjecteuris'
+        cobj._nested = None
+        cobj._id_header = backup_header
+
+        return self
+
+# specialized classes
+
+
+@add_metaclass(ElementType)
+class Project(EObject):
+
+    def __init__(self, uri, interface):
+        """
+            Parameters
+            ----------
+            uri: string
+                The file resource URI
+            interface: Interface Object
+        """
+
+        EObject.__init__(self, uri, interface)
+        self.pipelines = Pipelines(self, self._intf)
+
+    def __repr__(self):
+        interface = self._intf
+
+        # Check if project exists
+        if self.exists():
+            project_id = self.id()
+
+            data = interface.select('xnat:projectData').all().data
+            data = [e for e in data if e['id'] == project_id][0]
+
+            # Collecting project details
+            name = data['name']
+
+            n_subjects = len(list(self.subjects()))
+
+            # Listing experiments
+            exp = []
+            for e in ['mr', 'ct', 'pet', 'ut']:
+                field = 'proj_%s_count' % e
+                if data[field]:
+                    item = '{f} {e} experiment{s}'
+                    final_s = {True: 's', False: ''}[int(data[field]) > 1]
+                    item = item.format(f=data[field],
+                                       e=e.upper(),
+                                       s=final_s)
+                    exp.append(item)
+
+            owners = [e.strip(' ')
+                      for e in data['project_owners'].split(' <br/> ')]
+            # Creating the output string to be returned
+            output = '<{cl} Object> {id} `{label}` ({access}) {n_subjects}'\
+                ' subject{s} {exp} (owner: {owner}) (created on {insert_date}'\
+                ')'
+            output = output.format(cl=self.__class__.__name__,
+                                   id=project_id,
+                                   label=name,
+                                   s={True: 's', False: ''}[n_subjects > 1],
+                                   n_subjects=n_subjects,
+                                   owner='/'.join(owners),
+                                   insert_date=data['insert_date'],
+                                   access=data['project_access'],
+                                   exp=' '.join(exp))
+
+            if SHOW_URL:
+                url = interface._server + self._uri + '?format=html'
+                output += ' ' + url
+
+            return output
+        else:
+            return '<%s Object> %s' % (self.__class__.__name__,
+                                       self._urn)
+
+    def prearchive_code(self):
+        """ Gets project prearchive code.
+        """
+        return int(self._intf._exec(join_uri(self._uri, 'prearchive_code')))
+
+    def set_prearchive_code(self, code):
+        """ Sets project prearchive code.
+
+            Parameters
+            ----------
+            code: 0 to 4
+        """
+        self._intf._exec(join_uri(self._uri, 'prearchive_code', code),
+                         'PUT')
+
+    def quarantine_code(self):
+        """ Gets project quarantine code.
+        """
+        return int(self._intf._exec(join_uri(self._uri, 'quarantine_code')))
+
+    def set_quarantine_code(self, code):
+        """ Sets project quarantine code.
+
+            Parameters
+            ----------
+            code: 0 to 1
+        """
+        self._intf._exec(join_uri(self._uri, 'quarantine_code', code),
+                         'PUT')
+
+    def current_arc(self):
+        """ Gets project current archive folder on the server.
+        """
+        return self._intf._exec(join_uri(self._uri, 'current_arc'))
+
+    def set_subfolder_in_current_arc(self, subfolder):
+        """ Changes project current archive subfolder on the server.
+        """
+        current_arc = self._intf._exec(join_uri(self._uri, 'current_arc'))
+
+        self._intf._exec(join_uri(self._uri, 'current_arc',
+                                  current_arc, subfolder),
+                         'PUT')
+
+    def accessibility(self):
+        """ Gets project accessibility.
+        """
+        return self._intf._exec(join_uri(self._uri, 'accessibility'), 'GET')
+
+    def set_accessibility(self, accessibility='protected'):
+        """ Sets project accessibility.
+
+            .. note::
+                Write access is given or not by the user level for a
+                specific project.
+
+            Parameters
+            ----------
+            accessibility: public | protected | private
+                Sets the project accessibility:
+                    - public: the project is visible and provides read
+                      access for anyone.
+                    - protected: the project is visible by anyone but the
+                      data is accessible for allowed users only.
+                    - private: the project is visible by allowed users only.
+
+        """
+        return self._intf._exec(join_uri(self._uri, 'accessibility',
+                                         accessibility), 'PUT')
+
+    def users(self):
+        """ Gets all registered users for this project.
+        """
+        return JsonTable(self._intf._get_json(join_uri(self._uri, 'users'))
+                         ).get('login', always_list=True)
+
+    def owners(self):
+        """ Gets owners of this project.
+        """
+        return JsonTable(self._intf._get_json(join_uri(self._uri, 'users'))
+                         ).where(displayname='Owners'
+                                 ).get('login', always_list=True)
+
+    def members(self):
+        """ Gets members of this project.
+        """
+        return JsonTable(self._intf._get_json(join_uri(self._uri, 'users'))
+                         ).where(displayname='Members'
+                                 ).get('login', always_list=True)
+
+    def collaborators(self):
+        """ Gets collaborator of this project.
+        """
+        return JsonTable(self._intf._get_json(join_uri(self._uri, 'users'))
+                         ).where(displayname='Collaborators'
+                                 ).get('login', always_list=True)
+
+    def user_role(self, login):
+        """ Gets the user level of the user for this project.
+
+            Parameters
+            ----------
+            login: string
+                A user of the project.
+
+            Returns
+            -------
+            string : owner | member | collaborator
+
+        """
+        j = JsonTable(self._intf._get_json(join_uri(self._uri, 'users')))
+        return ''.join(j.where(login=login)['displayname']).lower().rstrip('s')
+
+    def add_user(self, login, role='member'):
+        """ Adds a user to the project. The user must already exist on
+            the server.
+
+            Parameters
+            ----------
+            login: string
+                Valid username for the XNAT database.
+            role: owner | member | collaborator
+                The user level for this project:
+                    - owner: read and write access, as well as
+                      administrative privileges such as adding and removing
+                      users.
+                    - member: read access and can create new resources but
+                      not remove them.
+                    - collaborator: read access only.
+        """
+        self._intf._exec(join_uri(self._uri, 'users',
+                                  role.lstrip('s').title() + 's',
+                                  login
+                                  ),
+                         'PUT')
+
+    def remove_user(self, login):
+        """ Removes a user from the project.
+
+            Parameters
+            ----------
+            login: string
+                Valid username for the XNAT database.
+        """
+        self._intf._exec(join_uri(self._uri, 'users',
+                                  self.user_role(login).title() + 's',
+                                  login
+                                  ),
+                         'DELETE')
+
+    def datatype(self):
+        return 'xnat:projectData'
+
+    def experiments(self, id_filter='*'):
+        datapath = '%s/projects/%s/experiments'
+        dp = datapath % (self._intf._get_entry_point(), self.id())
+        return Experiments(dp, self._intf, id_filter)
+
+    def experiment(self, ID):
+        datapath = '%s/projects/%s/experiments/%s'
+        dp = datapath % (self._intf._get_entry_point(), self.id(), ID)
+
+        tmp = Experiment(dp, self._intf)
+        if tmp.id() == ID:
+            return tmp
+        else:
+            # if id id not mach given id (which may have been a label
+            # re-select with the ID of the matching experiment.
+            return Experiment(datapath % (
+                self._intf._get_entry_point(), self.id(), tmp.id()),
+                self._intf
+                )
+
+    def last_modified(self):
+        """ Gets the last modified dates for all the project subjects.
+
+            If any element related to a subject changes, experiment,
+            variable, scan, image etc... the date will be changed.
+        """
+        uri = '%s/subjects?columns=last_modified' % self._uri
+
+        return dict(JsonTable(self._intf._get_json(uri),
+                              order_by=['ID', 'last_modified']
+                              ).select(['ID', 'last_modified']
+                                       ).items()
+                    )
+
+    def add_custom_variables(self, custom_variables,
+                             allow_data_deletion=False):
+        """Adds a custom variable to a specified group
+
+        Parameters
+        ----------
+
+        custom_variables: a dictionary
+        allow_data_deletion : a boolean
+
+        Examples
+        --------
+
+        >>> variables = {'Subjects' : {'newgroup' : {'foo' : 'string',
+            'bar': 'int'}}}
+        >>> project.add_custom_variables(variables)
+
+        """
+        tree = lxml.etree.fromstring(self.get())
+
+        update = False
+
+        for protocol, value in custom_variables.items():
+            try:
+                protocol_element = tree.xpath(
+                    "//xnat:studyProtocol[@name='%s']" % protocol,
+                    namespaces=tree.nsmap).pop()
+
+            except IndexError:
+                raise ValueError(
+                    'Protocol %s not in current schema' % protocol
+                    )
+
+            try:
+                definitions_element = protocol_element.xpath(
+                    'xnat:definitions', namespaces=tree.nsmap).pop()
+            except IndexError:
+                update = True
+                definitions_element = lxml.etree.Element(
+                    lxml.etree.QName(tree.nsmap['xnat'], 'definitions'),
+                    nsmap=tree.nsmap
+                    )
+                protocol_element.append(definitions_element)
+
+            for group, fields in value.items():
+                try:
+                    group_element = definitions_element.xpath(
+                        "xnat:definition[@ID='%s']" % group,
+                        namespaces=tree.nsmap).pop()
+
+                    fields_element = group_element.xpath(
+                        "xnat:fields",
+                        namespaces=tree.nsmap).pop()
+
+                except IndexError:
+                    update = True
+
+                    group_element = lxml.etree.Element(
+                        lxml.etree.QName(tree.nsmap['xnat'], 'definition'),
+                        nsmap=tree.nsmap)
+                    group_element.set('ID', group)
+                    group_element.set(
+                        'data-type', protocol_element.get('data-type'))
+                    group_element.set('description', '')
+                    group_element.set('project-specific', '1')
+                    definitions_element.append(group_element)
+                    fields_element = lxml.etree.Element(
+                        lxml.etree.QName(tree.nsmap['xnat'], 'fields'),
+                        nsmap=tree.nsmap)
+                    group_element.append(fields_element)
+
+                for field, datatype in fields.items():
+                    try:
+                        field_element = fields_element.xpath(
+                            "xnat:field[@name='%s']" % field,
+                            namespaces=tree.nsmap).pop()
+                    except IndexError:
+                        field_element = lxml.etree.Element(
+                            lxml.etree.QName(tree.nsmap['xnat'], 'field'),
+                            nsmap=tree.nsmap)
+                        field_element.set('name', field)
+                        field_element.set('datatype', datatype)
+                        field_element.set('type', 'custom')
+                        field_element.set('required', '0')
+                        field_element.set(
+                            'xmlPath',
+                            "xnat:%s/fields/field[name=%s]/field" % (
+                                protocol_element.get(
+                                    'data-type').split(':')[-1], field))
+                        fields_element.append(field_element)
+                        update = True
+        if update:
+            body, content_type = httputil.file_message(
+                lxml.etree.tostring(tree).decode('utf-8'),
+                'text/xml',
+                'cust.xml',
+                'cust.xml')
+
+            uri = self._uri
+            if allow_data_deletion:
+                uri = self._uri + '?allowDataDeletion=true'
+            self._intf._exec(uri, method='PUT', body=str(body),
+                             headers={'content-type': content_type})
+
+    def get_custom_variables(self):
+        """Retrieves custom variables as a dictionary
+
+        It has the format {studyProtocol: { setname : {field: type, ...}}}
+
+        """
+        tree = lxml.etree.fromstring(self.get())
+        nsmap = tree.nsmap
+        custom_variables = {}
+        for studyprotocols in tree.xpath('//xnat:studyProtocol',
+                                         namespaces=nsmap):
+
+            protocol_name = studyprotocols.get('name')
+            custom_variables[protocol_name] = {}
+
+            for definition in studyprotocols.xpath(('xnat:definitions'
+                                                    '/xnat:definition'),
+                                                   namespaces=nsmap):
+
+                definition_id = definition.get('ID')
+                custom_variables[protocol_name][definition_id] = {}
+                for field in definition.xpath('xnat:fields/xnat:field',
+                                              namespaces=nsmap):
+
+                    field_name = field.get('name')
+                    if field.get('type') == 'custom':
+                        custom_variables[protocol_name][definition_id][
+                            field_name] = field.get('datatype')
+
+        return custom_variables
+
+    def aliases(self):
+        """Returns the aliases for this project.
+
+           Returns
+           -------
+           List of aliases
+        """
+
+        uri = '/data/projects'
+        options = {'columns': 'alias', 'format': 'csv'}
+        data = self._intf.get(uri, params=options).text
+        from .jsonutil import csv_to_json
+        data = csv_to_json(data)
+
+        # parse the results
+        return [item['alias'] for item in data
+                if item['alias'] and item['ID'] == self._urn]
+
+    def description(self):
+        """Returns the description for this project.
+
+        Returns
+        -------
+        Description (string) of the project.
+        """
+        return self.attrs.get('description')
+
+
+@add_metaclass(ElementType)
+class Subject(EObject):
+
+    def datatype(self):
+        return 'xnat:subjectData'
+
+    def __repr__(self):
+        interface = self._intf
+
+        # Check if subject exists
+        if self.exists():
+            subject_id = self.id()
+            columns = ['xnat:subjectData/PROJECT',
+                       'xnat:subjectData/SUBJECT_ID',
+                       'xnat:subjectData/INSERT_DATE',
+                       'xnat:subjectData/INSERT_USER',
+                       'xnat:subjectData/GENDER_TEXT',
+                       'xnat:subjectData/HANDEDNESS_TEXT',
+                       'xnat:subjectData/SES',
+                       'xnat:subjectData/ADD_IDS',
+                       'xnat:subjectData/RACE',
+                       'xnat:subjectData/ETHNICITY',
+                       'xnat:subjectData/SUBJECT_LABEL']
+
+            dt = 'xnat:subjectData'
+            data = interface.select(dt, columns=columns).all().data
+            interface._subjectData = data
+            data = [e for e in data if e['subject_id'] == subject_id][0]
+
+            # Collecting subject details
+            project_id = data['project']
+            age = self.attrs.get('age')
+            gender = data['gender_text']
+            handedness = data['handedness_text']
+            label = data['subject_label']
+            n_expes = len(list(self.experiments()))
+
+            ag = ''
+            if [age, gender, handedness] != ['', '', '']:
+                ag = []
+                if age != '':
+                    ag.append('Age: %s' % age)
+                if gender != '':
+                    ag.append('Gender: %s' % gender)
+                if handedness != '':
+                    ag.append('Handedness: %s' % handedness)
+                ag = '(%s)' % ' - '.join(ag)
+
+            # Creating the output string to be returned
+            output = '<{cl} Object> {id} `{label}` (project: {project}) {ag}'\
+                ' {n_expes} experiment{final_s}'
+            output = output.format(cl=self.__class__.__name__,
+                                   label=label,
+                                   id=subject_id,
+                                   project=project_id,
+                                   ag=ag,
+                                   n_expes=n_expes,
+                                   final_s={True: 's', False: ''}[n_expes > 1])
+
+            if SHOW_URL:
+                url = interface._server + self._uri + '?format=html'
+                output += ' ' + url
+
+            return output
+        else:
+            return '<%s Object> %s' % (self.__class__.__name__,
+                                       unquote(uri_last(self._uri))
+                                       )
+
+    def shares(self, id_filter='*'):
+        """ Returns the projects sharing this subject.
+
+            Returns
+            -------
+            Collection object.
+        """
+        return Projects(join_uri(self._uri, 'projects'),
+                        self._intf, id_filter)
+
+    def share(self, project, label=None, primary=False):
+        """ Share the subject with another project.
+
+            Parameters
+            ----------
+                project: string
+                    Target project name.
+                label: string
+                    Subject label as shared resource. By default, the original
+                    subject label is used.
+                primary: boolean
+                    If True, the ownership of the subject will be transferred to
+                    the target project. User must be owner of both projects to
+                    perform this operation.
+        """
+        owner_project = self.attrs.get('project')
+        aliases = self._intf.select.project(owner_project).aliases()
+        if project in [owner_project] + aliases:
+            raise ValueError("Cannot share a subject with its owner project.")
+
+        options = []
+        if label:
+            options.append('label=%s' % label)
+        else:
+            options.append('label=%s' % self.label())
+        if primary:
+            options.append('primary=true')
+
+        options = '?' + '&'.join(options)
+
+        self._intf._exec(join_uri(self._uri, 'projects', project) + options, 'PUT')
+
+    def unshare(self, project):
+        """ Unlink subject from a project it was shared with. Subject cannot be
+            unshared from the project that owns it.
+
+            Parameters
+            ----------
+                project: string
+                    Target project name.
+        """
+        owner_project = self.attrs.get('project')
+        aliases = self._intf.select.project(owner_project).aliases()
+        if project in [owner_project] + aliases:
+            raise ValueError("Cannot unlink a subject from its owner project.")
+
+        self._intf._exec(join_uri(self._uri, 'projects', project), 'DELETE')
+
+
+@add_metaclass(ElementType)
+class Experiment(EObject):
+
+    def __init__(self, cbase, interface):
+        items = cbase.split('/')
+        e = []
+        if 'subjects' not in items \
+                and 'projects' in items and 'experiments' in items:
+            ID = uri_last(cbase)
+            e = interface.array.experiments(experiment_id=ID).data
+
+        if len(e) == 1:
+            subject_id = e[0]['subject_ID']
+            project_id = e[0]['project']
+
+            cbase = '%s/projects/%s/subjects/%s/experiments/%s'
+            cbase = cbase % (interface._get_entry_point(),
+                             project_id,
+                             subject_id,
+                             ID)
+            return super(Experiment, self).__init__(cbase, interface)
+
+        return super(Experiment, self).__init__(cbase, interface)
+
+    def __repr__(self):
+        intf = self._intf
+
+        # Check if experiment exists
+        if self.exists():
+            eid = self.id()
+
+            e = intf.array.experiments(experiment_id=eid).data[0]
+            filter = [('{}/{}'.format(e['xsiType'], 'ID'), '=', eid)]
+            data = intf.select(e['xsiType']).where(filter).data[0]
+
+            # Collecting experiment details
+            project_id = data['project']
+            label = self.label()
+            subject_id = data['subject_id']
+            e = intf.array.experiments(experiment_id=eid,
+                                       columns=['subject_label']).data[0]
+            subject_label = e['subject_label']
+            insert_date = data['insert_date']
+            n_res = len(list(self.resources()))
+
+            n_scans = len(list(self.scans()))
+
+            # Creating the output string
+            output = '<{cl} Object> {id} `{label}` (subject: {subject_id} '\
+                     '`{subject_label}`) (project: {project}) {n_scans} '\
+                     'scan{final_s1} {n_res} resource{final_s2} (created on '\
+                     '{insert_date})'
+
+            fs = {True: 's', False: ''}
+            output = output.format(cl=self.__class__.__name__,
+                                   id=eid,
+                                   label=label,
+                                   subject_id=subject_id,
+                                   subject_label=subject_label,
+                                   project=project_id,
+                                   n_res=n_res,
+                                   insert_date=insert_date,
+                                   n_scans=n_scans,
+                                   final_s1=fs[n_scans > 1],
+                                   final_s2=fs[n_res > 1])
+            if SHOW_URL:
+                url = intf._server + self._uri + '?format=html'
+                output += ' ' + url
+            return output
+        else:
+            return '<%s Object> %s' % (self.__class__.__name__,
+                                       unquote(uri_last(self._uri)))
+
+    def shares(self, id_filter='*'):
+        """ Returns the projects sharing this experiment.
+
+            Returns
+            -------
+            Collection object.
+        """
+        return Projects(join_uri(self._uri, 'projects'),
+                        self._intf, id_filter)
+
+    def share(self, project, label=None, primary=False):
+        """ Share the experiment with another project.
+
+            Parameters
+            ----------
+                project: string
+                    Target project name.
+                label: string
+                    Experiment label as shared resource. By default, the original
+                    experiment label is used.
+                primary: boolean
+                    If True, the ownership of the subject will be transferred to
+                    the target project. User must be owner of both projects to
+                    perform this operation.
+        """
+        owner_project = self.attrs.get('project')
+        aliases = self._intf.select.project(owner_project).aliases()
+        if project in [owner_project] + aliases:
+            raise ValueError("Cannot share an experiment with its owner project.")
+
+        options = []
+        if label:
+            options.append('label=%s' % label)
+        else:
+            options.append('label=%s' % self.label())
+        if primary:
+            options.append('primary=true')
+
+        options = '?' + '&'.join(options)
+
+        self._intf._exec(join_uri(self._uri, 'projects', project) + options, 'PUT')
+
+    def unshare(self, project):
+        """ Unlink experiment from a project it was shared with. Experiment cannot
+            be unshared from the project that owns it.
+
+            Parameters
+            ----------
+                project: string
+                    Target project name.
+        """
+        owner_project = self.attrs.get('project')
+        aliases = self._intf.select.project(owner_project).aliases()
+        if project in [owner_project] + aliases:
+            raise ValueError("Cannot unlink an experiment from its owner project.")
+
+        self._intf._exec(join_uri(self._uri, 'projects', project), 'DELETE')
+
+    def trigger_pipelines(self):
+        """ Triggers the AutoRun pipeline.
+        """
+        self._intf._exec(self._uri + '?triggerPipelines=true', 'PUT')
+
+    def fix_scan_types(self):
+        """ Populate empty scan TYPE attributes based on how similar
+            scans were populated.
+        """
+        self._intf._exec(self._uri + '?fixScanTypes=true', 'PUT')
+
+    def pull_data_from_headers(self):
+        """ Pull DICOM header values into the session.
+        """
+        self._intf._exec(self._uri + '?pullDataFromHeaders=true', 'PUT')
+
+    def trigger(self, pipelines=True, fix_types=True, scan_headers=True):
+        """ Run several triggers in a single call.
+
+            Parameters
+            ----------
+            pipelines: boolean
+                Same as trigger_pipelines.
+            fix_types: boolean
+                Same as fix_scan_types.
+            scan_headers: boolean
+                Same as pull_data_from headers.
+        """
+        if not all([not pipelines, not fix_types, not scan_headers]):
+            options = []
+            if pipelines:
+                options.append('triggerPipelines=true')
+            if fix_types:
+                options.append('fixScanTypes=true')
+            if scan_headers:
+                options.append('pullDataFromHeaders=true')
+
+            options = '?' + '&'.join(options)
+
+            self._intf._exec(self._uri + options, 'PUT', body=[])
+
+
+@add_metaclass(ElementType)
+class Assessor(EObject):
+
+    def __init__(self, uri, interface):
+        EObject.__init__(self, uri, interface)
+
+        self.provenance = Provenance(self)
+
+    def set_param(self, key, value):
+        self.attrs.set('%s/parameters/addParam[name=%s]/addField'
+                       % (self.datatype(), key),
+                       value
+                       )
+
+    def get_param(self, key):
+        return self.xpath(
+            "//xnat:addParam[@name='%s']/child::text()" % key)[-1]
+
+    def get_params(self):
+        return self.xpath("//xnat:addParam/child::text()")[1::2]
+
+    def params(self):
+        return self.xpath('//xnat:addParam/attribute::*')
+
+
+@add_metaclass(ElementType)
+class Reconstruction(EObject):
+
+    def __init__(self, uri, interface):
+        EObject.__init__(self, uri, interface)
+
+        self.provenance = Provenance(self)
+
+    def datatype(self):
+        return (super(Reconstruction, self).datatype()
+                or 'xnat:reconstructedImageData'
+                )
+
+
+@add_metaclass(ElementType)
+class Scan(EObject):
+
+    def __repr__(self):
+        interface = self._intf
+
+        # Check if scan exists
+        if self.exists():
+            scan_id = self.id()
+
+            # Collect scan details
+            attrs = ['ID', 'type', 'frames', 'quality']
+            base_url = uri_parent(self._uri)
+            scans = self._intf._get_json('{}?columns={}'.format(base_url,
+                                                                ','.join(attrs)))
+            scan_info = [r for r in scans if r['ID'] == scan_id][0]
+
+            # Creating the output string
+            output = '<{cl} Object> {id} (`{type}` {n_frames} frames) {quality}'
+            output = output.format(cl=self.__class__.__name__,
+                                   id=scan_id,
+                                   type=scan_info['type'],
+                                   n_frames=scan_info['frames'],
+                                   quality=scan_info['quality'])
+            if SHOW_URL:
+                url = interface._server + self._uri + '?format=html'
+                output += ' ' + url
+            return output
+        else:
+            return '<%s Object> %s' % (self.__class__.__name__,
+                                       unquote(uri_last(self._uri)))
+
+    def set_param(self, key, value):
+        self.attrs.set('%s/parameters/addParam[name=%s]/addField'
+                       % (self.datatype(), key),
+                       value)
+
+    def get_param(self, key):
+        return self.xpath(
+            "//xnat:addParam[@name='%s']/child::text()" % key)[-1]
+
+    def get_params(self):
+        return self.xpath("//xnat:addParam/child::text()")[1::2]
+
+    def params(self):
+        return self.xpath('//xnat:addParam/attribute::*')
+
+
+@add_metaclass(ElementType)
+class Resource(EObject):
+
+    def __init__(self, cbase, interface):
+        from pyxnat.core.errors import DatabaseError
+        super(Resource, self).__init__(cbase, interface)
+
+        mf = interface._mod_functions.get(self._urn, [])
+        if len(mf) == 0:
+            uri = uri_parent(self._uri)
+            try:
+                d = self._intf._get_json(uri)
+                r = [e for e in d if e['xnat_abstractresource_id'] == self._urn]
+                if len(r) == 1:
+                    label = r[0]['label']
+                    mf = interface._mod_functions.get(label, [])
+            except DatabaseError:
+                print('Warning:', self._uri, 'raising DatabaseError')
+
+        for f in mf:
+            setattr(self, f.__name__, types.MethodType(f, self))
+
+        return None
+
+    def __repr__(self):
+
+        def sizeof_fmt(num, suffix='B'):
+            for unit in ['', 'K', 'M', 'G', 'T', 'P', 'E', 'Z']:
+                if abs(num) < 1024.0:
+                    return "%3.2f %s%s" % (num, unit, suffix)
+                num /= 1024.0
+            return "%.2f %s%s" % (num, 'Y', suffix)
+
+        # Check if resource exists
+        if self.exists():
+            resource_id = self.id()
+            base_url = uri_parent(self._uri)
+            resources = self._intf._get_json(base_url)
+            res_info = [r for r in resources
+                        if r['xnat_abstractresource_id'] == resource_id][0]
+            fs = '0.0 B'
+            if res_info['file_size'] != '':
+                fs = sizeof_fmt(float(res_info['file_size']))
+
+            # Creating the output string
+            output = '<{cl} Object> {id} `{label}` ({fc} files {fs})'
+            output = output.format(label=self.label(),
+                                   cl=self.__class__.__name__,
+                                   id=resource_id,
+                                   fc=res_info['file_count'],
+                                   fs=fs)
+            return output
+        else:
+            return '<%s Object> %s' % (self.__class__.__name__,
+                                       unquote(uri_last(self._uri)))
+
+    def get(self, dest_dir, extract=False):
+        """ Downloads all the files within a resource.
+
+            ..warning::
+                Currently XNAT adds parent folders in the zip file that
+                is downloaded to avoid name clashes if several resources
+                are downloaded in the same folder. In order to be able to
+                download the data uploaded previously with the same
+                structure, pyxnat extracts the zip file, removes the extra
+                paths and if necessary re-zips it. Careful, it may take
+                time, and there is the problem of name clashes.
+
+            Parameters
+            ----------
+            dest_dir: string
+                Destination directory for the resource data.
+                if dest_dir is None, then the user's Downloads directory is
+                used as the default download location.
+            extract: boolean
+                If True, the downloaded zip file is extracted.
+                If False, not extracted.
+
+            Returns
+            -------
+            If extract is False, the zip file path.
+            If extract is True, the list of file paths previously in
+            the zip.
+        """
+        zip_location = op.join(dest_dir, uri_last(self._uri) + '.zip')
+
+        with open(zip_location, 'wb') as f:
+            response = self._intf.get(join_uri(self._uri, 'files') +
+                                      '?format=zip', stream=True)
+            try:
+                count = 0
+                for chunk in response.iter_content(chunk_size=1024):
+                    if chunk:  # filter out keep-alive new chunks
+                        f.write(chunk)
+                        count += 1
+                        if count % 10 == 0:
+                            # flush the buffer every once in a while.
+                            f.flush()
+                f.flush()  # and one last flush.
+            except Exception as e:
+                sys.stderr.write(e)
+            finally:
+                response.close()
+
+        if DEBUG:
+            print(zip_location)
+
+        fzip = zipfile.ZipFile(zip_location, 'r')
+        fzip.extractall(path=dest_dir)
+        fzip.close()
+
+        members = []
+        fzip_namelist = [str(Path(item)) for item in fzip.namelist()]
+        for member in fzip_namelist:
+            old_path = op.join(dest_dir, member)
+            if DEBUG:
+                print(member)
+                print(member.split('files', 1))
+            new_path = op.join(
+                dest_dir,
+                uri_last(self._uri),
+                member.split('files', 1)[1].split(os.sep, 1)[1]
+                )
+
+            if not op.exists(op.dirname(new_path)):
+                os.makedirs(op.dirname(new_path))
+
+            shutil.move(old_path, new_path)
+
+            members.append(new_path)
+
+        # TODO: cache.delete(...)
+        for extracted in fzip_namelist:
+            pth = op.join(dest_dir, extracted.split(os.sep, 1)[0])
+
+            if op.isdir(pth):
+                shutil.rmtree(pth)
+
+        os.remove(zip_location)
+
+        if not extract:
+            fzip = zipfile.ZipFile(zip_location, 'w')
+            arcprefix = op.commonprefix(members).rpartition(os.sep)[0]
+            arcroot = '/%s' % op.split(arcprefix.rstrip(os.sep))[1]
+            for member in members:
+                opj = op.join(arcroot, member.split(arcprefix)[1])
+                fzip.write(member, opj)
+            fzip.close()
+            unzippedTree = op.join(dest_dir, uri_last(self._uri))
+            if op.exists(unzippedTree):
+                if op.isdir(unzippedTree):
+                    shutil.rmtree(op.join(dest_dir, uri_last(self._uri)))
+                else:
+                    os.remove(unzippedTree)
+
+        return zip_location if op.exists(zip_location) else members
+
+    def put(self, sources, overwrite=False, extract=True, **datatypes):
+        """ Insert a list of files in a single resource element.
+
+            This method takes all the files an creates a zip with them
+            which will be the element to be uploaded and then extracted on
+            the server.
+            If the files have a common prefix directory, that directory name
+            will be used.  If not, then "files" will be used as the zip name.
+
+            If avaiable, compression will be used on the zip file.
+
+            Parameters
+            ----------
+            sources: List of paths of files to upload.
+
+            overwrite: boolean
+                If True, overwrite the files that already exist under the
+                    given id.
+                If False, do not overwrite (Default)
+
+            extract: boolean
+                If True, the uploaded zip file is extracted. (Default)
+                If False, the file is not extracted.
+
+        """
+        zip_location = tempfile.mkdtemp(suffix='pyxnat')
+
+        # get the largest common directory.
+        arcprefix, _, _ = op.commonprefix(sources).rpartition(op.sep)
+        # get just the name of the largest common directory.
+        zip_name = op.split(arcprefix.rstrip(op.sep))[1]
+        arcroot = '/%s' % zip_name
+
+        if not zip_name:
+            # if no common prefix, then use "files" as the zip file name.
+            # inside, each file will be directly under the zip root.
+            zip_name = "files"
+
+        zip_name = op.join(zip_location, zip_name + ".zip")
+        fzip = None
+        try:
+            # use compression if avaiable.
+            fzip = zipfile.ZipFile(zip_name, 'w', zipfile.ZIP_DEFLATED)
+        except RuntimeError:
+            print("Zip compression not supported for uploading files.")
+            fzip = zipfile.ZipFile(zip_name, 'w')
+
+        for src in sources:
+            fzip.write(src, op.join(arcroot, src.split(arcprefix)[1]))
+
+        fzip.close()
+
+        self.put_zip(zip_name, overwrite=overwrite, extract=extract,
+                     **datatypes)
+        os.remove(zip_name)
+        os.rmdir(zip_location)
+
+    def put_zip(self, zip_location, overwrite=False, extract=True,
+                **datatypes):
+        """ Uploads a zip or tgz file an then extracts it on the server.
+
+            After the compressed file is extracted the individual
+            files are accessible separately, or as a whole using get_zip.
+
+            Parameters
+            ----------
+            zip_location: Path to zip file for upload.
+
+            overwrite: boolean
+                If True, overwrite the files that already exist under the
+                    given id.
+                If False, do not overwrite (Default)
+
+            extract: boolean
+                If True, the uploaded zip file is extracted. (Default)
+                If False, the file is not extracted.
+        """
+        if not self.exists():
+            self.create(**datatypes)
+
+        if extract:
+            do_extract = '?extract=true'
+        else:
+            do_extract = ''
+
+        self.file(op.split(zip_location)[1] + do_extract
+                  ).put(zip_location, overwrite=overwrite, **datatypes)
+
+    def put_dir(self, src_dir, overwrite=False, extract=True, **datatypes):
+        """ Finds recursively all the files in a folder and uploads
+            them using `insert`. Uses put_zip internally.
+
+            Parameters
+            ----------
+            src_dir: Path to directory to upload.
+
+            overwrite: boolean
+                If True, overwrite the files that already exist under the
+                    given id.
+                If False, do not overwrite (Default)
+
+            extract: boolean
+                If True, the uploaded zip file is extracted. (Default)
+                If False, the file is not extracted.
+        """
+        self.put(find_files(src_dir), overwrite=overwrite, extract=extract,
+                 **datatypes)
+
+    batch_insert = put
+    zip_insert = put_zip
+    dir_insert = put_dir
+
+    def datatype(self):
+        return (super(Resource, self).datatype()
+                or 'xnat:abstractResource'
+                )
+
+    def attributes(self):
+        """ Resource attributes include:
+                - label
+                - file_count
+                - file_size in bytes
+                - tags
+                - format
+                - content
+            Returns
+            -------
+            dict : a dictionary with the resource attributes
+        """
+
+        return self._getcells(['label', 'file_count', 'file_size',
+                               'tags', 'format', 'content'])
+
+
+class In_Resource(Resource):
+
+    def parent(self):
+        uri = uri_grandparent(self._uri)
+        Klass = globals()[uri.split('/')[-3].title().rsplit('s', 1)[0]]
+        return Klass(uri_parent(uri), self._intf)
+
+
+@add_metaclass(ElementType)
+class Out_Resource(Resource):
+
+    def parent(self):
+        uri = uri_grandparent(self._uri)
+        Klass = globals()[uri.split('/')[-3].title().rsplit('s', 1)[0]]
+        return Klass(uri_parent(uri), self._intf)
+
+
+@add_metaclass(ElementType)
+class File(EObject):
+    """ EObject for files stored in XNAT.
+    """
+
+    def __init__(self, uri, interface):
+        """
+            Parameters
+            ----------
+            uri: string
+                The file resource URI
+            interface: Interface Object
+        """
+
+        EObject.__init__(self, uri, interface)
+        self._urn = file_path(uri)
+        self._absuri = None
+
+    def __repr__(self):
+        return '<%s Object> %s' % (self.__class__.__name__,
+                                   self._urn)
+
+    def attributes(self):
+        """ Files attributes include:
+                - URI
+                - Name
+                - Size in bytes
+                - path (relative to the parent resource)
+                - file_tags
+                - file_format
+                - file_content
+                - digest
+
+            Returns
+            -------
+            dict : a dictionary with the file attributes
+        """
+
+        return self._getcells(['URI', 'Name', 'Size', 'path', 'digest',
+                               'file_tags', 'file_format', 'file_content'])
+
+    def get(self, dest=None):
+        """ Downloads the file.
+
+            Parameters
+            ----------
+            dest: string | None
+
+                - If dest is None, then the user's Downloads directory is used
+                    as the default download location.
+                - Else the file is downloaded at the requested location.
+                    Path should include the file name.
+                    eg: /path/to/file.txt
+
+            Returns
+            -------
+            string : the file location.
+        """
+        if not self._absuri:
+            self._absuri = self._getcell('URI')
+
+        if self._absuri is None:
+            raise DataError('Cannot get file: does not exists')
+
+        if not dest:
+            dest = op.join(op.expanduser("~"), 'Downloads', self.id())
+            if not ensure_dir_exists(op.dirname(dest)):
+                if DEBUG:
+                    print("File.get: failed to create dir")
+                raise DataError('Cannot create dir for file: %s' % (dest))
+
+        if DEBUG:
+            print(("get_file:", dest))
+
+        with open(dest, 'wb') as f:
+            response = self._intf.get(self._uri, stream=True)
+            try:
+                count = 0
+                for chunk in response.iter_content(chunk_size=1024):
+                    if chunk:  # filter out keep-alive new chunks
+                        f.write(chunk)
+                        count += 1
+                        if count % 10 == 0:
+                            # flush the buffer every once in a while.
+                            f.flush()
+                f.flush()  # and one last flush.
+            except Exception as e:
+                sys.stderr.write(e)
+            finally:
+                response.close()
+        return dest
+
+    def get_copy(self, dest=None):
+        """ Downloads the file to the cache directory but creates a copy at
+            the specified location.
+
+            Parameters
+            ----------
+            dest: string | None
+                - file path for the copy
+                - if None a copy is created at a default location based
+                  on the file URI on the server
+
+            Returns
+            -------
+            string : the copy location.
+        """
+
+        return self.get(dest)
+
+    def put(self, src, format='U', content='U', tags='U', overwrite=False,
+            **datatypes):
+        """ Uploads a file to XNAT.
+
+            Parameters
+            ----------
+            src: string
+                Location of the local file to upload or the actual content
+                to upload.
+            format: string
+                Optional parameter to specify the file format.
+                Defaults to 'U'.
+            content: string
+                Optional parameter to specify the file content.
+                Defaults to 'U'.
+            tags: string
+                Optional parameter to specify tags for the file.
+                Defaults to 'U'.
+            overwrite: boolean
+                Optional parameter to specify if the file should be
+                overwritten. Defaults to False.
+        """
+
+        # First make sure parents and grandparents exist.
+
+        # URI is in the form of data/.../something/files/me so
+        # guri = data/.../something
+        guri = uri_grandparent(self._uri)
+
+        if not self._intf.select(guri).exists():
+            self._intf.select(guri).insert(**datatypes)
+
+        resource_id = self._intf.select(guri).id()
+        isFile = False
+
+        # Cleanup the src and make sure it exists.
+        try:
+            if op.exists(src):
+                isFile = True
+                # path = src
+                # name = op.basename(path).split('?')[0]
+            # else:
+                # path = self._uri.split('/')[-1]
+                # name = path
+        except Exception:
+            pass  # FIXME
+            # path = self._uri.split('/')[-1]
+            # name = path
+
+        self._absuri = unquote(
+            re.sub('resources/.*?/',
+                   'resources/%s/' % resource_id, self._uri)
+            )
+
+        query_args = {
+            'format': format,
+            'content': content,
+            'tags': tags,
+            'overwrite': 'true' if overwrite else 'false',
+            'inbody': 'true'
+            }
+
+        if 'params' in datatypes:
+            query_args.update(datatypes['params'])
+            # Pass on params such as event_reason
+
+        if '?' in self._absuri:
+            k, v = self._absuri.split('?')[1].split('=')
+            query_args[k] = v
+            self._absuri = self._absuri.split('?')[0]
+
+        if DEBUG:
+            print(('INSERT FILE', op.exists(src)))
+            print("URI is: " + self._absuri)
+
+        response = None
+        if isFile:
+            # If src was a file, use inbody streaming to send the file
+            with open(src, 'rb') as f:
+                response = self._intf.post(self._absuri, params=query_args,
+                                           data=f)
+        else:
+            # If it wasn't a file we can just dump the src as data directly.
+            response = self._intf.post(self._absuri, params=query_args,
+                                       data=src)
+
+        # default error handling.
+        if (response is not None and not response.ok) or \
+           is_xnat_error(response.content):
+            if DEBUG:
+                print(response.keys())
+                print(response.get("status"))
+            msg = '''pyxnat.file.put failure:
+                        URI: {response.url}
+                        status code: {response.status_code}
+                        headers: {response.headers}
+                        content: {response.content}
+                    '''.format(response=response)
+            catch_error(response.content, msg)
+
+    insert = put
+    create = put
+
+    def delete(self):
+        """ Deletes the file on the server.
+        """
+        if not self._absuri:
+            self._absuri = self._getcell('URI')
+
+        if self._absuri is None:
+            raise DataError('Cannot delete file: does not exists')
+
+        return self._intf._exec(self._absuri, 'DELETE')
+
+    def size(self):
+        """ Gets the file size.
+        """
+        return self._getcell('Size')
+
+    def labels(self):
+        """ Gets the file labels.
+        """
+        return self._getcell('file_tags')
+
+    def format(self):
+        """ Gets the file format.
+        """
+        return self._getcell('file_format')
+
+    def content(self):
+        """ Gets the file content description.
+        """
+        return self._getcell('file_content')
+
+    def last_modified(self):
+        """ Gets the file last-modified date.
+        """
+
+        if not self._absuri:
+            self._absuri = self._getcell('URI')
+
+        if self._absuri is None:
+            raise DataError('Cannot get file: does not exists')
+
+        info = self._intf._get_head(self._absuri)
+        return info['last-modified']
+
+
+@add_metaclass(ElementType)
+class In_File(File):
+    pass
+
+
+@add_metaclass(ElementType)
+class Out_File(File):
+    pass
+
+
+@add_metaclass(CollectionType)
+class Projects(CObject):
+    pass
+
+
+@add_metaclass(CollectionType)
+class Subjects(CObject):
+
+    def sharing(self, projects=[]):
+        return Subjects([eobj for eobj in self
+                         if set(projects).issubset(eobj.shares().get())],
+                        self._intf)
+
+    def share(self, project):
+        for eobj in self:
+            eobj.share(project)
+
+    def unshare(self, project):
+        for eobj in self:
+            eobj.unshare(project)
+
+
+@add_metaclass(CollectionType)
+class Experiments(CObject):
+
+    def sharing(self, projects=[]):
+        return Experiments([eobj for eobj in self
+                            if set(projects).issubset(eobj.shares().get())],
+                           self._intf)
+
+    def share(self, project):
+        for eobj in self:
+            eobj.share(project)
+
+    def unshare(self, project):
+        for eobj in self:
+            eobj.unshare(project)
+
+
+@add_metaclass(CollectionType)
+class Assessors(CObject):
+
+    def download(self, dest_dir, type="ALL",
+                 name=None, extract=False, safe=False, removeZip=False):
+        """
+        A wrapper around :func:`downloadutils.download`
+        """
+        return downloadutils.download(dest_dir, self, type, name,
+                                      extract, safe, removeZip)
+
+
+@add_metaclass(CollectionType)
+class Reconstructions(CObject):
+
+    def download(self, dest_dir, type="ALL",
+                 name=None, extract=False, safe=False, removeZip=False):
+        """
+        A wrapper around :func:`downloadutils.download`
+        """
+        return downloadutils.download(dest_dir, self, type, name,
+                                      extract, safe, removeZip)
+
+
+@add_metaclass(CollectionType)
+class Scans(CObject):
+
+    def download(self, dest_dir, type="ALL",
+                 name=None, extract=False, safe=False, removeZip=False):
+        """
+        A wrapper around :func:`downloadutils.download`
+
+        """
+        return downloadutils.download(dest_dir, self, type, name,
+                                      extract, safe, removeZip)
+
+
+@add_metaclass(CollectionType)
+class Resources(CObject):
+    pass
+
+
+@add_metaclass(CollectionType)
+class In_Resources(Resources):
+    pass
+
+
+@add_metaclass(CollectionType)
+class Out_Resources(Resources):
+    pass
+
+
+@add_metaclass(CollectionType)
+class Files(CObject):
+    pass
+
+
+@add_metaclass(CollectionType)
+class In_Files(Files):
+    pass
+
+
+@add_metaclass(CollectionType)
+class Out_Files(Files):
+    pass
+
+# Utility functions for downloading and extracting zip archives
+
+
+def _datatypes_from_query(query):
+    datatypes = []
+
+    for constraint in query:
+        if isinstance(constraint, list):
+            datatypes.extend(_datatypes_from_query(constraint))
+        elif isinstance(constraint, tuple):
+            datatypes.append(constraint[0].split('/')[0])
+
+    return datatypes
+
+
+def query_with(interface, join_field,
+               common_field, return_values, _filter):
+
+    _stm = (join_field.split('/')[0], return_values)
+    _cls = rewrite_query(interface, join_field,
+                         common_field, _filter)
+
+    return interface.select(*_stm).where(_cls)
+
+
+def rewrite_query(interface, join_field,
+                  common_field, _filter):
+
+    _new_filter = []
+
+    for _f in _filter:
+        if isinstance(_f, list):
+            _new_filter.append(rewrite_query(
+                interface, join_field, common_field, _f))
+
+        elif isinstance(_f, tuple):
+            _datatype = _f[0].split('/')[0]
+            _res = interface.select(
+                _datatype, ['%s/%s' % (_datatype, common_field)]
+                ).where([_f, 'AND'])
+
+            _new_f = [(join_field, '=', '%s' % sid)
+                      for sid in _res['subject_id']
+                      ]
+
+            _new_f.append('OR')
+            _new_filter.append(_new_f)
+
+        elif isinstance(_f, (str, unicode)):
+            _new_filter.append(_f)
+
+        else:
+            raise Exception('Invalid filter')
+
+    return _new_filter
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/schema.py` & `bbrc-pyxnat-1.6/pyxnat/core/schema.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-from six import string_types
-# REST collection resources tree
-resources_tree = {
-    'projects': ['subjects', 'resources'],
-    'subjects': ['experiments', 'resources'],
-    'experiments': ['assessors', 'reconstructions', 'scans', 'resources'],
-    'assessors': ['resources', 'in_resources', 'out_resources'],
-    'reconstructions': ['in_resources', 'out_resources'],
-    'scans': ['resources'],
-    'resources': ['files'],
-    'files': [],
-    'in_resources': ['files'],
-    'in_files': [],
-    'out_resources': ['files'],
-    'out_files': [],
-    }
-
-prearc_tree = {'projects': ['scans'],
-               'scans': ['resources'],
-               'resources': ['files']
-               }
-# REST resources that are not natively supported
-extra_resources_tree = {'projects': ['assessors', 'scans', 'reconstructions'],
-                        'subjects': ['assessors', 'scans', 'reconstructions'],
-                        }
-
-# REST <Python to URI> translation table
-rest_translation = {'in_resources': 'in/resources',
-                    'in_files': 'in/files',
-                    'out_resources': 'out/resources',
-                    'out_files': 'out/files',
-                    'in_resource': 'in/resource',
-                    'in_file': 'in/file',
-                    'out_resource': 'out/resource',
-                    'out_file': 'out/file',
-                    }
-
-
-# REST json format <id_header, label_header>
-json = {'projects': ['ID', 'ID'],
-        'subjects': ['ID', 'label'],
-        'experiments': ['ID', 'label'],
-        'assessors': ['ID', 'label'],
-        'reconstructions': ['ID', 'label'],
-        'scans': ['ID', 'ID'],
-        'resources': ['xnat_abstractresource_id', 'label'],
-        'out_resources': ['xnat_abstractresource_id', 'label'],
-        'in_resources': ['xnat_abstractresource_id', 'label'],
-        'files': ['path', 'path']}
-
-resources_singular = [key.rsplit('s', 1)[0] for key in resources_tree.keys()]
-resources_plural = resources_tree.keys()
-resources_types = resources_singular + list(resources_plural)
-
-default_datatypes = {'projects': 'xnat:projectData',
-                     'subjects': 'xnat:subjectData',
-                     'experiments': 'xnat:mrSessionData',
-                     'assessors': 'xnat:mrAssessorData',
-                     'reconstructions': 'xnat:reconstructedImageData',
-                     'scans': 'xnat:mrScanData',
-                     'resources': None,
-                     'in_resources': None,
-                     'out_resources': None,
-                     }
-
-
-def datatype_attributes(root, datatype):
-    def _iterchildren(node, pathsofar):
-        elements = []
-
-        for child in node.iterchildren():
-            if isinstance(child.tag, string_types) \
-               and child.tag.split('}')[1] == 'element':
-                elements.append('%s/%s' % (pathsofar, child.get('name')))
-                elements.extend(_iterchildren(child, '%s/%s' %
-                                (pathsofar, child.get('name'))))
-
-            elif isinstance(child.tag, string_types) and \
-                    child.tag.split('}')[1] == 'attribute':
-                elements.append('%s/%s' % (pathsofar, child.get('name')))
-
-            elif isinstance(child.tag, string_types) \
-                    and child.tag.split('}')[1] == 'extension':
-
-                ct_xpath = "/xs:schema/xs:complexType[@name='%s']" % \
-                    child.get('base').split(':')[1]
-
-                rt = node.getroottree()
-                for complex_type in rt.xpath(ct_xpath, namespaces=child.nsmap):
-
-                    same = False
-
-                    for ancestor in child.iterancestors():
-                        if ancestor.get('name') == \
-                                child.get('base').split(':')[1]:
-                            same = True
-                            break
-
-                    if not same:
-                        elements.extend(_iterchildren(complex_type,
-                                                      pathsofar)
-                                        )
-
-                    elements.extend(_iterchildren(child, pathsofar))
-
-            else:
-                elements.extend(_iterchildren(child, pathsofar))
-
-        return elements
-
-    ct_xpath = "/xs:schema/xs:complexType[@name='%s']" % \
-        datatype.split(':')[1]
-
-    attributes = []
-
-    for complex_type in root.xpath(ct_xpath, namespaces=root.nsmap):
-        for child in complex_type.iterchildren():
-            attributes.extend(_iterchildren(child, datatype))
-
-    return attributes
-
-
-def datatypes(root):
-    nsmap = get_nsmap(root)
-
-    return [element.get('type')
-            for element in root.xpath('/xs:schema/xs:element',
-                                      namespaces=nsmap)]
-                                      
-
-def get_nsmap(node):
-    nsmap = node.nsmap
-    none_ns = node.nsmap.get(None)
-
-    if none_ns is None:
-        nsmap[none_ns.rsplit('/', 1)[1]] = none_ns
-        del nsmap[None]
-
-    return nsmap
-
-
-def class_name(self):
-    """
-    Return the name of this class without qualification.
-    eg. If the class name is "x.y.class" return only "class"
-    """
-    return self.__class__.__name__.split('.')[-1]
+from six import string_types
+# REST collection resources tree
+resources_tree = {
+    'projects': ['subjects', 'resources'],
+    'subjects': ['experiments', 'resources'],
+    'experiments': ['assessors', 'reconstructions', 'scans', 'resources'],
+    'assessors': ['resources', 'in_resources', 'out_resources'],
+    'reconstructions': ['in_resources', 'out_resources'],
+    'scans': ['resources'],
+    'resources': ['files'],
+    'files': [],
+    'in_resources': ['files'],
+    'in_files': [],
+    'out_resources': ['files'],
+    'out_files': [],
+    }
+
+prearc_tree = {'projects': ['scans'],
+               'scans': ['resources'],
+               'resources': ['files']
+               }
+# REST resources that are not natively supported
+extra_resources_tree = {'projects': ['assessors', 'scans', 'reconstructions'],
+                        'subjects': ['assessors', 'scans', 'reconstructions'],
+                        }
+
+# REST <Python to URI> translation table
+rest_translation = {'in_resources': 'in/resources',
+                    'in_files': 'in/files',
+                    'out_resources': 'out/resources',
+                    'out_files': 'out/files',
+                    'in_resource': 'in/resource',
+                    'in_file': 'in/file',
+                    'out_resource': 'out/resource',
+                    'out_file': 'out/file',
+                    }
+
+
+# REST json format <id_header, label_header>
+json = {'projects': ['ID', 'ID'],
+        'subjects': ['ID', 'label'],
+        'experiments': ['ID', 'label'],
+        'assessors': ['ID', 'label'],
+        'reconstructions': ['ID', 'label'],
+        'scans': ['ID', 'ID'],
+        'resources': ['xnat_abstractresource_id', 'label'],
+        'out_resources': ['xnat_abstractresource_id', 'label'],
+        'in_resources': ['xnat_abstractresource_id', 'label'],
+        'files': ['path', 'path']}
+
+resources_singular = [key.rsplit('s', 1)[0] for key in resources_tree.keys()]
+resources_plural = resources_tree.keys()
+resources_types = resources_singular + list(resources_plural)
+
+default_datatypes = {'projects': 'xnat:projectData',
+                     'subjects': 'xnat:subjectData',
+                     'experiments': 'xnat:mrSessionData',
+                     'assessors': 'xnat:mrAssessorData',
+                     'reconstructions': 'xnat:reconstructedImageData',
+                     'scans': 'xnat:mrScanData',
+                     'resources': None,
+                     'in_resources': None,
+                     'out_resources': None,
+                     }
+
+
+def datatype_attributes(root, datatype):
+    def _iterchildren(node, pathsofar):
+        elements = []
+
+        for child in node.iterchildren():
+            if isinstance(child.tag, string_types) \
+               and child.tag.split('}')[1] == 'element':
+                elements.append('%s/%s' % (pathsofar, child.get('name')))
+                elements.extend(_iterchildren(child, '%s/%s' %
+                                (pathsofar, child.get('name'))))
+
+            elif isinstance(child.tag, string_types) and \
+                    child.tag.split('}')[1] == 'attribute':
+                elements.append('%s/%s' % (pathsofar, child.get('name')))
+
+            elif isinstance(child.tag, string_types) \
+                    and child.tag.split('}')[1] == 'extension':
+
+                ct_xpath = "/xs:schema/xs:complexType[@name='%s']" % \
+                    child.get('base').split(':')[1]
+
+                rt = node.getroottree()
+                for complex_type in rt.xpath(ct_xpath, namespaces=child.nsmap):
+
+                    same = False
+
+                    for ancestor in child.iterancestors():
+                        if ancestor.get('name') == \
+                                child.get('base').split(':')[1]:
+                            same = True
+                            break
+
+                    if not same:
+                        elements.extend(_iterchildren(complex_type,
+                                                      pathsofar)
+                                        )
+
+                    elements.extend(_iterchildren(child, pathsofar))
+
+            else:
+                elements.extend(_iterchildren(child, pathsofar))
+
+        return elements
+
+    ct_xpath = "/xs:schema/xs:complexType[@name='%s']" % \
+        datatype.split(':')[1]
+
+    attributes = []
+
+    for complex_type in root.xpath(ct_xpath, namespaces=root.nsmap):
+        for child in complex_type.iterchildren():
+            attributes.extend(_iterchildren(child, datatype))
+
+    return attributes
+
+
+def datatypes(root):
+    nsmap = get_nsmap(root)
+
+    return [element.get('type')
+            for element in root.xpath('/xs:schema/xs:element',
+                                      namespaces=nsmap)]
+                                      
+
+def get_nsmap(node):
+    nsmap = node.nsmap
+    none_ns = node.nsmap.get(None)
+
+    if none_ns is None:
+        nsmap[none_ns.rsplit('/', 1)[1]] = none_ns
+        del nsmap[None]
+
+    return nsmap
+
+
+def class_name(self):
+    """
+    Return the name of this class without qualification.
+    eg. If the class name is "x.y.class" return only "class"
+    """
+    return self.__class__.__name__.split('.')[-1]
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/search.py` & `bbrc-pyxnat-1.6/pyxnat/core/search.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,741 +1,741 @@
-import csv
-import difflib
-try:
-    from StringIO import StringIO
-except ImportError:
-    from io import StringIO
-try:
-    unicode
-    import sys
-    reload(sys)  # Reload does the trick!
-    sys.setdefaultencoding('UTF8')
-except NameError:
-    unicode = str
-from six import string_types
-
-from lxml import etree
-
-from .jsonutil import JsonTable, get_column, get_where, get_selection
-from .errors import is_xnat_error, catch_error
-from .errors import ProgrammingError, NotSupportedError
-from .errors import DataError, DatabaseError
-
-search_nsmap = {'xdat': 'http://nrg.wustl.edu/security',
-                'xsi': 'http://www.w3.org/2001/XMLSchema-instance'}
-
-special_ops = {'*': '%', }
-
-
-def build_search_document(root_element_name, columns, criteria_set,
-                          brief_description='', long_description='',
-                          allowed_users=[]):
-    root_node = \
-        etree.Element(etree.QName(search_nsmap['xdat'], 'bundle'),
-                      nsmap=search_nsmap
-                      )
-
-    root_node.set('ID', "@%s" % root_element_name)
-    root_node.set('brief-description', brief_description)
-    root_node.set('description', long_description)
-    root_node.set('allow-diff-columns', "0")
-    root_node.set('secure', "false")
-
-    root_element_name_node = \
-        etree.Element(etree.QName(search_nsmap['xdat'], 'root_element_name'),
-                      nsmap=search_nsmap
-                      )
-
-    root_element_name_node.text = root_element_name
-
-    root_node.append(root_element_name_node)
-
-    for i, column in enumerate(columns):
-        element_name, field_ID = column.split('/', 1)
-
-        search_field_node = \
-            etree.Element(etree.QName(search_nsmap['xdat'], 'search_field'),
-                          nsmap=search_nsmap
-                          )
-
-        element_name_node = \
-            etree.Element(etree.QName(search_nsmap['xdat'], 'element_name'),
-                          nsmap=search_nsmap
-                          )
-
-        element_name_node.text = element_name
-
-        field_ID_node = \
-            etree.Element(etree.QName(search_nsmap['xdat'], 'field_ID'),
-                          nsmap=search_nsmap
-                          )
-
-        field_ID_node.text = field_ID
-
-        sequence_node = \
-            etree.Element(etree.QName(search_nsmap['xdat'], 'sequence'),
-                          nsmap=search_nsmap
-                          )
-
-        sequence_node.text = str(i)
-
-        type_node = \
-            etree.Element(etree.QName(search_nsmap['xdat'], 'type'),
-                          nsmap=search_nsmap
-                          )
-
-        type_node.text = 'string'
-
-        header_node = \
-            etree.Element(etree.QName(search_nsmap['xdat'], 'header'),
-                          nsmap=search_nsmap
-                          )
-
-        header_node.text = column
-
-        search_field_node.extend([element_name_node,
-                                  field_ID_node,
-                                  sequence_node,
-                                  type_node, header_node
-                                  ])
-
-        root_node.append(search_field_node)
-
-    search_where_node = \
-        etree.Element(etree.QName(search_nsmap['xdat'], 'search_where'),
-                      nsmap=search_nsmap
-                      )
-
-    root_node.append(build_criteria_set(search_where_node, criteria_set))
-
-    if allowed_users != []:
-
-        allowed_users_node = \
-            etree.Element(etree.QName(search_nsmap['xdat'], 'allowed_user'),
-                          nsmap=search_nsmap
-                          )
-
-        for allowed_user in allowed_users:
-            login_node = \
-                etree.Element(etree.QName(search_nsmap['xdat'], 'login'),
-                              nsmap=search_nsmap
-                              )
-            login_node.text = allowed_user
-            allowed_users_node.append(login_node)
-
-        root_node.append(allowed_users_node)
-
-    return etree.tostring(root_node.getroottree())
-
-
-def build_criteria_set(container_node, criteria_set):
-
-    for criteria in criteria_set:
-        if isinstance(criteria, string_types):
-            container_node.set('method', criteria)
-
-        if isinstance(criteria, (list)):
-            sub_container_node = \
-                etree.Element(etree.QName(search_nsmap['xdat'], 'child_set'),
-                              nsmap=search_nsmap
-                              )
-
-            container_node.append(
-                build_criteria_set(sub_container_node, criteria))
-
-        if isinstance(criteria, (tuple)):
-            if len(criteria) != 3:
-                raise ProgrammingError('%s should be a 3-element tuple' %
-                                       str(criteria))
-
-            constraint_node = \
-                etree.Element(etree.QName(search_nsmap['xdat'], 'criteria'),
-                              nsmap=search_nsmap
-                              )
-
-            constraint_node.set('override_value_formatting', '0')
-
-            schema_field_node = \
-                etree.Element(etree.QName(search_nsmap['xdat'],
-                                          'schema_field'
-                                          ),
-                              nsmap=search_nsmap
-                              )
-
-            schema_field_node.text = criteria[0]
-
-            comparison_type_node = \
-                etree.Element(etree.QName(search_nsmap['xdat'],
-                                          'comparison_type'
-                                          ),
-                              nsmap=search_nsmap
-                              )
-
-            comparison_type_node.text = special_ops.get(criteria[1],
-                                                        criteria[1]
-                                                        )
-
-            value_node = \
-                etree.Element(etree.QName(search_nsmap['xdat'], 'value'),
-                              nsmap=search_nsmap
-                              )
-
-            value_node.text = criteria[2].replace('*', special_ops['*'])
-
-            constraint_node.extend([
-                    schema_field_node, comparison_type_node, value_node])
-
-            container_node.append(constraint_node)
-
-    return container_node
-
-
-def query_from_xml(document):
-    query = {}
-    root = etree.fromstring(document)
-    _nsmap = root.nsmap
-
-    query['description'] = root.get('description', default="")
-
-    query['row'] = root.xpath('xdat:root_element_name',
-                              namespaces=root.nsmap)[0].text
-
-    query['columns'] = []
-
-    for node in root.xpath('xdat:search_field',
-                           namespaces=_nsmap):
-
-        en = node.xpath('xdat:element_name', namespaces=root.nsmap)[0].text
-        fid = node.xpath('xdat:field_ID', namespaces=root.nsmap)[0].text
-
-        query['columns'].append('%s/%s' % (en, fid))
-
-    query['users'] = [
-        node.text
-        for node in root.xpath('xdat:allowed_user/xdat:login',
-                               namespaces=root.nsmap
-                               )
-        ]
-
-    try:
-        search_where = root.xpath('xdat:search_where',
-                                  namespaces=root.nsmap)[0]
-
-        query['constraints'] = query_from_criteria_set(search_where)
-    except Exception:
-        query['constraints'] = [('%s/ID' % query['row'], 'LIKE', '%'), 'AND']
-
-    return query
-
-
-def query_from_criteria_set(criteria_set):
-    query = []
-    query.append(criteria_set.get('method'))
-    _nsmap = criteria_set.nsmap
-
-    for criteria in criteria_set.xpath('xdat:criteria',
-                                       namespaces=_nsmap):
-
-        _f = criteria.xpath('xdat:schema_field', namespaces=_nsmap)[0]
-        _o = criteria.xpath('xdat:comparison_type', namespaces=_nsmap)[0]
-        _v = criteria.xpath('xdat:value', namespaces=_nsmap)[0]
-
-        constraint = (_f.text, _o.text, _v.text)
-        query.insert(0, constraint)
-
-    for child_set in criteria_set.xpath('xdat:child_set',
-                                        namespaces=_nsmap):
-
-        query.insert(0, query_from_criteria_set(child_set))
-
-    return query
-
-
-def rpn_contraints(rpn_exp):
-    left = []
-    right = []
-    triple = []
-
-    for i, t in enumerate(rpn_exp.split()):
-        if t in ['AND', 'OR']:
-            if 'AND' in right or 'OR' in right and left == []:
-                try:
-                    operator = right.pop(right.index('AND'))
-                except Exception:
-                    operator = right.pop(right.index('OR'))
-
-                left = [right[0]]
-                left.append(right[1:] + [t])
-                left.append(operator)
-
-                right = []
-
-            elif right != []:
-                right.append(t)
-
-                if left != []:
-                    left.append(right)
-                else:
-                    left = right[:]
-                    right = []
-
-            elif right == [] and left != []:
-                left = [left]
-                left.append(t)
-                right = left[:]
-                left = []
-            else:
-                raise ProgrammingError('in expression %s' % rpn_exp)
-
-        else:
-            triple.append(t)
-            if len(triple) == 3:
-                right.append(tuple(triple))
-                triple = []
-
-    return left if left != [] else right
-
-# ---------------------------------------------------------------
-
-
-class SearchManager(object):
-    """ Search interface.
-        Handles operations to save and get back searches on the server.
-
-        Examples
-        --------
-            >>> row = 'xnat:subjectData'
-            >>> columns = ['xnat:subjectData/PROJECT',
-                           'xnat:subjectData/SUBJECT_ID'
-                           ]
-            >>> criteria = [('xnat:subjectData/SUBJECT_ID', 'LIKE', '*'),
-                            'AND'
-                            ]
-            >>> interface.manage.search.save('mysearch', row, columns,
-                                             criteria, sharing='public',
-                                             description='my first search'
-                                             )
-    """
-    def __init__(self, interface):
-        self._intf = interface
-
-    def _save_search(self, row, columns, constraints, name, desc, sharing):
-        self._intf._get_entry_point()
-
-        name = name.replace(' ', '_')
-        if sharing == 'private':
-            users = [self._intf._user]
-        elif sharing == 'public':
-            users = []
-        elif isinstance(sharing, list):
-            users = sharing
-        else:
-            raise NotSupportedError('Share mode %s not valid' % sharing)
-
-        self._intf._exec(
-            '%s/search/saved/%s?inbody=true' % (self._intf._entry, name),
-            method='PUT',
-            body=build_search_document(row, columns,
-                                       constraints,
-                                       name, desc.replace('%', '%%'),
-                                       users
-                                       )
-            )
-
-    def save(self, name, row, columns, constraints,
-             sharing='private', description=''):
-        """ Saves a query on the XNAT server.
-
-            Parameters
-            ----------
-            name: string
-                Name of the query displayed on the Web Interface and
-                used to get back the results.
-            row: string
-                Datatype from `Interface.inspect.datatypes()`.
-                Usually ``xnat:subjectData``
-            columns: list
-                List of data fields from
-                `Interface.inspect.datatypes('*', '*')`
-            constraints: list
-                See also: `Search.where()`
-            sharing: string | list
-                Define by whom the query is visible.
-                If sharing is a string it may be either
-                ``private`` or ``public``.
-                Otherwise a list of valid logins for the XNAT server
-                from `Interface.users()`.
-
-            See Also
-            --------
-            :func:`Search.where`
-        """
-        self._save_search(row, columns, constraints,
-                          name, description, sharing)
-
-    def saved(self, with_description=False):
-        """ Returns the names of accessible saved search on the server.
-        """
-        self._intf._get_entry_point()
-
-        jdata = self._intf._get_json(
-            '%s/search/saved?format=json' % self._intf._entry)
-
-        if with_description:
-            return [(ld['brief_description'],
-                     ld['description'].replace('%%', '%'))
-                    for ld in get_selection(jdata, ['brief_description',
-                                                    'description'
-                                                    ]
-                                            )
-                    if not ld['brief_description'].startswith('template_')]
-        else:
-            return [name
-                    for name in get_column(jdata, 'brief_description')
-                    if not name.startswith('template_')]
-
-    def get(self, name, out_format='results'):
-        """ Returns the results of the query saved on the XNAT server or
-            the query itself to know what it does.
-
-            Parameters
-            ----------
-            name: string
-                Name of the saved search. An exception is raised if the name
-                does not exist.
-            out_format: string
-                Can take the following values:
-                    - results to download the results of the search
-                    - xml to download the XML document defining the search
-                    - query to get the pyxnat representation of the search
-        """
-        self._intf._get_entry_point()
-
-        jdata = self._intf._get_json(
-            '%s/search/saved?format=json' % self._intf._entry)
-
-        try:
-            search_id = get_where(jdata, brief_description=name)[0]['id']
-        except IndexError:
-            raise DatabaseError('%s not found' % name)
-
-        if out_format in ['xml', 'query']:
-            bundle = self._intf._exec(
-                '%s/search/saved/%s' % (self._intf._entry,
-                                        search_id
-                                        ), 'GET')
-
-            if out_format == 'xml':
-                return bundle
-            else:
-                return query_from_xml(bundle)
-
-        content = self._intf._exec(
-            '%s/search/saved/%s/results?format=csv' % (self._intf._entry,
-                                                       search_id), 'GET')
-
-        results = csv.reader(StringIO(content.decode('utf-8')), delimiter=',',
-                             quotechar='"')
-
-        headers = next(results)
-
-        return JsonTable([dict(zip(headers, res))
-                          for res in results
-                          ],
-                         headers
-                         )
-
-    def delete(self, name):
-        """ Removes the search from the server.
-        """
-        self._intf._get_entry_point()
-
-        jdata = self._intf._get_json(
-            '%s/search/saved?format=json' % self._intf._entry)
-
-        try:
-            search_id = get_where(jdata, brief_description=name)[0]['id']
-        except IndexError:
-            raise DatabaseError('%s not found' % name)
-
-        self._intf._exec('%s/search/saved/%s' % (self._intf._entry,
-                                                 search_id
-                                                 ), 'DELETE')
-
-    def save_template(self, name, row=None, columns=[],
-                      constraints=[], sharing='private', description=''):
-        """
-            Define and save a search template. Same as the save method, but
-            the values in the constraints are used as keywords for value
-            replacement when using the template.
-
-            Parameters
-            ----------
-            name: string
-                Name under which the template is save in XNAT. A template is
-                prepended to the name so that it appear clearly as a template
-                on the web interface.
-            row: string
-                Datatype from `Interface.inspect.datatypes()`.
-                Usually ``xnat:subjectData``
-            columns: list
-                List of data fields from
-                `Interface.inspect.datatypes('*', '*')`
-            constraints: list
-                See also: `Search.where()`, values are keywords for the
-                template
-            sharing: string | list
-                Define by whom the query is visible.
-                If sharing is a string it may be either
-                ``private`` or ``public``.
-                Otherwise a list of valid logins for the XNAT server
-                from `Interface.users()`.
-        """
-
-        def _make_template(query):
-            query_template = []
-
-            for constraint in query:
-                if isinstance(constraint, tuple):
-                    query_template.append((constraint[0],
-                                           constraint[1],
-                                           '%%(%s)s' % constraint[2])
-                                          )
-                elif isinstance(constraint, (unicode, str)):
-                    query_template.append(constraint)
-                elif isinstance(constraint, list):
-                    query_template.append(_make_template(constraint))
-                else:
-                    raise ProgrammingError('Unrecognized token '
-                                           'in query: %s' % constraint
-                                           )
-
-            return query_template
-
-        self._save_search(
-            row, columns, _make_template(constraints),
-            'template_%s' % name, description, sharing
-            )
-
-    def saved_templates(self, with_description=False):
-        """ Returns the names of accessible saved search templates on the server.
-        """
-        self._intf._get_entry_point()
-
-        jdata = self._intf._get_json(
-            '%s/search/saved?format=json' % self._intf._entry)
-
-        if with_description:
-            return [
-                (ld['brief_description'].split('template_')[1],
-                 ld['description'].replace('%%', '%')
-                 )
-                for ld in get_selection(jdata, ['brief_description',
-                                                'description'
-                                                ]
-                                        )
-                if ld['brief_description'].startswith('template_')
-                ]
-        else:
-            return [name.split('template_')[1]
-                    for name in get_column(jdata, 'brief_description')
-                    if name.startswith('template_')]
-
-    def use_template(self, name, values):
-        """
-            Performs a search query using a previously saved template.
-
-            Parameters
-            ----------
-            name: string
-                Name of the template.
-            values: dict
-                Values to put in the template, get the valid keys using
-                the get_template method.
-
-            Examples
-            --------
-            >>> interface.manage.search.use_template(name,
-                          {'subject_id':'ID',
-                           'age':'32'
-                           })
-
-        """
-        self._intf._get_entry_point()
-
-        bundle = self.get_template(name, True) % values
-
-        # have to remove search_id information before re-posting it
-        _query = query_from_xml(bundle)
-        bundle = build_search_document(_query['row'],
-                                       _query['columns'],
-                                       _query['constraints']
-                                       )
-
-        content = self._intf._exec(
-            "%s/search?format=csv" % self._intf._entry, 'POST', bundle)
-
-        results = csv.reader(StringIO(content), delimiter=',', quotechar='"')
-        headers = results.next()
-
-        return JsonTable([dict(zip(headers, res))
-                          for res in results
-                          ],
-                         headers
-                         )
-
-    def get_template(self, name, as_xml=False):
-        """ Get a saved template, either as an xml document, or as a pyxnat
-            representation, with the keys to be used in the template
-            between the parentheses in %()s.
-
-            Parameters
-            ----------
-            name: str
-                Name under which the template is saved
-            as_xml: boolean
-                If True returns an XML document, else return a list of
-                constraints. Defaults to False.
-        """
-        self._intf._get_entry_point()
-
-        jdata = self._intf._get_json(
-            '%s/search/saved?format=json' % self._intf._entry)
-
-        try:
-            search_id = get_where(jdata,
-                                  brief_description='template_%s' % name
-                                  )[0]['id']
-        except IndexError:
-            raise DatabaseError('%s not found' % name)
-
-        bundle = self._intf._exec(
-            '%s/search/saved/%s' % (self._intf._entry,
-                                    search_id
-                                    ), 'GET')
-
-        if as_xml:
-            return bundle
-        else:
-            _query = query_from_xml(bundle)
-            return (_query['row'], _query['columns'], _query['constraints'],
-                    _query['description'])
-
-    def delete_template(self, name):
-        """ Deletes a search template.
-        """
-        self.delete('template_%s' % name)
-
-    def eval_rpn_exp(self, rpnexp):
-        return rpn_contraints(rpnexp)
-
-
-class Search(object):
-    """ Define constraints to make a complex search on the database.
-
-        This :class:`Search` is available at different places throughout
-        the API:
-
-            >>> interface.select(DATA_SELECTION).where(QUERY)
-            >>> interface.manage.search.save('name', TABLE_DEFINITION, QUERY)
-
-        Examples
-        --------
-            >>> query = [('xnat:subjectData/SUBJECT_ID', 'LIKE', '%'),
-                         ('xnat:projectData/ID', '=', 'my_project'),
-                         [('xnat:subjectData/AGE', '>', '14'),
-                           'AND'
-                          ],
-                         'OR'
-                        ]
-    """
-    def __init__(self, row, columns, interface):
-        """ Configure the result table.
-
-            Parameters
-            ----------
-            row: string
-                The returned table will have one line for every matching
-                occurence of this type.
-                e.g. xnat:subjectData
-                --> table with one line per matching subject
-            columns: list
-                The returned table will have all the given columns.
-        """
-        self._row = row
-        self._columns = columns
-        self._intf = interface
-
-    def where(self, constraints=None, template=None, query=None):
-        """ Triggers the search.
-
-            Parameters
-            ----------
-            contraints: list
-                A query is an unordered list that contains
-                    - 1 or more constraints
-                    - 0 or more sub-queries (lists as this one)
-                    - 1 comparison method between the constraints
-                        ('AND' or 'OR')
-                A constraint is an ordered tuple that contains
-                    - 1 valid searchable_type/searchable_field
-                    - 1 operator among '=', '<', '>', '<=', '>=', 'LIKE'
-
-            Returns
-            -------
-            results: JsonTable object
-                An table-like object containing the results. It is
-                basically a list of dictionaries that has additional
-                helper methods.
-        """
-        self._intf._get_entry_point()
-
-        if isinstance(constraints, (str, unicode)):
-            constraints = rpn_contraints(constraints)
-        elif isinstance(template, (tuple)):
-            tmp_bundle = self._intf.manage.search.get_template(
-                template[0], True)
-
-            tmp_bundle = tmp_bundle % template[1]
-            constraints = query_from_xml(tmp_bundle)['constraints']
-        elif isinstance(query, (str, unicode)):
-            tmp_bundle = self._intf.manage.search.get(query, 'xml')
-            constraints = query_from_xml(tmp_bundle)['constraints']
-        elif isinstance(constraints, list):
-            pass
-        else:
-            raise ProgrammingError('One of contraints, template and query'
-                                   'parameters must be correctly set.')
-
-        bundle = build_search_document(self._row, self._columns, constraints)
-
-        content = self._intf._exec(
-            "%s/search?format=csv" % self._intf._entry, 'POST', bundle)
-
-        if is_xnat_error(content):
-            catch_error(content)
-
-        results = csv.reader(StringIO(content.decode('utf-8')), delimiter=',',
-                             quotechar='"')
-        headers = next(results)
-
-        headers_of_interest = []
-
-        for column in self._columns:
-            try:
-                headers_of_interest.append(
-                    difflib.get_close_matches(
-                        column.split(self._row + '/')[0].lower()
-                        or column.split(self._row + '/')[1].lower(),
-                        headers)[0]
-                    )
-            except IndexError:
-                headers_of_interest.append('unknown')
-
-        if len(self._columns) != len(headers_of_interest):
-            raise DataError('unvalid response headers')
-
-        return JsonTable([dict(zip(headers, res)) for res in results],
-                         headers_of_interest).select(headers_of_interest)
-
-    def all(self):
-        return self.where([(self._row + '/ID', 'LIKE', '%'), 'AND'])
+import csv
+import difflib
+try:
+    from StringIO import StringIO
+except ImportError:
+    from io import StringIO
+try:
+    unicode
+    import sys
+    reload(sys)  # Reload does the trick!
+    sys.setdefaultencoding('UTF8')
+except NameError:
+    unicode = str
+from six import string_types
+
+from lxml import etree
+
+from .jsonutil import JsonTable, get_column, get_where, get_selection
+from .errors import is_xnat_error, catch_error
+from .errors import ProgrammingError, NotSupportedError
+from .errors import DataError, DatabaseError
+
+search_nsmap = {'xdat': 'http://nrg.wustl.edu/security',
+                'xsi': 'http://www.w3.org/2001/XMLSchema-instance'}
+
+special_ops = {'*': '%', }
+
+
+def build_search_document(root_element_name, columns, criteria_set,
+                          brief_description='', long_description='',
+                          allowed_users=[]):
+    root_node = \
+        etree.Element(etree.QName(search_nsmap['xdat'], 'bundle'),
+                      nsmap=search_nsmap
+                      )
+
+    root_node.set('ID', "@%s" % root_element_name)
+    root_node.set('brief-description', brief_description)
+    root_node.set('description', long_description)
+    root_node.set('allow-diff-columns', "0")
+    root_node.set('secure', "false")
+
+    root_element_name_node = \
+        etree.Element(etree.QName(search_nsmap['xdat'], 'root_element_name'),
+                      nsmap=search_nsmap
+                      )
+
+    root_element_name_node.text = root_element_name
+
+    root_node.append(root_element_name_node)
+
+    for i, column in enumerate(columns):
+        element_name, field_ID = column.split('/', 1)
+
+        search_field_node = \
+            etree.Element(etree.QName(search_nsmap['xdat'], 'search_field'),
+                          nsmap=search_nsmap
+                          )
+
+        element_name_node = \
+            etree.Element(etree.QName(search_nsmap['xdat'], 'element_name'),
+                          nsmap=search_nsmap
+                          )
+
+        element_name_node.text = element_name
+
+        field_ID_node = \
+            etree.Element(etree.QName(search_nsmap['xdat'], 'field_ID'),
+                          nsmap=search_nsmap
+                          )
+
+        field_ID_node.text = field_ID
+
+        sequence_node = \
+            etree.Element(etree.QName(search_nsmap['xdat'], 'sequence'),
+                          nsmap=search_nsmap
+                          )
+
+        sequence_node.text = str(i)
+
+        type_node = \
+            etree.Element(etree.QName(search_nsmap['xdat'], 'type'),
+                          nsmap=search_nsmap
+                          )
+
+        type_node.text = 'string'
+
+        header_node = \
+            etree.Element(etree.QName(search_nsmap['xdat'], 'header'),
+                          nsmap=search_nsmap
+                          )
+
+        header_node.text = column
+
+        search_field_node.extend([element_name_node,
+                                  field_ID_node,
+                                  sequence_node,
+                                  type_node, header_node
+                                  ])
+
+        root_node.append(search_field_node)
+
+    search_where_node = \
+        etree.Element(etree.QName(search_nsmap['xdat'], 'search_where'),
+                      nsmap=search_nsmap
+                      )
+
+    root_node.append(build_criteria_set(search_where_node, criteria_set))
+
+    if allowed_users != []:
+
+        allowed_users_node = \
+            etree.Element(etree.QName(search_nsmap['xdat'], 'allowed_user'),
+                          nsmap=search_nsmap
+                          )
+
+        for allowed_user in allowed_users:
+            login_node = \
+                etree.Element(etree.QName(search_nsmap['xdat'], 'login'),
+                              nsmap=search_nsmap
+                              )
+            login_node.text = allowed_user
+            allowed_users_node.append(login_node)
+
+        root_node.append(allowed_users_node)
+
+    return etree.tostring(root_node.getroottree())
+
+
+def build_criteria_set(container_node, criteria_set):
+
+    for criteria in criteria_set:
+        if isinstance(criteria, string_types):
+            container_node.set('method', criteria)
+
+        if isinstance(criteria, (list)):
+            sub_container_node = \
+                etree.Element(etree.QName(search_nsmap['xdat'], 'child_set'),
+                              nsmap=search_nsmap
+                              )
+
+            container_node.append(
+                build_criteria_set(sub_container_node, criteria))
+
+        if isinstance(criteria, (tuple)):
+            if len(criteria) != 3:
+                raise ProgrammingError('%s should be a 3-element tuple' %
+                                       str(criteria))
+
+            constraint_node = \
+                etree.Element(etree.QName(search_nsmap['xdat'], 'criteria'),
+                              nsmap=search_nsmap
+                              )
+
+            constraint_node.set('override_value_formatting', '0')
+
+            schema_field_node = \
+                etree.Element(etree.QName(search_nsmap['xdat'],
+                                          'schema_field'
+                                          ),
+                              nsmap=search_nsmap
+                              )
+
+            schema_field_node.text = criteria[0]
+
+            comparison_type_node = \
+                etree.Element(etree.QName(search_nsmap['xdat'],
+                                          'comparison_type'
+                                          ),
+                              nsmap=search_nsmap
+                              )
+
+            comparison_type_node.text = special_ops.get(criteria[1],
+                                                        criteria[1]
+                                                        )
+
+            value_node = \
+                etree.Element(etree.QName(search_nsmap['xdat'], 'value'),
+                              nsmap=search_nsmap
+                              )
+
+            value_node.text = criteria[2].replace('*', special_ops['*'])
+
+            constraint_node.extend([
+                    schema_field_node, comparison_type_node, value_node])
+
+            container_node.append(constraint_node)
+
+    return container_node
+
+
+def query_from_xml(document):
+    query = {}
+    root = etree.fromstring(document)
+    _nsmap = root.nsmap
+
+    query['description'] = root.get('description', default="")
+
+    query['row'] = root.xpath('xdat:root_element_name',
+                              namespaces=root.nsmap)[0].text
+
+    query['columns'] = []
+
+    for node in root.xpath('xdat:search_field',
+                           namespaces=_nsmap):
+
+        en = node.xpath('xdat:element_name', namespaces=root.nsmap)[0].text
+        fid = node.xpath('xdat:field_ID', namespaces=root.nsmap)[0].text
+
+        query['columns'].append('%s/%s' % (en, fid))
+
+    query['users'] = [
+        node.text
+        for node in root.xpath('xdat:allowed_user/xdat:login',
+                               namespaces=root.nsmap
+                               )
+        ]
+
+    try:
+        search_where = root.xpath('xdat:search_where',
+                                  namespaces=root.nsmap)[0]
+
+        query['constraints'] = query_from_criteria_set(search_where)
+    except Exception:
+        query['constraints'] = [('%s/ID' % query['row'], 'LIKE', '%'), 'AND']
+
+    return query
+
+
+def query_from_criteria_set(criteria_set):
+    query = []
+    query.append(criteria_set.get('method'))
+    _nsmap = criteria_set.nsmap
+
+    for criteria in criteria_set.xpath('xdat:criteria',
+                                       namespaces=_nsmap):
+
+        _f = criteria.xpath('xdat:schema_field', namespaces=_nsmap)[0]
+        _o = criteria.xpath('xdat:comparison_type', namespaces=_nsmap)[0]
+        _v = criteria.xpath('xdat:value', namespaces=_nsmap)[0]
+
+        constraint = (_f.text, _o.text, _v.text)
+        query.insert(0, constraint)
+
+    for child_set in criteria_set.xpath('xdat:child_set',
+                                        namespaces=_nsmap):
+
+        query.insert(0, query_from_criteria_set(child_set))
+
+    return query
+
+
+def rpn_contraints(rpn_exp):
+    left = []
+    right = []
+    triple = []
+
+    for i, t in enumerate(rpn_exp.split()):
+        if t in ['AND', 'OR']:
+            if 'AND' in right or 'OR' in right and left == []:
+                try:
+                    operator = right.pop(right.index('AND'))
+                except Exception:
+                    operator = right.pop(right.index('OR'))
+
+                left = [right[0]]
+                left.append(right[1:] + [t])
+                left.append(operator)
+
+                right = []
+
+            elif right != []:
+                right.append(t)
+
+                if left != []:
+                    left.append(right)
+                else:
+                    left = right[:]
+                    right = []
+
+            elif right == [] and left != []:
+                left = [left]
+                left.append(t)
+                right = left[:]
+                left = []
+            else:
+                raise ProgrammingError('in expression %s' % rpn_exp)
+
+        else:
+            triple.append(t)
+            if len(triple) == 3:
+                right.append(tuple(triple))
+                triple = []
+
+    return left if left != [] else right
+
+# ---------------------------------------------------------------
+
+
+class SearchManager(object):
+    """ Search interface.
+        Handles operations to save and get back searches on the server.
+
+        Examples
+        --------
+            >>> row = 'xnat:subjectData'
+            >>> columns = ['xnat:subjectData/PROJECT',
+                           'xnat:subjectData/SUBJECT_ID'
+                           ]
+            >>> criteria = [('xnat:subjectData/SUBJECT_ID', 'LIKE', '*'),
+                            'AND'
+                            ]
+            >>> interface.manage.search.save('mysearch', row, columns,
+                                             criteria, sharing='public',
+                                             description='my first search'
+                                             )
+    """
+    def __init__(self, interface):
+        self._intf = interface
+
+    def _save_search(self, row, columns, constraints, name, desc, sharing):
+        self._intf._get_entry_point()
+
+        name = name.replace(' ', '_')
+        if sharing == 'private':
+            users = [self._intf._user]
+        elif sharing == 'public':
+            users = []
+        elif isinstance(sharing, list):
+            users = sharing
+        else:
+            raise NotSupportedError('Share mode %s not valid' % sharing)
+
+        self._intf._exec(
+            '%s/search/saved/%s?inbody=true' % (self._intf._entry, name),
+            method='PUT',
+            body=build_search_document(row, columns,
+                                       constraints,
+                                       name, desc.replace('%', '%%'),
+                                       users
+                                       )
+            )
+
+    def save(self, name, row, columns, constraints,
+             sharing='private', description=''):
+        """ Saves a query on the XNAT server.
+
+            Parameters
+            ----------
+            name: string
+                Name of the query displayed on the Web Interface and
+                used to get back the results.
+            row: string
+                Datatype from `Interface.inspect.datatypes()`.
+                Usually ``xnat:subjectData``
+            columns: list
+                List of data fields from
+                `Interface.inspect.datatypes('*', '*')`
+            constraints: list
+                See also: `Search.where()`
+            sharing: string | list
+                Define by whom the query is visible.
+                If sharing is a string it may be either
+                ``private`` or ``public``.
+                Otherwise a list of valid logins for the XNAT server
+                from `Interface.users()`.
+
+            See Also
+            --------
+            :func:`Search.where`
+        """
+        self._save_search(row, columns, constraints,
+                          name, description, sharing)
+
+    def saved(self, with_description=False):
+        """ Returns the names of accessible saved search on the server.
+        """
+        self._intf._get_entry_point()
+
+        jdata = self._intf._get_json(
+            '%s/search/saved?format=json' % self._intf._entry)
+
+        if with_description:
+            return [(ld['brief_description'],
+                     ld['description'].replace('%%', '%'))
+                    for ld in get_selection(jdata, ['brief_description',
+                                                    'description'
+                                                    ]
+                                            )
+                    if not ld['brief_description'].startswith('template_')]
+        else:
+            return [name
+                    for name in get_column(jdata, 'brief_description')
+                    if not name.startswith('template_')]
+
+    def get(self, name, out_format='results'):
+        """ Returns the results of the query saved on the XNAT server or
+            the query itself to know what it does.
+
+            Parameters
+            ----------
+            name: string
+                Name of the saved search. An exception is raised if the name
+                does not exist.
+            out_format: string
+                Can take the following values:
+                    - results to download the results of the search
+                    - xml to download the XML document defining the search
+                    - query to get the pyxnat representation of the search
+        """
+        self._intf._get_entry_point()
+
+        jdata = self._intf._get_json(
+            '%s/search/saved?format=json' % self._intf._entry)
+
+        try:
+            search_id = get_where(jdata, brief_description=name)[0]['id']
+        except IndexError:
+            raise DatabaseError('%s not found' % name)
+
+        if out_format in ['xml', 'query']:
+            bundle = self._intf._exec(
+                '%s/search/saved/%s' % (self._intf._entry,
+                                        search_id
+                                        ), 'GET')
+
+            if out_format == 'xml':
+                return bundle
+            else:
+                return query_from_xml(bundle)
+
+        content = self._intf._exec(
+            '%s/search/saved/%s/results?format=csv' % (self._intf._entry,
+                                                       search_id), 'GET')
+
+        results = csv.reader(StringIO(content.decode('utf-8')), delimiter=',',
+                             quotechar='"')
+
+        headers = next(results)
+
+        return JsonTable([dict(zip(headers, res))
+                          for res in results
+                          ],
+                         headers
+                         )
+
+    def delete(self, name):
+        """ Removes the search from the server.
+        """
+        self._intf._get_entry_point()
+
+        jdata = self._intf._get_json(
+            '%s/search/saved?format=json' % self._intf._entry)
+
+        try:
+            search_id = get_where(jdata, brief_description=name)[0]['id']
+        except IndexError:
+            raise DatabaseError('%s not found' % name)
+
+        self._intf._exec('%s/search/saved/%s' % (self._intf._entry,
+                                                 search_id
+                                                 ), 'DELETE')
+
+    def save_template(self, name, row=None, columns=[],
+                      constraints=[], sharing='private', description=''):
+        """
+            Define and save a search template. Same as the save method, but
+            the values in the constraints are used as keywords for value
+            replacement when using the template.
+
+            Parameters
+            ----------
+            name: string
+                Name under which the template is save in XNAT. A template is
+                prepended to the name so that it appear clearly as a template
+                on the web interface.
+            row: string
+                Datatype from `Interface.inspect.datatypes()`.
+                Usually ``xnat:subjectData``
+            columns: list
+                List of data fields from
+                `Interface.inspect.datatypes('*', '*')`
+            constraints: list
+                See also: `Search.where()`, values are keywords for the
+                template
+            sharing: string | list
+                Define by whom the query is visible.
+                If sharing is a string it may be either
+                ``private`` or ``public``.
+                Otherwise a list of valid logins for the XNAT server
+                from `Interface.users()`.
+        """
+
+        def _make_template(query):
+            query_template = []
+
+            for constraint in query:
+                if isinstance(constraint, tuple):
+                    query_template.append((constraint[0],
+                                           constraint[1],
+                                           '%%(%s)s' % constraint[2])
+                                          )
+                elif isinstance(constraint, (unicode, str)):
+                    query_template.append(constraint)
+                elif isinstance(constraint, list):
+                    query_template.append(_make_template(constraint))
+                else:
+                    raise ProgrammingError('Unrecognized token '
+                                           'in query: %s' % constraint
+                                           )
+
+            return query_template
+
+        self._save_search(
+            row, columns, _make_template(constraints),
+            'template_%s' % name, description, sharing
+            )
+
+    def saved_templates(self, with_description=False):
+        """ Returns the names of accessible saved search templates on the server.
+        """
+        self._intf._get_entry_point()
+
+        jdata = self._intf._get_json(
+            '%s/search/saved?format=json' % self._intf._entry)
+
+        if with_description:
+            return [
+                (ld['brief_description'].split('template_')[1],
+                 ld['description'].replace('%%', '%')
+                 )
+                for ld in get_selection(jdata, ['brief_description',
+                                                'description'
+                                                ]
+                                        )
+                if ld['brief_description'].startswith('template_')
+                ]
+        else:
+            return [name.split('template_')[1]
+                    for name in get_column(jdata, 'brief_description')
+                    if name.startswith('template_')]
+
+    def use_template(self, name, values):
+        """
+            Performs a search query using a previously saved template.
+
+            Parameters
+            ----------
+            name: string
+                Name of the template.
+            values: dict
+                Values to put in the template, get the valid keys using
+                the get_template method.
+
+            Examples
+            --------
+            >>> interface.manage.search.use_template(name,
+                          {'subject_id':'ID',
+                           'age':'32'
+                           })
+
+        """
+        self._intf._get_entry_point()
+
+        bundle = self.get_template(name, True) % values
+
+        # have to remove search_id information before re-posting it
+        _query = query_from_xml(bundle)
+        bundle = build_search_document(_query['row'],
+                                       _query['columns'],
+                                       _query['constraints']
+                                       )
+
+        content = self._intf._exec(
+            "%s/search?format=csv" % self._intf._entry, 'POST', bundle)
+
+        results = csv.reader(StringIO(content), delimiter=',', quotechar='"')
+        headers = results.next()
+
+        return JsonTable([dict(zip(headers, res))
+                          for res in results
+                          ],
+                         headers
+                         )
+
+    def get_template(self, name, as_xml=False):
+        """ Get a saved template, either as an xml document, or as a pyxnat
+            representation, with the keys to be used in the template
+            between the parentheses in %()s.
+
+            Parameters
+            ----------
+            name: str
+                Name under which the template is saved
+            as_xml: boolean
+                If True returns an XML document, else return a list of
+                constraints. Defaults to False.
+        """
+        self._intf._get_entry_point()
+
+        jdata = self._intf._get_json(
+            '%s/search/saved?format=json' % self._intf._entry)
+
+        try:
+            search_id = get_where(jdata,
+                                  brief_description='template_%s' % name
+                                  )[0]['id']
+        except IndexError:
+            raise DatabaseError('%s not found' % name)
+
+        bundle = self._intf._exec(
+            '%s/search/saved/%s' % (self._intf._entry,
+                                    search_id
+                                    ), 'GET')
+
+        if as_xml:
+            return bundle
+        else:
+            _query = query_from_xml(bundle)
+            return (_query['row'], _query['columns'], _query['constraints'],
+                    _query['description'])
+
+    def delete_template(self, name):
+        """ Deletes a search template.
+        """
+        self.delete('template_%s' % name)
+
+    def eval_rpn_exp(self, rpnexp):
+        return rpn_contraints(rpnexp)
+
+
+class Search(object):
+    """ Define constraints to make a complex search on the database.
+
+        This :class:`Search` is available at different places throughout
+        the API:
+
+            >>> interface.select(DATA_SELECTION).where(QUERY)
+            >>> interface.manage.search.save('name', TABLE_DEFINITION, QUERY)
+
+        Examples
+        --------
+            >>> query = [('xnat:subjectData/SUBJECT_ID', 'LIKE', '%'),
+                         ('xnat:projectData/ID', '=', 'my_project'),
+                         [('xnat:subjectData/AGE', '>', '14'),
+                           'AND'
+                          ],
+                         'OR'
+                        ]
+    """
+    def __init__(self, row, columns, interface):
+        """ Configure the result table.
+
+            Parameters
+            ----------
+            row: string
+                The returned table will have one line for every matching
+                occurence of this type.
+                e.g. xnat:subjectData
+                --> table with one line per matching subject
+            columns: list
+                The returned table will have all the given columns.
+        """
+        self._row = row
+        self._columns = columns
+        self._intf = interface
+
+    def where(self, constraints=None, template=None, query=None):
+        """ Triggers the search.
+
+            Parameters
+            ----------
+            contraints: list
+                A query is an unordered list that contains
+                    - 1 or more constraints
+                    - 0 or more sub-queries (lists as this one)
+                    - 1 comparison method between the constraints
+                        ('AND' or 'OR')
+                A constraint is an ordered tuple that contains
+                    - 1 valid searchable_type/searchable_field
+                    - 1 operator among '=', '<', '>', '<=', '>=', 'LIKE'
+
+            Returns
+            -------
+            results: JsonTable object
+                An table-like object containing the results. It is
+                basically a list of dictionaries that has additional
+                helper methods.
+        """
+        self._intf._get_entry_point()
+
+        if isinstance(constraints, (str, unicode)):
+            constraints = rpn_contraints(constraints)
+        elif isinstance(template, (tuple)):
+            tmp_bundle = self._intf.manage.search.get_template(
+                template[0], True)
+
+            tmp_bundle = tmp_bundle % template[1]
+            constraints = query_from_xml(tmp_bundle)['constraints']
+        elif isinstance(query, (str, unicode)):
+            tmp_bundle = self._intf.manage.search.get(query, 'xml')
+            constraints = query_from_xml(tmp_bundle)['constraints']
+        elif isinstance(constraints, list):
+            pass
+        else:
+            raise ProgrammingError('One of contraints, template and query'
+                                   'parameters must be correctly set.')
+
+        bundle = build_search_document(self._row, self._columns, constraints)
+
+        content = self._intf._exec(
+            "%s/search?format=csv" % self._intf._entry, 'POST', bundle)
+
+        if is_xnat_error(content):
+            catch_error(content)
+
+        results = csv.reader(StringIO(content.decode('utf-8')), delimiter=',',
+                             quotechar='"')
+        headers = next(results)
+
+        headers_of_interest = []
+
+        for column in self._columns:
+            try:
+                headers_of_interest.append(
+                    difflib.get_close_matches(
+                        column.split(self._row + '/')[0].lower()
+                        or column.split(self._row + '/')[1].lower(),
+                        headers)[0]
+                    )
+            except IndexError:
+                headers_of_interest.append('unknown')
+
+        if len(self._columns) != len(headers_of_interest):
+            raise DataError('unvalid response headers')
+
+        return JsonTable([dict(zip(headers, res)) for res in results],
+                         headers_of_interest).select(headers_of_interest)
+
+    def all(self):
+        return self.where([(self._row + '/ID', 'LIKE', '%'), 'AND'])
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/select.py` & `bbrc-pyxnat-1.6/pyxnat/core/select.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,382 +1,382 @@
-import re
-
-from . import schema
-from .search import Search
-from .resources import CObject, Project, Projects, Experiment, Experiments
-# imports used implicitly
-from .uriutil import inv_translate_uri
-# from .uriutil import uri_last
-from .errors import ProgrammingError
-
-DEBUG = False
-
-
-def is_type_level(element):
-    return element.strip('/') in schema.resources_types and \
-           not is_expand_level(element)
-
-
-def is_singular_type_level(element):
-    return element.strip('/') in schema.resources_singular and \
-           not is_expand_level(element)
-
-
-def is_expand_level(element):
-    return element.startswith('//') and \
-        element.strip('/') in schema.resources_types
-
-
-def is_id_level(element):
-    return element is not None and \
-        element.strip('/') not in schema.resources_types
-
-
-def is_wildid_level(element):
-    return element is not None and \
-        element.strip('/') not in schema.resources_types and \
-        ('?' in element or '*' in element)
-
-
-def expand_level(element, fullpath):
-
-    def find_paths(element, path=[]):
-        resources_dict = schema.resources_tree
-
-        element = element.strip('/')
-        paths = []
-
-        if path == []:
-            path = [element]
-
-        init_path = path[:]
-
-        for key in resources_dict.keys():
-
-            path = init_path[:]
-            if element in resources_dict[key]:
-                path.append(key)
-                look_again = find_paths(key, path)
-
-                if look_again != []:
-                    paths.extend(look_again)
-                else:
-                    path.reverse()
-                    paths.append('/' + '/'.join(path))
-
-        return paths
-
-    absolute_paths = find_paths(element)
-
-    els = re.findall('/{1,2}.*?(?=/{1,2}|$)', fullpath)
-
-    index = els.index(element)
-
-    if index == 0:
-        return absolute_paths
-    else:
-        for i in range(1, 4):
-            if is_type_level(els[index - i]) or\
-               is_expand_level(els[index - i]):
-                parent_level = els[index - i]
-                break
-
-    if parent_level.strip('/') in schema.resources_singular:
-        parent_level += 's'
-
-    return [abspath.split(parent_level)[1]
-            for abspath in absolute_paths
-            if parent_level in abspath]
-
-
-def mtransform(paths):
-    tpaths = []
-
-    for path in paths:
-        els = re.findall('/{1,2}.*?(?=/{1,2}|$)', path)
-        tels = []
-        ignore_path = False
-
-        for i, curr_el in enumerate(els):
-
-            if i + 1 < len(els):
-                next_el = els[i + 1]
-            else:
-                next_el = None
-
-            if is_type_level(curr_el):
-
-                if not is_id_level(next_el):
-                    if not is_singular_type_level(curr_el):
-                        tels.append(curr_el)
-                        tels.append('/*')
-                    else:
-                        tels.append(curr_el + 's')
-                        tels.append('/*')
-                else:
-                    if not is_singular_type_level(curr_el):
-                        if not is_wildid_level(next_el):
-                            tels.append(curr_el.rstrip('s'))
-                        else:
-                            tels.append(curr_el)
-                    else:
-                        if not is_wildid_level(next_el):
-                            tels.append(curr_el)
-                        else:
-                            tels.append(curr_el + 's')
-
-            elif is_expand_level(curr_el):
-
-                exp_paths = [''.join(els[:i] + [rel_path] + els[i + 1:])
-                             for rel_path in expand_level(curr_el, path)
-                             ]
-
-                tpaths.extend(mtransform(exp_paths))
-                ignore_path = True
-                break
-
-            elif is_id_level(curr_el):
-                tels.append(curr_el)
-
-            else:
-                raise ProgrammingError('in %s' % path)
-
-        if not ignore_path:
-            tpaths.append(''.join(tels))
-
-    return tpaths
-
-
-def group_paths(paths):
-    groups = {}
-
-    for path in paths:
-        resources = [el
-                     for el in re.findall('/{1,2}.*?(?=/{1,2}|$)', path)
-                     if el.strip('/') in schema.resources_types
-                     and el.strip('/') not in ['files', 'file']
-                     ]
-
-        if len(resources) == 1:
-            groups.setdefault(resources[0], set()).add(path)
-            continue
-
-        for alt_path in paths:
-            if alt_path.endswith(path):
-
-                alt_rsc = \
-                    [el for el in re.findall('/{1,2}.*?(?=/{1,2}|$)',
-                                             alt_path
-                                             )
-                     if el.strip('/') in schema.resources_types
-                        and el.strip('/') not in ['files', 'file']
-                     ]
-
-                if alt_rsc[-1].strip('/') in \
-                        ['files', 'file', 'resources', 'resource'] + \
-                        list(schema.rest_translation.keys()):
-
-                    groups.setdefault(alt_rsc[-2] + alt_rsc[-1], set()
-                                      ).add(alt_path)
-
-                else:
-                    groups.setdefault(alt_rsc[-1], set()).add(alt_path)
-
-    return groups
-
-
-def compute(path):
-    if not re.match('/project(s)?|//.+', path):
-        path = '/' + path
-
-    path = inv_translate_uri(path)
-
-    try:
-        groups = group_paths(mtransform([path]))
-    except Exception:
-        raise ProgrammingError('in %s' % path)
-
-    best = []
-
-    for name in groups:
-        lightest = (0, None)
-
-        for path in groups[name]:
-            score = len(path.split('/'))
-
-            if lightest == (0, None) or lightest[0] > score:
-                lightest = (score, path)
-
-        best.append(lightest[1])
-
-    return best
-
-
-class Select(object):
-    """ Data selection interface. Callable object that indicates the
-        data to be returned to the user.
-
-        Examples
-        --------
-            Select with a path:
-                >>> interface.select('/projects/myproj/subjects').get()
-
-            Select with a datatype:
-                >>> columns = ['xnat:subjectData/PROJECT',
-                               'xnat:subjectData/SUBJECT_ID'
-                               ]
-                >>> criteria = [('xnat:subjectData/SUBJECT_ID', 'LIKE', '*'),
-                                'AND'
-                                ]
-                >>> interface.select('xnat:subjectData', columns
-                            ).where(criteria)
-    """
-    def __init__(self, interface):
-        """
-            Parameters
-            ----------
-            interface: :class:`Interface`
-                Main interface reference.
-        """
-
-        self._intf = interface
-
-    def project(self, ID):
-        """ Access a particular project.
-
-            Parameters
-            ----------
-            ID: string
-                ID of the project.
-        """
-        self._intf._get_entry_point()
-
-        return globals()['Project'](
-            '%s/projects/%s' % (self._intf._entry, ID), self._intf)
-
-    def projects(self, id_filter='*'):
-        """ Returns the list of all visible projects for the server.
-
-            Parameters
-            ----------
-            id_filter: string
-                Name pattern to filter the returned projects.
-        """
-        self._intf._get_entry_point()
-
-        return globals()['Projects'](
-            '%s/projects' % self._intf._entry, self._intf, id_filter)
-
-    def experiment(self, ID):
-        """ Access a particular experiment.
-
-            Parameters
-            ----------
-            ID: string
-                XNAT ID of experiment (NOT LABEL).
-        """
-        self._intf._get_entry_point()
-
-        return globals()['Experiment'](
-            '%s/experiments/%s' % (self._intf._entry, ID), self._intf)
-
-    def experiments(self, id_filter='*'):
-        """ Returns the list of all visible experiments for the server.
-
-            Parameters
-            ----------
-            id_filter: string
-                Name pattern to filter the returned experiments
-                (MUST BE XNAT ID's not labels).
-        """
-        self._intf._get_entry_point()
-
-        return globals()['Experiments'](
-            '%s/experiments' % self._intf._entry, self._intf, id_filter)
-
-    def tag(self, name):
-        self._intf._get_entry_point()
-
-        return self._intf.manage.tags.get(name).references()
-
-    def tags(self):
-        self._intf._get_entry_point()
-
-        return self._intf.manage.tags()
-
-    def __repr__(self):
-        return '<Root Object>'
-
-    def __call__(self, datatype_or_path, columns=[]):
-        """ Select clause to specify what type of data is to be returned.
-
-            Parameters
-            ----------
-            datatype_or_path: string
-                Can either be a resource path or a datatype:
-                    - when a path, REST resources are returned, the
-                      `columns` argument is useless.
-                    - when a datatype, a search Object is returned,
-                      the `columns` argument has to be specified.
-            columns: list
-                List of fieldtypes e.g. xnat:subjectData/SUBJECT_ID
-                Datatype and columns are used to specify the search table
-                that has to be returned. Use the method `where` on the
-                `Search` object to trigger a search on the database.
-        """
-        self._intf._get_entry_point()
-
-        if datatype_or_path.startswith('/tag'):
-            if len(datatype_or_path.split('/')) == 3:
-                return self.tag(datatype_or_path.split('/')[-1])
-            else:
-                return self.tags()
-
-        if datatype_or_path in ['/', '//', self._intf._entry]:
-            return self
-
-        if datatype_or_path.startswith(self._intf._entry):
-            datatype_or_path = datatype_or_path.split(
-                self._intf._entry, 1)[1]
-
-        if datatype_or_path.startswith('/'):
-            return_list = []
-
-            try:
-                for path in compute(datatype_or_path):
-                    if DEBUG:
-                        print('path: %s' % path)
-
-                    pairs = zip(path.split('/')[1::2], path.split('/')[2::2])
-
-                    # # in case a level id has a / - allowed for files only
-                    # if len(path.split('/')[1:]) % 2 == 1 \
-                    #         and uri_last(path) not in schema.resources_types:
-
-                    #     pairs[-1] = (pairs[-1][0], uri_last(path))
-
-                    obj = self
-                    for resource, identifier in pairs:
-
-                        if isinstance(obj, list):
-                            obj = [getattr(sobj, resource)(identifier)
-                                   for sobj in obj]
-                        else:
-                            obj = getattr(obj, resource)(identifier)
-
-                    return_list.append(obj)
-
-                if len(return_list) == 1:
-                    return return_list[0]
-                else:
-                    return CObject(return_list, self._intf)
-
-            except Exception as e:
-                if DEBUG:
-                    print(e)
-                raise ProgrammingError('in %s' % datatype_or_path)
-
-        else:
-            if columns == []:
-                columns = self._intf.inspect.datatypes(datatype_or_path)
-
-            return Search(datatype_or_path, columns, self._intf)
+import re
+
+from . import schema
+from .search import Search
+from .resources import CObject, Project, Projects, Experiment, Experiments
+# imports used implicitly
+from .uriutil import inv_translate_uri
+# from .uriutil import uri_last
+from .errors import ProgrammingError
+
+DEBUG = False
+
+
+def is_type_level(element):
+    return element.strip('/') in schema.resources_types and \
+           not is_expand_level(element)
+
+
+def is_singular_type_level(element):
+    return element.strip('/') in schema.resources_singular and \
+           not is_expand_level(element)
+
+
+def is_expand_level(element):
+    return element.startswith('//') and \
+        element.strip('/') in schema.resources_types
+
+
+def is_id_level(element):
+    return element is not None and \
+        element.strip('/') not in schema.resources_types
+
+
+def is_wildid_level(element):
+    return element is not None and \
+        element.strip('/') not in schema.resources_types and \
+        ('?' in element or '*' in element)
+
+
+def expand_level(element, fullpath):
+
+    def find_paths(element, path=[]):
+        resources_dict = schema.resources_tree
+
+        element = element.strip('/')
+        paths = []
+
+        if path == []:
+            path = [element]
+
+        init_path = path[:]
+
+        for key in resources_dict.keys():
+
+            path = init_path[:]
+            if element in resources_dict[key]:
+                path.append(key)
+                look_again = find_paths(key, path)
+
+                if look_again != []:
+                    paths.extend(look_again)
+                else:
+                    path.reverse()
+                    paths.append('/' + '/'.join(path))
+
+        return paths
+
+    absolute_paths = find_paths(element)
+
+    els = re.findall('/{1,2}.*?(?=/{1,2}|$)', fullpath)
+
+    index = els.index(element)
+
+    if index == 0:
+        return absolute_paths
+    else:
+        for i in range(1, 4):
+            if is_type_level(els[index - i]) or\
+               is_expand_level(els[index - i]):
+                parent_level = els[index - i]
+                break
+
+    if parent_level.strip('/') in schema.resources_singular:
+        parent_level += 's'
+
+    return [abspath.split(parent_level)[1]
+            for abspath in absolute_paths
+            if parent_level in abspath]
+
+
+def mtransform(paths):
+    tpaths = []
+
+    for path in paths:
+        els = re.findall('/{1,2}.*?(?=/{1,2}|$)', path)
+        tels = []
+        ignore_path = False
+
+        for i, curr_el in enumerate(els):
+
+            if i + 1 < len(els):
+                next_el = els[i + 1]
+            else:
+                next_el = None
+
+            if is_type_level(curr_el):
+
+                if not is_id_level(next_el):
+                    if not is_singular_type_level(curr_el):
+                        tels.append(curr_el)
+                        tels.append('/*')
+                    else:
+                        tels.append(curr_el + 's')
+                        tels.append('/*')
+                else:
+                    if not is_singular_type_level(curr_el):
+                        if not is_wildid_level(next_el):
+                            tels.append(curr_el.rstrip('s'))
+                        else:
+                            tels.append(curr_el)
+                    else:
+                        if not is_wildid_level(next_el):
+                            tels.append(curr_el)
+                        else:
+                            tels.append(curr_el + 's')
+
+            elif is_expand_level(curr_el):
+
+                exp_paths = [''.join(els[:i] + [rel_path] + els[i + 1:])
+                             for rel_path in expand_level(curr_el, path)
+                             ]
+
+                tpaths.extend(mtransform(exp_paths))
+                ignore_path = True
+                break
+
+            elif is_id_level(curr_el):
+                tels.append(curr_el)
+
+            else:
+                raise ProgrammingError('in %s' % path)
+
+        if not ignore_path:
+            tpaths.append(''.join(tels))
+
+    return tpaths
+
+
+def group_paths(paths):
+    groups = {}
+
+    for path in paths:
+        resources = [el
+                     for el in re.findall('/{1,2}.*?(?=/{1,2}|$)', path)
+                     if el.strip('/') in schema.resources_types
+                     and el.strip('/') not in ['files', 'file']
+                     ]
+
+        if len(resources) == 1:
+            groups.setdefault(resources[0], set()).add(path)
+            continue
+
+        for alt_path in paths:
+            if alt_path.endswith(path):
+
+                alt_rsc = \
+                    [el for el in re.findall('/{1,2}.*?(?=/{1,2}|$)',
+                                             alt_path
+                                             )
+                     if el.strip('/') in schema.resources_types
+                        and el.strip('/') not in ['files', 'file']
+                     ]
+
+                if alt_rsc[-1].strip('/') in \
+                        ['files', 'file', 'resources', 'resource'] + \
+                        list(schema.rest_translation.keys()):
+
+                    groups.setdefault(alt_rsc[-2] + alt_rsc[-1], set()
+                                      ).add(alt_path)
+
+                else:
+                    groups.setdefault(alt_rsc[-1], set()).add(alt_path)
+
+    return groups
+
+
+def compute(path):
+    if not re.match('/project(s)?|//.+', path):
+        path = '/' + path
+
+    path = inv_translate_uri(path)
+
+    try:
+        groups = group_paths(mtransform([path]))
+    except Exception:
+        raise ProgrammingError('in %s' % path)
+
+    best = []
+
+    for name in groups:
+        lightest = (0, None)
+
+        for path in groups[name]:
+            score = len(path.split('/'))
+
+            if lightest == (0, None) or lightest[0] > score:
+                lightest = (score, path)
+
+        best.append(lightest[1])
+
+    return best
+
+
+class Select(object):
+    """ Data selection interface. Callable object that indicates the
+        data to be returned to the user.
+
+        Examples
+        --------
+            Select with a path:
+                >>> interface.select('/projects/myproj/subjects').get()
+
+            Select with a datatype:
+                >>> columns = ['xnat:subjectData/PROJECT',
+                               'xnat:subjectData/SUBJECT_ID'
+                               ]
+                >>> criteria = [('xnat:subjectData/SUBJECT_ID', 'LIKE', '*'),
+                                'AND'
+                                ]
+                >>> interface.select('xnat:subjectData', columns
+                            ).where(criteria)
+    """
+    def __init__(self, interface):
+        """
+            Parameters
+            ----------
+            interface: :class:`Interface`
+                Main interface reference.
+        """
+
+        self._intf = interface
+
+    def project(self, ID):
+        """ Access a particular project.
+
+            Parameters
+            ----------
+            ID: string
+                ID of the project.
+        """
+        self._intf._get_entry_point()
+
+        return globals()['Project'](
+            '%s/projects/%s' % (self._intf._entry, ID), self._intf)
+
+    def projects(self, id_filter='*'):
+        """ Returns the list of all visible projects for the server.
+
+            Parameters
+            ----------
+            id_filter: string
+                Name pattern to filter the returned projects.
+        """
+        self._intf._get_entry_point()
+
+        return globals()['Projects'](
+            '%s/projects' % self._intf._entry, self._intf, id_filter)
+
+    def experiment(self, ID):
+        """ Access a particular experiment.
+
+            Parameters
+            ----------
+            ID: string
+                XNAT ID of experiment (NOT LABEL).
+        """
+        self._intf._get_entry_point()
+
+        return globals()['Experiment'](
+            '%s/experiments/%s' % (self._intf._entry, ID), self._intf)
+
+    def experiments(self, id_filter='*'):
+        """ Returns the list of all visible experiments for the server.
+
+            Parameters
+            ----------
+            id_filter: string
+                Name pattern to filter the returned experiments
+                (MUST BE XNAT ID's not labels).
+        """
+        self._intf._get_entry_point()
+
+        return globals()['Experiments'](
+            '%s/experiments' % self._intf._entry, self._intf, id_filter)
+
+    def tag(self, name):
+        self._intf._get_entry_point()
+
+        return self._intf.manage.tags.get(name).references()
+
+    def tags(self):
+        self._intf._get_entry_point()
+
+        return self._intf.manage.tags()
+
+    def __repr__(self):
+        return '<Root Object>'
+
+    def __call__(self, datatype_or_path, columns=[]):
+        """ Select clause to specify what type of data is to be returned.
+
+            Parameters
+            ----------
+            datatype_or_path: string
+                Can either be a resource path or a datatype:
+                    - when a path, REST resources are returned, the
+                      `columns` argument is useless.
+                    - when a datatype, a search Object is returned,
+                      the `columns` argument has to be specified.
+            columns: list
+                List of fieldtypes e.g. xnat:subjectData/SUBJECT_ID
+                Datatype and columns are used to specify the search table
+                that has to be returned. Use the method `where` on the
+                `Search` object to trigger a search on the database.
+        """
+        self._intf._get_entry_point()
+
+        if datatype_or_path.startswith('/tag'):
+            if len(datatype_or_path.split('/')) == 3:
+                return self.tag(datatype_or_path.split('/')[-1])
+            else:
+                return self.tags()
+
+        if datatype_or_path in ['/', '//', self._intf._entry]:
+            return self
+
+        if datatype_or_path.startswith(self._intf._entry):
+            datatype_or_path = datatype_or_path.split(
+                self._intf._entry, 1)[1]
+
+        if datatype_or_path.startswith('/'):
+            return_list = []
+
+            try:
+                for path in compute(datatype_or_path):
+                    if DEBUG:
+                        print('path: %s' % path)
+
+                    pairs = zip(path.split('/')[1::2], path.split('/')[2::2])
+
+                    # # in case a level id has a / - allowed for files only
+                    # if len(path.split('/')[1:]) % 2 == 1 \
+                    #         and uri_last(path) not in schema.resources_types:
+
+                    #     pairs[-1] = (pairs[-1][0], uri_last(path))
+
+                    obj = self
+                    for resource, identifier in pairs:
+
+                        if isinstance(obj, list):
+                            obj = [getattr(sobj, resource)(identifier)
+                                   for sobj in obj]
+                        else:
+                            obj = getattr(obj, resource)(identifier)
+
+                    return_list.append(obj)
+
+                if len(return_list) == 1:
+                    return return_list[0]
+                else:
+                    return CObject(return_list, self._intf)
+
+            except Exception as e:
+                if DEBUG:
+                    print(e)
+                raise ProgrammingError('in %s' % datatype_or_path)
+
+        else:
+            if columns == []:
+                columns = self._intf.inspect.datatypes(datatype_or_path)
+
+            return Search(datatype_or_path, columns, self._intf)
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/uriutil.py` & `bbrc-pyxnat-1.6/pyxnat/core/uriutil.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-from .schema import rest_translation
-# from .schema import resources_types
-
-
-def translate_uri(uri):
-    segs = uri.split('/')
-    for key in rest_translation.keys():
-        if key in segs[-2:]:
-            uri = uri.replace(key, rest_translation[key])
-
-    return uri
-
-
-def inv_translate_uri(uri):
-    inv_table = dict(zip(rest_translation.values(), rest_translation.keys()))
-
-    for key in inv_table.keys():
-        uri = uri.replace('/%s' % key, '/%s' % inv_table[key])
-
-    return uri
-
-
-def join_uri(uri, *segments):
-    part1 = [seg.lstrip('/') for seg in segments]
-    return '/'.join(uri.split('/') + part1).rstrip('/')
-
-
-def uri_last(uri):
-    # return uri.split(uri_parent(uri))[1].strip('/')
-    return uri.split('/')[-1]
-
-
-def uri_nextlast(uri):
-    # return uri_last(uri.split(uri_last(uri))[0].strip('/'))
-    # support files in a hierarchy
-    if '/files/' in uri:
-        return 'files'
-    return uri.split('/')[-2]
-
-
-def uri_parent(uri):
-    # parent = uri
-
-    # if not os.path.split(uri)[1] in resources_types:
-    #     while os.path.split(parent)[1] not in resources_types:
-    #         parent = os.path.split(parent)[0]
-
-    #     return parent
-
-    # support files in a hierarchy by stripping all but one level
-    files_index = uri.find('/files/')
-    if files_index >= 0:
-        uri = uri[:7+files_index]
-    return uri_split(uri)[0]
-
-
-def uri_grandparent(uri):
-    return uri_parent(uri_parent(uri))
-
-
-def uri_split(uri):
-    return uri.rsplit('/', 1)
-
-
-def uri_segment(uri, start=None, end=None):
-    if start is None and end is None:
-        return uri
-    elif start is None:
-        return '/'+'/'.join(uri.split('/')[:end])
-    elif end is None:
-        return '/'+'/'.join(uri.split('/')[start:])
-    else:
-        return '/'+'/'.join(uri.split('/')[start:end])
-
-
-def uri_shape(uri):
-    import re
-
-    kwid_map = dict(zip(uri.split('/')[1::2], uri.split('/')[2::2]))
-    shapes = {}
-
-    for kw in kwid_map:
-        seps = kwid_map[kw]
-
-        for char in re.findall('[a-zA-Z0-9]', seps):
-            seps = seps.replace(char, '')
-            chunks = []
-            p = '|'.join(seps)
-            s = re.split(p, kwid_map[kw]) if p != '' else kwid_map[kw]
-            for chunk in s:
-                try:
-                    float(chunk)
-                    chunk = '*'
-                except Exception:
-                    pass
-
-                chunks.append(chunk)
-
-            shapes[kw] = '?'.join(chunks)
-
-    return make_uri(shapes)
-
-
-def make_uri(_dict):
-    uri = ''
-
-    kws = ['projects', 'subjects', 'experiments', 'assessors',
-           'reconstructions', 'scans', 'resources', 'in_resources',
-           'out_resources', 'files', 'in_files', 'out_files']
-
-    for kw in kws:
-        if kw in _dict.keys():
-            uri += '/%s/%s' % (kw, _dict.get(kw))
-
-    return uri
-
-
-def check_entry(func):
-    def inner(*args, **kwargs):
-        args[0]._intf._get_entry_point()
-        return func(*args, **kwargs)
-
-    return inner
-
-
-def extract_uri(uri):
-    """
-    Destructure the given REST uri into project,subject and experiment.
-
-    Returns None if any one of project,subject or experiment is unspecified in
-    the URI and a (project,subject,experiment) triple otherwise.
-    """
-    # elements in URLs are always separated by /, regardless of client
-    split = uri.split('/')
-    # a well qualified uri has a project subject, and experiment name
-    # so when split the following items should be present:
-    # ['', 'data', 'projects', 'project-name', 'subjects', 'subject-name',
-    # 'experiments', 'experiment-name', 'scans']
-
-    # Based on the above comment if there aren't 9 items in the split list the
-    # uri isn't well qualified
-    if (len(split) != 9):
-        return None
-
-    project = split[3]
-    subject = split[5]
-    experiment = split[7]
-
-    return (project, subject, experiment)
-
-
-def file_path(uri):
-    """return the relative path of the file in the given URI
-
-    for uri = '/.../files/a/b/c', return 'a/b/c'
-
-    raises ValueError (through .index()) if '/files/' is not in the URI
-    """
-    return uri[7+uri.index('/files/'):]
+from .schema import rest_translation
+# from .schema import resources_types
+
+
+def translate_uri(uri):
+    segs = uri.split('/')
+    for key in rest_translation.keys():
+        if key in segs[-2:]:
+            uri = uri.replace(key, rest_translation[key])
+
+    return uri
+
+
+def inv_translate_uri(uri):
+    inv_table = dict(zip(rest_translation.values(), rest_translation.keys()))
+
+    for key in inv_table.keys():
+        uri = uri.replace('/%s' % key, '/%s' % inv_table[key])
+
+    return uri
+
+
+def join_uri(uri, *segments):
+    part1 = [seg.lstrip('/') for seg in segments]
+    return '/'.join(uri.split('/') + part1).rstrip('/')
+
+
+def uri_last(uri):
+    # return uri.split(uri_parent(uri))[1].strip('/')
+    return uri.split('/')[-1]
+
+
+def uri_nextlast(uri):
+    # return uri_last(uri.split(uri_last(uri))[0].strip('/'))
+    # support files in a hierarchy
+    if '/files/' in uri:
+        return 'files'
+    return uri.split('/')[-2]
+
+
+def uri_parent(uri):
+    # parent = uri
+
+    # if not os.path.split(uri)[1] in resources_types:
+    #     while os.path.split(parent)[1] not in resources_types:
+    #         parent = os.path.split(parent)[0]
+
+    #     return parent
+
+    # support files in a hierarchy by stripping all but one level
+    files_index = uri.find('/files/')
+    if files_index >= 0:
+        uri = uri[:7+files_index]
+    return uri_split(uri)[0]
+
+
+def uri_grandparent(uri):
+    return uri_parent(uri_parent(uri))
+
+
+def uri_split(uri):
+    return uri.rsplit('/', 1)
+
+
+def uri_segment(uri, start=None, end=None):
+    if start is None and end is None:
+        return uri
+    elif start is None:
+        return '/'+'/'.join(uri.split('/')[:end])
+    elif end is None:
+        return '/'+'/'.join(uri.split('/')[start:])
+    else:
+        return '/'+'/'.join(uri.split('/')[start:end])
+
+
+def uri_shape(uri):
+    import re
+
+    kwid_map = dict(zip(uri.split('/')[1::2], uri.split('/')[2::2]))
+    shapes = {}
+
+    for kw in kwid_map:
+        seps = kwid_map[kw]
+
+        for char in re.findall('[a-zA-Z0-9]', seps):
+            seps = seps.replace(char, '')
+            chunks = []
+            p = '|'.join(seps)
+            s = re.split(p, kwid_map[kw]) if p != '' else kwid_map[kw]
+            for chunk in s:
+                try:
+                    float(chunk)
+                    chunk = '*'
+                except Exception:
+                    pass
+
+                chunks.append(chunk)
+
+            shapes[kw] = '?'.join(chunks)
+
+    return make_uri(shapes)
+
+
+def make_uri(_dict):
+    uri = ''
+
+    kws = ['projects', 'subjects', 'experiments', 'assessors',
+           'reconstructions', 'scans', 'resources', 'in_resources',
+           'out_resources', 'files', 'in_files', 'out_files']
+
+    for kw in kws:
+        if kw in _dict.keys():
+            uri += '/%s/%s' % (kw, _dict.get(kw))
+
+    return uri
+
+
+def check_entry(func):
+    def inner(*args, **kwargs):
+        args[0]._intf._get_entry_point()
+        return func(*args, **kwargs)
+
+    return inner
+
+
+def extract_uri(uri):
+    """
+    Destructure the given REST uri into project,subject and experiment.
+
+    Returns None if any one of project,subject or experiment is unspecified in
+    the URI and a (project,subject,experiment) triple otherwise.
+    """
+    # elements in URLs are always separated by /, regardless of client
+    split = uri.split('/')
+    # a well qualified uri has a project subject, and experiment name
+    # so when split the following items should be present:
+    # ['', 'data', 'projects', 'project-name', 'subjects', 'subject-name',
+    # 'experiments', 'experiment-name', 'scans']
+
+    # Based on the above comment if there aren't 9 items in the split list the
+    # uri isn't well qualified
+    if (len(split) != 9):
+        return None
+
+    project = split[3]
+    subject = split[5]
+    experiment = split[7]
+
+    return (project, subject, experiment)
+
+
+def file_path(uri):
+    """return the relative path of the file in the given URI
+
+    for uri = '/.../files/a/b/c', return 'a/b/c'
+
+    raises ValueError (through .index()) if '/files/' is not in the URI
+    """
+    return uri[7+uri.index('/files/'):]
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/users.py` & `bbrc-pyxnat-1.6/pyxnat/core/users.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from .jsonutil import JsonTable
-
-
-class Users(object):
-    """ Database user management interface. It is used to retrieve information
-        on users registered on a server.
-
-        .. note::
-
-            At the moment user creation and deletion is not supported through
-            the REST API but it will be at some point.
-
-        Examples
-        --------
-            >>> interface.manage.users()
-            ['list_of_users']
-            >>> interface.manage.users.firstname('nosetests')
-            'nose'
-
-        See Also
-        --------
-        :func:`Project.users`
-        :func:`Project.add_user`
-        :func:`Project.remove_user`
-    """
-
-    def __init__(self, interface):
-        """
-            Parameters
-            ----------
-            interface: :class:`Interface`
-                Main interface reference.
-        """
-        self._intf = interface
-
-    def __call__(self):
-        """ Returns the list of all registered users on the server.
-        """
-        self._intf._get_entry_point()
-
-        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
-                         ).get('login', always_list=True)
-
-    def firstname(self, login):
-        """ Returns the firstname of the user.
-        """
-        self._intf._get_entry_point()
-
-        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
-                         ).where(login=login)['firstname']
-
-    def lastname(self, login):
-        """ Returns the lastname of the user.
-        """
-        self._intf._get_entry_point()
-
-        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
-                         ).where(login=login)['lastname']
-
-    def id(self, login):
-        """ Returns the id of the user.
-        """
-        self._intf._get_entry_point()
-
-        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
-                         ).where(login=login)['xdat_user_id']
-
-    def email(self, login):
-        """ Returns the email of the user.
-        """
-        self._intf._get_entry_point()
-
-        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
-                         ).where(login=login)['email']
-
-    def resources(self):
-        """ Returns the resources of the user.
-        """
-        self._intf._get_entry_point()
-
-        print(self._intf._get_json(
-            '%s/user/cache/resources' % self._intf._entry))
+from .jsonutil import JsonTable
+
+
+class Users(object):
+    """ Database user management interface. It is used to retrieve information
+        on users registered on a server.
+
+        .. note::
+
+            At the moment user creation and deletion is not supported through
+            the REST API but it will be at some point.
+
+        Examples
+        --------
+            >>> interface.manage.users()
+            ['list_of_users']
+            >>> interface.manage.users.firstname('nosetests')
+            'nose'
+
+        See Also
+        --------
+        :func:`Project.users`
+        :func:`Project.add_user`
+        :func:`Project.remove_user`
+    """
+
+    def __init__(self, interface):
+        """
+            Parameters
+            ----------
+            interface: :class:`Interface`
+                Main interface reference.
+        """
+        self._intf = interface
+
+    def __call__(self):
+        """ Returns the list of all registered users on the server.
+        """
+        self._intf._get_entry_point()
+
+        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
+                         ).get('login', always_list=True)
+
+    def firstname(self, login):
+        """ Returns the firstname of the user.
+        """
+        self._intf._get_entry_point()
+
+        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
+                         ).where(login=login)['firstname']
+
+    def lastname(self, login):
+        """ Returns the lastname of the user.
+        """
+        self._intf._get_entry_point()
+
+        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
+                         ).where(login=login)['lastname']
+
+    def id(self, login):
+        """ Returns the id of the user.
+        """
+        self._intf._get_entry_point()
+
+        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
+                         ).where(login=login)['xdat_user_id']
+
+    def email(self, login):
+        """ Returns the email of the user.
+        """
+        self._intf._get_entry_point()
+
+        return JsonTable(self._intf._get_json('%s/users' % self._intf._entry)
+                         ).where(login=login)['email']
+
+    def resources(self):
+        """ Returns the resources of the user.
+        """
+        self._intf._get_entry_point()
+
+        print(self._intf._get_json(
+            '%s/user/cache/resources' % self._intf._entry))
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/xpass.py` & `bbrc-pyxnat-1.6/pyxnat/core/xpass.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import os
-from functools import partial
-
-
-# default path to xnat pass file
-def path():
-    return os.getenv('USERPROFILE') or os.getenv('HOME') + "/.xnatPass"
-
-
-# str ->  {'host': ..., 'u': ..., 'p': ..., 'port': ...} | None
-def read_xnat_pass(f):
-    if os.path.exists(f) and os.path.isfile(f):
-        infile = open(f)
-        return parse_xnat_pass(infile.readlines())
-    else:
-        # raise IOError('XNAT Pass file :' + f + " does not exist")
-        return None
-
-
-# [str] -> {'host': ..., 'u': ..., 'p': ..., 'port':...} | None
-def parse_xnat_pass(lines):
-    empty = {'host': None, 'u': None, 'p': None}
-    line = find_plus_line(lines)
-    u = ('u', partial(find_token, '@'), True)
-    host = ('host', partial(find_token, '='), True)
-    p = ('p', partial(lambda x: (x, x)), True)
-
-    def update_state(x, k, state):
-        state[k] = x
-        return state
-    if line is None:
-        return None
-    else:
-        return chain([u, host, p], line, empty, update_state)
-
-
-# [(str, str -> str, bool)] ->
-#  str ->
-#  dict
-#  dict -> dict
-#  dict | None
-def chain(ops, initEnv, initState, update_statef):
-    env = initEnv
-    state = initState
-    for op in ops:
-        (k, _op, mandatory) = op
-        tmp = _op(env)
-        if tmp is None:
-            if mandatory:
-                return None
-        else:
-            (v, rest) = tmp
-            env = rest
-            state = update_statef(v, k, state)
-    return state
-
-
-# [str] -> str | None
-def find_plus_line(lines):
-    plusLines = list(filter(lambda x: x.startswith('+'), lines))
-
-    if not plusLines:
-        return None
-    else:
-        return ''.join(plusLines[0])[1:]
-
-
-# char -> str -> (str,str) | None
-def find_token(tok, line):
-    splitString = list(map(lambda x: x.strip(), line.split(tok)))
-    #print([line, tok, splitString])
-    if splitString is None or len(splitString) == 0 or len(splitString) == 1 \
-            or splitString[0] == '':
-        return None
-    else:
-        return (splitString[0], tok.join(splitString[1:]))
+import os
+from functools import partial
+
+
+# default path to xnat pass file
+def path():
+    return os.getenv('USERPROFILE') or os.getenv('HOME') + "/.xnatPass"
+
+
+# str ->  {'host': ..., 'u': ..., 'p': ..., 'port': ...} | None
+def read_xnat_pass(f):
+    if os.path.exists(f) and os.path.isfile(f):
+        infile = open(f)
+        return parse_xnat_pass(infile.readlines())
+    else:
+        # raise IOError('XNAT Pass file :' + f + " does not exist")
+        return None
+
+
+# [str] -> {'host': ..., 'u': ..., 'p': ..., 'port':...} | None
+def parse_xnat_pass(lines):
+    empty = {'host': None, 'u': None, 'p': None}
+    line = find_plus_line(lines)
+    u = ('u', partial(find_token, '@'), True)
+    host = ('host', partial(find_token, '='), True)
+    p = ('p', partial(lambda x: (x, x)), True)
+
+    def update_state(x, k, state):
+        state[k] = x
+        return state
+    if line is None:
+        return None
+    else:
+        return chain([u, host, p], line, empty, update_state)
+
+
+# [(str, str -> str, bool)] ->
+#  str ->
+#  dict
+#  dict -> dict
+#  dict | None
+def chain(ops, initEnv, initState, update_statef):
+    env = initEnv
+    state = initState
+    for op in ops:
+        (k, _op, mandatory) = op
+        tmp = _op(env)
+        if tmp is None:
+            if mandatory:
+                return None
+        else:
+            (v, rest) = tmp
+            env = rest
+            state = update_statef(v, k, state)
+    return state
+
+
+# [str] -> str | None
+def find_plus_line(lines):
+    plusLines = list(filter(lambda x: x.startswith('+'), lines))
+
+    if not plusLines:
+        return None
+    else:
+        return ''.join(plusLines[0])[1:]
+
+
+# char -> str -> (str,str) | None
+def find_token(tok, line):
+    splitString = list(map(lambda x: x.strip(), line.split(tok)))
+    #print([line, tok, splitString])
+    if splitString is None or len(splitString) == 0 or len(splitString) == 1 \
+            or splitString[0] == '':
+        return None
+    else:
+        return (splitString[0], tok.join(splitString[1:]))
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/core/xpath_store.py` & `bbrc-pyxnat-1.6/pyxnat/core/xpath_store.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-import re
-from lxml import etree
-
-from .jsonutil import JsonTable
-
-
-def get_subject_id(location):
-    f = open(location, 'rb')
-    content = f.read()
-    f.close()
-
-    subject = re.findall('<xnat:Subject\sID="(.*?)"\s', content)
-
-    if subject != []:
-        return subject[0]
-
-
-class XpathStore(object):
-
-    """ This utility class is used to query XML files describing XNAT
-        subjects but which are stored in the cache directory. Xpath is
-        used as the query lanaguage but a few helpers are provided
-        to make simple queries.
-    """
-
-    def __init__(self, interface):
-        self._intf = interface
-        self._nsmap = {}
-        self._tree = etree.Element('Store')
-
-    def __call__(self, xpath):
-        if self._tree is None:
-            self._load()
-
-        return self._tree.xpath(xpath, namespaces=self._nsmap)
-
-    def _load(self, content):
-        if not content:
-            return
-        new_subject = etree.fromstring(content)
-        self._nsmap = new_subject.nsmap
-        subject_id = new_subject.xpath('@ID')[0]
-        old_subject = self.subject(subject_id)
-        if old_subject:
-            self._tree.replace(old_subject, new_subject)
-        else:
-            self._tree.append(new_subject)
-
-    def _last_modified(self):
-        entry_point = self._intf._get_entry_point()
-        uri = '%s/subjects?columns=last_modified' % entry_point
-
-        return dict(JsonTable(self._intf._get_json(uri),
-                              order_by=['ID', 'last_modified']
-                              ).select(['ID', 'last_modified']
-                                       ).items())
-
-    def update(self):
-        """ Updates the xml files in the cachedir.
-        """
-
-        self.checkout(subjects=self.subjects())
-
-    def checkout(self, project=None, subjects=None):
-        """ Downloads all the subject XMLs for a project or a list
-            of subjects.
-
-            Parameters
-            ----------
-            project: str
-                The id of the project
-            subjects: list
-                List of subjects that have to be downloaded.
-        """
-        if project is not None and subjects is None:
-            for s in self._intf.select('/project/%s/subjects' % project):
-                self._load(s.get())
-        elif subjects is not None:
-            for sid in subjects:
-                self._load(self._intf._exec('%s/subjects/%s?format=xml' % (
-                          self._intf._get_entry_point(), sid))
-                          )
-
-    def subject(self, subject_id):
-        tmp = self.__call__('//xnat:Subject[@ID="%s"]' % (subject_id))
-
-        if len(tmp) > 0:
-            return tmp[1]
-        return None
-
-    def subjects(self):
-        """ Returns all the subject ids.
-        """
-        return self.__call__('//xnat:Subject/attribute::ID')
-
-    def keys(self):
-        """ Returns attribute keys at the subject level.
-        """
-        return self.element_keys('xnat:Subject')
-
-    def values(self, key):
-        """ Returns the values for all subjects for a specific attribute.
-        """
-        return self.element_values('xnat:Subject', key)
-
-    def attrs(self):
-        """ Returns the attributes of all subjects.
-        """
-        return self.element_attrs('xnat:Subject')
-
-    def elements(self):
-        """ Returns the element names for all subjects elements.
-
-            .. note:: in xpath terms, this function is returning all
-                the names of the subjects descendant nodes.
-        """
-        elements = set()
-
-        for element in self.__call__('//xnat:Subject/descendant::*'):
-            for ns in element.nsmap:
-                if element.nsmap[ns] in element.tag:
-                    n = element.tag.replace('{%s}' % element.nsmap[ns],
-                                            '%s:' % ns)
-                    elements.add(n)
-
-        return list(elements)
-
-    def element_attrs(self, name):
-        """ Returns the attributes of this specific element.
-        """
-        attrs = []
-
-        for element in self.__call__('//%s' % name):
-            attrs.append(element.attrib)
-
-        return attrs
-
-    def element_keys(self, name):
-        """ Returns the attribute keys of this specific element.
-        """
-        keys = set()
-
-        for element in self.__call__('//%s' % name):
-            for element_key in element.keys():
-                keys.add(element_key)
-
-        return list(keys)
-
-    def element_values(self, name, key):
-        """ Returns the attribute values of this specific element.
-        """
-        values = set()
-
-        for subject in self.__call__('//%s' % name):
-            values.add(subject.get(key))
-
-        return list(values)
-
-    def element_text(self, name):
-        """ Returns the text values of this specific element.
-        """
-        return list(set(self.__call__('//%s/child::text()' % name)))
+import re
+from lxml import etree
+
+from .jsonutil import JsonTable
+
+
+def get_subject_id(location):
+    f = open(location, 'rb')
+    content = f.read()
+    f.close()
+
+    subject = re.findall('<xnat:Subject\sID="(.*?)"\s', content)
+
+    if subject != []:
+        return subject[0]
+
+
+class XpathStore(object):
+
+    """ This utility class is used to query XML files describing XNAT
+        subjects but which are stored in the cache directory. Xpath is
+        used as the query lanaguage but a few helpers are provided
+        to make simple queries.
+    """
+
+    def __init__(self, interface):
+        self._intf = interface
+        self._nsmap = {}
+        self._tree = etree.Element('Store')
+
+    def __call__(self, xpath):
+        if self._tree is None:
+            self._load()
+
+        return self._tree.xpath(xpath, namespaces=self._nsmap)
+
+    def _load(self, content):
+        if not content:
+            return
+        new_subject = etree.fromstring(content)
+        self._nsmap = new_subject.nsmap
+        subject_id = new_subject.xpath('@ID')[0]
+        old_subject = self.subject(subject_id)
+        if old_subject:
+            self._tree.replace(old_subject, new_subject)
+        else:
+            self._tree.append(new_subject)
+
+    def _last_modified(self):
+        entry_point = self._intf._get_entry_point()
+        uri = '%s/subjects?columns=last_modified' % entry_point
+
+        return dict(JsonTable(self._intf._get_json(uri),
+                              order_by=['ID', 'last_modified']
+                              ).select(['ID', 'last_modified']
+                                       ).items())
+
+    def update(self):
+        """ Updates the xml files in the cachedir.
+        """
+
+        self.checkout(subjects=self.subjects())
+
+    def checkout(self, project=None, subjects=None):
+        """ Downloads all the subject XMLs for a project or a list
+            of subjects.
+
+            Parameters
+            ----------
+            project: str
+                The id of the project
+            subjects: list
+                List of subjects that have to be downloaded.
+        """
+        if project is not None and subjects is None:
+            for s in self._intf.select('/project/%s/subjects' % project):
+                self._load(s.get())
+        elif subjects is not None:
+            for sid in subjects:
+                self._load(self._intf._exec('%s/subjects/%s?format=xml' % (
+                          self._intf._get_entry_point(), sid))
+                          )
+
+    def subject(self, subject_id):
+        tmp = self.__call__('//xnat:Subject[@ID="%s"]' % (subject_id))
+
+        if len(tmp) > 0:
+            return tmp[1]
+        return None
+
+    def subjects(self):
+        """ Returns all the subject ids.
+        """
+        return self.__call__('//xnat:Subject/attribute::ID')
+
+    def keys(self):
+        """ Returns attribute keys at the subject level.
+        """
+        return self.element_keys('xnat:Subject')
+
+    def values(self, key):
+        """ Returns the values for all subjects for a specific attribute.
+        """
+        return self.element_values('xnat:Subject', key)
+
+    def attrs(self):
+        """ Returns the attributes of all subjects.
+        """
+        return self.element_attrs('xnat:Subject')
+
+    def elements(self):
+        """ Returns the element names for all subjects elements.
+
+            .. note:: in xpath terms, this function is returning all
+                the names of the subjects descendant nodes.
+        """
+        elements = set()
+
+        for element in self.__call__('//xnat:Subject/descendant::*'):
+            for ns in element.nsmap:
+                if element.nsmap[ns] in element.tag:
+                    n = element.tag.replace('{%s}' % element.nsmap[ns],
+                                            '%s:' % ns)
+                    elements.add(n)
+
+        return list(elements)
+
+    def element_attrs(self, name):
+        """ Returns the attributes of this specific element.
+        """
+        attrs = []
+
+        for element in self.__call__('//%s' % name):
+            attrs.append(element.attrib)
+
+        return attrs
+
+    def element_keys(self, name):
+        """ Returns the attribute keys of this specific element.
+        """
+        keys = set()
+
+        for element in self.__call__('//%s' % name):
+            for element_key in element.keys():
+                keys.add(element_key)
+
+        return list(keys)
+
+    def element_values(self, name, key):
+        """ Returns the attribute values of this specific element.
+        """
+        values = set()
+
+        for subject in self.__call__('//%s' % name):
+            values.add(subject.get(key))
+
+        return list(values)
+
+    def element_text(self, name):
+        """ Returns the text values of this specific element.
+        """
+        return list(set(self.__call__('//%s/child::text()' % name)))
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/__init__.py` & `bbrc-pyxnat-1.6/pyxnat/tests/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from functools import wraps
-from nose import SkipTest
-from nose.plugins.attrib import attr
-import os
-
-
-def skip_if_no_network(func=None):
-    """Skip test completely in NONETWORK settings
-    If not used as a decorator, and just a function, could be used at the module level
-    """
-
-    def check_and_raise():
-        if os.environ.get('PYXNAT_SKIP_NETWORK_TESTS'):
-            raise SkipTest("Skipping since no network settings")
-
-    if func:
-        @wraps(func)
-        @attr('skip_if_no_network')
-        def newfunc(*args, **kwargs):
-            check_and_raise()
-            return func(*args, **kwargs)
-        return newfunc
-    else:
-        check_and_raise()
+from functools import wraps
+import pytest
+import os
+
+
+def skip_if_no_network(func=None):
+    """Skip test completely in NONETWORK settings
+    If not used as a decorator, and just a function, could be used at the module level
+    """
+
+    def check_and_raise():
+        if os.environ.get('PYXNAT_SKIP_NETWORK_TESTS'):
+            pytest.skip("Skipping since no network settings")
+
+    if func:
+        @wraps(func)
+        def newfunc(*args, **kwargs):
+            check_and_raise()
+            return func(*args, **kwargs)
+        return newfunc
+    else:
+        check_and_raise()
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/array_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/array_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import unittest
-import os.path as op
-from pyxnat import Interface
-from . import skip_if_no_network
-import logging as log
-log.basicConfig(level=log.INFO)
-
-
-class ArrayTests(unittest.TestCase):
-    ''' Resource-related XNAT connectivity test cases '''
-
-    def setUp(self):
-        fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-        self._intf = Interface(config=fp)
-
-    @skip_if_no_network
-    def test_array_experiments(self):
-        '''
-        Get a list of experiments from a given subject which has multiple types
-        of experiments (i.e. MRSessions and PETSessions) and assert it gathers
-        them all.
-        '''
-        e = self._intf.array.experiments(subject_id='CENTRAL_S06242').data
-        self.assertGreaterEqual(len(e), 3)
-
-    @skip_if_no_network
-    def test_array_mrsessions(self):
-        '''
-        From a given subject which has multiple types of experiments, get a
-        list of MRI sessions and assert its length matches the list of
-        experiments of type 'xnat:mrSessionData'
-        '''
-        mris = self._intf.array.mrsessions(subject_id='CENTRAL_S06242').data
-        e = self._intf.array.experiments(subject_id='CENTRAL_S06242',
-                                         experiment_type='xnat:mrSessionData')
-        exps = e.data
-        self.assertListEqual(mris, exps)
-
-    @skip_if_no_network
-    def test_array_scans(self):
-        '''
-        Get a list of scans from a given experiment which has multiple types
-        of scans (i.e. PETScans and CTScans) and assert it gathers them all.
-        '''
-        s = self._intf.array.scans(experiment_id='CENTRAL_E72012').data
-        self.assertEqual(len(s), 16)
-
-    @skip_if_no_network
-    def test_array_mrscans(self):
-        '''
-        Get a list of MRI scans from a given experiment which has multiple
-        scans mixed (i.e. MRScans and MRSpectroscopies, aka OtherDicomScans)
-        and assert its length matches the list of scans filtered by type
-        'xnat:mrScanData'
-        '''
-        mris = self._intf.array.mrscans(experiment_id='CENTRAL_E72012').data
-        exps = self._intf.array.scans(experiment_id='CENTRAL_E72012',
-                                      scan_type='xnat:mrScanData').data
-        self.assertListEqual([i['xnat:mrscandata/id'] for i in mris],
-                             [i['xnat:mrscandata/id'] for i in exps])
-
-    @skip_if_no_network
-    def test_search_experiments(self):
-        et = 'xnat:subjectData'
-        e = self._intf.array.search_experiments(project_id='nosetests5',
-                                                experiment_type=et)
-        res = e.data
-        self.assertGreaterEqual(len(res), 1)
+import unittest
+import os.path as op
+from pyxnat import Interface
+from pyxnat.tests import skip_if_no_network
+import logging as log
+log.basicConfig(level=log.INFO)
+
+
+class ArrayTests(unittest.TestCase):
+    ''' Resource-related XNAT connectivity test cases '''
+
+    def setUp(self):
+        fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+        self._intf = Interface(config=fp)
+
+    @skip_if_no_network
+    def test_array_experiments(self):
+        '''
+        Get a list of experiments from a given subject which has multiple types
+        of experiments (i.e. MRSessions and PETSessions) and assert it gathers
+        them all.
+        '''
+        e = self._intf.array.experiments(subject_id='CENTRAL02_S01346').data
+        self.assertGreaterEqual(len(e), 3)
+
+    @skip_if_no_network
+    def test_array_mrsessions(self):
+        '''
+        From a given subject which has multiple types of experiments, get a
+        list of MRI sessions and assert its length matches the list of
+        experiments of type 'xnat:mrSessionData'
+        '''
+        mris = self._intf.array.mrsessions(subject_id='CENTRAL02_S01346').data
+        e = self._intf.array.experiments(subject_id='CENTRAL02_S01346',
+                                         experiment_type='xnat:mrSessionData')
+        exps = e.data
+        self.assertListEqual(mris, exps)
+
+    @skip_if_no_network
+    def test_array_scans(self):
+        '''
+        Get a list of scans from a given experiment which has multiple types
+        of scans (i.e. PETScans and CTScans) and assert it gathers them all.
+        '''
+        s = self._intf.array.scans(experiment_id='CENTRAL03_E05157').data
+        self.assertEqual(len(s), 4)
+
+    @skip_if_no_network
+    def test_array_mrscans(self):
+        '''
+        Get a list of MRI scans from a given experiment which has multiple
+        scans mixed (i.e. MRScans and MRSpectroscopies, aka OtherDicomScans)
+        and assert its length matches the list of scans filtered by type
+        'xnat:mrScanData'
+        '''
+        mris = self._intf.array.mrscans(experiment_id='CENTRAL02_E01892').data
+        exps = self._intf.array.scans(experiment_id='CENTRAL02_E01892',
+                                      scan_type='xnat:mrScanData').data
+        self.assertListEqual([i['xnat:mrscandata/id'] for i in mris],
+                             [i['xnat:mrscandata/id'] for i in exps])
+
+    @skip_if_no_network
+    def test_search_experiments(self):
+        et = 'xnat:subjectData'
+        e = self._intf.array.search_experiments(project_id='nosetests5',
+                                                experiment_type=et)
+        res = e.data
+        self.assertGreaterEqual(len(res), 1)
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/attributes_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/attributes_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-import os.path as op
-from uuid import uuid1
-import time
-from . import skip_if_no_network
-from pyxnat import Interface
-from pyxnat.core import interfaces
-
-
-_modulepath = op.dirname(op.abspath(__file__))
-
-fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-central = Interface(config=fp)
-interfaces.STUBBORN = True
-
-sid = uuid1().hex
-eid = uuid1().hex
-
-subject = central.select.project('nosetests5').subject(sid)
-experiment = subject.experiment(eid)
-
-
-@skip_if_no_network
-def test_01_fancy_resource_create():
-
-    field_data = {'experiment': 'xnat:mrSessionData',
-                  'ID': 'TEST_%s' % eid,
-                  'xnat:mrSessionData/age': '42',
-                  'xnat:subjectData/investigator/lastname': 'doe',
-                  'xnat:subjectData/investigator/firstname': 'john',
-                  'xnat:subjectData/ID': 'TEST_%s' % sid,
-                  }
-
-    experiment.create(**field_data)
-    assert subject.exists()
-    assert experiment.exists()
-
-    globals()['subject'] = experiment.parent()
-    globals()['experiment'] = experiment
-
-
-@skip_if_no_network
-def test_02_attr_get():
-    assert experiment.attrs.get('xnat:mrSessionData/age') == '42.0'
-
-
-@skip_if_no_network
-def test_03_attr_mget():
-    time.sleep(5)
-    fields = ['xnat:subjectData/investigator/firstname',
-              'xnat:subjectData/investigator/lastname'
-              ]
-
-    assert subject.attrs.mget(fields) == ['john', 'doe']
-
-
-@skip_if_no_network
-def test_04_attr_set():
-    experiment.attrs.set('xnat:mrSessionData/age', '26')
-    assert experiment.attrs.get('xnat:mrSessionData/age') == '26.0'
-
-# def test_attr_mset():
-#     subject = central.select.project('nosetests').subject(sid)
-#     time.sleep(5)
-#     field_data = {'xnat:subjectData/investigator/firstname':'angus',
-#                   'xnat:subjectData/investigator/lastname':'young',
-#                   }
-#
-#     subject.attrs.mset(field_data)
-#     returned = subject.attrs.mget(field_data.keys())
-#
-#     assert set(returned) == \
-#         set(field_data.values()),
-#              '''set: %s returned: %s ''' %(field_data.values(), returned)
-
-
-@skip_if_no_network
-def test_05_cleanup():
-
-    subject.delete()
-    assert not subject.exists()
-
-
-@skip_if_no_network
-def test_06_list_project_attrs():
-
-    project_attributes = ['xnat:projectData/name',
-                          'xnat:projectData/type',
-                          'xnat:projectData/description',
-                          'xnat:projectData/keywords',
-                          'xnat:projectData/aliases',
-                          'xnat:projectData/aliases/alias',
-                          'xnat:projectData/aliases/alias/None',
-                          'xnat:projectData/publications',
-                          'xnat:projectData/publications/publication',
-                          'xnat:projectData/resources',
-                          'xnat:projectData/resources/resource',
-                          'xnat:projectData/studyProtocol',
-                          'xnat:projectData/PI',
-                          'xnat:projectData/investigators',
-                          'xnat:projectData/investigators/investigator',
-                          'xnat:projectData/fields',
-                          'xnat:projectData/fields/field',
-                          'xnat:projectData/fields/field/None']
-
-    p = central.select.project('nosetests')
-    assert(p.attrs() == [])
-
-    central.manage.schemas.add('xapi/schemas/xnat')
-    p = central.select.project('nosetests')
-    assert (p.attrs() == project_attributes)
+import os.path as op
+from uuid import uuid1
+import time
+from pyxnat.tests import skip_if_no_network
+from pyxnat import Interface
+from pyxnat.core import interfaces
+
+
+_modulepath = op.dirname(op.abspath(__file__))
+
+fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+central = Interface(config=fp)
+interfaces.STUBBORN = True
+
+sid = uuid1().hex
+eid = uuid1().hex
+
+subject = central.select.project('nosetests5').subject(sid)
+experiment = subject.experiment(eid)
+
+
+@skip_if_no_network
+def test_01_fancy_resource_create():
+
+    field_data = {'experiment': 'xnat:mrSessionData',
+                  'ID': 'TEST_%s' % eid,
+                  'xnat:mrSessionData/age': '42',
+                  'xnat:subjectData/investigator/lastname': 'doe',
+                  'xnat:subjectData/investigator/firstname': 'john',
+                  'xnat:subjectData/ID': 'TEST_%s' % sid,
+                  }
+
+    experiment.create(**field_data)
+    assert subject.exists()
+    assert experiment.exists()
+
+    globals()['subject'] = experiment.parent()
+    globals()['experiment'] = experiment
+
+
+@skip_if_no_network
+def test_02_attr_get():
+    assert experiment.attrs.get('xnat:mrSessionData/age') == '42.0'
+
+
+@skip_if_no_network
+def test_03_attr_mget():
+    time.sleep(5)
+    fields = ['xnat:subjectData/investigator/firstname',
+              'xnat:subjectData/investigator/lastname'
+              ]
+
+    assert subject.attrs.mget(fields) == ['john', 'doe']
+
+
+@skip_if_no_network
+def test_04_attr_set():
+    experiment.attrs.set('xnat:mrSessionData/age', '26')
+    assert experiment.attrs.get('xnat:mrSessionData/age') == '26.0'
+
+# def test_attr_mset():
+#     subject = central.select.project('nosetests').subject(sid)
+#     time.sleep(5)
+#     field_data = {'xnat:subjectData/investigator/firstname':'angus',
+#                   'xnat:subjectData/investigator/lastname':'young',
+#                   }
+#
+#     subject.attrs.mset(field_data)
+#     returned = subject.attrs.mget(field_data.keys())
+#
+#     assert set(returned) == \
+#         set(field_data.values()),
+#              '''set: %s returned: %s ''' %(field_data.values(), returned)
+
+
+@skip_if_no_network
+def test_05_cleanup():
+
+    subject.delete()
+    assert not subject.exists()
+
+
+@skip_if_no_network
+def test_06_list_project_attrs():
+
+    project_attributes = ['xnat:projectData/name',
+                          'xnat:projectData/type',
+                          'xnat:projectData/description',
+                          'xnat:projectData/keywords',
+                          'xnat:projectData/aliases',
+                          'xnat:projectData/aliases/alias',
+                          'xnat:projectData/aliases/alias/None',
+                          'xnat:projectData/publications',
+                          'xnat:projectData/publications/publication',
+                          'xnat:projectData/resources',
+                          'xnat:projectData/resources/resource',
+                          'xnat:projectData/studyProtocol',
+                          'xnat:projectData/PI',
+                          'xnat:projectData/investigators',
+                          'xnat:projectData/investigators/investigator',
+                          'xnat:projectData/fields',
+                          'xnat:projectData/fields/field',
+                          'xnat:projectData/fields/field/None']
+
+    p = central.select.project('nosetests')
+    assert(p.attrs() == [])
+
+    central.manage.schemas.add('xapi/schemas/xnat')
+    p = central.select.project('nosetests')
+    assert (p.attrs() == project_attributes)
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/custom_variables_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/custom_variables_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import os
-from uuid import uuid1
-from pyxnat import Interface
-import os.path as op
-from . import skip_if_no_network
-
-
-fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-central = Interface(config=fp)
-project = central.select.project('nosetests5')
-
-variables = {'Subjects': {'newgroup': {'foo': 'string', 'bar': 'int'}}}
-
-sid = uuid1().hex
-eid = uuid1().hex
-cid = uuid1().hex
-
-if not os.environ.get('PYXNAT_SKIP_NETWORK_TESTS'):
-    sc = project.subject(sid).experiment(eid).scan(cid)
-    scan = sc.insert(use_label=True)
-
-
-@skip_if_no_network
-def test_01_set_param():
-    scan.set_param('foo', 'foostring')
-    scan.set_param('bar', '1')
-
-    assert scan.params() == ['foo', 'bar']
-
-
-@skip_if_no_network
-def test_02_get_params():
-    assert scan.get_params() == ['foostring', '1']
-
-
-@skip_if_no_network
-def test_03_params_cleanup():
-    project.subject(sid).delete()
-    assert not project.subject(sid).exists()
-
-
-@skip_if_no_network
-def test_04_add_custom_variables():
-    project.add_custom_variables(variables)
-
-
-@skip_if_no_network
-def test_05_get_custom_variables():
-    project.get_custom_variables()
+import os
+from uuid import uuid1
+from pyxnat import Interface
+import os.path as op
+from pyxnat.tests import skip_if_no_network
+
+
+fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+central = Interface(config=fp)
+project = central.select.project('nosetests5')
+
+variables = {'Subjects': {'newgroup': {'foo': 'string', 'bar': 'int'}}}
+
+sid = uuid1().hex
+eid = uuid1().hex
+cid = uuid1().hex
+
+if not os.environ.get('PYXNAT_SKIP_NETWORK_TESTS'):
+    sc = project.subject(sid).experiment(eid).scan(cid)
+    scan = sc.insert(use_label=True)
+
+
+@skip_if_no_network
+def test_01_set_param():
+    scan.set_param('foo', 'foostring')
+    scan.set_param('bar', '1')
+
+    assert scan.params() == ['foo', 'bar']
+
+
+@skip_if_no_network
+def test_02_get_params():
+    assert scan.get_params() == ['foostring', '1']
+
+
+@skip_if_no_network
+def test_03_params_cleanup():
+    project.subject(sid).delete()
+    assert not project.subject(sid).exists()
+
+
+@skip_if_no_network
+def test_04_add_custom_variables():
+    project.add_custom_variables(variables)
+
+
+@skip_if_no_network
+def test_05_get_custom_variables():
+    project.get_custom_variables()
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/downloadutils_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/downloadutils_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from pyxnat import Interface
-from pyxnat.core import downloadutils as du
-import os.path as op
-from . import skip_if_no_network
-
-fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-central = Interface(config=fp)
-
-
-@skip_if_no_network
-def test_download():
-    s = central.select.project('CENTRAL_OASIS_LONG').subject('OAS2_0001')
-    e = s.experiment('CENTRAL_E00090')
-    du.download(dest_dir='/tmp',
-                instance=e.scans(),
-                extract=True,
-                removeZip=True)
+from pyxnat import Interface
+from pyxnat.core import downloadutils as du
+import os.path as op
+from pyxnat.tests import skip_if_no_network
+
+fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+central = Interface(config=fp)
+
+
+@skip_if_no_network
+def test_download():
+    s = central.select.project('CENTRAL_OASIS_LONG').subject('OAS2_0001')
+    e = s.experiment('CENTRAL_E00090')
+    du.download(dest_dir='/tmp',
+                instance=e.scans(),
+                extract=True,
+                removeZip=True)
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/interfaces_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/interfaces_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import os.path as op
-from pyxnat import Interface
-from . import skip_if_no_network
-
-fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-central = Interface(config=fp)
-central_anon = Interface('https://central.xnat.org', anonymous=True)
-
-
-def test_simple_object_listing():
-    assert isinstance(central.select.projects().get(), list)
-
-
-def test_simple_path_listing():
-    assert isinstance(central.select('/projects').get(), list)
-
-
-def test_nested_object_listing():
-    assert isinstance(central.select.projects('*OASIS*').subjects().get(),
-                      list)
-
-
-def test_nested_path_listing():
-    assert isinstance(central.select('/projects/*OASIS*/subjects').get(), list)
-
-
-@skip_if_no_network
-def test_search_access():
-    constraints = [('xnat:subjectData/PROJECT', '=', 'CENTRAL_OASIS_CS'),
-                   'AND']
-
-    for subject in central.select('//subjects').where(constraints):
-        assert '/projects/CENTRAL_OASIS_CS' in subject._uri
-
-
-def test_connection_with_explicit_parameters():
-    import json
-    cfg = json.load(open(fp))
-    Interface(server=cfg['server'], user=cfg['user'],
-              password=cfg['password'])
-
-
-def test_anonymous_access():
-    projects = central_anon.select.projects().get()
-    assert isinstance(projects, list)
-    assert list
-
-
-@skip_if_no_network
-def test_close_jsession():
-    config_file = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-    with Interface(config=config_file) as central:
-        assert central.select.project('nosetests').exists()
-
-
-def test_save_config():
-    central.save_config('/tmp/.xnat.cfg')
-
-
-@skip_if_no_network
-def test_version():
-    v = central.version()
-    assert(v['version'] == '1.7.5.2-SNAPSHOT')
-
-
-def test_login_using_explicit_credentials():
-    Interface(server='http://server/',
-              user='user', password='password')
+import os.path as op
+from pyxnat import Interface
+from pyxnat.tests import skip_if_no_network
+
+fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+central = Interface(config=fp)
+central_anon = Interface('https://central.xnat.org', anonymous=True)
+
+
+def test_simple_object_listing():
+    assert isinstance(central.select.projects().get(), list)
+
+
+def test_simple_path_listing():
+    assert isinstance(central.select('/projects').get(), list)
+
+
+def test_nested_object_listing():
+    assert isinstance(central.select.projects('*OASIS*').subjects().get(),
+                      list)
+
+
+def test_nested_path_listing():
+    assert isinstance(central.select('/projects/*OASIS*/subjects').get(), list)
+
+
+@skip_if_no_network
+def test_search_access():
+    constraints = [('xnat:subjectData/PROJECT', '=', 'CENTRAL_OASIS_CS'),
+                   'AND']
+
+    for subject in central.select('//subjects').where(constraints):
+        assert '/projects/CENTRAL_OASIS_CS' in subject._uri
+
+
+def test_connection_with_explicit_parameters():
+    import json
+    cfg = json.load(open(fp))
+    Interface(server=cfg['server'], user=cfg['user'],
+              password=cfg['password'])
+
+
+def test_anonymous_access():
+    projects = central_anon.select.projects().get()
+    assert isinstance(projects, list)
+    assert list
+
+
+@skip_if_no_network
+def test_close_jsession():
+    config_file = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+    with Interface(config=config_file) as central:
+        assert central.select.project('nosetests').exists()
+
+
+def test_save_config():
+    central.save_config('/tmp/.xnat.cfg')
+
+
+@skip_if_no_network
+def test_version():
+    v = central.version()
+    assert(v['version'] == '1.7.5.2-SNAPSHOT')
+
+
+def test_login_using_explicit_credentials():
+    Interface(server='http://server/',
+              user='user', password='password')
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/manage_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/manage_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import os.path as op
-from pyxnat import Interface
-from . import skip_if_no_network
-
-
-fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-central = Interface(config=fp)
-
-notified = []
-
-
-def notify(cobj, eobj):
-    notified.append(eobj)
-
-
-def test_register_callback():
-    local_notified = []
-    central.manage.register_callback(notify)
-    for element in central.select('/projects'):
-        local_notified.append(element)
-
-    assert notified == local_notified
-
-
-def test_unregister_callback():
-    central.manage.unregister_callback()
-    assert central._callback is None
-
-
-@skip_if_no_network
-def test_add_schema():
-    assert(len(central.manage.schemas()) == 0)
-    central.manage.schemas.add(url='/xapi/schemas/xnat')
-    assert(list(central.manage.schemas()) == ['xnat'])
+import os.path as op
+from pyxnat import Interface
+from pyxnat.tests import skip_if_no_network
+
+
+fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+central = Interface(config=fp)
+
+notified = []
+
+
+def notify(cobj, eobj):
+    notified.append(eobj)
+
+
+def test_register_callback():
+    local_notified = []
+    central.manage.register_callback(notify)
+    for element in central.select('/projects'):
+        local_notified.append(element)
+
+    assert notified == local_notified
+
+
+def test_unregister_callback():
+    central.manage.unregister_callback()
+    assert central._callback is None
+
+
+@skip_if_no_network
+def test_add_schema():
+    assert(len(central.manage.schemas()) == 0)
+    central.manage.schemas.add(url='/xapi/schemas/xnat')
+    assert(list(central.manage.schemas()) == ['xnat'])
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/pipelines_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/pipelines_test.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import os.path as op
-from pyxnat import Interface
-from pyxnat.core.pipelines import PipelineNotFoundError
-
-fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-central = Interface(config=fp)
-p = central.select.project('nosetests5')
-
-
-def test_pipelines_info():
-    info = p.pipelines.info('DicomToNifti')
-    assert (len(info) == 1)
-
-
-def test_pipelines_aliases():
-    aliases = p.pipelines.aliases()
-    assert (aliases == {'DicomToNifti': 'DicomToNifti'})
-
-
-def test_pipeline_info():
-    info_keys = ['appliesTo', 'authors', 'description',
-                 'inputParameters', 'path', 'steps', 'version']
-
-    pipe = p.pipelines.pipeline('DicomToNifti')
-    assert (pipe.exists())
-
-    pipe_info = pipe.info()
-    assert (int(pipe_info['version']) >= 20150114)
-    assert (sorted(pipe_info.keys()) == info_keys)
-
-
-def test_pipeline_run():
-    exp_id = 'CENTRAL02_E01603'
-
-    try:
-        wrong_pipe = p.pipelines.pipeline('INVALID_PIPELINE')
-        wrong_pipe.run(exp_id)
-    except PipelineNotFoundError as pe:
-        print(pe)
-
-    try:
-        pipe = p.pipelines.pipeline('DicomToNifti')
-        pipe.run('INVALID_EXP')
-    except ValueError as ve:
-        print(ve)
-
-    pipe = p.pipelines.pipeline('DicomToNifti')
-    pipe.run(exp_id)
-
-
-def test_pipeline_status():
-    exp_id = 'CENTRAL02_E01603'
-
-    try:
-        wrong_pipe = p.pipelines.pipeline('INVALID_PIPELINE')
-        wrong_pipe.status(exp_id)
-    except PipelineNotFoundError as pe:
-        print(pe)
-
-    try:
-        pipe = p.pipelines.pipeline('DicomToNifti')
-        pipe.status('INVALID_EXP')
-    except ValueError as ve:
-        print(ve)
-
-    pipe = p.pipelines.pipeline('DicomToNifti')
-    status = pipe.status(exp_id)
-    assert (isinstance(status, dict))
-    assert (status['status'] != 'Failed')
+import os.path as op
+from pyxnat import Interface
+from pyxnat.core.pipelines import PipelineNotFoundError
+
+fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+central = Interface(config=fp)
+p = central.select.project('nosetests5')
+
+
+def test_pipelines_info():
+    info = p.pipelines.info('DicomToNifti')
+    assert (len(info) == 1)
+
+
+def test_pipelines_aliases():
+    aliases = p.pipelines.aliases()
+    assert (aliases == {'DicomToNifti': 'DicomToNifti'})
+
+
+def test_pipeline_info():
+    info_keys = ['appliesTo', 'authors', 'description',
+                 'inputParameters', 'path', 'steps', 'version']
+
+    pipe = p.pipelines.pipeline('DicomToNifti')
+    assert (pipe.exists())
+
+    pipe_info = pipe.info()
+    assert (int(pipe_info['version']) >= 20150114)
+    assert (sorted(pipe_info.keys()) == info_keys)
+
+
+def test_pipeline_run():
+    exp_id = 'CENTRAL02_E01603'
+
+    try:
+        wrong_pipe = p.pipelines.pipeline('INVALID_PIPELINE')
+        wrong_pipe.run(exp_id)
+    except PipelineNotFoundError as pe:
+        print(pe)
+
+    try:
+        pipe = p.pipelines.pipeline('DicomToNifti')
+        pipe.run('INVALID_EXP')
+    except ValueError as ve:
+        print(ve)
+
+    pipe = p.pipelines.pipeline('DicomToNifti')
+    pipe.run(exp_id)
+
+
+def test_pipeline_status():
+    exp_id = 'CENTRAL02_E01603'
+
+    try:
+        wrong_pipe = p.pipelines.pipeline('INVALID_PIPELINE')
+        wrong_pipe.status(exp_id)
+    except PipelineNotFoundError as pe:
+        print(pe)
+
+    try:
+        pipe = p.pipelines.pipeline('DicomToNifti')
+        pipe.status('INVALID_EXP')
+    except ValueError as ve:
+        print(ve)
+
+    pipe = p.pipelines.pipeline('DicomToNifti')
+    status = pipe.status(exp_id)
+    assert (isinstance(status, dict))
+    assert (status['status'] != 'Failed')
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/provenance_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/provenance_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from uuid import uuid1
-from . import skip_if_no_network
-from pyxnat import Interface
-import os.path as op
-
-
-fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-central = Interface(config=fp)
-project = central.select.project('nosetests5')
-
-prov = {
-    'program': 'young',
-    'timestamp': '2011-03-01T12:01:01.897987',
-    'user': 'angus',
-    'machine': 'war',
-    'platform': 'linux',
-    }
-
-sid = uuid1().hex
-eid = uuid1().hex
-aid = uuid1().hex
-
-
-@skip_if_no_network
-def test_provenance():
-    assessor = project.subject(sid).experiment(eid).assessor(
-        aid).insert(use_label=True)
-    assert assessor.exists()
-    assessor.provenance.set(prov)
-    _prov = assessor.provenance.get()[0]
-
-    assert prov['program'] == _prov['program'], \
-        "Subject: %s Study: %s Prov: %s" % (sid, eid, aid)
-
-# def test_del_provenance():
-#     assessor.provenance.delete()
-#     print assessor.provenance.get()
-#     assert assessor.provenance.get()[0] == []
-
-
-@skip_if_no_network
-def test_provenance_cleanup():
-    project.subject(sid).delete()
-    assert not project.subject(sid).exists()
+from uuid import uuid1
+from pyxnat.tests import skip_if_no_network
+from pyxnat import Interface
+import os.path as op
+
+
+fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+central = Interface(config=fp)
+project = central.select.project('nosetests5')
+
+prov = {
+    'program': 'young',
+    'timestamp': '2011-03-01T12:01:01.897987',
+    'user': 'angus',
+    'machine': 'war',
+    'platform': 'linux',
+    }
+
+sid = uuid1().hex
+eid = uuid1().hex
+aid = uuid1().hex
+
+
+@skip_if_no_network
+def test_provenance():
+    assessor = project.subject(sid).experiment(eid).assessor(
+        aid).insert(use_label=True)
+    assert assessor.exists()
+    assessor.provenance.set(prov)
+    _prov = assessor.provenance.get()[0]
+
+    assert prov['program'] == _prov['program'], \
+        "Subject: %s Study: %s Prov: %s" % (sid, eid, aid)
+
+# def test_del_provenance():
+#     assessor.provenance.delete()
+#     print assessor.provenance.get()
+#     assert assessor.provenance.get()[0] == []
+
+
+@skip_if_no_network
+def test_provenance_cleanup():
+    project.subject(sid).delete()
+    assert not project.subject(sid).exists()
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/resources_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/resources_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,390 +1,390 @@
-import tempfile
-from uuid import uuid1
-from six import string_types
-import os.path as op
-import os
-from pyxnat import Interface
-from . import skip_if_no_network
-from nose import SkipTest
-from pyxnat.core import interfaces
-
-_modulepath = op.dirname(op.abspath(__file__))
-
-central = Interface(config=op.join(op.dirname(op.abspath(__file__)),
-                                   'central.cfg'))
-interfaces.STUBBORN = True
-
-_id_set1 = {
-    'sid': uuid1().hex,
-    'eid': uuid1().hex,
-    'aid': uuid1().hex,
-    'cid': uuid1().hex,
-    'rid': uuid1().hex,
-}
-
-_id_set2 = {
-    'sid': uuid1().hex,
-    'eid': uuid1().hex,
-    'aid': uuid1().hex,
-    'cid': uuid1().hex,
-    'rid': uuid1().hex,
-}
-
-subj_1 = central.select.project('nosetests5').subject(_id_set1['sid'])
-expe_1 = subj_1.experiment(_id_set1['eid'])
-asse_1 = expe_1.assessor(_id_set1['aid'])
-scan_1 = expe_1.scan(_id_set1['cid'])
-reco_1 = expe_1.reconstruction(_id_set1['rid'])
-
-
-@skip_if_no_network
-def test_01_subject_create():
-    assert not subj_1.exists()
-    subj_1.create()
-    assert subj_1.exists()
-
-
-@skip_if_no_network
-def test_02_experiment_create():
-    assert not expe_1.exists()
-    expe_1.create()
-    assert expe_1.exists()
-    expe_1.trigger(fix_types=True, pipelines=True, scan_headers=False)
-
-
-@skip_if_no_network
-def test_03_assessor_create():
-    assert not asse_1.exists()
-    asse_1.create()
-    assert asse_1.exists()
-
-
-@skip_if_no_network
-def test_04_scan_create():
-    assert not scan_1.exists()
-    scan_1.create()
-    assert scan_1.exists()
-
-
-@skip_if_no_network
-def test_05_reconstruction_create():
-    assert not reco_1.exists()
-    reco_1.create()
-    assert reco_1.exists()
-
-
-# def test_provenance():
-#     reco_1.provenance.set({'program':'nosetests'})
-#     assert reco_1.provenance.get()[0]['program'] == 'nosetests'
-
-@skip_if_no_network
-def test_06_multi_create():
-    asse_2 = central.select('/projects/nosetests5/subjects/%(sid)s'
-                            '/experiments/%(eid)s'
-                            '/assessors/%(aid)s' % _id_set2)
-
-    expe_2 = central.select('/projects/nosetests5/subjects/%(sid)s'
-                            '/experiments/%(eid)s' % _id_set2)
-
-    assert not asse_2.exists()
-    asse_2.create(experiments='xnat:petSessionData',
-                  assessors='xnat:petAssessorData')
-    assert asse_2.exists()
-
-    assert asse_2.datatype() == 'xnat:petAssessorData'
-    assert expe_2.datatype() == 'xnat:petSessionData'
-
-    scan_2 = central.select('/projects/nosetests5/subjects/%(sid)s'
-                            '/experiments/%(eid)s/scans/%(cid)s' % _id_set2
-                            ).create()
-
-    assert scan_2.datatype() == 'xnat:mrScanData'
-
-
-@skip_if_no_network
-def test_07_put_file():
-    local_path = op.join(_modulepath, 'hello_xnat.txt')
-    f = subj_1.resource('test').file('hello.txt')
-    subj_1.resource('test').file('hello.txt').put(local_path)
-    subj_1.resource('test').put([local_path])
-    assert f.exists()
-    assert int(f.size()) == os.stat(local_path).st_size
-
-
-@skip_if_no_network
-def test_08_get_file():
-    fh = subj_1.resource('test').file('hello.txt')
-
-    fpath = fh.get()
-    assert op.exists(fpath)
-    print(['toto3', open(fpath, 'rb').read()])
-    try:
-        assert open(fpath, 'rb').read() == bytes('Hello XNAT!%s' % os.linesep,
-                                                 encoding='utf8')
-    except TypeError:
-        pass
-
-    custom = op.join(tempfile.gettempdir(), uuid1().hex)
-
-    fh.get(custom)
-    assert op.exists(custom), "fpath: %s custom: %s" % (fpath, custom)
-    os.remove(custom)
-    os.remove(fpath)
-
-
-@skip_if_no_network
-def test_09_put_dir_file():
-    local_path = op.join(_modulepath, 'hello_again.txt')
-    subj_1.resource('test').file('dir/hello.txt').put(local_path)
-    assert subj_1.resource('test').file('dir/hello.txt').exists()
-    assert int(subj_1.resource('test').file('dir/hello.txt').size()) == \
-           os.stat(local_path).st_size
-
-
-@skip_if_no_network
-def test_10_get_dir_file():
-    fh = subj_1.resource('test').file('dir/hello.txt')
-
-    fpath = fh.get()
-    assert op.exists(fpath)
-    try:
-        assert open(fpath, 'rb').read() == bytes('Hello again!%s' % os.linesep,
-                                                 encoding='utf8')
-    except TypeError:
-        pass
-
-    custom = op.join(tempfile.gettempdir(), uuid1().hex)
-
-    fh.get(custom)
-    assert op.exists(custom), "fpath: %s custom: %s" % (fpath, custom)
-    os.remove(custom)
-    os.remove(fpath)
-
-
-@skip_if_no_network
-def test_11_get_copy_file():
-    fpath = op.join(tempfile.gettempdir(), uuid1().hex)
-    fpath = subj_1.resource('test').file('hello.txt').get_copy(fpath)
-    assert op.exists(fpath)
-    fd = open(fpath, 'rb')
-    try:
-        assert fd.read() == bytes('Hello XNAT!%s' % os.linesep,
-                                  encoding='utf8')
-    except TypeError:
-        pass
-    fd.close()
-    os.remove(fpath)
-
-
-@skip_if_no_network
-def test_12_file_last_modified():
-    f = subj_1.resource('test').file('hello.txt')
-    assert isinstance(f.last_modified(), string_types)
-    assert len(f.last_modified()) > 0
-    f.delete()
-    assert(not f.exists())
-    r = subj_1.resource('test')
-    r.delete()
-    assert(not r.exists())
-
-
-@skip_if_no_network
-def test_13_last_modified():
-    sid = subj_1.id()
-
-    t1 = central.select('/project/nosetests5').last_modified()[sid]
-    subj_1.attrs.set('age', '26')
-    assert subj_1.attrs.get('age') == '26'
-    t2 = central.select('/project/nosetests5').last_modified()[sid]
-
-    assert t1 != t2
-
-
-@skip_if_no_network
-def test_14_getitem_key():
-    projects = central.select.projects()
-    assert projects.first().id() == projects[0].id()
-    piter = projects.__iter__()
-    next(piter)
-    assert next(piter).id() == projects[1].id()
-
-
-@skip_if_no_network
-def test_15_getitem_slice():
-    projects = central.select.projects()
-    assert projects.first().id() == next(projects[:1]).id()
-    piter = projects.__iter__()
-    next(piter)
-    next(piter)
-    next(piter)
-    for pobj in projects[3:6]:
-        assert next(piter).id() == pobj.id()
-
-
-def test_subject1_parent():
-    project = central.select.project('nosetests5')
-    assert subj_1.parent()._uri == project._uri
-
-
-def test_project_parent():
-    project = central.select.project('nosetests5')
-    assert not project.parent()
-
-
-@skip_if_no_network
-def test_16_project_configuration():
-    project = central.select('/project/nosetests5')
-    version = central.version()
-    from pyxnat.core.errors import DatabaseError
-
-    try:
-        assert project.quarantine_code() == 0
-        assert project.prearchive_code() == 4, project.prearchive_code()
-    except DatabaseError:
-        if version['version'] == '1.7.5.2-SNAPSHOT':
-            msg = 'Version 1.7.5.2-SNAPSHOT gives trouble on some machines. \
-                   Skipping it'
-            raise SkipTest(msg)
-
-    if version['version'] != '1.7.5.2-SNAPSHOT':
-        try:
-            assert project.current_arc() == b'arc001'
-        except DatabaseError:
-            msg = 'Check if current_arc is supported in XNAT version %s.' \
-                  % version['version']
-            print(msg)
-
-    assert 'nosetests' in project.users()
-    assert 'nosetests' in project.owners()
-    assert project.user_role('nosetests') == 'owner'
-
-
-@skip_if_no_network
-def test_17_put_zip():
-    local_path = op.join(_modulepath, 'hello_dir.zip')
-    assert op.exists(local_path)
-
-    # Upload and confirm proper extraction
-    r1 = subj_1.resource('test_zip_extract')
-    r1.put_zip(local_path, extract=True)
-    assert r1.exists()
-    assert r1.file('hello_dir/hello_xnat_dir.txt').exists()
-    assert r1.file('hello_dir/hello_dir2/hello_xnat_dir2.txt').exists()
-
-    # Upload and confirm not extracted
-    r2 = subj_1.resource('test_zip_no_extract')
-    r2.put_zip(local_path, extract=False)
-    assert r2.exists()
-    assert r2.file('hello_dir.zip').exists()
-
-
-@skip_if_no_network
-def test_18_get_zip():
-    r = subj_1.resource('test_zip_extract')
-    local_dir = op.join(_modulepath, 'test_zip_download' + r.id())
-    file_list = ['test_zip_extract/hello_dir',
-                 'test_zip_extract/hello_dir/hello_xnat_dir.txt',
-                 'test_zip_extract/hello_dir/hello_dir2',
-                 'test_zip_extract/hello_dir/hello_dir2/hello_xnat_dir2.txt']
-    file_list = [op.join(local_dir, e) for e in file_list]
-
-    if not op.exists(local_dir):
-        os.mkdir(local_dir)
-
-    r.get(local_dir, extract=True)
-    for f in file_list:
-        assert op.exists(f)
-    r.get(local_dir, extract=False)
-    assert op.isfile(op.join(local_dir, 'test_zip_extract.zip'))
-
-
-@skip_if_no_network
-def test_19_project_aliases():
-    project = central.select('/project/nosetests5')
-    assert project.aliases() == ['nosetests52']
-
-
-@skip_if_no_network
-def test_20_project():
-    project = central.select.project('nosetests5')
-    project.datatype()
-    project.experiments()
-    project.experiment('nose')
-
-
-@skip_if_no_network
-def test_21_project_description():
-    project = central.select.project('nosetests5')
-    desc = project.description()
-    assert(desc == 'nosetests')
-
-
-@skip_if_no_network
-def test_22_share_subject():
-    target_project = central.select.project('metabase_nosetests')
-
-    shared_subj_1 = target_project.subject(_id_set1['sid'])
-    assert(not shared_subj_1.exists())
-    assert(subj_1.shares().get() == ['nosetests5'])
-
-    subj_1.share('metabase_nosetests')
-    shared_subj_1 = target_project.subject(_id_set1['sid'])
-    assert(shared_subj_1.exists())
-    assert(subj_1.shares().get() == ['nosetests5', 'metabase_nosetests'])
-
-
-@skip_if_no_network
-def test_23_unshare_subject():
-    target_project = central.select.project('metabase_nosetests')
-
-    shared_subj_1 = target_project.subject(_id_set1['sid'])
-    assert(shared_subj_1.exists())
-    assert(subj_1.shares().get() == ['nosetests5', 'metabase_nosetests'])
-
-    subj_1.unshare('metabase_nosetests')
-    shared_subj_1 = target_project.subject(_id_set1['sid'])
-    assert(not shared_subj_1.exists())
-    assert(subj_1.shares().get() == ['nosetests5'])
-
-
-@skip_if_no_network
-def test_24_share_experiment():
-    target_project = central.select.project('metabase_nosetests')
-
-    shared_expe_1 = target_project.experiment(_id_set1['eid'])
-    assert(not shared_expe_1.exists())
-    assert(expe_1.shares().get() == ['nosetests5'])
-
-    expe_1.share('metabase_nosetests')
-    shared_expe_1 = target_project.experiment(_id_set1['eid'])
-    assert(shared_expe_1.exists())
-    assert(expe_1.shares().get() == ['nosetests5', 'metabase_nosetests'])
-
-
-@skip_if_no_network
-def test_25_unshare_experiment():
-    target_project = central.select.project('metabase_nosetests')
-
-    shared_expe_1 = target_project.experiment(_id_set1['eid'])
-    assert(shared_expe_1.exists())
-    assert(expe_1.shares().get() == ['nosetests5', 'metabase_nosetests'])
-
-    expe_1.unshare('metabase_nosetests')
-    shared_expe_1 = target_project.experiment(_id_set1['eid'])
-    assert(not shared_expe_1.exists())
-    assert(expe_1.shares().get() == ['nosetests5'])
-
-
-@skip_if_no_network
-def test_26_subject1_delete():
-    assert subj_1.exists()
-    subj_1.delete()
-    assert not subj_1.exists()
-
-
-@skip_if_no_network
-def test_27_subject2_delete():
-    subj_2 = central.select('/projects/nosetests5/subjects/%(sid)s' % _id_set2)
-    assert subj_2.exists()
-    subj_2.delete()
-    assert not subj_2.exists()
+import tempfile
+from uuid import uuid1
+from six import string_types
+import os.path as op
+import os
+from pyxnat import Interface
+from pyxnat.tests import skip_if_no_network
+import pytest
+from pyxnat.core import interfaces
+
+_modulepath = op.dirname(op.abspath(__file__))
+
+central = Interface(config=op.join(op.dirname(op.abspath(__file__)),
+                                   'central.cfg'))
+interfaces.STUBBORN = True
+
+_id_set1 = {
+    'sid': uuid1().hex,
+    'eid': uuid1().hex,
+    'aid': uuid1().hex,
+    'cid': uuid1().hex,
+    'rid': uuid1().hex,
+}
+
+_id_set2 = {
+    'sid': uuid1().hex,
+    'eid': uuid1().hex,
+    'aid': uuid1().hex,
+    'cid': uuid1().hex,
+    'rid': uuid1().hex,
+}
+
+subj_1 = central.select.project('nosetests5').subject(_id_set1['sid'])
+expe_1 = subj_1.experiment(_id_set1['eid'])
+asse_1 = expe_1.assessor(_id_set1['aid'])
+scan_1 = expe_1.scan(_id_set1['cid'])
+reco_1 = expe_1.reconstruction(_id_set1['rid'])
+
+
+@skip_if_no_network
+def test_01_subject_create():
+    assert not subj_1.exists()
+    subj_1.create()
+    assert subj_1.exists()
+
+
+@skip_if_no_network
+def test_02_experiment_create():
+    assert not expe_1.exists()
+    expe_1.create()
+    assert expe_1.exists()
+    expe_1.trigger(fix_types=True, pipelines=True, scan_headers=False)
+
+
+@skip_if_no_network
+def test_03_assessor_create():
+    assert not asse_1.exists()
+    asse_1.create()
+    assert asse_1.exists()
+
+
+@skip_if_no_network
+def test_04_scan_create():
+    assert not scan_1.exists()
+    scan_1.create()
+    assert scan_1.exists()
+
+
+@skip_if_no_network
+def test_05_reconstruction_create():
+    assert not reco_1.exists()
+    reco_1.create()
+    assert reco_1.exists()
+
+
+# def test_provenance():
+#     reco_1.provenance.set({'program':'nosetests'})
+#     assert reco_1.provenance.get()[0]['program'] == 'nosetests'
+
+@skip_if_no_network
+def test_06_multi_create():
+    asse_2 = central.select('/projects/nosetests5/subjects/%(sid)s'
+                            '/experiments/%(eid)s'
+                            '/assessors/%(aid)s' % _id_set2)
+
+    expe_2 = central.select('/projects/nosetests5/subjects/%(sid)s'
+                            '/experiments/%(eid)s' % _id_set2)
+
+    assert not asse_2.exists()
+    asse_2.create(experiments='xnat:petSessionData',
+                  assessors='xnat:petAssessorData')
+    assert asse_2.exists()
+
+    assert asse_2.datatype() == 'xnat:petAssessorData'
+    assert expe_2.datatype() == 'xnat:petSessionData'
+
+    scan_2 = central.select('/projects/nosetests5/subjects/%(sid)s'
+                            '/experiments/%(eid)s/scans/%(cid)s' % _id_set2
+                            ).create()
+
+    assert scan_2.datatype() == 'xnat:mrScanData'
+
+
+@skip_if_no_network
+def test_07_put_file():
+    local_path = op.join(_modulepath, 'hello_xnat.txt')
+    f = subj_1.resource('test').file('hello.txt')
+    subj_1.resource('test').file('hello.txt').put(local_path)
+    subj_1.resource('test').put([local_path])
+    assert f.exists()
+    assert int(f.size()) == os.stat(local_path).st_size
+
+
+@skip_if_no_network
+def test_08_get_file():
+    fh = subj_1.resource('test').file('hello.txt')
+
+    fpath = fh.get()
+    assert op.exists(fpath)
+    print(['toto3', open(fpath, 'rb').read()])
+    try:
+        assert open(fpath, 'rb').read() == bytes('Hello XNAT!%s' % os.linesep,
+                                                 encoding='utf8')
+    except TypeError:
+        pass
+
+    custom = op.join(tempfile.gettempdir(), uuid1().hex)
+
+    fh.get(custom)
+    assert op.exists(custom), "fpath: %s custom: %s" % (fpath, custom)
+    os.remove(custom)
+    os.remove(fpath)
+
+
+@skip_if_no_network
+def test_09_put_dir_file():
+    local_path = op.join(_modulepath, 'hello_again.txt')
+    subj_1.resource('test').file('dir/hello.txt').put(local_path)
+    assert subj_1.resource('test').file('dir/hello.txt').exists()
+    assert int(subj_1.resource('test').file('dir/hello.txt').size()) == \
+           os.stat(local_path).st_size
+
+
+@skip_if_no_network
+def test_10_get_dir_file():
+    fh = subj_1.resource('test').file('dir/hello.txt')
+
+    fpath = fh.get()
+    assert op.exists(fpath)
+    try:
+        assert open(fpath, 'rb').read() == bytes('Hello again!%s' % os.linesep,
+                                                 encoding='utf8')
+    except TypeError:
+        pass
+
+    custom = op.join(tempfile.gettempdir(), uuid1().hex)
+
+    fh.get(custom)
+    assert op.exists(custom), "fpath: %s custom: %s" % (fpath, custom)
+    os.remove(custom)
+    os.remove(fpath)
+
+
+@skip_if_no_network
+def test_11_get_copy_file():
+    fpath = op.join(tempfile.gettempdir(), uuid1().hex)
+    fpath = subj_1.resource('test').file('hello.txt').get_copy(fpath)
+    assert op.exists(fpath)
+    fd = open(fpath, 'rb')
+    try:
+        assert fd.read() == bytes('Hello XNAT!%s' % os.linesep,
+                                  encoding='utf8')
+    except TypeError:
+        pass
+    fd.close()
+    os.remove(fpath)
+
+
+@skip_if_no_network
+def test_12_file_last_modified():
+    f = subj_1.resource('test').file('hello.txt')
+    assert isinstance(f.last_modified(), string_types)
+    assert len(f.last_modified()) > 0
+    f.delete()
+    assert(not f.exists())
+    r = subj_1.resource('test')
+    r.delete()
+    assert(not r.exists())
+
+
+@skip_if_no_network
+def test_13_last_modified():
+    sid = subj_1.id()
+
+    t1 = central.select('/project/nosetests5').last_modified()[sid]
+    subj_1.attrs.set('age', '26')
+    assert subj_1.attrs.get('age') == '26'
+    t2 = central.select('/project/nosetests5').last_modified()[sid]
+
+    assert t1 != t2
+
+
+@skip_if_no_network
+def test_14_getitem_key():
+    projects = central.select.projects()
+    assert projects.first().id() == projects[0].id()
+    piter = projects.__iter__()
+    next(piter)
+    assert next(piter).id() == projects[1].id()
+
+
+@skip_if_no_network
+def test_15_getitem_slice():
+    projects = central.select.projects()
+    assert projects.first().id() == next(projects[:1]).id()
+    piter = projects.__iter__()
+    next(piter)
+    next(piter)
+    next(piter)
+    for pobj in projects[3:6]:
+        assert next(piter).id() == pobj.id()
+
+
+def test_subject1_parent():
+    project = central.select.project('nosetests5')
+    assert subj_1.parent()._uri == project._uri
+
+
+def test_project_parent():
+    project = central.select.project('nosetests5')
+    assert not project.parent()
+
+
+@skip_if_no_network
+def test_16_project_configuration():
+    project = central.select('/project/nosetests5')
+    version = central.version()
+    from pyxnat.core.errors import DatabaseError
+
+    try:
+        assert project.quarantine_code() == 0
+        assert project.prearchive_code() == 4, project.prearchive_code()
+    except DatabaseError:
+        if version['version'] == '1.7.5.2-SNAPSHOT':
+            msg = 'Version 1.7.5.2-SNAPSHOT gives trouble on some machines. \
+                   Skipping it'
+            pytest.skip(msg)
+
+    if version['version'] != '1.7.5.2-SNAPSHOT':
+        try:
+            assert project.current_arc() == b'arc001'
+        except DatabaseError:
+            msg = 'Check if current_arc is supported in XNAT version %s.' \
+                  % version['version']
+            print(msg)
+
+    assert 'nosetests' in project.users()
+    assert 'nosetests' in project.owners()
+    assert project.user_role('nosetests') == 'owner'
+
+
+@skip_if_no_network
+def test_17_put_zip():
+    local_path = op.join(_modulepath, 'hello_dir.zip')
+    assert op.exists(local_path)
+
+    # Upload and confirm proper extraction
+    r1 = subj_1.resource('test_zip_extract')
+    r1.put_zip(local_path, extract=True)
+    assert r1.exists()
+    assert r1.file('hello_dir/hello_xnat_dir.txt').exists()
+    assert r1.file('hello_dir/hello_dir2/hello_xnat_dir2.txt').exists()
+
+    # Upload and confirm not extracted
+    r2 = subj_1.resource('test_zip_no_extract')
+    r2.put_zip(local_path, extract=False)
+    assert r2.exists()
+    assert r2.file('hello_dir.zip').exists()
+
+
+@skip_if_no_network
+def test_18_get_zip():
+    r = subj_1.resource('test_zip_extract')
+    local_dir = op.join(_modulepath, 'test_zip_download' + r.id())
+    file_list = ['test_zip_extract/hello_dir',
+                 'test_zip_extract/hello_dir/hello_xnat_dir.txt',
+                 'test_zip_extract/hello_dir/hello_dir2',
+                 'test_zip_extract/hello_dir/hello_dir2/hello_xnat_dir2.txt']
+    file_list = [op.join(local_dir, e) for e in file_list]
+
+    if not op.exists(local_dir):
+        os.mkdir(local_dir)
+
+    r.get(local_dir, extract=True)
+    for f in file_list:
+        assert op.exists(f)
+    r.get(local_dir, extract=False)
+    assert op.isfile(op.join(local_dir, 'test_zip_extract.zip'))
+
+
+@skip_if_no_network
+def test_19_project_aliases():
+    project = central.select('/project/nosetests5')
+    assert project.aliases() == ['nosetests52']
+
+
+@skip_if_no_network
+def test_20_project():
+    project = central.select.project('nosetests5')
+    project.datatype()
+    project.experiments()
+    project.experiment('nose')
+
+
+@skip_if_no_network
+def test_21_project_description():
+    project = central.select.project('nosetests5')
+    desc = project.description()
+    assert(desc == 'nosetests')
+
+
+@skip_if_no_network
+def test_22_share_subject():
+    target_project = central.select.project('metabase_nosetests')
+
+    shared_subj_1 = target_project.subject(_id_set1['sid'])
+    assert(not shared_subj_1.exists())
+    assert(subj_1.shares().get() == ['nosetests5'])
+
+    subj_1.share('metabase_nosetests')
+    shared_subj_1 = target_project.subject(_id_set1['sid'])
+    assert(shared_subj_1.exists())
+    assert(subj_1.shares().get() == ['nosetests5', 'metabase_nosetests'])
+
+
+@skip_if_no_network
+def test_23_unshare_subject():
+    target_project = central.select.project('metabase_nosetests')
+
+    shared_subj_1 = target_project.subject(_id_set1['sid'])
+    assert(shared_subj_1.exists())
+    assert(subj_1.shares().get() == ['nosetests5', 'metabase_nosetests'])
+
+    subj_1.unshare('metabase_nosetests')
+    shared_subj_1 = target_project.subject(_id_set1['sid'])
+    assert(not shared_subj_1.exists())
+    assert(subj_1.shares().get() == ['nosetests5'])
+
+
+@skip_if_no_network
+def test_24_share_experiment():
+    target_project = central.select.project('metabase_nosetests')
+
+    shared_expe_1 = target_project.experiment(_id_set1['eid'])
+    assert(not shared_expe_1.exists())
+    assert(expe_1.shares().get() == ['nosetests5'])
+
+    expe_1.share('metabase_nosetests')
+    shared_expe_1 = target_project.experiment(_id_set1['eid'])
+    assert(shared_expe_1.exists())
+    assert(expe_1.shares().get() == ['nosetests5', 'metabase_nosetests'])
+
+
+@skip_if_no_network
+def test_25_unshare_experiment():
+    target_project = central.select.project('metabase_nosetests')
+
+    shared_expe_1 = target_project.experiment(_id_set1['eid'])
+    assert(shared_expe_1.exists())
+    assert(expe_1.shares().get() == ['nosetests5', 'metabase_nosetests'])
+
+    expe_1.unshare('metabase_nosetests')
+    shared_expe_1 = target_project.experiment(_id_set1['eid'])
+    assert(not shared_expe_1.exists())
+    assert(expe_1.shares().get() == ['nosetests5'])
+
+
+@skip_if_no_network
+def test_26_subject1_delete():
+    assert subj_1.exists()
+    subj_1.delete()
+    assert not subj_1.exists()
+
+
+@skip_if_no_network
+def test_27_subject2_delete():
+    subj_2 = central.select('/projects/nosetests5/subjects/%(sid)s' % _id_set2)
+    assert subj_2.exists()
+    subj_2.delete()
+    assert not subj_2.exists()
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/scans_tests.py` & `bbrc-pyxnat-1.6/pyxnat/tests/scans_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from pyxnat import Interface
-import os.path as op
-from . import skip_if_no_network
-
-
-_modulepath = op.dirname(op.abspath(__file__))
-
-fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-central = Interface(config=fp)
-
-
-@skip_if_no_network
-def test_global_scan_listing():
-    assert central.array.scans(project_id='CENTRAL_OASIS_CS',
-                               experiment_type='xnat:mrSessionData',
-                               scan_type='xnat:mrScanData'
-                               )
+from pyxnat import Interface
+import os.path as op
+from pyxnat.tests import skip_if_no_network
+
+
+_modulepath = op.dirname(op.abspath(__file__))
+
+fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+central = Interface(config=fp)
+
+
+@skip_if_no_network
+def test_global_scan_listing():
+    assert central.array.scans(project_id='CENTRAL_OASIS_CS',
+                               experiment_type='xnat:mrSessionData',
+                               scan_type='xnat:mrScanData'
+                               )
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/select_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/select_test.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from pyxnat import select
-
-
-def test_switch_to_singular():
-    assert select.compute('/projects/nosetests') == ['/project/nosetests']
-
-
-def test_switch_to_plural():
-    assert select.compute('/project') == ['/projects/*']
-
-
-def test_complete_stars_plural():
-    assert select.compute('/projects/subjects/experiments') == \
-           ['/projects/*/subjects/*/experiments/*']
-
-
-def test_complete_stars_singular():
-    assert select.compute('/project/subject/experiment') == \
-           ['/projects/*/subjects/*/experiments/*']
-
-
-def test_simple_root_expand():
-    assert select.compute('//experiments') == \
-           ['/projects/*/subjects/*/experiments/*']
-
-
-def test_simple_level_expand():
-    assert select.compute('/projects/IMAGEN//experiments') == \
-           ['/project/IMAGEN/subjects/*/experiments/*']
-
-
-def test_leaf_level_expand():
-    assert set(select.compute('//files')) == \
-        set(['/projects/*/subjects/*/experiments/*/resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/reconstructions/*/in_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/scans/*/resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/out_resources/*/files/*',
-             '/projects/*/subjects/*/resources/*/files/*',
-             '/projects/*/resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/reconstructions/*/out_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/in_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/resources/*/files/*'])
-
-
-def test_double_level_expand():
-    assert set(select.compute('//experiments//files')) == \
-        set(['/projects/*/subjects/*/experiments/*/resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/reconstructions/*/in_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/scans/*/resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/out_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/in_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/reconstructions/*/out_resources/*/files/*',
-             '/projects/*/subjects/*/experiments/*/assessors/*/resources/*/files/*'])
-
-
-def test_compute_all():
-    assert set(select.compute('/projects/nosetests//experiments/*Session*//files/myfile.txt')) == \
-        set(['/project/nosetests/subjects/*/experiments/*Session*/resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/reconstructions/*/in_resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/scans/*/resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/out_resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/in_resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/reconstructions/*/out_resources/*/file/myfile.txt',
-             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/resources/*/file/myfile.txt'])
+from pyxnat import select
+
+
+def test_switch_to_singular():
+    assert select.compute('/projects/nosetests') == ['/project/nosetests']
+
+
+def test_switch_to_plural():
+    assert select.compute('/project') == ['/projects/*']
+
+
+def test_complete_stars_plural():
+    assert select.compute('/projects/subjects/experiments') == \
+           ['/projects/*/subjects/*/experiments/*']
+
+
+def test_complete_stars_singular():
+    assert select.compute('/project/subject/experiment') == \
+           ['/projects/*/subjects/*/experiments/*']
+
+
+def test_simple_root_expand():
+    assert select.compute('//experiments') == \
+           ['/projects/*/subjects/*/experiments/*']
+
+
+def test_simple_level_expand():
+    assert select.compute('/projects/IMAGEN//experiments') == \
+           ['/project/IMAGEN/subjects/*/experiments/*']
+
+
+def test_leaf_level_expand():
+    assert set(select.compute('//files')) == \
+        set(['/projects/*/subjects/*/experiments/*/resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/reconstructions/*/in_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/scans/*/resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/out_resources/*/files/*',
+             '/projects/*/subjects/*/resources/*/files/*',
+             '/projects/*/resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/reconstructions/*/out_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/in_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/resources/*/files/*'])
+
+
+def test_double_level_expand():
+    assert set(select.compute('//experiments//files')) == \
+        set(['/projects/*/subjects/*/experiments/*/resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/reconstructions/*/in_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/scans/*/resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/out_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/in_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/reconstructions/*/out_resources/*/files/*',
+             '/projects/*/subjects/*/experiments/*/assessors/*/resources/*/files/*'])
+
+
+def test_compute_all():
+    assert set(select.compute('/projects/nosetests//experiments/*Session*//files/myfile.txt')) == \
+        set(['/project/nosetests/subjects/*/experiments/*Session*/resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/reconstructions/*/in_resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/scans/*/resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/out_resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/in_resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/reconstructions/*/out_resources/*/file/myfile.txt',
+             '/project/nosetests/subjects/*/experiments/*Session*/assessors/*/resources/*/file/myfile.txt'])
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/sessionmirror_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/sessionmirror_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import sys
-import os.path as op
-import pyxnat
-from . import skip_if_no_network
-
-_modulepath = op.dirname(op.abspath(pyxnat.__file__))
-dd = op.join(op.split(_modulepath)[0], 'bin')
-sys.path.append(dd)
-
-cfg = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-central = pyxnat.Interface(config=cfg)
-
-src_project = 'nosetests5'
-dest_project = 'testing_new'
-
-
-@skip_if_no_network
-def test_001_sessionmirror():
-    from sessionmirror import create_parser, main, subj_compare
-    e = 'CENTRAL02_E01892'
-    parser = create_parser()
-    args = ['--h1', cfg, '--h2', cfg, '-e', e, '-p', dest_project]
-    args = parser.parse_args(args)
-    main(args)
-
-    cols = ['label', 'subject_label']
-    data = central.array.experiments(experiment_id=e, columns=cols).data[0]
-    s1 = central.select.project(src_project).subject(data['subject_label'])
-    s2 = central.select.project(dest_project).subject(data['subject_label'])
-    assert(subj_compare(s1, s2) == 0)
-
-
-@skip_if_no_network
-def test_002_delete_experiment():
-    print('DELETING')
-    e = 'CENTRAL02_E01892'
-    cols = ['subject_label', 'label']
-    e0 = central.array.experiments(experiment_id=e, columns=cols).data[0]
-    subject_label = e0['subject_label']
-    experiment_label = e0['label']
-    e1 = central.array.experiments(project_id=dest_project,
-                                   subject_label=subject_label,
-                                   experiment_label=experiment_label,
-                                   columns=['subject_id']).data[0]
-    p = central.select.project(dest_project)
-    e2 = p.subject(e1['subject_ID']).experiment(e1['ID'])
-    assert(e2.exists())
-    e2.delete()
-    assert(not e2.exists())
-
+import sys
+import os.path as op
+import pyxnat
+from pyxnat.tests import skip_if_no_network
+
+_modulepath = op.dirname(op.abspath(pyxnat.__file__))
+dd = op.join(op.split(_modulepath)[0], 'bin')
+sys.path.append(dd)
+
+cfg = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+central = pyxnat.Interface(config=cfg)
+
+src_project = 'nosetests5'
+dest_project = 'testing_new'
+
+
+@skip_if_no_network
+def test_001_sessionmirror():
+    from sessionmirror import create_parser, main, subj_compare
+    e = 'CENTRAL02_E01892'
+    parser = create_parser()
+    args = ['--h1', cfg, '--h2', cfg, '-e', e, '-p', dest_project]
+    args = parser.parse_args(args)
+    main(args)
+
+    cols = ['label', 'subject_label']
+    data = central.array.experiments(experiment_id=e, columns=cols).data[0]
+    s1 = central.select.project(src_project).subject(data['subject_label'])
+    s2 = central.select.project(dest_project).subject(data['subject_label'])
+    assert(subj_compare(s1, s2) == 0)
+
+
+@skip_if_no_network
+def test_002_delete_experiment():
+    print('DELETING')
+    e = 'CENTRAL02_E01892'
+    cols = ['subject_label', 'label']
+    e0 = central.array.experiments(experiment_id=e, columns=cols).data[0]
+    subject_label = e0['subject_label']
+    experiment_label = e0['label']
+    e1 = central.array.experiments(project_id=dest_project,
+                                   subject_label=subject_label,
+                                   experiment_label=experiment_label,
+                                   columns=['subject_id']).data[0]
+    p = central.select.project(dest_project)
+    e2 = p.subject(e1['subject_ID']).experiment(e1['ID'])
+    assert(e2.exists())
+    e2.delete()
+    assert(not e2.exists())
+
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/uriutil_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/uriutil_test.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from pyxnat import uriutil
-
-
-def test_translate_uri():
-    assert uriutil.translate_uri('/assessors/out_resources/files') == \
-           '/assessors/out/resources/files'
-    assert uriutil.translate_uri('/assessors/out_resource/files') == \
-           '/assessors/out/resource/files'
-    assert uriutil.translate_uri('/assessors/in_resources/files') == \
-           '/assessors/in/resources/files'
-    assert uriutil.translate_uri('/assessors/in_resource/files') == \
-           '/assessors/in/resource/files'
-
-
-def test_inv_translate_uri():
-    assert uriutil.inv_translate_uri('/assessors/out/resources/files') == \
-           '/assessors/out_resources/files'
-    assert uriutil.inv_translate_uri('/assessors/out/resource/files') == \
-           '/assessors/out_resource/files'
-    assert uriutil.inv_translate_uri('/assessors/in/resources/files') == \
-           '/assessors/in_resources/files'
-    assert uriutil.inv_translate_uri('/assessors/in/resource/files') == \
-           '/assessors/in_resource/files'
-
-
-def test_join_uri():
-    uri = uriutil.join_uri('/projects', 'project_id', 'subjects', 'subject_id')
-    assert uri == '/projects/project_id/subjects/subject_id'
-
-
-def test_uri_last():
-    assert uriutil.uri_last('/projects/1/subjects/2') == '2'
-
-
-def test_uri_nextlast():
-    assert uriutil.uri_nextlast('/projects/1/subjects/2') == 'subjects'
-
-
-def test_uri_parent():
-    uri = uriutil.uri_parent('/projects/1/subjects/2')
-    assert uri == '/projects/1/subjects'
-
-
-def test_uri_grandparent():
-    uri = uriutil.uri_grandparent('/projects/1/subjects/2')
-    assert uri == '/projects/1'
-
-
-def test_uri_split():
-    uri = uriutil.uri_split('/projects/1/subjects/2')
-    assert uri == ['/projects/1/subjects', '2']
+from pyxnat import uriutil
+
+
+def test_translate_uri():
+    assert uriutil.translate_uri('/assessors/out_resources/files') == \
+           '/assessors/out/resources/files'
+    assert uriutil.translate_uri('/assessors/out_resource/files') == \
+           '/assessors/out/resource/files'
+    assert uriutil.translate_uri('/assessors/in_resources/files') == \
+           '/assessors/in/resources/files'
+    assert uriutil.translate_uri('/assessors/in_resource/files') == \
+           '/assessors/in/resource/files'
+
+
+def test_inv_translate_uri():
+    assert uriutil.inv_translate_uri('/assessors/out/resources/files') == \
+           '/assessors/out_resources/files'
+    assert uriutil.inv_translate_uri('/assessors/out/resource/files') == \
+           '/assessors/out_resource/files'
+    assert uriutil.inv_translate_uri('/assessors/in/resources/files') == \
+           '/assessors/in_resources/files'
+    assert uriutil.inv_translate_uri('/assessors/in/resource/files') == \
+           '/assessors/in_resource/files'
+
+
+def test_join_uri():
+    uri = uriutil.join_uri('/projects', 'project_id', 'subjects', 'subject_id')
+    assert uri == '/projects/project_id/subjects/subject_id'
+
+
+def test_uri_last():
+    assert uriutil.uri_last('/projects/1/subjects/2') == '2'
+
+
+def test_uri_nextlast():
+    assert uriutil.uri_nextlast('/projects/1/subjects/2') == 'subjects'
+
+
+def test_uri_parent():
+    uri = uriutil.uri_parent('/projects/1/subjects/2')
+    assert uri == '/projects/1/subjects'
+
+
+def test_uri_grandparent():
+    uri = uriutil.uri_grandparent('/projects/1/subjects/2')
+    assert uri == '/projects/1'
+
+
+def test_uri_split():
+    uri = uriutil.uri_split('/projects/1/subjects/2')
+    assert uri == ['/projects/1/subjects', '2']
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/xpass_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/xpass_test.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from pyxnat import xpass
-
-
-def test_find_plus_line():
-    print("Testing find_plus_line")
-    test = ['hello', '+hello world', '']
-    assert(xpass.find_plus_line(test) == 'hello world')
-    test2 = ['', 'hello world']
-    assert(xpass.find_plus_line(test2) is None)
-    test3 = []
-    assert(xpass.find_plus_line(test3) is None)
-
-
-def test_find_token():
-    print("Testing find_token")
-    str = "hello,world"
-    assert(xpass.find_token(',', str) == ('hello', 'world'))
-    assert(xpass.find_token(' ', str) is None)
-
-
-def test_parse_xnat_pass():
-    print("Testing parse_xnat_pass")
-    nothingLine = ""
-    line = "+user@localhost:8080/xnat=password"
-    lineWithSpaces = "+user@localhost:8080/xnat=password     "
-    lineWithoutPlus = "user@localhost:8080/xnat=password"
-    lineWithoutUser = "+@localhost:8080/xnat=password"
-    lineWithoutHost = "+user=password"
-    lineWithoutPass = "+user@localhost:8080/xnat"
-    xp = xpass.parse_xnat_pass([nothingLine, line])
-    assert(xp == {'p': 'password', 'host': 'localhost:8080/xnat', 'u': 'user'})
-    xp = xpass.parse_xnat_pass([lineWithSpaces])
-    assert(xp == {'p': 'password', 'host': 'localhost:8080/xnat', 'u': 'user'})
-    assert(xpass.parse_xnat_pass([lineWithoutPlus]) is None)
-    assert(xpass.parse_xnat_pass([lineWithoutUser]) is None)
-    assert(xpass.parse_xnat_pass([lineWithoutHost]) is None)
-    assert(xpass.parse_xnat_pass([lineWithoutPass]) is None)
+from pyxnat import xpass
+
+
+def test_find_plus_line():
+    print("Testing find_plus_line")
+    test = ['hello', '+hello world', '']
+    assert(xpass.find_plus_line(test) == 'hello world')
+    test2 = ['', 'hello world']
+    assert(xpass.find_plus_line(test2) is None)
+    test3 = []
+    assert(xpass.find_plus_line(test3) is None)
+
+
+def test_find_token():
+    print("Testing find_token")
+    str = "hello,world"
+    assert(xpass.find_token(',', str) == ('hello', 'world'))
+    assert(xpass.find_token(' ', str) is None)
+
+
+def test_parse_xnat_pass():
+    print("Testing parse_xnat_pass")
+    nothingLine = ""
+    line = "+user@localhost:8080/xnat=password"
+    lineWithSpaces = "+user@localhost:8080/xnat=password     "
+    lineWithoutPlus = "user@localhost:8080/xnat=password"
+    lineWithoutUser = "+@localhost:8080/xnat=password"
+    lineWithoutHost = "+user=password"
+    lineWithoutPass = "+user@localhost:8080/xnat"
+    xp = xpass.parse_xnat_pass([nothingLine, line])
+    assert(xp == {'p': 'password', 'host': 'localhost:8080/xnat', 'u': 'user'})
+    xp = xpass.parse_xnat_pass([lineWithSpaces])
+    assert(xp == {'p': 'password', 'host': 'localhost:8080/xnat', 'u': 'user'})
+    assert(xpass.parse_xnat_pass([lineWithoutPlus]) is None)
+    assert(xpass.parse_xnat_pass([lineWithoutUser]) is None)
+    assert(xpass.parse_xnat_pass([lineWithoutHost]) is None)
+    assert(xpass.parse_xnat_pass([lineWithoutPass]) is None)
```

### Comparing `bbrc-pyxnat-1.5.1/pyxnat/tests/xpath_test.py` & `bbrc-pyxnat-1.6/pyxnat/tests/xpath_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import os.path as op
-from pyxnat import Interface
-from . import skip_if_no_network
-
-fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
-central = Interface(config=fp)
-
-
-@skip_if_no_network
-def test_001_xpath_checkout():
-    central.xpath.checkout(subjects=['OAS1_0001', 'OAS1_0002'])
-    assert 'OAS1_0001' in central.xpath.subjects() and \
-        'OAS1_0002' in central.xpath.subjects()
-
-
-@skip_if_no_network
-def test_elements():
-    assert 'fs:region' in central.xpath.elements()
-
-
-@skip_if_no_network
-def test_keys():
-    assert 'ID' in central.xpath.keys()
-
-
-@skip_if_no_network
-def test_values():
-    assert 'OAS1_0002' in central.xpath.values('ID')
-
-
-@skip_if_no_network
-def test_element_attrs():
-    assert isinstance(central.xpath.element_attrs('fs:region'), list)
-
-    assert set(['SegId', 'hemisphere', 'name']).issubset(
-        central.xpath.element_keys('fs:region'))
-
-    assert 'Left-Putamen' in \
-        central.xpath.element_values('fs:region', 'name')
+import os.path as op
+from pyxnat import Interface
+from pyxnat.tests import skip_if_no_network
+
+fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
+central = Interface(config=fp)
+
+
+@skip_if_no_network
+def test_001_xpath_checkout():
+    central.xpath.checkout(subjects=['OAS1_0001', 'OAS1_0002'])
+    assert 'OAS1_0001' in central.xpath.subjects() and \
+        'OAS1_0002' in central.xpath.subjects()
+
+
+@skip_if_no_network
+def test_elements():
+    assert 'fs:region' in central.xpath.elements()
+
+
+@skip_if_no_network
+def test_keys():
+    assert 'ID' in central.xpath.keys()
+
+
+@skip_if_no_network
+def test_values():
+    assert 'OAS1_0002' in central.xpath.values('ID')
+
+
+@skip_if_no_network
+def test_element_attrs():
+    assert isinstance(central.xpath.element_attrs('fs:region'), list)
+
+    assert set(['SegId', 'hemisphere', 'name']).issubset(
+        central.xpath.element_keys('fs:region'))
+
+    assert 'Left-Putamen' in \
+        central.xpath.element_values('fs:region', 'name')
```

### Comparing `bbrc-pyxnat-1.5.1/setup.py` & `bbrc-pyxnat-1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-#!/usr/bin/env python
-
-import setuptools
-import os.path as op
-
-
-def get_version():
-    try:
-        import re
-        import os.path as op
-        fp = op.join(op.dirname(__file__), 'pyxnat', 'version.py')
-        s = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format('VERSION'),
-                      open(fp).read())
-        return s.group(1)
-    except Exception:
-        raise RuntimeError("No version found")
-
-
-this_directory = op.abspath(op.dirname(__file__))
-with open(op.join(this_directory, 'README.rst')) as f:
-    long_description = f.read()
-
-
-setuptools.setup(name='bbrc-pyxnat',
-                 version=get_version(),
-                 summary='XNAT in Python',
-                 author='Yannick Schwartz',
-                 author_email='yannick.schwartz@cea.fr',
-                 url='https://github.com/pyxnat/pyxnat',
-                 packages=setuptools.find_packages(exclude=('doc*', 'tests')),
-                 description='XNAT in Python',
-                 long_description=long_description,
-                 long_description_content_type='text/x-rst',
-                 license='BSD',
-                 classifiers=[
-                      'Development Status :: 4 - Beta',
-                      'Environment :: Console',
-                      'Intended Audience :: Developers',
-                      'Intended Audience :: Science/Research',
-                      'Intended Audience :: Education',
-                      'License :: OSI Approved :: BSD License',
-                      'Operating System :: OS Independent',
-                      'Topic :: Scientific/Engineering',
-                      'Topic :: Utilities',
-                      'Topic :: Internet :: WWW/HTTP',
-                      'Programming Language :: Python :: 3.7',
-                      'Programming Language :: Python :: 3.8',
-                 ],
-
-                 platforms='any',
-                 scripts=['bin/sessionmirror.py'],
-                 install_requires=['lxml>=4.3',
-                                   'requests>=2.20',
-                                   'pathlib>=1.0',
-                                   'six>=1.15',
-                                   'future>=0.16',
-                                   'pandas>=0.24',
-                                   'pymupdf>=1.18',
-                                   'pydicom',
-                                   'nibabel>=3.1'],
-                 package_data={'pyxnat': ['README.rst'], },
-
-                 )
+#!/usr/bin/env python
+
+import setuptools
+import os.path as op
+
+
+def get_version():
+    try:
+        import re
+        import os.path as op
+        fp = op.join(op.dirname(__file__), 'pyxnat', 'version.py')
+        s = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format('VERSION'),
+                      open(fp).read())
+        return s.group(1)
+    except Exception:
+        raise RuntimeError("No version found")
+
+
+this_directory = op.abspath(op.dirname(__file__))
+with open(op.join(this_directory, 'README.rst')) as f:
+    long_description = f.read()
+
+
+setuptools.setup(name='bbrc-pyxnat',
+                 version=get_version(),
+                 summary='XNAT in Python',
+                 author='Yannick Schwartz',
+                 author_email='yannick.schwartz@cea.fr',
+                 url='https://github.com/pyxnat/pyxnat',
+                 packages=setuptools.find_packages(exclude=('doc*', 'tests')),
+                 description='XNAT in Python',
+                 long_description=long_description,
+                 long_description_content_type='text/x-rst',
+                 license='BSD',
+                 classifiers=[
+                      'Development Status :: 4 - Beta',
+                      'Environment :: Console',
+                      'Intended Audience :: Developers',
+                      'Intended Audience :: Science/Research',
+                      'Intended Audience :: Education',
+                      'License :: OSI Approved :: BSD License',
+                      'Operating System :: OS Independent',
+                      'Topic :: Scientific/Engineering',
+                      'Topic :: Utilities',
+                      'Topic :: Internet :: WWW/HTTP',
+                      'Programming Language :: Python :: 3.8',
+                      'Programming Language :: Python :: 3.9',
+                 ],
+
+                 platforms='any',
+                 scripts=['bin/sessionmirror.py'],
+                 install_requires=['lxml>=4.3',
+                                   'requests>=2.20',
+                                   'pathlib>=1.0',
+                                   'six>=1.15',
+                                   'future>=0.16',
+                                   'pandas>=0.24',
+                                   'pymupdf>=1.18',
+                                   'pydicom',
+                                   'nibabel>=3.1'],
+                 package_data={'pyxnat': ['README.rst'], },
+
+                 )
```

