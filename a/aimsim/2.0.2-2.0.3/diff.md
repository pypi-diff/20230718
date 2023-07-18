# Comparing `tmp/aimsim-2.0.2.tar.gz` & `tmp/aimsim-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jwb1j\OneDrive\Documents\GitHub\AIMSim\dist\.tmp-r8juhqzq\aimsim-2.0.2.tar", last modified: Thu Feb 23 03:13:00 2023, max compression
+gzip compressed data, was "aimsim-2.0.3.tar", last modified: Tue Jul 18 13:49:22 2023, max compression
```

## Comparing `aimsim-2.0.2.tar` & `aimsim-2.0.3.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.769594 aimsim-2.0.2/
--rw-rw-rw-   0        0        0    13916 2023-02-23 03:00:40.000000 aimsim-2.0.2/20230222220038771.csv
--rw-rw-rw-   0        0        0    28657 2022-08-23 20:09:19.000000 aimsim-2.0.2/AIMSim-GUI.png
--rw-rw-rw-   0        0        0     1116 2022-06-28 20:09:01.000000 aimsim-2.0.2/LICENSE
--rw-rw-rw-   0        0        0       60 2022-06-28 20:09:01.000000 aimsim-2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    13473 2023-02-23 03:13:00.765836 aimsim-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    13027 2023-02-23 02:51:05.000000 aimsim-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.529539 aimsim-2.0.2/aimsim/
--rw-rw-rw-   0        0        0      125 2023-02-23 03:11:19.000000 aimsim-2.0.2/aimsim/__init__.py
--rw-rw-rw-   0        0        0      473 2022-06-28 20:09:01.000000 aimsim-2.0.2/aimsim/__main__.py
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.594740 aimsim-2.0.2/aimsim/chemical_datastructures/
--rw-rw-rw-   0        0        0       71 2022-06-28 20:09:01.000000 aimsim-2.0.2/aimsim/chemical_datastructures/__init__.py
--rw-rw-rw-   0        0        0    11226 2022-06-29 01:27:53.000000 aimsim-2.0.2/aimsim/chemical_datastructures/molecule.py
--rw-rw-rw-   0        0        0    49798 2023-02-23 02:07:14.000000 aimsim-2.0.2/aimsim/chemical_datastructures/molecule_set.py
--rw-rw-rw-   0        0        0     1112 2023-02-23 02:07:14.000000 aimsim-2.0.2/aimsim/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.613783 aimsim-2.0.2/aimsim/ops/
--rw-rw-rw-   0        0        0      121 2022-06-28 20:09:01.000000 aimsim-2.0.2/aimsim/ops/__init__.py
--rw-rw-rw-   0        0        0     7322 2022-06-28 20:09:01.000000 aimsim-2.0.2/aimsim/ops/clustering.py
--rw-rw-rw-   0        0        0    77372 2023-02-23 02:35:55.000000 aimsim-2.0.2/aimsim/ops/descriptor.py
--rw-rw-rw-   0        0        0    81997 2023-02-23 02:07:14.000000 aimsim-2.0.2/aimsim/ops/similarity_measures.py
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.653742 aimsim-2.0.2/aimsim/tasks/
--rw-rw-rw-   0        0        0      423 2022-06-28 20:09:01.000000 aimsim-2.0.2/aimsim/tasks/__init__.py
--rw-rw-rw-   0        0        0     7126 2022-06-29 00:55:08.000000 aimsim-2.0.2/aimsim/tasks/cluster_data.py
--rw-rw-rw-   0        0        0     6824 2022-06-29 01:25:21.000000 aimsim-2.0.2/aimsim/tasks/compare_target_molecule.py
--rw-rw-rw-   0        0        0     3145 2022-06-28 20:09:01.000000 aimsim-2.0.2/aimsim/tasks/identify_outliers.py
--rw-rw-rw-   0        0        0    16125 2023-02-23 02:07:14.000000 aimsim-2.0.2/aimsim/tasks/measure_search.py
--rw-rw-rw-   0        0        0     7055 2022-06-29 00:55:08.000000 aimsim-2.0.2/aimsim/tasks/see_property_variation_with_similarity.py
--rw-rw-rw-   0        0        0      509 2022-06-28 20:09:01.000000 aimsim-2.0.2/aimsim/tasks/task.py
--rw-rw-rw-   0        0        0     6419 2023-02-23 02:07:14.000000 aimsim-2.0.2/aimsim/tasks/task_manager.py
--rw-rw-rw-   0        0        0     4390 2022-06-29 00:55:08.000000 aimsim-2.0.2/aimsim/tasks/visualize_dataset.py
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.672048 aimsim-2.0.2/aimsim/utils/
--rw-rw-rw-   0        0        0        0 2022-06-28 20:09:01.000000 aimsim-2.0.2/aimsim/utils/__init__.py
--rw-rw-rw-   0        0        0     3973 2022-06-28 20:09:01.000000 aimsim-2.0.2/aimsim/utils/ccbmlib_fingerprints.py
--rw-rw-rw-   0        0        0      567 2023-02-23 02:30:26.000000 aimsim-2.0.2/aimsim/utils/extras.py
--rw-rw-rw-   0        0        0    19436 2023-02-23 02:07:14.000000 aimsim-2.0.2/aimsim/utils/plotting_scripts.py
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.588600 aimsim-2.0.2/aimsim.egg-info/
--rw-rw-rw-   0        0        0    13473 2023-02-23 03:13:00.000000 aimsim-2.0.2/aimsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1868 2023-02-23 03:13:00.000000 aimsim-2.0.2/aimsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 03:13:00.000000 aimsim-2.0.2/aimsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-02-23 03:13:00.000000 aimsim-2.0.2/aimsim.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      223 2023-02-23 03:13:00.000000 aimsim-2.0.2/aimsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-02-23 03:13:00.000000 aimsim-2.0.2/aimsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      805 2022-06-28 20:09:01.000000 aimsim-2.0.2/config.yaml
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.474466 aimsim-2.0.2/docs/
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.679532 aimsim-2.0.2/docs/_images/
--rw-rw-rw-   0        0        0    90321 2022-06-28 20:09:01.000000 aimsim-2.0.2/docs/_images/AIMSim-logo.png
--rw-rw-rw-   0        0        0   147925 2022-06-28 20:09:01.000000 aimsim-2.0.2/docs/_images/sulfonamide-substrate-scope.png
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.687600 aimsim-2.0.2/docs/_static/
--rw-rw-rw-   0        0        0      286 2022-06-28 20:09:01.000000 aimsim-2.0.2/docs/_static/file.png
--rw-rw-rw-   0        0        0       90 2022-06-28 20:09:01.000000 aimsim-2.0.2/docs/_static/minus.png
--rw-rw-rw-   0        0        0       90 2022-06-28 20:09:01.000000 aimsim-2.0.2/docs/_static/plus.png
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.473363 aimsim-2.0.2/docs/interfaces/
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.691080 aimsim-2.0.2/docs/interfaces/UI/
--rw-rw-rw-   0        0        0    90321 2022-06-28 20:09:01.000000 aimsim-2.0.2/docs/interfaces/UI/AIMSim-logo.png
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.698745 aimsim-2.0.2/docs/tests/
--rw-rw-rw-   0        0        0   147925 2022-06-28 20:09:01.000000 aimsim-2.0.2/docs/tests/sulfonamide-substrate-scope.png
--rw-rw-rw-   0        0        0     2090 2023-02-23 02:07:14.000000 aimsim-2.0.2/implemented_metrics.md
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.704425 aimsim-2.0.2/interfaces/
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.716719 aimsim-2.0.2/interfaces/UI/
--rw-rw-rw-   0        0        0    31374 2022-08-16 20:43:40.000000 aimsim-2.0.2/interfaces/UI/AIMSim-GUI-corner-logo.png
--rw-rw-rw-   0        0        0    90321 2022-06-28 20:09:01.000000 aimsim-2.0.2/interfaces/UI/AIMSim-logo.png
--rw-rw-rw-   0        0        0    19864 2023-01-11 19:17:15.000000 aimsim-2.0.2/interfaces/UI/AIMSim_ui_main.py
--rw-rw-rw-   0        0        0        0 2022-06-28 20:09:01.000000 aimsim-2.0.2/interfaces/UI/__init__.py
--rw-rw-rw-   0        0        0        0 2022-06-28 20:09:01.000000 aimsim-2.0.2/interfaces/__init__.py
--rw-rw-rw-   0        0        0     2145 2022-06-29 00:58:57.000000 aimsim-2.0.2/interfaces/config_reader.py
--rw-rw-rw-   0        0        0      190 2023-02-23 02:07:14.000000 aimsim-2.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-23 03:13:00.770083 aimsim-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1502 2023-02-23 02:59:28.000000 aimsim-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.760349 aimsim-2.0.2/tests/
--rw-rw-rw-   0        0        0        0 2022-06-28 20:09:01.000000 aimsim-2.0.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-23 03:13:00.764160 aimsim-2.0.2/tests/data/
--rw-rw-rw-   0        0        0      432 2022-06-28 20:09:01.000000 aimsim-2.0.2/tests/data/README.md
--rw-rw-rw-   0        0        0    29710 2022-06-28 20:09:01.000000 aimsim-2.0.2/tests/sulfonamide-substrate-scope-PDF.png
--rw-rw-rw-   0        0        0   147925 2022-06-28 20:09:01.000000 aimsim-2.0.2/tests/sulfonamide-substrate-scope.png
--rw-rw-rw-   0        0        0     8133 2023-01-10 21:58:40.000000 aimsim-2.0.2/tests/test_CompareTargetMolecule.py
--rw-rw-rw-   0        0        0    17129 2023-02-23 02:07:14.000000 aimsim-2.0.2/tests/test_Descriptor.py
--rw-rw-rw-   0        0        0     1495 2022-06-28 20:09:01.000000 aimsim-2.0.2/tests/test_LoadingErrorException.py
--rw-rw-rw-   0        0        0    10520 2023-02-23 02:07:14.000000 aimsim-2.0.2/tests/test_MeasureSearch.py
--rw-rw-rw-   0        0        0    12826 2022-06-28 20:09:01.000000 aimsim-2.0.2/tests/test_Molecule.py
--rw-rw-rw-   0        0        0    54177 2023-02-23 02:07:14.000000 aimsim-2.0.2/tests/test_MoleculeSet.py
--rw-rw-rw-   0        0        0     6545 2023-01-10 21:58:40.000000 aimsim-2.0.2/tests/test_SimilarityMeasure.py
--rw-rw-rw-   0        0        0     2321 2023-01-10 21:58:31.000000 aimsim-2.0.2/tests/test_SimilarityMeasureValueErrors.py
--rw-rw-rw-   0        0        0     3686 2022-06-28 20:09:01.000000 aimsim-2.0.2/tests/test_TaskManager.py
--rw-rw-rw-   0        0        0      533 2023-01-11 19:17:15.000000 aimsim-2.0.2/tests/test_ToolTip.py
--rw-rw-rw-   0        0        0    67744 2022-06-28 20:09:01.000000 aimsim-2.0.2/tests/test_multithreading.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.513853 aimsim-2.0.3/
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.417000 aimsim-2.0.3/.pytest_cache/
+-rw-r--r--   0 jackson    (501) staff       (20)      302 2023-03-28 19:30:31.000000 aimsim-2.0.3/.pytest_cache/README.md
+-rw-r--r--   0 jackson    (501) staff       (20)    28657 2023-03-28 19:10:29.000000 aimsim-2.0.3/AIMSim-GUI.png
+-rw-r--r--   0 jackson    (501) staff       (20)     1095 2023-03-28 19:10:29.000000 aimsim-2.0.3/LICENSE
+-rw-r--r--   0 jackson    (501) staff       (20)       60 2023-03-28 19:10:29.000000 aimsim-2.0.3/MANIFEST.in
+-rw-r--r--   0 jackson    (501) staff       (20)    13302 2023-07-18 13:49:22.512897 aimsim-2.0.3/PKG-INFO
+-rw-r--r--   0 jackson    (501) staff       (20)    12910 2023-07-18 13:40:02.000000 aimsim-2.0.3/README.md
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.420751 aimsim-2.0.3/aimsim/
+-rw-r--r--   0 jackson    (501) staff       (20)      119 2023-07-18 13:40:02.000000 aimsim-2.0.3/aimsim/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)      453 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/__main__.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.428344 aimsim-2.0.3/aimsim/chemical_datastructures/
+-rw-r--r--   0 jackson    (501) staff       (20)       69 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/chemical_datastructures/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)    10937 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/chemical_datastructures/molecule.py
+-rw-r--r--   0 jackson    (501) staff       (20)    49022 2023-03-28 19:38:26.000000 aimsim-2.0.3/aimsim/chemical_datastructures/molecule_set.py
+-rw-r--r--   0 jackson    (501) staff       (20)     1074 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/exceptions.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.435295 aimsim-2.0.3/aimsim/ops/
+-rw-r--r--   0 jackson    (501) staff       (20)      118 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/ops/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)     7152 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/ops/clustering.py
+-rw-r--r--   0 jackson    (501) staff       (20)    76163 2023-07-18 13:40:02.000000 aimsim-2.0.3/aimsim/ops/descriptor.py
+-rw-r--r--   0 jackson    (501) staff       (20)    79872 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/ops/similarity_measures.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.446533 aimsim-2.0.3/aimsim/tasks/
+-rw-r--r--   0 jackson    (501) staff       (20)      413 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/tasks/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)     6954 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/tasks/cluster_data.py
+-rw-r--r--   0 jackson    (501) staff       (20)     6668 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/tasks/compare_target_molecule.py
+-rw-r--r--   0 jackson    (501) staff       (20)     3061 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/tasks/identify_outliers.py
+-rw-r--r--   0 jackson    (501) staff       (20)    15813 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/tasks/measure_search.py
+-rw-r--r--   0 jackson    (501) staff       (20)     6883 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/tasks/see_property_variation_with_similarity.py
+-rw-r--r--   0 jackson    (501) staff       (20)      485 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/tasks/task.py
+-rw-r--r--   0 jackson    (501) staff       (20)     6272 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/tasks/task_manager.py
+-rw-r--r--   0 jackson    (501) staff       (20)     4277 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/tasks/visualize_dataset.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.451218 aimsim-2.0.3/aimsim/utils/
+-rw-r--r--   0 jackson    (501) staff       (20)        0 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/utils/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)     3853 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/utils/ccbmlib_fingerprints.py
+-rw-r--r--   0 jackson    (501) staff       (20)      549 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/utils/extras.py
+-rw-r--r--   0 jackson    (501) staff       (20)    18934 2023-03-28 19:10:29.000000 aimsim-2.0.3/aimsim/utils/plotting_scripts.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.425493 aimsim-2.0.3/aimsim.egg-info/
+-rw-r--r--   0 jackson    (501) staff       (20)    13302 2023-07-18 13:49:22.000000 aimsim-2.0.3/aimsim.egg-info/PKG-INFO
+-rw-r--r--   0 jackson    (501) staff       (20)     1870 2023-07-18 13:49:22.000000 aimsim-2.0.3/aimsim.egg-info/SOURCES.txt
+-rw-r--r--   0 jackson    (501) staff       (20)        1 2023-07-18 13:49:22.000000 aimsim-2.0.3/aimsim.egg-info/dependency_links.txt
+-rw-r--r--   0 jackson    (501) staff       (20)       56 2023-07-18 13:49:22.000000 aimsim-2.0.3/aimsim.egg-info/entry_points.txt
+-rw-r--r--   0 jackson    (501) staff       (20)      226 2023-07-18 13:49:22.000000 aimsim-2.0.3/aimsim.egg-info/requires.txt
+-rw-r--r--   0 jackson    (501) staff       (20)       24 2023-07-18 13:49:22.000000 aimsim-2.0.3/aimsim.egg-info/top_level.txt
+-rw-r--r--   0 jackson    (501) staff       (20)      785 2023-03-28 19:10:29.000000 aimsim-2.0.3/config.yaml
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.406593 aimsim-2.0.3/docs/
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.455742 aimsim-2.0.3/docs/_images/
+-rw-r--r--   0 jackson    (501) staff       (20)    90321 2023-03-28 19:10:29.000000 aimsim-2.0.3/docs/_images/AIMSim-logo.png
+-rw-r--r--   0 jackson    (501) staff       (20)   147925 2023-03-28 19:10:29.000000 aimsim-2.0.3/docs/_images/sulfonamide-substrate-scope.png
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.463789 aimsim-2.0.3/docs/_static/
+-rw-r--r--   0 jackson    (501) staff       (20)      286 2023-03-28 19:10:29.000000 aimsim-2.0.3/docs/_static/file.png
+-rw-r--r--   0 jackson    (501) staff       (20)       90 2023-03-28 19:10:29.000000 aimsim-2.0.3/docs/_static/minus.png
+-rw-r--r--   0 jackson    (501) staff       (20)       90 2023-03-28 19:10:29.000000 aimsim-2.0.3/docs/_static/plus.png
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.406375 aimsim-2.0.3/docs/interfaces/
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.465280 aimsim-2.0.3/docs/interfaces/UI/
+-rw-r--r--   0 jackson    (501) staff       (20)    90321 2023-03-28 19:10:29.000000 aimsim-2.0.3/docs/interfaces/UI/AIMSim-logo.png
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.467913 aimsim-2.0.3/docs/tests/
+-rw-r--r--   0 jackson    (501) staff       (20)   147925 2023-03-28 19:10:29.000000 aimsim-2.0.3/docs/tests/sulfonamide-substrate-scope.png
+-rw-r--r--   0 jackson    (501) staff       (20)     2040 2023-03-28 19:10:29.000000 aimsim-2.0.3/implemented_metrics.md
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.473067 aimsim-2.0.3/interfaces/
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.482354 aimsim-2.0.3/interfaces/UI/
+-rw-r--r--   0 jackson    (501) staff       (20)    31374 2023-03-28 19:10:29.000000 aimsim-2.0.3/interfaces/UI/AIMSim-GUI-corner-logo.png
+-rw-r--r--   0 jackson    (501) staff       (20)    90321 2023-03-28 19:10:29.000000 aimsim-2.0.3/interfaces/UI/AIMSim-logo.png
+-rw-r--r--   0 jackson    (501) staff       (20)    19253 2023-03-28 19:10:29.000000 aimsim-2.0.3/interfaces/UI/AIMSim_ui_main.py
+-rw-r--r--   0 jackson    (501) staff       (20)        0 2023-03-28 19:10:29.000000 aimsim-2.0.3/interfaces/UI/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)        0 2023-03-28 19:10:29.000000 aimsim-2.0.3/interfaces/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)     2095 2023-03-28 19:10:29.000000 aimsim-2.0.3/interfaces/config_reader.py
+-rw-r--r--   0 jackson    (501) staff       (20)      177 2023-07-18 13:40:02.000000 aimsim-2.0.3/requirements.txt
+-rw-r--r--   0 jackson    (501) staff       (20)       38 2023-07-18 13:49:22.514067 aimsim-2.0.3/setup.cfg
+-rw-r--r--   0 jackson    (501) staff       (20)     1448 2023-03-28 19:10:29.000000 aimsim-2.0.3/setup.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.508637 aimsim-2.0.3/tests/
+-rw-r--r--   0 jackson    (501) staff       (20)        0 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/__init__.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-18 13:49:22.510936 aimsim-2.0.3/tests/data/
+-rw-r--r--   0 jackson    (501) staff       (20)      428 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/data/README.md
+-rw-r--r--   0 jackson    (501) staff       (20)    29710 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/sulfonamide-substrate-scope-PDF.png
+-rw-r--r--   0 jackson    (501) staff       (20)   147925 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/sulfonamide-substrate-scope.png
+-rw-r--r--   0 jackson    (501) staff       (20)     7954 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/test_CompareTargetMolecule.py
+-rw-r--r--   0 jackson    (501) staff       (20)    17620 2023-07-18 13:40:02.000000 aimsim-2.0.3/tests/test_Descriptor.py
+-rw-r--r--   0 jackson    (501) staff       (20)     1445 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/test_LoadingErrorException.py
+-rw-r--r--   0 jackson    (501) staff       (20)    10253 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/test_MeasureSearch.py
+-rw-r--r--   0 jackson    (501) staff       (20)    12482 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/test_Molecule.py
+-rw-r--r--   0 jackson    (501) staff       (20)    52827 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/test_MoleculeSet.py
+-rw-r--r--   0 jackson    (501) staff       (20)     6381 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/test_SimilarityMeasure.py
+-rw-r--r--   0 jackson    (501) staff       (20)     2253 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/test_SimilarityMeasureValueErrors.py
+-rw-r--r--   0 jackson    (501) staff       (20)     3585 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/test_TaskManager.py
+-rw-r--r--   0 jackson    (501) staff       (20)      512 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/test_ToolTip.py
+-rw-r--r--   0 jackson    (501) staff       (20)    66192 2023-03-28 19:10:29.000000 aimsim-2.0.3/tests/test_multithreading.py
```

### Comparing `aimsim-2.0.2/AIMSim-GUI.png` & `aimsim-2.0.3/AIMSim-GUI.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.0.2/LICENSE` & `aimsim-2.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 himaghna bhattacharjee & Jackson Burns
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
+MIT License
+
+Copyright (c) 2020 himaghna bhattacharjee & Jackson Burns
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
```

### Comparing `aimsim-2.0.2/PKG-INFO` & `aimsim-2.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,200 +1,188 @@
-Metadata-Version: 2.1
-Name: aimsim
-Version: 2.0.2
-Summary: Python command line and GUI tool to analyze molecular similarity.
-Home-page: https://github.com/VlachosGroup/AIMSim
-Author: Himaghna Bhattacharjee, Jackson Burns
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: mordred
-License-File: LICENSE
-
-<h1 align="center">AIMSim README</h1> 
-<h3 align="center">Visualizing Diversity in your Molecular Dataset</h3>
-
-![AIMSim Logo](interfaces/UI/AIMSim-logo.png)
-<p align="center">
-  <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/VlachosGroup/AIMSim?style=social">
-  <img alt="Total Downloads" src="https://static.pepy.tech/personalized-badge/aimsim?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/aimsim">
-  <img alt="commits since" src="https://img.shields.io/github/commits-since/VlachosGroup/AIMSim/latest.svg">
-  <img alt="PyPI" src="https://img.shields.io/pypi/v/aimsim">
-  <img alt="PyPI - License" src="https://img.shields.io/github/license/VlachosGroup/AIMSim">
-  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/run_tests.yml/badge.svg?branch=master&event=schedule">
-</p>
-
-## Documentation and Tutorial
-[View our Online Documentation](https://vlachosgroup.github.io/AIMSim/) or try the [_AIMSim_ comprehensive tutorial in your browser](https://mybinder.org/v2/gh/VlachosGroup/AIMSim/master?labpath=AIMSim-demo.ipynb).
-
-## Purpose
-
-__Why Do We Need To Visualize Molecular Similarity / Diversity?__
-
-There are several contexts where it is helpful to visualize the diversity of a molecular dataset:
-
-_Exploratory Experimental Synthesis_
-
-For a chemist, synthesizing new molecules with targeted properties is often a laborious and time consuming task.
-In such a case, it becomes useful to check the similarity of a newly proposed (un-synthesized) molecule to the ones already synthesized.
-If the proposed molecule is too similar to the existing repertoire of molecules, it will probably not yield not enough new information /
-property and thus need not be synthesized. Thus, a chemist can avoid spending
-time and effort synthesizing molecules not useful for the project.
-
-_Lead Optimization and Virtual Screening_
-
-This application is the converse of exploratory synthesis where the interest is to find molecules in a database which are structurally similar to an "active" molecule. In this context, "active" might refer to pharmocological activity (drug discover campaigns) or desirable chemical properties (for example, to discover alternative chemicals and solvents for an application). In such a case, AIMSim helps to run virtual screenings over a molecular database and visualize the results.
-
-_Machine Learning Molecular Properties_
-
-In the context of machine learning, visualizing the diversity of the training set gives a good idea about its information quality.
-A more diverse training data-set yields a more robust model, which generalizes well to unseen data. Additionally, such a visualization can 
-identify "clusters of similarity" indicating the need for separately trained models for each cluster.
-
-_Substrate Scope Robustness Verification_
-
-When proposing a novel reaction it is essential for the practicing chemist to evaluate the transformation's tolerance of diverse functional groups and substrates (Glorius, 2013). Using `AIMSim`, one can evaluate the structural and chemical similarity across an entire susbtrate scope to ensure that it avoids redundant species. Below is an example similarity heatmap generated to visualize the diversity of a three-component sulfonamide coupling reaction with a substantial number of substrates (Chen, 2018).
-![Image of sulfonamide substrate scope](tests/sulfonamide-substrate-scope.png)
-
-Many of the substrates appear similar to one another and thereby redundant, but in reality the core sulfone moiety and the use of the same coupling partner when evaluating functional group tolerance accounts for this apparent shortcoming. Also of note is the region of high similarity along the diagonal where the substrates often differ by a single halide heteratom or substitution pattern.
-
-## Installing AIMSim
-`AIMSim` can be installed with a single command:
-`pip install aimsim`
-This command also installs the required dependencies. It is recommended to install `AIMSim` in a separate virtual environment.
-
-_Optional:_ Previous versions of AIMSim provided direct support for the descriptors provided in the `mordred` package. Unforunately, `mordred` is no longer recieving updates and causes significant depdendency conflicts. Because of this, it is an _optional_ add-on to `AIMSim` that is only compatible with Python 3.8. To install with `mordred` support, use `pip install 'aimsim[mordred]'` (note the single quotes, necessary in `zsh`).
-
-Unit tests from previous versions of `AIMSim` have been kept but are not actively maintained due to the limitations above. Use `mordred` at your own risk.
-
-## Running AIMSim
-`AIMSim` is compatible with Python 3.7 to 3.9.
-Start `AIMSim` with a graphical user interface:
-
-`aimsim`
-
-Start `AIMSim` with a prepared configuration YAML file (`config.yaml`):
-
-`aimsim config.yaml`
-
-### Currently Implemented Fingerprints
-
-1. Morgan Fingerprint (Equivalent to the ECFP fingerprints)
-2. RDKit Topological Fingerprint
-3. RDKit Daylight Fingerprint
-
-_The following are available via command line use (config.yaml) only:_
-
-4. All fingerprints available from the [ccbmlib](https://github.com/vogt-m/ccbmlib) package (_specify 'ccbmlib:descriptorname' for command line input_).
-5. All descriptors and fingerprints available from [PaDELPy](https://github.com/ecrl/padelpy), an interface to PaDEL-Descriptor. (_specify 'padelpy:desciptorname' for command line input._).
-6. All descriptors available through the [Mordred](https://github.com/mordred-descriptor/mordred) library (_specify 'mordred:desciptorname' for command line input._). To enable this option, you must install with `pip install 'aimsim[mordred]'` (see disclaimer in the Installation section above).
-
-### Currently Implemented Similarity Scores
-
-44 commonly used similarity scores are implemented in AIMSim.
-Additional L0, L1 and L2 norm based similarities are also implemented. [View our Online Documentation](https://vlachosgroup.github.io/AIMSim/implemented_metrics.html) for a complete list of implemented similarity scores.
-
-
-### Currently Implemented Functionalities
-
-1. Measure Search: Automate the search of fingerprint and similarity metric (called a "measure") using the following algorithm:
-  Step 1: Select an arbitrary featurization scheme.
-  Step 2: Featurize the molecule set using the selected scheme.
-  Step 3: Choose an arbitrary similarity measure.
-  Step 4: Select each moleculeâ€™s nearest and furthest neighbors in the set using the similarity measure.
-  Step 5: Measure the correlation between a moleculeâ€™s QoI and its nearest neighborâ€™s QoI.
-  Step 6: Measure the correlation between a moleculeâ€™s QoI and its further neighborâ€™s QoI.
-  Step 7: Define a score which maximizes the value in Step 5 and minimizes the value in Step 6.
-  Step 8: Iterate Steps 1 â€“ 7 to select the featurization scheme and similarity measure to maximize the result of Step 7. 
-2. See Property Variation with Similarity: Visualize the correlation in the QoI between nearest neighbor molecules (most similar pairs in the molecule set) and between the furthest neighbor molecules (most dissimilar pairs in the molecule set). This is used to verify that the chosen measure is appropriate for the task.
-
-3. Visualize Dataset: Visualize the diversity of the molecule set in the form of a pairwise similarity density and a similarity heatmap of the molecule set. Embed the molecule set in 2D space using using principal component analysis (PCA)[3], multi-dimensional scaling[4], t-SNE[5], Spectral Embedding[6], or Isomap[7].
-
-4. Compare Target Molecule to Molecule Set: Run a similarity search of a molecule against a database of molecules (molecule set). This task can be used to identify the most similar (useful in virtual screening operations) or most dissimilar (useful in application that require high diversity such as training set design for machine learning models) molecules.
-
-5. Cluster Data: Cluster the molecule set. The following algorithms are implemented: 
-
-For arbitrary molecular features or similarity metrics with defined Euclidean distances: K-Medoids[3] and Ward[8] (hierarchical clustering).
-
-For binary fingerprints: Complete, single and average linkage hierarchical clustering[8].
-
-The clustered data is plotted in two dimensions using principal component analysis (PCA)[3], multi-dimensional scaling[4], or TSNE[5].
-
-6. Outlier Detection: Using an isolation forest, check for which molecules are potentially novel or are outliers according to the selected descriptor. Output can be directly to the command line by specifiying `output` to be `terminal` or to a text file by instead providing a filename.
-
-## Contributors
-
-Developer: Himaghna Bhattacharjee, Vlachos Research Lab. ([LinkedIn](www.linkedin.com/in/himaghna-bhattacharjee))
-
-Developer: Jackson Burns, Don Watson Lab. ([Personal Site](https://www.jacksonwarnerburns.com/))
-
-## Developer Notes
-Issues and Pull Requests are welcomed! To propose an addition to `AIMSim` open an issue and the developers will tag it as an _enhancement_ and start discussion.
-
-`AIMSim` includes an automated testing apparatus operated by Python's _unittest_ built-in package. To execute tests related to the core functionality of `AIMSim`, run this command:
-
-`python -m unittest discover`
-
-Full multiprocessing speedup and efficiency tests take more than 10 hours to run due to the number of replicates required. To run these tests, create a file called `.speedup-test` in the `AIMSim` directory and execute the above command as shown.
-
-To manually build the docs, execute the following with `sphinx` and `m2r` installed and from the `/docs` directory:
-
-`m2r ../README.md | mv ../README.rst . | sphinx-apidoc -f -o . .. | make html | cp _build/html/* .`
-
-Documentation should manually build on push to master branch via an automated GitHub action.
-
-For packaging on PyPI:
-
-`python -m build; twine upload dist/*`
-
-Be sure to bump the version in `__init__.py`.
-
-## Citation
-If you use this code for scientific publications, please cite the following paper.
-
-Bhattacharjee, H.Ò‚; Burns, J.Ò‚; Vlachos, D.G. (2021): AIMSim: An Accessible Cheminformatics Platform for Similarity Operations on Chemicals Datasets. ChemRxiv. Preprint. https://doi.org/10.26434/chemrxiv-2022-nw6f5
-
-## License
-This code is made available under the terms of the _MIT Open License_:
-
-Copyright (c) 2020 Himaghna Bhattacharjee & Jackson Burns
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
-
-
-## Works Cited
-[1] Collins, K. and Glorius, F., A robustness screen for the rapid assessment of chemical reactions. Nature Chem 5, 597â€“601 (2013). https://doi.org/10.1038/nchem.1669
-
-[2] Chen, Y., Murray, P.R.D., Davies, A.T., and Willis M.C., J. Am. Chem. Soc. 140 (28), 8781-8787 (2018). https://doi.org/10.1021/jacs.8b04532
-
-[3] Hastie, T., Tibshirani R. and Friedman J., The Elements of statistical Learning: Data Mining, Inference, and Prediction, 2nd Ed., Springer Series in Statistics (2009).
-
-[4] Borg, I. and Groenen, P.J.F., Modern Multidimensional Scaling: Theory and Applications, Springer Series in Statistics (2005).
-
-[5] van der Maaten, L.J.P. and Hinton, G.E., Visualizing High-Dimensional Data Using t-SNE. Journal of Machine Learning Research 9:2579-2605 (2008).
-
-[6] Ng, A.Y., Jordan, M.I. and Weiss, Y., On Spectral Clustering: Analysis and an algorithm. ADVANCES IN NEURAL INFORMATION PROCESSING SYSTEMS, MIT Press (2001).
-
-[7] Tenenbaum, J.B., De Silva, V. and Langford, J.C, A global geometric framework for nonlinear dimensionality reduction, Science 290 (5500), 2319-23 (2000). https://doi.org/10.1126/science.290.5500.2319.
-
-[8] Murtagh, F. and Contreras, P., Algorithms for hierarchical clustering: an overview. WIREs Data Mining Knowl Discov (2011). https://doi.org/10.1002/widm.53
-
-
-
+<h1 align="center">AIMSim README</h1> 
+<h3 align="center">Visualizing Diversity in your Molecular Dataset</h3>
+
+![AIMSim Logo](interfaces/UI/AIMSim-logo.png)
+<p align="center">
+  <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/VlachosGroup/AIMSim?style=social">
+  <img alt="Total Downloads" src="https://static.pepy.tech/personalized-badge/aimsim?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads">
+  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/aimsim">
+  <img alt="commits since" src="https://img.shields.io/github/commits-since/VlachosGroup/AIMSim/latest.svg">
+  <img alt="PyPI" src="https://img.shields.io/pypi/v/aimsim">
+  <img alt="PyPI - License" src="https://img.shields.io/github/license/VlachosGroup/AIMSim">
+  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/run_tests.yml/badge.svg?branch=master&event=schedule">
+</p>
+
+## Documentation and Tutorial
+[View our Online Documentation](https://vlachosgroup.github.io/AIMSim/) or try the [_AIMSim_ comprehensive tutorial in your browser](https://mybinder.org/v2/gh/VlachosGroup/AIMSim/master?labpath=AIMSim-demo.ipynb).
+
+## Purpose
+
+__Why Do We Need To Visualize Molecular Similarity / Diversity?__
+
+There are several contexts where it is helpful to visualize the diversity of a molecular dataset:
+
+_Exploratory Experimental Synthesis_
+
+For a chemist, synthesizing new molecules with targeted properties is often a laborious and time consuming task.
+In such a case, it becomes useful to check the similarity of a newly proposed (un-synthesized) molecule to the ones already synthesized.
+If the proposed molecule is too similar to the existing repertoire of molecules, it will probably not yield not enough new information /
+property and thus need not be synthesized. Thus, a chemist can avoid spending
+time and effort synthesizing molecules not useful for the project.
+
+_Lead Optimization and Virtual Screening_
+
+This application is the converse of exploratory synthesis where the interest is to find molecules in a database which are structurally similar to an "active" molecule. In this context, "active" might refer to pharmocological activity (drug discover campaigns) or desirable chemical properties (for example, to discover alternative chemicals and solvents for an application). In such a case, AIMSim helps to run virtual screenings over a molecular database and visualize the results.
+
+_Machine Learning Molecular Properties_
+
+In the context of machine learning, visualizing the diversity of the training set gives a good idea about its information quality.
+A more diverse training data-set yields a more robust model, which generalizes well to unseen data. Additionally, such a visualization can 
+identify "clusters of similarity" indicating the need for separately trained models for each cluster.
+
+_Substrate Scope Robustness Verification_
+
+When proposing a novel reaction it is essential for the practicing chemist to evaluate the transformation's tolerance of diverse functional groups and substrates (Glorius, 2013). Using `AIMSim`, one can evaluate the structural and chemical similarity across an entire susbtrate scope to ensure that it avoids redundant species. Below is an example similarity heatmap generated to visualize the diversity of a three-component sulfonamide coupling reaction with a substantial number of substrates (Chen, 2018).
+![Image of sulfonamide substrate scope](tests/sulfonamide-substrate-scope.png)
+
+Many of the substrates appear similar to one another and thereby redundant, but in reality the core sulfone moiety and the use of the same coupling partner when evaluating functional group tolerance accounts for this apparent shortcoming. Also of note is the region of high similarity along the diagonal where the substrates often differ by a single halide heteratom or substitution pattern.
+
+## Installing AIMSim
+`AIMSim` can be installed with a single command:
+`pip install aimsim`
+This command also installs the required dependencies. It is recommended to install `AIMSim` in a separate virtual environment.
+
+_Optional:_ Previous versions of AIMSim provided direct support for the descriptors provided in the `mordred` package. Unforunately, `mordred` is no longer recieving updates and causes significant depdendency conflicts. Because of this, it is an _optional_ add-on to `AIMSim` that is only compatible with Python 3.8. To install with `mordred` support, use `pip install 'aimsim[mordred]'` (note the single quotes, necessary in `zsh`).
+
+Unit tests from previous versions of `AIMSim` have been kept but are not actively maintained due to the limitations above. Use `mordred` at your own risk.
+
+## Running AIMSim
+`AIMSim` is compatible with Python 3.7 to 3.9.
+Start `AIMSim` with a graphical user interface:
+
+`aimsim`
+
+Start `AIMSim` with a prepared configuration YAML file (`config.yaml`):
+
+`aimsim config.yaml`
+
+### Currently Implemented Fingerprints
+
+1. Morgan Fingerprint (Equivalent to the ECFP fingerprints)
+2. RDKit Topological Fingerprint
+3. RDKit Daylight Fingerprint
+
+_The following are available via command line use (config.yaml) only:_
+
+4. MinHash Fingerprint (see [MHFP](https://github.com/reymond-group/mhfp))
+5. All fingerprints available from the [ccbmlib](https://github.com/vogt-m/ccbmlib) package (_specify 'ccbmlib:descriptorname' for command line input_).
+6. All descriptors and fingerprints available from [PaDELPy](https://github.com/ecrl/padelpy), an interface to PaDEL-Descriptor. (_specify 'padelpy:desciptorname' for command line input._).
+7. All descriptors available through the [Mordred](https://github.com/mordred-descriptor/mordred) library (_specify 'mordred:desciptorname' for command line input._). To enable this option, you must install with `pip install 'aimsim[mordred]'` (see disclaimer in the Installation section above).
+
+### Currently Implemented Similarity Scores
+
+44 commonly used similarity scores are implemented in AIMSim.
+Additional L0, L1 and L2 norm based similarities are also implemented. [View our Online Documentation](https://vlachosgroup.github.io/AIMSim/implemented_metrics.html) for a complete list of implemented similarity scores.
+
+
+### Currently Implemented Functionalities
+
+1. Measure Search: Automate the search of fingerprint and similarity metric (called a "measure") using the following algorithm:
+  Step 1: Select an arbitrary featurization scheme.
+  Step 2: Featurize the molecule set using the selected scheme.
+  Step 3: Choose an arbitrary similarity measure.
+  Step 4: Select each molecule’s nearest and furthest neighbors in the set using the similarity measure.
+  Step 5: Measure the correlation between a molecule’s QoI and its nearest neighbor’s QoI.
+  Step 6: Measure the correlation between a molecule’s QoI and its further neighbor’s QoI.
+  Step 7: Define a score which maximizes the value in Step 5 and minimizes the value in Step 6.
+  Step 8: Iterate Steps 1 – 7 to select the featurization scheme and similarity measure to maximize the result of Step 7. 
+2. See Property Variation with Similarity: Visualize the correlation in the QoI between nearest neighbor molecules (most similar pairs in the molecule set) and between the furthest neighbor molecules (most dissimilar pairs in the molecule set). This is used to verify that the chosen measure is appropriate for the task.
+
+3. Visualize Dataset: Visualize the diversity of the molecule set in the form of a pairwise similarity density and a similarity heatmap of the molecule set. Embed the molecule set in 2D space using using principal component analysis (PCA)[3], multi-dimensional scaling[4], t-SNE[5], Spectral Embedding[6], or Isomap[7].
+
+4. Compare Target Molecule to Molecule Set: Run a similarity search of a molecule against a database of molecules (molecule set). This task can be used to identify the most similar (useful in virtual screening operations) or most dissimilar (useful in application that require high diversity such as training set design for machine learning models) molecules.
+
+5. Cluster Data: Cluster the molecule set. The following algorithms are implemented: 
+
+For arbitrary molecular features or similarity metrics with defined Euclidean distances: K-Medoids[3] and Ward[8] (hierarchical clustering).
+
+For binary fingerprints: Complete, single and average linkage hierarchical clustering[8].
+
+The clustered data is plotted in two dimensions using principal component analysis (PCA)[3], multi-dimensional scaling[4], or TSNE[5].
+
+6. Outlier Detection: Using an isolation forest, check for which molecules are potentially novel or are outliers according to the selected descriptor. Output can be directly to the command line by specifiying `output` to be `terminal` or to a text file by instead providing a filename.
+
+## Contributors
+
+Developer: Himaghna Bhattacharjee, Vlachos Research Lab. ([LinkedIn](www.linkedin.com/in/himaghna-bhattacharjee))
+
+Developer: Jackson Burns, Don Watson Lab. ([Personal Site](https://www.jacksonwarnerburns.com/))
+
+## Developer Notes
+Issues and Pull Requests are welcomed! To propose an addition to `AIMSim` open an issue and the developers will tag it as an _enhancement_ and start discussion.
+
+`AIMSim` includes an automated testing apparatus operated by Python's _unittest_ built-in package. To execute tests related to the core functionality of `AIMSim`, run this command:
+
+`python -m unittest discover`
+
+Full multiprocessing speedup and efficiency tests take more than 10 hours to run due to the number of replicates required. To run these tests, create a file called `.speedup-test` in the `AIMSim` directory and execute the above command as shown.
+
+To manually build the docs, execute the following with `sphinx` and `m2r` installed and from the `/docs` directory:
+
+`m2r ../README.md | mv ../README.rst . | sphinx-apidoc -f -o . .. | make html | cp _build/html/* .`
+
+Documentation should manually build on push to master branch via an automated GitHub action.
+
+For packaging on PyPI:
+
+`python -m build; twine upload dist/*`
+
+Be sure to bump the version in `__init__.py`.
+
+## Citation
+If you use this code for scientific publications, please cite the following paper.
+
+Bhattacharjee, H.҂; Burns, J.҂; Vlachos, D.G. (2021): AIMSim: An Accessible Cheminformatics Platform for Similarity Operations on Chemicals Datasets. ChemRxiv. Preprint. https://doi.org/10.26434/chemrxiv-2022-nw6f5
+
+## License
+This code is made available under the terms of the _MIT Open License_:
+
+Copyright (c) 2020 Himaghna Bhattacharjee & Jackson Burns
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
+
+
+## Works Cited
+[1] Collins, K. and Glorius, F., A robustness screen for the rapid assessment of chemical reactions. Nature Chem 5, 597–601 (2013). https://doi.org/10.1038/nchem.1669
+
+[2] Chen, Y., Murray, P.R.D., Davies, A.T., and Willis M.C., J. Am. Chem. Soc. 140 (28), 8781-8787 (2018). https://doi.org/10.1021/jacs.8b04532
+
+[3] Hastie, T., Tibshirani R. and Friedman J., The Elements of statistical Learning: Data Mining, Inference, and Prediction, 2nd Ed., Springer Series in Statistics (2009).
+
+[4] Borg, I. and Groenen, P.J.F., Modern Multidimensional Scaling: Theory and Applications, Springer Series in Statistics (2005).
+
+[5] van der Maaten, L.J.P. and Hinton, G.E., Visualizing High-Dimensional Data Using t-SNE. Journal of Machine Learning Research 9:2579-2605 (2008).
+
+[6] Ng, A.Y., Jordan, M.I. and Weiss, Y., On Spectral Clustering: Analysis and an algorithm. ADVANCES IN NEURAL INFORMATION PROCESSING SYSTEMS, MIT Press (2001).
+
+[7] Tenenbaum, J.B., De Silva, V. and Langford, J.C, A global geometric framework for nonlinear dimensionality reduction, Science 290 (5500), 2319-23 (2000). https://doi.org/10.1126/science.290.5500.2319.
+
+[8] Murtagh, F. and Contreras, P., Algorithms for hierarchical clustering: an overview. WIREs Data Mining Knowl Discov (2011). https://doi.org/10.1002/widm.53
+
+
+
```

### Comparing `aimsim-2.0.2/README.md` & `aimsim-2.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,187 +1,201 @@
-<h1 align="center">AIMSim README</h1> 
-<h3 align="center">Visualizing Diversity in your Molecular Dataset</h3>
-
-![AIMSim Logo](interfaces/UI/AIMSim-logo.png)
-<p align="center">
-  <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/VlachosGroup/AIMSim?style=social">
-  <img alt="Total Downloads" src="https://static.pepy.tech/personalized-badge/aimsim?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/aimsim">
-  <img alt="commits since" src="https://img.shields.io/github/commits-since/VlachosGroup/AIMSim/latest.svg">
-  <img alt="PyPI" src="https://img.shields.io/pypi/v/aimsim">
-  <img alt="PyPI - License" src="https://img.shields.io/github/license/VlachosGroup/AIMSim">
-  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/run_tests.yml/badge.svg?branch=master&event=schedule">
-</p>
-
-## Documentation and Tutorial
-[View our Online Documentation](https://vlachosgroup.github.io/AIMSim/) or try the [_AIMSim_ comprehensive tutorial in your browser](https://mybinder.org/v2/gh/VlachosGroup/AIMSim/master?labpath=AIMSim-demo.ipynb).
-
-## Purpose
-
-__Why Do We Need To Visualize Molecular Similarity / Diversity?__
-
-There are several contexts where it is helpful to visualize the diversity of a molecular dataset:
-
-_Exploratory Experimental Synthesis_
-
-For a chemist, synthesizing new molecules with targeted properties is often a laborious and time consuming task.
-In such a case, it becomes useful to check the similarity of a newly proposed (un-synthesized) molecule to the ones already synthesized.
-If the proposed molecule is too similar to the existing repertoire of molecules, it will probably not yield not enough new information /
-property and thus need not be synthesized. Thus, a chemist can avoid spending
-time and effort synthesizing molecules not useful for the project.
-
-_Lead Optimization and Virtual Screening_
-
-This application is the converse of exploratory synthesis where the interest is to find molecules in a database which are structurally similar to an "active" molecule. In this context, "active" might refer to pharmocological activity (drug discover campaigns) or desirable chemical properties (for example, to discover alternative chemicals and solvents for an application). In such a case, AIMSim helps to run virtual screenings over a molecular database and visualize the results.
-
-_Machine Learning Molecular Properties_
-
-In the context of machine learning, visualizing the diversity of the training set gives a good idea about its information quality.
-A more diverse training data-set yields a more robust model, which generalizes well to unseen data. Additionally, such a visualization can 
-identify "clusters of similarity" indicating the need for separately trained models for each cluster.
-
-_Substrate Scope Robustness Verification_
-
-When proposing a novel reaction it is essential for the practicing chemist to evaluate the transformation's tolerance of diverse functional groups and substrates (Glorius, 2013). Using `AIMSim`, one can evaluate the structural and chemical similarity across an entire susbtrate scope to ensure that it avoids redundant species. Below is an example similarity heatmap generated to visualize the diversity of a three-component sulfonamide coupling reaction with a substantial number of substrates (Chen, 2018).
-![Image of sulfonamide substrate scope](tests/sulfonamide-substrate-scope.png)
-
-Many of the substrates appear similar to one another and thereby redundant, but in reality the core sulfone moiety and the use of the same coupling partner when evaluating functional group tolerance accounts for this apparent shortcoming. Also of note is the region of high similarity along the diagonal where the substrates often differ by a single halide heteratom or substitution pattern.
-
-## Installing AIMSim
-`AIMSim` can be installed with a single command:
-`pip install aimsim`
-This command also installs the required dependencies. It is recommended to install `AIMSim` in a separate virtual environment.
-
-_Optional:_ Previous versions of AIMSim provided direct support for the descriptors provided in the `mordred` package. Unforunately, `mordred` is no longer recieving updates and causes significant depdendency conflicts. Because of this, it is an _optional_ add-on to `AIMSim` that is only compatible with Python 3.8. To install with `mordred` support, use `pip install 'aimsim[mordred]'` (note the single quotes, necessary in `zsh`).
-
-Unit tests from previous versions of `AIMSim` have been kept but are not actively maintained due to the limitations above. Use `mordred` at your own risk.
-
-## Running AIMSim
-`AIMSim` is compatible with Python 3.7 to 3.9.
-Start `AIMSim` with a graphical user interface:
-
-`aimsim`
-
-Start `AIMSim` with a prepared configuration YAML file (`config.yaml`):
-
-`aimsim config.yaml`
-
-### Currently Implemented Fingerprints
-
-1. Morgan Fingerprint (Equivalent to the ECFP fingerprints)
-2. RDKit Topological Fingerprint
-3. RDKit Daylight Fingerprint
-
-_The following are available via command line use (config.yaml) only:_
-
-4. All fingerprints available from the [ccbmlib](https://github.com/vogt-m/ccbmlib) package (_specify 'ccbmlib:descriptorname' for command line input_).
-5. All descriptors and fingerprints available from [PaDELPy](https://github.com/ecrl/padelpy), an interface to PaDEL-Descriptor. (_specify 'padelpy:desciptorname' for command line input._).
-6. All descriptors available through the [Mordred](https://github.com/mordred-descriptor/mordred) library (_specify 'mordred:desciptorname' for command line input._). To enable this option, you must install with `pip install 'aimsim[mordred]'` (see disclaimer in the Installation section above).
-
-### Currently Implemented Similarity Scores
-
-44 commonly used similarity scores are implemented in AIMSim.
-Additional L0, L1 and L2 norm based similarities are also implemented. [View our Online Documentation](https://vlachosgroup.github.io/AIMSim/implemented_metrics.html) for a complete list of implemented similarity scores.
-
-
-### Currently Implemented Functionalities
-
-1. Measure Search: Automate the search of fingerprint and similarity metric (called a "measure") using the following algorithm:
-  Step 1: Select an arbitrary featurization scheme.
-  Step 2: Featurize the molecule set using the selected scheme.
-  Step 3: Choose an arbitrary similarity measure.
-  Step 4: Select each molecule’s nearest and furthest neighbors in the set using the similarity measure.
-  Step 5: Measure the correlation between a molecule’s QoI and its nearest neighbor’s QoI.
-  Step 6: Measure the correlation between a molecule’s QoI and its further neighbor’s QoI.
-  Step 7: Define a score which maximizes the value in Step 5 and minimizes the value in Step 6.
-  Step 8: Iterate Steps 1 – 7 to select the featurization scheme and similarity measure to maximize the result of Step 7. 
-2. See Property Variation with Similarity: Visualize the correlation in the QoI between nearest neighbor molecules (most similar pairs in the molecule set) and between the furthest neighbor molecules (most dissimilar pairs in the molecule set). This is used to verify that the chosen measure is appropriate for the task.
-
-3. Visualize Dataset: Visualize the diversity of the molecule set in the form of a pairwise similarity density and a similarity heatmap of the molecule set. Embed the molecule set in 2D space using using principal component analysis (PCA)[3], multi-dimensional scaling[4], t-SNE[5], Spectral Embedding[6], or Isomap[7].
-
-4. Compare Target Molecule to Molecule Set: Run a similarity search of a molecule against a database of molecules (molecule set). This task can be used to identify the most similar (useful in virtual screening operations) or most dissimilar (useful in application that require high diversity such as training set design for machine learning models) molecules.
-
-5. Cluster Data: Cluster the molecule set. The following algorithms are implemented: 
-
-For arbitrary molecular features or similarity metrics with defined Euclidean distances: K-Medoids[3] and Ward[8] (hierarchical clustering).
-
-For binary fingerprints: Complete, single and average linkage hierarchical clustering[8].
-
-The clustered data is plotted in two dimensions using principal component analysis (PCA)[3], multi-dimensional scaling[4], or TSNE[5].
-
-6. Outlier Detection: Using an isolation forest, check for which molecules are potentially novel or are outliers according to the selected descriptor. Output can be directly to the command line by specifiying `output` to be `terminal` or to a text file by instead providing a filename.
-
-## Contributors
-
-Developer: Himaghna Bhattacharjee, Vlachos Research Lab. ([LinkedIn](www.linkedin.com/in/himaghna-bhattacharjee))
-
-Developer: Jackson Burns, Don Watson Lab. ([Personal Site](https://www.jacksonwarnerburns.com/))
-
-## Developer Notes
-Issues and Pull Requests are welcomed! To propose an addition to `AIMSim` open an issue and the developers will tag it as an _enhancement_ and start discussion.
-
-`AIMSim` includes an automated testing apparatus operated by Python's _unittest_ built-in package. To execute tests related to the core functionality of `AIMSim`, run this command:
-
-`python -m unittest discover`
-
-Full multiprocessing speedup and efficiency tests take more than 10 hours to run due to the number of replicates required. To run these tests, create a file called `.speedup-test` in the `AIMSim` directory and execute the above command as shown.
-
-To manually build the docs, execute the following with `sphinx` and `m2r` installed and from the `/docs` directory:
-
-`m2r ../README.md | mv ../README.rst . | sphinx-apidoc -f -o . .. | make html | cp _build/html/* .`
-
-Documentation should manually build on push to master branch via an automated GitHub action.
-
-For packaging on PyPI:
-
-`python -m build; twine upload dist/*`
-
-Be sure to bump the version in `__init__.py`.
-
-## Citation
-If you use this code for scientific publications, please cite the following paper.
-
-Bhattacharjee, H.҂; Burns, J.҂; Vlachos, D.G. (2021): AIMSim: An Accessible Cheminformatics Platform for Similarity Operations on Chemicals Datasets. ChemRxiv. Preprint. https://doi.org/10.26434/chemrxiv-2022-nw6f5
-
-## License
-This code is made available under the terms of the _MIT Open License_:
-
-Copyright (c) 2020 Himaghna Bhattacharjee & Jackson Burns
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
-
-
-## Works Cited
-[1] Collins, K. and Glorius, F., A robustness screen for the rapid assessment of chemical reactions. Nature Chem 5, 597–601 (2013). https://doi.org/10.1038/nchem.1669
-
-[2] Chen, Y., Murray, P.R.D., Davies, A.T., and Willis M.C., J. Am. Chem. Soc. 140 (28), 8781-8787 (2018). https://doi.org/10.1021/jacs.8b04532
-
-[3] Hastie, T., Tibshirani R. and Friedman J., The Elements of statistical Learning: Data Mining, Inference, and Prediction, 2nd Ed., Springer Series in Statistics (2009).
-
-[4] Borg, I. and Groenen, P.J.F., Modern Multidimensional Scaling: Theory and Applications, Springer Series in Statistics (2005).
-
-[5] van der Maaten, L.J.P. and Hinton, G.E., Visualizing High-Dimensional Data Using t-SNE. Journal of Machine Learning Research 9:2579-2605 (2008).
-
-[6] Ng, A.Y., Jordan, M.I. and Weiss, Y., On Spectral Clustering: Analysis and an algorithm. ADVANCES IN NEURAL INFORMATION PROCESSING SYSTEMS, MIT Press (2001).
-
-[7] Tenenbaum, J.B., De Silva, V. and Langford, J.C, A global geometric framework for nonlinear dimensionality reduction, Science 290 (5500), 2319-23 (2000). https://doi.org/10.1126/science.290.5500.2319.
-
-[8] Murtagh, F. and Contreras, P., Algorithms for hierarchical clustering: an overview. WIREs Data Mining Knowl Discov (2011). https://doi.org/10.1002/widm.53
-
-
-
+Metadata-Version: 2.1
+Name: aimsim
+Version: 2.0.3
+Summary: Python command line and GUI tool to analyze molecular similarity.
+Home-page: https://github.com/VlachosGroup/AIMSim
+Author: Himaghna Bhattacharjee, Jackson Burns
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: mordred
+License-File: LICENSE
+
+<h1 align="center">AIMSim README</h1> 
+<h3 align="center">Visualizing Diversity in your Molecular Dataset</h3>
+
+![AIMSim Logo](interfaces/UI/AIMSim-logo.png)
+<p align="center">
+  <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/VlachosGroup/AIMSim?style=social">
+  <img alt="Total Downloads" src="https://static.pepy.tech/personalized-badge/aimsim?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads">
+  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/aimsim">
+  <img alt="commits since" src="https://img.shields.io/github/commits-since/VlachosGroup/AIMSim/latest.svg">
+  <img alt="PyPI" src="https://img.shields.io/pypi/v/aimsim">
+  <img alt="PyPI - License" src="https://img.shields.io/github/license/VlachosGroup/AIMSim">
+  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/run_tests.yml/badge.svg?branch=master&event=schedule">
+</p>
+
+## Documentation and Tutorial
+[View our Online Documentation](https://vlachosgroup.github.io/AIMSim/) or try the [_AIMSim_ comprehensive tutorial in your browser](https://mybinder.org/v2/gh/VlachosGroup/AIMSim/master?labpath=AIMSim-demo.ipynb).
+
+## Purpose
+
+__Why Do We Need To Visualize Molecular Similarity / Diversity?__
+
+There are several contexts where it is helpful to visualize the diversity of a molecular dataset:
+
+_Exploratory Experimental Synthesis_
+
+For a chemist, synthesizing new molecules with targeted properties is often a laborious and time consuming task.
+In such a case, it becomes useful to check the similarity of a newly proposed (un-synthesized) molecule to the ones already synthesized.
+If the proposed molecule is too similar to the existing repertoire of molecules, it will probably not yield not enough new information /
+property and thus need not be synthesized. Thus, a chemist can avoid spending
+time and effort synthesizing molecules not useful for the project.
+
+_Lead Optimization and Virtual Screening_
+
+This application is the converse of exploratory synthesis where the interest is to find molecules in a database which are structurally similar to an "active" molecule. In this context, "active" might refer to pharmocological activity (drug discover campaigns) or desirable chemical properties (for example, to discover alternative chemicals and solvents for an application). In such a case, AIMSim helps to run virtual screenings over a molecular database and visualize the results.
+
+_Machine Learning Molecular Properties_
+
+In the context of machine learning, visualizing the diversity of the training set gives a good idea about its information quality.
+A more diverse training data-set yields a more robust model, which generalizes well to unseen data. Additionally, such a visualization can 
+identify "clusters of similarity" indicating the need for separately trained models for each cluster.
+
+_Substrate Scope Robustness Verification_
+
+When proposing a novel reaction it is essential for the practicing chemist to evaluate the transformation's tolerance of diverse functional groups and substrates (Glorius, 2013). Using `AIMSim`, one can evaluate the structural and chemical similarity across an entire susbtrate scope to ensure that it avoids redundant species. Below is an example similarity heatmap generated to visualize the diversity of a three-component sulfonamide coupling reaction with a substantial number of substrates (Chen, 2018).
+![Image of sulfonamide substrate scope](tests/sulfonamide-substrate-scope.png)
+
+Many of the substrates appear similar to one another and thereby redundant, but in reality the core sulfone moiety and the use of the same coupling partner when evaluating functional group tolerance accounts for this apparent shortcoming. Also of note is the region of high similarity along the diagonal where the substrates often differ by a single halide heteratom or substitution pattern.
+
+## Installing AIMSim
+`AIMSim` can be installed with a single command:
+`pip install aimsim`
+This command also installs the required dependencies. It is recommended to install `AIMSim` in a separate virtual environment.
+
+_Optional:_ Previous versions of AIMSim provided direct support for the descriptors provided in the `mordred` package. Unforunately, `mordred` is no longer recieving updates and causes significant depdendency conflicts. Because of this, it is an _optional_ add-on to `AIMSim` that is only compatible with Python 3.8. To install with `mordred` support, use `pip install 'aimsim[mordred]'` (note the single quotes, necessary in `zsh`).
+
+Unit tests from previous versions of `AIMSim` have been kept but are not actively maintained due to the limitations above. Use `mordred` at your own risk.
+
+## Running AIMSim
+`AIMSim` is compatible with Python 3.7 to 3.9.
+Start `AIMSim` with a graphical user interface:
+
+`aimsim`
+
+Start `AIMSim` with a prepared configuration YAML file (`config.yaml`):
+
+`aimsim config.yaml`
+
+### Currently Implemented Fingerprints
+
+1. Morgan Fingerprint (Equivalent to the ECFP fingerprints)
+2. RDKit Topological Fingerprint
+3. RDKit Daylight Fingerprint
+
+_The following are available via command line use (config.yaml) only:_
+
+4. MinHash Fingerprint (see [MHFP](https://github.com/reymond-group/mhfp))
+5. All fingerprints available from the [ccbmlib](https://github.com/vogt-m/ccbmlib) package (_specify 'ccbmlib:descriptorname' for command line input_).
+6. All descriptors and fingerprints available from [PaDELPy](https://github.com/ecrl/padelpy), an interface to PaDEL-Descriptor. (_specify 'padelpy:desciptorname' for command line input._).
+7. All descriptors available through the [Mordred](https://github.com/mordred-descriptor/mordred) library (_specify 'mordred:desciptorname' for command line input._). To enable this option, you must install with `pip install 'aimsim[mordred]'` (see disclaimer in the Installation section above).
+
+### Currently Implemented Similarity Scores
+
+44 commonly used similarity scores are implemented in AIMSim.
+Additional L0, L1 and L2 norm based similarities are also implemented. [View our Online Documentation](https://vlachosgroup.github.io/AIMSim/implemented_metrics.html) for a complete list of implemented similarity scores.
+
+
+### Currently Implemented Functionalities
+
+1. Measure Search: Automate the search of fingerprint and similarity metric (called a "measure") using the following algorithm:
+  Step 1: Select an arbitrary featurization scheme.
+  Step 2: Featurize the molecule set using the selected scheme.
+  Step 3: Choose an arbitrary similarity measure.
+  Step 4: Select each molecule’s nearest and furthest neighbors in the set using the similarity measure.
+  Step 5: Measure the correlation between a molecule’s QoI and its nearest neighbor’s QoI.
+  Step 6: Measure the correlation between a molecule’s QoI and its further neighbor’s QoI.
+  Step 7: Define a score which maximizes the value in Step 5 and minimizes the value in Step 6.
+  Step 8: Iterate Steps 1 – 7 to select the featurization scheme and similarity measure to maximize the result of Step 7. 
+2. See Property Variation with Similarity: Visualize the correlation in the QoI between nearest neighbor molecules (most similar pairs in the molecule set) and between the furthest neighbor molecules (most dissimilar pairs in the molecule set). This is used to verify that the chosen measure is appropriate for the task.
+
+3. Visualize Dataset: Visualize the diversity of the molecule set in the form of a pairwise similarity density and a similarity heatmap of the molecule set. Embed the molecule set in 2D space using using principal component analysis (PCA)[3], multi-dimensional scaling[4], t-SNE[5], Spectral Embedding[6], or Isomap[7].
+
+4. Compare Target Molecule to Molecule Set: Run a similarity search of a molecule against a database of molecules (molecule set). This task can be used to identify the most similar (useful in virtual screening operations) or most dissimilar (useful in application that require high diversity such as training set design for machine learning models) molecules.
+
+5. Cluster Data: Cluster the molecule set. The following algorithms are implemented: 
+
+For arbitrary molecular features or similarity metrics with defined Euclidean distances: K-Medoids[3] and Ward[8] (hierarchical clustering).
+
+For binary fingerprints: Complete, single and average linkage hierarchical clustering[8].
+
+The clustered data is plotted in two dimensions using principal component analysis (PCA)[3], multi-dimensional scaling[4], or TSNE[5].
+
+6. Outlier Detection: Using an isolation forest, check for which molecules are potentially novel or are outliers according to the selected descriptor. Output can be directly to the command line by specifiying `output` to be `terminal` or to a text file by instead providing a filename.
+
+## Contributors
+
+Developer: Himaghna Bhattacharjee, Vlachos Research Lab. ([LinkedIn](www.linkedin.com/in/himaghna-bhattacharjee))
+
+Developer: Jackson Burns, Don Watson Lab. ([Personal Site](https://www.jacksonwarnerburns.com/))
+
+## Developer Notes
+Issues and Pull Requests are welcomed! To propose an addition to `AIMSim` open an issue and the developers will tag it as an _enhancement_ and start discussion.
+
+`AIMSim` includes an automated testing apparatus operated by Python's _unittest_ built-in package. To execute tests related to the core functionality of `AIMSim`, run this command:
+
+`python -m unittest discover`
+
+Full multiprocessing speedup and efficiency tests take more than 10 hours to run due to the number of replicates required. To run these tests, create a file called `.speedup-test` in the `AIMSim` directory and execute the above command as shown.
+
+To manually build the docs, execute the following with `sphinx` and `m2r` installed and from the `/docs` directory:
+
+`m2r ../README.md | mv ../README.rst . | sphinx-apidoc -f -o . .. | make html | cp _build/html/* .`
+
+Documentation should manually build on push to master branch via an automated GitHub action.
+
+For packaging on PyPI:
+
+`python -m build; twine upload dist/*`
+
+Be sure to bump the version in `__init__.py`.
+
+## Citation
+If you use this code for scientific publications, please cite the following paper.
+
+Bhattacharjee, H.҂; Burns, J.҂; Vlachos, D.G. (2021): AIMSim: An Accessible Cheminformatics Platform for Similarity Operations on Chemicals Datasets. ChemRxiv. Preprint. https://doi.org/10.26434/chemrxiv-2022-nw6f5
+
+## License
+This code is made available under the terms of the _MIT Open License_:
+
+Copyright (c) 2020 Himaghna Bhattacharjee & Jackson Burns
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
+
+
+## Works Cited
+[1] Collins, K. and Glorius, F., A robustness screen for the rapid assessment of chemical reactions. Nature Chem 5, 597–601 (2013). https://doi.org/10.1038/nchem.1669
+
+[2] Chen, Y., Murray, P.R.D., Davies, A.T., and Willis M.C., J. Am. Chem. Soc. 140 (28), 8781-8787 (2018). https://doi.org/10.1021/jacs.8b04532
+
+[3] Hastie, T., Tibshirani R. and Friedman J., The Elements of statistical Learning: Data Mining, Inference, and Prediction, 2nd Ed., Springer Series in Statistics (2009).
+
+[4] Borg, I. and Groenen, P.J.F., Modern Multidimensional Scaling: Theory and Applications, Springer Series in Statistics (2005).
+
+[5] van der Maaten, L.J.P. and Hinton, G.E., Visualizing High-Dimensional Data Using t-SNE. Journal of Machine Learning Research 9:2579-2605 (2008).
+
+[6] Ng, A.Y., Jordan, M.I. and Weiss, Y., On Spectral Clustering: Analysis and an algorithm. ADVANCES IN NEURAL INFORMATION PROCESSING SYSTEMS, MIT Press (2001).
+
+[7] Tenenbaum, J.B., De Silva, V. and Langford, J.C, A global geometric framework for nonlinear dimensionality reduction, Science 290 (5500), 2319-23 (2000). https://doi.org/10.1126/science.290.5500.2319.
+
+[8] Murtagh, F. and Contreras, P., Algorithms for hierarchical clustering: an overview. WIREs Data Mining Knowl Discov (2011). https://doi.org/10.1002/widm.53
+
+
+
```

### Comparing `aimsim-2.0.2/aimsim/chemical_datastructures/molecule.py` & `aimsim-2.0.3/aimsim/chemical_datastructures/molecule.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,289 +1,289 @@
-"""Abstraction of RDKit molecule with relevant property manipulation methods."""
-import os.path
-
-import numpy as np
-from rdkit import Chem
-from rdkit.Chem import Draw
-
-from aimsim.exceptions import *
-from aimsim.ops.descriptor import Descriptor
-
-
-class Molecule:
-    """An abstraction of a molecule
-
-    Attributes:
-        mol_graph (RDKIT mol object): Graph-level information of molecule.
-            Implemented as an RDKIT mol object.
-        mol_text (str): Text identifier of the molecule.
-        mol_property_val (float): Some property associated with the molecule.
-                This is typically the response being studied.
-                E.g. Boiling point, Selectivity etc.
-        descriptor (Descriptor object): Vector representation of a molecule.
-             Commonly a fingerprint.
-
-    Methods:
-        set_descriptor(
-            arbitrary_descriptor_val=None,
-            fingerprint_type=None,
-            fingerprint_params=None): Set the descriptor value either by passing
-            an arbitrary value or by specifying a fingerprint that will be
-            generated.
-        get_descriptor_val(): Get the descriptor value as an numpy array.
-        match_fingerprint_from(reference_mol): Generate the same fingerprint
-            as the reference_mol.
-        get_similarity_to(target_mol, similarity_measure): Get the similarity
-            to target_mol using a similarity_measure of choice.
-        get_name(): Get the mol_text attribute.
-        get_mol_property_val(): Get mol_property_val attribute.
-        draw(fpath=None, **kwargs): Draw the molecule.
-        is_same(source_molecule, target_molecule): Static method used to check
-            equivalence of two molecules.
-
-    """
-
-    def __init__(
-        self,
-        mol_graph=None,
-        mol_text=None,
-        mol_property_val=None,
-        mol_descriptor_val=None,
-        mol_src=None,
-        mol_smiles=None,
-    ):
-        """Constructor
-
-        Args:
-            mol_graph (RDKIT mol object): Graph-level information of molecule.
-                Implemented as an RDKIT mol object. Default is None.
-            mol_text (str): Text identifier of the molecule. Default is None.
-                Identifiers can be:
-                ------------------
-                1. Name of the molecule.
-                2. SMILES string representing the molecule.
-            mol_property_val (float): Some property associated with the
-                molecule. This is typically the response being studied.
-                E.g. Boiling point, Selectivity etc. Default is None.
-            mol_descriptor_val (numpy ndarray): Descriptor value for the
-                molecule. Must be numpy array or list. Default is None.
-            mol_src (str):
-                Source file or SMILES string to load molecule. Acceptable files:
-                -> .pdb file
-                -> .txt file with SMILE string in first column, first row and
-                        (optionally) property in second column, first row.
-                Default is None.
-                If provided mol_graph is attempted to be loaded from it.
-            mol_smiles (str): SMILES string for molecule. If provided, mol_graph
-                is loaded from it. If mol_text not set in keyword argument,
-                this string is used to set it.
-        """
-        self.mol_graph = mol_graph
-        self.mol_text = mol_text
-        self.mol_property_val = mol_property_val
-        self.descriptor = (
-            Descriptor()
-            if mol_descriptor_val is None
-            else Descriptor(value=np.array(mol_descriptor_val))
-        )
-        if mol_src is not None:
-            try:
-                self._set_molecule_from_file(mol_src)
-            except LoadingError as e:
-                raise e
-        if mol_smiles is not None:
-            try:
-                self._set_molecule_from_smiles(mol_smiles)
-            except LoadingError as e:
-                raise e
-
-    def _set_molecule_from_pdb(self, fpath):
-        """Set the mol_graph attribute from a PDB file.
-        If self.mol_text is not set, it is set to the base of the filname.
-
-        Args:
-            fpath (str): Path of PDB file.
-
-        Raises:
-             LoadingError: If Molecule cannot be loaded from PDB file.
-        """
-        try:
-            self.mol_graph = Chem.MolFromPDBFile(fpath)
-        except Exception:
-            raise LoadingError(f'{fpath} could not be loaded')
-        if self.mol_graph is None:
-            raise LoadingError(f'{fpath} could not be loaded')
-        if self.mol_text is None:
-            self.mol_text = os.path.basename(fpath).split('.')[0]
-
-    def _set_molecule_from_smiles(self, mol_smiles):
-        """Set the mol_graph attribute from smiles string.
-        If self.mol_text is not set, it is set to the smiles string.
-
-        Args:
-            mol_smiles (str): SMILES string for molecule. If provided,
-                mol_graph is loaded from it. If mol_text not set in keyword
-                argument, this string is used to set it.
-
-        Raises:
-             LoadingError: If Molecule cannot be loaded from SMILES string.
-        """
-        try:
-            self.mol_graph = Chem.MolFromSmiles(mol_smiles)
-        except Exception:
-            raise LoadingError(f'{mol_smiles} could not be loaded')
-        if self.mol_graph is None:
-            raise LoadingError(f'{mol_smiles} could not be loaded')
-        if self.mol_text is None:
-            self.mol_text = mol_smiles
-
-    def _set_molecule_from_file(self, mol_src):
-        """Load molecule graph from file.
-
-        Args:
-            mol_src (str): Source file or SMILES string to load molecule.
-                Acceptable files are
-                -> .pdb file
-                -> .txt file with SMILE string in first column, first row.
-
-        Raises:
-             LoadingError: If Molecule cannot be loaded from source.
-        """
-        if os.path.isfile(mol_src):
-            mol_fname, extension = os.path.basename(mol_src).split(".")
-            if extension == "pdb":
-                try:
-                    self._set_molecule_from_pdb(mol_src)
-                except LoadingError as e:
-                    raise e
-            elif extension == "txt":
-                with open(mol_src, "r") as fp:
-                    mol_smiles = fp.readline().split()[0]
-                try:
-                    self._set_molecule_from_smiles(mol_smiles)
-                except LoadingError as e:
-                    raise e
-        else:
-            raise LoadingError(message=f"File {mol_src} does not exist.")
-
-    def set_descriptor(
-        self,
-        arbitrary_descriptor_val=None,
-        fingerprint_type=None,
-        fingerprint_params=None,
-    ):
-        """Sets molecular descriptor attribute.
-
-        Args:
-            arbitrary_descriptor_val (np.array or list): Arbitrary descriptor
-                vector. Default is None.
-            fingerprint_type (str): String label specifying which fingerprint
-                to use. Default is None.
-            fingerprint_params (dict): Additional parameters for modifying
-                fingerprint defaults. Default is None.
-        """
-        if arbitrary_descriptor_val is not None:
-            self.descriptor.set_manually(arbitrary_descriptor_val)
-        elif fingerprint_type is not None:
-            if self.mol_graph is None:
-                raise ValueError(
-                    "Molecular graph not present. "
-                    "Fingerprint cannot be calculated."
-                )
-            self.descriptor.make_fingerprint(
-                self.mol_graph,
-                fingerprint_type=fingerprint_type,
-                fingerprint_params=fingerprint_params,
-            )
-        else:
-            raise ValueError(f"No descriptor vector were passed.")
-
-    def get_descriptor_val(self):
-        """Get value of molecule descriptor.
-
-        Returns:
-            np.ndarray: value(s) of the descriptor.
-
-        """
-        return self.descriptor.to_numpy()
-
-    def match_fingerprint_from(self, reference_mol):
-        """
-        If target_mol.descriptor is a fingerprint, this method will try
-        to calculate the fingerprint of the self molecules.
-        If this fails because of the absence of mol_graph attribute in
-        target_molecule, a ValueError is raised.
-
-        Args:
-            reference_mol (AIMSim.ops Molecule): Target molecule. Fingerprint
-            of this molecule is used as the reference.
-
-        Raises:
-            ValueError
-        """
-        if reference_mol.descriptor.is_fingerprint():
-            try:
-                self.set_descriptor(
-                    fingerprint_type=reference_mol.descriptor.get_label(),
-                    fingerprint_params=reference_mol.descriptor.get_params(),
-                )
-            except ValueError as e:
-                raise ValueError(f" For {self.mol_text}") from e
-
-    def get_similarity_to(self, target_mol, similarity_measure):
-        """Get a similarity metric to a target molecule
-
-        Args:
-            target_mol (AIMSim.ops Molecule): Target molecule. Similarity
-                score is with respect to this molecule
-            similarity_measure (AIMSim.ops SimilarityMeasure). The similarity
-                metric used.
-
-        Returns:
-            similarity_score (float): Similarity coefficient by the chosen
-                method.
-
-        Raises
-        ------
-            NotInitializedError
-                If target_molecule has uninitialized descriptor. See note.
-        """
-        try:
-            return similarity_measure(self.descriptor, target_mol.descriptor)
-        except NotInitializedError as e:
-            raise NotInitializedError(
-                "Similarity could not be calculated.") from e
-
-    def get_name(self):
-        return self.mol_text
-
-    def get_mol_property_val(self):
-        return self.mol_property_val
-
-    def draw(self, fpath=None, **kwargs):
-        """Draw or molecule graph.
-
-        Args:
-            fpath (str): Path of file to store image. If None, image is
-                displayed in io as a Tkinter windows. Default is None.
-            kwargs (keyword arguments): Arguments to modify plot properties.
-        """
-        if fpath is None:
-            Draw.ShowMol(self.mol_graph, **kwargs)
-        else:
-            Draw.MolToFile(self.mol_graph, fpath, **kwargs)
-
-    @staticmethod
-    def is_same(source_molecule, target_molecule):
-        """Check if the target_molecule is a duplicate of source_molecule.
-
-        Args:
-            source_molecule (AIMSim.chemical_datastructures Molecule): Source
-                molecule to compare.
-            target_molecule (AIMSim.chemical_datastructures Molecule): Target
-                molecule to compare.
-
-        Returns:
-            bool: True if the molecules are the same.
-
-        """
-        return source_molecule.mol_text == target_molecule.mol_text
+"""Abstraction of RDKit molecule with relevant property manipulation methods."""
+import os.path
+
+import numpy as np
+from rdkit import Chem
+from rdkit.Chem import Draw
+
+from aimsim.exceptions import *
+from aimsim.ops.descriptor import Descriptor
+
+
+class Molecule:
+    """An abstraction of a molecule
+
+    Attributes:
+        mol_graph (RDKIT mol object): Graph-level information of molecule.
+            Implemented as an RDKIT mol object.
+        mol_text (str): Text identifier of the molecule.
+        mol_property_val (float): Some property associated with the molecule.
+                This is typically the response being studied.
+                E.g. Boiling point, Selectivity etc.
+        descriptor (Descriptor object): Vector representation of a molecule.
+             Commonly a fingerprint.
+
+    Methods:
+        set_descriptor(
+            arbitrary_descriptor_val=None,
+            fingerprint_type=None,
+            fingerprint_params=None): Set the descriptor value either by passing
+            an arbitrary value or by specifying a fingerprint that will be
+            generated.
+        get_descriptor_val(): Get the descriptor value as an numpy array.
+        match_fingerprint_from(reference_mol): Generate the same fingerprint
+            as the reference_mol.
+        get_similarity_to(target_mol, similarity_measure): Get the similarity
+            to target_mol using a similarity_measure of choice.
+        get_name(): Get the mol_text attribute.
+        get_mol_property_val(): Get mol_property_val attribute.
+        draw(fpath=None, **kwargs): Draw the molecule.
+        is_same(source_molecule, target_molecule): Static method used to check
+            equivalence of two molecules.
+
+    """
+
+    def __init__(
+        self,
+        mol_graph=None,
+        mol_text=None,
+        mol_property_val=None,
+        mol_descriptor_val=None,
+        mol_src=None,
+        mol_smiles=None,
+    ):
+        """Constructor
+
+        Args:
+            mol_graph (RDKIT mol object): Graph-level information of molecule.
+                Implemented as an RDKIT mol object. Default is None.
+            mol_text (str): Text identifier of the molecule. Default is None.
+                Identifiers can be:
+                ------------------
+                1. Name of the molecule.
+                2. SMILES string representing the molecule.
+            mol_property_val (float): Some property associated with the
+                molecule. This is typically the response being studied.
+                E.g. Boiling point, Selectivity etc. Default is None.
+            mol_descriptor_val (numpy ndarray): Descriptor value for the
+                molecule. Must be numpy array or list. Default is None.
+            mol_src (str):
+                Source file or SMILES string to load molecule. Acceptable files:
+                -> .pdb file
+                -> .txt file with SMILE string in first column, first row and
+                        (optionally) property in second column, first row.
+                Default is None.
+                If provided mol_graph is attempted to be loaded from it.
+            mol_smiles (str): SMILES string for molecule. If provided, mol_graph
+                is loaded from it. If mol_text not set in keyword argument,
+                this string is used to set it.
+        """
+        self.mol_graph = mol_graph
+        self.mol_text = mol_text
+        self.mol_property_val = mol_property_val
+        self.descriptor = (
+            Descriptor()
+            if mol_descriptor_val is None
+            else Descriptor(value=np.array(mol_descriptor_val))
+        )
+        if mol_src is not None:
+            try:
+                self._set_molecule_from_file(mol_src)
+            except LoadingError as e:
+                raise e
+        if mol_smiles is not None:
+            try:
+                self._set_molecule_from_smiles(mol_smiles)
+            except LoadingError as e:
+                raise e
+
+    def _set_molecule_from_pdb(self, fpath):
+        """Set the mol_graph attribute from a PDB file.
+        If self.mol_text is not set, it is set to the base of the filname.
+
+        Args:
+            fpath (str): Path of PDB file.
+
+        Raises:
+             LoadingError: If Molecule cannot be loaded from PDB file.
+        """
+        try:
+            self.mol_graph = Chem.MolFromPDBFile(fpath)
+        except Exception:
+            raise LoadingError(f'{fpath} could not be loaded')
+        if self.mol_graph is None:
+            raise LoadingError(f'{fpath} could not be loaded')
+        if self.mol_text is None:
+            self.mol_text = os.path.basename(fpath).split('.')[0]
+
+    def _set_molecule_from_smiles(self, mol_smiles):
+        """Set the mol_graph attribute from smiles string.
+        If self.mol_text is not set, it is set to the smiles string.
+
+        Args:
+            mol_smiles (str): SMILES string for molecule. If provided,
+                mol_graph is loaded from it. If mol_text not set in keyword
+                argument, this string is used to set it.
+
+        Raises:
+             LoadingError: If Molecule cannot be loaded from SMILES string.
+        """
+        try:
+            self.mol_graph = Chem.MolFromSmiles(mol_smiles)
+        except Exception:
+            raise LoadingError(f'{mol_smiles} could not be loaded')
+        if self.mol_graph is None:
+            raise LoadingError(f'{mol_smiles} could not be loaded')
+        if self.mol_text is None:
+            self.mol_text = mol_smiles
+
+    def _set_molecule_from_file(self, mol_src):
+        """Load molecule graph from file.
+
+        Args:
+            mol_src (str): Source file or SMILES string to load molecule.
+                Acceptable files are
+                -> .pdb file
+                -> .txt file with SMILE string in first column, first row.
+
+        Raises:
+             LoadingError: If Molecule cannot be loaded from source.
+        """
+        if os.path.isfile(mol_src):
+            mol_fname, extension = os.path.basename(mol_src).split(".")
+            if extension == "pdb":
+                try:
+                    self._set_molecule_from_pdb(mol_src)
+                except LoadingError as e:
+                    raise e
+            elif extension == "txt":
+                with open(mol_src, "r") as fp:
+                    mol_smiles = fp.readline().split()[0]
+                try:
+                    self._set_molecule_from_smiles(mol_smiles)
+                except LoadingError as e:
+                    raise e
+        else:
+            raise LoadingError(message=f"File {mol_src} does not exist.")
+
+    def set_descriptor(
+        self,
+        arbitrary_descriptor_val=None,
+        fingerprint_type=None,
+        fingerprint_params=None,
+    ):
+        """Sets molecular descriptor attribute.
+
+        Args:
+            arbitrary_descriptor_val (np.array or list): Arbitrary descriptor
+                vector. Default is None.
+            fingerprint_type (str): String label specifying which fingerprint
+                to use. Default is None.
+            fingerprint_params (dict): Additional parameters for modifying
+                fingerprint defaults. Default is None.
+        """
+        if arbitrary_descriptor_val is not None:
+            self.descriptor.set_manually(arbitrary_descriptor_val)
+        elif fingerprint_type is not None:
+            if self.mol_graph is None:
+                raise ValueError(
+                    "Molecular graph not present. "
+                    "Fingerprint cannot be calculated."
+                )
+            self.descriptor.make_fingerprint(
+                self.mol_graph,
+                fingerprint_type=fingerprint_type,
+                fingerprint_params=fingerprint_params,
+            )
+        else:
+            raise ValueError(f"No descriptor vector were passed.")
+
+    def get_descriptor_val(self):
+        """Get value of molecule descriptor.
+
+        Returns:
+            np.ndarray: value(s) of the descriptor.
+
+        """
+        return self.descriptor.to_numpy()
+
+    def match_fingerprint_from(self, reference_mol):
+        """
+        If target_mol.descriptor is a fingerprint, this method will try
+        to calculate the fingerprint of the self molecules.
+        If this fails because of the absence of mol_graph attribute in
+        target_molecule, a ValueError is raised.
+
+        Args:
+            reference_mol (AIMSim.ops Molecule): Target molecule. Fingerprint
+            of this molecule is used as the reference.
+
+        Raises:
+            ValueError
+        """
+        if reference_mol.descriptor.is_fingerprint():
+            try:
+                self.set_descriptor(
+                    fingerprint_type=reference_mol.descriptor.get_label(),
+                    fingerprint_params=reference_mol.descriptor.get_params(),
+                )
+            except ValueError as e:
+                raise ValueError(f" For {self.mol_text}") from e
+
+    def get_similarity_to(self, target_mol, similarity_measure):
+        """Get a similarity metric to a target molecule
+
+        Args:
+            target_mol (AIMSim.ops Molecule): Target molecule. Similarity
+                score is with respect to this molecule
+            similarity_measure (AIMSim.ops SimilarityMeasure). The similarity
+                metric used.
+
+        Returns:
+            similarity_score (float): Similarity coefficient by the chosen
+                method.
+
+        Raises
+        ------
+            NotInitializedError
+                If target_molecule has uninitialized descriptor. See note.
+        """
+        try:
+            return similarity_measure(self.descriptor, target_mol.descriptor)
+        except NotInitializedError as e:
+            raise NotInitializedError(
+                "Similarity could not be calculated.") from e
+
+    def get_name(self):
+        return self.mol_text
+
+    def get_mol_property_val(self):
+        return self.mol_property_val
+
+    def draw(self, fpath=None, **kwargs):
+        """Draw or molecule graph.
+
+        Args:
+            fpath (str): Path of file to store image. If None, image is
+                displayed in io as a Tkinter windows. Default is None.
+            kwargs (keyword arguments): Arguments to modify plot properties.
+        """
+        if fpath is None:
+            Draw.ShowMol(self.mol_graph, **kwargs)
+        else:
+            Draw.MolToFile(self.mol_graph, fpath, **kwargs)
+
+    @staticmethod
+    def is_same(source_molecule, target_molecule):
+        """Check if the target_molecule is a duplicate of source_molecule.
+
+        Args:
+            source_molecule (AIMSim.chemical_datastructures Molecule): Source
+                molecule to compare.
+            target_molecule (AIMSim.chemical_datastructures Molecule): Target
+                molecule to compare.
+
+        Returns:
+            bool: True if the molecules are the same.
+
+        """
+        return source_molecule.mol_text == target_molecule.mol_text
```

### Comparing `aimsim-2.0.2/aimsim/exceptions.py` & `aimsim-2.0.3/aimsim/exceptions.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-class NotInitializedError(AttributeError):
-    """Used when a class is called without proper initialization."""
-
-    def __init__(self, message=None):
-        self.message = message
-        super().__init__(message)
-
-
-class MordredCalculatorError(RuntimeError):
-    """Used in descriptor.py when the Mordred property calculator fails."""
-
-    def __init__(self, message=None):
-        self.message = message
-        super().__init__(message)
-
-
-class MordredNotInstalledWarning(RuntimeWarning):
-    """Used in descriptor.py when the Mordred property calculator is not present."""
-
-    def __init__(self, message=None):
-        self.message = message
-        super().__init__(message)
-
-
-class InvalidConfigurationError(IOError):
-    """Used when a configuration parameter is invalid."""
-
-    def __init__(self, message=None):
-        self.message = message
-        super().__init__(message)
-
-
-class LoadingError(ValueError):
-    """Used when an object cannot be loaded"""
-
-    def __init__(self, message=None):
-        self.message = message
-        super().__init__(message)
+class NotInitializedError(AttributeError):
+    """Used when a class is called without proper initialization."""
+
+    def __init__(self, message=None):
+        self.message = message
+        super().__init__(message)
+
+
+class MordredCalculatorError(RuntimeError):
+    """Used in descriptor.py when the Mordred property calculator fails."""
+
+    def __init__(self, message=None):
+        self.message = message
+        super().__init__(message)
+
+
+class MordredNotInstalledWarning(RuntimeWarning):
+    """Used in descriptor.py when the Mordred property calculator is not present."""
+
+    def __init__(self, message=None):
+        self.message = message
+        super().__init__(message)
+
+
+class InvalidConfigurationError(IOError):
+    """Used when a configuration parameter is invalid."""
+
+    def __init__(self, message=None):
+        self.message = message
+        super().__init__(message)
+
+
+class LoadingError(ValueError):
+    """Used when an object cannot be loaded"""
+
+    def __init__(self, message=None):
+        self.message = message
+        super().__init__(message)
```

### Comparing `aimsim-2.0.2/aimsim/ops/similarity_measures.py` & `aimsim-2.0.3/aimsim/ops/similarity_measures.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,2125 +1,2125 @@
-"""This module contains methods to find similarities between molecules."""
-from functools import lru_cache
-import numpy as np
-from rdkit import DataStructs
-from scipy.spatial.distance import cosine as scipy_cosine
-
-from aimsim.ops import Descriptor
-from aimsim.exceptions import InvalidConfigurationError
-
-SMALL_NUMBER = 1e-10
-
-
-class SimilarityMeasure:
-    def __init__(self, metric):
-        if metric.lower() in ["l0_similarity"]:
-            self.metric = "l0_similarity"
-            self.type_ = "continuous"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in [
-            "l1_similarity",
-            "manhattan_similarity",
-            "taxicab_similarity",
-            "city_block_similarity",
-            "snake_similarity",
-        ]:
-            self.metric = "l1_similarity"
-            self.type_ = "continuous"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["l2_similarity", "euclidean_similarity"]:
-            self.metric = "l2_similarity"
-            self.type_ = "continuous"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["cosine", "driver-kroeber", "ochiai"]:
-            self.metric = "cosine"
-            self.type_ = "discrete"
-            # angular distance
-            self.to_distance = lambda x: np.arccos(x) / np.pi
-
-        elif metric.lower() in ["dice", "sorenson", "gleason"]:
-            self.metric = "dice"
-            self.type_ = "discrete"
-            # convert to jaccard for distance
-            self.to_distance = lambda x: 1 - x / (2 - x)
-
-        elif metric.lower() in ["dice_2"]:
-            self.metric = "dice_2"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["dice_3"]:
-            self.metric = "dice_3"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["tanimoto", "jaccard-tanimoto"]:
-            self.metric = "tanimoto"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["simple_matching", "sokal-michener", "rand"]:
-            self.metric = "simple_matching"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["rogers-tanimoto"]:
-            self.metric = "rogers_tanimoto"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["russel-rao"]:
-            self.metric = "russel_rao"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["forbes"]:
-            self.metric = "forbes"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["simpson"]:
-            self.metric = "simpson"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["braun-blanquet"]:
-            self.metric = "braun_blanquet"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["baroni-urbani-buser"]:
-            self.metric = "baroni_urbani_buser"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["kulczynski"]:
-            self.metric = "kulczynski"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["sokal-sneath", "sokal-sneath_1"]:
-            self.metric = "sokal_sneath"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in [
-            "sokal-sneath_2",
-            "sokal-sneath-2",
-            "symmetric_sokal_sneath",
-            "symmetric-sokal-sneath",
-        ]:
-            self.metric = "symmetric_sokal_sneath"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["sokal-sneath-3", "sokal-sneath_3"]:
-            self.metric = "sokal_sneath_3"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["sokal-sneath-4", "sokal-sneath_4"]:
-            self.metric = "sokal_sneath_4"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["jaccard"]:
-            self.metric = "jaccard"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["faith"]:
-            self.metric = "faith"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["michael"]:
-            self.metric = "michael"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["mountford"]:
-            self.metric = "mountford"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["rogot-goldberg"]:
-            self.metric = "rogot_goldberg"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["hawkins-dotson"]:
-            self.metric = "hawkins_dotson"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["maxwell-pilliner"]:
-            self.metric = "maxwell_pilliner"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["harris-lahey"]:
-            self.metric = "harris_lahey"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["consonni-todeschini-1", "consonni-todeschini_1"]:
-            self.metric = "consonni_todeschini_1"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["consonni-todeschini-2", "consonni-todeschini_2"]:
-            self.metric = "consonni_todeschini_2"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["consonni-todeschini-3", "consonni-todeschini_3"]:
-            self.metric = "consonni_todeschini_3"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["consonni-todeschini-4", "consonni-todeschini_4"]:
-            self.metric = "consonni_todeschini_4"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["consonni-todeschini-5", "consonni-todeschini_5"]:
-            self.metric = "consonni_todeschini_5"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["austin-colwell"]:
-            self.metric = "austin_colwell"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["yule-1", "yule_1"]:
-            self.metric = "yule_1"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["yule-2", "yule_2"]:
-            self.metric = "yule_2"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["fossum", "holiday-fossum", "holiday_fossum"]:
-            self.metric = "fossum"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["dennis", "holiday-dennis", "holiday_dennis"]:
-            self.metric = "dennis"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["cole-1", "cole_1"]:
-            self.metric = "cole_1"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["cole-2", "cole_2"]:
-            self.metric = "cole_2"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["dispersion", "choi"]:
-            self.metric = "dispersion"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["goodman-kruskal", "goodman_kruskal"]:
-            self.metric = "goodman_kruskal"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["pearson-heron", "pearson_heron"]:
-            self.metric = "pearson_heron"
-            self.type_ = "discrete"
-            self.to_distance = lambda x: 1 - x
-
-        elif metric.lower() in ["sorgenfrei"]:
-            self.metric = "sorgenfrei"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["cohen"]:
-            self.metric = "cohen"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["peirce_1", "peirce-1"]:
-            self.metric = "peirce_1"
-            self.type_ = "discrete"
-
-        elif metric.lower() in ["peirce_2", "peirce-2"]:
-            self.metric = "peirce_2"
-            self.type_ = "discrete"
-
-        else:
-            raise ValueError(f"Similarity metric: {metric} is not implemented")
-        self.normalize_fn = {"shift_": 0.0, "scale_": 1.0}
-        self.label_ = metric
-
-    def __call__(self, mol1_descriptor, mol2_descriptor):
-        """Compare two descriptors.
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            similarity_ (float): Similarity value
-        """
-        if not self._validate_fprint(mol1_descriptor) or not self._validate_fprint(
-            mol2_descriptor
-        ):
-            raise ValueError(
-                f"Molecule descriptor ({mol1_descriptor.label_}) has no active bits."
-            )
-        similarity_ = None
-        if self.metric == "l0_similarity":
-            try:
-                similarity_ = self._get_vector_norm_similarity(
-                    mol1_descriptor, mol2_descriptor, ord=0
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "l1_similarity":
-            try:
-                similarity_ = self._get_vector_norm_similarity(
-                    mol1_descriptor, mol2_descriptor, ord=1
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "l2_similarity":
-            try:
-                similarity_ = self._get_vector_norm_similarity(
-                    mol1_descriptor, mol2_descriptor, ord=2
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "austin_colwell":
-            try:
-                similarity_ = self._get_austin_colwell(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "baroni_urbani_buser":
-            try:
-                similarity_ = self._get_baroni_urbani_buser(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "braun_blanquet":
-            try:
-                similarity_ = self._get_braun_blanquet(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "cohen":
-            try:
-                similarity_ = self._get_cohen(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "cole_1":
-            try:
-                similarity_ = self._get_cole_1(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "cole_2":
-            try:
-                similarity_ = self._get_cole_2(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "consonni_todeschini_1":
-            try:
-                similarity_ = self._get_consonni_todeschini_1(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "consonni_todeschini_2":
-            try:
-                similarity_ = self._get_consonni_todeschini_2(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "consonni_todeschini_3":
-            try:
-                similarity_ = self._get_consonni_todeschini_3(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "consonni_todeschini_4":
-            try:
-                similarity_ = self._get_consonni_todeschini_4(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "consonni_todeschini_5":
-            try:
-                similarity_ = self._get_consonni_todeschini_5(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "cosine":
-            try:
-                similarity_ = self._get_cosine_similarity(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "dennis":
-            try:
-                similarity_ = self._get_dennis(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "dice":
-            try:
-                similarity_ = self._get_dice(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "dice_2":
-            try:
-                similarity_ = self._get_dice_2(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "dice_3":
-            try:
-                similarity_ = self._get_dice_3(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "dispersion":
-            try:
-                similarity_ = self._get_dispersion(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "faith":
-            try:
-                similarity_ = self._get_faith(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "forbes":
-            try:
-                similarity_ = self._get_forbes(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "fossum":
-            try:
-                similarity_ = self._get_fossum(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "goodman_kruskal":
-            try:
-                similarity_ = self._get_goodman_kruskal(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "harris_lahey":
-            try:
-                similarity_ = self._get_harris_lahey(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "hawkins_dotson":
-            try:
-                similarity_ = self._get_hawkins_dotson(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "jaccard":
-            try:
-                similarity_ = self._get_jaccard(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "kulczynski":
-            try:
-                similarity_ = self._get_kulczynski(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-        elif self.metric == "maxwell_pilliner":
-            try:
-                similarity_ = self._get_maxwell_pilliner(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "michael":
-            try:
-                similarity_ = self._get_michael(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "mountford":
-            try:
-                similarity_ = self._get_mountford(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "pearson_heron":
-            try:
-                similarity_ = self._get_pearson_heron(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "peirce_1":
-            try:
-                similarity_ = self._get_peirce_1(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "peirce_2":
-            try:
-                similarity_ = self._get_peirce_2(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "rogers_tanimoto":
-            try:
-                similarity_ = self._get_rogers_tanimoto(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "rogot_goldberg":
-            try:
-                similarity_ = self._get_rogot_goldberg(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "russel_rao":
-            try:
-                similarity_ = self._get_russel_rao(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "simple_matching":
-            try:
-                similarity_ = self._get_simple_matching(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "simpson":
-            try:
-                similarity_ = self._get_simpson(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "sokal_sneath":
-            try:
-                similarity_ = self._get_sokal_sneath(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "symmetric_sokal_sneath":
-            try:
-                similarity_ = self._get_symmetric_sokal_sneath(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "sokal_sneath_3":
-            try:
-                similarity_ = self._get_sokal_sneath_3(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "sokal_sneath_4":
-            try:
-                similarity_ = self._get_sokal_sneath_4(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "sorgenfrei":
-            try:
-                similarity_ = self._get_sorgenfrei(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "tanimoto":
-            try:
-                similarity_ = DataStructs.TanimotoSimilarity(
-                    mol1_descriptor.to_rdkit(), mol2_descriptor.to_rdkit()
-                )
-            except ValueError as e:
-                raise ValueError(
-                    "Tanimoto similarity is only useful for bit strings "
-                    "generated from fingerprints. Consider using "
-                    "other similarity measures for arbitrary vectors."
-                )
-        elif self.metric == "yule_1":
-            try:
-                similarity_ = self._get_yule_1(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        elif self.metric == "yule_2":
-            try:
-                similarity_ = self._get_yule_2(mol1_descriptor, mol2_descriptor)
-            except ValueError as e:
-                raise e
-
-        else:
-            raise ValueError(f"{self.metric} could not be implemented")
-
-        return similarity_
-
-    def _get_vector_norm_similarity(self, mol1_descriptor, mol2_descriptor, ord):
-        """Calculate the norm based similarity between two molecules.
-        This is defined as:
-        Norm similarity (order n) = 1 / (1 + n-norm(A - B)
-        where n-norm(A - B) represents the n-th order norm of the difference
-        of two vector A and B.
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-            ord (int): Order of the norm
-
-        Returns:
-            (float): Norm similarity value
-        """
-        arr1 = mol1_descriptor.to_numpy()
-        arr2 = mol2_descriptor.to_numpy()
-        if len(arr1) != len(arr2):
-            try:
-                arr1, arr2 = Descriptor.fold_to_equal_length(
-                    mol1_descriptor, mol2_descriptor
-                )
-            except ValueError as e:
-                raise ValueError(
-                    "Fingerprints are of unequal length and cannot be folded."
-                ) from e
-
-        norm_ = np.linalg.norm(arr1 - arr2, ord=ord)
-        similarity_ = 1 / (1 + norm_)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_austin_colwell(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Austin-Colwell similarity between two molecules.
-        This is defined for two binary arrays as:
-        Austin-Colwell similarity = (2 / pi) * arcsin(sqrt( (a + d) / p ))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Austin-Colwell similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Austin-Colwell similarity is only useful for "
-                "bit strings generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        similarity_ = (2 / np.pi) * np.arcsin(np.sqrt((a + d) / p))
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_baroni_urbani_buser(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Baroni-Urbani-Buser similarity between two molecules.
-        This is defined for two binary arrays as:
-        Baroni-Urbani-Buser similarity = (sqrt(a * d) + a)
-                                         / (sqrt(a * d) + a + b + c)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Baroni-Urbani-Buser similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Baroni-Urbani-Buser similarity is only useful for "
-                "bit strings generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if d == p:
-            return 1.0
-        similarity_ = (np.sqrt(a * d) + a) / (np.sqrt(a * d) + a + b + c)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_braun_blanquet(self, mol1_descriptor, mol2_descriptor):
-        """Calculate braun-blanquet similarity between two molecules.
-        This is defined for two binary arrays as:
-        Braun-Blanquet Similarity = a / max{(a + b), (a + c)}
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Braun-Blanquet similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Braun-Blanquet similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        if a < SMALL_NUMBER:
-            return 0.0
-        similarity_ = a / max((a + b), (a + c))
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_cohen(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Cohen similarity between two molecules.
-        This is defined for two binary arrays as:
-        Cohen Similarity = 2*(a*d - b*c) / ((a + b)*(b + d) + (a + c)*(c + d))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Cohen similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Cohen similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        denominator_ = (a + b) * (b + d) + (a + c) * (c + d)
-        if a == p or d == p:
-            return 1.0
-        if denominator_ < SMALL_NUMBER:
-            return 0.0
-
-        similarity_ = 2 * (a * d - b * c) / denominator_
-        self.normalize_fn["shift_"] = 1.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_cole_1(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Cole(1) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Cole(1) Similarity = (a*d - b*c) / ((a + c)*(c + d))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Cole(1)  similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Cole(1) similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        denominator = (a + c) * (c + d)
-        if denominator < SMALL_NUMBER:
-            return 0.0
-        similarity_ = (a * d - b * c) / denominator
-        self.normalize_fn["shift_"] = p - 1
-        self.normalize_fn["scale_"] = p
-        return self._normalize(similarity_)
-
-    def _get_cole_2(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Cole(2) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Cole(2) Similarity = (a*d - b*c) / ((a + b)*(b + d))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Cole(2)  similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Cole(2) similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        denominator = (a + b) * (b + d)
-        if denominator < SMALL_NUMBER:
-            return 0.0
-        similarity_ = (a * d - b * c) / denominator
-        self.normalize_fn["shift_"] = p - 1
-        self.normalize_fn["scale_"] = p
-        return self._normalize(similarity_)
-
-    def _get_consonni_todeschini_1(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Consonni-Todeschini(1) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Consonni-Todeschini(1) similarity = ln(1 + a + d) / ln(1 + p)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Consonni-Todeschini(1)  similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Consonni-Todeschini(1)  similarity is only useful for "
-                "bit strings generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        similarity_ = np.log(1 + a + d) / np.log(1 + p)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_consonni_todeschini_2(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Consonni-Todeschini(2) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Consonni-Todeschini(2) similarity =
-            (ln(1 + p) - ln(1 + b + c)) / ln(1 + p)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Consonni-Todeschini(2)  similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Consonni-Todeschini(2) similarity is only useful for "
-                "bit strings generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        similarity_ = (np.log(1 + p) - np.log(1 + b + c)) / np.log(1 + p)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_consonni_todeschini_3(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Consonni-Todeschini(3) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Consonni-Todeschini(3) similarity = ln(1 + a) / ln(1 + p)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Consonni-Todeschini(3)  similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Consonni-Todeschini(3) similarity is only useful for "
-                "bit strings generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        similarity_ = np.log(1 + a) / np.log(1 + p)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_consonni_todeschini_4(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Consonni-Todeschini(4) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Consonni-Todeschini(4) similarity = ln(1 + a) / ln(1 + a + b + c)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Consonni-Todeschini(4)  similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Consonni-Todeschini(4) similarity is only useful for "
-                "bit strings generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        if np.log(1 + a + b + c) == 0:
-            raise InvalidConfigurationError("Empty string supplied")
-        similarity_ = np.log(1 + a) / np.log(1 + a + b + c)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_consonni_todeschini_5(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Consonni-Todeschini(5) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Consonni-Todeschini(5) similarity = (ln(1 + a*d) - ln(1 + b*c))
-                                            / ln(1 + p**2 / 4)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Consonni-Todeschini(5)  similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Consonni-Todeschini(5) similarity is only useful for "
-                "bit strings generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        similarity_ = (np.log(1 + a * d) - np.log(1 + b * c)) / np.log(1 + (p**2) / 4)
-        self.normalize_fn["shift_"] = 1.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_cosine_similarity(self, mol1_descriptor, mol2_descriptor):
-        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        denominator = np.sqrt((a + b) * (a + c))
-        if denominator < SMALL_NUMBER:
-            return 0.0
-        similarity_ = a / denominator
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_dennis(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Dennis similarity between two molecules.
-        This is defined for two binary arrays as:
-        Dennis similarity = (a*d - b*c) / sqrt(p*(a + b)*(a + c))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Dennis similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Dennis similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        denominator = np.sqrt(p * (a + b) * (a + c))
-        if denominator < SMALL_NUMBER:
-            return 0.0
-        similarity_ = (a * d - b * c) / denominator
-        self.normalize_fn["shift_"] = np.sqrt(p) / 2
-        self.normalize_fn["scale_"] = 3 * np.sqrt(p) / 2
-        return self._normalize(similarity_)
-
-    def _get_dice(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Dice similarity between two molecules.
-        This is defined for two binary arrays as:
-        Dice similarity = 2a / (2a + b + c)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Dice similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Dice similarity is only useful for bit strings "
-                "generated from fingerprints, not {} and {}. Consider using "
-                "other similarity measures for arbitrary vectors.".format(
-                    mol1_descriptor.get_label(), mol2_descriptor.get_label()
-                )
-            )
-        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        if a < SMALL_NUMBER:
-            return 0.0
-        similarity_ = 2 * a / (2 * a + b + c)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_dice_2(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Dice(2) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Dice(2) similarity = a / (a + b)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Dice(2) similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Dice(2) similarity is only useful for bit strings "
-                "generated from fingerprints, not {} and {}. Consider using "
-                "other similarity measures for arbitrary vectors.".format(
-                    mol1_descriptor.get_label(), mol2_descriptor.get_label()
-                )
-            )
-        a, b, _, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        if a < SMALL_NUMBER:
-            return 0.0
-        similarity_ = a / (a + b)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_dice_3(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Dice(3) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Dice(3) similarity = a / (a + c)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Dice(3) similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Dice(3) similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, _, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
-
-        if a < SMALL_NUMBER:
-            return 0.0
-        similarity_ = a / (a + c)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_dispersion(self, mol1_descriptor, mol2_descriptor):
-        """Calculate dispersion similarity in Choi et al (2012)
-         between two molecules. This is defined for two binary arrays as:
-        dispersion similarity = (a*d - b*c) / p**2
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): dispersion similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Dispersion similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        similarity_ = (a * d - b * c) / p**2
-        self.normalize_fn["shift_"] = 1 / 4
-        self.normalize_fn["scale_"] = 1 / 2
-        return self._normalize(similarity_)
-
-    def _get_faith(self, mol1_descriptor, mol2_descriptor):
-        """Calculate faith similarity between two molecules.
-        This is defined for two binary arrays as:
-        Faith similarity = (a + 0.5*d) / p
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Faith similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Faith similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        similarity_ = (a + 0.5 * d) / p
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_forbes(self, mol1_descriptor, mol2_descriptor):
-        """Calculate forbes similarity between two molecules.
-        This is defined for two binary arrays as:
-        Forbes similarity = (p * a) / ((a + b) * (a + c))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Forbes similarity value
-
-        Note:
-            The Forbes similarity is normalized to [0, 1]
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Forbes similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        if (a + b) * (a + c) < SMALL_NUMBER or a < SMALL_NUMBER:
-            return 0.0
-        p = a + b + c + d
-        similarity_ = (p * a) / ((a + b) * (a + c) + SMALL_NUMBER)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = p / a
-        return self._normalize(similarity_)
-
-    def _get_fossum(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Fossum similarity between two molecules.
-        This is defined for two binary arrays as:
-        Fossum similarity = p * (a - 0.5)**2 / ((a + b) * (a + c))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Fossum similarity value
-
-        Note:
-            The similarity is normalized to [0, 1].
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Fossum similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        denominator = (a + b) * (a + c)
-        if denominator < SMALL_NUMBER:
-            return 0.0
-        p = a + b + c + d
-        similarity_ = p * (a - 0.5) ** 2 / denominator
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = (p - 0.5) ** 2 / p
-        return self._normalize(similarity_)
-
-    def _get_goodman_kruskal(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Goodman-Kruskal similarity between two molecules.
-        This is defined for two binary arrays as:
-        Goodman-Kruskal similarity =
-            (2 * min(a, d) - b - c) / (2 * min(a, d) + b + c)
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Goodman-Kruskal similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Goodman-Kruskal similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        min_a_d = np.min([a, d])
-        similarity_ = (2 * min_a_d - b - c) / (2 * min_a_d + b + c)
-        self.normalize_fn["shift_"] = 1.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_harris_lahey(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Harris-Lahey similarity between two molecules.
-        This is defined for two binary arrays as:
-        Harris-Lahey similarity =
-            (a/2) * (2*d + b + c)/(a + b + c)
-             + (d/2) * (2*a + b + c)/( b + c + d)
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Harris-Lahey similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Harris-Lahey similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        if (a + b + c) < SMALL_NUMBER or (b + c + d) < SMALL_NUMBER:
-            return 0.0
-
-        similarity_ = (a / 2) * (2 * d + b + c) / (a + b + c) + (d / 2) * (
-            2 * a + b + c
-        ) / (b + c + d)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = p
-        return self._normalize(similarity_)
-
-    def _get_hawkins_dotson(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Hawkins-Dotson similarity between two molecules.
-        This is defined for two binary arrays as:
-        Hawkins-Dotson similarity = 0.5 * (a / (a + b + c)
-                                           + d / (d + b + c))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Hawkins-Dotson similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Hawkins-Dotson similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        similarity_ = 0.5 * (
-            a / (a + b + c + SMALL_NUMBER) + d / (d + b + c + SMALL_NUMBER)
-        )
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_jaccard(self, mol1_descriptor, mol2_descriptor):
-        """Calculate jaccard similarity between two molecules.
-        This is defined for two binary arrays as:
-        jaccard similarity = 3*a / (3*a + b + c)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Jaccard similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Jaccard similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        if a < SMALL_NUMBER:
-            return 0.0
-        similarity_ = 3 * a / (3 * a + b + c)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_kulczynski(self, mol1_descriptor, mol2_descriptor):
-        """Calculate kulczynski similarity between two molecules.
-        This is defined for two binary arrays as:
-        kulczynski similarity = 0.5 * a / ((a + b) + (a + c))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Kulczynski similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Kulczynski similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        if a < SMALL_NUMBER:
-            return 0.0
-        similarity_ = 0.5 * a / ((a + b) + (a + c))
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_michael(self, mol1_descriptor, mol2_descriptor):
-        """Calculate michael similarity between two molecules.
-        This is defined for two binary arrays as:
-        michael similarity = 4*(a*d - b*c) / ((a + d)**2 + (b + c)**2)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Michael similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Michael similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p or (b + c) < SMALL_NUMBER:
-            return 1.0
-        similarity_ = 4 * (a * d - b * c) / ((a + d) ** 2 + (b + c) ** 2)
-        self.normalize_fn["shift_"] = 1.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_maxwell_pilliner(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Maxwell-Pilliner similarity between two molecules.
-        This is defined for two binary arrays as:
-        Maxwell-Pilliner similarity =
-            2*(a*d - b*c) / ((a + b)*(c + d) + (a + c)*(b + d))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Maxwell-Pilliner similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Maxwell-Pilliner similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        denominator = (a + b) * (c + d) + (a + c) * (b + d)
-        if a == p or d == p:
-            return 1.0
-        if denominator < SMALL_NUMBER:
-            return 0.0
-
-        similarity_ = 2 * (a * d - b * c) / denominator
-        self.normalize_fn["shift_"] = 1.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_mountford(self, mol1_descriptor, mol2_descriptor):
-        """Calculate mountford similarity between two molecules.
-        This is defined for two binary arrays as:
-        mountford similarity = 2*a / (a*b + a*c + 2*b*c)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Mountford similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Mountford similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        denominator = a * b + a * c + 2 * b * c
-        if denominator < SMALL_NUMBER:
-            return a / p
-        similarity_ = 2 * a / denominator
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_pearson_heron(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Pearson-Heron similarity between two molecules.
-        This is defined for two binary arrays as:
-        Pearson-Heron similarity =
-         (a*d - b*c)/sqrt((a + b)*(a + c)*(b + d)*(c + d))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Pearson-Heron similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Pearson-Heron similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        if b == p or c == p:
-            return 0.0
-        denominator_ = np.sqrt(
-            np.int64(a + b) * np.int64(a + c) * np.int64(b + d) * np.int64(c + d)
-        )
-        if denominator_ < SMALL_NUMBER:
-            return 0.0
-        similarity_ = (a * d - b * c) / denominator_
-        self.normalize_fn["shift_"] = 1.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_peirce_1(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Peirce(1) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Peirce(1) similarity = (a*d - b*c) / ((a + b)*(c + d))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Peirce(1) similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Peirce(1) similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        if b == p or c == p:
-            return 0.0
-        similarity_ = (a * d - b * c) / ((a + b) * (c + d) + SMALL_NUMBER)
-        self.normalize_fn["shift_"] = 1.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_peirce_2(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Peirce(2) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Peirce(2) similarity = (a*d - b*c) / ((a + c)*(b + d))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Peirce(2) similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Peirce(2) similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        if b == p or c == p:
-            return 0.0
-        similarity_ = (a * d - b * c) / ((a + c) * (b + d) + SMALL_NUMBER)
-        self.normalize_fn["shift_"] = 1.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_rogers_tanimoto(self, mol1_descriptor, mol2_descriptor):
-        """Calculate rogers-tanimoto similarity between two molecules.
-        This is defined for two binary arrays as:
-        Rogers-Tanimoto similarity = (a + d) / (p + b + c)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Rogers-Tanimoto similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Rogers-Tanimoto similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        similarity_ = (a + d) / (p + b + c)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_rogot_goldberg(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Rogot-Goldberg similarity between two molecules.
-        This is defined for two binary arrays as:
-        Rogot-Goldberg similarity = (a / (2*a + b + c)) + (d / (2*d + b + c))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Rogot-Goldberg  similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Rogot-Goldberg  similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        similarity_ = (a / (2 * a + b + c)) + (d / (2 * d + b + c))
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_russel_rao(self, mol1_descriptor, mol2_descriptor):
-        """Calculate russel-rao similarity between two molecules.
-        This is defined for two binary arrays as:
-        Russel-Rao = a / p
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Russel-Rao similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Russel-Rao similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        similarity_ = a / p
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_simple_matching(self, mol1_descriptor, mol2_descriptor):
-        """Calculate simple matching similarity between two molecules.
-        This is defined for two binary arrays as:
-        Simple Matching = (a + d) / p
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Simple Matching similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Simple Matching similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        similarity_ = (a + d) / p
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_simpson(self, mol1_descriptor, mol2_descriptor):
-        """Calculate simpson similarity between two molecules.
-        This is defined for two binary arrays as:
-        Simpson Similarity = a / min{(a + b), (a + c)}
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Simpson similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Simpson similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        if min((a + b), (a + c)) < SMALL_NUMBER or a < SMALL_NUMBER:
-            return 0.0
-        similarity_ = a / min((a + b), (a + c))
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_sokal_sneath(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Sokal-Sneath similarity between two molecules.
-        This is defined for two binary arrays as:
-        Sokal-Sneath similarity = a / (a + 2*b + 2*c)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Sokal-Sneath similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Sokal-Sneath similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        if a < SMALL_NUMBER:
-            return 0.0
-        similarity_ = a / (a + 2 * b + 2 * c)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_symmetric_sokal_sneath(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Symmetric Sokal-Sneath similarity between two molecules.
-        This is defined for two binary arrays as:
-        Symmetric Sokal-Sneath similarity = (2*a + 2*d) / (p + a + d)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Symmetric Sokal-Sneath similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Symmetric Sokal-Sneath similarity is only useful "
-                "for bit strings generated from fingerprints. Consider "
-                "using other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        similarity_ = (2 * a + 2 * d) / (p + a + d)
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_sokal_sneath_3(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Sokal-Sneath(3) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Sokal-Sneath(3) similarity =
-        (1/4) * (a/(a + b) + a/(a + c) + d/(b + d) + d/(c + d))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Sokal-Sneath(3) similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Sokal-Sneath(3) similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        if a < SMALL_NUMBER and d < SMALL_NUMBER:
-            return 0.0
-        similarity_ = (1 / 4) * (
-            a / (a + b + SMALL_NUMBER)
-            + a / (a + c + SMALL_NUMBER)
-            + d / (b + d + SMALL_NUMBER)
-            + d / (c + d + SMALL_NUMBER)
-        )
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_sokal_sneath_4(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Sokal-Sneath(4) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Sokal-Sneath(4) similarity =
-         a/sqrt((a + b) * (a + c)) * d/sqrt((b + d) *(c + d))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Sokal-Sneath(4) similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Sokal-Sneath(4) similarity is only useful for bit strings "
-                "generated from fingerprints. Consider using "
-                "other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        if a == p or d == p:
-            return 1.0
-        if a < SMALL_NUMBER or d < SMALL_NUMBER:
-            return 0.0
-        similarity_ = (
-            a
-            / (np.sqrt((a + b) * (a + c)) + SMALL_NUMBER)
-            * d
-            / (np.sqrt((b + d) * (c + d) + SMALL_NUMBER))
-        )
-
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_sorgenfrei(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Sorgenfrei similarity between two molecules.
-        This is defined for two binary arrays as:
-        Sorgenfrei similarity = a**2 / ((a + b)*(a + c))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Sorgenfrei similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Sorgenfrei similarity is only useful "
-                "for bit strings generated from fingerprints. Consider "
-                "using other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        if a < SMALL_NUMBER:
-            return 0.0
-        similarity_ = a**2 / ((a + b) * (a + c))
-        self.normalize_fn["shift_"] = 0.0
-        self.normalize_fn["scale_"] = 1.0
-        return self._normalize(similarity_)
-
-    def _get_yule_1(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Yule(1) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Symmetric Yule(1) similarity = (a*d - b*c) / (a*d + b*c)
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Yule(1) similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Yule(1) similarity is only useful "
-                "for bit strings generated from fingerprints. Consider "
-                "using other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        denominator = a * d + b * c + SMALL_NUMBER
-        if a == p or d == p or b * c < SMALL_NUMBER:
-            return 1.0
-        similarity_ = (a * d - b * c) / denominator
-        self.normalize_fn["shift_"] = 1.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_yule_2(self, mol1_descriptor, mol2_descriptor):
-        """Calculate Yule(2) similarity between two molecules.
-        This is defined for two binary arrays as:
-        Symmetric Yule(2) similarity = (sqrt(a*d) - sqrt(b*c))
-                                       / (sqrt(a*d) + sqrt(b*c))
-
-        Args:
-            mol1_descriptor (AIMSim.ops Descriptor)
-            mol2_descriptor (AIMSim.ops Descriptor)
-
-        Returns:
-            (float): Yule(2) similarity value
-        """
-        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
-            raise ValueError(
-                "Yule(2) similarity is only useful "
-                "for bit strings generated from fingerprints. Consider "
-                "using other similarity measures for arbitrary vectors."
-            )
-        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
-        p = a + b + c + d
-        denominator = np.sqrt(a * d) + np.sqrt(b * c) + SMALL_NUMBER
-        if a == p or d == p or b * c < SMALL_NUMBER:
-            return 1.0
-        similarity_ = (np.sqrt(a * d) - np.sqrt(b * c)) / denominator
-        self.normalize_fn["shift_"] = 1.0
-        self.normalize_fn["scale_"] = 2.0
-        return self._normalize(similarity_)
-
-    def _get_abcd(self, fingerprint1, fingerprint2):
-        """Get a, b, c, d, where:
-        a = #bits(bits(array 1) and bits(array 2))
-        b = #bits(bits(array 1) and bits(~array 2))
-        c = #bits(bits(~array 1) and bits(array 2))
-        d = #bits(bits(~array 1) and bits(~array 2)) // "~": complement operator
-        p = a + b + c + d = bits(array 1 or array 2)
-
-        Args:
-            fingerprint1 (Descriptor)
-            fingerprint2 (Descriptor)
-
-        Returns:
-            (tuple): (a, b, c, d)
-
-        Note:
-            If arrays of unequal lengths are passed, the larger array is folded
-            to the length of the smaller array.
-
-        """
-        arr1, arr2 = Descriptor.fold_to_equal_length(fingerprint1, fingerprint2)
-        not_arr1 = np.logical_not(arr1)
-        not_arr2 = np.logical_not(arr2)
-        a = np.sum(arr1 & arr2)
-        b = np.sum(arr1 & not_arr2)
-        c = np.sum(not_arr1 & arr2)
-        d = np.sum(not_arr1 & not_arr2)
-        assert (a + b + c + d) == arr1.size == arr2.size
-        return a, b, c, d
-
-    def _normalize(self, similarity_):
-        return (similarity_ + self.normalize_fn["shift_"]) / self.normalize_fn["scale_"]
-
-    def is_distance_metric(self):
-        """Check if the similarity measure is a distance metric.
-
-        Returns:
-            bool: True if it is a distance metric.
-        """
-        return hasattr(self, "to_distance")
-
-    @staticmethod
-    @lru_cache(maxsize=None)
-    def _validate_fprint(descriptor: Descriptor) -> bool:
-        """Are there any non-zero bits in this descriptor?
-
-        Args:
-            descriptor (Descriptor): AIMSim.ops.Descriptor object
-
-        Returns:
-            boolean: False if descriptor is all zero, True otherwise
-        """
-        return np.any(descriptor.to_numpy())
-
-    @staticmethod
-    def get_compatible_metrics():
-        """Return a dictionary with which types of metrics each fingerprint supports.
-
-        Returns:
-            dict: comptabile FP's: metrics
-        """
-        out = {}
-        fprints = Descriptor.get_all_supported_descriptors()
-        for fp in fprints:
-            if fp in [
-                "morgan_fingerprint",
-                "topological_fingerprint",
-                "daylight_fingerprint",
-                "maccs_keys",
-            ]:  # explicit bit vectors
-                out[fp] = SimilarityMeasure.get_supported_binary_metrics()
-            elif fp in ["atom-pair_fingerprint", "torsion_fingerprint"]:
-                # int vectors
-                out[fp] = SimilarityMeasure.get_supported_metrics()
-            else:  # mordred descriptors, custom descriptors
-                out[fp] = SimilarityMeasure.get_supported_general_metrics()
-        return out
-
-    @staticmethod
-    def get_supported_general_metrics():
-        """Return a list of strings for the currently implemented
-        similarity measures, aka metrics, which support vectors other
-        then binary vectors.
-
-        Returns:
-            List: List of strings.
-        """
-        return list(
-            set(SimilarityMeasure.get_supported_metrics())
-            - set(SimilarityMeasure.get_supported_binary_metrics())
-        )
-
-    @staticmethod
-    def get_supported_binary_metrics():
-        """Return a list of strings for the currently implemented
-        similarity measures, aka metrics, which only support binary
-        vectors.
-
-        Returns:
-            List: List of strings.
-        """
-        return [
-            "tanimoto",
-            "dice",
-            "austin-colwell",
-            "sorenson",
-            "gleason",
-            "dice_2",
-            "dice_3",
-            "jaccard",
-            "cosine",
-            "driver-kroeber",
-            "ochiai",
-            "simple_matching",
-            "sokal-michener",
-            "rand",
-            "rogers-tanimoto",
-            "russel-rao",
-            "forbes",
-            "simpson",
-            "braun-blanquet",
-            "baroni-urbani-buser",
-            "kulczynski",
-            "sokal-sneath",
-            "sokal-sneath-2",
-            "symmetric_sokal_sneath",
-            "symmetric-sokal-sneath",
-            "sokal-sneath-3",
-            "sokal-sneath_3",
-            "sokal-sneath-4",
-            "sokal-sneath_4",
-            "faith",
-            "mountford",
-            "michael",
-            "rogot-goldberg",
-            "hawkins-dotson",
-            "maxwell-pilliner",
-            "harris-lahey",
-            "consonni-todeschini-1",
-            "consonni-todeschini-2",
-            "consonni-todeschini-3",
-            "consonni-todeschini-4",
-            "consonni-todeschini-5",
-            "yule-1",
-            "yule_1",
-            "yule_2",
-            "yule_2",
-            "fossum",
-            "holiday-fossum",
-            "holiday_fossum",
-            "dennis",
-            "holiday-dennis",
-            "holiday_dennis",
-            "cole-1",
-            "cole_1",
-            "cole-2",
-            "cole_2",
-            "dispersion",
-            "choi",
-            "goodman-kruskal",
-            "pearson-heron",
-            "sorgenfrei",
-            "cohen",
-            "peirce_1",
-            "peirce_2",
-        ]
-
-    @staticmethod
-    def get_supported_metrics():
-        """Return a list of strings for the currently implemented
-        similarity measures, aka metrics.
-
-        Returns:
-            List: List of strings.
-        """
-        return [
-            "tanimoto",
-            "jaccard-tanimoto",
-            "l0_similarity",
-            "l1_similarity",
-            "manhattan_similarity",
-            "l2_similarity",
-            "euclidean_similarity",
-            "dice",
-            "sorenson",
-            "gleason",
-            "dice_2",
-            "dice_3",
-            "cosine",
-            "driver-kroeber",
-            "ochiai",
-            "simple_matching",
-            "sokal-michener",
-            "rand",
-            "rogers-tanimoto",
-            "russel-rao",
-            "forbes",
-            "simpson",
-            "braun-blanquet",
-            "baroni-urbani-buser",
-            "kulczynski",
-            "sokal-sneath",
-            "sokal-sneath_1",
-            "sokal-sneath-2",
-            "symmetric_sokal_sneath",
-            "symmetric-sokal-sneath",
-            "sokal-sneath-3",
-            "sokal-sneath_3",
-            "sokal-sneath-4",
-            "sokal-sneath_4",
-            "jaccard",
-            "faith",
-            "mountford",
-            "michael",
-            "rogot-goldberg",
-            "hawkins-dotson",
-            "maxwell-pilliner",
-            "harris-lahey",
-            "consonni-todeschini-1",
-            "consonni-todeschini-2",
-            "consonni-todeschini-3",
-            "consonni-todeschini-4",
-            "consonni-todeschini-5",
-            "consonni-todeschini_1",
-            "consonni-todeschini_2",
-            "consonni-todeschini_3",
-            "consonni-todeschini_4",
-            "consonni-todeschini_5",
-            "austin-colwell",
-            "yule-1",
-            "yule_1",
-            "yule_2",
-            "yule_2",
-            "fossum",
-            "holiday-fossum",
-            "holiday_fossum",
-            "dennis",
-            "holiday-dennis",
-            "holiday_dennis",
-            "cole-1",
-            "cole_1",
-            "cole-2",
-            "cole_2",
-            "dispersion",
-            "choi",
-            "goodman-kruskal",
-            "pearson-heron",
-            "sorgenfrei",
-            "cohen",
-            "peirce_1",
-            "peirce-1",
-            "peirce_2",
-            "peirce-2",
-        ]
-
-    @staticmethod
-    def get_uniq_metrics():
-        """Return a list of strings for the currently implemented
-        similarity measures, aka metrics. Each unique similarity metric is
-        uniquely represented with redundant tags removed.
-
-        Returns:
-            List: List of strings.
-        """
-        return [
-            "tanimoto",
-            "l0_similarity",
-            "l1_similarity",
-            "l2_similarity",
-            "dice",
-            "dice_2",
-            "dice_3",
-            "cosine",
-            "simple_matching",
-            "rogers-tanimoto",
-            "russel-rao",
-            "forbes",
-            "simpson",
-            "braun-blanquet",
-            "baroni-urbani-buser",
-            "kulczynski",
-            "sokal-sneath",
-            "sokal-sneath-2",
-            "sokal-sneath-3",
-            "sokal-sneath-4",
-            "jaccard",
-            "faith",
-            "mountford",
-            "michael",
-            "rogot-goldberg",
-            "hawkins-dotson",
-            "maxwell-pilliner",
-            "harris-lahey",
-            "consonni-todeschini-1",
-            "consonni-todeschini-2",
-            "consonni-todeschini-3",
-            "consonni-todeschini-4",
-            "consonni-todeschini-5",
-            "austin-colwell",
-            "yule-1",
-            "yule_2",
-            "fossum",
-            "dennis",
-            "cole-1",
-            "cole-2",
-            "dispersion",
-            "goodman-kruskal",
-            "pearson-heron",
-            "sorgenfrei",
-            "cohen",
-            "peirce-1",
-            "peirce-2",
-        ]
-
-    def __str__(self):
-        return self.label_
+"""This module contains methods to find similarities between molecules."""
+from functools import lru_cache
+import numpy as np
+from rdkit import DataStructs
+from scipy.spatial.distance import cosine as scipy_cosine
+
+from aimsim.ops import Descriptor
+from aimsim.exceptions import InvalidConfigurationError
+
+SMALL_NUMBER = 1e-10
+
+
+class SimilarityMeasure:
+    def __init__(self, metric):
+        if metric.lower() in ["l0_similarity"]:
+            self.metric = "l0_similarity"
+            self.type_ = "continuous"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in [
+            "l1_similarity",
+            "manhattan_similarity",
+            "taxicab_similarity",
+            "city_block_similarity",
+            "snake_similarity",
+        ]:
+            self.metric = "l1_similarity"
+            self.type_ = "continuous"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["l2_similarity", "euclidean_similarity"]:
+            self.metric = "l2_similarity"
+            self.type_ = "continuous"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["cosine", "driver-kroeber", "ochiai"]:
+            self.metric = "cosine"
+            self.type_ = "discrete"
+            # angular distance
+            self.to_distance = lambda x: np.arccos(x) / np.pi
+
+        elif metric.lower() in ["dice", "sorenson", "gleason"]:
+            self.metric = "dice"
+            self.type_ = "discrete"
+            # convert to jaccard for distance
+            self.to_distance = lambda x: 1 - x / (2 - x)
+
+        elif metric.lower() in ["dice_2"]:
+            self.metric = "dice_2"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["dice_3"]:
+            self.metric = "dice_3"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["tanimoto", "jaccard-tanimoto"]:
+            self.metric = "tanimoto"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["simple_matching", "sokal-michener", "rand"]:
+            self.metric = "simple_matching"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["rogers-tanimoto"]:
+            self.metric = "rogers_tanimoto"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["russel-rao"]:
+            self.metric = "russel_rao"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["forbes"]:
+            self.metric = "forbes"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["simpson"]:
+            self.metric = "simpson"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["braun-blanquet"]:
+            self.metric = "braun_blanquet"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["baroni-urbani-buser"]:
+            self.metric = "baroni_urbani_buser"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["kulczynski"]:
+            self.metric = "kulczynski"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["sokal-sneath", "sokal-sneath_1"]:
+            self.metric = "sokal_sneath"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in [
+            "sokal-sneath_2",
+            "sokal-sneath-2",
+            "symmetric_sokal_sneath",
+            "symmetric-sokal-sneath",
+        ]:
+            self.metric = "symmetric_sokal_sneath"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["sokal-sneath-3", "sokal-sneath_3"]:
+            self.metric = "sokal_sneath_3"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["sokal-sneath-4", "sokal-sneath_4"]:
+            self.metric = "sokal_sneath_4"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["jaccard"]:
+            self.metric = "jaccard"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["faith"]:
+            self.metric = "faith"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["michael"]:
+            self.metric = "michael"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["mountford"]:
+            self.metric = "mountford"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["rogot-goldberg"]:
+            self.metric = "rogot_goldberg"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["hawkins-dotson"]:
+            self.metric = "hawkins_dotson"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["maxwell-pilliner"]:
+            self.metric = "maxwell_pilliner"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["harris-lahey"]:
+            self.metric = "harris_lahey"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["consonni-todeschini-1", "consonni-todeschini_1"]:
+            self.metric = "consonni_todeschini_1"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["consonni-todeschini-2", "consonni-todeschini_2"]:
+            self.metric = "consonni_todeschini_2"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["consonni-todeschini-3", "consonni-todeschini_3"]:
+            self.metric = "consonni_todeschini_3"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["consonni-todeschini-4", "consonni-todeschini_4"]:
+            self.metric = "consonni_todeschini_4"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["consonni-todeschini-5", "consonni-todeschini_5"]:
+            self.metric = "consonni_todeschini_5"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["austin-colwell"]:
+            self.metric = "austin_colwell"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["yule-1", "yule_1"]:
+            self.metric = "yule_1"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["yule-2", "yule_2"]:
+            self.metric = "yule_2"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["fossum", "holiday-fossum", "holiday_fossum"]:
+            self.metric = "fossum"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["dennis", "holiday-dennis", "holiday_dennis"]:
+            self.metric = "dennis"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["cole-1", "cole_1"]:
+            self.metric = "cole_1"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["cole-2", "cole_2"]:
+            self.metric = "cole_2"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["dispersion", "choi"]:
+            self.metric = "dispersion"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["goodman-kruskal", "goodman_kruskal"]:
+            self.metric = "goodman_kruskal"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["pearson-heron", "pearson_heron"]:
+            self.metric = "pearson_heron"
+            self.type_ = "discrete"
+            self.to_distance = lambda x: 1 - x
+
+        elif metric.lower() in ["sorgenfrei"]:
+            self.metric = "sorgenfrei"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["cohen"]:
+            self.metric = "cohen"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["peirce_1", "peirce-1"]:
+            self.metric = "peirce_1"
+            self.type_ = "discrete"
+
+        elif metric.lower() in ["peirce_2", "peirce-2"]:
+            self.metric = "peirce_2"
+            self.type_ = "discrete"
+
+        else:
+            raise ValueError(f"Similarity metric: {metric} is not implemented")
+        self.normalize_fn = {"shift_": 0.0, "scale_": 1.0}
+        self.label_ = metric
+
+    def __call__(self, mol1_descriptor, mol2_descriptor):
+        """Compare two descriptors.
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            similarity_ (float): Similarity value
+        """
+        if not self._validate_fprint(mol1_descriptor) or not self._validate_fprint(
+            mol2_descriptor
+        ):
+            raise ValueError(
+                f"Molecule descriptor ({mol1_descriptor.label_}) has no active bits."
+            )
+        similarity_ = None
+        if self.metric == "l0_similarity":
+            try:
+                similarity_ = self._get_vector_norm_similarity(
+                    mol1_descriptor, mol2_descriptor, ord=0
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "l1_similarity":
+            try:
+                similarity_ = self._get_vector_norm_similarity(
+                    mol1_descriptor, mol2_descriptor, ord=1
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "l2_similarity":
+            try:
+                similarity_ = self._get_vector_norm_similarity(
+                    mol1_descriptor, mol2_descriptor, ord=2
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "austin_colwell":
+            try:
+                similarity_ = self._get_austin_colwell(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "baroni_urbani_buser":
+            try:
+                similarity_ = self._get_baroni_urbani_buser(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "braun_blanquet":
+            try:
+                similarity_ = self._get_braun_blanquet(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "cohen":
+            try:
+                similarity_ = self._get_cohen(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "cole_1":
+            try:
+                similarity_ = self._get_cole_1(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "cole_2":
+            try:
+                similarity_ = self._get_cole_2(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "consonni_todeschini_1":
+            try:
+                similarity_ = self._get_consonni_todeschini_1(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "consonni_todeschini_2":
+            try:
+                similarity_ = self._get_consonni_todeschini_2(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "consonni_todeschini_3":
+            try:
+                similarity_ = self._get_consonni_todeschini_3(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "consonni_todeschini_4":
+            try:
+                similarity_ = self._get_consonni_todeschini_4(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "consonni_todeschini_5":
+            try:
+                similarity_ = self._get_consonni_todeschini_5(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "cosine":
+            try:
+                similarity_ = self._get_cosine_similarity(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "dennis":
+            try:
+                similarity_ = self._get_dennis(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "dice":
+            try:
+                similarity_ = self._get_dice(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "dice_2":
+            try:
+                similarity_ = self._get_dice_2(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "dice_3":
+            try:
+                similarity_ = self._get_dice_3(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "dispersion":
+            try:
+                similarity_ = self._get_dispersion(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "faith":
+            try:
+                similarity_ = self._get_faith(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "forbes":
+            try:
+                similarity_ = self._get_forbes(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "fossum":
+            try:
+                similarity_ = self._get_fossum(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "goodman_kruskal":
+            try:
+                similarity_ = self._get_goodman_kruskal(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "harris_lahey":
+            try:
+                similarity_ = self._get_harris_lahey(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "hawkins_dotson":
+            try:
+                similarity_ = self._get_hawkins_dotson(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "jaccard":
+            try:
+                similarity_ = self._get_jaccard(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "kulczynski":
+            try:
+                similarity_ = self._get_kulczynski(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+        elif self.metric == "maxwell_pilliner":
+            try:
+                similarity_ = self._get_maxwell_pilliner(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "michael":
+            try:
+                similarity_ = self._get_michael(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "mountford":
+            try:
+                similarity_ = self._get_mountford(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "pearson_heron":
+            try:
+                similarity_ = self._get_pearson_heron(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "peirce_1":
+            try:
+                similarity_ = self._get_peirce_1(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "peirce_2":
+            try:
+                similarity_ = self._get_peirce_2(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "rogers_tanimoto":
+            try:
+                similarity_ = self._get_rogers_tanimoto(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "rogot_goldberg":
+            try:
+                similarity_ = self._get_rogot_goldberg(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "russel_rao":
+            try:
+                similarity_ = self._get_russel_rao(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "simple_matching":
+            try:
+                similarity_ = self._get_simple_matching(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "simpson":
+            try:
+                similarity_ = self._get_simpson(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "sokal_sneath":
+            try:
+                similarity_ = self._get_sokal_sneath(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "symmetric_sokal_sneath":
+            try:
+                similarity_ = self._get_symmetric_sokal_sneath(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "sokal_sneath_3":
+            try:
+                similarity_ = self._get_sokal_sneath_3(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "sokal_sneath_4":
+            try:
+                similarity_ = self._get_sokal_sneath_4(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "sorgenfrei":
+            try:
+                similarity_ = self._get_sorgenfrei(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "tanimoto":
+            try:
+                similarity_ = DataStructs.TanimotoSimilarity(
+                    mol1_descriptor.to_rdkit(), mol2_descriptor.to_rdkit()
+                )
+            except ValueError as e:
+                raise ValueError(
+                    "Tanimoto similarity is only useful for bit strings "
+                    "generated from fingerprints. Consider using "
+                    "other similarity measures for arbitrary vectors."
+                )
+        elif self.metric == "yule_1":
+            try:
+                similarity_ = self._get_yule_1(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        elif self.metric == "yule_2":
+            try:
+                similarity_ = self._get_yule_2(mol1_descriptor, mol2_descriptor)
+            except ValueError as e:
+                raise e
+
+        else:
+            raise ValueError(f"{self.metric} could not be implemented")
+
+        return similarity_
+
+    def _get_vector_norm_similarity(self, mol1_descriptor, mol2_descriptor, ord):
+        """Calculate the norm based similarity between two molecules.
+        This is defined as:
+        Norm similarity (order n) = 1 / (1 + n-norm(A - B)
+        where n-norm(A - B) represents the n-th order norm of the difference
+        of two vector A and B.
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+            ord (int): Order of the norm
+
+        Returns:
+            (float): Norm similarity value
+        """
+        arr1 = mol1_descriptor.to_numpy()
+        arr2 = mol2_descriptor.to_numpy()
+        if len(arr1) != len(arr2):
+            try:
+                arr1, arr2 = Descriptor.fold_to_equal_length(
+                    mol1_descriptor, mol2_descriptor
+                )
+            except ValueError as e:
+                raise ValueError(
+                    "Fingerprints are of unequal length and cannot be folded."
+                ) from e
+
+        norm_ = np.linalg.norm(arr1 - arr2, ord=ord)
+        similarity_ = 1 / (1 + norm_)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_austin_colwell(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Austin-Colwell similarity between two molecules.
+        This is defined for two binary arrays as:
+        Austin-Colwell similarity = (2 / pi) * arcsin(sqrt( (a + d) / p ))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Austin-Colwell similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Austin-Colwell similarity is only useful for "
+                "bit strings generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        similarity_ = (2 / np.pi) * np.arcsin(np.sqrt((a + d) / p))
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_baroni_urbani_buser(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Baroni-Urbani-Buser similarity between two molecules.
+        This is defined for two binary arrays as:
+        Baroni-Urbani-Buser similarity = (sqrt(a * d) + a)
+                                         / (sqrt(a * d) + a + b + c)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Baroni-Urbani-Buser similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Baroni-Urbani-Buser similarity is only useful for "
+                "bit strings generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if d == p:
+            return 1.0
+        similarity_ = (np.sqrt(a * d) + a) / (np.sqrt(a * d) + a + b + c)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_braun_blanquet(self, mol1_descriptor, mol2_descriptor):
+        """Calculate braun-blanquet similarity between two molecules.
+        This is defined for two binary arrays as:
+        Braun-Blanquet Similarity = a / max{(a + b), (a + c)}
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Braun-Blanquet similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Braun-Blanquet similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        if a < SMALL_NUMBER:
+            return 0.0
+        similarity_ = a / max((a + b), (a + c))
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_cohen(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Cohen similarity between two molecules.
+        This is defined for two binary arrays as:
+        Cohen Similarity = 2*(a*d - b*c) / ((a + b)*(b + d) + (a + c)*(c + d))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Cohen similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Cohen similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        denominator_ = (a + b) * (b + d) + (a + c) * (c + d)
+        if a == p or d == p:
+            return 1.0
+        if denominator_ < SMALL_NUMBER:
+            return 0.0
+
+        similarity_ = 2 * (a * d - b * c) / denominator_
+        self.normalize_fn["shift_"] = 1.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_cole_1(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Cole(1) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Cole(1) Similarity = (a*d - b*c) / ((a + c)*(c + d))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Cole(1)  similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Cole(1) similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        denominator = (a + c) * (c + d)
+        if denominator < SMALL_NUMBER:
+            return 0.0
+        similarity_ = (a * d - b * c) / denominator
+        self.normalize_fn["shift_"] = p - 1
+        self.normalize_fn["scale_"] = p
+        return self._normalize(similarity_)
+
+    def _get_cole_2(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Cole(2) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Cole(2) Similarity = (a*d - b*c) / ((a + b)*(b + d))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Cole(2)  similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Cole(2) similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        denominator = (a + b) * (b + d)
+        if denominator < SMALL_NUMBER:
+            return 0.0
+        similarity_ = (a * d - b * c) / denominator
+        self.normalize_fn["shift_"] = p - 1
+        self.normalize_fn["scale_"] = p
+        return self._normalize(similarity_)
+
+    def _get_consonni_todeschini_1(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Consonni-Todeschini(1) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Consonni-Todeschini(1) similarity = ln(1 + a + d) / ln(1 + p)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Consonni-Todeschini(1)  similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Consonni-Todeschini(1)  similarity is only useful for "
+                "bit strings generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        similarity_ = np.log(1 + a + d) / np.log(1 + p)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_consonni_todeschini_2(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Consonni-Todeschini(2) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Consonni-Todeschini(2) similarity =
+            (ln(1 + p) - ln(1 + b + c)) / ln(1 + p)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Consonni-Todeschini(2)  similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Consonni-Todeschini(2) similarity is only useful for "
+                "bit strings generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        similarity_ = (np.log(1 + p) - np.log(1 + b + c)) / np.log(1 + p)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_consonni_todeschini_3(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Consonni-Todeschini(3) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Consonni-Todeschini(3) similarity = ln(1 + a) / ln(1 + p)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Consonni-Todeschini(3)  similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Consonni-Todeschini(3) similarity is only useful for "
+                "bit strings generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        similarity_ = np.log(1 + a) / np.log(1 + p)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_consonni_todeschini_4(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Consonni-Todeschini(4) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Consonni-Todeschini(4) similarity = ln(1 + a) / ln(1 + a + b + c)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Consonni-Todeschini(4)  similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Consonni-Todeschini(4) similarity is only useful for "
+                "bit strings generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        if np.log(1 + a + b + c) == 0:
+            raise InvalidConfigurationError("Empty string supplied")
+        similarity_ = np.log(1 + a) / np.log(1 + a + b + c)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_consonni_todeschini_5(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Consonni-Todeschini(5) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Consonni-Todeschini(5) similarity = (ln(1 + a*d) - ln(1 + b*c))
+                                            / ln(1 + p**2 / 4)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Consonni-Todeschini(5)  similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Consonni-Todeschini(5) similarity is only useful for "
+                "bit strings generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        similarity_ = (np.log(1 + a * d) - np.log(1 + b * c)) / np.log(1 + (p**2) / 4)
+        self.normalize_fn["shift_"] = 1.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_cosine_similarity(self, mol1_descriptor, mol2_descriptor):
+        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        denominator = np.sqrt((a + b) * (a + c))
+        if denominator < SMALL_NUMBER:
+            return 0.0
+        similarity_ = a / denominator
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_dennis(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Dennis similarity between two molecules.
+        This is defined for two binary arrays as:
+        Dennis similarity = (a*d - b*c) / sqrt(p*(a + b)*(a + c))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Dennis similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Dennis similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        denominator = np.sqrt(p * (a + b) * (a + c))
+        if denominator < SMALL_NUMBER:
+            return 0.0
+        similarity_ = (a * d - b * c) / denominator
+        self.normalize_fn["shift_"] = np.sqrt(p) / 2
+        self.normalize_fn["scale_"] = 3 * np.sqrt(p) / 2
+        return self._normalize(similarity_)
+
+    def _get_dice(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Dice similarity between two molecules.
+        This is defined for two binary arrays as:
+        Dice similarity = 2a / (2a + b + c)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Dice similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Dice similarity is only useful for bit strings "
+                "generated from fingerprints, not {} and {}. Consider using "
+                "other similarity measures for arbitrary vectors.".format(
+                    mol1_descriptor.get_label(), mol2_descriptor.get_label()
+                )
+            )
+        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        if a < SMALL_NUMBER:
+            return 0.0
+        similarity_ = 2 * a / (2 * a + b + c)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_dice_2(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Dice(2) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Dice(2) similarity = a / (a + b)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Dice(2) similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Dice(2) similarity is only useful for bit strings "
+                "generated from fingerprints, not {} and {}. Consider using "
+                "other similarity measures for arbitrary vectors.".format(
+                    mol1_descriptor.get_label(), mol2_descriptor.get_label()
+                )
+            )
+        a, b, _, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        if a < SMALL_NUMBER:
+            return 0.0
+        similarity_ = a / (a + b)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_dice_3(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Dice(3) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Dice(3) similarity = a / (a + c)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Dice(3) similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Dice(3) similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, _, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
+
+        if a < SMALL_NUMBER:
+            return 0.0
+        similarity_ = a / (a + c)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_dispersion(self, mol1_descriptor, mol2_descriptor):
+        """Calculate dispersion similarity in Choi et al (2012)
+         between two molecules. This is defined for two binary arrays as:
+        dispersion similarity = (a*d - b*c) / p**2
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): dispersion similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Dispersion similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        similarity_ = (a * d - b * c) / p**2
+        self.normalize_fn["shift_"] = 1 / 4
+        self.normalize_fn["scale_"] = 1 / 2
+        return self._normalize(similarity_)
+
+    def _get_faith(self, mol1_descriptor, mol2_descriptor):
+        """Calculate faith similarity between two molecules.
+        This is defined for two binary arrays as:
+        Faith similarity = (a + 0.5*d) / p
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Faith similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Faith similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        similarity_ = (a + 0.5 * d) / p
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_forbes(self, mol1_descriptor, mol2_descriptor):
+        """Calculate forbes similarity between two molecules.
+        This is defined for two binary arrays as:
+        Forbes similarity = (p * a) / ((a + b) * (a + c))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Forbes similarity value
+
+        Note:
+            The Forbes similarity is normalized to [0, 1]
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Forbes similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        if (a + b) * (a + c) < SMALL_NUMBER or a < SMALL_NUMBER:
+            return 0.0
+        p = a + b + c + d
+        similarity_ = (p * a) / ((a + b) * (a + c) + SMALL_NUMBER)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = p / a
+        return self._normalize(similarity_)
+
+    def _get_fossum(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Fossum similarity between two molecules.
+        This is defined for two binary arrays as:
+        Fossum similarity = p * (a - 0.5)**2 / ((a + b) * (a + c))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Fossum similarity value
+
+        Note:
+            The similarity is normalized to [0, 1].
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Fossum similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        denominator = (a + b) * (a + c)
+        if denominator < SMALL_NUMBER:
+            return 0.0
+        p = a + b + c + d
+        similarity_ = p * (a - 0.5) ** 2 / denominator
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = (p - 0.5) ** 2 / p
+        return self._normalize(similarity_)
+
+    def _get_goodman_kruskal(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Goodman-Kruskal similarity between two molecules.
+        This is defined for two binary arrays as:
+        Goodman-Kruskal similarity =
+            (2 * min(a, d) - b - c) / (2 * min(a, d) + b + c)
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Goodman-Kruskal similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Goodman-Kruskal similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        min_a_d = np.min([a, d])
+        similarity_ = (2 * min_a_d - b - c) / (2 * min_a_d + b + c)
+        self.normalize_fn["shift_"] = 1.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_harris_lahey(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Harris-Lahey similarity between two molecules.
+        This is defined for two binary arrays as:
+        Harris-Lahey similarity =
+            (a/2) * (2*d + b + c)/(a + b + c)
+             + (d/2) * (2*a + b + c)/( b + c + d)
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Harris-Lahey similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Harris-Lahey similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        if (a + b + c) < SMALL_NUMBER or (b + c + d) < SMALL_NUMBER:
+            return 0.0
+
+        similarity_ = (a / 2) * (2 * d + b + c) / (a + b + c) + (d / 2) * (
+            2 * a + b + c
+        ) / (b + c + d)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = p
+        return self._normalize(similarity_)
+
+    def _get_hawkins_dotson(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Hawkins-Dotson similarity between two molecules.
+        This is defined for two binary arrays as:
+        Hawkins-Dotson similarity = 0.5 * (a / (a + b + c)
+                                           + d / (d + b + c))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Hawkins-Dotson similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Hawkins-Dotson similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        similarity_ = 0.5 * (
+            a / (a + b + c + SMALL_NUMBER) + d / (d + b + c + SMALL_NUMBER)
+        )
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_jaccard(self, mol1_descriptor, mol2_descriptor):
+        """Calculate jaccard similarity between two molecules.
+        This is defined for two binary arrays as:
+        jaccard similarity = 3*a / (3*a + b + c)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Jaccard similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Jaccard similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        if a < SMALL_NUMBER:
+            return 0.0
+        similarity_ = 3 * a / (3 * a + b + c)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_kulczynski(self, mol1_descriptor, mol2_descriptor):
+        """Calculate kulczynski similarity between two molecules.
+        This is defined for two binary arrays as:
+        kulczynski similarity = 0.5 * a / ((a + b) + (a + c))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Kulczynski similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Kulczynski similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        if a < SMALL_NUMBER:
+            return 0.0
+        similarity_ = 0.5 * a / ((a + b) + (a + c))
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_michael(self, mol1_descriptor, mol2_descriptor):
+        """Calculate michael similarity between two molecules.
+        This is defined for two binary arrays as:
+        michael similarity = 4*(a*d - b*c) / ((a + d)**2 + (b + c)**2)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Michael similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Michael similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p or (b + c) < SMALL_NUMBER:
+            return 1.0
+        similarity_ = 4 * (a * d - b * c) / ((a + d) ** 2 + (b + c) ** 2)
+        self.normalize_fn["shift_"] = 1.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_maxwell_pilliner(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Maxwell-Pilliner similarity between two molecules.
+        This is defined for two binary arrays as:
+        Maxwell-Pilliner similarity =
+            2*(a*d - b*c) / ((a + b)*(c + d) + (a + c)*(b + d))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Maxwell-Pilliner similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Maxwell-Pilliner similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        denominator = (a + b) * (c + d) + (a + c) * (b + d)
+        if a == p or d == p:
+            return 1.0
+        if denominator < SMALL_NUMBER:
+            return 0.0
+
+        similarity_ = 2 * (a * d - b * c) / denominator
+        self.normalize_fn["shift_"] = 1.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_mountford(self, mol1_descriptor, mol2_descriptor):
+        """Calculate mountford similarity between two molecules.
+        This is defined for two binary arrays as:
+        mountford similarity = 2*a / (a*b + a*c + 2*b*c)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Mountford similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Mountford similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        denominator = a * b + a * c + 2 * b * c
+        if denominator < SMALL_NUMBER:
+            return a / p
+        similarity_ = 2 * a / denominator
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_pearson_heron(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Pearson-Heron similarity between two molecules.
+        This is defined for two binary arrays as:
+        Pearson-Heron similarity =
+         (a*d - b*c)/sqrt((a + b)*(a + c)*(b + d)*(c + d))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Pearson-Heron similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Pearson-Heron similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        if b == p or c == p:
+            return 0.0
+        denominator_ = np.sqrt(
+            np.int64(a + b) * np.int64(a + c) * np.int64(b + d) * np.int64(c + d)
+        )
+        if denominator_ < SMALL_NUMBER:
+            return 0.0
+        similarity_ = (a * d - b * c) / denominator_
+        self.normalize_fn["shift_"] = 1.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_peirce_1(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Peirce(1) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Peirce(1) similarity = (a*d - b*c) / ((a + b)*(c + d))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Peirce(1) similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Peirce(1) similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        if b == p or c == p:
+            return 0.0
+        similarity_ = (a * d - b * c) / ((a + b) * (c + d) + SMALL_NUMBER)
+        self.normalize_fn["shift_"] = 1.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_peirce_2(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Peirce(2) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Peirce(2) similarity = (a*d - b*c) / ((a + c)*(b + d))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Peirce(2) similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Peirce(2) similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        if b == p or c == p:
+            return 0.0
+        similarity_ = (a * d - b * c) / ((a + c) * (b + d) + SMALL_NUMBER)
+        self.normalize_fn["shift_"] = 1.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_rogers_tanimoto(self, mol1_descriptor, mol2_descriptor):
+        """Calculate rogers-tanimoto similarity between two molecules.
+        This is defined for two binary arrays as:
+        Rogers-Tanimoto similarity = (a + d) / (p + b + c)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Rogers-Tanimoto similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Rogers-Tanimoto similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        similarity_ = (a + d) / (p + b + c)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_rogot_goldberg(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Rogot-Goldberg similarity between two molecules.
+        This is defined for two binary arrays as:
+        Rogot-Goldberg similarity = (a / (2*a + b + c)) + (d / (2*d + b + c))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Rogot-Goldberg  similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Rogot-Goldberg  similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        similarity_ = (a / (2 * a + b + c)) + (d / (2 * d + b + c))
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_russel_rao(self, mol1_descriptor, mol2_descriptor):
+        """Calculate russel-rao similarity between two molecules.
+        This is defined for two binary arrays as:
+        Russel-Rao = a / p
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Russel-Rao similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Russel-Rao similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        similarity_ = a / p
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_simple_matching(self, mol1_descriptor, mol2_descriptor):
+        """Calculate simple matching similarity between two molecules.
+        This is defined for two binary arrays as:
+        Simple Matching = (a + d) / p
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Simple Matching similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Simple Matching similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        similarity_ = (a + d) / p
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_simpson(self, mol1_descriptor, mol2_descriptor):
+        """Calculate simpson similarity between two molecules.
+        This is defined for two binary arrays as:
+        Simpson Similarity = a / min{(a + b), (a + c)}
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Simpson similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Simpson similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        if min((a + b), (a + c)) < SMALL_NUMBER or a < SMALL_NUMBER:
+            return 0.0
+        similarity_ = a / min((a + b), (a + c))
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_sokal_sneath(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Sokal-Sneath similarity between two molecules.
+        This is defined for two binary arrays as:
+        Sokal-Sneath similarity = a / (a + 2*b + 2*c)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Sokal-Sneath similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Sokal-Sneath similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, _ = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        if a < SMALL_NUMBER:
+            return 0.0
+        similarity_ = a / (a + 2 * b + 2 * c)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_symmetric_sokal_sneath(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Symmetric Sokal-Sneath similarity between two molecules.
+        This is defined for two binary arrays as:
+        Symmetric Sokal-Sneath similarity = (2*a + 2*d) / (p + a + d)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Symmetric Sokal-Sneath similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Symmetric Sokal-Sneath similarity is only useful "
+                "for bit strings generated from fingerprints. Consider "
+                "using other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        similarity_ = (2 * a + 2 * d) / (p + a + d)
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_sokal_sneath_3(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Sokal-Sneath(3) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Sokal-Sneath(3) similarity =
+        (1/4) * (a/(a + b) + a/(a + c) + d/(b + d) + d/(c + d))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Sokal-Sneath(3) similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Sokal-Sneath(3) similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        if a < SMALL_NUMBER and d < SMALL_NUMBER:
+            return 0.0
+        similarity_ = (1 / 4) * (
+            a / (a + b + SMALL_NUMBER)
+            + a / (a + c + SMALL_NUMBER)
+            + d / (b + d + SMALL_NUMBER)
+            + d / (c + d + SMALL_NUMBER)
+        )
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_sokal_sneath_4(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Sokal-Sneath(4) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Sokal-Sneath(4) similarity =
+         a/sqrt((a + b) * (a + c)) * d/sqrt((b + d) *(c + d))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Sokal-Sneath(4) similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Sokal-Sneath(4) similarity is only useful for bit strings "
+                "generated from fingerprints. Consider using "
+                "other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        if a == p or d == p:
+            return 1.0
+        if a < SMALL_NUMBER or d < SMALL_NUMBER:
+            return 0.0
+        similarity_ = (
+            a
+            / (np.sqrt((a + b) * (a + c)) + SMALL_NUMBER)
+            * d
+            / (np.sqrt((b + d) * (c + d) + SMALL_NUMBER))
+        )
+
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_sorgenfrei(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Sorgenfrei similarity between two molecules.
+        This is defined for two binary arrays as:
+        Sorgenfrei similarity = a**2 / ((a + b)*(a + c))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Sorgenfrei similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Sorgenfrei similarity is only useful "
+                "for bit strings generated from fingerprints. Consider "
+                "using other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        if a < SMALL_NUMBER:
+            return 0.0
+        similarity_ = a**2 / ((a + b) * (a + c))
+        self.normalize_fn["shift_"] = 0.0
+        self.normalize_fn["scale_"] = 1.0
+        return self._normalize(similarity_)
+
+    def _get_yule_1(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Yule(1) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Symmetric Yule(1) similarity = (a*d - b*c) / (a*d + b*c)
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Yule(1) similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Yule(1) similarity is only useful "
+                "for bit strings generated from fingerprints. Consider "
+                "using other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        denominator = a * d + b * c + SMALL_NUMBER
+        if a == p or d == p or b * c < SMALL_NUMBER:
+            return 1.0
+        similarity_ = (a * d - b * c) / denominator
+        self.normalize_fn["shift_"] = 1.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_yule_2(self, mol1_descriptor, mol2_descriptor):
+        """Calculate Yule(2) similarity between two molecules.
+        This is defined for two binary arrays as:
+        Symmetric Yule(2) similarity = (sqrt(a*d) - sqrt(b*c))
+                                       / (sqrt(a*d) + sqrt(b*c))
+
+        Args:
+            mol1_descriptor (AIMSim.ops Descriptor)
+            mol2_descriptor (AIMSim.ops Descriptor)
+
+        Returns:
+            (float): Yule(2) similarity value
+        """
+        if not (mol1_descriptor.is_fingerprint() and mol2_descriptor.is_fingerprint()):
+            raise ValueError(
+                "Yule(2) similarity is only useful "
+                "for bit strings generated from fingerprints. Consider "
+                "using other similarity measures for arbitrary vectors."
+            )
+        a, b, c, d = self._get_abcd(mol1_descriptor, mol2_descriptor)
+        p = a + b + c + d
+        denominator = np.sqrt(a * d) + np.sqrt(b * c) + SMALL_NUMBER
+        if a == p or d == p or b * c < SMALL_NUMBER:
+            return 1.0
+        similarity_ = (np.sqrt(a * d) - np.sqrt(b * c)) / denominator
+        self.normalize_fn["shift_"] = 1.0
+        self.normalize_fn["scale_"] = 2.0
+        return self._normalize(similarity_)
+
+    def _get_abcd(self, fingerprint1, fingerprint2):
+        """Get a, b, c, d, where:
+        a = #bits(bits(array 1) and bits(array 2))
+        b = #bits(bits(array 1) and bits(~array 2))
+        c = #bits(bits(~array 1) and bits(array 2))
+        d = #bits(bits(~array 1) and bits(~array 2)) // "~": complement operator
+        p = a + b + c + d = bits(array 1 or array 2)
+
+        Args:
+            fingerprint1 (Descriptor)
+            fingerprint2 (Descriptor)
+
+        Returns:
+            (tuple): (a, b, c, d)
+
+        Note:
+            If arrays of unequal lengths are passed, the larger array is folded
+            to the length of the smaller array.
+
+        """
+        arr1, arr2 = Descriptor.fold_to_equal_length(fingerprint1, fingerprint2)
+        not_arr1 = np.logical_not(arr1)
+        not_arr2 = np.logical_not(arr2)
+        a = np.sum(arr1 & arr2)
+        b = np.sum(arr1 & not_arr2)
+        c = np.sum(not_arr1 & arr2)
+        d = np.sum(not_arr1 & not_arr2)
+        assert (a + b + c + d) == arr1.size == arr2.size
+        return a, b, c, d
+
+    def _normalize(self, similarity_):
+        return (similarity_ + self.normalize_fn["shift_"]) / self.normalize_fn["scale_"]
+
+    def is_distance_metric(self):
+        """Check if the similarity measure is a distance metric.
+
+        Returns:
+            bool: True if it is a distance metric.
+        """
+        return hasattr(self, "to_distance")
+
+    @staticmethod
+    @lru_cache(maxsize=None)
+    def _validate_fprint(descriptor: Descriptor) -> bool:
+        """Are there any non-zero bits in this descriptor?
+
+        Args:
+            descriptor (Descriptor): AIMSim.ops.Descriptor object
+
+        Returns:
+            boolean: False if descriptor is all zero, True otherwise
+        """
+        return np.any(descriptor.to_numpy())
+
+    @staticmethod
+    def get_compatible_metrics():
+        """Return a dictionary with which types of metrics each fingerprint supports.
+
+        Returns:
+            dict: comptabile FP's: metrics
+        """
+        out = {}
+        fprints = Descriptor.get_all_supported_descriptors()
+        for fp in fprints:
+            if fp in [
+                "morgan_fingerprint",
+                "topological_fingerprint",
+                "daylight_fingerprint",
+                "maccs_keys",
+            ]:  # explicit bit vectors
+                out[fp] = SimilarityMeasure.get_supported_binary_metrics()
+            elif fp in ["atom-pair_fingerprint", "torsion_fingerprint"]:
+                # int vectors
+                out[fp] = SimilarityMeasure.get_supported_metrics()
+            else:  # mordred descriptors, custom descriptors
+                out[fp] = SimilarityMeasure.get_supported_general_metrics()
+        return out
+
+    @staticmethod
+    def get_supported_general_metrics():
+        """Return a list of strings for the currently implemented
+        similarity measures, aka metrics, which support vectors other
+        then binary vectors.
+
+        Returns:
+            List: List of strings.
+        """
+        return list(
+            set(SimilarityMeasure.get_supported_metrics())
+            - set(SimilarityMeasure.get_supported_binary_metrics())
+        )
+
+    @staticmethod
+    def get_supported_binary_metrics():
+        """Return a list of strings for the currently implemented
+        similarity measures, aka metrics, which only support binary
+        vectors.
+
+        Returns:
+            List: List of strings.
+        """
+        return [
+            "tanimoto",
+            "dice",
+            "austin-colwell",
+            "sorenson",
+            "gleason",
+            "dice_2",
+            "dice_3",
+            "jaccard",
+            "cosine",
+            "driver-kroeber",
+            "ochiai",
+            "simple_matching",
+            "sokal-michener",
+            "rand",
+            "rogers-tanimoto",
+            "russel-rao",
+            "forbes",
+            "simpson",
+            "braun-blanquet",
+            "baroni-urbani-buser",
+            "kulczynski",
+            "sokal-sneath",
+            "sokal-sneath-2",
+            "symmetric_sokal_sneath",
+            "symmetric-sokal-sneath",
+            "sokal-sneath-3",
+            "sokal-sneath_3",
+            "sokal-sneath-4",
+            "sokal-sneath_4",
+            "faith",
+            "mountford",
+            "michael",
+            "rogot-goldberg",
+            "hawkins-dotson",
+            "maxwell-pilliner",
+            "harris-lahey",
+            "consonni-todeschini-1",
+            "consonni-todeschini-2",
+            "consonni-todeschini-3",
+            "consonni-todeschini-4",
+            "consonni-todeschini-5",
+            "yule-1",
+            "yule_1",
+            "yule_2",
+            "yule_2",
+            "fossum",
+            "holiday-fossum",
+            "holiday_fossum",
+            "dennis",
+            "holiday-dennis",
+            "holiday_dennis",
+            "cole-1",
+            "cole_1",
+            "cole-2",
+            "cole_2",
+            "dispersion",
+            "choi",
+            "goodman-kruskal",
+            "pearson-heron",
+            "sorgenfrei",
+            "cohen",
+            "peirce_1",
+            "peirce_2",
+        ]
+
+    @staticmethod
+    def get_supported_metrics():
+        """Return a list of strings for the currently implemented
+        similarity measures, aka metrics.
+
+        Returns:
+            List: List of strings.
+        """
+        return [
+            "tanimoto",
+            "jaccard-tanimoto",
+            "l0_similarity",
+            "l1_similarity",
+            "manhattan_similarity",
+            "l2_similarity",
+            "euclidean_similarity",
+            "dice",
+            "sorenson",
+            "gleason",
+            "dice_2",
+            "dice_3",
+            "cosine",
+            "driver-kroeber",
+            "ochiai",
+            "simple_matching",
+            "sokal-michener",
+            "rand",
+            "rogers-tanimoto",
+            "russel-rao",
+            "forbes",
+            "simpson",
+            "braun-blanquet",
+            "baroni-urbani-buser",
+            "kulczynski",
+            "sokal-sneath",
+            "sokal-sneath_1",
+            "sokal-sneath-2",
+            "symmetric_sokal_sneath",
+            "symmetric-sokal-sneath",
+            "sokal-sneath-3",
+            "sokal-sneath_3",
+            "sokal-sneath-4",
+            "sokal-sneath_4",
+            "jaccard",
+            "faith",
+            "mountford",
+            "michael",
+            "rogot-goldberg",
+            "hawkins-dotson",
+            "maxwell-pilliner",
+            "harris-lahey",
+            "consonni-todeschini-1",
+            "consonni-todeschini-2",
+            "consonni-todeschini-3",
+            "consonni-todeschini-4",
+            "consonni-todeschini-5",
+            "consonni-todeschini_1",
+            "consonni-todeschini_2",
+            "consonni-todeschini_3",
+            "consonni-todeschini_4",
+            "consonni-todeschini_5",
+            "austin-colwell",
+            "yule-1",
+            "yule_1",
+            "yule_2",
+            "yule_2",
+            "fossum",
+            "holiday-fossum",
+            "holiday_fossum",
+            "dennis",
+            "holiday-dennis",
+            "holiday_dennis",
+            "cole-1",
+            "cole_1",
+            "cole-2",
+            "cole_2",
+            "dispersion",
+            "choi",
+            "goodman-kruskal",
+            "pearson-heron",
+            "sorgenfrei",
+            "cohen",
+            "peirce_1",
+            "peirce-1",
+            "peirce_2",
+            "peirce-2",
+        ]
+
+    @staticmethod
+    def get_uniq_metrics():
+        """Return a list of strings for the currently implemented
+        similarity measures, aka metrics. Each unique similarity metric is
+        uniquely represented with redundant tags removed.
+
+        Returns:
+            List: List of strings.
+        """
+        return [
+            "tanimoto",
+            "l0_similarity",
+            "l1_similarity",
+            "l2_similarity",
+            "dice",
+            "dice_2",
+            "dice_3",
+            "cosine",
+            "simple_matching",
+            "rogers-tanimoto",
+            "russel-rao",
+            "forbes",
+            "simpson",
+            "braun-blanquet",
+            "baroni-urbani-buser",
+            "kulczynski",
+            "sokal-sneath",
+            "sokal-sneath-2",
+            "sokal-sneath-3",
+            "sokal-sneath-4",
+            "jaccard",
+            "faith",
+            "mountford",
+            "michael",
+            "rogot-goldberg",
+            "hawkins-dotson",
+            "maxwell-pilliner",
+            "harris-lahey",
+            "consonni-todeschini-1",
+            "consonni-todeschini-2",
+            "consonni-todeschini-3",
+            "consonni-todeschini-4",
+            "consonni-todeschini-5",
+            "austin-colwell",
+            "yule-1",
+            "yule_2",
+            "fossum",
+            "dennis",
+            "cole-1",
+            "cole-2",
+            "dispersion",
+            "goodman-kruskal",
+            "pearson-heron",
+            "sorgenfrei",
+            "cohen",
+            "peirce-1",
+            "peirce-2",
+        ]
+
+    def __str__(self):
+        return self.label_
```

### Comparing `aimsim-2.0.2/aimsim/tasks/cluster_data.py` & `aimsim-2.0.3/aimsim/tasks/cluster_data.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-"""Data clustering task."""
-from os import makedirs
-from os.path import dirname
-
-import matplotlib.pyplot as plt
-from matplotlib.colors import rgb2hex
-import yaml
-
-from .task import Task
-from aimsim.exceptions import InvalidConfigurationError
-from aimsim.utils.plotting_scripts import plot_barchart, plot_density
-from aimsim.utils.plotting_scripts import plot_scatter_interactive
-
-
-class ClusterData(Task):
-    def __init__(self, configs=None, **kwargs):
-        """Constructor for the ClusterData class.
-
-        Args:
-            configs(dict): Dictionary of configurations. Default is None.
-            **kwargs: Keyword arguments to modify configs fields.
-        Notes:
-            The configuration structure with default values are:
-            'n_clusters' (int):
-            'clustering_method' (str): None
-            cluster_plot_settings: {'cluster_colors' (list):
-                                                         colors from tab20 cmap,
-                                    'response' (str): 'Response'}
-
-            embedding_plot_settings:
-                    {'plot_color': 'red'
-                     'plot_title': '2-D projected space',
-                     'xlabel': 'Dimension 1',
-                     'ylabel': 'Dimension 2',
-                     'embedding': {'method': "mds",
-                                    'params': {'random_state': 42}}}
-
-        """
-        if configs is None:
-            if kwargs == {}:
-                raise IOError(f"No config supplied for {str(self)}")
-            else:
-                configs = {}
-                configs.update(kwargs)
-        super().__init__(configs)
-        self.n_clusters = None
-        self.plot_settings = None
-        self.log_fpath = None
-        self._extract_configs()
-
-    def _extract_configs(self):
-        self.n_clusters = self.configs["n_clusters"]
-        self.clustering_method = self.configs.get("clustering_method", None)
-        self.plot_settings = dict()
-        self.plot_settings["cluster_plot"] = {
-            "cluster_colors": [
-                rgb2hex(plt.cm.get_cmap("tab20", self.n_clusters)(cluster_id))
-                for cluster_id in range(self.n_clusters)],
-            "response": "Response",
-        }
-
-        self.plot_settings["cluster_plot"].update(
-            self.configs.get("cluster_plot_settings", {}))
-        self.plot_settings["embedding_plot"] = {
-            "plot_title": f"2-D projected space",
-            "xlabel": "Dimension 1",
-            "ylabel": "Dimension 2",
-            "embedding": {"method": "mds",
-                          "params": {"random_state": 42, }
-                          },
-        }
-        self.plot_settings["embedding_plot"].update(self.configs.get(
-            "embedding_plot_settings",
-            {}))
-
-        self.log_fpath = self.configs.get("log_file_path", None)
-        if self.log_fpath is not None:
-            log_dir = dirname(self.log_fpath)
-            makedirs(log_dir, exist_ok=True)
-
-        self.cluster_fpath = self.configs.get("cluster_file_path", None)
-        if self.cluster_fpath is not None:
-            cluster_dir = dirname(self.cluster_fpath)
-            makedirs(cluster_dir, exist_ok=True)
-
-    def __call__(self, molecule_set):
-        try:
-            molecule_set.cluster(
-                n_clusters=self.n_clusters,
-                clustering_method=self.clustering_method
-            )
-        except InvalidConfigurationError as e:
-            raise e
-        mol_names = molecule_set.get_mol_names()
-        mol_properties = molecule_set.get_mol_properties()
-        cluster_labels = molecule_set.get_cluster_labels()
-        cluster_grouped_mol_names = {}
-        cluster_grouped_mol_properties = {}
-        for cluster_id in range(self.n_clusters):
-            cluster_grouped_mol_names[cluster_id] = mol_names[
-                cluster_labels == cluster_id
-            ].tolist()
-            if mol_properties is not None:
-                cluster_grouped_mol_properties[cluster_id] = mol_properties[
-                    cluster_labels == cluster_id
-                ].tolist()
-
-        if self.cluster_fpath is not None:
-            print("Writing to file ", self.cluster_fpath)
-            with open(self.cluster_fpath, "w") as fp:
-                yaml.dump(cluster_grouped_mol_names, fp)
-                if cluster_grouped_mol_properties != {}:
-                    yaml.dump('Properties By Cluster', fp)
-                    yaml.dump(cluster_grouped_mol_properties, fp)
-
-        if self.log_fpath is not None:
-            print("Writing to file ", self.log_fpath)
-            with open(self.log_fpath, "w") as fp:
-                fp.write(
-                    f'Embedding method '
-                    f'{self.plot_settings["embedding_plot"]["embedding"]["method"]}. '
-                    f'random seed '
-                    f'{self.plot_settings["embedding_plot"]["embedding"]["params"]["random_state"]}')
-
-        plot_barchart(
-            [_ for _ in range(self.n_clusters)],
-            heights=[
-                len(cluster_grouped_mol_names[cluster_id])
-                for cluster_id in range(self.n_clusters)
-            ],
-            colors=self.plot_settings["cluster_plot"]["cluster_colors"],
-            xtick_labels=[_ for _ in range(self.n_clusters)],
-            xlabel="Cluster Index",
-            ylabel="Cluster Population",
-        )
-        if mol_properties is not None:
-            densities = []
-            for cluster_id in range(self.n_clusters):
-                densities.append(cluster_grouped_mol_properties[cluster_id])
-            plot_density(
-                densities=densities,
-                n_densities=self.n_clusters,
-                legends=['Cluster'+str(_)
-                         for _ in range(self.n_clusters)],
-                plot_color=self.plot_settings[
-                    "cluster_plot"]["cluster_colors"],
-                legend_fontsize=20,
-                xlabel=self.plot_settings["cluster_plot"]["response"],
-                ylabel='Density',
-                shade=True,
-            )
-        method_ = self.plot_settings["embedding_plot"]["embedding"]["method"]
-        reduced_features = molecule_set.get_transformed_descriptors(
-            method_=method_,
-            n_components=2,
-            **self.plot_settings["embedding_plot"]["embedding"].get("params", {}))
-        dimension_1 = reduced_features[:, 0]
-        dimension_2 = reduced_features[:, 1]
-
-        plot_scatter_interactive(
-            dimension_1,
-            dimension_2,
-            cluster_memberships=cluster_labels,
-            xlabel=self.plot_settings["embedding_plot"]["xlabel"],
-            ylabel=self.plot_settings["embedding_plot"]["ylabel"],
-            title=self.plot_settings["embedding_plot"]['plot_title'],
-            hover_names=mol_names,
-            cluster_colors=self.plot_settings["cluster_plot"]["cluster_colors"],
-        )
-
-    def __str__(self):
-        return "Task: Cluster data"
+"""Data clustering task."""
+from os import makedirs
+from os.path import dirname
+
+import matplotlib.pyplot as plt
+from matplotlib.colors import rgb2hex
+import yaml
+
+from .task import Task
+from aimsim.exceptions import InvalidConfigurationError
+from aimsim.utils.plotting_scripts import plot_barchart, plot_density
+from aimsim.utils.plotting_scripts import plot_scatter_interactive
+
+
+class ClusterData(Task):
+    def __init__(self, configs=None, **kwargs):
+        """Constructor for the ClusterData class.
+
+        Args:
+            configs(dict): Dictionary of configurations. Default is None.
+            **kwargs: Keyword arguments to modify configs fields.
+        Notes:
+            The configuration structure with default values are:
+            'n_clusters' (int):
+            'clustering_method' (str): None
+            cluster_plot_settings: {'cluster_colors' (list):
+                                                         colors from tab20 cmap,
+                                    'response' (str): 'Response'}
+
+            embedding_plot_settings:
+                    {'plot_color': 'red'
+                     'plot_title': '2-D projected space',
+                     'xlabel': 'Dimension 1',
+                     'ylabel': 'Dimension 2',
+                     'embedding': {'method': "mds",
+                                    'params': {'random_state': 42}}}
+
+        """
+        if configs is None:
+            if kwargs == {}:
+                raise IOError(f"No config supplied for {str(self)}")
+            else:
+                configs = {}
+                configs.update(kwargs)
+        super().__init__(configs)
+        self.n_clusters = None
+        self.plot_settings = None
+        self.log_fpath = None
+        self._extract_configs()
+
+    def _extract_configs(self):
+        self.n_clusters = self.configs["n_clusters"]
+        self.clustering_method = self.configs.get("clustering_method", None)
+        self.plot_settings = dict()
+        self.plot_settings["cluster_plot"] = {
+            "cluster_colors": [
+                rgb2hex(plt.cm.get_cmap("tab20", self.n_clusters)(cluster_id))
+                for cluster_id in range(self.n_clusters)],
+            "response": "Response",
+        }
+
+        self.plot_settings["cluster_plot"].update(
+            self.configs.get("cluster_plot_settings", {}))
+        self.plot_settings["embedding_plot"] = {
+            "plot_title": f"2-D projected space",
+            "xlabel": "Dimension 1",
+            "ylabel": "Dimension 2",
+            "embedding": {"method": "mds",
+                          "params": {"random_state": 42, }
+                          },
+        }
+        self.plot_settings["embedding_plot"].update(self.configs.get(
+            "embedding_plot_settings",
+            {}))
+
+        self.log_fpath = self.configs.get("log_file_path", None)
+        if self.log_fpath is not None:
+            log_dir = dirname(self.log_fpath)
+            makedirs(log_dir, exist_ok=True)
+
+        self.cluster_fpath = self.configs.get("cluster_file_path", None)
+        if self.cluster_fpath is not None:
+            cluster_dir = dirname(self.cluster_fpath)
+            makedirs(cluster_dir, exist_ok=True)
+
+    def __call__(self, molecule_set):
+        try:
+            molecule_set.cluster(
+                n_clusters=self.n_clusters,
+                clustering_method=self.clustering_method
+            )
+        except InvalidConfigurationError as e:
+            raise e
+        mol_names = molecule_set.get_mol_names()
+        mol_properties = molecule_set.get_mol_properties()
+        cluster_labels = molecule_set.get_cluster_labels()
+        cluster_grouped_mol_names = {}
+        cluster_grouped_mol_properties = {}
+        for cluster_id in range(self.n_clusters):
+            cluster_grouped_mol_names[cluster_id] = mol_names[
+                cluster_labels == cluster_id
+            ].tolist()
+            if mol_properties is not None:
+                cluster_grouped_mol_properties[cluster_id] = mol_properties[
+                    cluster_labels == cluster_id
+                ].tolist()
+
+        if self.cluster_fpath is not None:
+            print("Writing to file ", self.cluster_fpath)
+            with open(self.cluster_fpath, "w") as fp:
+                yaml.dump(cluster_grouped_mol_names, fp)
+                if cluster_grouped_mol_properties != {}:
+                    yaml.dump('Properties By Cluster', fp)
+                    yaml.dump(cluster_grouped_mol_properties, fp)
+
+        if self.log_fpath is not None:
+            print("Writing to file ", self.log_fpath)
+            with open(self.log_fpath, "w") as fp:
+                fp.write(
+                    f'Embedding method '
+                    f'{self.plot_settings["embedding_plot"]["embedding"]["method"]}. '
+                    f'random seed '
+                    f'{self.plot_settings["embedding_plot"]["embedding"]["params"]["random_state"]}')
+
+        plot_barchart(
+            [_ for _ in range(self.n_clusters)],
+            heights=[
+                len(cluster_grouped_mol_names[cluster_id])
+                for cluster_id in range(self.n_clusters)
+            ],
+            colors=self.plot_settings["cluster_plot"]["cluster_colors"],
+            xtick_labels=[_ for _ in range(self.n_clusters)],
+            xlabel="Cluster Index",
+            ylabel="Cluster Population",
+        )
+        if mol_properties is not None:
+            densities = []
+            for cluster_id in range(self.n_clusters):
+                densities.append(cluster_grouped_mol_properties[cluster_id])
+            plot_density(
+                densities=densities,
+                n_densities=self.n_clusters,
+                legends=['Cluster'+str(_)
+                         for _ in range(self.n_clusters)],
+                plot_color=self.plot_settings[
+                    "cluster_plot"]["cluster_colors"],
+                legend_fontsize=20,
+                xlabel=self.plot_settings["cluster_plot"]["response"],
+                ylabel='Density',
+                shade=True,
+            )
+        method_ = self.plot_settings["embedding_plot"]["embedding"]["method"]
+        reduced_features = molecule_set.get_transformed_descriptors(
+            method_=method_,
+            n_components=2,
+            **self.plot_settings["embedding_plot"]["embedding"].get("params", {}))
+        dimension_1 = reduced_features[:, 0]
+        dimension_2 = reduced_features[:, 1]
+
+        plot_scatter_interactive(
+            dimension_1,
+            dimension_2,
+            cluster_memberships=cluster_labels,
+            xlabel=self.plot_settings["embedding_plot"]["xlabel"],
+            ylabel=self.plot_settings["embedding_plot"]["ylabel"],
+            title=self.plot_settings["embedding_plot"]['plot_title'],
+            hover_names=mol_names,
+            cluster_colors=self.plot_settings["cluster_plot"]["cluster_colors"],
+        )
+
+    def __str__(self):
+        return "Task: Cluster data"
```

### Comparing `aimsim-2.0.2/aimsim/tasks/compare_target_molecule.py` & `aimsim-2.0.3/aimsim/tasks/compare_target_molecule.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-from os import makedirs
-from os.path import dirname
-import matplotlib.pyplot as plt
-from aimsim.chemical_datastructures import Molecule
-import numpy as np
-
-from aimsim.utils.plotting_scripts import plot_density
-from aimsim.exceptions import InvalidConfigurationError
-from .task import Task
-
-
-class CompareTargetMolecule(Task):
-    def __init__(self, configs=None, **kwargs):
-        if configs is None:
-            if kwargs == {}:
-                raise IOError(f"No config supplied for {str(self)}")
-            else:
-                configs = {}
-                configs.update(kwargs)
-        super().__init__(configs)
-        self.target_molecule = None
-        self.log_fpath = None
-        self.plot_settings = None
-        self._extract_configs()
-
-    def _extract_configs(self):
-        target_molecule_smiles = self.configs.get("target_molecule_smiles")
-        target_molecule_src = self.configs.get("target_molecule_src")
-        if target_molecule_smiles:
-            self.target_molecule = Molecule(mol_smiles=target_molecule_smiles)
-        elif target_molecule_src:
-            self.target_molecule = Molecule(mol_src=target_molecule_src)
-        else:
-            raise IOError("Target molecule source is not specified")
-
-        self.log_fpath = self.configs.get("log_file_path", None)
-        if self.log_fpath is not None:
-            log_dir = dirname(self.log_fpath)
-            makedirs(log_dir, exist_ok=True)
-
-        self.plot_settings = self.configs.get("similarity_plot_settings", {})
-        self.n_hits = self.configs.get("n_hits", 1)
-        self.draw_molecules = self.configs.get("draw_molecules", False)
-
-    def __call__(self, molecule_set):
-        """
-        Compare a target molecule with molecular database in terms
-        of similarity.
-        Args:
-            molecule_set (AIMSim.chemical_datastructures Molecule): Target
-                molecule.
-
-        """
-        most_similar_mols, sims = self.get_hits_similar_to(
-            molecule_set=molecule_set)
-        most_dissimilar_mols, dissims = self.get_hits_dissimilar_to(
-            molecule_set=molecule_set)
-        most_similar_mols = [molecule_set.molecule_database[mol_id]
-                             for mol_id in most_similar_mols]
-        most_dissimilar_mols = [molecule_set.molecule_database[mol_id]
-                                for mol_id in most_dissimilar_mols]
-        text_prompt = "***** "
-        text_prompt += f"FOR MOLECULE {self.target_molecule.mol_text} *****"
-        text_prompt += "\n\n"
-        text_prompt += "****Maximum Similarity Molecules ****\n"
-        for molecule, similarity in zip(most_similar_mols, sims):
-            text_prompt += f"Molecule: {molecule.mol_text}\n"
-            text_prompt += "Similarity: "
-            text_prompt += str(similarity)
-            if self.draw_molecules:
-                molecule.draw(title=molecule.mol_text)
-
-        text_prompt += "\n\n"
-        text_prompt += "****Minimum Similarity Molecules ****\n"
-        for molecule, similarity in zip(most_dissimilar_mols, dissims):
-            text_prompt += f"Molecule: {molecule.mol_text}\n"
-            text_prompt += "Similarity: "
-            text_prompt += str(similarity)
-            if self.draw_molecules:
-                molecule.draw(title=molecule.mol_text)
-        text_prompt += "\n\n\n"
-        if self.log_fpath is None:
-            print(text_prompt)
-        else:
-            if molecule_set.is_verbose:
-                print(text_prompt)
-            print("Writing to file ", self.log_fpath)
-            with open(self.log_fpath, "w") as fp:
-                fp.write(text_prompt)
-        plot_density(self.similarities_, **self.plot_settings)
-
-    def __str__(self):
-        return "Task: Compare to a target molecule"
-
-    def get_hits_similar_to(self, molecule_set=None):
-        """Get sorted list of num_hits Molecule in the Set most
-        similar to a query Molecule.This is defined as the sorted set
-        (decreasing similarity)  of molecules with the highest
-        (query_molecule, set_molecule) similarity.
-
-        Args:
-            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
-                MoleculeSet object used to calculate sorted similarities.
-                Only used if self.similarities or
-                self.sorted_similarities not set.
-
-        Returns:
-            np.ndarray(int): Ids of most similar
-                molecules in decreasing order of similarity.
-            np.ndarray(float): Corresponding similarity values.
-
-        """
-        if not hasattr(self, 'sorted_similarities_'):
-            if not hasattr(self, 'similarities_'):
-                if molecule_set is None:
-                    raise InvalidConfigurationError('MoleculeSet object not '
-                                                    'passed for task')
-                else:
-                    self.similarities_ = molecule_set.compare_against_molecule(
-                        self.target_molecule)
-            self.sorted_similarities_ = np.argsort(self.similarities_)
-        ids = np.array([self.sorted_similarities_[-1 - hit_id]
-                        for hit_id in range(self.n_hits)])
-
-        return ids, self.similarities_[ids]
-
-    def get_hits_dissimilar_to(self, molecule_set=None):
-        """Get sorted list of num_hits Molecule in the Set most
-        dissimilar to a query Molecule.This is defined as the sorted set
-        (decreasing dissimilarity)  of molecules with the highest
-        (query_molecule, set_molecule) dissimilarity.
-
-        Args:
-            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
-                MoleculeSet object used to calculate sorted similarities.
-                Only used if self.similarities or
-                self.sorted_similarities not set.
-
-        Returns:
-            np.ndarray(int): Ids of most similar molecules in decreasing
-                order of dissimilarity.
-            np.ndarray(float): Corresponding similarity values.
-
-        """
-        if not hasattr(self, 'sorted_similarities_'):
-            if not hasattr(self, 'similarities_'):
-                if molecule_set is None:
-                    raise InvalidConfigurationError('MoleculeSet object not '
-                                                    'passed for task')
-                else:
-                    self.similarities_ = molecule_set.compare_against_molecule(
-                        self.target_molecule)
-            self.sorted_similarities_ = np.argsort(self.similarities_)
-        ids = np.array([self.sorted_similarities_[hit_id]
-                        for hit_id in range(self.n_hits)])
-        return ids, self.similarities_[ids]
+from os import makedirs
+from os.path import dirname
+import matplotlib.pyplot as plt
+from aimsim.chemical_datastructures import Molecule
+import numpy as np
+
+from aimsim.utils.plotting_scripts import plot_density
+from aimsim.exceptions import InvalidConfigurationError
+from .task import Task
+
+
+class CompareTargetMolecule(Task):
+    def __init__(self, configs=None, **kwargs):
+        if configs is None:
+            if kwargs == {}:
+                raise IOError(f"No config supplied for {str(self)}")
+            else:
+                configs = {}
+                configs.update(kwargs)
+        super().__init__(configs)
+        self.target_molecule = None
+        self.log_fpath = None
+        self.plot_settings = None
+        self._extract_configs()
+
+    def _extract_configs(self):
+        target_molecule_smiles = self.configs.get("target_molecule_smiles")
+        target_molecule_src = self.configs.get("target_molecule_src")
+        if target_molecule_smiles:
+            self.target_molecule = Molecule(mol_smiles=target_molecule_smiles)
+        elif target_molecule_src:
+            self.target_molecule = Molecule(mol_src=target_molecule_src)
+        else:
+            raise IOError("Target molecule source is not specified")
+
+        self.log_fpath = self.configs.get("log_file_path", None)
+        if self.log_fpath is not None:
+            log_dir = dirname(self.log_fpath)
+            makedirs(log_dir, exist_ok=True)
+
+        self.plot_settings = self.configs.get("similarity_plot_settings", {})
+        self.n_hits = self.configs.get("n_hits", 1)
+        self.draw_molecules = self.configs.get("draw_molecules", False)
+
+    def __call__(self, molecule_set):
+        """
+        Compare a target molecule with molecular database in terms
+        of similarity.
+        Args:
+            molecule_set (AIMSim.chemical_datastructures Molecule): Target
+                molecule.
+
+        """
+        most_similar_mols, sims = self.get_hits_similar_to(
+            molecule_set=molecule_set)
+        most_dissimilar_mols, dissims = self.get_hits_dissimilar_to(
+            molecule_set=molecule_set)
+        most_similar_mols = [molecule_set.molecule_database[mol_id]
+                             for mol_id in most_similar_mols]
+        most_dissimilar_mols = [molecule_set.molecule_database[mol_id]
+                                for mol_id in most_dissimilar_mols]
+        text_prompt = "***** "
+        text_prompt += f"FOR MOLECULE {self.target_molecule.mol_text} *****"
+        text_prompt += "\n\n"
+        text_prompt += "****Maximum Similarity Molecules ****\n"
+        for molecule, similarity in zip(most_similar_mols, sims):
+            text_prompt += f"Molecule: {molecule.mol_text}\n"
+            text_prompt += "Similarity: "
+            text_prompt += str(similarity)
+            if self.draw_molecules:
+                molecule.draw(title=molecule.mol_text)
+
+        text_prompt += "\n\n"
+        text_prompt += "****Minimum Similarity Molecules ****\n"
+        for molecule, similarity in zip(most_dissimilar_mols, dissims):
+            text_prompt += f"Molecule: {molecule.mol_text}\n"
+            text_prompt += "Similarity: "
+            text_prompt += str(similarity)
+            if self.draw_molecules:
+                molecule.draw(title=molecule.mol_text)
+        text_prompt += "\n\n\n"
+        if self.log_fpath is None:
+            print(text_prompt)
+        else:
+            if molecule_set.is_verbose:
+                print(text_prompt)
+            print("Writing to file ", self.log_fpath)
+            with open(self.log_fpath, "w") as fp:
+                fp.write(text_prompt)
+        plot_density(self.similarities_, **self.plot_settings)
+
+    def __str__(self):
+        return "Task: Compare to a target molecule"
+
+    def get_hits_similar_to(self, molecule_set=None):
+        """Get sorted list of num_hits Molecule in the Set most
+        similar to a query Molecule.This is defined as the sorted set
+        (decreasing similarity)  of molecules with the highest
+        (query_molecule, set_molecule) similarity.
+
+        Args:
+            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
+                MoleculeSet object used to calculate sorted similarities.
+                Only used if self.similarities or
+                self.sorted_similarities not set.
+
+        Returns:
+            np.ndarray(int): Ids of most similar
+                molecules in decreasing order of similarity.
+            np.ndarray(float): Corresponding similarity values.
+
+        """
+        if not hasattr(self, 'sorted_similarities_'):
+            if not hasattr(self, 'similarities_'):
+                if molecule_set is None:
+                    raise InvalidConfigurationError('MoleculeSet object not '
+                                                    'passed for task')
+                else:
+                    self.similarities_ = molecule_set.compare_against_molecule(
+                        self.target_molecule)
+            self.sorted_similarities_ = np.argsort(self.similarities_)
+        ids = np.array([self.sorted_similarities_[-1 - hit_id]
+                        for hit_id in range(self.n_hits)])
+
+        return ids, self.similarities_[ids]
+
+    def get_hits_dissimilar_to(self, molecule_set=None):
+        """Get sorted list of num_hits Molecule in the Set most
+        dissimilar to a query Molecule.This is defined as the sorted set
+        (decreasing dissimilarity)  of molecules with the highest
+        (query_molecule, set_molecule) dissimilarity.
+
+        Args:
+            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
+                MoleculeSet object used to calculate sorted similarities.
+                Only used if self.similarities or
+                self.sorted_similarities not set.
+
+        Returns:
+            np.ndarray(int): Ids of most similar molecules in decreasing
+                order of dissimilarity.
+            np.ndarray(float): Corresponding similarity values.
+
+        """
+        if not hasattr(self, 'sorted_similarities_'):
+            if not hasattr(self, 'similarities_'):
+                if molecule_set is None:
+                    raise InvalidConfigurationError('MoleculeSet object not '
+                                                    'passed for task')
+                else:
+                    self.similarities_ = molecule_set.compare_against_molecule(
+                        self.target_molecule)
+            self.sorted_similarities_ = np.argsort(self.similarities_)
+        ids = np.array([self.sorted_similarities_[hit_id]
+                        for hit_id in range(self.n_hits)])
+        return ids, self.similarities_[ids]
```

### Comparing `aimsim-2.0.2/aimsim/tasks/identify_outliers.py` & `aimsim-2.0.3/aimsim/tasks/identify_outliers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-"""Subclass of Task that implements an IsolationForest to identify outliers."""
-from .task import Task
-from sklearn.ensemble import IsolationForest
-import warnings
-from aimsim.utils.plotting_scripts import plot_scatter_interactive
-import matplotlib.pyplot as plt
-
-
-class IdentifyOutliers(Task):
-    """Subclass of Task to identify outliers via an IsolationForest.
-
-    Args:
-        Task (abstract class): Parent abstract class.
-    """
-
-    def __init__(self, configs=None, **kwargs):
-        if configs is None:
-            configs = dict()  # all configs are optional
-        configs.update(kwargs)
-        super().__init__(configs)
-        self.plot_settings = {}
-        self._extract_configs()
-
-    def _extract_configs(self):
-        self.plot_settings["pairwise_plot"] = self.configs.get(
-            "pairwise_similarity_plot_settings", {}
-        )
-        self.output = self.configs.get("output", "terminal")
-        self.plot_outlier = self.configs.get("plot_ouliers", True)
-        self.random_state = self.configs.get("random_state", 42)
-
-    def __call__(self, molecule_set):
-        """Iterates through all molecules in molecule_set,
-        trains an IsolationForest, and identifies outliers.
-
-        Args:
-            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
-                Molecules object of the molecule database.
-
-        """
-        descs = []
-        for molecule in molecule_set.molecule_database:
-            descs.append(molecule.descriptor.to_numpy())
-        iof = IsolationForest(random_state=self.random_state)
-        iof.fit(descs)
-        print("~" * 58)
-        print(" ~" * 10 + " Outlier Detection " + "~ " * 10)
-        print("~" * 58)
-        outlier_idxs = []
-        for nmol, anomaly in zip(
-            range(len(molecule_set.molecule_database)), iof.predict(descs)
-        ):
-            if anomaly == -1:
-                outlier_idxs.append(nmol)
-                msg = (
-                    "Molecule {} (name: {}) is a potential outlier "
-                    "({:.2f} outlier score)".format(
-                        nmol + 1,
-                        molecule_set.molecule_database[nmol],
-                        iof.decision_function(descs[nmol].reshape(1, -1))[0],
-                    )
-                )
-                if self.output == "terminal":
-                    warnings.warn(msg)
-                else:
-                    with open(self.output + ".log", "a") as file:
-                        file.write(msg + "\n")
-        if self.plot_outlier:
-            reduced_features = molecule_set.get_transformed_descriptors(
-                method_="pca")
-            plot_scatter_interactive(
-                reduced_features[:, 0],
-                reduced_features[:, 1],
-                outlier_idxs=outlier_idxs,
-                title=f"2-D projected space",
-                **self.plot_settings["pairwise_plot"],
-            )
-
-        print("~" * 58)
-        print("Outlier detection complete.")
-        print("~" * 58)
-
-    def __str__(self):
-        return "Task: Identify outliers"
+"""Subclass of Task that implements an IsolationForest to identify outliers."""
+from .task import Task
+from sklearn.ensemble import IsolationForest
+import warnings
+from aimsim.utils.plotting_scripts import plot_scatter_interactive
+import matplotlib.pyplot as plt
+
+
+class IdentifyOutliers(Task):
+    """Subclass of Task to identify outliers via an IsolationForest.
+
+    Args:
+        Task (abstract class): Parent abstract class.
+    """
+
+    def __init__(self, configs=None, **kwargs):
+        if configs is None:
+            configs = dict()  # all configs are optional
+        configs.update(kwargs)
+        super().__init__(configs)
+        self.plot_settings = {}
+        self._extract_configs()
+
+    def _extract_configs(self):
+        self.plot_settings["pairwise_plot"] = self.configs.get(
+            "pairwise_similarity_plot_settings", {}
+        )
+        self.output = self.configs.get("output", "terminal")
+        self.plot_outlier = self.configs.get("plot_ouliers", True)
+        self.random_state = self.configs.get("random_state", 42)
+
+    def __call__(self, molecule_set):
+        """Iterates through all molecules in molecule_set,
+        trains an IsolationForest, and identifies outliers.
+
+        Args:
+            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
+                Molecules object of the molecule database.
+
+        """
+        descs = []
+        for molecule in molecule_set.molecule_database:
+            descs.append(molecule.descriptor.to_numpy())
+        iof = IsolationForest(random_state=self.random_state)
+        iof.fit(descs)
+        print("~" * 58)
+        print(" ~" * 10 + " Outlier Detection " + "~ " * 10)
+        print("~" * 58)
+        outlier_idxs = []
+        for nmol, anomaly in zip(
+            range(len(molecule_set.molecule_database)), iof.predict(descs)
+        ):
+            if anomaly == -1:
+                outlier_idxs.append(nmol)
+                msg = (
+                    "Molecule {} (name: {}) is a potential outlier "
+                    "({:.2f} outlier score)".format(
+                        nmol + 1,
+                        molecule_set.molecule_database[nmol],
+                        iof.decision_function(descs[nmol].reshape(1, -1))[0],
+                    )
+                )
+                if self.output == "terminal":
+                    warnings.warn(msg)
+                else:
+                    with open(self.output + ".log", "a") as file:
+                        file.write(msg + "\n")
+        if self.plot_outlier:
+            reduced_features = molecule_set.get_transformed_descriptors(
+                method_="pca")
+            plot_scatter_interactive(
+                reduced_features[:, 0],
+                reduced_features[:, 1],
+                outlier_idxs=outlier_idxs,
+                title=f"2-D projected space",
+                **self.plot_settings["pairwise_plot"],
+            )
+
+        print("~" * 58)
+        print("Outlier detection complete.")
+        print("~" * 58)
+
+    def __str__(self):
+        return "Task: Identify outliers"
```

### Comparing `aimsim-2.0.2/aimsim/tasks/measure_search.py` & `aimsim-2.0.3/aimsim/tasks/measure_search.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,312 +1,312 @@
-"""Identify most appropriate choice of fingerprint and similarity measure by
-evaluating the response of the nearest and furthest neighbors. This is called
-measure choice for brevity (although both measure and features are chosen)"""
-from collections import namedtuple
-import json
-from os import makedirs
-from os.path import dirname
-
-import numpy as np
-
-from aimsim.chemical_datastructures import MoleculeSet
-from aimsim.exceptions import InvalidConfigurationError
-from aimsim.ops import Descriptor, SimilarityMeasure
-from aimsim.utils.plotting_scripts import plot_multiple_barchart
-from .task import Task
-from .see_property_variation_with_similarity \
-    import SeePropertyVariationWithSimilarity
-
-
-class MeasureSearch(Task):
-    def __init__(self, configs=None, **kwargs):
-        if configs is None:
-            configs = dict()
-        configs.update(kwargs)
-        super().__init__(configs)
-        self.plot_settings = None
-        self.log_fpath = None
-        self._extract_configs()
-
-    def _extract_configs(self):
-        """
-        Raises:
-        InvalidConfigurationError: If correlation_type does not match
-                                   implemented types.
-        """
-        self.plot_settings = {'colors': ['#78DEC7', '#FB7AFC', '#FBC7F7'],
-                              'xticksize': 10,
-                              'yticksize': 20,
-                              'title': "",
-                              'title_fontsize': 24,
-                              'xlabel_fontsize': 20,
-                              'ylabel_fontsize': 20,
-                              }
-        self.plot_settings.update(self.configs.get("plot_settings",
-                                                   {}))
-        try:
-            self.prop_var_w_similarity = SeePropertyVariationWithSimilarity(
-                correlation_type=self.configs.get('correlation_type'))
-        except InvalidConfigurationError as e:
-            raise e
-        self.log_fpath = self.configs.get("log_file_path", None)
-        if self.log_fpath is not None:
-            log_dir = dirname(self.log_fpath)
-            makedirs(log_dir, exist_ok=True)
-
-    def __call__(self,
-                 molecule_set_configs,
-                 fingerprint_type=None,
-                 fingerprint_params=None,
-                 similarity_measure=None,
-                 subsample_subset_size=0.01,
-                 optim_algo='max_min',
-                 show_top=0,
-                 only_metric=True,
-                 ):
-        """
-        Calculate the correlation in the properties of molecules in set
-        and their nearest and furthest neighbors using different
-        fingerprints / similarity measure choices. Choose the best fingerprint
-        and similarity measure pair (called measure choice for brevity)
-        based on an optimization strategy.
-
-        Args:
-            molecule_set_configs (dict): All configurations (except
-                fingerprint_type, fingerprint_params and similarity_measure)
-                needed to form the moleculeSet.
-            fingerprint_type (str): Label to indicate which fingerprint to
-                use. If supplied, fingerprint is fixed and optimization
-                carried out over similarity measures. Use None to indicate
-                that optimization needs to be carried out over fingerprints.
-                Default is None.
-            fingerprint_params (dict): Hyper-parameters for fingerprints.
-                Passed to the MoleculeSet constructor. If None is passed,
-                set to empty dictionary before passing to MoleculeSet.
-            similarity_measure (str): Label to indicate which similarity
-                measure to use. If supplied, similarity measure is fixed
-                and optimization carried out over similarity measures.
-                Use None to indicate that optimization needs to be carried
-                out over fingerprints. Default is None.
-            subsample_subset_size (float): Fraction of molecule_set to
-                subsample. This is separate from the sample_ratio parameter
-                used when creating a moleculeSet since it is recommended
-                to have an more aggressive subsampling strategy for this task
-                due to the combinatorial explosion of looking at multiple
-                fingerprints and similarity measures. Default is 0.01.
-            optim_algo (str): Label to indicate the optimization algorithm
-                chosen. Options are:
-                'max': The measure choice which maximizes correlation
-                    of properties between nearest neighbors (most similar).
-                    This is the default.
-                'min': The measure choice which minimizes the absolute value
-                    of property correlation
-                    between furthest neighbors (most dissimilar).
-                'max_min': The measure choice which maximizes correlation
-                    of properties between nearest neighbors (most similar)
-                    and minimizes he absolute value of property correlation
-                    between furthest neighbors (most dissimilar).
-                    This is the default.
-            show_top (int): Number of top performing measures to show in plot.
-                If 0, no plots are generated and the top performer is returned.
-            only_metric (bool): If True only similarity measures satisfying
-                the metricity property
-                (i.e. can be converted to distance metrics) are selected.
-
-        Returns:
-            (NamedTuple): Top performer with fields:
-                fingerprint_type (str): Label for fingerprint type
-               similarity_measure (str): Label for similarity measure
-               nearest_neighbor_correlation (float): Correlation of property
-                   of molecule and its nearest neighbor.
-               furthest_neighbor_correlation (float): Correlation of property
-                   of molecule and its furthest neighbor.
-               score_ (float): Overall score based on optimization strategy.
-                   More is better.
-
-        """
-        print(f'Using subsample size {subsample_subset_size} for '
-              f'measure search')
-        trial_ = namedtuple('trial_', ['fingerprint_type',
-                                       'similarity_measure',
-                                       'nearest_neighbor_correlation',
-                                       'furthest_neighbor_correlation',
-                                       'score_'])
-        if fingerprint_type is None:
-            all_fingerprint_types = Descriptor.get_supported_fprints()
-            fingerprint_params = None
-        else:
-            all_fingerprint_types = [fingerprint_type]
-        if similarity_measure is None:
-            if only_metric:
-                print('Only trying measures with valid distance metrics')
-            all_similarity_measures = SimilarityMeasure.get_uniq_metrics()
-        else:
-            all_similarity_measures = [similarity_measure]
-        is_verbose = molecule_set_configs.get("is_verbose", False)
-        all_scores = []
-        if fingerprint_params is None:
-            fingerprint_params = {}
-        for similarity_measure in all_similarity_measures:
-            if only_metric and not SimilarityMeasure(
-                    metric=similarity_measure).is_distance_metric():
-                continue
-            if is_verbose:
-                print(f'Trying {similarity_measure} similarity')
-            for fingerprint_type in all_fingerprint_types:
-                if is_verbose:
-                    print(f'Trying {fingerprint_type} fingerprint')
-                try:
-                    molecule_set = MoleculeSet(
-                        molecule_database_src=molecule_set_configs[
-                            'molecule_database_src'],
-                        molecule_database_src_type=molecule_set_configs[
-                            'molecule_database_src_type'],
-                        similarity_measure=similarity_measure,
-                        fingerprint_type=fingerprint_type,
-                        fingerprint_params=fingerprint_params,
-                        is_verbose=is_verbose,
-                        n_threads=molecule_set_configs.get(
-                            'n_threads', 1),
-                        sampling_ratio=subsample_subset_size)
-                except (InvalidConfigurationError, ValueError, RuntimeError) as e:
-                    if is_verbose:
-                        print(f'Could not try {fingerprint_type} with '
-                              f'similarity measure {similarity_measure} due to '
-                              f'{e}')
-                    continue
-                nearest_corr, nearest_p_val = self.prop_var_w_similarity. \
-                    get_property_correlations_in_most_similar(
-                        molecule_set)
-                furthest_corr, furthest_p_val = self.prop_var_w_similarity. \
-                    get_property_correlations_in_most_dissimilar(
-                        molecule_set)
-                if optim_algo == 'max_min':
-                    score_ = nearest_corr - abs(furthest_corr)
-                elif optim_algo == 'max':
-                    score_ = nearest_corr
-                elif optim_algo == 'min':
-                    score_ = -abs(furthest_corr)
-                else:
-                    raise InvalidConfigurationError(f'{optim_algo} '
-                                                    f'not implemented')
-                all_scores.append(trial_(
-                    fingerprint_type=fingerprint_type,
-                    similarity_measure=similarity_measure,
-                    nearest_neighbor_correlation=nearest_corr,
-                    furthest_neighbor_correlation=furthest_corr,
-                    score_=score_))
-        all_scores.sort(key=lambda x: x[-1], reverse=True)
-        if self.log_fpath is not None:
-            print('Writing to ', self.log_fpath)
-            log_data = [trial._asdict() for trial in all_scores]
-            with open(self.log_fpath, "w") as fp:
-                json.dump(log_data, fp)
-
-        if show_top > 0:
-            top_performers = all_scores[:show_top]
-            all_nearest_neighbor_correlations = []
-            all_furthest_neighbor_correlations = []
-            top_scores = []
-            all_measures = []
-            for trial in top_performers:
-                all_nearest_neighbor_correlations.append(
-                    trial.nearest_neighbor_correlation)
-                all_furthest_neighbor_correlations.append(
-                    trial.furthest_neighbor_correlation)
-                top_scores.append(trial.score_)
-                all_measures.append(Descriptor.shorten_label(
-                    trial.fingerprint_type)
-                    + '\n'
-                    + trial.similarity_measure)
-            bar_heights = np.array([top_scores,
-                                    all_nearest_neighbor_correlations,
-                                    all_furthest_neighbor_correlations])
-            colors = self.plot_settings.pop('colors')
-            plot_multiple_barchart(x=[_ for _ in range(len(top_performers))],
-                                   heights=bar_heights,
-                                   legend_labels=['Overall scores',
-                                                  'Nearest neighbor property '
-                                                  'correlation',
-                                                  'Furthest neighbor property '
-                                                  'correlations'],
-                                   colors=colors,
-                                   xtick_labels=all_measures,
-                                   ylabel='Value',
-                                   xlabel='Measure',
-                                   **self.plot_settings)
-
-        return all_scores[0]
-
-    def __str__(self):
-        return "Task: determine appropriate fingerprint type and " \
-               "similarity measure for property of interest"
-
-    def get_best_measure(self,
-                         molecule_set_configs,
-                         fingerprint_type=None,
-                         similarity_measure=None,
-                         subsample_subset_size=0.01,
-                         optim_algo='max_min',
-                         only_metric=False,
-                         show_top=0,
-                         ):
-        """Get the best measure for quantity of interest.
-
-        Args:
-            molecule_set_configs (dict): All configurations (except
-                fingerprint_type and similarity_measure) needed to form
-                the moleculeSet.
-            fingerprint_type (str): Label to indicate which fingerprint to
-                use. If supplied, fingerprint is fixed and optimization
-                carried out over similarity measures. Use None to indicate
-                that optimization needs to be carried out over fingerprints.
-                Default is None.
-            similarity_measure (str): Label to indicate which similarity
-                measure to use. If supplied, similarity measure is fixed
-                and optimization carried out over similarity measures.
-                Use None to indicate that optimization needs to be carried
-                out over fingerprints. Default is None.
-            subsample_subset_size (float): Fraction of molecule_set to
-                subsample. This is separate from the sample_ratio parameter
-                used when creating a moleculeSet since it is recommended
-                to have an more aggressive subsampling strategy for this task
-                due to the combinatorial explosion of looking at multiple
-                fingerprints and similarity measures. Default is 0.01.
-            optim_algo (str): Label to indicate the optimization algorithm
-                chosen. Options are:
-                'max': The measure choice which maximizes correlation
-                    of properties between nearest neighbors (most similar).
-                    This is the default.
-                'min': The measure choice which minimizes the absolute value of
-                    property correlation between furthest neighbors
-                    (most dissimilar).
-                'max_min': The measure choice which maximizes correlation
-                    of properties between nearest neighbors (most similar)
-                    and minimizes he absolute value of property correlation
-                    between furthest neighbors (most dissimilar).
-                    This is the default.
-            only_metric (bool): If True only similarity measures satisfying
-                the metricity property
-                (i.e. can be converted to distance metrics) are selected.
-
-        Returns:
-            (NamedTuple): Top performer with fields:
-                fingerprint_type (str): Label for fingerprint type
-               similarity_measure (str): Label for similarity measure
-               nearest_neighbor_correlation (float): Correlation of property
-                   of molecule and its nearest neighbor.
-               furthest_neighbor_correlation (float): Correlation of property
-                   of molecule and its furthest neighbor.
-               score_ (float): Overall score based on optimization strategy.
-                   More is better.
-
-        """
-        return self.__call__(
-            molecule_set_configs,
-            fingerprint_type=fingerprint_type,
-            similarity_measure=similarity_measure,
-            subsample_subset_size=subsample_subset_size,
-            optim_algo=optim_algo,
-            only_metric=only_metric,
-            show_top=show_top,
-        )
+"""Identify most appropriate choice of fingerprint and similarity measure by
+evaluating the response of the nearest and furthest neighbors. This is called
+measure choice for brevity (although both measure and features are chosen)"""
+from collections import namedtuple
+import json
+from os import makedirs
+from os.path import dirname
+
+import numpy as np
+
+from aimsim.chemical_datastructures import MoleculeSet
+from aimsim.exceptions import InvalidConfigurationError
+from aimsim.ops import Descriptor, SimilarityMeasure
+from aimsim.utils.plotting_scripts import plot_multiple_barchart
+from .task import Task
+from .see_property_variation_with_similarity \
+    import SeePropertyVariationWithSimilarity
+
+
+class MeasureSearch(Task):
+    def __init__(self, configs=None, **kwargs):
+        if configs is None:
+            configs = dict()
+        configs.update(kwargs)
+        super().__init__(configs)
+        self.plot_settings = None
+        self.log_fpath = None
+        self._extract_configs()
+
+    def _extract_configs(self):
+        """
+        Raises:
+        InvalidConfigurationError: If correlation_type does not match
+                                   implemented types.
+        """
+        self.plot_settings = {'colors': ['#78DEC7', '#FB7AFC', '#FBC7F7'],
+                              'xticksize': 10,
+                              'yticksize': 20,
+                              'title': "",
+                              'title_fontsize': 24,
+                              'xlabel_fontsize': 20,
+                              'ylabel_fontsize': 20,
+                              }
+        self.plot_settings.update(self.configs.get("plot_settings",
+                                                   {}))
+        try:
+            self.prop_var_w_similarity = SeePropertyVariationWithSimilarity(
+                correlation_type=self.configs.get('correlation_type'))
+        except InvalidConfigurationError as e:
+            raise e
+        self.log_fpath = self.configs.get("log_file_path", None)
+        if self.log_fpath is not None:
+            log_dir = dirname(self.log_fpath)
+            makedirs(log_dir, exist_ok=True)
+
+    def __call__(self,
+                 molecule_set_configs,
+                 fingerprint_type=None,
+                 fingerprint_params=None,
+                 similarity_measure=None,
+                 subsample_subset_size=0.01,
+                 optim_algo='max_min',
+                 show_top=0,
+                 only_metric=True,
+                 ):
+        """
+        Calculate the correlation in the properties of molecules in set
+        and their nearest and furthest neighbors using different
+        fingerprints / similarity measure choices. Choose the best fingerprint
+        and similarity measure pair (called measure choice for brevity)
+        based on an optimization strategy.
+
+        Args:
+            molecule_set_configs (dict): All configurations (except
+                fingerprint_type, fingerprint_params and similarity_measure)
+                needed to form the moleculeSet.
+            fingerprint_type (str): Label to indicate which fingerprint to
+                use. If supplied, fingerprint is fixed and optimization
+                carried out over similarity measures. Use None to indicate
+                that optimization needs to be carried out over fingerprints.
+                Default is None.
+            fingerprint_params (dict): Hyper-parameters for fingerprints.
+                Passed to the MoleculeSet constructor. If None is passed,
+                set to empty dictionary before passing to MoleculeSet.
+            similarity_measure (str): Label to indicate which similarity
+                measure to use. If supplied, similarity measure is fixed
+                and optimization carried out over similarity measures.
+                Use None to indicate that optimization needs to be carried
+                out over fingerprints. Default is None.
+            subsample_subset_size (float): Fraction of molecule_set to
+                subsample. This is separate from the sample_ratio parameter
+                used when creating a moleculeSet since it is recommended
+                to have an more aggressive subsampling strategy for this task
+                due to the combinatorial explosion of looking at multiple
+                fingerprints and similarity measures. Default is 0.01.
+            optim_algo (str): Label to indicate the optimization algorithm
+                chosen. Options are:
+                'max': The measure choice which maximizes correlation
+                    of properties between nearest neighbors (most similar).
+                    This is the default.
+                'min': The measure choice which minimizes the absolute value
+                    of property correlation
+                    between furthest neighbors (most dissimilar).
+                'max_min': The measure choice which maximizes correlation
+                    of properties between nearest neighbors (most similar)
+                    and minimizes he absolute value of property correlation
+                    between furthest neighbors (most dissimilar).
+                    This is the default.
+            show_top (int): Number of top performing measures to show in plot.
+                If 0, no plots are generated and the top performer is returned.
+            only_metric (bool): If True only similarity measures satisfying
+                the metricity property
+                (i.e. can be converted to distance metrics) are selected.
+
+        Returns:
+            (NamedTuple): Top performer with fields:
+                fingerprint_type (str): Label for fingerprint type
+               similarity_measure (str): Label for similarity measure
+               nearest_neighbor_correlation (float): Correlation of property
+                   of molecule and its nearest neighbor.
+               furthest_neighbor_correlation (float): Correlation of property
+                   of molecule and its furthest neighbor.
+               score_ (float): Overall score based on optimization strategy.
+                   More is better.
+
+        """
+        print(f'Using subsample size {subsample_subset_size} for '
+              f'measure search')
+        trial_ = namedtuple('trial_', ['fingerprint_type',
+                                       'similarity_measure',
+                                       'nearest_neighbor_correlation',
+                                       'furthest_neighbor_correlation',
+                                       'score_'])
+        if fingerprint_type is None:
+            all_fingerprint_types = Descriptor.get_supported_fprints()
+            fingerprint_params = None
+        else:
+            all_fingerprint_types = [fingerprint_type]
+        if similarity_measure is None:
+            if only_metric:
+                print('Only trying measures with valid distance metrics')
+            all_similarity_measures = SimilarityMeasure.get_uniq_metrics()
+        else:
+            all_similarity_measures = [similarity_measure]
+        is_verbose = molecule_set_configs.get("is_verbose", False)
+        all_scores = []
+        if fingerprint_params is None:
+            fingerprint_params = {}
+        for similarity_measure in all_similarity_measures:
+            if only_metric and not SimilarityMeasure(
+                    metric=similarity_measure).is_distance_metric():
+                continue
+            if is_verbose:
+                print(f'Trying {similarity_measure} similarity')
+            for fingerprint_type in all_fingerprint_types:
+                if is_verbose:
+                    print(f'Trying {fingerprint_type} fingerprint')
+                try:
+                    molecule_set = MoleculeSet(
+                        molecule_database_src=molecule_set_configs[
+                            'molecule_database_src'],
+                        molecule_database_src_type=molecule_set_configs[
+                            'molecule_database_src_type'],
+                        similarity_measure=similarity_measure,
+                        fingerprint_type=fingerprint_type,
+                        fingerprint_params=fingerprint_params,
+                        is_verbose=is_verbose,
+                        n_threads=molecule_set_configs.get(
+                            'n_threads', 1),
+                        sampling_ratio=subsample_subset_size)
+                except (InvalidConfigurationError, ValueError, RuntimeError) as e:
+                    if is_verbose:
+                        print(f'Could not try {fingerprint_type} with '
+                              f'similarity measure {similarity_measure} due to '
+                              f'{e}')
+                    continue
+                nearest_corr, nearest_p_val = self.prop_var_w_similarity. \
+                    get_property_correlations_in_most_similar(
+                        molecule_set)
+                furthest_corr, furthest_p_val = self.prop_var_w_similarity. \
+                    get_property_correlations_in_most_dissimilar(
+                        molecule_set)
+                if optim_algo == 'max_min':
+                    score_ = nearest_corr - abs(furthest_corr)
+                elif optim_algo == 'max':
+                    score_ = nearest_corr
+                elif optim_algo == 'min':
+                    score_ = -abs(furthest_corr)
+                else:
+                    raise InvalidConfigurationError(f'{optim_algo} '
+                                                    f'not implemented')
+                all_scores.append(trial_(
+                    fingerprint_type=fingerprint_type,
+                    similarity_measure=similarity_measure,
+                    nearest_neighbor_correlation=nearest_corr,
+                    furthest_neighbor_correlation=furthest_corr,
+                    score_=score_))
+        all_scores.sort(key=lambda x: x[-1], reverse=True)
+        if self.log_fpath is not None:
+            print('Writing to ', self.log_fpath)
+            log_data = [trial._asdict() for trial in all_scores]
+            with open(self.log_fpath, "w") as fp:
+                json.dump(log_data, fp)
+
+        if show_top > 0:
+            top_performers = all_scores[:show_top]
+            all_nearest_neighbor_correlations = []
+            all_furthest_neighbor_correlations = []
+            top_scores = []
+            all_measures = []
+            for trial in top_performers:
+                all_nearest_neighbor_correlations.append(
+                    trial.nearest_neighbor_correlation)
+                all_furthest_neighbor_correlations.append(
+                    trial.furthest_neighbor_correlation)
+                top_scores.append(trial.score_)
+                all_measures.append(Descriptor.shorten_label(
+                    trial.fingerprint_type)
+                    + '\n'
+                    + trial.similarity_measure)
+            bar_heights = np.array([top_scores,
+                                    all_nearest_neighbor_correlations,
+                                    all_furthest_neighbor_correlations])
+            colors = self.plot_settings.pop('colors')
+            plot_multiple_barchart(x=[_ for _ in range(len(top_performers))],
+                                   heights=bar_heights,
+                                   legend_labels=['Overall scores',
+                                                  'Nearest neighbor property '
+                                                  'correlation',
+                                                  'Furthest neighbor property '
+                                                  'correlations'],
+                                   colors=colors,
+                                   xtick_labels=all_measures,
+                                   ylabel='Value',
+                                   xlabel='Measure',
+                                   **self.plot_settings)
+
+        return all_scores[0]
+
+    def __str__(self):
+        return "Task: determine appropriate fingerprint type and " \
+               "similarity measure for property of interest"
+
+    def get_best_measure(self,
+                         molecule_set_configs,
+                         fingerprint_type=None,
+                         similarity_measure=None,
+                         subsample_subset_size=0.01,
+                         optim_algo='max_min',
+                         only_metric=False,
+                         show_top=0,
+                         ):
+        """Get the best measure for quantity of interest.
+
+        Args:
+            molecule_set_configs (dict): All configurations (except
+                fingerprint_type and similarity_measure) needed to form
+                the moleculeSet.
+            fingerprint_type (str): Label to indicate which fingerprint to
+                use. If supplied, fingerprint is fixed and optimization
+                carried out over similarity measures. Use None to indicate
+                that optimization needs to be carried out over fingerprints.
+                Default is None.
+            similarity_measure (str): Label to indicate which similarity
+                measure to use. If supplied, similarity measure is fixed
+                and optimization carried out over similarity measures.
+                Use None to indicate that optimization needs to be carried
+                out over fingerprints. Default is None.
+            subsample_subset_size (float): Fraction of molecule_set to
+                subsample. This is separate from the sample_ratio parameter
+                used when creating a moleculeSet since it is recommended
+                to have an more aggressive subsampling strategy for this task
+                due to the combinatorial explosion of looking at multiple
+                fingerprints and similarity measures. Default is 0.01.
+            optim_algo (str): Label to indicate the optimization algorithm
+                chosen. Options are:
+                'max': The measure choice which maximizes correlation
+                    of properties between nearest neighbors (most similar).
+                    This is the default.
+                'min': The measure choice which minimizes the absolute value of
+                    property correlation between furthest neighbors
+                    (most dissimilar).
+                'max_min': The measure choice which maximizes correlation
+                    of properties between nearest neighbors (most similar)
+                    and minimizes he absolute value of property correlation
+                    between furthest neighbors (most dissimilar).
+                    This is the default.
+            only_metric (bool): If True only similarity measures satisfying
+                the metricity property
+                (i.e. can be converted to distance metrics) are selected.
+
+        Returns:
+            (NamedTuple): Top performer with fields:
+                fingerprint_type (str): Label for fingerprint type
+               similarity_measure (str): Label for similarity measure
+               nearest_neighbor_correlation (float): Correlation of property
+                   of molecule and its nearest neighbor.
+               furthest_neighbor_correlation (float): Correlation of property
+                   of molecule and its furthest neighbor.
+               score_ (float): Overall score based on optimization strategy.
+                   More is better.
+
+        """
+        return self.__call__(
+            molecule_set_configs,
+            fingerprint_type=fingerprint_type,
+            similarity_measure=similarity_measure,
+            subsample_subset_size=subsample_subset_size,
+            optim_algo=optim_algo,
+            only_metric=only_metric,
+            show_top=show_top,
+        )
```

### Comparing `aimsim-2.0.2/aimsim/tasks/see_property_variation_with_similarity.py` & `aimsim-2.0.3/aimsim/tasks/see_property_variation_with_similarity.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-"""Task to visualize property similarity over a dataset."""
-from os import makedirs
-from os.path import dirname
-
-import matplotlib.pyplot as plt
-from scipy.stats import pearsonr
-
-from aimsim.utils.plotting_scripts import plot_parity
-from aimsim.exceptions import InvalidConfigurationError
-from .task import Task
-
-
-class SeePropertyVariationWithSimilarity(Task):
-    def __init__(self, configs=None, **kwargs):
-        if configs is None:
-            configs = dict()  # all configs are optional
-        configs.update(kwargs)
-        super().__init__(configs)
-        self.plot_settings = None
-        self.log_fpath = None
-        self._extract_configs()
-
-    def _extract_configs(self):
-        """
-        Raises:
-        InvalidConfigurationError: If correlation_type does not match
-                                   implemented types.
-        """
-        self.plot_settings = {"response": "response"}
-        self.plot_settings.update(self.configs.get("property_plot_settings",
-                                                   {}))
-        self.log_fpath = self.configs.get("log_file_path", None)
-        self.correlation_type = self.configs.get('correlation_type')
-        if self.correlation_type is None:
-            self.correlation_type = 'pearson'
-        if self.correlation_type.lower() in ['pearson', 'linear']:
-            self.correlation_fn = pearsonr
-        else:
-            raise InvalidConfigurationError(f'{self.correlation_type} correlation '
-                                            f'not supported')
-        if self.log_fpath is not None:
-            log_dir = dirname(self.log_fpath)
-            makedirs(log_dir, exist_ok=True)
-
-    def __call__(self, molecule_set):
-        """Plot the variation of molecular property with molecular fingerprint.
-
-        Args:
-            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
-                Molecules object of the molecule database.
-
-        """
-        ref_prop, similar_prop = self._get_ref_neighbor_properties(
-            molecule_set)
-
-        # scipy gives a remarkably unhelpful error if properties are not provided
-        try:
-            similar_correlation_ = self.correlation_fn(ref_prop, similar_prop)
-        except ValueError as e:
-            raise ValueError(
-                "Unable to generate Property Simlilarty plot.\n" +
-                "Check for properly formatted properties in your input file."
-            )
-        if molecule_set.is_verbose:
-            print("Plotting Responses of Similar Molecules")
-        plot_parity(
-            ref_prop,
-            similar_prop,
-            xlabel=f'Reference molecule {self.plot_settings["response"]}',
-            ylabel=f'Most similar molecule {self.plot_settings["response"]}',
-            text="Correlation: {:.2f} (p-value {:.2f})".format(
-                similar_correlation_[0], similar_correlation_[1]),
-            **self.plot_settings,
-        )
-
-        ref_prop, dissimilar_prop = self._get_ref_neighbor_properties(
-            molecule_set=molecule_set,
-            nearest=False)
-        dissimilar_correlation_ = self.correlation_fn(
-            ref_prop, dissimilar_prop)
-        if molecule_set.is_verbose:
-            print("Plotting Responses of Dissimilar Molecules")
-        plot_parity(
-            ref_prop,
-            dissimilar_prop,
-            xlabel=f'Reference molecule {self.plot_settings["response"]}',
-            ylabel=f'Most dissimilar molecule {self.plot_settings["response"]}',
-            text="Correlation: {:.2f} (p-value {:.2f})".format(
-                dissimilar_correlation_[0], dissimilar_correlation_[1]),
-            **self.plot_settings,
-        )
-
-        text_prompt = (
-            f"{self.correlation_type} correlation in the properties of the "
-            "most similar molecules\n"
-        )
-        text_prompt += "-" * 60
-        text_prompt += "\n\n"
-        text_prompt += f"{similar_correlation_[0]}"
-        text_prompt += "\n"
-        text_prompt += f"2 tailed p-value: {similar_correlation_[1]}"
-        text_prompt += "\n\n\n\n"
-        text_prompt = (
-            f"{self.correlation_type} in the properties of the "
-            f"most dissimilar molecules\n"
-        )
-        text_prompt += "-" * 60
-        text_prompt += "\n\n"
-        text_prompt += f"{dissimilar_correlation_[0]}"
-        text_prompt += "\n"
-        text_prompt += "2 tailed p-value: "
-        text_prompt += f"{dissimilar_correlation_[1]}"
-        if self.log_fpath is None:
-            print(text_prompt)
-        else:
-            if molecule_set.is_verbose:
-                print(text_prompt)
-            print("Writing to file ", self.log_fpath)
-            with open(self.log_fpath, "w") as fp:
-                fp.write(text_prompt)
-
-    def get_property_correlations_in_most_similar(self, molecule_set):
-        """Get the correlation between the property of molecules and their
-        nearest (most similar) neighbors
-        Args:
-            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
-                Molecules object of the molecule database.
-        Return:
-            (float): Correlation between properties.
-
-        """
-        ref_prop, similar_prop = self._get_ref_neighbor_properties(
-            molecule_set)
-        return self.correlation_fn(ref_prop, similar_prop)
-
-    def get_property_correlations_in_most_dissimilar(self, molecule_set):
-        """Get the correlation between the property of molecules and their
-        furthest (most dissimilar) neighbors
-        Args:
-            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
-                Molecules object of the molecule database.
-        Return:
-            (float): Correlation between properties.
-
-        """
-        ref_prop, dissimilar_prop = self._get_ref_neighbor_properties(
-            molecule_set=molecule_set,
-            nearest=False)
-        return self.correlation_fn(ref_prop, dissimilar_prop)
-
-    def _get_ref_neighbor_properties(self, molecule_set, nearest=True):
-        """Get the properties of reference molecules and their nearest
-        or furthest neighbors.
-        Args:
-            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
-                Molecules object of the molecule database.
-            nearest (bool):
-                If True nearest (most similar) neighbors are used,
-                else furthest (most dissimilar). Default is True.
-        Returns:
-            (tuple): The first index is an array of reference mol
-            properties and the second index is an array of the
-            property of their respective neighbors.
-
-        """
-        if nearest:
-            return molecule_set.get_property_of_most_similar()
-        else:
-            return molecule_set.get_property_of_most_dissimilar()
-
-    def __str__(self):
-        return "Task: see variation of molecule property with similarity"
+"""Task to visualize property similarity over a dataset."""
+from os import makedirs
+from os.path import dirname
+
+import matplotlib.pyplot as plt
+from scipy.stats import pearsonr
+
+from aimsim.utils.plotting_scripts import plot_parity
+from aimsim.exceptions import InvalidConfigurationError
+from .task import Task
+
+
+class SeePropertyVariationWithSimilarity(Task):
+    def __init__(self, configs=None, **kwargs):
+        if configs is None:
+            configs = dict()  # all configs are optional
+        configs.update(kwargs)
+        super().__init__(configs)
+        self.plot_settings = None
+        self.log_fpath = None
+        self._extract_configs()
+
+    def _extract_configs(self):
+        """
+        Raises:
+        InvalidConfigurationError: If correlation_type does not match
+                                   implemented types.
+        """
+        self.plot_settings = {"response": "response"}
+        self.plot_settings.update(self.configs.get("property_plot_settings",
+                                                   {}))
+        self.log_fpath = self.configs.get("log_file_path", None)
+        self.correlation_type = self.configs.get('correlation_type')
+        if self.correlation_type is None:
+            self.correlation_type = 'pearson'
+        if self.correlation_type.lower() in ['pearson', 'linear']:
+            self.correlation_fn = pearsonr
+        else:
+            raise InvalidConfigurationError(f'{self.correlation_type} correlation '
+                                            f'not supported')
+        if self.log_fpath is not None:
+            log_dir = dirname(self.log_fpath)
+            makedirs(log_dir, exist_ok=True)
+
+    def __call__(self, molecule_set):
+        """Plot the variation of molecular property with molecular fingerprint.
+
+        Args:
+            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
+                Molecules object of the molecule database.
+
+        """
+        ref_prop, similar_prop = self._get_ref_neighbor_properties(
+            molecule_set)
+
+        # scipy gives a remarkably unhelpful error if properties are not provided
+        try:
+            similar_correlation_ = self.correlation_fn(ref_prop, similar_prop)
+        except ValueError as e:
+            raise ValueError(
+                "Unable to generate Property Simlilarty plot.\n" +
+                "Check for properly formatted properties in your input file."
+            )
+        if molecule_set.is_verbose:
+            print("Plotting Responses of Similar Molecules")
+        plot_parity(
+            ref_prop,
+            similar_prop,
+            xlabel=f'Reference molecule {self.plot_settings["response"]}',
+            ylabel=f'Most similar molecule {self.plot_settings["response"]}',
+            text="Correlation: {:.2f} (p-value {:.2f})".format(
+                similar_correlation_[0], similar_correlation_[1]),
+            **self.plot_settings,
+        )
+
+        ref_prop, dissimilar_prop = self._get_ref_neighbor_properties(
+            molecule_set=molecule_set,
+            nearest=False)
+        dissimilar_correlation_ = self.correlation_fn(
+            ref_prop, dissimilar_prop)
+        if molecule_set.is_verbose:
+            print("Plotting Responses of Dissimilar Molecules")
+        plot_parity(
+            ref_prop,
+            dissimilar_prop,
+            xlabel=f'Reference molecule {self.plot_settings["response"]}',
+            ylabel=f'Most dissimilar molecule {self.plot_settings["response"]}',
+            text="Correlation: {:.2f} (p-value {:.2f})".format(
+                dissimilar_correlation_[0], dissimilar_correlation_[1]),
+            **self.plot_settings,
+        )
+
+        text_prompt = (
+            f"{self.correlation_type} correlation in the properties of the "
+            "most similar molecules\n"
+        )
+        text_prompt += "-" * 60
+        text_prompt += "\n\n"
+        text_prompt += f"{similar_correlation_[0]}"
+        text_prompt += "\n"
+        text_prompt += f"2 tailed p-value: {similar_correlation_[1]}"
+        text_prompt += "\n\n\n\n"
+        text_prompt = (
+            f"{self.correlation_type} in the properties of the "
+            f"most dissimilar molecules\n"
+        )
+        text_prompt += "-" * 60
+        text_prompt += "\n\n"
+        text_prompt += f"{dissimilar_correlation_[0]}"
+        text_prompt += "\n"
+        text_prompt += "2 tailed p-value: "
+        text_prompt += f"{dissimilar_correlation_[1]}"
+        if self.log_fpath is None:
+            print(text_prompt)
+        else:
+            if molecule_set.is_verbose:
+                print(text_prompt)
+            print("Writing to file ", self.log_fpath)
+            with open(self.log_fpath, "w") as fp:
+                fp.write(text_prompt)
+
+    def get_property_correlations_in_most_similar(self, molecule_set):
+        """Get the correlation between the property of molecules and their
+        nearest (most similar) neighbors
+        Args:
+            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
+                Molecules object of the molecule database.
+        Return:
+            (float): Correlation between properties.
+
+        """
+        ref_prop, similar_prop = self._get_ref_neighbor_properties(
+            molecule_set)
+        return self.correlation_fn(ref_prop, similar_prop)
+
+    def get_property_correlations_in_most_dissimilar(self, molecule_set):
+        """Get the correlation between the property of molecules and their
+        furthest (most dissimilar) neighbors
+        Args:
+            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
+                Molecules object of the molecule database.
+        Return:
+            (float): Correlation between properties.
+
+        """
+        ref_prop, dissimilar_prop = self._get_ref_neighbor_properties(
+            molecule_set=molecule_set,
+            nearest=False)
+        return self.correlation_fn(ref_prop, dissimilar_prop)
+
+    def _get_ref_neighbor_properties(self, molecule_set, nearest=True):
+        """Get the properties of reference molecules and their nearest
+        or furthest neighbors.
+        Args:
+            molecule_set (AIMSim.chemical_datastructures MoleculeSet):
+                Molecules object of the molecule database.
+            nearest (bool):
+                If True nearest (most similar) neighbors are used,
+                else furthest (most dissimilar). Default is True.
+        Returns:
+            (tuple): The first index is an array of reference mol
+            properties and the second index is an array of the
+            property of their respective neighbors.
+
+        """
+        if nearest:
+            return molecule_set.get_property_of_most_similar()
+        else:
+            return molecule_set.get_property_of_most_dissimilar()
+
+    def __str__(self):
+        return "Task: see variation of molecule property with similarity"
```

### Comparing `aimsim-2.0.2/aimsim/tasks/task_manager.py` & `aimsim-2.0.3/aimsim/tasks/task_manager.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-"""Class to call al tasks in sequence."""
-import plotly.graph_objects as go
-from aimsim.chemical_datastructures import MoleculeSet
-from aimsim.exceptions import InvalidConfigurationError
-from aimsim.tasks import *
-
-import matplotlib.pyplot as plt
-
-
-class TaskManager:
-    def __init__(self, tasks):
-        """Sequentially launches all the tasks from the configuration file.
-
-        Args:
-            tasks (dict): The tasks field of the config yaml containing various
-                tasks and their parameters.
-        """
-        self.to_do = []
-        self.molecule_set = None
-        self._set_tasks(tasks)
-
-    def _set_tasks(self, tasks):
-        """
-        Args:
-            tasks (dict): The tasks field of the config yaml containing various
-            tasks and their parameters.
-        """
-        for task, task_configs in tasks.items():
-            try:
-                if task == "compare_target_molecule":
-                    loaded_task = CompareTargetMolecule(task_configs)
-                elif task == "visualize_dataset":
-                    loaded_task = VisualizeDataset(task_configs)
-                elif task == "see_property_variation_w_similarity":
-                    loaded_task = SeePropertyVariationWithSimilarity(
-                        task_configs)
-                elif task == "identify_outliers":
-                    loaded_task = IdentifyOutliers(task_configs)
-                elif task == "cluster":
-                    loaded_task = ClusterData(task_configs)
-                else:
-                    print(f"{task} not recognized")
-                    continue
-                self.to_do.append(loaded_task)
-            except InvalidConfigurationError as e:
-                print(f"Error in the config file for task: ", task)
-                print("\n", e)
-                raise e
-
-        if len(self.to_do) == 0:
-            raise InvalidConfigurationError("No tasks were read, exiting.")
-
-    def _initialize_molecule_set(self, molecule_set_configs):
-        """Initialize molecule_set attribute to a MoleculeSet object
-        based on parameters in the config file.
-
-        Args:
-            molecule_set_configs (dict): Configurations for initializing
-                the MoleculeSet object.
-        """
-        molecule_database_src = molecule_set_configs.get(
-            "molecule_database",
-            None,
-        )
-        database_src_type = molecule_set_configs.get(
-            "molecule_database_source_type", None
-        )
-        if molecule_database_src is None or database_src_type is None:
-            print("molecule_database fields not set in config file")
-            print(f"molecule_database: {molecule_database_src}")
-            print(f"molecule_database_source_type: {database_src_type}")
-            raise InvalidConfigurationError
-        is_verbose = molecule_set_configs.get("is_verbose", False)
-        n_threads = molecule_set_configs.get("n_workers", 1)
-        similarity_measure = molecule_set_configs.get("similarity_measure",
-                                                      'determine')
-        fingerprint_type = molecule_set_configs.get('fingerprint_type',
-                                                    'determine')
-        fingerprint_params = molecule_set_configs.get('fingerprint_params', {})
-        if similarity_measure == 'determine' or fingerprint_type == 'determine':
-            subsample_subset_size = molecule_set_configs.get(
-                'measure_id_subsample',
-                0.05)
-            only_valid_dist = molecule_set_configs.get(
-                    'only_valid_dist',
-                    True)
-            if is_verbose:
-                print('Determining best fingerprint_type / similarity_measure')
-            measure_search = MeasureSearch(correlation_type='pearson')
-            if similarity_measure == 'determine':
-                similarity_measure = None
-            if fingerprint_type == 'determine':
-                fingerprint_type = None
-                fingerprint_params = {}
-            measure_search_molset_configs = {
-                'molecule_database_src': molecule_database_src,
-                'molecule_database_src_type': database_src_type,
-                'is_verbose': is_verbose,
-                'n_threads': n_threads,
-            }
-
-            best_measure = measure_search(
-                molecule_set_configs=measure_search_molset_configs,
-                similarity_measure=similarity_measure,
-                fingerprint_type=fingerprint_type,
-                fingerprint_params=fingerprint_params,
-                subsample_subset_size=subsample_subset_size,
-                show_top=5,
-                only_metric=only_valid_dist)
-            similarity_measure = best_measure.similarity_measure
-            fingerprint_type = best_measure.fingerprint_type
-            print(f'Chosen measure: {fingerprint_type} '
-                  f'and {similarity_measure}.')
-
-        sampling_ratio = molecule_set_configs.get("sampling_ratio", 1.)
-        print(f'Choosing sampling ratio of {sampling_ratio} for tasks')
-        self.molecule_set = MoleculeSet(
-            molecule_database_src=molecule_database_src,
-            molecule_database_src_type=database_src_type,
-            similarity_measure=similarity_measure,
-            fingerprint_type=fingerprint_type,
-            fingerprint_params=fingerprint_params,
-            is_verbose=is_verbose,
-            n_threads=n_threads,
-            sampling_ratio=sampling_ratio,
-        )
-
-    def __call__(self, molecule_set_configs):
-        """Launch all tasks from the queue.
-
-        Args:
-            molecule_set_configs (dict): Configurations for the molecule_set.
-        """
-        self._initialize_molecule_set(molecule_set_configs)
-        if self.molecule_set.is_verbose:
-            print("Beginning tasks...")
-        for task_id, task in enumerate(self.to_do):
-            print(f"Task ({task_id + 1} / {len(self.to_do)}) {task}")
-            try:
-                task(self.molecule_set)
-            except InvalidConfigurationError as e:
-                print(
-                    f"{task} could not be performed due to the "
-                    f"following error: {e.message}"
-                )
-                continue
-        plt.show()
+"""Class to call al tasks in sequence."""
+import plotly.graph_objects as go
+from aimsim.chemical_datastructures import MoleculeSet
+from aimsim.exceptions import InvalidConfigurationError
+from aimsim.tasks import *
+
+import matplotlib.pyplot as plt
+
+
+class TaskManager:
+    def __init__(self, tasks):
+        """Sequentially launches all the tasks from the configuration file.
+
+        Args:
+            tasks (dict): The tasks field of the config yaml containing various
+                tasks and their parameters.
+        """
+        self.to_do = []
+        self.molecule_set = None
+        self._set_tasks(tasks)
+
+    def _set_tasks(self, tasks):
+        """
+        Args:
+            tasks (dict): The tasks field of the config yaml containing various
+            tasks and their parameters.
+        """
+        for task, task_configs in tasks.items():
+            try:
+                if task == "compare_target_molecule":
+                    loaded_task = CompareTargetMolecule(task_configs)
+                elif task == "visualize_dataset":
+                    loaded_task = VisualizeDataset(task_configs)
+                elif task == "see_property_variation_w_similarity":
+                    loaded_task = SeePropertyVariationWithSimilarity(
+                        task_configs)
+                elif task == "identify_outliers":
+                    loaded_task = IdentifyOutliers(task_configs)
+                elif task == "cluster":
+                    loaded_task = ClusterData(task_configs)
+                else:
+                    print(f"{task} not recognized")
+                    continue
+                self.to_do.append(loaded_task)
+            except InvalidConfigurationError as e:
+                print(f"Error in the config file for task: ", task)
+                print("\n", e)
+                raise e
+
+        if len(self.to_do) == 0:
+            raise InvalidConfigurationError("No tasks were read, exiting.")
+
+    def _initialize_molecule_set(self, molecule_set_configs):
+        """Initialize molecule_set attribute to a MoleculeSet object
+        based on parameters in the config file.
+
+        Args:
+            molecule_set_configs (dict): Configurations for initializing
+                the MoleculeSet object.
+        """
+        molecule_database_src = molecule_set_configs.get(
+            "molecule_database",
+            None,
+        )
+        database_src_type = molecule_set_configs.get(
+            "molecule_database_source_type", None
+        )
+        if molecule_database_src is None or database_src_type is None:
+            print("molecule_database fields not set in config file")
+            print(f"molecule_database: {molecule_database_src}")
+            print(f"molecule_database_source_type: {database_src_type}")
+            raise InvalidConfigurationError
+        is_verbose = molecule_set_configs.get("is_verbose", False)
+        n_threads = molecule_set_configs.get("n_workers", 1)
+        similarity_measure = molecule_set_configs.get("similarity_measure",
+                                                      'determine')
+        fingerprint_type = molecule_set_configs.get('fingerprint_type',
+                                                    'determine')
+        fingerprint_params = molecule_set_configs.get('fingerprint_params', {})
+        if similarity_measure == 'determine' or fingerprint_type == 'determine':
+            subsample_subset_size = molecule_set_configs.get(
+                'measure_id_subsample',
+                0.05)
+            only_valid_dist = molecule_set_configs.get(
+                    'only_valid_dist',
+                    True)
+            if is_verbose:
+                print('Determining best fingerprint_type / similarity_measure')
+            measure_search = MeasureSearch(correlation_type='pearson')
+            if similarity_measure == 'determine':
+                similarity_measure = None
+            if fingerprint_type == 'determine':
+                fingerprint_type = None
+                fingerprint_params = {}
+            measure_search_molset_configs = {
+                'molecule_database_src': molecule_database_src,
+                'molecule_database_src_type': database_src_type,
+                'is_verbose': is_verbose,
+                'n_threads': n_threads,
+            }
+
+            best_measure = measure_search(
+                molecule_set_configs=measure_search_molset_configs,
+                similarity_measure=similarity_measure,
+                fingerprint_type=fingerprint_type,
+                fingerprint_params=fingerprint_params,
+                subsample_subset_size=subsample_subset_size,
+                show_top=5,
+                only_metric=only_valid_dist)
+            similarity_measure = best_measure.similarity_measure
+            fingerprint_type = best_measure.fingerprint_type
+            print(f'Chosen measure: {fingerprint_type} '
+                  f'and {similarity_measure}.')
+
+        sampling_ratio = molecule_set_configs.get("sampling_ratio", 1.)
+        print(f'Choosing sampling ratio of {sampling_ratio} for tasks')
+        self.molecule_set = MoleculeSet(
+            molecule_database_src=molecule_database_src,
+            molecule_database_src_type=database_src_type,
+            similarity_measure=similarity_measure,
+            fingerprint_type=fingerprint_type,
+            fingerprint_params=fingerprint_params,
+            is_verbose=is_verbose,
+            n_threads=n_threads,
+            sampling_ratio=sampling_ratio,
+        )
+
+    def __call__(self, molecule_set_configs):
+        """Launch all tasks from the queue.
+
+        Args:
+            molecule_set_configs (dict): Configurations for the molecule_set.
+        """
+        self._initialize_molecule_set(molecule_set_configs)
+        if self.molecule_set.is_verbose:
+            print("Beginning tasks...")
+        for task_id, task in enumerate(self.to_do):
+            print(f"Task ({task_id + 1} / {len(self.to_do)}) {task}")
+            try:
+                task(self.molecule_set)
+            except InvalidConfigurationError as e:
+                print(
+                    f"{task} could not be performed due to the "
+                    f"following error: {e.message}"
+                )
+                continue
+        plt.show()
```

### Comparing `aimsim-2.0.2/aimsim/tasks/visualize_dataset.py` & `aimsim-2.0.3/aimsim/tasks/visualize_dataset.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-"""Create similarity plots for the dataset."""
-import matplotlib.pyplot as plt
-
-from .task import Task
-from aimsim.utils.plotting_scripts import (
-    plot_density,
-    plot_heatmap,
-    plot_scatter,
-    plot_scatter_interactive,
-)
-
-
-class VisualizeDataset(Task):
-    def __init__(self, configs=None, **kwargs):
-        """
-        Constructor for the VisualizeDataset class.
-
-        Args:
-            configs(dict): Dictionary of configurations. Default is None.
-            **kwargs: Keyword arguments to modify configs fields.
-        Notes:
-            The configuration structure with default values are:
-            heatmap_plot_settings: {}  # pass through keywords for
-                                       # aimsim.utils.plotting_scripts.\
-                                       #  plot_heatmap
-            similarity_plot_settings: {}   # pass through keywords for
-                                           # aimsim.utils.plotting_scripts. \
-                                           #plot_density
-            embedding_plot_settings:
-                    {'plot_color': 'red'
-                     'plot_title': '2-D projected space',
-                     'xlabel': 'Dimension 1',
-                     'ylabel': 'Dimension 2',
-                     'embedding': {'method': "mds",
-                                    'params': {'random_state': 42}}}
-
-        """
-        if configs is None:
-            configs = dict()  # all configs are optional
-        configs.update(kwargs)
-        super().__init__(configs)
-        self.plot_settings = {}
-        self._extract_configs()
-
-    def _extract_configs(self):
-        self.plot_settings = dict()
-        self.plot_settings["heatmap_plot"] = self.configs.get(
-            "heatmap_plot_settings", {}
-        )
-        self.plot_settings["pairwise_plot"] = self.configs.get(
-            "similarity_plot_settings", {}
-        )
-        self.plot_settings["embedding_plot"] = {
-            "plot_color": 'red',
-            "plot_title": '2-D projected space',
-            "xlabel": "Dimension 1",
-            "ylabel": "Dimension 2",
-            "embedding": {"method": "mds",
-                          "params": {"random_state": 42, }
-                          },
-        }
-        self.plot_settings["embedding_plot"].update(self.configs.get(
-            "embedding_plot_settings",
-            {}))
-
-    def __call__(self, molecule_set):
-        """Visualize essential properties of the dataset.
-
-        Args:
-            molecule_set(AIMSim.chemical_datastructures MoleculeSet):
-                Molecular database.
-
-        Plots Generated
-        ---------------
-        1. Heatmap of Molecular Similarity.
-        2. PDF of the similarity distribution of the molecules in the database.
-
-        """
-        similarity_matrix = molecule_set.get_similarity_matrix()
-        if molecule_set.is_verbose:
-            print("Plotting similarity heatmap")
-        plot_heatmap(similarity_matrix, **self.plot_settings["heatmap_plot"])
-        if molecule_set.is_verbose:
-            print("Generating pairwise similarities")
-        pairwise_similarity_vector = molecule_set.get_pairwise_similarities()
-        if molecule_set.is_verbose:
-            print("Plotting density of pairwise similarities")
-        plot_density(
-            pairwise_similarity_vector,
-            **self.plot_settings["pairwise_plot"],
-        )
-
-        method_ = self.plot_settings["embedding_plot"]["embedding"]["method"]
-        reduced_features = molecule_set.get_transformed_descriptors(
-            method_=method_,
-            n_components=2,
-            **self.plot_settings["embedding_plot"]["embedding"].get("params", {}))
-        dimension_1 = reduced_features[:, 0]
-        dimension_2 = reduced_features[:, 1]
-
-        plot_scatter_interactive(
-            dimension_1,
-            dimension_2,
-            hover_names=molecule_set.get_mol_names(),
-            xlabel=self.plot_settings["embedding_plot"]["xlabel"],
-            ylabel=self.plot_settings["embedding_plot"]["ylabel"],
-            title=self.plot_settings["embedding_plot"]["plot_title"],
-            plot_color=self.plot_settings["embedding_plot"]["plot_color"],
-            offset=0,
-        )
-
-    def __str__(self):
-        return "Task: Visualize a dataset"
+"""Create similarity plots for the dataset."""
+import matplotlib.pyplot as plt
+
+from .task import Task
+from aimsim.utils.plotting_scripts import (
+    plot_density,
+    plot_heatmap,
+    plot_scatter,
+    plot_scatter_interactive,
+)
+
+
+class VisualizeDataset(Task):
+    def __init__(self, configs=None, **kwargs):
+        """
+        Constructor for the VisualizeDataset class.
+
+        Args:
+            configs(dict): Dictionary of configurations. Default is None.
+            **kwargs: Keyword arguments to modify configs fields.
+        Notes:
+            The configuration structure with default values are:
+            heatmap_plot_settings: {}  # pass through keywords for
+                                       # aimsim.utils.plotting_scripts.\
+                                       #  plot_heatmap
+            similarity_plot_settings: {}   # pass through keywords for
+                                           # aimsim.utils.plotting_scripts. \
+                                           #plot_density
+            embedding_plot_settings:
+                    {'plot_color': 'red'
+                     'plot_title': '2-D projected space',
+                     'xlabel': 'Dimension 1',
+                     'ylabel': 'Dimension 2',
+                     'embedding': {'method': "mds",
+                                    'params': {'random_state': 42}}}
+
+        """
+        if configs is None:
+            configs = dict()  # all configs are optional
+        configs.update(kwargs)
+        super().__init__(configs)
+        self.plot_settings = {}
+        self._extract_configs()
+
+    def _extract_configs(self):
+        self.plot_settings = dict()
+        self.plot_settings["heatmap_plot"] = self.configs.get(
+            "heatmap_plot_settings", {}
+        )
+        self.plot_settings["pairwise_plot"] = self.configs.get(
+            "similarity_plot_settings", {}
+        )
+        self.plot_settings["embedding_plot"] = {
+            "plot_color": 'red',
+            "plot_title": '2-D projected space',
+            "xlabel": "Dimension 1",
+            "ylabel": "Dimension 2",
+            "embedding": {"method": "mds",
+                          "params": {"random_state": 42, }
+                          },
+        }
+        self.plot_settings["embedding_plot"].update(self.configs.get(
+            "embedding_plot_settings",
+            {}))
+
+    def __call__(self, molecule_set):
+        """Visualize essential properties of the dataset.
+
+        Args:
+            molecule_set(AIMSim.chemical_datastructures MoleculeSet):
+                Molecular database.
+
+        Plots Generated
+        ---------------
+        1. Heatmap of Molecular Similarity.
+        2. PDF of the similarity distribution of the molecules in the database.
+
+        """
+        similarity_matrix = molecule_set.get_similarity_matrix()
+        if molecule_set.is_verbose:
+            print("Plotting similarity heatmap")
+        plot_heatmap(similarity_matrix, **self.plot_settings["heatmap_plot"])
+        if molecule_set.is_verbose:
+            print("Generating pairwise similarities")
+        pairwise_similarity_vector = molecule_set.get_pairwise_similarities()
+        if molecule_set.is_verbose:
+            print("Plotting density of pairwise similarities")
+        plot_density(
+            pairwise_similarity_vector,
+            **self.plot_settings["pairwise_plot"],
+        )
+
+        method_ = self.plot_settings["embedding_plot"]["embedding"]["method"]
+        reduced_features = molecule_set.get_transformed_descriptors(
+            method_=method_,
+            n_components=2,
+            **self.plot_settings["embedding_plot"]["embedding"].get("params", {}))
+        dimension_1 = reduced_features[:, 0]
+        dimension_2 = reduced_features[:, 1]
+
+        plot_scatter_interactive(
+            dimension_1,
+            dimension_2,
+            hover_names=molecule_set.get_mol_names(),
+            xlabel=self.plot_settings["embedding_plot"]["xlabel"],
+            ylabel=self.plot_settings["embedding_plot"]["ylabel"],
+            title=self.plot_settings["embedding_plot"]["plot_title"],
+            plot_color=self.plot_settings["embedding_plot"]["plot_color"],
+            offset=0,
+        )
+
+    def __str__(self):
+        return "Task: Visualize a dataset"
```

### Comparing `aimsim-2.0.2/aimsim/utils/ccbmlib_fingerprints.py` & `aimsim-2.0.3/aimsim/utils/ccbmlib_fingerprints.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-#   Copyright 2020 Martin Vogt, Antonio de la Vega de Leon
-#
-#  Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
-#  associated documentation files (the "Software"), to deal in the Software without restriction,
-#  including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
-#  and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do
-#  so, subject to the following conditions:
-#
-#  The above copyright notice and this permission notice shall be included in all copies or substantial
-#  portions of the Software.
-#
-#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
-#  INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-#  PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-#  COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
-#  AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-#  WITH  THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-# This file has been edited to include only the functions used in the molSim
-# repository in which it is now included by Jackson Burns (UDel). In compliance
-# with the license above, the code is included with the repository.
-from zlib import adler32
-
-
-from rdkit.Chem.rdMolDescriptors import GetMACCSKeysFingerprint
-from rdkit.Chem.rdMolDescriptors import GetAtomPairFingerprint
-from rdkit.Chem.rdMolDescriptors import GetTopologicalTorsionFingerprint
-from rdkit.Chem.rdMolDescriptors import GetMorganFingerprint
-from rdkit.Chem.rdMolDescriptors import GetHashedAtomPairFingerprint
-from rdkit.Chem.rdMolDescriptors import GetHashedTopologicalTorsionFingerprint
-from rdkit.Chem.rdMolDescriptors import GetHashedMorganFingerprint
-from rdkit.Avalon.pyAvalonTools import GetAvalonFP
-from rdkit.Chem import RDKFingerprint
-
-# Functions for calculating different fingerprints
-# All fingerprints are returned as lists of features
-
-
-def rdkit_fingerprint(mol, **kwargs):
-    return list(RDKFingerprint(mol, **kwargs).GetOnBits())
-
-
-def maccs_keys(mol, **kwargs):
-    return list(GetMACCSKeysFingerprint(mol).GetOnBits())
-
-
-def atom_pairs(mol, **kwargs):
-    return list(GetAtomPairFingerprint(mol, **kwargs).GetNonzeroElements())
-
-
-def torsions(mol, **kwargs):
-    return list(
-        GetTopologicalTorsionFingerprint(
-            mol,
-            **kwargs,
-        ).GetNonzeroElements()
-    )
-
-
-def morgan(mol, **kwargs):
-    return list(GetMorganFingerprint(mol, **kwargs).GetNonzeroElements())
-
-
-def hashed_atom_pairs(mol, **kwargs):
-    return list(
-        GetHashedAtomPairFingerprint(
-            mol,
-            **kwargs,
-        ).GetNonzeroElements()
-    )
-
-
-def hashed_torsions(mol, **kwargs):
-    return list(
-        GetHashedTopologicalTorsionFingerprint(
-            mol,
-            **kwargs,
-        ).GetNonzeroElements()
-    )
-
-
-def hashed_morgan(mol, **kwargs):
-    return list(
-        GetHashedMorganFingerprint(
-            mol,
-            **kwargs,
-        ).GetNonzeroElements()
-    )
-
-
-def avalon(mol, **kwargs):
-    return list(GetAvalonFP(mol, **kwargs).GetOnBits())
-
-
-def generate_fingerprints(mol_suppl, fp, **pars):
-    for mol in mol_suppl:
-        if mol:
-            yield fp(mol, **pars)
-
-
-def hash_parameter_set(pars):
-    s = sorted(pars.items())
-    return adler32(str(s).encode("UTF-8"))
-
-
-def to_key_val_string(pars):
-    return " ".join("{}:{}".format(k, v) for k, v in sorted(pars.items()))
-
-
-fingerprints = {
-    "rdkit": rdkit_fingerprint,
-    "maccs": maccs_keys,
-    "atom_pairs": atom_pairs,
-    "torsions": torsions,
-    "morgan": morgan,
-    "hashed_atom_pairs": hashed_atom_pairs,
-    "hashed_torsions": hashed_torsions,
-    "hashed_morgan": hashed_morgan,
-    "avalon": avalon,
-}
+#   Copyright 2020 Martin Vogt, Antonio de la Vega de Leon
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
+#  associated documentation files (the "Software"), to deal in the Software without restriction,
+#  including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
+#  and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do
+#  so, subject to the following conditions:
+#
+#  The above copyright notice and this permission notice shall be included in all copies or substantial
+#  portions of the Software.
+#
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
+#  INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+#  PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+#  COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
+#  AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+#  WITH  THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+# This file has been edited to include only the functions used in the molSim
+# repository in which it is now included by Jackson Burns (UDel). In compliance
+# with the license above, the code is included with the repository.
+from zlib import adler32
+
+
+from rdkit.Chem.rdMolDescriptors import GetMACCSKeysFingerprint
+from rdkit.Chem.rdMolDescriptors import GetAtomPairFingerprint
+from rdkit.Chem.rdMolDescriptors import GetTopologicalTorsionFingerprint
+from rdkit.Chem.rdMolDescriptors import GetMorganFingerprint
+from rdkit.Chem.rdMolDescriptors import GetHashedAtomPairFingerprint
+from rdkit.Chem.rdMolDescriptors import GetHashedTopologicalTorsionFingerprint
+from rdkit.Chem.rdMolDescriptors import GetHashedMorganFingerprint
+from rdkit.Avalon.pyAvalonTools import GetAvalonFP
+from rdkit.Chem import RDKFingerprint
+
+# Functions for calculating different fingerprints
+# All fingerprints are returned as lists of features
+
+
+def rdkit_fingerprint(mol, **kwargs):
+    return list(RDKFingerprint(mol, **kwargs).GetOnBits())
+
+
+def maccs_keys(mol, **kwargs):
+    return list(GetMACCSKeysFingerprint(mol).GetOnBits())
+
+
+def atom_pairs(mol, **kwargs):
+    return list(GetAtomPairFingerprint(mol, **kwargs).GetNonzeroElements())
+
+
+def torsions(mol, **kwargs):
+    return list(
+        GetTopologicalTorsionFingerprint(
+            mol,
+            **kwargs,
+        ).GetNonzeroElements()
+    )
+
+
+def morgan(mol, **kwargs):
+    return list(GetMorganFingerprint(mol, **kwargs).GetNonzeroElements())
+
+
+def hashed_atom_pairs(mol, **kwargs):
+    return list(
+        GetHashedAtomPairFingerprint(
+            mol,
+            **kwargs,
+        ).GetNonzeroElements()
+    )
+
+
+def hashed_torsions(mol, **kwargs):
+    return list(
+        GetHashedTopologicalTorsionFingerprint(
+            mol,
+            **kwargs,
+        ).GetNonzeroElements()
+    )
+
+
+def hashed_morgan(mol, **kwargs):
+    return list(
+        GetHashedMorganFingerprint(
+            mol,
+            **kwargs,
+        ).GetNonzeroElements()
+    )
+
+
+def avalon(mol, **kwargs):
+    return list(GetAvalonFP(mol, **kwargs).GetOnBits())
+
+
+def generate_fingerprints(mol_suppl, fp, **pars):
+    for mol in mol_suppl:
+        if mol:
+            yield fp(mol, **pars)
+
+
+def hash_parameter_set(pars):
+    s = sorted(pars.items())
+    return adler32(str(s).encode("UTF-8"))
+
+
+def to_key_val_string(pars):
+    return " ".join("{}:{}".format(k, v) for k, v in sorted(pars.items()))
+
+
+fingerprints = {
+    "rdkit": rdkit_fingerprint,
+    "maccs": maccs_keys,
+    "atom_pairs": atom_pairs,
+    "torsions": torsions,
+    "morgan": morgan,
+    "hashed_atom_pairs": hashed_atom_pairs,
+    "hashed_torsions": hashed_torsions,
+    "hashed_morgan": hashed_morgan,
+    "avalon": avalon,
+}
```

### Comparing `aimsim-2.0.2/aimsim/utils/extras.py` & `aimsim-2.0.3/aimsim/utils/extras.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from warnings import warn
-
-from aimsim.exceptions import MordredNotInstalledWarning
-
-
-def requires_mordred(function):
-    try:
-        from mordred import Calculator, descriptors
-
-        return function
-    except ImportError:
-        return MordredNotInstalledWarning(
-            """Attempting to call this function ({:s}) requires mordred to be installed.
-            Please use 'pip install aimsim[mordred]' in an environment with the appropriate version of Python.
-        """.format(
-                function.__name__
-            )
-        )
+from warnings import warn
+
+from aimsim.exceptions import MordredNotInstalledWarning
+
+
+def requires_mordred(function):
+    try:
+        from mordred import Calculator, descriptors
+
+        return function
+    except ImportError:
+        return MordredNotInstalledWarning(
+            """Attempting to call this function ({:s}) requires mordred to be installed.
+            Please use 'pip install aimsim[mordred]' in an environment with the appropriate version of Python.
+        """.format(
+                function.__name__
+            )
+        )
```

### Comparing `aimsim-2.0.2/aimsim/utils/plotting_scripts.py` & `aimsim-2.0.3/aimsim/utils/plotting_scripts.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,502 +1,502 @@
-"""Plotting functions"""
-import matplotlib.pyplot as plt
-import matplotlib.ticker as ticker
-import numpy as np
-import pandas as pd
-import plotly.express as px
-import plotly.graph_objects as go
-from seaborn import kdeplot, heatmap
-
-from aimsim.exceptions import InvalidConfigurationError
-
-
-def plot_density(densities, n_densities=1, legends=None, **kwargs):
-    """Plot the similarity density.
-
-    Args:
-        densities (list or numpy ndarray): Vector(s) of densities to plot.
-            Shape (n_densities, n_points_per_density). n_densities can be 1.
-        n_densities (int): Number of densities.
-        Pass this if passing more than one densities.
-        legends (list): Optional list of legends for annotating
-            different densities.
-
-    kwargs: dict
-        Keyword arguments to modify plot. Some common ones:
-        xlabel: str
-            Label of the x-axis. Default is "Samples"
-        ylabel: str
-            Label of the y-axis. Default is "Similarity Density"
-        xlabel_fontsize: int
-            Fontsize of the x-axis label. Default is 20.
-        ylabel_fontsize: int
-            Fontsize of the y-axis label. Default is 20.
-        plot_title: str
-            Plot title. Default is None.
-        plot_title_fontsize: int
-            Fontsize of the title. Default is 24.
-        color: str or list
-            Color of the plot. Multiple colors can be passed as list
-            if multiple densities are plotted.
-        shade: bool
-            To shade the plot or not.
-    """
-    plot_title = kwargs.pop("plot_title", None)
-    xlabel = kwargs.pop("xlabel", "Samples")
-    ylabel = kwargs.pop("ylabel", "Similarity Density")
-    plot_title_fontsize = kwargs.pop("plot_title_fontsize", 24)
-    xlabel_fontsize = int(kwargs.pop("xlabel_fontsize", 20))
-    ylabel_fontsize = int(kwargs.pop("ylabel_fontsize", 20))
-    legend_fontsize = int(kwargs.pop("legend_fontsize", 20))
-    color = kwargs.pop("plot_color", None)
-    shade = kwargs.pop("shade", False)
-
-    if n_densities == 1:
-        valid_number_types = (float, np.int64, int, float)
-        for density in densities:
-            is_number = isinstance(density, valid_number_types)
-            if not is_number:
-                raise InvalidConfigurationError(f'Element of type '
-                                                f'{type(density)} passed when '
-                                                f'expecting types '
-                                                f'{valid_number_types}')
-        # converting to 2D array for uniform processing
-        densities = [densities]
-    if color is None or isinstance(color, str):
-        color = [color] * n_densities
-    if legends is None:
-        legends = [None] * n_densities
-    if len(color) < n_densities:
-        raise InvalidConfigurationError(f'{len(color)} colors supplied '
-                                        f'for {n_densities} '
-                                        f'densities')
-    if len(legends) < n_densities:
-        raise InvalidConfigurationError(f'{len(legends)} colors supplied '
-                                        f'for {n_densities} '
-                                        f'densities')
-
-    plt.figure()
-    plt.rcParams["svg.fonttype"] = "none"
-    for density_id, density in enumerate(densities):
-        kdeplot(density,
-                color=color[density_id],
-                label=legends[density_id],
-                shade=shade,
-                **kwargs)
-    plt.xlabel(xlabel, fontsize=xlabel_fontsize)
-    plt.ylabel(ylabel, fontsize=ylabel_fontsize)
-    if not legends == [None] * n_densities:
-        plt.legend(fontsize=legend_fontsize)
-    if plot_title is not None:
-        plt.title(plot_title, fontsize=plot_title_fontsize)
-
-
-def plot_heatmap(input_matrix, **kwargs):
-    """Plot a heatmap representing the input matrix.
-
-    Args:
-        input_matrix (np.ndarray): Matrix to be plotted.
-
-    kwargs: dict
-        Keyword arguments to modify plot. Some common ones:
-        xlabel: str
-            Label of the x-axis. Default is "Samples"
-        ylabel: str
-            Label of the y-axis. Default is "Similarity Density"
-        xlabel_fontsize: int
-            Fontsize of the x-axis label. Default is 20.
-        ylabel_fontsize: int
-            Fontsize of the y-axis label. Default is 20.
-        plot_title: str
-            Plot title. Default is None.
-        plot_title_fontsize: int
-            Fontsize of the title. Default is 24.
-        color: str
-            Color of the plot.
-        shade: bool
-            To shade the plot or not.
-
-    """
-    parameters = {
-        "xticklabels": False,
-        "yticklabels": False,
-        "cmap": "autumn",
-        "mask_upper": False,
-        "annotate": False,
-        "plot_title": "",
-    }
-    parameters.update(**kwargs)
-    plt.figure()
-    plt.rcParams["svg.fonttype"] = "none"
-    mask = None
-    if parameters["mask_upper"] is True:
-        mask = np.triu(np.ones(shape=input_matrix.shape), k=0)
-    heatmap_obj = heatmap(
-        input_matrix,
-        xticklabels=parameters["xticklabels"],
-        yticklabels=parameters["yticklabels"],
-        cmap=parameters["cmap"],
-        mask=mask,
-        annot=parameters["annotate"],
-    )
-    plt.title(parameters["plot_title"], fontsize=24)
-
-
-def plot_parity(x, y, **kwargs):
-    """Plot parity plot of x vs y.
-
-    Args:
-        x (n x 1 np.ndarray): values plotted along x axis
-        y (n x 1 np.ndarray): values plotted along y axis
-
-    Returns:
-        if kwargs.show_plot set to False, returns pyplot axis.
-
-    """
-    plot_params = {
-        "alpha": 0.7,
-        "s": 100,
-        "plot_color": "green",
-    }
-    if kwargs is not None:
-        plot_params.update(kwargs)
-    plt.figure()
-    plt.rcParams["svg.fonttype"] = "none"
-    plt.scatter(
-        x=x,
-        y=y,
-        alpha=plot_params["alpha"],
-        s=plot_params["s"],
-        c=plot_params["plot_color"],
-    )
-    max_entry = max(max(x), max(y)) + plot_params.get("offset", 1.0)
-    min_entry = min(min(x), min(y)) - plot_params.get("offset", 1.0)
-    axes = plt.gca()
-    axes.set_xlim([min_entry, max_entry])
-    axes.set_ylim([min_entry, max_entry])
-    plt.plot(
-        [min_entry, max_entry],
-        [min_entry, max_entry],
-        color=plot_params.get("linecolor", "black"),
-    )
-    plt.title(
-        plot_params.get("title", ""),
-        fontsize=plot_params.get("title_fontsize", 24)
-    )
-    plt.xlabel(
-        plot_params.get("xlabel", ""),
-        fontsize=plot_params.get("xlabel_fontsize", 20)
-    )
-    plt.ylabel(
-        plot_params.get("ylabel", ""),
-        fontsize=plot_params.get("ylabel_fontsize", 20)
-    )
-    plt.xticks(fontsize=plot_params.get("xticksize", 24))
-    plt.yticks(fontsize=plot_params.get("yticksize", 24))
-    start, end = axes.get_xlim()
-    stepsize = (end - start) / 5
-    axes.xaxis.set_ticks(np.arange(start, end, stepsize))
-    axes.xaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
-    # set y tick stepsize
-    start, end = axes.get_ylim()
-    stepsize = (end - start) / 5
-    axes.yaxis.set_ticks(np.arange(start, end, stepsize))
-    axes.yaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
-    plt.text(
-        plot_params.pop("text_x", 0.05),
-        plot_params.pop("text_y", 0.9),
-        plot_params.pop("text", None),
-        transform=axes.transAxes,
-        fontsize=plot_params.pop("text_fontsize", 16),
-    )
-    if kwargs.get("show_plot", True):
-        pass
-    else:
-        return axes
-
-
-def plot_barchart(x, heights, colors, xtick_labels=None, **kwargs):
-    """Plot a bar chart
-
-    Args:
-        x (list or numpy array): X axis grid.
-        heights (list or numpy array): Height of the bars.
-        colors (list or str): Plot colors.
-        xtick_labels (list, optional): Labels to use for each bar. Default is
-            None in which case just the indices of the height are used.
-    """
-    plot_params = {
-        "title": kwargs.pop("title", ""),
-        "title_fontsize": kwargs.pop("title_fontsize", 24),
-        "xlabel": kwargs.pop("xlabel", ""),
-        "xlabel_fontsize": kwargs.pop("xlabel_fontsize", 20),
-        "ylabel": kwargs.pop("ylabel", ""),
-        "ylabel_fontsize": kwargs.pop("ylabel_fontsize", 20),
-        "xticksize": kwargs.pop("xticksize", 24),
-        "yticksize": kwargs.pop("yticksize", 24),
-    }
-    plt.figure()
-    plt.tight_layout()
-    plt.rcParams["svg.fonttype"] = "none"
-    if xtick_labels is None:
-        xtick_labels = [_ for _ in range(len(heights))]
-    plt.bar(x, height=heights, color=colors, tick_label=xtick_labels, **kwargs)
-    plt.title(plot_params["title"], fontsize=plot_params["title_fontsize"])
-    plt.xlabel(plot_params["xlabel"], fontsize=plot_params["xlabel_fontsize"])
-    plt.ylabel(plot_params["ylabel"], fontsize=plot_params["ylabel_fontsize"])
-    plt.xticks(fontsize=plot_params["xticksize"])
-    plt.yticks(fontsize=plot_params["yticksize"])
-
-
-def plot_multiple_barchart(x,
-                           heights,
-                           colors,
-                           legend_labels=None,
-                           xtick_labels=None,
-                           **kwargs):
-    """Plot a bar chart with multiplears per category.
-
-    Args:
-        x (list or numpy array): X axis grid.
-        heights (list or numpy array): Heights of the sets of bars.
-            Size of the array is (n_bars_per_xtick, n_xticks),
-        colors (list or str): Plot colors. If list supplied,
-            list[0] is used for first series, list[1] is used for
-            second series and list[2] is used for third series etc.
-        legend_labels (list or numpy array): Array of legend names for
-            each bar type. Size is (n_bars_per_xticks). Default is None.
-        xtick_labels (list, optional): Labels to use for each bar. Default is
-            None in which case just the indices of the heights are used.
-
-    Raises:
-        InvalidConfigurationError: If number of colors or legend labels
-        supplied is less than (or equal to, for legend_labels) n_bars
-        (per xtick).
-    """
-    plot_params = {
-        "title": kwargs.pop("title", ""),
-        "title_fontsize": kwargs.pop("title_fontsize", 24),
-        "xlabel": kwargs.pop("xlabel", ""),
-        "xlabel_fontsize": kwargs.pop("xlabel_fontsize", 20),
-        "ylabel": kwargs.pop("ylabel", ""),
-        "ylabel_fontsize": kwargs.pop("ylabel_fontsize", 20),
-        "xticksize": kwargs.pop("xticksize", 24),
-        "yticksize": kwargs.pop("yticksize", 24),
-    }
-    x = np.array(x)
-    heights = np.array(heights)
-    bar_width = kwargs.pop('bar_width', 0.2)
-    n_bars_per_xtick = heights.shape[0]
-    if isinstance(colors, str):
-        colors = [colors] * n_bars_per_xtick
-    if len(colors) < n_bars_per_xtick:
-        raise InvalidConfigurationError(f'{len(colors)} colors supplied '
-                                        f'insufficient for '
-                                        f'{n_bars_per_xtick} bars')
-    plt.figure()
-    plt.tight_layout()
-    plt.rcParams["svg.fonttype"] = "none"
-    if xtick_labels is None:
-        xtick_labels = x
-    bars = []
-    for bar_id in range(n_bars_per_xtick):
-        bars.append(plt.bar(x + bar_id*bar_width,
-                            heights[bar_id],
-                            bar_width,
-                            color=colors[bar_id],
-                            **kwargs))
-
-    plt.title(plot_params["title"], fontsize=plot_params["title_fontsize"])
-    plt.xlabel(plot_params["xlabel"], fontsize=plot_params["xlabel_fontsize"])
-    plt.ylabel(plot_params["ylabel"], fontsize=plot_params["ylabel_fontsize"])
-    plt.xticks(x + bar_width * ((n_bars_per_xtick-1)/2),
-               xtick_labels,
-               fontsize=plot_params["xticksize"])
-    plt.yticks(fontsize=plot_params["yticksize"])
-    if legend_labels is not None:
-        if len(legend_labels) != n_bars_per_xtick:
-            raise InvalidConfigurationError(f'{len(legend_labels)} legend '
-                                            f'labels not sufficient for '
-                                            f'{n_bars_per_xtick} bars')
-        plt.legend(bars, legend_labels)
-
-
-def plot_scatter(x, y, outlier_idxs=None, **kwargs):
-    """Plot scatter plot of x vs y.
-
-    Args:
-        x(np.ndarray or list): Values plotted along x axis.
-        y(np.ndarray or list): Values plotted along y axis.
-
-    Returns:
-        if kwargs.show_plot set to False, returns pyplot axis.
-
-    """
-    plot_params = {
-        "alpha": 0.7,
-        "s": 100,
-        "plot_color": "green",
-    }
-    if kwargs is not None:
-        plot_params.update(kwargs)
-    plt.figure()
-    plt.tight_layout()
-    plt.rcParams["svg.fonttype"] = "none"
-    plt.scatter(
-        x=x,
-        y=y,
-        alpha=plot_params["alpha"],
-        s=plot_params["s"],
-        c=plot_params["plot_color"],
-    )
-    if outlier_idxs is not None:
-        plt.scatter(
-            x=[x[i] for i in outlier_idxs],
-            y=[y[i] for i in outlier_idxs],
-            s=plot_params["s"],
-            c="r",
-        )
-    max_entry = max(max(x), max(y)) + plot_params.get("offset", 5.0)
-    min_entry = min(min(x), min(y)) - plot_params.get("offset", 5.0)
-    axes = plt.gca()
-    axes.set_xlim([min_entry, max_entry])
-    axes.set_ylim([min_entry, max_entry])
-    plt.title(
-        plot_params.get("title", ""), fontsize=plot_params.get("title_fontsize", 24)
-    )
-    plt.xlabel(
-        plot_params.get("xlabel", ""), fontsize=plot_params.get("xlabel_fontsize", 20)
-    )
-    plt.ylabel(
-        plot_params.get("ylabel", ""), fontsize=plot_params.get("ylabel_fontsize", 20)
-    )
-    plt.xticks(fontsize=plot_params.get("xticksize", 24))
-    plt.yticks(fontsize=plot_params.get("yticksize", 24))
-    start, end = axes.get_xlim()
-    stepsize = (end - start) / 5
-    axes.xaxis.set_ticks(np.arange(start, end, stepsize))
-    axes.xaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
-    # set y tick stepsize
-    start, end = axes.get_ylim()
-    stepsize = (end - start) / 5
-    axes.yaxis.set_ticks(np.arange(start, end, stepsize))
-    axes.yaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
-    if kwargs.get("show_plot", True):
-        pass
-    else:
-        return axes
-
-
-def plot_scatter_interactive(
-    x,
-    y,
-    hover_names=None,
-    outlier_idxs=None,
-    cluster_memberships=None,
-    **kwargs
-):
-    """Plot interactive scatter plot of x vs y.
-
-    Args:
-        x (np.ndarray or list): Values plotted along x axis.
-        y (np.ndarray or list): Values plotted along y axis.
-        hover_names (n x 1 np.ndarray): Names of points that will appear
-            when cursor is hovered around. Default is None in which case
-            the default is used.
-        outlier_idxs (list or np.ndarray): List of idx of points which
-            corresponds to outliers.
-        cluster_memberships (list or np.ndarray): List of cluster
-            memberships of all the points.
-            Should be the same shape as x or y.
-
-    """
-    opacity = kwargs.get('alpha', 0.7)
-    marker_size = kwargs.get('s', 20)
-    plot_color = kwargs.get('plot_color', 'green')
-    outlier_color = kwargs.get('outlier_color', 'red')
-    cluster_colors = kwargs.get('cluster_colors', None)
-    title = kwargs.get('title', None)
-    xlabel = kwargs.get('xlabel', 'Dimension 1')
-    ylabel = kwargs.get('ylabel', 'Dimension 2')
-
-    if cluster_memberships is not None:
-        df = pd.DataFrame({
-            'x': x,
-            'y': y,
-            'cluster_memberships': cluster_memberships,
-            'hover_names': hover_names
-        })
-        fig = go.Figure()
-        all_cluster_idx = np.unique(cluster_memberships)
-        if cluster_colors is None \
-                or len(cluster_colors) < len(all_cluster_idx):
-            cluster_colors = [None] * len(all_cluster_idx)
-
-        for idx, cluster_id in enumerate(all_cluster_idx):
-            cluster_df = df.loc[df['cluster_memberships'] == cluster_id]
-            fig.add_trace(go.Scatter(x=cluster_df['x'].values,
-                                     y=cluster_df['y'].values,
-                                     name=f'cluster {cluster_id}',
-                                     text=cluster_df['hover_names'].values,
-                                     mode='markers',
-                                     marker_size=marker_size,
-                                     marker_color=cluster_colors[idx],
-                                     opacity=opacity,
-                                     marker_symbol='circle',
-                                     marker_line_width=0))
-
-    else:
-        is_outlier = [0] * len(x)
-        if outlier_idxs is not None:
-            for id in outlier_idxs:
-                is_outlier[id] = 1
-        df = pd.DataFrame({
-            'x': x,
-            'y': y,
-            'is_outlier': is_outlier,
-            'hover_names': hover_names
-        })
-
-        fig = go.Figure()
-        non_outliers = df.loc[df['is_outlier'] == 0]
-        fig.add_trace(go.Scatter(x=non_outliers['x'].values,
-                                 y=non_outliers['y'].values,
-                                 name='molecule',
-                                 text=non_outliers['hover_names'].values,
-                                 mode='markers',
-                                 marker_size=marker_size,
-                                 opacity=opacity,
-                                 marker_color=plot_color,
-                                 marker_symbol='circle',
-                                 marker_line_width=0))
-        if outlier_idxs is not None:
-            outliers = df.loc[df['is_outlier'] == 1]
-            fig.add_trace(go.Scatter(x=outliers['x'].values,
-                                     y=outliers['y'].values,
-                                     name='outlier',
-                                     text=outliers['hover_names'].values,
-                                     mode='markers',
-                                     marker_size=marker_size,
-                                     opacity=opacity,
-                                     marker_color=outlier_color,
-                                     marker_symbol='x',
-                                     marker_line_width=int(marker_size/10),
-                                     marker_line_color='black'))
-    fig.update_layout(
-        xaxis_title=xlabel,
-        yaxis_title=ylabel,
-        font=dict(
-            family="Courier New, monospace",
-            size=40))
-
-    if title is not None:
-        fig.update_layout(title={'text': title,
-                                 'y': 0.9,
-                                 'x': 0.5,
-                                 'xanchor': 'center',
-                                 'yanchor': 'top',
-                                 'font_size': 40})
-
-    if hover_names is not None:
-        fig.update_traces(hovertemplate="<b>%{text}</b><br><br>")
-    fig.show()
+"""Plotting functions"""
+import matplotlib.pyplot as plt
+import matplotlib.ticker as ticker
+import numpy as np
+import pandas as pd
+import plotly.express as px
+import plotly.graph_objects as go
+from seaborn import kdeplot, heatmap
+
+from aimsim.exceptions import InvalidConfigurationError
+
+
+def plot_density(densities, n_densities=1, legends=None, **kwargs):
+    """Plot the similarity density.
+
+    Args:
+        densities (list or numpy ndarray): Vector(s) of densities to plot.
+            Shape (n_densities, n_points_per_density). n_densities can be 1.
+        n_densities (int): Number of densities.
+        Pass this if passing more than one densities.
+        legends (list): Optional list of legends for annotating
+            different densities.
+
+    kwargs: dict
+        Keyword arguments to modify plot. Some common ones:
+        xlabel: str
+            Label of the x-axis. Default is "Samples"
+        ylabel: str
+            Label of the y-axis. Default is "Similarity Density"
+        xlabel_fontsize: int
+            Fontsize of the x-axis label. Default is 20.
+        ylabel_fontsize: int
+            Fontsize of the y-axis label. Default is 20.
+        plot_title: str
+            Plot title. Default is None.
+        plot_title_fontsize: int
+            Fontsize of the title. Default is 24.
+        color: str or list
+            Color of the plot. Multiple colors can be passed as list
+            if multiple densities are plotted.
+        shade: bool
+            To shade the plot or not.
+    """
+    plot_title = kwargs.pop("plot_title", None)
+    xlabel = kwargs.pop("xlabel", "Samples")
+    ylabel = kwargs.pop("ylabel", "Similarity Density")
+    plot_title_fontsize = kwargs.pop("plot_title_fontsize", 24)
+    xlabel_fontsize = int(kwargs.pop("xlabel_fontsize", 20))
+    ylabel_fontsize = int(kwargs.pop("ylabel_fontsize", 20))
+    legend_fontsize = int(kwargs.pop("legend_fontsize", 20))
+    color = kwargs.pop("plot_color", None)
+    shade = kwargs.pop("shade", False)
+
+    if n_densities == 1:
+        valid_number_types = (float, np.int64, int, float)
+        for density in densities:
+            is_number = isinstance(density, valid_number_types)
+            if not is_number:
+                raise InvalidConfigurationError(f'Element of type '
+                                                f'{type(density)} passed when '
+                                                f'expecting types '
+                                                f'{valid_number_types}')
+        # converting to 2D array for uniform processing
+        densities = [densities]
+    if color is None or isinstance(color, str):
+        color = [color] * n_densities
+    if legends is None:
+        legends = [None] * n_densities
+    if len(color) < n_densities:
+        raise InvalidConfigurationError(f'{len(color)} colors supplied '
+                                        f'for {n_densities} '
+                                        f'densities')
+    if len(legends) < n_densities:
+        raise InvalidConfigurationError(f'{len(legends)} colors supplied '
+                                        f'for {n_densities} '
+                                        f'densities')
+
+    plt.figure()
+    plt.rcParams["svg.fonttype"] = "none"
+    for density_id, density in enumerate(densities):
+        kdeplot(density,
+                color=color[density_id],
+                label=legends[density_id],
+                shade=shade,
+                **kwargs)
+    plt.xlabel(xlabel, fontsize=xlabel_fontsize)
+    plt.ylabel(ylabel, fontsize=ylabel_fontsize)
+    if not legends == [None] * n_densities:
+        plt.legend(fontsize=legend_fontsize)
+    if plot_title is not None:
+        plt.title(plot_title, fontsize=plot_title_fontsize)
+
+
+def plot_heatmap(input_matrix, **kwargs):
+    """Plot a heatmap representing the input matrix.
+
+    Args:
+        input_matrix (np.ndarray): Matrix to be plotted.
+
+    kwargs: dict
+        Keyword arguments to modify plot. Some common ones:
+        xlabel: str
+            Label of the x-axis. Default is "Samples"
+        ylabel: str
+            Label of the y-axis. Default is "Similarity Density"
+        xlabel_fontsize: int
+            Fontsize of the x-axis label. Default is 20.
+        ylabel_fontsize: int
+            Fontsize of the y-axis label. Default is 20.
+        plot_title: str
+            Plot title. Default is None.
+        plot_title_fontsize: int
+            Fontsize of the title. Default is 24.
+        color: str
+            Color of the plot.
+        shade: bool
+            To shade the plot or not.
+
+    """
+    parameters = {
+        "xticklabels": False,
+        "yticklabels": False,
+        "cmap": "autumn",
+        "mask_upper": False,
+        "annotate": False,
+        "plot_title": "",
+    }
+    parameters.update(**kwargs)
+    plt.figure()
+    plt.rcParams["svg.fonttype"] = "none"
+    mask = None
+    if parameters["mask_upper"] is True:
+        mask = np.triu(np.ones(shape=input_matrix.shape), k=0)
+    heatmap_obj = heatmap(
+        input_matrix,
+        xticklabels=parameters["xticklabels"],
+        yticklabels=parameters["yticklabels"],
+        cmap=parameters["cmap"],
+        mask=mask,
+        annot=parameters["annotate"],
+    )
+    plt.title(parameters["plot_title"], fontsize=24)
+
+
+def plot_parity(x, y, **kwargs):
+    """Plot parity plot of x vs y.
+
+    Args:
+        x (n x 1 np.ndarray): values plotted along x axis
+        y (n x 1 np.ndarray): values plotted along y axis
+
+    Returns:
+        if kwargs.show_plot set to False, returns pyplot axis.
+
+    """
+    plot_params = {
+        "alpha": 0.7,
+        "s": 100,
+        "plot_color": "green",
+    }
+    if kwargs is not None:
+        plot_params.update(kwargs)
+    plt.figure()
+    plt.rcParams["svg.fonttype"] = "none"
+    plt.scatter(
+        x=x,
+        y=y,
+        alpha=plot_params["alpha"],
+        s=plot_params["s"],
+        c=plot_params["plot_color"],
+    )
+    max_entry = max(max(x), max(y)) + plot_params.get("offset", 1.0)
+    min_entry = min(min(x), min(y)) - plot_params.get("offset", 1.0)
+    axes = plt.gca()
+    axes.set_xlim([min_entry, max_entry])
+    axes.set_ylim([min_entry, max_entry])
+    plt.plot(
+        [min_entry, max_entry],
+        [min_entry, max_entry],
+        color=plot_params.get("linecolor", "black"),
+    )
+    plt.title(
+        plot_params.get("title", ""),
+        fontsize=plot_params.get("title_fontsize", 24)
+    )
+    plt.xlabel(
+        plot_params.get("xlabel", ""),
+        fontsize=plot_params.get("xlabel_fontsize", 20)
+    )
+    plt.ylabel(
+        plot_params.get("ylabel", ""),
+        fontsize=plot_params.get("ylabel_fontsize", 20)
+    )
+    plt.xticks(fontsize=plot_params.get("xticksize", 24))
+    plt.yticks(fontsize=plot_params.get("yticksize", 24))
+    start, end = axes.get_xlim()
+    stepsize = (end - start) / 5
+    axes.xaxis.set_ticks(np.arange(start, end, stepsize))
+    axes.xaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
+    # set y tick stepsize
+    start, end = axes.get_ylim()
+    stepsize = (end - start) / 5
+    axes.yaxis.set_ticks(np.arange(start, end, stepsize))
+    axes.yaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
+    plt.text(
+        plot_params.pop("text_x", 0.05),
+        plot_params.pop("text_y", 0.9),
+        plot_params.pop("text", None),
+        transform=axes.transAxes,
+        fontsize=plot_params.pop("text_fontsize", 16),
+    )
+    if kwargs.get("show_plot", True):
+        pass
+    else:
+        return axes
+
+
+def plot_barchart(x, heights, colors, xtick_labels=None, **kwargs):
+    """Plot a bar chart
+
+    Args:
+        x (list or numpy array): X axis grid.
+        heights (list or numpy array): Height of the bars.
+        colors (list or str): Plot colors.
+        xtick_labels (list, optional): Labels to use for each bar. Default is
+            None in which case just the indices of the height are used.
+    """
+    plot_params = {
+        "title": kwargs.pop("title", ""),
+        "title_fontsize": kwargs.pop("title_fontsize", 24),
+        "xlabel": kwargs.pop("xlabel", ""),
+        "xlabel_fontsize": kwargs.pop("xlabel_fontsize", 20),
+        "ylabel": kwargs.pop("ylabel", ""),
+        "ylabel_fontsize": kwargs.pop("ylabel_fontsize", 20),
+        "xticksize": kwargs.pop("xticksize", 24),
+        "yticksize": kwargs.pop("yticksize", 24),
+    }
+    plt.figure()
+    plt.tight_layout()
+    plt.rcParams["svg.fonttype"] = "none"
+    if xtick_labels is None:
+        xtick_labels = [_ for _ in range(len(heights))]
+    plt.bar(x, height=heights, color=colors, tick_label=xtick_labels, **kwargs)
+    plt.title(plot_params["title"], fontsize=plot_params["title_fontsize"])
+    plt.xlabel(plot_params["xlabel"], fontsize=plot_params["xlabel_fontsize"])
+    plt.ylabel(plot_params["ylabel"], fontsize=plot_params["ylabel_fontsize"])
+    plt.xticks(fontsize=plot_params["xticksize"])
+    plt.yticks(fontsize=plot_params["yticksize"])
+
+
+def plot_multiple_barchart(x,
+                           heights,
+                           colors,
+                           legend_labels=None,
+                           xtick_labels=None,
+                           **kwargs):
+    """Plot a bar chart with multiplears per category.
+
+    Args:
+        x (list or numpy array): X axis grid.
+        heights (list or numpy array): Heights of the sets of bars.
+            Size of the array is (n_bars_per_xtick, n_xticks),
+        colors (list or str): Plot colors. If list supplied,
+            list[0] is used for first series, list[1] is used for
+            second series and list[2] is used for third series etc.
+        legend_labels (list or numpy array): Array of legend names for
+            each bar type. Size is (n_bars_per_xticks). Default is None.
+        xtick_labels (list, optional): Labels to use for each bar. Default is
+            None in which case just the indices of the heights are used.
+
+    Raises:
+        InvalidConfigurationError: If number of colors or legend labels
+        supplied is less than (or equal to, for legend_labels) n_bars
+        (per xtick).
+    """
+    plot_params = {
+        "title": kwargs.pop("title", ""),
+        "title_fontsize": kwargs.pop("title_fontsize", 24),
+        "xlabel": kwargs.pop("xlabel", ""),
+        "xlabel_fontsize": kwargs.pop("xlabel_fontsize", 20),
+        "ylabel": kwargs.pop("ylabel", ""),
+        "ylabel_fontsize": kwargs.pop("ylabel_fontsize", 20),
+        "xticksize": kwargs.pop("xticksize", 24),
+        "yticksize": kwargs.pop("yticksize", 24),
+    }
+    x = np.array(x)
+    heights = np.array(heights)
+    bar_width = kwargs.pop('bar_width', 0.2)
+    n_bars_per_xtick = heights.shape[0]
+    if isinstance(colors, str):
+        colors = [colors] * n_bars_per_xtick
+    if len(colors) < n_bars_per_xtick:
+        raise InvalidConfigurationError(f'{len(colors)} colors supplied '
+                                        f'insufficient for '
+                                        f'{n_bars_per_xtick} bars')
+    plt.figure()
+    plt.tight_layout()
+    plt.rcParams["svg.fonttype"] = "none"
+    if xtick_labels is None:
+        xtick_labels = x
+    bars = []
+    for bar_id in range(n_bars_per_xtick):
+        bars.append(plt.bar(x + bar_id*bar_width,
+                            heights[bar_id],
+                            bar_width,
+                            color=colors[bar_id],
+                            **kwargs))
+
+    plt.title(plot_params["title"], fontsize=plot_params["title_fontsize"])
+    plt.xlabel(plot_params["xlabel"], fontsize=plot_params["xlabel_fontsize"])
+    plt.ylabel(plot_params["ylabel"], fontsize=plot_params["ylabel_fontsize"])
+    plt.xticks(x + bar_width * ((n_bars_per_xtick-1)/2),
+               xtick_labels,
+               fontsize=plot_params["xticksize"])
+    plt.yticks(fontsize=plot_params["yticksize"])
+    if legend_labels is not None:
+        if len(legend_labels) != n_bars_per_xtick:
+            raise InvalidConfigurationError(f'{len(legend_labels)} legend '
+                                            f'labels not sufficient for '
+                                            f'{n_bars_per_xtick} bars')
+        plt.legend(bars, legend_labels)
+
+
+def plot_scatter(x, y, outlier_idxs=None, **kwargs):
+    """Plot scatter plot of x vs y.
+
+    Args:
+        x(np.ndarray or list): Values plotted along x axis.
+        y(np.ndarray or list): Values plotted along y axis.
+
+    Returns:
+        if kwargs.show_plot set to False, returns pyplot axis.
+
+    """
+    plot_params = {
+        "alpha": 0.7,
+        "s": 100,
+        "plot_color": "green",
+    }
+    if kwargs is not None:
+        plot_params.update(kwargs)
+    plt.figure()
+    plt.tight_layout()
+    plt.rcParams["svg.fonttype"] = "none"
+    plt.scatter(
+        x=x,
+        y=y,
+        alpha=plot_params["alpha"],
+        s=plot_params["s"],
+        c=plot_params["plot_color"],
+    )
+    if outlier_idxs is not None:
+        plt.scatter(
+            x=[x[i] for i in outlier_idxs],
+            y=[y[i] for i in outlier_idxs],
+            s=plot_params["s"],
+            c="r",
+        )
+    max_entry = max(max(x), max(y)) + plot_params.get("offset", 5.0)
+    min_entry = min(min(x), min(y)) - plot_params.get("offset", 5.0)
+    axes = plt.gca()
+    axes.set_xlim([min_entry, max_entry])
+    axes.set_ylim([min_entry, max_entry])
+    plt.title(
+        plot_params.get("title", ""), fontsize=plot_params.get("title_fontsize", 24)
+    )
+    plt.xlabel(
+        plot_params.get("xlabel", ""), fontsize=plot_params.get("xlabel_fontsize", 20)
+    )
+    plt.ylabel(
+        plot_params.get("ylabel", ""), fontsize=plot_params.get("ylabel_fontsize", 20)
+    )
+    plt.xticks(fontsize=plot_params.get("xticksize", 24))
+    plt.yticks(fontsize=plot_params.get("yticksize", 24))
+    start, end = axes.get_xlim()
+    stepsize = (end - start) / 5
+    axes.xaxis.set_ticks(np.arange(start, end, stepsize))
+    axes.xaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
+    # set y tick stepsize
+    start, end = axes.get_ylim()
+    stepsize = (end - start) / 5
+    axes.yaxis.set_ticks(np.arange(start, end, stepsize))
+    axes.yaxis.set_major_formatter(ticker.FormatStrFormatter("%0.1f"))
+    if kwargs.get("show_plot", True):
+        pass
+    else:
+        return axes
+
+
+def plot_scatter_interactive(
+    x,
+    y,
+    hover_names=None,
+    outlier_idxs=None,
+    cluster_memberships=None,
+    **kwargs
+):
+    """Plot interactive scatter plot of x vs y.
+
+    Args:
+        x (np.ndarray or list): Values plotted along x axis.
+        y (np.ndarray or list): Values plotted along y axis.
+        hover_names (n x 1 np.ndarray): Names of points that will appear
+            when cursor is hovered around. Default is None in which case
+            the default is used.
+        outlier_idxs (list or np.ndarray): List of idx of points which
+            corresponds to outliers.
+        cluster_memberships (list or np.ndarray): List of cluster
+            memberships of all the points.
+            Should be the same shape as x or y.
+
+    """
+    opacity = kwargs.get('alpha', 0.7)
+    marker_size = kwargs.get('s', 20)
+    plot_color = kwargs.get('plot_color', 'green')
+    outlier_color = kwargs.get('outlier_color', 'red')
+    cluster_colors = kwargs.get('cluster_colors', None)
+    title = kwargs.get('title', None)
+    xlabel = kwargs.get('xlabel', 'Dimension 1')
+    ylabel = kwargs.get('ylabel', 'Dimension 2')
+
+    if cluster_memberships is not None:
+        df = pd.DataFrame({
+            'x': x,
+            'y': y,
+            'cluster_memberships': cluster_memberships,
+            'hover_names': hover_names
+        })
+        fig = go.Figure()
+        all_cluster_idx = np.unique(cluster_memberships)
+        if cluster_colors is None \
+                or len(cluster_colors) < len(all_cluster_idx):
+            cluster_colors = [None] * len(all_cluster_idx)
+
+        for idx, cluster_id in enumerate(all_cluster_idx):
+            cluster_df = df.loc[df['cluster_memberships'] == cluster_id]
+            fig.add_trace(go.Scatter(x=cluster_df['x'].values,
+                                     y=cluster_df['y'].values,
+                                     name=f'cluster {cluster_id}',
+                                     text=cluster_df['hover_names'].values,
+                                     mode='markers',
+                                     marker_size=marker_size,
+                                     marker_color=cluster_colors[idx],
+                                     opacity=opacity,
+                                     marker_symbol='circle',
+                                     marker_line_width=0))
+
+    else:
+        is_outlier = [0] * len(x)
+        if outlier_idxs is not None:
+            for id in outlier_idxs:
+                is_outlier[id] = 1
+        df = pd.DataFrame({
+            'x': x,
+            'y': y,
+            'is_outlier': is_outlier,
+            'hover_names': hover_names
+        })
+
+        fig = go.Figure()
+        non_outliers = df.loc[df['is_outlier'] == 0]
+        fig.add_trace(go.Scatter(x=non_outliers['x'].values,
+                                 y=non_outliers['y'].values,
+                                 name='molecule',
+                                 text=non_outliers['hover_names'].values,
+                                 mode='markers',
+                                 marker_size=marker_size,
+                                 opacity=opacity,
+                                 marker_color=plot_color,
+                                 marker_symbol='circle',
+                                 marker_line_width=0))
+        if outlier_idxs is not None:
+            outliers = df.loc[df['is_outlier'] == 1]
+            fig.add_trace(go.Scatter(x=outliers['x'].values,
+                                     y=outliers['y'].values,
+                                     name='outlier',
+                                     text=outliers['hover_names'].values,
+                                     mode='markers',
+                                     marker_size=marker_size,
+                                     opacity=opacity,
+                                     marker_color=outlier_color,
+                                     marker_symbol='x',
+                                     marker_line_width=int(marker_size/10),
+                                     marker_line_color='black'))
+    fig.update_layout(
+        xaxis_title=xlabel,
+        yaxis_title=ylabel,
+        font=dict(
+            family="Courier New, monospace",
+            size=40))
+
+    if title is not None:
+        fig.update_layout(title={'text': title,
+                                 'y': 0.9,
+                                 'x': 0.5,
+                                 'xanchor': 'center',
+                                 'yanchor': 'top',
+                                 'font_size': 40})
+
+    if hover_names is not None:
+        fig.update_traces(hovertemplate="<b>%{text}</b><br><br>")
+    fig.show()
```

### Comparing `aimsim-2.0.2/aimsim.egg-info/PKG-INFO` & `aimsim-2.0.3/aimsim.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,200 +1,201 @@
-Metadata-Version: 2.1
-Name: aimsim
-Version: 2.0.2
-Summary: Python command line and GUI tool to analyze molecular similarity.
-Home-page: https://github.com/VlachosGroup/AIMSim
-Author: Himaghna Bhattacharjee, Jackson Burns
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: mordred
-License-File: LICENSE
-
-<h1 align="center">AIMSim README</h1> 
-<h3 align="center">Visualizing Diversity in your Molecular Dataset</h3>
-
-![AIMSim Logo](interfaces/UI/AIMSim-logo.png)
-<p align="center">
-  <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/VlachosGroup/AIMSim?style=social">
-  <img alt="Total Downloads" src="https://static.pepy.tech/personalized-badge/aimsim?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/aimsim">
-  <img alt="commits since" src="https://img.shields.io/github/commits-since/VlachosGroup/AIMSim/latest.svg">
-  <img alt="PyPI" src="https://img.shields.io/pypi/v/aimsim">
-  <img alt="PyPI - License" src="https://img.shields.io/github/license/VlachosGroup/AIMSim">
-  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/run_tests.yml/badge.svg?branch=master&event=schedule">
-</p>
-
-## Documentation and Tutorial
-[View our Online Documentation](https://vlachosgroup.github.io/AIMSim/) or try the [_AIMSim_ comprehensive tutorial in your browser](https://mybinder.org/v2/gh/VlachosGroup/AIMSim/master?labpath=AIMSim-demo.ipynb).
-
-## Purpose
-
-__Why Do We Need To Visualize Molecular Similarity / Diversity?__
-
-There are several contexts where it is helpful to visualize the diversity of a molecular dataset:
-
-_Exploratory Experimental Synthesis_
-
-For a chemist, synthesizing new molecules with targeted properties is often a laborious and time consuming task.
-In such a case, it becomes useful to check the similarity of a newly proposed (un-synthesized) molecule to the ones already synthesized.
-If the proposed molecule is too similar to the existing repertoire of molecules, it will probably not yield not enough new information /
-property and thus need not be synthesized. Thus, a chemist can avoid spending
-time and effort synthesizing molecules not useful for the project.
-
-_Lead Optimization and Virtual Screening_
-
-This application is the converse of exploratory synthesis where the interest is to find molecules in a database which are structurally similar to an "active" molecule. In this context, "active" might refer to pharmocological activity (drug discover campaigns) or desirable chemical properties (for example, to discover alternative chemicals and solvents for an application). In such a case, AIMSim helps to run virtual screenings over a molecular database and visualize the results.
-
-_Machine Learning Molecular Properties_
-
-In the context of machine learning, visualizing the diversity of the training set gives a good idea about its information quality.
-A more diverse training data-set yields a more robust model, which generalizes well to unseen data. Additionally, such a visualization can 
-identify "clusters of similarity" indicating the need for separately trained models for each cluster.
-
-_Substrate Scope Robustness Verification_
-
-When proposing a novel reaction it is essential for the practicing chemist to evaluate the transformation's tolerance of diverse functional groups and substrates (Glorius, 2013). Using `AIMSim`, one can evaluate the structural and chemical similarity across an entire susbtrate scope to ensure that it avoids redundant species. Below is an example similarity heatmap generated to visualize the diversity of a three-component sulfonamide coupling reaction with a substantial number of substrates (Chen, 2018).
-![Image of sulfonamide substrate scope](tests/sulfonamide-substrate-scope.png)
-
-Many of the substrates appear similar to one another and thereby redundant, but in reality the core sulfone moiety and the use of the same coupling partner when evaluating functional group tolerance accounts for this apparent shortcoming. Also of note is the region of high similarity along the diagonal where the substrates often differ by a single halide heteratom or substitution pattern.
-
-## Installing AIMSim
-`AIMSim` can be installed with a single command:
-`pip install aimsim`
-This command also installs the required dependencies. It is recommended to install `AIMSim` in a separate virtual environment.
-
-_Optional:_ Previous versions of AIMSim provided direct support for the descriptors provided in the `mordred` package. Unforunately, `mordred` is no longer recieving updates and causes significant depdendency conflicts. Because of this, it is an _optional_ add-on to `AIMSim` that is only compatible with Python 3.8. To install with `mordred` support, use `pip install 'aimsim[mordred]'` (note the single quotes, necessary in `zsh`).
-
-Unit tests from previous versions of `AIMSim` have been kept but are not actively maintained due to the limitations above. Use `mordred` at your own risk.
-
-## Running AIMSim
-`AIMSim` is compatible with Python 3.7 to 3.9.
-Start `AIMSim` with a graphical user interface:
-
-`aimsim`
-
-Start `AIMSim` with a prepared configuration YAML file (`config.yaml`):
-
-`aimsim config.yaml`
-
-### Currently Implemented Fingerprints
-
-1. Morgan Fingerprint (Equivalent to the ECFP fingerprints)
-2. RDKit Topological Fingerprint
-3. RDKit Daylight Fingerprint
-
-_The following are available via command line use (config.yaml) only:_
-
-4. All fingerprints available from the [ccbmlib](https://github.com/vogt-m/ccbmlib) package (_specify 'ccbmlib:descriptorname' for command line input_).
-5. All descriptors and fingerprints available from [PaDELPy](https://github.com/ecrl/padelpy), an interface to PaDEL-Descriptor. (_specify 'padelpy:desciptorname' for command line input._).
-6. All descriptors available through the [Mordred](https://github.com/mordred-descriptor/mordred) library (_specify 'mordred:desciptorname' for command line input._). To enable this option, you must install with `pip install 'aimsim[mordred]'` (see disclaimer in the Installation section above).
-
-### Currently Implemented Similarity Scores
-
-44 commonly used similarity scores are implemented in AIMSim.
-Additional L0, L1 and L2 norm based similarities are also implemented. [View our Online Documentation](https://vlachosgroup.github.io/AIMSim/implemented_metrics.html) for a complete list of implemented similarity scores.
-
-
-### Currently Implemented Functionalities
-
-1. Measure Search: Automate the search of fingerprint and similarity metric (called a "measure") using the following algorithm:
-  Step 1: Select an arbitrary featurization scheme.
-  Step 2: Featurize the molecule set using the selected scheme.
-  Step 3: Choose an arbitrary similarity measure.
-  Step 4: Select each moleculeâ€™s nearest and furthest neighbors in the set using the similarity measure.
-  Step 5: Measure the correlation between a moleculeâ€™s QoI and its nearest neighborâ€™s QoI.
-  Step 6: Measure the correlation between a moleculeâ€™s QoI and its further neighborâ€™s QoI.
-  Step 7: Define a score which maximizes the value in Step 5 and minimizes the value in Step 6.
-  Step 8: Iterate Steps 1 â€“ 7 to select the featurization scheme and similarity measure to maximize the result of Step 7. 
-2. See Property Variation with Similarity: Visualize the correlation in the QoI between nearest neighbor molecules (most similar pairs in the molecule set) and between the furthest neighbor molecules (most dissimilar pairs in the molecule set). This is used to verify that the chosen measure is appropriate for the task.
-
-3. Visualize Dataset: Visualize the diversity of the molecule set in the form of a pairwise similarity density and a similarity heatmap of the molecule set. Embed the molecule set in 2D space using using principal component analysis (PCA)[3], multi-dimensional scaling[4], t-SNE[5], Spectral Embedding[6], or Isomap[7].
-
-4. Compare Target Molecule to Molecule Set: Run a similarity search of a molecule against a database of molecules (molecule set). This task can be used to identify the most similar (useful in virtual screening operations) or most dissimilar (useful in application that require high diversity such as training set design for machine learning models) molecules.
-
-5. Cluster Data: Cluster the molecule set. The following algorithms are implemented: 
-
-For arbitrary molecular features or similarity metrics with defined Euclidean distances: K-Medoids[3] and Ward[8] (hierarchical clustering).
-
-For binary fingerprints: Complete, single and average linkage hierarchical clustering[8].
-
-The clustered data is plotted in two dimensions using principal component analysis (PCA)[3], multi-dimensional scaling[4], or TSNE[5].
-
-6. Outlier Detection: Using an isolation forest, check for which molecules are potentially novel or are outliers according to the selected descriptor. Output can be directly to the command line by specifiying `output` to be `terminal` or to a text file by instead providing a filename.
-
-## Contributors
-
-Developer: Himaghna Bhattacharjee, Vlachos Research Lab. ([LinkedIn](www.linkedin.com/in/himaghna-bhattacharjee))
-
-Developer: Jackson Burns, Don Watson Lab. ([Personal Site](https://www.jacksonwarnerburns.com/))
-
-## Developer Notes
-Issues and Pull Requests are welcomed! To propose an addition to `AIMSim` open an issue and the developers will tag it as an _enhancement_ and start discussion.
-
-`AIMSim` includes an automated testing apparatus operated by Python's _unittest_ built-in package. To execute tests related to the core functionality of `AIMSim`, run this command:
-
-`python -m unittest discover`
-
-Full multiprocessing speedup and efficiency tests take more than 10 hours to run due to the number of replicates required. To run these tests, create a file called `.speedup-test` in the `AIMSim` directory and execute the above command as shown.
-
-To manually build the docs, execute the following with `sphinx` and `m2r` installed and from the `/docs` directory:
-
-`m2r ../README.md | mv ../README.rst . | sphinx-apidoc -f -o . .. | make html | cp _build/html/* .`
-
-Documentation should manually build on push to master branch via an automated GitHub action.
-
-For packaging on PyPI:
-
-`python -m build; twine upload dist/*`
-
-Be sure to bump the version in `__init__.py`.
-
-## Citation
-If you use this code for scientific publications, please cite the following paper.
-
-Bhattacharjee, H.Ò‚; Burns, J.Ò‚; Vlachos, D.G. (2021): AIMSim: An Accessible Cheminformatics Platform for Similarity Operations on Chemicals Datasets. ChemRxiv. Preprint. https://doi.org/10.26434/chemrxiv-2022-nw6f5
-
-## License
-This code is made available under the terms of the _MIT Open License_:
-
-Copyright (c) 2020 Himaghna Bhattacharjee & Jackson Burns
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
-
-
-## Works Cited
-[1] Collins, K. and Glorius, F., A robustness screen for the rapid assessment of chemical reactions. Nature Chem 5, 597â€“601 (2013). https://doi.org/10.1038/nchem.1669
-
-[2] Chen, Y., Murray, P.R.D., Davies, A.T., and Willis M.C., J. Am. Chem. Soc. 140 (28), 8781-8787 (2018). https://doi.org/10.1021/jacs.8b04532
-
-[3] Hastie, T., Tibshirani R. and Friedman J., The Elements of statistical Learning: Data Mining, Inference, and Prediction, 2nd Ed., Springer Series in Statistics (2009).
-
-[4] Borg, I. and Groenen, P.J.F., Modern Multidimensional Scaling: Theory and Applications, Springer Series in Statistics (2005).
-
-[5] van der Maaten, L.J.P. and Hinton, G.E., Visualizing High-Dimensional Data Using t-SNE. Journal of Machine Learning Research 9:2579-2605 (2008).
-
-[6] Ng, A.Y., Jordan, M.I. and Weiss, Y., On Spectral Clustering: Analysis and an algorithm. ADVANCES IN NEURAL INFORMATION PROCESSING SYSTEMS, MIT Press (2001).
-
-[7] Tenenbaum, J.B., De Silva, V. and Langford, J.C, A global geometric framework for nonlinear dimensionality reduction, Science 290 (5500), 2319-23 (2000). https://doi.org/10.1126/science.290.5500.2319.
-
-[8] Murtagh, F. and Contreras, P., Algorithms for hierarchical clustering: an overview. WIREs Data Mining Knowl Discov (2011). https://doi.org/10.1002/widm.53
-
-
-
+Metadata-Version: 2.1
+Name: aimsim
+Version: 2.0.3
+Summary: Python command line and GUI tool to analyze molecular similarity.
+Home-page: https://github.com/VlachosGroup/AIMSim
+Author: Himaghna Bhattacharjee, Jackson Burns
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: mordred
+License-File: LICENSE
+
+<h1 align="center">AIMSim README</h1> 
+<h3 align="center">Visualizing Diversity in your Molecular Dataset</h3>
+
+![AIMSim Logo](interfaces/UI/AIMSim-logo.png)
+<p align="center">
+  <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/VlachosGroup/AIMSim?style=social">
+  <img alt="Total Downloads" src="https://static.pepy.tech/personalized-badge/aimsim?period=total&units=none&left_color=grey&right_color=blue&left_text=Lifetime%20Downloads">
+  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/aimsim">
+  <img alt="commits since" src="https://img.shields.io/github/commits-since/VlachosGroup/AIMSim/latest.svg">
+  <img alt="PyPI" src="https://img.shields.io/pypi/v/aimsim">
+  <img alt="PyPI - License" src="https://img.shields.io/github/license/VlachosGroup/AIMSim">
+  <img alt="Test Status" src="https://github.com/VlachosGroup/AIMSim/actions/workflows/run_tests.yml/badge.svg?branch=master&event=schedule">
+</p>
+
+## Documentation and Tutorial
+[View our Online Documentation](https://vlachosgroup.github.io/AIMSim/) or try the [_AIMSim_ comprehensive tutorial in your browser](https://mybinder.org/v2/gh/VlachosGroup/AIMSim/master?labpath=AIMSim-demo.ipynb).
+
+## Purpose
+
+__Why Do We Need To Visualize Molecular Similarity / Diversity?__
+
+There are several contexts where it is helpful to visualize the diversity of a molecular dataset:
+
+_Exploratory Experimental Synthesis_
+
+For a chemist, synthesizing new molecules with targeted properties is often a laborious and time consuming task.
+In such a case, it becomes useful to check the similarity of a newly proposed (un-synthesized) molecule to the ones already synthesized.
+If the proposed molecule is too similar to the existing repertoire of molecules, it will probably not yield not enough new information /
+property and thus need not be synthesized. Thus, a chemist can avoid spending
+time and effort synthesizing molecules not useful for the project.
+
+_Lead Optimization and Virtual Screening_
+
+This application is the converse of exploratory synthesis where the interest is to find molecules in a database which are structurally similar to an "active" molecule. In this context, "active" might refer to pharmocological activity (drug discover campaigns) or desirable chemical properties (for example, to discover alternative chemicals and solvents for an application). In such a case, AIMSim helps to run virtual screenings over a molecular database and visualize the results.
+
+_Machine Learning Molecular Properties_
+
+In the context of machine learning, visualizing the diversity of the training set gives a good idea about its information quality.
+A more diverse training data-set yields a more robust model, which generalizes well to unseen data. Additionally, such a visualization can 
+identify "clusters of similarity" indicating the need for separately trained models for each cluster.
+
+_Substrate Scope Robustness Verification_
+
+When proposing a novel reaction it is essential for the practicing chemist to evaluate the transformation's tolerance of diverse functional groups and substrates (Glorius, 2013). Using `AIMSim`, one can evaluate the structural and chemical similarity across an entire susbtrate scope to ensure that it avoids redundant species. Below is an example similarity heatmap generated to visualize the diversity of a three-component sulfonamide coupling reaction with a substantial number of substrates (Chen, 2018).
+![Image of sulfonamide substrate scope](tests/sulfonamide-substrate-scope.png)
+
+Many of the substrates appear similar to one another and thereby redundant, but in reality the core sulfone moiety and the use of the same coupling partner when evaluating functional group tolerance accounts for this apparent shortcoming. Also of note is the region of high similarity along the diagonal where the substrates often differ by a single halide heteratom or substitution pattern.
+
+## Installing AIMSim
+`AIMSim` can be installed with a single command:
+`pip install aimsim`
+This command also installs the required dependencies. It is recommended to install `AIMSim` in a separate virtual environment.
+
+_Optional:_ Previous versions of AIMSim provided direct support for the descriptors provided in the `mordred` package. Unforunately, `mordred` is no longer recieving updates and causes significant depdendency conflicts. Because of this, it is an _optional_ add-on to `AIMSim` that is only compatible with Python 3.8. To install with `mordred` support, use `pip install 'aimsim[mordred]'` (note the single quotes, necessary in `zsh`).
+
+Unit tests from previous versions of `AIMSim` have been kept but are not actively maintained due to the limitations above. Use `mordred` at your own risk.
+
+## Running AIMSim
+`AIMSim` is compatible with Python 3.7 to 3.9.
+Start `AIMSim` with a graphical user interface:
+
+`aimsim`
+
+Start `AIMSim` with a prepared configuration YAML file (`config.yaml`):
+
+`aimsim config.yaml`
+
+### Currently Implemented Fingerprints
+
+1. Morgan Fingerprint (Equivalent to the ECFP fingerprints)
+2. RDKit Topological Fingerprint
+3. RDKit Daylight Fingerprint
+
+_The following are available via command line use (config.yaml) only:_
+
+4. MinHash Fingerprint (see [MHFP](https://github.com/reymond-group/mhfp))
+5. All fingerprints available from the [ccbmlib](https://github.com/vogt-m/ccbmlib) package (_specify 'ccbmlib:descriptorname' for command line input_).
+6. All descriptors and fingerprints available from [PaDELPy](https://github.com/ecrl/padelpy), an interface to PaDEL-Descriptor. (_specify 'padelpy:desciptorname' for command line input._).
+7. All descriptors available through the [Mordred](https://github.com/mordred-descriptor/mordred) library (_specify 'mordred:desciptorname' for command line input._). To enable this option, you must install with `pip install 'aimsim[mordred]'` (see disclaimer in the Installation section above).
+
+### Currently Implemented Similarity Scores
+
+44 commonly used similarity scores are implemented in AIMSim.
+Additional L0, L1 and L2 norm based similarities are also implemented. [View our Online Documentation](https://vlachosgroup.github.io/AIMSim/implemented_metrics.html) for a complete list of implemented similarity scores.
+
+
+### Currently Implemented Functionalities
+
+1. Measure Search: Automate the search of fingerprint and similarity metric (called a "measure") using the following algorithm:
+  Step 1: Select an arbitrary featurization scheme.
+  Step 2: Featurize the molecule set using the selected scheme.
+  Step 3: Choose an arbitrary similarity measure.
+  Step 4: Select each molecule’s nearest and furthest neighbors in the set using the similarity measure.
+  Step 5: Measure the correlation between a molecule’s QoI and its nearest neighbor’s QoI.
+  Step 6: Measure the correlation between a molecule’s QoI and its further neighbor’s QoI.
+  Step 7: Define a score which maximizes the value in Step 5 and minimizes the value in Step 6.
+  Step 8: Iterate Steps 1 – 7 to select the featurization scheme and similarity measure to maximize the result of Step 7. 
+2. See Property Variation with Similarity: Visualize the correlation in the QoI between nearest neighbor molecules (most similar pairs in the molecule set) and between the furthest neighbor molecules (most dissimilar pairs in the molecule set). This is used to verify that the chosen measure is appropriate for the task.
+
+3. Visualize Dataset: Visualize the diversity of the molecule set in the form of a pairwise similarity density and a similarity heatmap of the molecule set. Embed the molecule set in 2D space using using principal component analysis (PCA)[3], multi-dimensional scaling[4], t-SNE[5], Spectral Embedding[6], or Isomap[7].
+
+4. Compare Target Molecule to Molecule Set: Run a similarity search of a molecule against a database of molecules (molecule set). This task can be used to identify the most similar (useful in virtual screening operations) or most dissimilar (useful in application that require high diversity such as training set design for machine learning models) molecules.
+
+5. Cluster Data: Cluster the molecule set. The following algorithms are implemented: 
+
+For arbitrary molecular features or similarity metrics with defined Euclidean distances: K-Medoids[3] and Ward[8] (hierarchical clustering).
+
+For binary fingerprints: Complete, single and average linkage hierarchical clustering[8].
+
+The clustered data is plotted in two dimensions using principal component analysis (PCA)[3], multi-dimensional scaling[4], or TSNE[5].
+
+6. Outlier Detection: Using an isolation forest, check for which molecules are potentially novel or are outliers according to the selected descriptor. Output can be directly to the command line by specifiying `output` to be `terminal` or to a text file by instead providing a filename.
+
+## Contributors
+
+Developer: Himaghna Bhattacharjee, Vlachos Research Lab. ([LinkedIn](www.linkedin.com/in/himaghna-bhattacharjee))
+
+Developer: Jackson Burns, Don Watson Lab. ([Personal Site](https://www.jacksonwarnerburns.com/))
+
+## Developer Notes
+Issues and Pull Requests are welcomed! To propose an addition to `AIMSim` open an issue and the developers will tag it as an _enhancement_ and start discussion.
+
+`AIMSim` includes an automated testing apparatus operated by Python's _unittest_ built-in package. To execute tests related to the core functionality of `AIMSim`, run this command:
+
+`python -m unittest discover`
+
+Full multiprocessing speedup and efficiency tests take more than 10 hours to run due to the number of replicates required. To run these tests, create a file called `.speedup-test` in the `AIMSim` directory and execute the above command as shown.
+
+To manually build the docs, execute the following with `sphinx` and `m2r` installed and from the `/docs` directory:
+
+`m2r ../README.md | mv ../README.rst . | sphinx-apidoc -f -o . .. | make html | cp _build/html/* .`
+
+Documentation should manually build on push to master branch via an automated GitHub action.
+
+For packaging on PyPI:
+
+`python -m build; twine upload dist/*`
+
+Be sure to bump the version in `__init__.py`.
+
+## Citation
+If you use this code for scientific publications, please cite the following paper.
+
+Bhattacharjee, H.҂; Burns, J.҂; Vlachos, D.G. (2021): AIMSim: An Accessible Cheminformatics Platform for Similarity Operations on Chemicals Datasets. ChemRxiv. Preprint. https://doi.org/10.26434/chemrxiv-2022-nw6f5
+
+## License
+This code is made available under the terms of the _MIT Open License_:
+
+Copyright (c) 2020 Himaghna Bhattacharjee & Jackson Burns
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
+
+
+## Works Cited
+[1] Collins, K. and Glorius, F., A robustness screen for the rapid assessment of chemical reactions. Nature Chem 5, 597–601 (2013). https://doi.org/10.1038/nchem.1669
+
+[2] Chen, Y., Murray, P.R.D., Davies, A.T., and Willis M.C., J. Am. Chem. Soc. 140 (28), 8781-8787 (2018). https://doi.org/10.1021/jacs.8b04532
+
+[3] Hastie, T., Tibshirani R. and Friedman J., The Elements of statistical Learning: Data Mining, Inference, and Prediction, 2nd Ed., Springer Series in Statistics (2009).
+
+[4] Borg, I. and Groenen, P.J.F., Modern Multidimensional Scaling: Theory and Applications, Springer Series in Statistics (2005).
+
+[5] van der Maaten, L.J.P. and Hinton, G.E., Visualizing High-Dimensional Data Using t-SNE. Journal of Machine Learning Research 9:2579-2605 (2008).
+
+[6] Ng, A.Y., Jordan, M.I. and Weiss, Y., On Spectral Clustering: Analysis and an algorithm. ADVANCES IN NEURAL INFORMATION PROCESSING SYSTEMS, MIT Press (2001).
+
+[7] Tenenbaum, J.B., De Silva, V. and Langford, J.C, A global geometric framework for nonlinear dimensionality reduction, Science 290 (5500), 2319-23 (2000). https://doi.org/10.1126/science.290.5500.2319.
+
+[8] Murtagh, F. and Contreras, P., Algorithms for hierarchical clustering: an overview. WIREs Data Mining Knowl Discov (2011). https://doi.org/10.1002/widm.53
+
+
+
```

### Comparing `aimsim-2.0.2/aimsim.egg-info/SOURCES.txt` & `aimsim-2.0.3/aimsim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-20230222220038771.csv
 AIMSim-GUI.png
 LICENSE
 MANIFEST.in
 README.md
 config.yaml
 implemented_metrics.md
 requirements.txt
 setup.py
+.pytest_cache/README.md
 aimsim/__init__.py
 aimsim/__main__.py
 aimsim/exceptions.py
 aimsim.egg-info/PKG-INFO
 aimsim.egg-info/SOURCES.txt
 aimsim.egg-info/dependency_links.txt
 aimsim.egg-info/entry_points.txt
```

### Comparing `aimsim-2.0.2/config.yaml` & `aimsim-2.0.3/config.yaml`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-is_verbose: True
-molecule_database: 'tests\small.smi'
-molecule_database_source_type: text
-similarity_measure: 'tanimoto'
-# currently implements: 'rdkit topological' / 'morgan_fingerprint' (DEFAULT)
-fingerprint_type: 'topological_fingerprint'
-
-# The task field decides what you want to do
-# Each task field contains a sub-task field which further modifies the task.
-# The task fields are arranged as:
-  # tasks:
-     # task 1:
-        # sub-tasks of task 1
-# The lines beginning with '#!' can be directly uncommented to implement them.
-
-tasks:
-  visualize_dataset:
-      heatmap_plot_settings:
-          plot_color: 'green' # Set a color recognized by matplotlib.
-                             # Default is 'red'.
+is_verbose: True
+molecule_database: 'tests\small.smi'
+molecule_database_source_type: text
+similarity_measure: 'tanimoto'
+# currently implements: 'rdkit topological' / 'morgan_fingerprint' (DEFAULT)
+fingerprint_type: 'topological_fingerprint'
+
+# The task field decides what you want to do
+# Each task field contains a sub-task field which further modifies the task.
+# The task fields are arranged as:
+  # tasks:
+     # task 1:
+        # sub-tasks of task 1
+# The lines beginning with '#!' can be directly uncommented to implement them.
+
+tasks:
+  visualize_dataset:
+      heatmap_plot_settings:
+          plot_color: 'green' # Set a color recognized by matplotlib.
+                             # Default is 'red'.
           plot_title: 'Entire Dataset'  # Set a title for plot if needed.
```

### Comparing `aimsim-2.0.2/docs/_images/AIMSim-logo.png` & `aimsim-2.0.3/docs/_images/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.0.2/docs/_images/sulfonamide-substrate-scope.png` & `aimsim-2.0.3/docs/_images/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.0.2/docs/interfaces/UI/AIMSim-logo.png` & `aimsim-2.0.3/docs/interfaces/UI/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.0.2/docs/tests/sulfonamide-substrate-scope.png` & `aimsim-2.0.3/docs/tests/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.0.2/interfaces/UI/AIMSim-GUI-corner-logo.png` & `aimsim-2.0.3/interfaces/UI/AIMSim-GUI-corner-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.0.2/interfaces/UI/AIMSim-logo.png` & `aimsim-2.0.3/interfaces/UI/AIMSim-logo.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.0.2/interfaces/config_reader.py` & `aimsim-2.0.3/interfaces/config_reader.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-"""Reads a configuration file from the command line input and calls AIMSim.
-
-Raises:
-    IOError: If the tasks field is empty in the input file,
-    an IOError will be raised.
-"""
-from argparse import ArgumentParser
-import yaml
-import random
-
-from aimsim.tasks import TaskManager
-
-
-def main():
-    parser = ArgumentParser()
-    parser.add_argument("config", help="Path to config yaml file.")
-    args = parser.parse_args()
-    configs = yaml.load(open(args.config, "r"), Loader=yaml.FullLoader)
-    tasks = configs.pop("tasks", None)
-    if tasks is None:
-        raise IOError('"tasks" field not set in config file')
-    # if the global_random_seed has been specified, overwrite
-    # other random seeds
-    if configs.get('global_random_seed', None):
-        if configs.get('global_random_seed') == 'random' or type(configs.get('global_random_seed')) is not int:
-            configs['global_random_Seed'] = random.randint(0, 2**30)
-        if 'cluster' in tasks:
-            cluster_configs = tasks.get('cluster')
-            if cluster_configs.get('cluster_plot_settings', None):
-                cluster_plot_settings = cluster_configs.get(
-                    'cluster_plot_settings')
-                if cluster_plot_settings.get('embedding', None):
-                    embedding_settings = cluster_plot_settings.get('embedding')
-                    embedding_settings['random_state'] = configs['global_random_seed']
-                else:
-                    # need to make the embedding dict
-                    cluster_plot_settings['embedding'] = {
-                        'random_state': configs['global_random_seed']}
-            else:
-                # need to make all dictionaries
-                cluster_configs['cluster_plot_settings'] = {
-                    'embedding': {'random_state': configs['global_random_seed']}}
-        if 'identify_outliers' in tasks:
-            tasks['identify_outliers']['random_state'] = configs['global_random_seed']
-    task_manager = TaskManager(tasks=tasks)
-    task_manager(molecule_set_configs=configs)
-
-
-if __name__ == "__main__":
-    main()
+"""Reads a configuration file from the command line input and calls AIMSim.
+
+Raises:
+    IOError: If the tasks field is empty in the input file,
+    an IOError will be raised.
+"""
+from argparse import ArgumentParser
+import yaml
+import random
+
+from aimsim.tasks import TaskManager
+
+
+def main():
+    parser = ArgumentParser()
+    parser.add_argument("config", help="Path to config yaml file.")
+    args = parser.parse_args()
+    configs = yaml.load(open(args.config, "r"), Loader=yaml.FullLoader)
+    tasks = configs.pop("tasks", None)
+    if tasks is None:
+        raise IOError('"tasks" field not set in config file')
+    # if the global_random_seed has been specified, overwrite
+    # other random seeds
+    if configs.get('global_random_seed', None):
+        if configs.get('global_random_seed') == 'random' or type(configs.get('global_random_seed')) is not int:
+            configs['global_random_Seed'] = random.randint(0, 2**30)
+        if 'cluster' in tasks:
+            cluster_configs = tasks.get('cluster')
+            if cluster_configs.get('cluster_plot_settings', None):
+                cluster_plot_settings = cluster_configs.get(
+                    'cluster_plot_settings')
+                if cluster_plot_settings.get('embedding', None):
+                    embedding_settings = cluster_plot_settings.get('embedding')
+                    embedding_settings['random_state'] = configs['global_random_seed']
+                else:
+                    # need to make the embedding dict
+                    cluster_plot_settings['embedding'] = {
+                        'random_state': configs['global_random_seed']}
+            else:
+                # need to make all dictionaries
+                cluster_configs['cluster_plot_settings'] = {
+                    'embedding': {'random_state': configs['global_random_seed']}}
+        if 'identify_outliers' in tasks:
+            tasks['identify_outliers']['random_state'] = configs['global_random_seed']
+    task_manager = TaskManager(tasks=tasks)
+    task_manager(molecule_set_configs=configs)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `aimsim-2.0.2/tests/sulfonamide-substrate-scope-PDF.png` & `aimsim-2.0.3/tests/sulfonamide-substrate-scope-PDF.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.0.2/tests/sulfonamide-substrate-scope.png` & `aimsim-2.0.3/tests/sulfonamide-substrate-scope.png`

 * *Files identical despite different names*

### Comparing `aimsim-2.0.2/tests/test_Descriptor.py` & `aimsim-2.0.3/tests/test_Descriptor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,437 +1,463 @@
-"""Tests for the Descriptor class"""
-import unittest
-import numpy as np
-from rdkit.DataStructs.cDataStructs import ExplicitBitVect
-from rdkit.Chem import MolFromSmiles
-from aimsim.ops import Descriptor
-from aimsim.exceptions import MordredCalculatorError, InvalidConfigurationError
-from aimsim.utils.extras import requires_mordred
-
-SUPPORTED_FPRINTS = Descriptor.get_supported_fprints()
-
-
-class TestDescriptor(unittest.TestCase):
-    """Tests for methods of the Descriptor class.
-
-    Args:
-        unittest (unittest): Python unittest module.
-    """
-
-    def test_descriptor_empty_init(self):
-        """
-        Test to verify empty Descriptor object can be created.
-
-        """
-        descriptor = Descriptor()
-        self.assertFalse(
-            descriptor.check_init(),
-            "Expected Descriptor object to be uninitialized",
-        )
-
-    def test_descriptor_arbitrary_list_init(self):
-        """
-        Test to verify creation of Descriptor object initialized
-        by arbitrary list.
-
-        """
-        descriptor_value = [1, 2, 3]
-        descriptor = Descriptor(value=descriptor_value)
-        self.assertTrue(
-            descriptor.check_init(),
-            "Expected Descriptor object to be initialized",
-        )
-        self.assertEqual(
-            descriptor.label_,
-            "arbitrary",
-            "Expected label of descriptor initialized with "
-            'arbitrary vector to be "arbitrary"',
-        )
-        self.assertIsInstance(
-            descriptor.to_numpy(),
-            np.ndarray,
-            "Expected numpy.ndarray value from to_numpy()",
-        )
-        self.assertEqual(
-            descriptor.to_numpy().tolist(),
-            descriptor_value,
-            "Expected descriptor value to match init value",
-        )
-        with self.assertRaises(ValueError):
-            descriptor.to_rdkit()
-
-    def test_descriptor_arbitrary_numpy_init(self):
-        """
-        Test to verify creation of Descriptor object initialized
-        by arbitrary numpy array.
-
-        """
-        descriptor_value = np.array([1, 2, 3])
-        descriptor = Descriptor(value=descriptor_value)
-        self.assertTrue(
-            descriptor.check_init(),
-            "Expected Descriptor object to be initialized",
-        )
-        self.assertEqual(
-            descriptor.label_,
-            "arbitrary",
-            "Expected label of descriptor initialized with "
-            'arbitrary vector to be "arbitrary"',
-        )
-        self.assertIsInstance(
-            descriptor.to_numpy(), np.ndarray, "Expected numpy.ndarray from to_numpy()"
-        )
-        self.assertTrue(
-            (descriptor.to_numpy() == descriptor_value).all(),
-            "Expected descriptor value to match init value",
-        )
-        with self.assertRaises(ValueError):
-            descriptor.to_rdkit()
-
-    def test_topological_fprint_min_path_lesser_than_atoms(self):
-        atomic_mols = [MolFromSmiles(smiles) for smiles in ["C", "O", "N", "P"]]
-        diatomic_mols = [MolFromSmiles(smiles) for smiles in ["CC", "CO", "CN", "CP"]]
-        triatomic_mols = [
-            MolFromSmiles(smiles) for smiles in ["CCC", "COO", "CCN", "CCP"]
-        ]
-        min_path = 1
-        for mol in atomic_mols:
-            with self.assertRaises(InvalidConfigurationError):
-                descriptor = Descriptor()
-                descriptor.make_fingerprint(
-                    molecule_graph=mol,
-                    fingerprint_type="topological_fingerprint",
-                    fingerprint_params={"min_path": min_path},
-                )
-        for diatomic_mol in diatomic_mols:
-            descriptor = Descriptor()
-            try:
-                descriptor.make_fingerprint(
-                    molecule_graph=diatomic_mol,
-                    fingerprint_type="topological_fingerprint",
-                    fingerprint_params={"min_path": min_path},
-                )
-            except InvalidConfigurationError:
-                self.fail(
-                    "Did not expect Descriptor to raise " "InvalidConfigurationError"
-                )
-        for triatomic_mol in triatomic_mols:
-            descriptor = Descriptor()
-            try:
-                descriptor.make_fingerprint(
-                    molecule_graph=triatomic_mol,
-                    fingerprint_type="topological_fingerprint",
-                    fingerprint_params={"min_path": min_path},
-                )
-            except InvalidConfigurationError:
-                self.fail(
-                    "Did not expect Descriptor to raise " "InvalidConfigurationError"
-                )
-
-        min_path = 2
-        for mol in atomic_mols:
-            with self.assertRaises(InvalidConfigurationError):
-                descriptor = Descriptor()
-                descriptor.make_fingerprint(
-                    molecule_graph=mol,
-                    fingerprint_type="topological_fingerprint",
-                    fingerprint_params={"min_path": min_path},
-                )
-        for diatomic_mol in diatomic_mols:
-            with self.assertRaises(InvalidConfigurationError):
-                descriptor = Descriptor()
-                descriptor.make_fingerprint(
-                    molecule_graph=diatomic_mol,
-                    fingerprint_type="topological_fingerprint",
-                    fingerprint_params={"min_path": min_path},
-                )
-        for triatomic_mol in triatomic_mols:
-            descriptor = Descriptor()
-            try:
-                descriptor.make_fingerprint(
-                    molecule_graph=triatomic_mol,
-                    fingerprint_type="topological_fingerprint",
-                    fingerprint_params={"min_path": min_path},
-                )
-            except InvalidConfigurationError:
-                self.fail(
-                    "Did not expect Descriptor to raise " "InvalidConfigurationError"
-                )
-
-        min_path = 3
-        for mol in atomic_mols:
-            with self.assertRaises(InvalidConfigurationError):
-                descriptor = Descriptor()
-                descriptor.make_fingerprint(
-                    molecule_graph=mol,
-                    fingerprint_type="topological_fingerprint",
-                    fingerprint_params={"min_path": min_path},
-                )
-        for diatomic_mol in diatomic_mols:
-            with self.assertRaises(InvalidConfigurationError):
-                descriptor = Descriptor()
-                descriptor.make_fingerprint(
-                    molecule_graph=diatomic_mol,
-                    fingerprint_type="topological_fingerprint",
-                    fingerprint_params={"min_path": min_path},
-                )
-        for triatomic_mol in triatomic_mols:
-            with self.assertRaises(InvalidConfigurationError):
-                descriptor = Descriptor()
-                descriptor.make_fingerprint(
-                    molecule_graph=triatomic_mol,
-                    fingerprint_type="topological_fingerprint",
-                    fingerprint_params={"min_path": min_path},
-                )
-
-    def test_descriptor_make_fingerprint(self):
-        """
-        Test to verify creation of Descriptor object by
-        creating molecular fingerprints from the molecule graph.
-
-        """
-        mol_graph = MolFromSmiles("CCC")
-        for fprint in SUPPORTED_FPRINTS:
-            descriptor = Descriptor()
-            descriptor.make_fingerprint(
-                molecule_graph=mol_graph, fingerprint_type=fprint
-            )
-            self.assertTrue(
-                descriptor.check_init(),
-                "Expected Descriptor object to be initialized",
-            )
-            self.assertEqual(
-                descriptor.label_,
-                fprint,
-                "Expected label of descriptor initialized with "
-                "fingerprint to match the fingerprint",
-            )
-            self.assertIsInstance(
-                descriptor.to_numpy(),
-                np.ndarray,
-                "Expected numpy.ndarray from to_numpy()",
-            )
-            self.assertIsInstance(
-                descriptor.to_rdkit(),
-                ExplicitBitVect,
-                "Expected to_rdkit() to return "
-                "ExplicitBitVect representation "
-                f"of {fprint} fingerprint",
-            )
-
-    @requires_mordred
-    def test_mordred_descriptors(self):
-        """Test ability to passthrough descriptors to Mordred."""
-        mol_graph = MolFromSmiles(
-            "CC(C)C1=CC(=C(C(=C1)C(C)C)C2=CC=CC=C2P(C3CCCCC3)C4CCCCC4)C(C)C"
-        )
-        for desc in ["MW", "LogEE_Dt", "BalabanJ"]:
-            descriptor = Descriptor()
-            descriptor.make_fingerprint(
-                molecule_graph=mol_graph, fingerprint_type="mordred:" + desc
-            )
-            self.assertTrue(
-                descriptor.check_init(),
-                "Expected Descriptor object to be initialized",
-            )
-            self.assertEqual(
-                descriptor.label_,
-                desc,
-                "Expected label of descriptor initialized with "
-                "{} to match the fingerprint".format(desc),
-            )
-            self.assertIsInstance(
-                descriptor.to_numpy(),
-                np.ndarray,
-                "Expected numpy.ndarray from to_numpy()",
-            )
-            with self.assertRaises(ValueError):
-                descriptor.to_rdkit()
-
-    def test_padelpy_descriptors(self):
-        """Test ability to passthrough descriptors to PadelPy."""
-        mol_graph = MolFromSmiles("CCOCC")
-        for desc in ["MATS7e", "Ti", "ATSC6p"]:
-            descriptor = Descriptor()
-            descriptor.make_fingerprint(
-                molecule_graph=mol_graph, fingerprint_type="padelpy:" + desc
-            )
-            self.assertTrue(
-                descriptor.check_init(),
-                "Expected Descriptor object to be initialized",
-            )
-            self.assertEqual(
-                descriptor.label_,
-                desc,
-                "Expected label of descriptor initialized with "
-                "{} to match the fingerprint".format(desc),
-            )
-            self.assertIsInstance(
-                descriptor.to_numpy(),
-                np.ndarray,
-                "Expected numpy.ndarray from to_numpy()",
-            )
-            with self.assertRaises(ValueError):
-                descriptor.to_rdkit()
-
-    def test_ccbmlib_descriptors(self):
-        """Test ability to passthrough descriptors to ccbmlib."""
-        mol_graph = MolFromSmiles("CCOCC")
-        fprint_list = [
-            "atom_pairs",
-            "hashed_atom_pairs",
-            "avalon",
-            "maccs_keys",
-            "morgan",
-            "hashed_morgan",
-            "rdkit_fingerprint",
-            "torsions",
-            "hashed_torsions",
-        ]
-        for desc in fprint_list:
-            descriptor = Descriptor()
-            descriptor.make_fingerprint(
-                molecule_graph=mol_graph, fingerprint_type="ccbmlib:" + desc
-            )
-            self.assertTrue(
-                descriptor.check_init(),
-                "Expected Descriptor object to be initialized",
-            )
-            self.assertEqual(
-                descriptor.label_,
-                desc,
-                "Expected label of descriptor initialized with "
-                "{} to match the fingerprint".format(desc),
-            )
-
-    def test_exptl_descriptors(self):
-        """Test ability to use experimental descriptors."""
-        mol_graph = MolFromSmiles("CCOCC")
-        fprint_list = [
-            "maccs_keys",
-            "atom-pair_fingerprint",
-            "torsion_fingerprint",
-        ]
-        for desc in fprint_list:
-            descriptor = Descriptor()
-            descriptor.make_fingerprint(molecule_graph=mol_graph, fingerprint_type=desc)
-            self.assertTrue(
-                descriptor.check_init(),
-                "Expected Descriptor object to be initialized",
-            )
-            self.assertEqual(
-                descriptor.label_,
-                desc,
-                "Expected label of descriptor initialized with "
-                "{} to match the fingerprint".format(desc),
-            )
-
-    @requires_mordred
-    def test_nonexistent_mordred_descriptors(self):
-        """Test ability to pass through descriptors to Mordred."""
-        mol_graph = MolFromSmiles("C")
-        for desc in ["", "ReallyInvalidDescriptorName"]:
-            descriptor = Descriptor()
-            with self.assertRaises(MordredCalculatorError):
-                descriptor.make_fingerprint(
-                    molecule_graph=mol_graph,
-                    fingerprint_type="mordred:" + desc,
-                )
-
-    def test_bad_descriptors_padelpy_descriptors(self):
-        """Test ability to pass through invalid descriptors to padelpy."""
-        mol_graph = MolFromSmiles("C")
-        for desc in ["", "ReallyInvalidDescriptorName"]:
-            descriptor = Descriptor()
-            with self.assertRaises(RuntimeError):
-                descriptor.make_fingerprint(
-                    molecule_graph=mol_graph,
-                    fingerprint_type="padelpy:" + desc,
-                    fingerprint_params={"timeout": 2},
-                )
-
-    def test_fingerprint_folding(self):
-        """Create arbitrary fingerprint vector to check fold method"""
-        # Case 1
-        arbit_vector = np.array([1, 1, 1, 1, 1, 1, 1, 1, 1, 1])
-        arbit_label = "arbitrary"
-        desc = Descriptor()
-        desc.label_ = arbit_label
-        desc.numpy_ = arbit_vector
-        with self.assertRaises(ValueError):
-            desc.get_folded_fprint(fold_to_length=2)
-
-        # Case 2
-        arbit_vector = np.array([1, 0, 1, 0, 1, 0])
-        folded_vector = np.array([1, 1, 1])
-        arbit_label = "arbitrary_fingerprint"
-        desc = Descriptor()
-        desc.label_ = arbit_label
-        desc.numpy_ = arbit_vector
-        with self.assertRaises(InvalidConfigurationError):
-            desc.get_folded_fprint(fold_to_length=4)
-        with self.assertRaises(InvalidConfigurationError):
-            desc.get_folded_fprint(fold_to_length=10)
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=3) == folded_vector).all())
-        )
-
-        # Case 3
-        arbit_vector = np.array([1, 0, 1, 0, 0, 0, 0, 0])
-        folded_once_vector = np.array([1, 0, 1, 0])
-        folded_twice_vector = np.array([1, 0])
-        arbit_label = "arbitrary_fingerprint"
-        desc = Descriptor()
-        desc.label_ = arbit_label
-        desc.numpy_ = arbit_vector
-        with self.assertRaises(InvalidConfigurationError):
-            desc.get_folded_fprint(fold_to_length=3)
-        with self.assertRaises(InvalidConfigurationError):
-            desc.get_folded_fprint(fold_to_length=10)
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all())
-        )
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all())
-        )
-
-        # Case 3
-        arbit_vector = np.array([0, 0, 0, 0, 0, 0, 0, 0])
-        folded_once_vector = np.array([0, 0, 0, 0])
-        folded_twice_vector = np.array([0, 0])
-        arbit_label = "arbitrary_fingerprint"
-        desc = Descriptor()
-        desc.label_ = arbit_label
-        desc.numpy_ = arbit_vector
-        with self.assertRaises(InvalidConfigurationError):
-            desc.get_folded_fprint(fold_to_length=3)
-        with self.assertRaises(InvalidConfigurationError):
-            desc.get_folded_fprint(fold_to_length=10)
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all())
-        )
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all())
-        )
-
-        # Case 4
-        arbit_vector = np.array([1, 1, 1, 1, 1, 1, 1, 1])
-        folded_once_vector = np.array([1, 1, 1, 1])
-        folded_twice_vector = np.array([1, 1])
-        arbit_label = "arbitrary_fingerprint"
-        desc = Descriptor()
-        desc.label_ = arbit_label
-        desc.numpy_ = arbit_vector
-        with self.assertRaises(InvalidConfigurationError):
-            desc.get_folded_fprint(fold_to_length=3)
-        with self.assertRaises(InvalidConfigurationError):
-            desc.get_folded_fprint(fold_to_length=10)
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all())
-        )
-        self.assertTrue(
-            ((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all())
-        )
-
-
-if __name__ == "__main__":
-    unittest.main()
+"""Tests for the Descriptor class"""
+import unittest
+import numpy as np
+from rdkit.DataStructs.cDataStructs import ExplicitBitVect
+from rdkit.Chem import MolFromSmiles
+from aimsim.ops import Descriptor
+from aimsim.exceptions import MordredCalculatorError, InvalidConfigurationError
+from aimsim.utils.extras import requires_mordred
+
+SUPPORTED_FPRINTS = Descriptor.get_supported_fprints()
+
+
+class TestDescriptor(unittest.TestCase):
+    """Tests for methods of the Descriptor class.
+
+    Args:
+        unittest (unittest): Python unittest module.
+    """
+
+    def test_descriptor_empty_init(self):
+        """
+        Test to verify empty Descriptor object can be created.
+
+        """
+        descriptor = Descriptor()
+        self.assertFalse(
+            descriptor.check_init(),
+            "Expected Descriptor object to be uninitialized",
+        )
+
+    def test_descriptor_arbitrary_list_init(self):
+        """
+        Test to verify creation of Descriptor object initialized
+        by arbitrary list.
+
+        """
+        descriptor_value = [1, 2, 3]
+        descriptor = Descriptor(value=descriptor_value)
+        self.assertTrue(
+            descriptor.check_init(),
+            "Expected Descriptor object to be initialized",
+        )
+        self.assertEqual(
+            descriptor.label_,
+            "arbitrary",
+            "Expected label of descriptor initialized with "
+            'arbitrary vector to be "arbitrary"',
+        )
+        self.assertIsInstance(
+            descriptor.to_numpy(),
+            np.ndarray,
+            "Expected numpy.ndarray value from to_numpy()",
+        )
+        self.assertEqual(
+            descriptor.to_numpy().tolist(),
+            descriptor_value,
+            "Expected descriptor value to match init value",
+        )
+        with self.assertRaises(ValueError):
+            descriptor.to_rdkit()
+
+    def test_descriptor_arbitrary_numpy_init(self):
+        """
+        Test to verify creation of Descriptor object initialized
+        by arbitrary numpy array.
+
+        """
+        descriptor_value = np.array([1, 2, 3])
+        descriptor = Descriptor(value=descriptor_value)
+        self.assertTrue(
+            descriptor.check_init(),
+            "Expected Descriptor object to be initialized",
+        )
+        self.assertEqual(
+            descriptor.label_,
+            "arbitrary",
+            "Expected label of descriptor initialized with "
+            'arbitrary vector to be "arbitrary"',
+        )
+        self.assertIsInstance(
+            descriptor.to_numpy(), np.ndarray, "Expected numpy.ndarray from to_numpy()"
+        )
+        self.assertTrue(
+            (descriptor.to_numpy() == descriptor_value).all(),
+            "Expected descriptor value to match init value",
+        )
+        with self.assertRaises(ValueError):
+            descriptor.to_rdkit()
+
+    def test_topological_fprint_min_path_lesser_than_atoms(self):
+        atomic_mols = [MolFromSmiles(smiles) for smiles in ["C", "O", "N", "P"]]
+        diatomic_mols = [MolFromSmiles(smiles) for smiles in ["CC", "CO", "CN", "CP"]]
+        triatomic_mols = [
+            MolFromSmiles(smiles) for smiles in ["CCC", "COO", "CCN", "CCP"]
+        ]
+        min_path = 1
+        for mol in atomic_mols:
+            with self.assertRaises(InvalidConfigurationError):
+                descriptor = Descriptor()
+                descriptor.make_fingerprint(
+                    molecule_graph=mol,
+                    fingerprint_type="topological_fingerprint",
+                    fingerprint_params={"min_path": min_path},
+                )
+        for diatomic_mol in diatomic_mols:
+            descriptor = Descriptor()
+            try:
+                descriptor.make_fingerprint(
+                    molecule_graph=diatomic_mol,
+                    fingerprint_type="topological_fingerprint",
+                    fingerprint_params={"min_path": min_path},
+                )
+            except InvalidConfigurationError:
+                self.fail(
+                    "Did not expect Descriptor to raise " "InvalidConfigurationError"
+                )
+        for triatomic_mol in triatomic_mols:
+            descriptor = Descriptor()
+            try:
+                descriptor.make_fingerprint(
+                    molecule_graph=triatomic_mol,
+                    fingerprint_type="topological_fingerprint",
+                    fingerprint_params={"min_path": min_path},
+                )
+            except InvalidConfigurationError:
+                self.fail(
+                    "Did not expect Descriptor to raise " "InvalidConfigurationError"
+                )
+
+        min_path = 2
+        for mol in atomic_mols:
+            with self.assertRaises(InvalidConfigurationError):
+                descriptor = Descriptor()
+                descriptor.make_fingerprint(
+                    molecule_graph=mol,
+                    fingerprint_type="topological_fingerprint",
+                    fingerprint_params={"min_path": min_path},
+                )
+        for diatomic_mol in diatomic_mols:
+            with self.assertRaises(InvalidConfigurationError):
+                descriptor = Descriptor()
+                descriptor.make_fingerprint(
+                    molecule_graph=diatomic_mol,
+                    fingerprint_type="topological_fingerprint",
+                    fingerprint_params={"min_path": min_path},
+                )
+        for triatomic_mol in triatomic_mols:
+            descriptor = Descriptor()
+            try:
+                descriptor.make_fingerprint(
+                    molecule_graph=triatomic_mol,
+                    fingerprint_type="topological_fingerprint",
+                    fingerprint_params={"min_path": min_path},
+                )
+            except InvalidConfigurationError:
+                self.fail(
+                    "Did not expect Descriptor to raise " "InvalidConfigurationError"
+                )
+
+        min_path = 3
+        for mol in atomic_mols:
+            with self.assertRaises(InvalidConfigurationError):
+                descriptor = Descriptor()
+                descriptor.make_fingerprint(
+                    molecule_graph=mol,
+                    fingerprint_type="topological_fingerprint",
+                    fingerprint_params={"min_path": min_path},
+                )
+        for diatomic_mol in diatomic_mols:
+            with self.assertRaises(InvalidConfigurationError):
+                descriptor = Descriptor()
+                descriptor.make_fingerprint(
+                    molecule_graph=diatomic_mol,
+                    fingerprint_type="topological_fingerprint",
+                    fingerprint_params={"min_path": min_path},
+                )
+        for triatomic_mol in triatomic_mols:
+            with self.assertRaises(InvalidConfigurationError):
+                descriptor = Descriptor()
+                descriptor.make_fingerprint(
+                    molecule_graph=triatomic_mol,
+                    fingerprint_type="topological_fingerprint",
+                    fingerprint_params={"min_path": min_path},
+                )
+
+    def test_descriptor_make_fingerprint(self):
+        """
+        Test to verify creation of Descriptor object by
+        creating molecular fingerprints from the molecule graph.
+
+        """
+        mol_graph = MolFromSmiles("CCC")
+        for fprint in SUPPORTED_FPRINTS:
+            descriptor = Descriptor()
+            descriptor.make_fingerprint(
+                molecule_graph=mol_graph, fingerprint_type=fprint
+            )
+            self.assertTrue(
+                descriptor.check_init(),
+                "Expected Descriptor object to be initialized",
+            )
+            self.assertEqual(
+                descriptor.label_,
+                fprint,
+                "Expected label of descriptor initialized with "
+                "fingerprint to match the fingerprint",
+            )
+            self.assertIsInstance(
+                descriptor.to_numpy(),
+                np.ndarray,
+                "Expected numpy.ndarray from to_numpy()",
+            )
+            self.assertIsInstance(
+                descriptor.to_rdkit(),
+                ExplicitBitVect,
+                "Expected to_rdkit() to return "
+                "ExplicitBitVect representation "
+                f"of {fprint} fingerprint",
+            )
+
+    @requires_mordred
+    def test_mordred_descriptors(self):
+        """Test ability to passthrough descriptors to Mordred."""
+        mol_graph = MolFromSmiles(
+            "CC(C)C1=CC(=C(C(=C1)C(C)C)C2=CC=CC=C2P(C3CCCCC3)C4CCCCC4)C(C)C"
+        )
+        for desc in ["MW", "LogEE_Dt", "BalabanJ"]:
+            descriptor = Descriptor()
+            descriptor.make_fingerprint(
+                molecule_graph=mol_graph, fingerprint_type="mordred:" + desc
+            )
+            self.assertTrue(
+                descriptor.check_init(),
+                "Expected Descriptor object to be initialized",
+            )
+            self.assertEqual(
+                descriptor.label_,
+                desc,
+                "Expected label of descriptor initialized with "
+                "{} to match the fingerprint".format(desc),
+            )
+            self.assertIsInstance(
+                descriptor.to_numpy(),
+                np.ndarray,
+                "Expected numpy.ndarray from to_numpy()",
+            )
+            with self.assertRaises(ValueError):
+                descriptor.to_rdkit()
+
+    def test_padelpy_descriptors(self):
+        """Test ability to passthrough descriptors to PadelPy."""
+        mol_graph = MolFromSmiles("CCOCC")
+        for desc in ["MATS7e", "Ti", "ATSC6p"]:
+            descriptor = Descriptor()
+            descriptor.make_fingerprint(
+                molecule_graph=mol_graph, fingerprint_type="padelpy:" + desc
+            )
+            self.assertTrue(
+                descriptor.check_init(),
+                "Expected Descriptor object to be initialized",
+            )
+            self.assertEqual(
+                descriptor.label_,
+                desc,
+                "Expected label of descriptor initialized with "
+                "{} to match the fingerprint".format(desc),
+            )
+            self.assertIsInstance(
+                descriptor.to_numpy(),
+                np.ndarray,
+                "Expected numpy.ndarray from to_numpy()",
+            )
+            with self.assertRaises(ValueError):
+                descriptor.to_rdkit()
+
+    def test_minhash_fingerprint(self):
+        """Test creation of minhash fingerprint"""
+        mol_graph = MolFromSmiles("CCOCC")
+        descriptor = Descriptor()
+        descriptor.make_fingerprint(
+            molecule_graph=mol_graph, fingerprint_type="minhash_fingerprint"
+        )
+        self.assertTrue(
+            descriptor.check_init(),
+            "Expected Descriptor object to be initialized",
+        )
+        self.assertEqual(
+            descriptor.label_,
+            "minhash_fingerprint",
+            "Expected label of descriptor initialized with "
+            "{} to match the fingerprint".format("minhash_fingerprint"),
+        )
+        self.assertIsInstance(
+            descriptor.to_numpy(),
+            np.ndarray,
+            "Expected numpy.ndarray from to_numpy()",
+        )
+        with self.assertRaises(ValueError):
+            descriptor.to_rdkit()
+
+    def test_ccbmlib_descriptors(self):
+        """Test ability to passthrough descriptors to ccbmlib."""
+        mol_graph = MolFromSmiles("CCOCC")
+        fprint_list = [
+            "atom_pairs",
+            "hashed_atom_pairs",
+            "avalon",
+            "maccs_keys",
+            "morgan",
+            "hashed_morgan",
+            "rdkit_fingerprint",
+            "torsions",
+            "hashed_torsions",
+        ]
+        for desc in fprint_list:
+            descriptor = Descriptor()
+            descriptor.make_fingerprint(
+                molecule_graph=mol_graph, fingerprint_type="ccbmlib:" + desc
+            )
+            self.assertTrue(
+                descriptor.check_init(),
+                "Expected Descriptor object to be initialized",
+            )
+            self.assertEqual(
+                descriptor.label_,
+                desc,
+                "Expected label of descriptor initialized with "
+                "{} to match the fingerprint".format(desc),
+            )
+
+    def test_exptl_descriptors(self):
+        """Test ability to use experimental descriptors."""
+        mol_graph = MolFromSmiles("CCOCC")
+        fprint_list = [
+            "maccs_keys",
+            "atom-pair_fingerprint",
+            "torsion_fingerprint",
+            "minhash_fingerprint",
+        ]
+        for desc in fprint_list:
+            descriptor = Descriptor()
+            descriptor.make_fingerprint(molecule_graph=mol_graph, fingerprint_type=desc)
+            self.assertTrue(
+                descriptor.check_init(),
+                "Expected Descriptor object to be initialized",
+            )
+            self.assertEqual(
+                descriptor.label_,
+                desc,
+                "Expected label of descriptor initialized with "
+                "{} to match the fingerprint".format(desc),
+            )
+
+    @requires_mordred
+    def test_nonexistent_mordred_descriptors(self):
+        """Test ability to pass through descriptors to Mordred."""
+        mol_graph = MolFromSmiles("C")
+        for desc in ["", "ReallyInvalidDescriptorName"]:
+            descriptor = Descriptor()
+            with self.assertRaises(MordredCalculatorError):
+                descriptor.make_fingerprint(
+                    molecule_graph=mol_graph,
+                    fingerprint_type="mordred:" + desc,
+                )
+
+    def test_bad_descriptors_padelpy_descriptors(self):
+        """Test ability to pass through invalid descriptors to padelpy."""
+        mol_graph = MolFromSmiles("C")
+        for desc in ["", "ReallyInvalidDescriptorName"]:
+            descriptor = Descriptor()
+            with self.assertRaises(RuntimeError):
+                descriptor.make_fingerprint(
+                    molecule_graph=mol_graph,
+                    fingerprint_type="padelpy:" + desc,
+                    fingerprint_params={"timeout": 2},
+                )
+
+    def test_fingerprint_folding(self):
+        """Create arbitrary fingerprint vector to check fold method"""
+        # Case 1
+        arbit_vector = np.array([1, 1, 1, 1, 1, 1, 1, 1, 1, 1])
+        arbit_label = "arbitrary"
+        desc = Descriptor()
+        desc.label_ = arbit_label
+        desc.numpy_ = arbit_vector
+        with self.assertRaises(ValueError):
+            desc.get_folded_fprint(fold_to_length=2)
+
+        # Case 2
+        arbit_vector = np.array([1, 0, 1, 0, 1, 0])
+        folded_vector = np.array([1, 1, 1])
+        arbit_label = "arbitrary_fingerprint"
+        desc = Descriptor()
+        desc.label_ = arbit_label
+        desc.numpy_ = arbit_vector
+        with self.assertRaises(InvalidConfigurationError):
+            desc.get_folded_fprint(fold_to_length=4)
+        with self.assertRaises(InvalidConfigurationError):
+            desc.get_folded_fprint(fold_to_length=10)
+        self.assertTrue(
+            ((desc.get_folded_fprint(fold_to_length=3) == folded_vector).all())
+        )
+
+        # Case 3
+        arbit_vector = np.array([1, 0, 1, 0, 0, 0, 0, 0])
+        folded_once_vector = np.array([1, 0, 1, 0])
+        folded_twice_vector = np.array([1, 0])
+        arbit_label = "arbitrary_fingerprint"
+        desc = Descriptor()
+        desc.label_ = arbit_label
+        desc.numpy_ = arbit_vector
+        with self.assertRaises(InvalidConfigurationError):
+            desc.get_folded_fprint(fold_to_length=3)
+        with self.assertRaises(InvalidConfigurationError):
+            desc.get_folded_fprint(fold_to_length=10)
+        self.assertTrue(
+            ((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all())
+        )
+        self.assertTrue(
+            ((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all())
+        )
+
+        # Case 3
+        arbit_vector = np.array([0, 0, 0, 0, 0, 0, 0, 0])
+        folded_once_vector = np.array([0, 0, 0, 0])
+        folded_twice_vector = np.array([0, 0])
+        arbit_label = "arbitrary_fingerprint"
+        desc = Descriptor()
+        desc.label_ = arbit_label
+        desc.numpy_ = arbit_vector
+        with self.assertRaises(InvalidConfigurationError):
+            desc.get_folded_fprint(fold_to_length=3)
+        with self.assertRaises(InvalidConfigurationError):
+            desc.get_folded_fprint(fold_to_length=10)
+        self.assertTrue(
+            ((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all())
+        )
+        self.assertTrue(
+            ((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all())
+        )
+
+        # Case 4
+        arbit_vector = np.array([1, 1, 1, 1, 1, 1, 1, 1])
+        folded_once_vector = np.array([1, 1, 1, 1])
+        folded_twice_vector = np.array([1, 1])
+        arbit_label = "arbitrary_fingerprint"
+        desc = Descriptor()
+        desc.label_ = arbit_label
+        desc.numpy_ = arbit_vector
+        with self.assertRaises(InvalidConfigurationError):
+            desc.get_folded_fprint(fold_to_length=3)
+        with self.assertRaises(InvalidConfigurationError):
+            desc.get_folded_fprint(fold_to_length=10)
+        self.assertTrue(
+            ((desc.get_folded_fprint(fold_to_length=4) == folded_once_vector).all())
+        )
+        self.assertTrue(
+            ((desc.get_folded_fprint(fold_to_length=2) == folded_twice_vector).all())
+        )
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `aimsim-2.0.2/tests/test_LoadingErrorException.py` & `aimsim-2.0.3/tests/test_LoadingErrorException.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-""" Test the LoadingError Exception """
-import unittest
-
-from aimsim.exceptions import LoadingError
-from aimsim.chemical_datastructures import Molecule
-
-from pathlib import Path
-from os import remove
-
-
-class TestLoadingERrorException(unittest.TestCase):
-    """
-    Tests for LoadingError custom exception.
-
-    """
-
-    def test_missing_smiles(self):
-        """
-        Missing smiles strings should raise a LoadingError.
-        """
-        with self.assertRaises(LoadingError):
-            test_molecule = Molecule()
-            test_molecule._set_molecule_from_smiles([])
-
-    def test_invalid_smiles(self):
-        """Invalid SMILES strings should raise a LoadingError.
-        """
-        with self.assertRaises(LoadingError):
-            test_molecule = Molecule()
-            test_molecule._set_molecule_from_smiles("XYZ")
-
-    def test_missing_pdb(self):
-        """Missing PDB files should raise a LoadingError.
-        """
-        with self.assertRaises(LoadingError):
-            test_molecule = Molecule()
-            test_molecule._set_molecule_from_pdb("missing.pdb")
-
-    def test_invalid_pdb(self):
-        """Invalid PDB files should raise a LoadingError.
-        """
-        Path('blank.pdb').touch()
-        with self.assertRaises(LoadingError):
-            test_molecule = Molecule()
-            test_molecule._set_molecule_from_pdb("blank.pdb")
-        remove('blank.pdb')
-
-
-if __name__ == "__main__":
-    unittest.main()
+""" Test the LoadingError Exception """
+import unittest
+
+from aimsim.exceptions import LoadingError
+from aimsim.chemical_datastructures import Molecule
+
+from pathlib import Path
+from os import remove
+
+
+class TestLoadingERrorException(unittest.TestCase):
+    """
+    Tests for LoadingError custom exception.
+
+    """
+
+    def test_missing_smiles(self):
+        """
+        Missing smiles strings should raise a LoadingError.
+        """
+        with self.assertRaises(LoadingError):
+            test_molecule = Molecule()
+            test_molecule._set_molecule_from_smiles([])
+
+    def test_invalid_smiles(self):
+        """Invalid SMILES strings should raise a LoadingError.
+        """
+        with self.assertRaises(LoadingError):
+            test_molecule = Molecule()
+            test_molecule._set_molecule_from_smiles("XYZ")
+
+    def test_missing_pdb(self):
+        """Missing PDB files should raise a LoadingError.
+        """
+        with self.assertRaises(LoadingError):
+            test_molecule = Molecule()
+            test_molecule._set_molecule_from_pdb("missing.pdb")
+
+    def test_invalid_pdb(self):
+        """Invalid PDB files should raise a LoadingError.
+        """
+        Path('blank.pdb').touch()
+        with self.assertRaises(LoadingError):
+            test_molecule = Molecule()
+            test_molecule._set_molecule_from_pdb("blank.pdb")
+        remove('blank.pdb')
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `aimsim-2.0.2/tests/test_Molecule.py` & `aimsim-2.0.3/tests/test_Molecule.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,344 +1,344 @@
-""" Test the methods of the Molecule class """
-from os import remove
-import os.path
-import unittest
-
-import numpy as np
-import rdkit
-from rdkit.Chem import MolFromSmiles
-from rdkit.Chem.rdmolfiles import MolToPDBFile
-
-from aimsim.chemical_datastructures import Molecule
-from aimsim.exceptions import LoadingError
-from aimsim.ops import SimilarityMeasure
-
-
-class TestMolecule(unittest.TestCase):
-    """
-    Tests for methods of Molecule class.
-
-    """
-
-    def test_molecule_created_with_no_attributes(self):
-        """
-        Test for creation of empty Molecule object with no attributes.
-
-        """
-        test_molecule = Molecule()
-        self.assertIsNone(
-            test_molecule.mol_graph,
-            "Expected attribute mol_graph to be None for uninitialized Molecule",
-        )
-        self.assertIsNone(
-            test_molecule.mol_text,
-            "Expected attribute mol_text to be None for uninitialized Molecule",
-        )
-        self.assertIsNone(
-            test_molecule.mol_property_val,
-            "Expected attribute mol_property_val to be None "
-            "for uninitialized Molecule",
-        )
-        self.assertFalse(
-            test_molecule.descriptor.check_init(),
-            "Expected molecule.descriptor to be unitialized  "
-            "for uninitialized Molecule",
-        )
-
-    def test_molecule_created_w_attributes(self):
-        """
-        Test to create Molecule object with descriptor value (list) and a
-        response scalar.
-
-        """
-        test_molecule = Molecule(
-            mol_text="test_molecule", mol_property_val=42, mol_descriptor_val=[1, 2, 3]
-        )
-        self.assertEqual(
-            test_molecule.mol_text,
-            "test_molecule",
-            "Expected mol_text attribute to be set.",
-        )
-        self.assertEqual(
-            test_molecule.mol_property_val, 42, "Expected mol_property_val to be set."
-        )
-        self.assertIsInstance(
-            test_molecule.descriptor.to_numpy(),
-            np.ndarray,
-            "Expected descriptor.to_numpy()to be np.ndarray",
-        )
-        self.assertTrue(
-            np.all(test_molecule.descriptor.to_numpy() == np.array([1, 2, 3])),
-            "Expected descriptor.to_numpy() to be array[1, 2, 3]",
-        )
-        self.assertEqual(
-            test_molecule.descriptor.label_,
-            "arbitrary",
-            "Expected descriptor.label to be arbitrary since "
-            "it was initialized by list/array",
-        )
-
-    def test_set_molecule_from_smiles(self):
-        """
-        Test to create Molecule object by reading SMILES string.
-
-        """
-        test_smiles = "CC"
-        test_molecule = Molecule()
-        test_molecule._set_molecule_from_smiles(test_smiles)
-        self.assertEqual(
-            test_molecule.mol_text,
-            test_smiles,
-            "Expected mol_text attribute to be set " "to smiles string",
-        )
-        self.assertIsNotNone(
-            test_molecule.mol_graph,
-            "Expected mol_graph attribute to be set " "from the smiles",
-        )
-        self.assertIsInstance(
-            test_molecule.mol_graph,
-            rdkit.Chem.rdchem.Mol,
-            "Expected initialized mol_graph to " "be rdkit.Chem.rdchem.Mol object",
-        )
-
-    def test_set_molecule_from_file(self):
-        """
-        Test to create Molecule object by reading the contents of a file.
-
-        Case #1: text file
-        Case #2: PDB file
-
-        """
-        test_smiles = "CC"
-        # Case 1: text file
-        test_text_molecule = Molecule()
-        text_fpath = "test_mol_src.txt"
-        print(f"Creating file {text_fpath}...")
-        with open(text_fpath, "w") as fp:
-            fp.write(test_smiles + " garbage vals")
-        test_text_molecule._set_molecule_from_file(text_fpath)
-        self.assertEqual(
-            test_text_molecule.mol_text,
-            test_smiles,
-            "Expected mol_text attribute to be set "
-            "to smiles string when loading from txt file",
-        )
-        self.assertIsNotNone(
-            test_text_molecule.mol_graph,
-            "Expected mol_graph attribute to be set "
-            "from the smiles when loading from txt file",
-        )
-        self.assertIsInstance(
-            test_text_molecule.mol_graph,
-            rdkit.Chem.rdchem.Mol,
-            "Expected initialized mol_graph to "
-            "be rdkit.Chem.rdchem.Mol object "
-            "when loading from txt file",
-        )
-        print(f"Test complete. Deleting file {text_fpath}...")
-        remove(text_fpath)
-
-        # Case 2: pdb file
-        test_pdb_molecule = Molecule()
-        test_pdb_filename = "test_mol_src.pdb"
-        print(f"Creating file {test_pdb_filename}...")
-        test_mol = MolFromSmiles(test_smiles)
-        MolToPDBFile(test_mol, test_pdb_filename)
-        test_pdb_molecule._set_molecule_from_file(test_pdb_filename)
-        self.assertEqual(
-            test_pdb_molecule.mol_text,
-            os.path.basename(test_pdb_filename).split('.')[0],
-            "Expected mol_text attribute to be set "
-            "to name of file when loading from pdb file",
-        )
-        self.assertIsNotNone(
-            test_pdb_molecule.mol_graph,
-            "Expected mol_graph attribute to be set "
-            "from the smiles when loading from pdb file",
-        )
-        self.assertIsInstance(
-            test_pdb_molecule.mol_graph,
-            rdkit.Chem.rdchem.Mol,
-            "Expected initialized mol_graph to "
-            "be rdkit.Chem.rdchem.Mol object "
-            "when loading from pdb file",
-        )
-        print(f"Test complete. Deleting file {test_pdb_filename}...")
-        remove(test_pdb_filename)
-
-    def test_molecule_draw(self):
-        """
-        Test to draw molecule stored in Molecule object.
-
-        """
-        test_smiles = "CC"
-        test_molecule = Molecule()
-        test_molecule._set_molecule_from_smiles(test_smiles)
-        test_image_fpath = test_smiles + ".png"
-        test_molecule.draw(fpath=test_image_fpath)
-        self.assertTrue(os.path.isfile(test_image_fpath))
-        try:
-            print(f"Deleting {test_image_fpath}")
-            remove(test_image_fpath)
-        except FileNotFoundError:
-            print(f"Could not find {test_image_fpath}")
-
-    def test_molecule_graph_similar_to_itself_morgan_tanimoto(self):
-        """
-        Test that the morgan fingerprint of a Molecule object is similar
-        to itself using Tanimoto similarity.
-
-        """
-        test_smiles = "CC"
-        fingerprint_type = "morgan_fingerprint"
-        similarity_metric = "tanimoto"
-        test_molecule = Molecule()
-        test_molecule._set_molecule_from_smiles(test_smiles)
-        test_molecule_duplicate = Molecule()
-        test_molecule_duplicate._set_molecule_from_smiles(test_smiles)
-        test_molecule.set_descriptor(fingerprint_type=fingerprint_type)
-        test_molecule_duplicate.set_descriptor(
-            fingerprint_type=fingerprint_type)
-        similarity_measure = SimilarityMeasure(metric=similarity_metric)
-        tanimoto_similarity = test_molecule.get_similarity_to(
-            test_molecule_duplicate, similarity_measure=similarity_measure
-        )
-        self.assertEqual(
-            tanimoto_similarity,
-            1.0,
-            "Expected tanimoto similarity to be 1 when comparing "
-            "molecule graph to itself",
-        )
-
-    def test_mol_mol_similarity_w_morgan_tanimoto(self):
-        """
-        Test that the tanimoto similarity of the morgan fingerprints of
-        two Molecules are in (0, 1).
-
-        """
-        mol1_smiles = "CCCCCCCCC"
-        mol2_smiles = "CCCCCCCCCCC"
-        fingerprint_type = "morgan_fingerprint"
-        similarity_metric = "tanimoto"
-        molecules = []
-        for smiles in [mol1_smiles, mol2_smiles]:
-            molecule = Molecule(mol_smiles=smiles)
-            molecule.set_descriptor(fingerprint_type=fingerprint_type)
-            molecules.append(molecule)
-        similarity_measure = SimilarityMeasure(metric=similarity_metric)
-        tanimoto_similarity = molecules[0].get_similarity_to(
-            molecules[1], similarity_measure=similarity_measure
-        )
-        self.assertGreaterEqual(
-            tanimoto_similarity, 0.0, "Expected tanimoto similarity to be >= 0."
-        )
-        self.assertLessEqual(
-            tanimoto_similarity, 1.0, "Expected tanimoto similarity to be <= 1."
-        )
-
-    def test_molecule_graph_similar_to_itself_morgan_l0(self):
-        """
-        Test that the morgan fingerprint of a Molecule object is similar
-        to itself using L0 norm similarity.
-
-        """
-        test_smiles = "CC"
-        fingerprint_type = "morgan_fingerprint"
-        similarity_metric = "l0_similarity"
-        test_molecule = Molecule()
-        test_molecule._set_molecule_from_smiles(test_smiles)
-        test_molecule_duplicate = Molecule()
-        test_molecule_duplicate._set_molecule_from_smiles(test_smiles)
-        test_molecule.set_descriptor(fingerprint_type=fingerprint_type)
-        test_molecule_duplicate.set_descriptor(
-            fingerprint_type=fingerprint_type)
-        similarity_measure = SimilarityMeasure(metric=similarity_metric)
-        negl0_similarity = test_molecule.get_similarity_to(
-            test_molecule_duplicate, similarity_measure=similarity_measure
-        )
-        self.assertEqual(
-            negl0_similarity,
-            1.0,
-            "Expected l0_norm similarity to be 1. when comparing "
-            "molecule graph to itself",
-        )
-
-    def test_molecule_graph_similar_to_itself_morgan_dice(self):
-        """
-        Test that the morgan fingerprint of a Molecule object is similar
-        to itself using dice similarity.
-
-        """
-        test_smiles = "CCO"
-        fingerprint_type = "morgan_fingerprint"
-        similarity_metric = "dice"
-        test_molecule = Molecule()
-        test_molecule._set_molecule_from_smiles(test_smiles)
-        test_molecule_duplicate = Molecule()
-        test_molecule_duplicate._set_molecule_from_smiles(test_smiles)
-        test_molecule.set_descriptor(fingerprint_type=fingerprint_type)
-        test_molecule_duplicate.set_descriptor(
-            fingerprint_type=fingerprint_type)
-        similarity_measure = SimilarityMeasure(metric=similarity_metric)
-        dice_similarity = test_molecule.get_similarity_to(
-            test_molecule_duplicate, similarity_measure=similarity_measure
-        )
-        self.assertEqual(
-            dice_similarity,
-            1.0,
-            "Expected dice similarity to be 1 when comparing "
-            "molecule graph to itself",
-        )
-
-    def test_mol_src_pdb_loadingerror(self):
-        """Error in mol_src should raise LoadingError
-        """
-        with self.assertRaises(LoadingError):
-            Molecule(mol_src='non-existent file.pdb')
-
-    def test_mol_src_txt_loadingerror(self):
-        """Error in mol_src should raise LoadingError
-        """
-        with self.assertRaises(LoadingError):
-            Molecule(mol_src='non-existent file.txt')
-
-    def test_mol_smiles_loadingerror(self):
-        """Error in mol_smiles should raise LoadingError
-        """
-        with self.assertRaises(LoadingError):
-            Molecule(mol_smiles="XYZ")
-
-    def test_is_same(self):
-        """Two identical molecules should be identifed as such.
-        """
-        mol_1 = Molecule(mol_text="C")
-        mol_2 = Molecule(mol_text="C")
-        self.assertTrue(Molecule.is_same(mol_1, mol_2))
-
-    def test_get_name(self):
-        """Retrieve the name from the molecule.
-        """
-        mol = Molecule(mol_text="C")
-        self.assertEqual(mol.get_name(), "C")
-
-    def test_get_property_value(self):
-        """Retrieve the property value from the molecule
-        """
-        correct_val = 10
-        mol = Molecule(mol_text="C", mol_property_val=correct_val)
-        self.assertEqual(mol.get_mol_property_val(), correct_val)
-
-    def test_match_fprint_error(self):
-        """Trying to match fingerprint from molecule w/o graph should throw an error.
-        """
-        # initialize a molecule normally
-        ref_mol = Molecule(mol_smiles="C")
-        ref_mol.set_descriptor(fingerprint_type="morgan_fingerprint")
-        # delete the molecular graph
-        ref_mol.mol_graph = np.array([])
-        mol = Molecule()
-        with self.assertRaises(ValueError):
-            mol.match_fingerprint_from(ref_mol)
-
-
-if __name__ == "__main__":
-    unittest.main()
+""" Test the methods of the Molecule class """
+from os import remove
+import os.path
+import unittest
+
+import numpy as np
+import rdkit
+from rdkit.Chem import MolFromSmiles
+from rdkit.Chem.rdmolfiles import MolToPDBFile
+
+from aimsim.chemical_datastructures import Molecule
+from aimsim.exceptions import LoadingError
+from aimsim.ops import SimilarityMeasure
+
+
+class TestMolecule(unittest.TestCase):
+    """
+    Tests for methods of Molecule class.
+
+    """
+
+    def test_molecule_created_with_no_attributes(self):
+        """
+        Test for creation of empty Molecule object with no attributes.
+
+        """
+        test_molecule = Molecule()
+        self.assertIsNone(
+            test_molecule.mol_graph,
+            "Expected attribute mol_graph to be None for uninitialized Molecule",
+        )
+        self.assertIsNone(
+            test_molecule.mol_text,
+            "Expected attribute mol_text to be None for uninitialized Molecule",
+        )
+        self.assertIsNone(
+            test_molecule.mol_property_val,
+            "Expected attribute mol_property_val to be None "
+            "for uninitialized Molecule",
+        )
+        self.assertFalse(
+            test_molecule.descriptor.check_init(),
+            "Expected molecule.descriptor to be unitialized  "
+            "for uninitialized Molecule",
+        )
+
+    def test_molecule_created_w_attributes(self):
+        """
+        Test to create Molecule object with descriptor value (list) and a
+        response scalar.
+
+        """
+        test_molecule = Molecule(
+            mol_text="test_molecule", mol_property_val=42, mol_descriptor_val=[1, 2, 3]
+        )
+        self.assertEqual(
+            test_molecule.mol_text,
+            "test_molecule",
+            "Expected mol_text attribute to be set.",
+        )
+        self.assertEqual(
+            test_molecule.mol_property_val, 42, "Expected mol_property_val to be set."
+        )
+        self.assertIsInstance(
+            test_molecule.descriptor.to_numpy(),
+            np.ndarray,
+            "Expected descriptor.to_numpy()to be np.ndarray",
+        )
+        self.assertTrue(
+            np.all(test_molecule.descriptor.to_numpy() == np.array([1, 2, 3])),
+            "Expected descriptor.to_numpy() to be array[1, 2, 3]",
+        )
+        self.assertEqual(
+            test_molecule.descriptor.label_,
+            "arbitrary",
+            "Expected descriptor.label to be arbitrary since "
+            "it was initialized by list/array",
+        )
+
+    def test_set_molecule_from_smiles(self):
+        """
+        Test to create Molecule object by reading SMILES string.
+
+        """
+        test_smiles = "CC"
+        test_molecule = Molecule()
+        test_molecule._set_molecule_from_smiles(test_smiles)
+        self.assertEqual(
+            test_molecule.mol_text,
+            test_smiles,
+            "Expected mol_text attribute to be set " "to smiles string",
+        )
+        self.assertIsNotNone(
+            test_molecule.mol_graph,
+            "Expected mol_graph attribute to be set " "from the smiles",
+        )
+        self.assertIsInstance(
+            test_molecule.mol_graph,
+            rdkit.Chem.rdchem.Mol,
+            "Expected initialized mol_graph to " "be rdkit.Chem.rdchem.Mol object",
+        )
+
+    def test_set_molecule_from_file(self):
+        """
+        Test to create Molecule object by reading the contents of a file.
+
+        Case #1: text file
+        Case #2: PDB file
+
+        """
+        test_smiles = "CC"
+        # Case 1: text file
+        test_text_molecule = Molecule()
+        text_fpath = "test_mol_src.txt"
+        print(f"Creating file {text_fpath}...")
+        with open(text_fpath, "w") as fp:
+            fp.write(test_smiles + " garbage vals")
+        test_text_molecule._set_molecule_from_file(text_fpath)
+        self.assertEqual(
+            test_text_molecule.mol_text,
+            test_smiles,
+            "Expected mol_text attribute to be set "
+            "to smiles string when loading from txt file",
+        )
+        self.assertIsNotNone(
+            test_text_molecule.mol_graph,
+            "Expected mol_graph attribute to be set "
+            "from the smiles when loading from txt file",
+        )
+        self.assertIsInstance(
+            test_text_molecule.mol_graph,
+            rdkit.Chem.rdchem.Mol,
+            "Expected initialized mol_graph to "
+            "be rdkit.Chem.rdchem.Mol object "
+            "when loading from txt file",
+        )
+        print(f"Test complete. Deleting file {text_fpath}...")
+        remove(text_fpath)
+
+        # Case 2: pdb file
+        test_pdb_molecule = Molecule()
+        test_pdb_filename = "test_mol_src.pdb"
+        print(f"Creating file {test_pdb_filename}...")
+        test_mol = MolFromSmiles(test_smiles)
+        MolToPDBFile(test_mol, test_pdb_filename)
+        test_pdb_molecule._set_molecule_from_file(test_pdb_filename)
+        self.assertEqual(
+            test_pdb_molecule.mol_text,
+            os.path.basename(test_pdb_filename).split('.')[0],
+            "Expected mol_text attribute to be set "
+            "to name of file when loading from pdb file",
+        )
+        self.assertIsNotNone(
+            test_pdb_molecule.mol_graph,
+            "Expected mol_graph attribute to be set "
+            "from the smiles when loading from pdb file",
+        )
+        self.assertIsInstance(
+            test_pdb_molecule.mol_graph,
+            rdkit.Chem.rdchem.Mol,
+            "Expected initialized mol_graph to "
+            "be rdkit.Chem.rdchem.Mol object "
+            "when loading from pdb file",
+        )
+        print(f"Test complete. Deleting file {test_pdb_filename}...")
+        remove(test_pdb_filename)
+
+    def test_molecule_draw(self):
+        """
+        Test to draw molecule stored in Molecule object.
+
+        """
+        test_smiles = "CC"
+        test_molecule = Molecule()
+        test_molecule._set_molecule_from_smiles(test_smiles)
+        test_image_fpath = test_smiles + ".png"
+        test_molecule.draw(fpath=test_image_fpath)
+        self.assertTrue(os.path.isfile(test_image_fpath))
+        try:
+            print(f"Deleting {test_image_fpath}")
+            remove(test_image_fpath)
+        except FileNotFoundError:
+            print(f"Could not find {test_image_fpath}")
+
+    def test_molecule_graph_similar_to_itself_morgan_tanimoto(self):
+        """
+        Test that the morgan fingerprint of a Molecule object is similar
+        to itself using Tanimoto similarity.
+
+        """
+        test_smiles = "CC"
+        fingerprint_type = "morgan_fingerprint"
+        similarity_metric = "tanimoto"
+        test_molecule = Molecule()
+        test_molecule._set_molecule_from_smiles(test_smiles)
+        test_molecule_duplicate = Molecule()
+        test_molecule_duplicate._set_molecule_from_smiles(test_smiles)
+        test_molecule.set_descriptor(fingerprint_type=fingerprint_type)
+        test_molecule_duplicate.set_descriptor(
+            fingerprint_type=fingerprint_type)
+        similarity_measure = SimilarityMeasure(metric=similarity_metric)
+        tanimoto_similarity = test_molecule.get_similarity_to(
+            test_molecule_duplicate, similarity_measure=similarity_measure
+        )
+        self.assertEqual(
+            tanimoto_similarity,
+            1.0,
+            "Expected tanimoto similarity to be 1 when comparing "
+            "molecule graph to itself",
+        )
+
+    def test_mol_mol_similarity_w_morgan_tanimoto(self):
+        """
+        Test that the tanimoto similarity of the morgan fingerprints of
+        two Molecules are in (0, 1).
+
+        """
+        mol1_smiles = "CCCCCCCCC"
+        mol2_smiles = "CCCCCCCCCCC"
+        fingerprint_type = "morgan_fingerprint"
+        similarity_metric = "tanimoto"
+        molecules = []
+        for smiles in [mol1_smiles, mol2_smiles]:
+            molecule = Molecule(mol_smiles=smiles)
+            molecule.set_descriptor(fingerprint_type=fingerprint_type)
+            molecules.append(molecule)
+        similarity_measure = SimilarityMeasure(metric=similarity_metric)
+        tanimoto_similarity = molecules[0].get_similarity_to(
+            molecules[1], similarity_measure=similarity_measure
+        )
+        self.assertGreaterEqual(
+            tanimoto_similarity, 0.0, "Expected tanimoto similarity to be >= 0."
+        )
+        self.assertLessEqual(
+            tanimoto_similarity, 1.0, "Expected tanimoto similarity to be <= 1."
+        )
+
+    def test_molecule_graph_similar_to_itself_morgan_l0(self):
+        """
+        Test that the morgan fingerprint of a Molecule object is similar
+        to itself using L0 norm similarity.
+
+        """
+        test_smiles = "CC"
+        fingerprint_type = "morgan_fingerprint"
+        similarity_metric = "l0_similarity"
+        test_molecule = Molecule()
+        test_molecule._set_molecule_from_smiles(test_smiles)
+        test_molecule_duplicate = Molecule()
+        test_molecule_duplicate._set_molecule_from_smiles(test_smiles)
+        test_molecule.set_descriptor(fingerprint_type=fingerprint_type)
+        test_molecule_duplicate.set_descriptor(
+            fingerprint_type=fingerprint_type)
+        similarity_measure = SimilarityMeasure(metric=similarity_metric)
+        negl0_similarity = test_molecule.get_similarity_to(
+            test_molecule_duplicate, similarity_measure=similarity_measure
+        )
+        self.assertEqual(
+            negl0_similarity,
+            1.0,
+            "Expected l0_norm similarity to be 1. when comparing "
+            "molecule graph to itself",
+        )
+
+    def test_molecule_graph_similar_to_itself_morgan_dice(self):
+        """
+        Test that the morgan fingerprint of a Molecule object is similar
+        to itself using dice similarity.
+
+        """
+        test_smiles = "CCO"
+        fingerprint_type = "morgan_fingerprint"
+        similarity_metric = "dice"
+        test_molecule = Molecule()
+        test_molecule._set_molecule_from_smiles(test_smiles)
+        test_molecule_duplicate = Molecule()
+        test_molecule_duplicate._set_molecule_from_smiles(test_smiles)
+        test_molecule.set_descriptor(fingerprint_type=fingerprint_type)
+        test_molecule_duplicate.set_descriptor(
+            fingerprint_type=fingerprint_type)
+        similarity_measure = SimilarityMeasure(metric=similarity_metric)
+        dice_similarity = test_molecule.get_similarity_to(
+            test_molecule_duplicate, similarity_measure=similarity_measure
+        )
+        self.assertEqual(
+            dice_similarity,
+            1.0,
+            "Expected dice similarity to be 1 when comparing "
+            "molecule graph to itself",
+        )
+
+    def test_mol_src_pdb_loadingerror(self):
+        """Error in mol_src should raise LoadingError
+        """
+        with self.assertRaises(LoadingError):
+            Molecule(mol_src='non-existent file.pdb')
+
+    def test_mol_src_txt_loadingerror(self):
+        """Error in mol_src should raise LoadingError
+        """
+        with self.assertRaises(LoadingError):
+            Molecule(mol_src='non-existent file.txt')
+
+    def test_mol_smiles_loadingerror(self):
+        """Error in mol_smiles should raise LoadingError
+        """
+        with self.assertRaises(LoadingError):
+            Molecule(mol_smiles="XYZ")
+
+    def test_is_same(self):
+        """Two identical molecules should be identifed as such.
+        """
+        mol_1 = Molecule(mol_text="C")
+        mol_2 = Molecule(mol_text="C")
+        self.assertTrue(Molecule.is_same(mol_1, mol_2))
+
+    def test_get_name(self):
+        """Retrieve the name from the molecule.
+        """
+        mol = Molecule(mol_text="C")
+        self.assertEqual(mol.get_name(), "C")
+
+    def test_get_property_value(self):
+        """Retrieve the property value from the molecule
+        """
+        correct_val = 10
+        mol = Molecule(mol_text="C", mol_property_val=correct_val)
+        self.assertEqual(mol.get_mol_property_val(), correct_val)
+
+    def test_match_fprint_error(self):
+        """Trying to match fingerprint from molecule w/o graph should throw an error.
+        """
+        # initialize a molecule normally
+        ref_mol = Molecule(mol_smiles="C")
+        ref_mol.set_descriptor(fingerprint_type="morgan_fingerprint")
+        # delete the molecular graph
+        ref_mol.mol_graph = np.array([])
+        mol = Molecule()
+        with self.assertRaises(ValueError):
+            mol.match_fingerprint_from(ref_mol)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `aimsim-2.0.2/tests/test_MoleculeSet.py` & `aimsim-2.0.3/tests/test_MoleculeSet.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,1350 +1,1350 @@
-"""Test the MoleculeSet class."""
-from os import remove, mkdir
-import os.path
-from shutil import rmtree
-import unittest
-
-import numpy as np
-import pandas as pd
-from rdkit.Chem import MolFromSmiles
-from rdkit.Chem.rdmolfiles import MolToPDBFile
-from sklearn.decomposition import PCA
-from sklearn.manifold import MDS, TSNE, Isomap, SpectralEmbedding
-from sklearn.preprocessing import StandardScaler
-
-from aimsim.chemical_datastructures import Molecule, MoleculeSet
-from aimsim.ops import Descriptor, SimilarityMeasure
-from aimsim.exceptions import NotInitializedError, InvalidConfigurationError
-
-
-SUPPORTED_SIMILARITIES = SimilarityMeasure.get_supported_metrics()
-
-SUPPORTED_FPRINTS = Descriptor.get_supported_fprints()
-
-
-class TestMoleculeSet(unittest.TestCase):
-    test_smarts = [
-        "[CH3:1][S:2][c:3]1[cH:4][cH:5][c:6]([B:7]([OH:8])[OH:9])[cH:10][cH:11]1",
-        "[NH:1]1[CH2:2][CH2:3][O:4][CH2:5][CH2:6]1.[O:7]=[S:8]=[O:9]",
-    ]
-
-    test_smiles = [
-        "CCCCCCC",
-        "CCCC",
-        "CCC",
-        "CO",
-        "CN",
-        "C1=CC=CC=C1",
-        "CC1=CC=CC=C1",
-        "C(=O)(N)N",
-    ]
-
-    def get_feature_set(self, dimensionality=10):
-        n_test_mols = len(self.test_smiles)
-        test_feature_set = []
-        feature_value_upper_limit = 1000
-        for i in range(n_test_mols):
-            test_feature_set.append(
-                [
-                    np.random.random() * feature_value_upper_limit
-                    for _ in range(dimensionality)
-                ]
-            )
-        return np.array(test_feature_set)
-
-    def smiles_seq_to_textfile(self, property_seq=None):
-        """Helper method to convert a SMILES sequence to a text file.
-
-        Args:
-            property_seq (list or np.ndarray, optional): Optional sequence of
-                molecular responses.. Defaults to None.
-
-        Returns:
-            str: Path to created file.
-        """
-        text_fpath = "temp_smiles_seq.txt"
-        print(f"Creating text file {text_fpath}")
-        with open(text_fpath, "w") as fp:
-            for id, smiles in enumerate(self.test_smiles):
-                write_txt = smiles
-                if property_seq is not None:
-                    write_txt += " " + str(property_seq[id])
-                if id < len(self.test_smiles) - 1:
-                    write_txt += "\n"
-
-                fp.write(write_txt)
-        return text_fpath
-
-    def smiles_seq_to_smi_file(self, property_seq=None):
-        """Helper method to convert a SMILES sequence to a .smi file.
-
-        Args:
-            property_seq (list or np.ndarray, optional): Optional sequence of
-                molecular responses. Defaults to None.
-
-        Returns:
-            str: Path to created file.
-        """
-        smi_fpath = "temp_smiles_seq.smi"
-        print(f"Creating text file {smi_fpath}")
-        with open(smi_fpath, "w") as fp:
-            for id, smiles in enumerate(self.test_smiles):
-                write_txt = smiles
-                if property_seq is not None:
-                    write_txt += " " + str(property_seq[id])
-                if id < len(self.test_smiles) - 1:
-                    write_txt += "\n"
-
-                fp.write(write_txt)
-        return smi_fpath
-
-    def smiles_seq_to_smiles_file(self, property_seq=None):
-        """Helper method to convert a SMILES sequence to a .SMILES file.
-
-        Args:
-            property_seq (list or np.ndarray, optional): Optional sequence of
-                molecular responses. Defaults to None.
-
-        Returns:
-            str: Path to created file.
-        """
-        SMILES_fpath = "temp_smiles_seq.SMILES"
-        print(f"Creating text file {SMILES_fpath}")
-        with open(SMILES_fpath, "w") as fp:
-            for id, smiles in enumerate(self.test_smiles):
-                write_txt = smiles
-                if property_seq is not None:
-                    write_txt += " " + str(property_seq[id])
-                if id < len(self.test_smiles) - 1:
-                    write_txt += "\n"
-
-                fp.write(write_txt)
-        return SMILES_fpath
-
-    def smarts_seq_to_smiles_file(self, property_seq=None):
-        """Helper method to convert a SMARTS sequence to a .SMILES file.
-
-        Args:
-            property_seq (list or np.ndarray, optional): Optional sequence of
-                molecular responses. Defaults to None.
-
-        Returns:
-            str: Path to created file.
-        """
-        SMILES_fpath = "temp_smiles_seq.SMILES"
-        print(f"Creating text file {SMILES_fpath}")
-        with open(SMILES_fpath, "w") as fp:
-            for id, smiles in enumerate(self.test_smarts):
-                write_txt = smiles
-                if property_seq is not None:
-                    write_txt += " " + str(property_seq[id])
-                if id < len(self.test_smiles) - 1:
-                    write_txt += "\n"
-
-                fp.write(write_txt)
-        return SMILES_fpath
-
-    def smiles_seq_to_pdb_dir(self, property_seq=None):
-        """Helper method to convert a SMILES sequence to a pdb files
-        stored in a directory.
-
-        Args:
-            property_seq (list or np.ndarray, optional): Optional sequence of
-                molecular responses. Defaults to None.
-
-        Returns:
-            str: Path to created directory.
-        """
-        dir_path = "test_dir"
-        if not os.path.isdir(dir_path):
-            print(f"Creating directory {dir_path}")
-            mkdir(dir_path)
-        for smiles_str in self.test_smiles:
-            mol_graph = MolFromSmiles(smiles_str)
-            assert mol_graph is not None
-            pdb_fpath = os.path.join(dir_path, smiles_str + ".pdb")
-            print(f"Creating file {pdb_fpath}")
-            MolToPDBFile(mol_graph, pdb_fpath)
-        return dir_path
-
-    def smiles_seq_to_xl_or_csv(
-        self, ftype, property_seq=None, name_seq=None, feature_arr=None
-    ):
-        """Helper method to convert a SMILES sequence or arbitrary features
-        to Excel or CSV files.
-
-        Args:
-            ftype (str): String label to denote the filetype. 'csv' or 'excel'.
-            property_seq (list or np.ndarray, optional): Optional sequence of
-                molecular responses. Defaults to None.
-            name_seq (list or np.ndarray, optional): Optional sequence of
-                molecular names. Defaults to None.
-            feature_arr (np.ndarray, optional): Optional array of molecular
-                descriptor values. Defaults to None.
-
-        Raises:
-            ValueError: Invalid file type specified.
-
-        Returns:
-            str: Path to created file.
-        """
-        data = {"descriptor_smiles": self.test_smiles}
-        if property_seq is not None:
-            data.update({"response_random": property_seq})
-        if name_seq is not None:
-            data.update({"descriptor_name": name_seq})
-        if feature_arr is not None:
-            feature_arr = np.array(feature_arr)
-            for feature_num in range(feature_arr.shape[1]):
-                data.update({f"descriptor_{feature_num}": feature_arr[:, feature_num]})
-        data_df = pd.DataFrame(data)
-        fpath = "temp_mol_file"
-        if ftype == "excel":
-            fpath += ".xlsx"
-            print(f"Creating {ftype} file {fpath}")
-            data_df.to_excel(fpath)
-        elif ftype == "csv":
-            fpath += ".csv"
-            print(f"Creating {ftype} file {fpath}")
-            data_df.to_csv(fpath)
-        else:
-            raise ValueError(f"{ftype} not supported")
-        return fpath
-
-    def test_set_molecule_database_from_textfile(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        from a textfile.
-
-        """
-        text_fpath = self.smiles_seq_to_textfile()
-        molecule_set = MoleculeSet(
-            molecule_database_src=text_fpath,
-            molecule_database_src_type="text",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from text",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number "
-            "of smiles in text file",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smiles[id],
-                "Expected mol_text attribute of Molecule object to be smiles",
-            )
-            self.assertIsNone(
-                molecule.mol_property_val,
-                "Expected mol_property_val of Molecule object "
-                "initialized without property to be None",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to " "be Molecule object",
-            )
-        print(f"Test complete. Deleting file {text_fpath}...")
-        remove(text_fpath)
-
-    def test_set_molecule_database_from_smi_file(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        from a smi file.
-
-        """
-        text_fpath = self.smiles_seq_to_smi_file()
-        molecule_set = MoleculeSet(
-            molecule_database_src=text_fpath,
-            molecule_database_src_type="text",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from text",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number "
-            "of smiles in text file",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smiles[id],
-                "Expected mol_text attribute of Molecule object to be smiles",
-            )
-            self.assertIsNone(
-                molecule.mol_property_val,
-                "Expected mol_property_val of Molecule object "
-                "initialized without property to be None",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to " "be Molecule object",
-            )
-        print(f"Test complete. Deleting file {text_fpath}...")
-        remove(text_fpath)
-
-    def test_set_molecule_database_from_smiles_file(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        from a SMILES file.
-
-        """
-        text_fpath = self.smiles_seq_to_smiles_file()
-        molecule_set = MoleculeSet(
-            molecule_database_src=text_fpath,
-            molecule_database_src_type="text",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from text",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number "
-            "of smiles in text file",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smiles[id],
-                "Expected mol_text attribute of Molecule object to be smiles",
-            )
-            self.assertIsNone(
-                molecule.mol_property_val,
-                "Expected mol_property_val of Molecule object "
-                "initialized without property to be None",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to " "be Molecule object",
-            )
-        print(f"Test complete. Deleting file {text_fpath}...")
-        remove(text_fpath)
-
-    def test_set_molecule_database_from_smarts_file(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        from a SMILES file containing SMARTS strings.
-
-        """
-        text_fpath = self.smarts_seq_to_smiles_file()
-        molecule_set = MoleculeSet(
-            molecule_database_src=text_fpath,
-            molecule_database_src_type="text",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from text",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smarts),
-            "Expected the size of database to be equal to number "
-            "of smiles in text file",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smarts[id],
-                "Expected mol_text attribute of Molecule object to be smiles",
-            )
-            self.assertIsNone(
-                molecule.mol_property_val,
-                "Expected mol_property_val of Molecule object "
-                "initialized without property to be None",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to " "be Molecule object",
-            )
-        print(f"Test complete. Deleting file {text_fpath}...")
-        remove(text_fpath)
-
-    def test_subsample_molecule_database_from_textfile(self):
-        """
-        Test to randomly subsample a molecule database loaded from a textfile.
-
-        """
-        text_fpath = self.smiles_seq_to_textfile()
-        sampling_ratio = 0.5
-        molecule_set = MoleculeSet(
-            molecule_database_src=text_fpath,
-            molecule_database_src_type="text",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-            sampling_ratio=sampling_ratio,
-        )
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from text",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            int(sampling_ratio * len(self.test_smiles)),
-            "Expected the size of subsampled database to be equal "
-            "to number of smiles in text file * sampling_ratio",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to " "be Molecule object",
-            )
-        print(f"Test complete. Deleting file {text_fpath}...")
-        remove(text_fpath)
-
-    def test_set_molecule_database_w_property_from_textfile(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        and molecular responses from a textfile.
-
-        """
-        properties = np.random.normal(size=len(self.test_smiles))
-        text_fpath = self.smiles_seq_to_textfile(property_seq=properties)
-        molecule_set = MoleculeSet(
-            molecule_database_src=text_fpath,
-            molecule_database_src_type="text",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from text",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number "
-            "of smiles in text file",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smiles[id],
-                "Expected mol_text attribute of Molecule object " "to be smiles",
-            )
-            self.assertAlmostEqual(
-                molecule.mol_property_val,
-                properties[id],
-                places=7,
-                msg="Expected mol_property_val of"
-                "Molecule object "
-                "to be set to value in text file",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to " "be Molecule object",
-            )
-        print(f"Test complete. Deleting file {text_fpath}...")
-        remove(text_fpath)
-
-    def test_set_molecule_database_from_pdb_dir(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        from a directory of pdb files.
-
-        """
-        dir_path = self.smiles_seq_to_pdb_dir(self.test_smiles)
-        molecule_set = MoleculeSet(
-            molecule_database_src=dir_path,
-            molecule_database_src_type="directory",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from dir",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number " "of files in dir",
-        )
-        for molecule in molecule_set.molecule_database:
-            self.assertIn(
-                molecule.mol_text,
-                self.test_smiles,
-                "Expected molecule text to be a smiles string",
-            )
-            self.assertIsNone(
-                molecule.mol_property_val,
-                "Expected mol_property_val of Molecule object"
-                "initialized without property to be None",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to " "be Molecule object",
-            )
-        print(f"Test complete. Deleting directory {dir_path}...")
-        rmtree(dir_path)
-
-    def test_subsample_molecule_database_from_pdb_dir(self):
-        """
-        Test to randomly subsample a molecule database loaded from a
-        directory of pdb files.
-
-        """
-        dir_path = self.smiles_seq_to_pdb_dir(self.test_smiles)
-        sampling_ratio = 0.5
-        molecule_set = MoleculeSet(
-            molecule_database_src=dir_path,
-            molecule_database_src_type="directory",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-            sampling_ratio=sampling_ratio,
-        )
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from dir",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            int(sampling_ratio * len(self.test_smiles)),
-            "Expected the size of subsampled database to be "
-            "equal to number of files in dir * sampling_ratio",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to " "be Molecule object",
-            )
-        print(f"Test complete. Deleting directory {dir_path}...")
-        rmtree(dir_path)
-
-    def test_set_molecule_database_from_excel(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        from an Excel file.
-
-        """
-        xl_fpath = self.smiles_seq_to_xl_or_csv(ftype="excel")
-        molecule_set = MoleculeSet(
-            molecule_database_src=xl_fpath,
-            molecule_database_src_type="excel",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from excel file",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number of smiles",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smiles[id],
-                "Expected mol_text attribute of Molecule object "
-                "to be smiles when names not present in excel",
-            )
-            self.assertIsNone(
-                molecule.mol_property_val,
-                "Expected mol_property_val of Molecule object"
-                "initialized without property to be None",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to be Molecule object",
-            )
-        print(f"Test complete. Deleting file {xl_fpath}...")
-        remove(xl_fpath)
-
-    def test_set_molecule_database_from_excel_without_smiles_name(self):
-        xl_fpath = "test_files.xlsx"
-        features = self.get_feature_set()  # n_samples x dimensionality
-        data = dict()
-        for feature_id in range(features.shape[-1]):
-            data[f"descriptor_{feature_id}"] = features[:, feature_id].flatten()
-        df = pd.DataFrame(data)
-        print(f"Creating text file {xl_fpath}")
-        df.to_excel(xl_fpath)
-        molecule_set = MoleculeSet(
-            molecule_database_src=xl_fpath,
-            molecule_database_src_type="excel",
-            similarity_measure="l2_similarity",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from excel file",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number of smiles",
-        )
-        self.assertTrue(
-            np.allclose(features, molecule_set.get_mol_features(), rtol=1e-4),
-            "Expected molecule feature vectors to "
-            "be the same as features in input file",
-        )
-        with self.assertRaises(ValueError):
-            molecule_set = MoleculeSet(
-                molecule_database_src=xl_fpath,
-                molecule_database_src_type="excel",
-                fingerprint_type="morgan_fingerprint",
-                similarity_measure="l2_similarity",
-                is_verbose=True,
-            )
-        with self.assertRaises(ValueError):
-            molecule_set = MoleculeSet(
-                molecule_database_src=xl_fpath,
-                molecule_database_src_type="excel",
-                similarity_measure="tanimoto_similarity",
-                is_verbose=True,
-            )
-        print(f"Test complete. Deleting file {xl_fpath}...")
-        remove(xl_fpath)
-
-    def test_subsample_molecule_database_from_excel(self):
-        """
-        Test to randomly subsample a molecule database loaded from an
-        Excel file.
-
-        """
-        xl_fpath = self.smiles_seq_to_xl_or_csv(ftype="excel")
-        sampling_ratio = 0.5
-        molecule_set = MoleculeSet(
-            molecule_database_src=xl_fpath,
-            molecule_database_src_type="excel",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-            sampling_ratio=sampling_ratio,
-        )
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from excel file",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            int(sampling_ratio * len(self.test_smiles)),
-            "Expected the size of subsampled database to be "
-            "equal to number of smiles * sampling ratio",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to be Molecule object",
-            )
-        print(f"Test complete. Deleting file {xl_fpath}...")
-        remove(xl_fpath)
-
-    def test_set_molecule_database_w_property_from_excel(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        and molecular responses from an Excel file.
-
-        """
-        properties = np.random.normal(size=len(self.test_smiles))
-        xl_fpath = self.smiles_seq_to_xl_or_csv(ftype="excel", property_seq=properties)
-        molecule_set = MoleculeSet(
-            molecule_database_src=xl_fpath,
-            molecule_database_src_type="excel",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from excel file",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number "
-            "of smiles in excel file",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smiles[id],
-                "Expected mol_text attribute of Molecule object "
-                "to be smiles when names not present in excel",
-            )
-            self.assertAlmostEqual(
-                molecule.mol_property_val,
-                properties[id],
-                places=7,
-                msg="Expected mol_property_val of"
-                "Molecule object "
-                "to be set to value in excel file",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to be Molecule object",
-            )
-            print(f"Test complete. Deleting file {xl_fpath}...")
-        remove(xl_fpath)
-
-    def test_set_molecule_database_w_descriptor_property_from_excel(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        containing arbitrary molecular descriptor values from an Excel file.
-
-        """
-        properties = np.random.normal(size=len(self.test_smiles))
-        n_features = 20
-        features = np.random.normal(size=(len(self.test_smiles), n_features))
-        xl_fpath = self.smiles_seq_to_xl_or_csv(
-            ftype="excel", property_seq=properties, feature_arr=features
-        )
-        molecule_set = MoleculeSet(
-            molecule_database_src=xl_fpath,
-            molecule_database_src_type="excel",
-            similarity_measure="l0_similarity",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from " "excel file",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number "
-            "of smiles in excel file",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smiles[id],
-                "Expected mol_text attribute of Molecule object "
-                "to be smiles when names not present in excel",
-            )
-            self.assertAlmostEqual(
-                molecule.mol_property_val,
-                properties[id],
-                places=7,
-                msg="Expected mol_property_val of"
-                "Molecule object "
-                "to be set to value in excel file",
-            )
-            self.assertTrue(
-                (molecule.descriptor.to_numpy() == features[id]).all,
-                "Expected descriptor value to be same as the "
-                "vector used to initialize descriptor",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to " "be Molecule object",
-            )
-            print(f"Test complete. Deleting file {xl_fpath}...")
-        remove(xl_fpath)
-
-    def test_set_molecule_database_from_csv(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        and molecular responses from a CSV file.
-
-        """
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from " "csv file",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number " "of smiles",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smiles[id],
-                "Expected mol_text attribute of Molecule object "
-                "to be smiles when names not present in csv",
-            )
-            self.assertIsNone(
-                molecule.mol_property_val,
-                "Expected mol_property_val of Molecule object"
-                "initialized without property to be None",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to be Molecule object",
-            )
-        print(f"Test complete. Deleting file {csv_fpath}...")
-        remove(csv_fpath)
-
-    def test_subsample_molecule_database_from_csv(self):
-        """
-        Test to randomly subsample a molecule database loaded from an
-        CSV file.
-
-        """
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
-        sampling_ratio = 0.5
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            sampling_ratio=sampling_ratio,
-            is_verbose=True,
-        )
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from csv file",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            int(sampling_ratio * len(self.test_smiles)),
-            "Expected the size of database to be equal to number "
-            "of smiles * sampling_ratio",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to be Molecule object",
-            )
-        print(f"Test complete. Deleting file {csv_fpath}...")
-        remove(csv_fpath)
-
-    def test_set_molecule_database_w_property_from_csv(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        and molecular responses from a CSV file.
-
-        """
-        properties = np.random.normal(size=len(self.test_smiles))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from csv file",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smiles[id],
-                "Expected mol_text attribute of Molecule object "
-                "to be smiles when names not present in csv",
-            )
-            self.assertAlmostEqual(
-                molecule.mol_property_val,
-                properties[id],
-                places=7,
-                msg="Expected mol_property_val of"
-                "Molecule object "
-                "to be set to value in csv file",
-            )
-            self.assertIsInstance(molecule, Molecule)
-        print(f"Test complete. Deleting file {csv_fpath}...")
-        remove(csv_fpath)
-
-    def test_set_molecule_database_w_descriptor_property_from_csv(self):
-        """
-        Test to create MoleculeSet object by reading molecule database
-        containing arbitrary molecular descriptors and molecular responses
-        from a CSV file.
-
-        """
-        properties = np.random.normal(size=len(self.test_smiles))
-        n_features = 20
-        features = np.random.normal(size=(len(self.test_smiles), n_features))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(
-            ftype="csv", property_seq=properties, feature_arr=features
-        )
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            similarity_measure="l0_similarity",
-            is_verbose=True,
-        )
-        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
-        self.assertIsNotNone(
-            molecule_set.molecule_database,
-            "Expected molecule_database to be set from " "excel file",
-        )
-        self.assertEqual(
-            len(molecule_set.molecule_database),
-            len(self.test_smiles),
-            "Expected the size of database to be equal to number "
-            "of smiles in csv file",
-        )
-        for id, molecule in enumerate(molecule_set.molecule_database):
-            self.assertEqual(
-                molecule.mol_text,
-                self.test_smiles[id],
-                "Expected mol_text attribute of Molecule object "
-                "to be smiles when names not present in csv",
-            )
-            self.assertAlmostEqual(
-                molecule.mol_property_val,
-                properties[id],
-                places=7,
-                msg="Expected mol_property_val of"
-                "Molecule object "
-                "to be set to value in csv file",
-            )
-            self.assertTrue(
-                (molecule.descriptor.to_numpy() == features[id]).all,
-                "Expected descriptor value to be same as the "
-                "vector used to initialize descriptor",
-            )
-            self.assertIsInstance(
-                molecule,
-                Molecule,
-                "Expected member of molecule_set to be Molecule object",
-            )
-        print(f"Test complete. Deleting file {csv_fpath}...")
-        remove(csv_fpath)
-
-    def test_set_molecule_database_w_similarity_from_csv(self):
-        """
-        Verify that a NotInitializedError is raised if no fingerprint_type
-        is specified when instantiating a MoleculeSet object.
-
-        """
-        properties = np.random.normal(size=len(self.test_smiles))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
-        for similarity_measure in SUPPORTED_SIMILARITIES:
-            with self.assertRaises(NotInitializedError):
-                MoleculeSet(
-                    molecule_database_src=csv_fpath,
-                    molecule_database_src_type="csv",
-                    similarity_measure=similarity_measure,
-                    is_verbose=False,
-                )
-
-        print(f"Test complete. Deleting file {csv_fpath}...")
-        remove(csv_fpath)
-
-    def test_set_molecule_database_fingerprint_from_csv(self):
-        """
-        Verify that a TypeError is raised if no similarity_measure
-        is specified when instantiating a MoleculeSet object.
-
-        """
-        properties = np.random.normal(size=len(self.test_smiles))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
-        for descriptor in SUPPORTED_FPRINTS:
-            with self.assertRaises(TypeError):
-                MoleculeSet(
-                    molecule_database_src=csv_fpath,
-                    molecule_database_src_type="csv",
-                    fingerprint_type=descriptor,
-                    is_verbose=False,
-                )
-
-        print(f"Test complete. Deleting file {csv_fpath}...")
-        remove(csv_fpath)
-
-    def test_set_molecule_database_w_fingerprint_similarity_from_csv(self):
-        """
-        Test all combinations of fingerprints and similarity measures with the
-        MoleculeSet class.
-
-        """
-        properties = np.random.normal(size=len(self.test_smiles))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
-        for descriptor in SUPPORTED_FPRINTS:
-            for similarity_measure in SUPPORTED_SIMILARITIES:
-                molecule_set = MoleculeSet(
-                    molecule_database_src=csv_fpath,
-                    molecule_database_src_type="csv",
-                    fingerprint_type=descriptor,
-                    similarity_measure=similarity_measure,
-                    is_verbose=False,
-                )
-                self.assertFalse(
-                    molecule_set.is_verbose, "Expected is_verbose to be False"
-                )
-                self.assertIsNotNone(
-                    molecule_set.molecule_database,
-                    "Expected molecule_database to be set from csv file",
-                )
-                for molecule in molecule_set.molecule_database:
-                    self.assertTrue(
-                        molecule.descriptor.check_init(),
-                        "Expected descriptor to be set",
-                    )
-                self.assertIsNotNone(
-                    molecule_set.similarity_matrix,
-                    "Expected similarity_matrix to be set",
-                )
-        print(f"Test complete. Deleting file {csv_fpath}...")
-        remove(csv_fpath)
-
-    def test_get_most_similar_pairs(self):
-        """
-        Test that all combinations of fingerprint_type and similarity measure
-        works with the MoleculeSet.get_most_similar_pairs() method.
-
-        """
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
-        for descriptor in SUPPORTED_FPRINTS:
-            for similarity_measure in SUPPORTED_SIMILARITIES:
-                molecule_set = MoleculeSet(
-                    molecule_database_src=csv_fpath,
-                    molecule_database_src_type="csv",
-                    fingerprint_type=descriptor,
-                    similarity_measure=similarity_measure,
-                    is_verbose=False,
-                )
-                molecule_pairs = molecule_set.get_most_similar_pairs()
-                self.assertIsInstance(
-                    molecule_pairs,
-                    list,
-                    "Expected get_most_similar_pairs() to return list",
-                )
-                for pair in molecule_pairs:
-                    self.assertIsInstance(
-                        pair,
-                        tuple,
-                        "Expected elements of list "
-                        "returned by get_most_similar_pairs()"
-                        " to be tuples",
-                    )
-        remove(csv_fpath)
-
-    def test_get_most_dissimilar_pairs(self):
-        """
-        Test that all combinations of fingerprint_type and similarity measure
-        works with the MoleculeSet.get_most_dissimilar_pairs() method.
-
-        """
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
-        for descriptor in SUPPORTED_FPRINTS:
-            for similarity_measure in SUPPORTED_SIMILARITIES:
-                molecule_set = MoleculeSet(
-                    molecule_database_src=csv_fpath,
-                    molecule_database_src_type="csv",
-                    fingerprint_type=descriptor,
-                    similarity_measure=similarity_measure,
-                    is_verbose=False,
-                )
-                molecule_pairs = molecule_set.get_most_dissimilar_pairs()
-                self.assertIsInstance(
-                    molecule_pairs,
-                    list,
-                    "Expected get_most_dissimilar_pairs() " "to return list",
-                )
-                for pair in molecule_pairs:
-                    self.assertIsInstance(
-                        pair,
-                        tuple,
-                        "Expected elements of list returned"
-                        " by get_most_dissimilar_pairs() "
-                        "to be tuples",
-                    )
-        remove(csv_fpath)
-
-    def test_pca_transform(self):
-        """
-        Test the unsupervised transformation of molecules in
-        MoleculSet using Principal Component Analysis.
-
-        """
-        n_features = 20
-        features = np.random.normal(size=(len(self.test_smiles), n_features))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            similarity_measure="l0_similarity",
-            is_verbose=True,
-        )
-        features = StandardScaler().fit_transform(features)
-        features = PCA(n_components=2).fit_transform(features)
-        error_matrix = features - molecule_set.get_transformed_descriptors()
-        error_threshold = 1e-6
-        self.assertLessEqual(
-            error_matrix.min(),
-            error_threshold,
-            "Expected transformed molecular descriptors to be "
-            "equal to PCA decomposed features",
-        )
-        remove(csv_fpath)
-
-    def test_mds_transform(self):
-        """
-        Test the unsupervised transformation of molecules in
-        MoleculSet using MDS.
-
-        """
-        n_features = 20
-        features = np.random.normal(size=(len(self.test_smiles), n_features))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            similarity_measure="l0_similarity",
-            is_verbose=True,
-        )
-        features = StandardScaler().fit_transform(features)
-        features = MDS().fit_transform(features)
-        error_matrix = features - molecule_set.get_transformed_descriptors(
-            method_="mds"
-        )
-        error_threshold = 1e-6
-        self.assertLessEqual(
-            error_matrix.min(),
-            error_threshold,
-            "Expected transformed molecular descriptors to be "
-            "equal to MDS decomposed features",
-        )
-        remove(csv_fpath)
-
-    def test_tsne_transform(self):
-        """
-        Test the unsupervised transformation of molecules in
-        MoleculSet using TSNE.
-
-        """
-        n_features = 20
-        features = np.random.normal(size=(len(self.test_smiles), n_features))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            similarity_measure="l0_similarity",
-            is_verbose=True,
-        )
-        features = StandardScaler().fit_transform(features)
-        features = TSNE(perplexity=len(self.test_smiles) / 2).fit_transform(features)
-        error_matrix = features - molecule_set.get_transformed_descriptors(
-            method_="tsne",
-            perplexity=1,
-        )
-        error_threshold = 1e-6
-        self.assertLessEqual(
-            error_matrix.min(),
-            error_threshold,
-            "Expected transformed molecular descriptors to be "
-            "equal to TSNE decomposed features",
-        )
-        remove(csv_fpath)
-
-    def test_isomap_transform(self):
-        """
-        Test the unsupervised transformation of molecules in
-        MoleculSet using Isomap.
-
-        """
-        n_features = 20
-        features = np.random.normal(size=(len(self.test_smiles), n_features))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            similarity_measure="l0_similarity",
-            is_verbose=True,
-        )
-        features = StandardScaler().fit_transform(features)
-        features = Isomap().fit_transform(features)
-        error_matrix = features - molecule_set.get_transformed_descriptors(
-            method_="isomap"
-        )
-        error_threshold = 1e-6
-        self.assertLessEqual(
-            error_matrix.min(),
-            error_threshold,
-            "Expected transformed molecular descriptors to be "
-            "equal to Isomap decomposed features",
-        )
-        remove(csv_fpath)
-
-    def test_spectral_embedding_transform(self):
-        """
-        Test the unsupervised transformation of molecules in
-        MoleculSet using Isomap.
-
-        """
-        n_features = 20
-        features = np.random.normal(size=(len(self.test_smiles), n_features))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            similarity_measure="l0_similarity",
-            is_verbose=True,
-        )
-        features = StandardScaler().fit_transform(features)
-        features = SpectralEmbedding().fit_transform(features)
-        error_matrix = features - molecule_set.get_transformed_descriptors(
-            method_="spectral_embedding"
-        )
-        error_threshold = 1e-6
-        self.assertLessEqual(
-            error_matrix.min(),
-            error_threshold,
-            "Expected transformed molecular descriptors to be "
-            "equal to SpectralEmbedding decomposed features",
-        )
-        remove(csv_fpath)
-
-    def test_invalid_transform_error(self):
-        """Using an invalid or unimplemented dimensionality reduction method
-        should throw an error.
-        """
-        n_features = 20
-        features = np.random.normal(size=(len(self.test_smiles), n_features))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            similarity_measure="l0_similarity",
-            is_verbose=True,
-        )
-        features = StandardScaler().fit_transform(features)
-        features = TSNE(perplexity=len(self.test_smiles) / 2).fit_transform(features)
-        with self.assertRaises(InvalidConfigurationError):
-            error_matrix = features - molecule_set.get_transformed_descriptors(
-                method_="not a real method"
-            )
-        remove(csv_fpath)
-
-    def test_clustering_fingerprints(self):
-        """
-        Test the clustering of molecules featurized by their fingerprints.
-
-        """
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
-        n_clusters = 3
-        for descriptor in SUPPORTED_FPRINTS:
-            for similarity_measure in SUPPORTED_SIMILARITIES:
-                molecule_set = MoleculeSet(
-                    molecule_database_src=csv_fpath,
-                    molecule_database_src_type="csv",
-                    fingerprint_type=descriptor,
-                    similarity_measure=similarity_measure,
-                    is_verbose=True,
-                )
-                with self.assertRaises(NotInitializedError):
-                    molecule_set.get_cluster_labels()
-                if molecule_set.similarity_measure.is_distance_metric():
-                    molecule_set.cluster(n_clusters=n_clusters)
-                    self.assertLessEqual(
-                        len(set(molecule_set.get_cluster_labels())),
-                        n_clusters,
-                        "Expected number of cluster labels to be "
-                        "less than equal to number of clusters",
-                    )
-                    if molecule_set.similarity_measure.type_ == "continuous":
-                        self.assertEqual(
-                            str(molecule_set.clusters_),
-                            "kmedoids",
-                            f"Expected kmedoids clustering for "
-                            f"similarity: {similarity_measure}",
-                        )
-                    else:
-                        self.assertEqual(
-                            str(molecule_set.clusters_),
-                            "complete_linkage",
-                            f"Expected complete_linkage clustering"
-                            f"for similarity: {similarity_measure}",
-                        )
-                else:
-                    with self.assertRaises(InvalidConfigurationError):
-                        molecule_set.cluster(n_clusters=n_clusters)
-        remove(csv_fpath)
-
-    def test_molecule_set_getters(self):
-        """Retrieve names and properties of mols using MoleculeSet."""
-        properties = np.random.normal(size=len(self.test_smiles))
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-
-        self.assertListEqual(self.test_smiles, molecule_set.get_mol_names().tolist())
-
-        for a, b in zip(
-            properties.tolist(), molecule_set.get_mol_properties().tolist()
-        ):
-            self.assertAlmostEqual(a, b)
-        remove(csv_fpath)
-
-    def test_molecule_set_sim_getters(self):
-        """Get the properties for most and least similar molecule pairs."""
-        properties = np.array([i for i in range(len(self.test_smiles))])
-        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
-        molecule_set = MoleculeSet(
-            molecule_database_src=csv_fpath,
-            molecule_database_src_type="csv",
-            fingerprint_type="morgan_fingerprint",
-            similarity_measure="tanimoto",
-            is_verbose=True,
-        )
-        _, ref_props = molecule_set.get_property_of_most_dissimilar()
-        self.assertListEqual(ref_props, [5, 5, 5, 5, 5, 0, 7, 0])
-
-        _, ref_props = molecule_set.get_property_of_most_similar()
-        self.assertListEqual(ref_props, [1, 2, 1, 4, 3, 6, 5, 3])
-
-        remove(csv_fpath)
-
-
-if __name__ == "__main__":
-    unittest.main()
+"""Test the MoleculeSet class."""
+from os import remove, mkdir
+import os.path
+from shutil import rmtree
+import unittest
+
+import numpy as np
+import pandas as pd
+from rdkit.Chem import MolFromSmiles
+from rdkit.Chem.rdmolfiles import MolToPDBFile
+from sklearn.decomposition import PCA
+from sklearn.manifold import MDS, TSNE, Isomap, SpectralEmbedding
+from sklearn.preprocessing import StandardScaler
+
+from aimsim.chemical_datastructures import Molecule, MoleculeSet
+from aimsim.ops import Descriptor, SimilarityMeasure
+from aimsim.exceptions import NotInitializedError, InvalidConfigurationError
+
+
+SUPPORTED_SIMILARITIES = SimilarityMeasure.get_supported_metrics()
+
+SUPPORTED_FPRINTS = Descriptor.get_supported_fprints()
+
+
+class TestMoleculeSet(unittest.TestCase):
+    test_smarts = [
+        "[CH3:1][S:2][c:3]1[cH:4][cH:5][c:6]([B:7]([OH:8])[OH:9])[cH:10][cH:11]1",
+        "[NH:1]1[CH2:2][CH2:3][O:4][CH2:5][CH2:6]1.[O:7]=[S:8]=[O:9]",
+    ]
+
+    test_smiles = [
+        "CCCCCCC",
+        "CCCC",
+        "CCC",
+        "CO",
+        "CN",
+        "C1=CC=CC=C1",
+        "CC1=CC=CC=C1",
+        "C(=O)(N)N",
+    ]
+
+    def get_feature_set(self, dimensionality=10):
+        n_test_mols = len(self.test_smiles)
+        test_feature_set = []
+        feature_value_upper_limit = 1000
+        for i in range(n_test_mols):
+            test_feature_set.append(
+                [
+                    np.random.random() * feature_value_upper_limit
+                    for _ in range(dimensionality)
+                ]
+            )
+        return np.array(test_feature_set)
+
+    def smiles_seq_to_textfile(self, property_seq=None):
+        """Helper method to convert a SMILES sequence to a text file.
+
+        Args:
+            property_seq (list or np.ndarray, optional): Optional sequence of
+                molecular responses.. Defaults to None.
+
+        Returns:
+            str: Path to created file.
+        """
+        text_fpath = "temp_smiles_seq.txt"
+        print(f"Creating text file {text_fpath}")
+        with open(text_fpath, "w") as fp:
+            for id, smiles in enumerate(self.test_smiles):
+                write_txt = smiles
+                if property_seq is not None:
+                    write_txt += " " + str(property_seq[id])
+                if id < len(self.test_smiles) - 1:
+                    write_txt += "\n"
+
+                fp.write(write_txt)
+        return text_fpath
+
+    def smiles_seq_to_smi_file(self, property_seq=None):
+        """Helper method to convert a SMILES sequence to a .smi file.
+
+        Args:
+            property_seq (list or np.ndarray, optional): Optional sequence of
+                molecular responses. Defaults to None.
+
+        Returns:
+            str: Path to created file.
+        """
+        smi_fpath = "temp_smiles_seq.smi"
+        print(f"Creating text file {smi_fpath}")
+        with open(smi_fpath, "w") as fp:
+            for id, smiles in enumerate(self.test_smiles):
+                write_txt = smiles
+                if property_seq is not None:
+                    write_txt += " " + str(property_seq[id])
+                if id < len(self.test_smiles) - 1:
+                    write_txt += "\n"
+
+                fp.write(write_txt)
+        return smi_fpath
+
+    def smiles_seq_to_smiles_file(self, property_seq=None):
+        """Helper method to convert a SMILES sequence to a .SMILES file.
+
+        Args:
+            property_seq (list or np.ndarray, optional): Optional sequence of
+                molecular responses. Defaults to None.
+
+        Returns:
+            str: Path to created file.
+        """
+        SMILES_fpath = "temp_smiles_seq.SMILES"
+        print(f"Creating text file {SMILES_fpath}")
+        with open(SMILES_fpath, "w") as fp:
+            for id, smiles in enumerate(self.test_smiles):
+                write_txt = smiles
+                if property_seq is not None:
+                    write_txt += " " + str(property_seq[id])
+                if id < len(self.test_smiles) - 1:
+                    write_txt += "\n"
+
+                fp.write(write_txt)
+        return SMILES_fpath
+
+    def smarts_seq_to_smiles_file(self, property_seq=None):
+        """Helper method to convert a SMARTS sequence to a .SMILES file.
+
+        Args:
+            property_seq (list or np.ndarray, optional): Optional sequence of
+                molecular responses. Defaults to None.
+
+        Returns:
+            str: Path to created file.
+        """
+        SMILES_fpath = "temp_smiles_seq.SMILES"
+        print(f"Creating text file {SMILES_fpath}")
+        with open(SMILES_fpath, "w") as fp:
+            for id, smiles in enumerate(self.test_smarts):
+                write_txt = smiles
+                if property_seq is not None:
+                    write_txt += " " + str(property_seq[id])
+                if id < len(self.test_smiles) - 1:
+                    write_txt += "\n"
+
+                fp.write(write_txt)
+        return SMILES_fpath
+
+    def smiles_seq_to_pdb_dir(self, property_seq=None):
+        """Helper method to convert a SMILES sequence to a pdb files
+        stored in a directory.
+
+        Args:
+            property_seq (list or np.ndarray, optional): Optional sequence of
+                molecular responses. Defaults to None.
+
+        Returns:
+            str: Path to created directory.
+        """
+        dir_path = "test_dir"
+        if not os.path.isdir(dir_path):
+            print(f"Creating directory {dir_path}")
+            mkdir(dir_path)
+        for smiles_str in self.test_smiles:
+            mol_graph = MolFromSmiles(smiles_str)
+            assert mol_graph is not None
+            pdb_fpath = os.path.join(dir_path, smiles_str + ".pdb")
+            print(f"Creating file {pdb_fpath}")
+            MolToPDBFile(mol_graph, pdb_fpath)
+        return dir_path
+
+    def smiles_seq_to_xl_or_csv(
+        self, ftype, property_seq=None, name_seq=None, feature_arr=None
+    ):
+        """Helper method to convert a SMILES sequence or arbitrary features
+        to Excel or CSV files.
+
+        Args:
+            ftype (str): String label to denote the filetype. 'csv' or 'excel'.
+            property_seq (list or np.ndarray, optional): Optional sequence of
+                molecular responses. Defaults to None.
+            name_seq (list or np.ndarray, optional): Optional sequence of
+                molecular names. Defaults to None.
+            feature_arr (np.ndarray, optional): Optional array of molecular
+                descriptor values. Defaults to None.
+
+        Raises:
+            ValueError: Invalid file type specified.
+
+        Returns:
+            str: Path to created file.
+        """
+        data = {"descriptor_smiles": self.test_smiles}
+        if property_seq is not None:
+            data.update({"response_random": property_seq})
+        if name_seq is not None:
+            data.update({"descriptor_name": name_seq})
+        if feature_arr is not None:
+            feature_arr = np.array(feature_arr)
+            for feature_num in range(feature_arr.shape[1]):
+                data.update({f"descriptor_{feature_num}": feature_arr[:, feature_num]})
+        data_df = pd.DataFrame(data)
+        fpath = "temp_mol_file"
+        if ftype == "excel":
+            fpath += ".xlsx"
+            print(f"Creating {ftype} file {fpath}")
+            data_df.to_excel(fpath)
+        elif ftype == "csv":
+            fpath += ".csv"
+            print(f"Creating {ftype} file {fpath}")
+            data_df.to_csv(fpath)
+        else:
+            raise ValueError(f"{ftype} not supported")
+        return fpath
+
+    def test_set_molecule_database_from_textfile(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        from a textfile.
+
+        """
+        text_fpath = self.smiles_seq_to_textfile()
+        molecule_set = MoleculeSet(
+            molecule_database_src=text_fpath,
+            molecule_database_src_type="text",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from text",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number "
+            "of smiles in text file",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smiles[id],
+                "Expected mol_text attribute of Molecule object to be smiles",
+            )
+            self.assertIsNone(
+                molecule.mol_property_val,
+                "Expected mol_property_val of Molecule object "
+                "initialized without property to be None",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to " "be Molecule object",
+            )
+        print(f"Test complete. Deleting file {text_fpath}...")
+        remove(text_fpath)
+
+    def test_set_molecule_database_from_smi_file(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        from a smi file.
+
+        """
+        text_fpath = self.smiles_seq_to_smi_file()
+        molecule_set = MoleculeSet(
+            molecule_database_src=text_fpath,
+            molecule_database_src_type="text",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from text",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number "
+            "of smiles in text file",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smiles[id],
+                "Expected mol_text attribute of Molecule object to be smiles",
+            )
+            self.assertIsNone(
+                molecule.mol_property_val,
+                "Expected mol_property_val of Molecule object "
+                "initialized without property to be None",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to " "be Molecule object",
+            )
+        print(f"Test complete. Deleting file {text_fpath}...")
+        remove(text_fpath)
+
+    def test_set_molecule_database_from_smiles_file(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        from a SMILES file.
+
+        """
+        text_fpath = self.smiles_seq_to_smiles_file()
+        molecule_set = MoleculeSet(
+            molecule_database_src=text_fpath,
+            molecule_database_src_type="text",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from text",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number "
+            "of smiles in text file",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smiles[id],
+                "Expected mol_text attribute of Molecule object to be smiles",
+            )
+            self.assertIsNone(
+                molecule.mol_property_val,
+                "Expected mol_property_val of Molecule object "
+                "initialized without property to be None",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to " "be Molecule object",
+            )
+        print(f"Test complete. Deleting file {text_fpath}...")
+        remove(text_fpath)
+
+    def test_set_molecule_database_from_smarts_file(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        from a SMILES file containing SMARTS strings.
+
+        """
+        text_fpath = self.smarts_seq_to_smiles_file()
+        molecule_set = MoleculeSet(
+            molecule_database_src=text_fpath,
+            molecule_database_src_type="text",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from text",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smarts),
+            "Expected the size of database to be equal to number "
+            "of smiles in text file",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smarts[id],
+                "Expected mol_text attribute of Molecule object to be smiles",
+            )
+            self.assertIsNone(
+                molecule.mol_property_val,
+                "Expected mol_property_val of Molecule object "
+                "initialized without property to be None",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to " "be Molecule object",
+            )
+        print(f"Test complete. Deleting file {text_fpath}...")
+        remove(text_fpath)
+
+    def test_subsample_molecule_database_from_textfile(self):
+        """
+        Test to randomly subsample a molecule database loaded from a textfile.
+
+        """
+        text_fpath = self.smiles_seq_to_textfile()
+        sampling_ratio = 0.5
+        molecule_set = MoleculeSet(
+            molecule_database_src=text_fpath,
+            molecule_database_src_type="text",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+            sampling_ratio=sampling_ratio,
+        )
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from text",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            int(sampling_ratio * len(self.test_smiles)),
+            "Expected the size of subsampled database to be equal "
+            "to number of smiles in text file * sampling_ratio",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to " "be Molecule object",
+            )
+        print(f"Test complete. Deleting file {text_fpath}...")
+        remove(text_fpath)
+
+    def test_set_molecule_database_w_property_from_textfile(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        and molecular responses from a textfile.
+
+        """
+        properties = np.random.normal(size=len(self.test_smiles))
+        text_fpath = self.smiles_seq_to_textfile(property_seq=properties)
+        molecule_set = MoleculeSet(
+            molecule_database_src=text_fpath,
+            molecule_database_src_type="text",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from text",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number "
+            "of smiles in text file",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smiles[id],
+                "Expected mol_text attribute of Molecule object " "to be smiles",
+            )
+            self.assertAlmostEqual(
+                molecule.mol_property_val,
+                properties[id],
+                places=7,
+                msg="Expected mol_property_val of"
+                "Molecule object "
+                "to be set to value in text file",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to " "be Molecule object",
+            )
+        print(f"Test complete. Deleting file {text_fpath}...")
+        remove(text_fpath)
+
+    def test_set_molecule_database_from_pdb_dir(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        from a directory of pdb files.
+
+        """
+        dir_path = self.smiles_seq_to_pdb_dir(self.test_smiles)
+        molecule_set = MoleculeSet(
+            molecule_database_src=dir_path,
+            molecule_database_src_type="directory",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from dir",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number " "of files in dir",
+        )
+        for molecule in molecule_set.molecule_database:
+            self.assertIn(
+                molecule.mol_text,
+                self.test_smiles,
+                "Expected molecule text to be a smiles string",
+            )
+            self.assertIsNone(
+                molecule.mol_property_val,
+                "Expected mol_property_val of Molecule object"
+                "initialized without property to be None",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to " "be Molecule object",
+            )
+        print(f"Test complete. Deleting directory {dir_path}...")
+        rmtree(dir_path)
+
+    def test_subsample_molecule_database_from_pdb_dir(self):
+        """
+        Test to randomly subsample a molecule database loaded from a
+        directory of pdb files.
+
+        """
+        dir_path = self.smiles_seq_to_pdb_dir(self.test_smiles)
+        sampling_ratio = 0.5
+        molecule_set = MoleculeSet(
+            molecule_database_src=dir_path,
+            molecule_database_src_type="directory",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+            sampling_ratio=sampling_ratio,
+        )
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from dir",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            int(sampling_ratio * len(self.test_smiles)),
+            "Expected the size of subsampled database to be "
+            "equal to number of files in dir * sampling_ratio",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to " "be Molecule object",
+            )
+        print(f"Test complete. Deleting directory {dir_path}...")
+        rmtree(dir_path)
+
+    def test_set_molecule_database_from_excel(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        from an Excel file.
+
+        """
+        xl_fpath = self.smiles_seq_to_xl_or_csv(ftype="excel")
+        molecule_set = MoleculeSet(
+            molecule_database_src=xl_fpath,
+            molecule_database_src_type="excel",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from excel file",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number of smiles",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smiles[id],
+                "Expected mol_text attribute of Molecule object "
+                "to be smiles when names not present in excel",
+            )
+            self.assertIsNone(
+                molecule.mol_property_val,
+                "Expected mol_property_val of Molecule object"
+                "initialized without property to be None",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to be Molecule object",
+            )
+        print(f"Test complete. Deleting file {xl_fpath}...")
+        remove(xl_fpath)
+
+    def test_set_molecule_database_from_excel_without_smiles_name(self):
+        xl_fpath = "test_files.xlsx"
+        features = self.get_feature_set()  # n_samples x dimensionality
+        data = dict()
+        for feature_id in range(features.shape[-1]):
+            data[f"descriptor_{feature_id}"] = features[:, feature_id].flatten()
+        df = pd.DataFrame(data)
+        print(f"Creating text file {xl_fpath}")
+        df.to_excel(xl_fpath)
+        molecule_set = MoleculeSet(
+            molecule_database_src=xl_fpath,
+            molecule_database_src_type="excel",
+            similarity_measure="l2_similarity",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from excel file",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number of smiles",
+        )
+        self.assertTrue(
+            np.allclose(features, molecule_set.get_mol_features(), rtol=1e-4),
+            "Expected molecule feature vectors to "
+            "be the same as features in input file",
+        )
+        with self.assertRaises(ValueError):
+            molecule_set = MoleculeSet(
+                molecule_database_src=xl_fpath,
+                molecule_database_src_type="excel",
+                fingerprint_type="morgan_fingerprint",
+                similarity_measure="l2_similarity",
+                is_verbose=True,
+            )
+        with self.assertRaises(ValueError):
+            molecule_set = MoleculeSet(
+                molecule_database_src=xl_fpath,
+                molecule_database_src_type="excel",
+                similarity_measure="tanimoto_similarity",
+                is_verbose=True,
+            )
+        print(f"Test complete. Deleting file {xl_fpath}...")
+        remove(xl_fpath)
+
+    def test_subsample_molecule_database_from_excel(self):
+        """
+        Test to randomly subsample a molecule database loaded from an
+        Excel file.
+
+        """
+        xl_fpath = self.smiles_seq_to_xl_or_csv(ftype="excel")
+        sampling_ratio = 0.5
+        molecule_set = MoleculeSet(
+            molecule_database_src=xl_fpath,
+            molecule_database_src_type="excel",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+            sampling_ratio=sampling_ratio,
+        )
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from excel file",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            int(sampling_ratio * len(self.test_smiles)),
+            "Expected the size of subsampled database to be "
+            "equal to number of smiles * sampling ratio",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to be Molecule object",
+            )
+        print(f"Test complete. Deleting file {xl_fpath}...")
+        remove(xl_fpath)
+
+    def test_set_molecule_database_w_property_from_excel(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        and molecular responses from an Excel file.
+
+        """
+        properties = np.random.normal(size=len(self.test_smiles))
+        xl_fpath = self.smiles_seq_to_xl_or_csv(ftype="excel", property_seq=properties)
+        molecule_set = MoleculeSet(
+            molecule_database_src=xl_fpath,
+            molecule_database_src_type="excel",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from excel file",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number "
+            "of smiles in excel file",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smiles[id],
+                "Expected mol_text attribute of Molecule object "
+                "to be smiles when names not present in excel",
+            )
+            self.assertAlmostEqual(
+                molecule.mol_property_val,
+                properties[id],
+                places=7,
+                msg="Expected mol_property_val of"
+                "Molecule object "
+                "to be set to value in excel file",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to be Molecule object",
+            )
+            print(f"Test complete. Deleting file {xl_fpath}...")
+        remove(xl_fpath)
+
+    def test_set_molecule_database_w_descriptor_property_from_excel(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        containing arbitrary molecular descriptor values from an Excel file.
+
+        """
+        properties = np.random.normal(size=len(self.test_smiles))
+        n_features = 20
+        features = np.random.normal(size=(len(self.test_smiles), n_features))
+        xl_fpath = self.smiles_seq_to_xl_or_csv(
+            ftype="excel", property_seq=properties, feature_arr=features
+        )
+        molecule_set = MoleculeSet(
+            molecule_database_src=xl_fpath,
+            molecule_database_src_type="excel",
+            similarity_measure="l0_similarity",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from " "excel file",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number "
+            "of smiles in excel file",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smiles[id],
+                "Expected mol_text attribute of Molecule object "
+                "to be smiles when names not present in excel",
+            )
+            self.assertAlmostEqual(
+                molecule.mol_property_val,
+                properties[id],
+                places=7,
+                msg="Expected mol_property_val of"
+                "Molecule object "
+                "to be set to value in excel file",
+            )
+            self.assertTrue(
+                (molecule.descriptor.to_numpy() == features[id]).all,
+                "Expected descriptor value to be same as the "
+                "vector used to initialize descriptor",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to " "be Molecule object",
+            )
+            print(f"Test complete. Deleting file {xl_fpath}...")
+        remove(xl_fpath)
+
+    def test_set_molecule_database_from_csv(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        and molecular responses from a CSV file.
+
+        """
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from " "csv file",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number " "of smiles",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smiles[id],
+                "Expected mol_text attribute of Molecule object "
+                "to be smiles when names not present in csv",
+            )
+            self.assertIsNone(
+                molecule.mol_property_val,
+                "Expected mol_property_val of Molecule object"
+                "initialized without property to be None",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to be Molecule object",
+            )
+        print(f"Test complete. Deleting file {csv_fpath}...")
+        remove(csv_fpath)
+
+    def test_subsample_molecule_database_from_csv(self):
+        """
+        Test to randomly subsample a molecule database loaded from an
+        CSV file.
+
+        """
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
+        sampling_ratio = 0.5
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            sampling_ratio=sampling_ratio,
+            is_verbose=True,
+        )
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from csv file",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            int(sampling_ratio * len(self.test_smiles)),
+            "Expected the size of database to be equal to number "
+            "of smiles * sampling_ratio",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to be Molecule object",
+            )
+        print(f"Test complete. Deleting file {csv_fpath}...")
+        remove(csv_fpath)
+
+    def test_set_molecule_database_w_property_from_csv(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        and molecular responses from a CSV file.
+
+        """
+        properties = np.random.normal(size=len(self.test_smiles))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from csv file",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smiles[id],
+                "Expected mol_text attribute of Molecule object "
+                "to be smiles when names not present in csv",
+            )
+            self.assertAlmostEqual(
+                molecule.mol_property_val,
+                properties[id],
+                places=7,
+                msg="Expected mol_property_val of"
+                "Molecule object "
+                "to be set to value in csv file",
+            )
+            self.assertIsInstance(molecule, Molecule)
+        print(f"Test complete. Deleting file {csv_fpath}...")
+        remove(csv_fpath)
+
+    def test_set_molecule_database_w_descriptor_property_from_csv(self):
+        """
+        Test to create MoleculeSet object by reading molecule database
+        containing arbitrary molecular descriptors and molecular responses
+        from a CSV file.
+
+        """
+        properties = np.random.normal(size=len(self.test_smiles))
+        n_features = 20
+        features = np.random.normal(size=(len(self.test_smiles), n_features))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(
+            ftype="csv", property_seq=properties, feature_arr=features
+        )
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            similarity_measure="l0_similarity",
+            is_verbose=True,
+        )
+        self.assertTrue(molecule_set.is_verbose, "Expected is_verbose to be True")
+        self.assertIsNotNone(
+            molecule_set.molecule_database,
+            "Expected molecule_database to be set from " "excel file",
+        )
+        self.assertEqual(
+            len(molecule_set.molecule_database),
+            len(self.test_smiles),
+            "Expected the size of database to be equal to number "
+            "of smiles in csv file",
+        )
+        for id, molecule in enumerate(molecule_set.molecule_database):
+            self.assertEqual(
+                molecule.mol_text,
+                self.test_smiles[id],
+                "Expected mol_text attribute of Molecule object "
+                "to be smiles when names not present in csv",
+            )
+            self.assertAlmostEqual(
+                molecule.mol_property_val,
+                properties[id],
+                places=7,
+                msg="Expected mol_property_val of"
+                "Molecule object "
+                "to be set to value in csv file",
+            )
+            self.assertTrue(
+                (molecule.descriptor.to_numpy() == features[id]).all,
+                "Expected descriptor value to be same as the "
+                "vector used to initialize descriptor",
+            )
+            self.assertIsInstance(
+                molecule,
+                Molecule,
+                "Expected member of molecule_set to be Molecule object",
+            )
+        print(f"Test complete. Deleting file {csv_fpath}...")
+        remove(csv_fpath)
+
+    def test_set_molecule_database_w_similarity_from_csv(self):
+        """
+        Verify that a NotInitializedError is raised if no fingerprint_type
+        is specified when instantiating a MoleculeSet object.
+
+        """
+        properties = np.random.normal(size=len(self.test_smiles))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
+        for similarity_measure in SUPPORTED_SIMILARITIES:
+            with self.assertRaises(NotInitializedError):
+                MoleculeSet(
+                    molecule_database_src=csv_fpath,
+                    molecule_database_src_type="csv",
+                    similarity_measure=similarity_measure,
+                    is_verbose=False,
+                )
+
+        print(f"Test complete. Deleting file {csv_fpath}...")
+        remove(csv_fpath)
+
+    def test_set_molecule_database_fingerprint_from_csv(self):
+        """
+        Verify that a TypeError is raised if no similarity_measure
+        is specified when instantiating a MoleculeSet object.
+
+        """
+        properties = np.random.normal(size=len(self.test_smiles))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
+        for descriptor in SUPPORTED_FPRINTS:
+            with self.assertRaises(TypeError):
+                MoleculeSet(
+                    molecule_database_src=csv_fpath,
+                    molecule_database_src_type="csv",
+                    fingerprint_type=descriptor,
+                    is_verbose=False,
+                )
+
+        print(f"Test complete. Deleting file {csv_fpath}...")
+        remove(csv_fpath)
+
+    def test_set_molecule_database_w_fingerprint_similarity_from_csv(self):
+        """
+        Test all combinations of fingerprints and similarity measures with the
+        MoleculeSet class.
+
+        """
+        properties = np.random.normal(size=len(self.test_smiles))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
+        for descriptor in SUPPORTED_FPRINTS:
+            for similarity_measure in SUPPORTED_SIMILARITIES:
+                molecule_set = MoleculeSet(
+                    molecule_database_src=csv_fpath,
+                    molecule_database_src_type="csv",
+                    fingerprint_type=descriptor,
+                    similarity_measure=similarity_measure,
+                    is_verbose=False,
+                )
+                self.assertFalse(
+                    molecule_set.is_verbose, "Expected is_verbose to be False"
+                )
+                self.assertIsNotNone(
+                    molecule_set.molecule_database,
+                    "Expected molecule_database to be set from csv file",
+                )
+                for molecule in molecule_set.molecule_database:
+                    self.assertTrue(
+                        molecule.descriptor.check_init(),
+                        "Expected descriptor to be set",
+                    )
+                self.assertIsNotNone(
+                    molecule_set.similarity_matrix,
+                    "Expected similarity_matrix to be set",
+                )
+        print(f"Test complete. Deleting file {csv_fpath}...")
+        remove(csv_fpath)
+
+    def test_get_most_similar_pairs(self):
+        """
+        Test that all combinations of fingerprint_type and similarity measure
+        works with the MoleculeSet.get_most_similar_pairs() method.
+
+        """
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
+        for descriptor in SUPPORTED_FPRINTS:
+            for similarity_measure in SUPPORTED_SIMILARITIES:
+                molecule_set = MoleculeSet(
+                    molecule_database_src=csv_fpath,
+                    molecule_database_src_type="csv",
+                    fingerprint_type=descriptor,
+                    similarity_measure=similarity_measure,
+                    is_verbose=False,
+                )
+                molecule_pairs = molecule_set.get_most_similar_pairs()
+                self.assertIsInstance(
+                    molecule_pairs,
+                    list,
+                    "Expected get_most_similar_pairs() to return list",
+                )
+                for pair in molecule_pairs:
+                    self.assertIsInstance(
+                        pair,
+                        tuple,
+                        "Expected elements of list "
+                        "returned by get_most_similar_pairs()"
+                        " to be tuples",
+                    )
+        remove(csv_fpath)
+
+    def test_get_most_dissimilar_pairs(self):
+        """
+        Test that all combinations of fingerprint_type and similarity measure
+        works with the MoleculeSet.get_most_dissimilar_pairs() method.
+
+        """
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
+        for descriptor in SUPPORTED_FPRINTS:
+            for similarity_measure in SUPPORTED_SIMILARITIES:
+                molecule_set = MoleculeSet(
+                    molecule_database_src=csv_fpath,
+                    molecule_database_src_type="csv",
+                    fingerprint_type=descriptor,
+                    similarity_measure=similarity_measure,
+                    is_verbose=False,
+                )
+                molecule_pairs = molecule_set.get_most_dissimilar_pairs()
+                self.assertIsInstance(
+                    molecule_pairs,
+                    list,
+                    "Expected get_most_dissimilar_pairs() " "to return list",
+                )
+                for pair in molecule_pairs:
+                    self.assertIsInstance(
+                        pair,
+                        tuple,
+                        "Expected elements of list returned"
+                        " by get_most_dissimilar_pairs() "
+                        "to be tuples",
+                    )
+        remove(csv_fpath)
+
+    def test_pca_transform(self):
+        """
+        Test the unsupervised transformation of molecules in
+        MoleculSet using Principal Component Analysis.
+
+        """
+        n_features = 20
+        features = np.random.normal(size=(len(self.test_smiles), n_features))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            similarity_measure="l0_similarity",
+            is_verbose=True,
+        )
+        features = StandardScaler().fit_transform(features)
+        features = PCA(n_components=2).fit_transform(features)
+        error_matrix = features - molecule_set.get_transformed_descriptors()
+        error_threshold = 1e-6
+        self.assertLessEqual(
+            error_matrix.min(),
+            error_threshold,
+            "Expected transformed molecular descriptors to be "
+            "equal to PCA decomposed features",
+        )
+        remove(csv_fpath)
+
+    def test_mds_transform(self):
+        """
+        Test the unsupervised transformation of molecules in
+        MoleculSet using MDS.
+
+        """
+        n_features = 20
+        features = np.random.normal(size=(len(self.test_smiles), n_features))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            similarity_measure="l0_similarity",
+            is_verbose=True,
+        )
+        features = StandardScaler().fit_transform(features)
+        features = MDS().fit_transform(features)
+        error_matrix = features - molecule_set.get_transformed_descriptors(
+            method_="mds"
+        )
+        error_threshold = 1e-6
+        self.assertLessEqual(
+            error_matrix.min(),
+            error_threshold,
+            "Expected transformed molecular descriptors to be "
+            "equal to MDS decomposed features",
+        )
+        remove(csv_fpath)
+
+    def test_tsne_transform(self):
+        """
+        Test the unsupervised transformation of molecules in
+        MoleculSet using TSNE.
+
+        """
+        n_features = 20
+        features = np.random.normal(size=(len(self.test_smiles), n_features))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            similarity_measure="l0_similarity",
+            is_verbose=True,
+        )
+        features = StandardScaler().fit_transform(features)
+        features = TSNE(perplexity=len(self.test_smiles) / 2).fit_transform(features)
+        error_matrix = features - molecule_set.get_transformed_descriptors(
+            method_="tsne",
+            perplexity=1,
+        )
+        error_threshold = 1e-6
+        self.assertLessEqual(
+            error_matrix.min(),
+            error_threshold,
+            "Expected transformed molecular descriptors to be "
+            "equal to TSNE decomposed features",
+        )
+        remove(csv_fpath)
+
+    def test_isomap_transform(self):
+        """
+        Test the unsupervised transformation of molecules in
+        MoleculSet using Isomap.
+
+        """
+        n_features = 20
+        features = np.random.normal(size=(len(self.test_smiles), n_features))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            similarity_measure="l0_similarity",
+            is_verbose=True,
+        )
+        features = StandardScaler().fit_transform(features)
+        features = Isomap().fit_transform(features)
+        error_matrix = features - molecule_set.get_transformed_descriptors(
+            method_="isomap"
+        )
+        error_threshold = 1e-6
+        self.assertLessEqual(
+            error_matrix.min(),
+            error_threshold,
+            "Expected transformed molecular descriptors to be "
+            "equal to Isomap decomposed features",
+        )
+        remove(csv_fpath)
+
+    def test_spectral_embedding_transform(self):
+        """
+        Test the unsupervised transformation of molecules in
+        MoleculSet using Isomap.
+
+        """
+        n_features = 20
+        features = np.random.normal(size=(len(self.test_smiles), n_features))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            similarity_measure="l0_similarity",
+            is_verbose=True,
+        )
+        features = StandardScaler().fit_transform(features)
+        features = SpectralEmbedding().fit_transform(features)
+        error_matrix = features - molecule_set.get_transformed_descriptors(
+            method_="spectral_embedding"
+        )
+        error_threshold = 1e-6
+        self.assertLessEqual(
+            error_matrix.min(),
+            error_threshold,
+            "Expected transformed molecular descriptors to be "
+            "equal to SpectralEmbedding decomposed features",
+        )
+        remove(csv_fpath)
+
+    def test_invalid_transform_error(self):
+        """Using an invalid or unimplemented dimensionality reduction method
+        should throw an error.
+        """
+        n_features = 20
+        features = np.random.normal(size=(len(self.test_smiles), n_features))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", feature_arr=features)
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            similarity_measure="l0_similarity",
+            is_verbose=True,
+        )
+        features = StandardScaler().fit_transform(features)
+        features = TSNE(perplexity=len(self.test_smiles) / 2).fit_transform(features)
+        with self.assertRaises(InvalidConfigurationError):
+            error_matrix = features - molecule_set.get_transformed_descriptors(
+                method_="not a real method"
+            )
+        remove(csv_fpath)
+
+    def test_clustering_fingerprints(self):
+        """
+        Test the clustering of molecules featurized by their fingerprints.
+
+        """
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv")
+        n_clusters = 3
+        for descriptor in SUPPORTED_FPRINTS:
+            for similarity_measure in SUPPORTED_SIMILARITIES:
+                molecule_set = MoleculeSet(
+                    molecule_database_src=csv_fpath,
+                    molecule_database_src_type="csv",
+                    fingerprint_type=descriptor,
+                    similarity_measure=similarity_measure,
+                    is_verbose=True,
+                )
+                with self.assertRaises(NotInitializedError):
+                    molecule_set.get_cluster_labels()
+                if molecule_set.similarity_measure.is_distance_metric():
+                    molecule_set.cluster(n_clusters=n_clusters)
+                    self.assertLessEqual(
+                        len(set(molecule_set.get_cluster_labels())),
+                        n_clusters,
+                        "Expected number of cluster labels to be "
+                        "less than equal to number of clusters",
+                    )
+                    if molecule_set.similarity_measure.type_ == "continuous":
+                        self.assertEqual(
+                            str(molecule_set.clusters_),
+                            "kmedoids",
+                            f"Expected kmedoids clustering for "
+                            f"similarity: {similarity_measure}",
+                        )
+                    else:
+                        self.assertEqual(
+                            str(molecule_set.clusters_),
+                            "complete_linkage",
+                            f"Expected complete_linkage clustering"
+                            f"for similarity: {similarity_measure}",
+                        )
+                else:
+                    with self.assertRaises(InvalidConfigurationError):
+                        molecule_set.cluster(n_clusters=n_clusters)
+        remove(csv_fpath)
+
+    def test_molecule_set_getters(self):
+        """Retrieve names and properties of mols using MoleculeSet."""
+        properties = np.random.normal(size=len(self.test_smiles))
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+
+        self.assertListEqual(self.test_smiles, molecule_set.get_mol_names().tolist())
+
+        for a, b in zip(
+            properties.tolist(), molecule_set.get_mol_properties().tolist()
+        ):
+            self.assertAlmostEqual(a, b)
+        remove(csv_fpath)
+
+    def test_molecule_set_sim_getters(self):
+        """Get the properties for most and least similar molecule pairs."""
+        properties = np.array([i for i in range(len(self.test_smiles))])
+        csv_fpath = self.smiles_seq_to_xl_or_csv(ftype="csv", property_seq=properties)
+        molecule_set = MoleculeSet(
+            molecule_database_src=csv_fpath,
+            molecule_database_src_type="csv",
+            fingerprint_type="morgan_fingerprint",
+            similarity_measure="tanimoto",
+            is_verbose=True,
+        )
+        _, ref_props = molecule_set.get_property_of_most_dissimilar()
+        self.assertListEqual(ref_props, [5, 5, 5, 5, 5, 0, 7, 0])
+
+        _, ref_props = molecule_set.get_property_of_most_similar()
+        self.assertListEqual(ref_props, [1, 2, 1, 4, 3, 6, 5, 3])
+
+        remove(csv_fpath)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `aimsim-2.0.2/tests/test_TaskManager.py` & `aimsim-2.0.3/tests/test_TaskManager.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-"""Test the TaskManager class."""
-from aimsim.exceptions import InvalidConfigurationError
-from aimsim.tasks.task_manager import TaskManager
-
-import unittest
-from unittest.mock import patch
-
-
-class TestTaskManager(unittest.TestCase):
-    @classmethod
-    def setUpClass(self):
-        self.test_smiles = [
-            "CCCCCCC",
-            "CCCC",
-            "CCC",
-            "CO",
-            "CN",
-            "C1=CC=CC=C1",
-            "CC1=CC=CC=C1",
-            "C(=O)(N)N",
-        ]
-
-        property_seq = [i for i in range(len(self.test_smiles))]
-        self.text_fpath = "temp_smiles_seq.txt"
-        print(f"Creating text file {self.text_fpath}")
-        with open(self.text_fpath, "w") as fp:
-            for id, smiles in enumerate(self.test_smiles):
-                write_txt = smiles
-                if property_seq is not None:
-                    write_txt += " " + str(property_seq[id])
-                if id < len(self.test_smiles) - 1:
-                    write_txt += "\n"
-
-                fp.write(write_txt)
-
-        self.tasks_dict = {}
-        self.inner_dict = {}
-        self.inner_dict["plot_settings"] = {
-            "plot_color": "green",
-            "plot_title": "Entire Dataset",
-        }
-        self.inner_dict["pairwise_heatmap_settings"] = {
-            "annotate": False,
-            "cmap": "viridis",
-        }
-        self.tasks_dict["visualize_dataset"] = self.inner_dict
-        self.tasks_dict["identify_outliers"] = {"output": "terminal"}
-        self.tasks_dict["compare_target_molecule"] = {
-            "target_molecule_smiles": "CCCC",
-            "plot_settings": {
-                "plot_color": "orange",
-                "plot_title": "Compared to Target Molecule",
-            },
-            "identify_closest_furthest": {"out_file_path": "AIMSim-ui_output.txt"},
-        }
-        self.tasks_dict["see_property_variation_w_similarity"] = {
-            "property_file": self.text_fpath,
-            "most_dissimilar": True,
-            "similarity_plot_settings": {"plot_color": "red"},
-        }
-        self.tasks_dict["cluster"] = {
-            "n_clusters": 2,
-        }
-        self.tasks_dict["invalid_test_task"] = {
-            "property_file": self.text_fpath,
-            "most_dissimilar": True,
-            "similarity_plot_settings": {"plot_color": "red"},
-        }
-
-    def test_no_tasks_task_manager(self):
-        """Instant stop test for TaskManager class.
-        """
-        with self.assertRaises(InvalidConfigurationError):
-            task_man = TaskManager(
-                {}
-            )
-
-    def test_task_manager(self):
-        """Complete run test for TaskManager class.
-        """
-        # this magical context manager sends all plots to a blank function
-        with patch("aimsim.utils.plotting_scripts.plt.show") as test_plot:
-            with patch("aimsim.utils.plotting_scripts.go.Figure.show") as test_int_plot:
-                task_man = TaskManager(
-                    tasks=self.tasks_dict
-                )
-                task_man(
-                    molecule_set_configs={
-                        'molecule_database': self.text_fpath,
-                        'molecule_database_source_type': 'text',
-                        'fingerprint_type': "morgan_fingerprint",
-                        'similarity_measure': "tanimoto",
-                        'is_verbose': False,
-                    }
-                )
-                self.assertTrue(
-                    test_plot.called or test_int_plot.called, "No plots were created.")
-
-
-if __name__ == "__main__":
-    unittest.main()
+"""Test the TaskManager class."""
+from aimsim.exceptions import InvalidConfigurationError
+from aimsim.tasks.task_manager import TaskManager
+
+import unittest
+from unittest.mock import patch
+
+
+class TestTaskManager(unittest.TestCase):
+    @classmethod
+    def setUpClass(self):
+        self.test_smiles = [
+            "CCCCCCC",
+            "CCCC",
+            "CCC",
+            "CO",
+            "CN",
+            "C1=CC=CC=C1",
+            "CC1=CC=CC=C1",
+            "C(=O)(N)N",
+        ]
+
+        property_seq = [i for i in range(len(self.test_smiles))]
+        self.text_fpath = "temp_smiles_seq.txt"
+        print(f"Creating text file {self.text_fpath}")
+        with open(self.text_fpath, "w") as fp:
+            for id, smiles in enumerate(self.test_smiles):
+                write_txt = smiles
+                if property_seq is not None:
+                    write_txt += " " + str(property_seq[id])
+                if id < len(self.test_smiles) - 1:
+                    write_txt += "\n"
+
+                fp.write(write_txt)
+
+        self.tasks_dict = {}
+        self.inner_dict = {}
+        self.inner_dict["plot_settings"] = {
+            "plot_color": "green",
+            "plot_title": "Entire Dataset",
+        }
+        self.inner_dict["pairwise_heatmap_settings"] = {
+            "annotate": False,
+            "cmap": "viridis",
+        }
+        self.tasks_dict["visualize_dataset"] = self.inner_dict
+        self.tasks_dict["identify_outliers"] = {"output": "terminal"}
+        self.tasks_dict["compare_target_molecule"] = {
+            "target_molecule_smiles": "CCCC",
+            "plot_settings": {
+                "plot_color": "orange",
+                "plot_title": "Compared to Target Molecule",
+            },
+            "identify_closest_furthest": {"out_file_path": "AIMSim-ui_output.txt"},
+        }
+        self.tasks_dict["see_property_variation_w_similarity"] = {
+            "property_file": self.text_fpath,
+            "most_dissimilar": True,
+            "similarity_plot_settings": {"plot_color": "red"},
+        }
+        self.tasks_dict["cluster"] = {
+            "n_clusters": 2,
+        }
+        self.tasks_dict["invalid_test_task"] = {
+            "property_file": self.text_fpath,
+            "most_dissimilar": True,
+            "similarity_plot_settings": {"plot_color": "red"},
+        }
+
+    def test_no_tasks_task_manager(self):
+        """Instant stop test for TaskManager class.
+        """
+        with self.assertRaises(InvalidConfigurationError):
+            task_man = TaskManager(
+                {}
+            )
+
+    def test_task_manager(self):
+        """Complete run test for TaskManager class.
+        """
+        # this magical context manager sends all plots to a blank function
+        with patch("aimsim.utils.plotting_scripts.plt.show") as test_plot:
+            with patch("aimsim.utils.plotting_scripts.go.Figure.show") as test_int_plot:
+                task_man = TaskManager(
+                    tasks=self.tasks_dict
+                )
+                task_man(
+                    molecule_set_configs={
+                        'molecule_database': self.text_fpath,
+                        'molecule_database_source_type': 'text',
+                        'fingerprint_type': "morgan_fingerprint",
+                        'similarity_measure': "tanimoto",
+                        'is_verbose': False,
+                    }
+                )
+                self.assertTrue(
+                    test_plot.called or test_int_plot.called, "No plots were created.")
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `aimsim-2.0.2/tests/test_ToolTip.py` & `aimsim-2.0.3/tests/test_ToolTip.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-""" Test the ToolTip package (and all UI packages) """
-import unittest
-
-
-class TestToolTip(unittest.TestCase):
-    """
-    Test the ToolTip package (and all UI packages) by importing them
-
-    """
-
-    def test_import(self):
-        """Attempt to import the UI app to ensure imports are correct
-        """
-        try:
-            from interfaces.UI.AIMSim_ui_main import AIMSimUiApp
-        except Exception:
-            self.fail('Unable to import AIMSim UI')
-
-
-if __name__ == "__main__":
-    unittest.main()
+""" Test the ToolTip package (and all UI packages) """
+import unittest
+
+
+class TestToolTip(unittest.TestCase):
+    """
+    Test the ToolTip package (and all UI packages) by importing them
+
+    """
+
+    def test_import(self):
+        """Attempt to import the UI app to ensure imports are correct
+        """
+        try:
+            from interfaces.UI.AIMSim_ui_main import AIMSimUiApp
+        except Exception:
+            self.fail('Unable to import AIMSim UI')
+
+
+if __name__ == "__main__":
+    unittest.main()
```

