# Comparing `tmp/trajectopy-0.1.7.tar.gz` & `tmp/trajectopy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajectopy-0.1.7.tar", last modified: Tue Jul 18 14:43:21 2023, max compression
+gzip compressed data, was "trajectopy-0.1.8.tar", max compression
```

## Comparing `trajectopy-0.1.7.tar` & `trajectopy-0.1.8.tar`

### file list

```diff
@@ -1,129 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.324335 trajectopy-0.1.7/
--rw-rw-rw-   0        0        0    35790 2023-07-17 11:38:17.000000 trajectopy-0.1.7/LICENSE
--rw-rw-rw-   0        0        0    13685 2023-07-18 14:43:21.323333 trajectopy-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    13287 2023-07-18 13:15:56.000000 trajectopy-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 14:43:21.324335 trajectopy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2526 2023-07-18 14:42:47.000000 trajectopy-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.236059 trajectopy-0.1.7/test/
--rw-rw-rw-   0        0        0     7503 2023-07-14 07:10:55.000000 trajectopy-0.1.7/test/test_alignment.py
--rw-rw-rw-   0        0        0     5569 2023-07-14 07:19:57.000000 trajectopy-0.1.7/test/test_comparison.py
--rw-rw-rw-   0        0        0     2347 2023-07-14 07:19:57.000000 trajectopy-0.1.7/test/test_settings.py
--rw-rw-rw-   0        0        0     1372 2023-07-14 07:10:55.000000 trajectopy-0.1.7/test/test_sorting.py
--rw-rw-rw-   0        0        0     6331 2023-07-14 07:10:55.000000 trajectopy-0.1.7/test/test_trajectory.py
--rw-rw-rw-   0        0        0      339 2023-07-14 07:10:55.000000 trajectopy-0.1.7/test/testdata.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.239088 trajectopy-0.1.7/trajectopy/
--rw-rw-rw-   0        0        0    35790 2023-07-17 11:38:17.000000 trajectopy-0.1.7/trajectopy/LICENSE
--rw-rw-rw-   0        0        0        0 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/__init__.py
--rw-rw-rw-   0        0        0      630 2023-07-18 14:11:40.000000 trajectopy-0.1.7/trajectopy/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.261805 trajectopy-0.1.7/trajectopy/alignment/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/alignment/__init__.py
--rw-rw-rw-   0        0        0    39680 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/alignment/alignment.py
--rw-rw-rw-   0        0        0     9340 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/alignment/data.py
--rw-rw-rw-   0        0        0     2421 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/alignment/direct_helmert_transformation.py
--rw-rw-rw-   0        0        0     5335 2023-07-18 06:46:36.000000 trajectopy-0.1.7/trajectopy/alignment/direct_leverarm.py
--rw-rw-rw-   0        0        0     2181 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/alignment/direct_timeshift.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.263804 trajectopy-0.1.7/trajectopy/alignment/functional_model/
--rw-rw-rw-   0        0        0        0 2023-07-18 14:24:36.000000 trajectopy-0.1.7/trajectopy/alignment/functional_model/__init__.py
--rw-rw-rw-   0        0        0    14944 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/alignment/functional_model/equations.py
--rw-rw-rw-   0        0        0     8022 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/alignment/functional_model/interface.py
--rw-rw-rw-   0        0        0    19324 2023-07-18 06:46:36.000000 trajectopy-0.1.7/trajectopy/alignment/parameters.py
--rw-rw-rw-   0        0        0     3910 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/alignment/util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.268807 trajectopy-0.1.7/trajectopy/approximation/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/approximation/__init__.py
--rw-rw-rw-   0        0        0     8005 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/approximation/cubic_approximation.py
--rw-rw-rw-   0        0        0     5795 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/approximation/mls_approximation.py
--rw-rw-rw-   0        0        0     5303 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/approximation/rot_approximation.py
--rw-rw-rw-   0        0        0     6116 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/approximation/trajectory_approximation.py
--rw-rw-rw-   0        0        0     4272 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/approximation/util.py
--rw-rw-rw-   0        0        0     4843 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/approximation/voxelizer.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.271807 trajectopy-0.1.7/trajectopy/evaluation/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/evaluation/__init__.py
--rw-rw-rw-   0        0        0    14610 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/evaluation/comparison.py
--rw-rw-rw-   0        0        0     4872 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/evaluation/matching.py
--rw-rw-rw-   0        0        0    29211 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/evaluation/trajectory_deviations.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.273805 trajectopy-0.1.7/trajectopy/gui/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/__init__.py
--rw-rw-rw-   0        0        0    14315 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.278806 trajectopy-0.1.7/trajectopy/gui/managers/
--rw-rw-rw-   0        0        0        0 2023-07-18 13:57:14.000000 trajectopy-0.1.7/trajectopy/gui/managers/__init__.py
--rw-rw-rw-   0        0        0     4431 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/managers/file_manager.py
--rw-rw-rw-   0        0        0     1692 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/managers/manager.py
--rw-rw-rw-   0        0        0     3827 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/managers/plot_manager.py
--rw-rw-rw-   0        0        0     3812 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/managers/session_manager.py
--rw-rw-rw-   0        0        0    31349 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/managers/trajectory_manager.py
--rw-rw-rw-   0        0        0     8040 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/managers/ui_manager.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.282805 trajectopy-0.1.7/trajectopy/gui/models/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/models/__init__.py
--rw-rw-rw-   0        0        0    11894 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/gui/models/entry.py
--rw-rw-rw-   0        0        0     1115 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/models/property_model.py
--rw-rw-rw-   0        0        0     3904 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/models/result_model.py
--rw-rw-rw-   0        0        0      977 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/models/selection.py
--rw-rw-rw-   0        0        0     4017 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/models/table_model.py
--rw-rw-rw-   0        0        0     4805 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/models/trajectory_model.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.290808 trajectopy-0.1.7/trajectopy/gui/requests/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/requests/__init__.py
--rw-rw-rw-   0        0        0      666 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/requests/file_request.py
--rw-rw-rw-   0        0        0      635 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/requests/plot_requests.py
--rw-rw-rw-   0        0        0      424 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/requests/plot_settings_request.py
--rw-rw-rw-   0        0        0      371 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/requests/property_request.py
--rw-rw-rw-   0        0        0      469 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/requests/request.py
--rw-rw-rw-   0        0        0      565 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/requests/result_model_request.py
--rw-rw-rw-   0        0        0      388 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/requests/session_request.py
--rw-rw-rw-   0        0        0     1029 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/requests/trajectory_manager_request.py
--rw-rw-rw-   0        0        0      593 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/requests/trajectory_model_request.py
--rw-rw-rw-   0        0        0      836 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/requests/ui_request.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.292809 trajectopy-0.1.7/trajectopy/gui/resources/
--rw-rw-rw-   0        0        0   120742 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/resources/full-icon-poppins.png
--rw-rw-rw-   0        0        0    24491 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/resources/icon.png
--rw-rw-rw-   0        0        0     1751 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.301810 trajectopy-0.1.7/trajectopy/gui/views/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/views/__init__.py
--rw-rw-rw-   0        0        0     3757 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/views/about_window.py
--rw-rw-rw-   0        0        0     9601 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/views/alignment_edit_window.py
--rw-rw-rw-   0        0        0    24148 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/views/plot_settings_window.py
--rw-rw-rw-   0        0        0     2483 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/views/progress_window.py
--rw-rw-rw-   0        0        0     4013 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/views/properties_window.py
--rw-rw-rw-   0        0        0     6154 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/views/result_context_menu.py
--rw-rw-rw-   0        0        0     4717 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/gui/views/result_selection_window.py
--rw-rw-rw-   0        0        0     4668 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/views/result_table_view.py
--rw-rw-rw-   0        0        0    53999 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/views/settings_window.py
--rw-rw-rw-   0        0        0    20852 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/views/trajectory_context_menu.py
--rw-rw-rw-   0        0        0     6744 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/gui/views/trajectory_table_view.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.309334 trajectopy-0.1.7/trajectopy/plotting/
--rw-rw-rw-   0        0        0       81 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/plotting/__init__.py
--rw-rw-rw-   0        0        0     2185 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/plotting/alignment_plot.py
--rw-rw-rw-   0        0        0      498 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/plotting/default.mplstyle
--rw-rw-rw-   0        0        0    21569 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/plotting/deviation_plot.py
--rw-rw-rw-   0        0        0     2316 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/plotting/image_request.py
--rw-rw-rw-   0        0        0     7342 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/plotting/plot_tabs.py
--rw-rw-rw-   0        0        0     4916 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/plotting/trajectory_plot.py
--rw-rw-rw-   0        0        0     7826 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/plotting/util.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.315330 trajectopy-0.1.7/trajectopy/settings/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/settings/__init__.py
--rw-rw-rw-   0        0        0     8255 2023-07-17 11:38:21.000000 trajectopy-0.1.7/trajectopy/settings/alignment_settings.py
--rw-rw-rw-   0        0        0     1558 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/settings/approximation_settings.py
--rw-rw-rw-   0        0        0     5669 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/settings/comparison_settings.py
--rw-rw-rw-   0        0        0     3578 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/settings/core.py
--rw-rw-rw-   0        0        0     1804 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/settings/plot_settings.py
--rw-rw-rw-   0        0        0     2433 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/settings/processing_settings.py
--rw-rw-rw-   0        0        0      945 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/settings/sorting_settings.py
--rw-rw-rw-   0        0        0    35024 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/trajectory.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.322330 trajectopy-0.1.7/trajectopy/util/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/util/__init__.py
--rw-rw-rw-   0        0        0    18312 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/util/datahandling.py
--rw-rw-rw-   0        0        0     1490 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/util/definitions.py
--rw-rw-rw-   0        0        0      935 2023-07-14 07:19:57.000000 trajectopy-0.1.7/trajectopy/util/path.py
--rw-rw-rw-   0        0        0     5389 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/util/printing.py
--rw-rw-rw-   0        0        0    13599 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/util/reading.py
--rw-rw-rw-   0        0        0     1956 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/util/rotationset.py
--rw-rw-rw-   0        0        0    16143 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/util/spatialsorter.py
--rw-rw-rw-   0        0        0      973 2023-07-14 07:10:55.000000 trajectopy-0.1.7/trajectopy/util/trajectory_processing_state.py
--rw-rw-rw-   0        0        0        5 2023-07-18 14:43:18.000000 trajectopy-0.1.7/trajectopy/version
-drwxrwxrwx   0        0        0        0 2023-07-18 14:43:21.255805 trajectopy-0.1.7/trajectopy.egg-info/
--rw-rw-rw-   0        0        0    13685 2023-07-18 14:43:21.000000 trajectopy-0.1.7/trajectopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3965 2023-07-18 14:43:21.000000 trajectopy-0.1.7/trajectopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 14:43:21.000000 trajectopy-0.1.7/trajectopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-18 14:43:21.000000 trajectopy-0.1.7/trajectopy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 07:19:20.000000 trajectopy-0.1.7/trajectopy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      706 2023-07-18 14:43:21.000000 trajectopy-0.1.7/trajectopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-18 14:43:21.000000 trajectopy-0.1.7/trajectopy.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35790 2023-07-18 19:10:13.451318 trajectopy-0.1.8/LICENSE
+-rw-r--r--   0        0        0      787 2023-07-18 20:52:35.826896 trajectopy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    13484 2023-07-18 19:25:25.689316 trajectopy-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.476172 trajectopy-0.1.8/trajectopy/__init__.py
+-rw-r--r--   0        0        0      630 2023-07-18 19:10:13.477146 trajectopy-0.1.8/trajectopy/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.477146 trajectopy-0.1.8/trajectopy/alignment/__init__.py
+-rw-r--r--   0        0        0    39680 2023-07-18 19:10:13.478145 trajectopy-0.1.8/trajectopy/alignment/alignment.py
+-rw-r--r--   0        0        0     9340 2023-07-18 19:10:13.479197 trajectopy-0.1.8/trajectopy/alignment/data.py
+-rw-r--r--   0        0        0     2421 2023-07-18 19:10:13.479723 trajectopy-0.1.8/trajectopy/alignment/direct_helmert_transformation.py
+-rw-r--r--   0        0        0     5335 2023-07-18 19:10:13.480823 trajectopy-0.1.8/trajectopy/alignment/direct_leverarm.py
+-rw-r--r--   0        0        0     2181 2023-07-18 19:10:13.481855 trajectopy-0.1.8/trajectopy/alignment/direct_timeshift.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.481855 trajectopy-0.1.8/trajectopy/alignment/functional_model/__init__.py
+-rw-r--r--   0        0        0    14944 2023-07-18 19:10:13.482915 trajectopy-0.1.8/trajectopy/alignment/functional_model/equations.py
+-rw-r--r--   0        0        0     8022 2023-07-18 19:10:13.483423 trajectopy-0.1.8/trajectopy/alignment/functional_model/interface.py
+-rw-r--r--   0        0        0    19324 2023-07-18 19:10:13.483423 trajectopy-0.1.8/trajectopy/alignment/parameters.py
+-rw-r--r--   0        0        0     3910 2023-07-18 19:10:13.484435 trajectopy-0.1.8/trajectopy/alignment/util.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.485449 trajectopy-0.1.8/trajectopy/approximation/__init__.py
+-rw-r--r--   0        0        0     8005 2023-07-18 19:10:13.486483 trajectopy-0.1.8/trajectopy/approximation/cubic_approximation.py
+-rw-r--r--   0        0        0     5795 2023-07-18 19:10:13.486483 trajectopy-0.1.8/trajectopy/approximation/mls_approximation.py
+-rw-r--r--   0        0        0     5303 2023-07-18 19:10:13.487709 trajectopy-0.1.8/trajectopy/approximation/rot_approximation.py
+-rw-r--r--   0        0        0     6116 2023-07-18 19:10:13.488738 trajectopy-0.1.8/trajectopy/approximation/trajectory_approximation.py
+-rw-r--r--   0        0        0     4272 2023-07-18 19:10:13.488738 trajectopy-0.1.8/trajectopy/approximation/util.py
+-rw-r--r--   0        0        0     4843 2023-07-18 19:10:13.488738 trajectopy-0.1.8/trajectopy/approximation/voxelizer.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.490229 trajectopy-0.1.8/trajectopy/evaluation/__init__.py
+-rw-r--r--   0        0        0    14610 2023-07-18 19:10:13.491239 trajectopy-0.1.8/trajectopy/evaluation/comparison.py
+-rw-r--r--   0        0        0     4872 2023-07-18 19:10:13.491239 trajectopy-0.1.8/trajectopy/evaluation/matching.py
+-rw-r--r--   0        0        0    29211 2023-07-18 19:10:13.492252 trajectopy-0.1.8/trajectopy/evaluation/trajectory_deviations.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.493251 trajectopy-0.1.8/trajectopy/gui/__init__.py
+-rw-r--r--   0        0        0    14315 2023-07-18 19:10:13.494249 trajectopy-0.1.8/trajectopy/gui/main_window.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.494249 trajectopy-0.1.8/trajectopy/gui/managers/__init__.py
+-rw-r--r--   0        0        0     4431 2023-07-18 19:10:13.495421 trajectopy-0.1.8/trajectopy/gui/managers/file_manager.py
+-rw-r--r--   0        0        0     1692 2023-07-18 19:10:13.496439 trajectopy-0.1.8/trajectopy/gui/managers/manager.py
+-rw-r--r--   0        0        0     3762 2023-07-18 20:45:59.436991 trajectopy-0.1.8/trajectopy/gui/managers/plot_manager.py
+-rw-r--r--   0        0        0     3812 2023-07-18 19:10:13.497462 trajectopy-0.1.8/trajectopy/gui/managers/session_manager.py
+-rw-r--r--   0        0        0    31349 2023-07-18 19:10:13.498475 trajectopy-0.1.8/trajectopy/gui/managers/trajectory_manager.py
+-rw-r--r--   0        0        0     8040 2023-07-18 19:10:13.499476 trajectopy-0.1.8/trajectopy/gui/managers/ui_manager.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.499476 trajectopy-0.1.8/trajectopy/gui/models/__init__.py
+-rw-r--r--   0        0        0    11894 2023-07-18 19:10:13.500660 trajectopy-0.1.8/trajectopy/gui/models/entry.py
+-rw-r--r--   0        0        0     1115 2023-07-18 19:10:13.500660 trajectopy-0.1.8/trajectopy/gui/models/property_model.py
+-rw-r--r--   0        0        0     3904 2023-07-18 19:10:13.502144 trajectopy-0.1.8/trajectopy/gui/models/result_model.py
+-rw-r--r--   0        0        0      977 2023-07-18 19:10:13.503193 trajectopy-0.1.8/trajectopy/gui/models/selection.py
+-rw-r--r--   0        0        0     4017 2023-07-18 19:10:13.504188 trajectopy-0.1.8/trajectopy/gui/models/table_model.py
+-rw-r--r--   0        0        0     4805 2023-07-18 19:10:13.504188 trajectopy-0.1.8/trajectopy/gui/models/trajectory_model.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.505176 trajectopy-0.1.8/trajectopy/gui/requests/__init__.py
+-rw-r--r--   0        0        0      666 2023-07-18 19:10:13.506183 trajectopy-0.1.8/trajectopy/gui/requests/file_request.py
+-rw-r--r--   0        0        0      635 2023-07-18 19:10:13.506693 trajectopy-0.1.8/trajectopy/gui/requests/plot_requests.py
+-rw-r--r--   0        0        0      424 2023-07-18 19:10:13.507866 trajectopy-0.1.8/trajectopy/gui/requests/plot_settings_request.py
+-rw-r--r--   0        0        0      371 2023-07-18 19:10:13.507866 trajectopy-0.1.8/trajectopy/gui/requests/property_request.py
+-rw-r--r--   0        0        0      469 2023-07-18 19:10:13.508878 trajectopy-0.1.8/trajectopy/gui/requests/request.py
+-rw-r--r--   0        0        0      565 2023-07-18 19:10:13.508878 trajectopy-0.1.8/trajectopy/gui/requests/result_model_request.py
+-rw-r--r--   0        0        0      388 2023-07-18 19:10:13.509882 trajectopy-0.1.8/trajectopy/gui/requests/session_request.py
+-rw-r--r--   0        0        0     1029 2023-07-18 19:10:13.509882 trajectopy-0.1.8/trajectopy/gui/requests/trajectory_manager_request.py
+-rw-r--r--   0        0        0      593 2023-07-18 19:10:13.509882 trajectopy-0.1.8/trajectopy/gui/requests/trajectory_model_request.py
+-rw-r--r--   0        0        0      836 2023-07-18 19:10:13.509882 trajectopy-0.1.8/trajectopy/gui/requests/ui_request.py
+-rw-r--r--   0        0        0   120742 2023-07-18 19:10:13.512963 trajectopy-0.1.8/trajectopy/gui/resources/full-icon-poppins.png
+-rw-r--r--   0        0        0    24491 2023-07-18 19:10:13.513949 trajectopy-0.1.8/trajectopy/gui/resources/icon.png
+-rw-r--r--   0        0        0     1751 2023-07-18 19:10:13.514950 trajectopy-0.1.8/trajectopy/gui/util.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.514950 trajectopy-0.1.8/trajectopy/gui/views/__init__.py
+-rw-r--r--   0        0        0     3757 2023-07-18 19:10:13.515949 trajectopy-0.1.8/trajectopy/gui/views/about_window.py
+-rw-r--r--   0        0        0     9601 2023-07-18 19:10:13.515949 trajectopy-0.1.8/trajectopy/gui/views/alignment_edit_window.py
+-rw-r--r--   0        0        0    21480 2023-07-18 20:44:08.483997 trajectopy-0.1.8/trajectopy/gui/views/plot_settings_window.py
+-rw-r--r--   0        0        0     2483 2023-07-18 19:10:13.518972 trajectopy-0.1.8/trajectopy/gui/views/progress_window.py
+-rw-r--r--   0        0        0     4013 2023-07-18 19:10:13.519966 trajectopy-0.1.8/trajectopy/gui/views/properties_window.py
+-rw-r--r--   0        0        0     6154 2023-07-18 19:10:13.519966 trajectopy-0.1.8/trajectopy/gui/views/result_context_menu.py
+-rw-r--r--   0        0        0     4717 2023-07-18 19:10:13.521474 trajectopy-0.1.8/trajectopy/gui/views/result_selection_window.py
+-rw-r--r--   0        0        0     4668 2023-07-18 19:10:13.521474 trajectopy-0.1.8/trajectopy/gui/views/result_table_view.py
+-rw-r--r--   0        0        0    53999 2023-07-18 19:10:13.522498 trajectopy-0.1.8/trajectopy/gui/views/settings_window.py
+-rw-r--r--   0        0        0    20852 2023-07-18 19:10:13.522498 trajectopy-0.1.8/trajectopy/gui/views/trajectory_context_menu.py
+-rw-r--r--   0        0        0     6744 2023-07-18 19:10:13.523699 trajectopy-0.1.8/trajectopy/gui/views/trajectory_table_view.py
+-rw-r--r--   0        0        0    35790 2023-07-18 19:10:13.476172 trajectopy-0.1.8/trajectopy/LICENSE
+-rw-r--r--   0        0        0       81 2023-07-18 19:10:13.523699 trajectopy-0.1.8/trajectopy/plotting/__init__.py
+-rw-r--r--   0        0        0     2185 2023-07-18 19:10:13.525076 trajectopy-0.1.8/trajectopy/plotting/alignment_plot.py
+-rw-r--r--   0        0        0      498 2023-07-18 19:10:13.525076 trajectopy-0.1.8/trajectopy/plotting/default.mplstyle
+-rw-r--r--   0        0        0    21569 2023-07-18 19:10:13.526220 trajectopy-0.1.8/trajectopy/plotting/deviation_plot.py
+-rw-r--r--   0        0        0     7342 2023-07-18 19:10:13.527436 trajectopy-0.1.8/trajectopy/plotting/plot_tabs.py
+-rw-r--r--   0        0        0     4242 2023-07-18 20:45:32.812467 trajectopy-0.1.8/trajectopy/plotting/trajectory_plot.py
+-rw-r--r--   0        0        0     7826 2023-07-18 19:10:13.528680 trajectopy-0.1.8/trajectopy/plotting/util.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.528680 trajectopy-0.1.8/trajectopy/settings/__init__.py
+-rw-r--r--   0        0        0     8255 2023-07-18 19:10:13.529894 trajectopy-0.1.8/trajectopy/settings/alignment_settings.py
+-rw-r--r--   0        0        0     1558 2023-07-18 19:10:13.529894 trajectopy-0.1.8/trajectopy/settings/approximation_settings.py
+-rw-r--r--   0        0        0     5669 2023-07-18 19:10:13.531054 trajectopy-0.1.8/trajectopy/settings/comparison_settings.py
+-rw-r--r--   0        0        0     3578 2023-07-18 19:10:13.531054 trajectopy-0.1.8/trajectopy/settings/core.py
+-rw-r--r--   0        0        0     1703 2023-07-18 20:45:43.990959 trajectopy-0.1.8/trajectopy/settings/plot_settings.py
+-rw-r--r--   0        0        0     2433 2023-07-18 19:10:13.532825 trajectopy-0.1.8/trajectopy/settings/processing_settings.py
+-rw-r--r--   0        0        0      945 2023-07-18 19:10:13.532825 trajectopy-0.1.8/trajectopy/settings/sorting_settings.py
+-rw-r--r--   0        0        0    35024 2023-07-18 19:10:13.533867 trajectopy-0.1.8/trajectopy/trajectory.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:10:13.533867 trajectopy-0.1.8/trajectopy/util/__init__.py
+-rw-r--r--   0        0        0    18312 2023-07-18 19:10:13.535080 trajectopy-0.1.8/trajectopy/util/datahandling.py
+-rw-r--r--   0        0        0     1490 2023-07-18 19:10:13.535080 trajectopy-0.1.8/trajectopy/util/definitions.py
+-rw-r--r--   0        0        0      935 2023-07-18 19:10:13.536340 trajectopy-0.1.8/trajectopy/util/path.py
+-rw-r--r--   0        0        0     5389 2023-07-18 19:10:13.536340 trajectopy-0.1.8/trajectopy/util/printing.py
+-rw-r--r--   0        0        0    13599 2023-07-18 19:10:13.537764 trajectopy-0.1.8/trajectopy/util/reading.py
+-rw-r--r--   0        0        0     1956 2023-07-18 19:10:13.537764 trajectopy-0.1.8/trajectopy/util/rotationset.py
+-rw-r--r--   0        0        0    16143 2023-07-18 19:10:13.538831 trajectopy-0.1.8/trajectopy/util/spatialsorter.py
+-rw-r--r--   0        0        0      973 2023-07-18 19:10:13.538831 trajectopy-0.1.8/trajectopy/util/trajectory_processing_state.py
+-rw-r--r--   0        0        0        5 2023-07-18 20:51:49.838306 trajectopy-0.1.8/trajectopy/version
+-rw-r--r--   0        0        0    14397 1970-01-01 00:00:00.000000 trajectopy-0.1.8/PKG-INFO
```

### Comparing `trajectopy-0.1.7/LICENSE` & `trajectopy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/PKG-INFO` & `trajectopy-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,29 @@
-Metadata-Version: 2.1
-Name: trajectopy
-Version: 0.1.7
-Summary: Trajectory Evaluation in Python
-Home-page: https://github.com/gereon-t/trajectopy
-Author: Gereon Tombrink
-Author-email: tombrink@igg.uni-bonn.de
-License: GPLv3
-Keywords: trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Trajectopy - Trajectory Evaluation in Python
 Welcome to Trajectopy, a Python package designed to simplify the alignment and comparison of trajectories using an intuitive graphical user interface (GUI).
 ![](.images/main_gui.png)
+![](.images/evaluation_example.png)
 
 ## Key Features
 
 Trajectopy offers a range of features, including:
 
 - Interactive GUI: A user-friendly interface that enables seamless interaction with your trajectory data, making it easy to visualize, align, and compare trajectories.
 - Alignment Algorithm: An advanced algorithm that can be tailored to the specific application and supports a similarity transformation, a leverarm and a time shift estimation.
 - Comparison Metrics: Absolute and relative comparison metrics that can be computed using various pose-matching methods
 - Data Import/Export: Support for importing and exporting data, ensuring compatibility with your existing workflows.
 - Customizable Visualization: A flexible visualization that allows users to customize plot styles, tailoring the output to their specific needs.
 
 ## Installation
-Clone this repository using:
+Using pip:
+```console
+pip install trajectopy
+```
+
+Or using the repository:
 ```console
 $ git clone https://github.com/gereon-t/trajectopy.git
 ```
 ```console
 cd trajectopy
 ```
 
@@ -89,19 +82,21 @@
 - Similarity x translation
 - Similarity y translation
 - Similarity z translation
 - Similarity x rotation
 - Similarity y rotation
 - Similarity z rotation
 - Similarity scale
-- Time shift
+- (small) Time shift
 - Lever arm x
 - Lever arm y
 - Lever arm z
 
+Both trajectories should be roughly synchronized to improve trajectory matching before alignment.
+
 
 ## Comparing Trajectories
 This toolbox allows the comparison of two trajectories using absolute and relative metrics. Before comparison, both trajectories to be compared must be matched. After this, either absolute or relative metrics can be computed.
 
 ### Matching
 There are three different types of trajectory matching implemented in trajectopy:
 * Matching via interpolation: Poses are matched by interpolating one trajectory onto the timestamps of the other.
```

#### html2text {}

```diff
@@ -1,35 +1,31 @@
-Metadata-Version: 2.1 Name: trajectopy Version: 0.1.7 Summary: Trajectory
-Evaluation in Python Home-page: https://github.com/gereon-t/trajectopy Author:
-Gereon Tombrink Author-email: tombrink@igg.uni-bonn.de License: GPLv3 Keywords:
-trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics Requires-
-Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE #
-Trajectopy - Trajectory Evaluation in Python Welcome to Trajectopy, a Python
+# Trajectopy - Trajectory Evaluation in Python Welcome to Trajectopy, a Python
 package designed to simplify the alignment and comparison of trajectories using
-an intuitive graphical user interface (GUI). ![](.images/main_gui.png) ## Key
-Features Trajectopy offers a range of features, including: - Interactive GUI: A
-user-friendly interface that enables seamless interaction with your trajectory
-data, making it easy to visualize, align, and compare trajectories. - Alignment
-Algorithm: An advanced algorithm that can be tailored to the specific
-application and supports a similarity transformation, a leverarm and a time
-shift estimation. - Comparison Metrics: Absolute and relative comparison
-metrics that can be computed using various pose-matching methods - Data Import/
-Export: Support for importing and exporting data, ensuring compatibility with
-your existing workflows. - Customizable Visualization: A flexible visualization
-that allows users to customize plot styles, tailoring the output to their
-specific needs. ## Installation Clone this repository using: ```console $ git
-clone https://github.com/gereon-t/trajectopy.git ``` ```console cd trajectopy
-``` Install ``` python3 -m pip install -e . ``` Run ``` trajectopy ``` ##
-Importing Trajectories Trajectories can be imported using the "Add" button
-below the trajectory table or by dragging files into the area of the trajectory
-table. Trajectory files must be ASCII files with a csv-like layout, by default,
-trajectopy filters for the ".traj" extension. The default column structure that
-can be read without any configuration is the following: | time | position x |
-position y | position z | quaternion x | quaternion y | quaternion z |
-quaternion w | |---|---|---|---|---|---|---|---| Columns are expected to be
+an intuitive graphical user interface (GUI). ![](.images/main_gui.png) ![]
+(.images/evaluation_example.png) ## Key Features Trajectopy offers a range of
+features, including: - Interactive GUI: A user-friendly interface that enables
+seamless interaction with your trajectory data, making it easy to visualize,
+align, and compare trajectories. - Alignment Algorithm: An advanced algorithm
+that can be tailored to the specific application and supports a similarity
+transformation, a leverarm and a time shift estimation. - Comparison Metrics:
+Absolute and relative comparison metrics that can be computed using various
+pose-matching methods - Data Import/Export: Support for importing and exporting
+data, ensuring compatibility with your existing workflows. - Customizable
+Visualization: A flexible visualization that allows users to customize plot
+styles, tailoring the output to their specific needs. ## Installation Using
+pip: ```console pip install trajectopy ``` Or using the repository: ```console
+$ git clone https://github.com/gereon-t/trajectopy.git ``` ```console cd
+trajectopy ``` Install ``` python3 -m pip install -e . ``` Run ``` trajectopy
+``` ## Importing Trajectories Trajectories can be imported using the "Add"
+button below the trajectory table or by dragging files into the area of the
+trajectory table. Trajectory files must be ASCII files with a csv-like layout,
+by default, trajectopy filters for the ".traj" extension. The default column
+structure that can be read without any configuration is the following: | time |
+position x | position y | position z | quaternion x | quaternion y | quaternion
+z | quaternion w | |---|---|---|---|---|---|---|---| Columns are expected to be
 separated by commas by default. It is recommended to provide a header at the
 beginning of the trajectory file. Header entries always begin with a "#". Below
 you can find a table of all allowed header entries and their meaning. | Header
 | Description | |---|---| | #name | The name provided here is displayed in the
 table view and in plots of the trajectory | | #epsg | [EPSG Code](https://
 epsg.io/) of the datum of the input positions. Required, if geodetic datum
 transformations are desired. Default: 0, meaning local coordinates without any
@@ -89,92 +85,94 @@
 Observation groups are: xy_from, z_from, xy_to, z_to, roll_pitch, yaw, speed. |
 | Observation Standard Deviations | Standard deviations of the trajectory data
 involved. | | Estimation Of | Toggle for individual parameters that should be
 estimated. Furthermore, the user can specify which components of the 3d speed
 vector should be used for time shift estimation. | Parameters that can be
 estimated: - Similarity x translation - Similarity y translation - Similarity z
 translation - Similarity x rotation - Similarity y rotation - Similarity z
-rotation - Similarity scale - Time shift - Lever arm x - Lever arm y - Lever
-arm z ## Comparing Trajectories This toolbox allows the comparison of two
-trajectories using absolute and relative metrics. Before comparison, both
-trajectories to be compared must be matched. After this, either absolute or
-relative metrics can be computed. ### Matching There are three different types
-of trajectory matching implemented in trajectopy: * Matching via interpolation:
-Poses are matched by interpolating one trajectory onto the timestamps of the
-other. * Matching via Nearest Temporal Neighbor: Poses are matched using their
-timestamps while considering some pre-defined tolerance. * Matching via Nearest
-Spatial Neighbor: Poses are matched using their nearest neighbors while
-considering some pre-defined distance tolerance. Matching tolerances can be set
-in the settings of the corresponding trajectory. ### Absolute This metric is
-often referred to as Absolute Trajectory Error (ATE). It measures the
-translational and rotational difference between two matched poses. By default,
-trajectopy splits the deviations into vertical cross-track, horizontal cross-
-track, and along-track deviations to simplify interpretation. This behavior can
-be turned off. ### Relative For this metric, relative pose-pair differences are
-compared. The distance between two poses can be specified by the user and can
-be either time- or distance-based. The comparison involves finding pose pairs
-separated by a specific distance or time interval, computing the relative
-translation and rotation between the reference and estimated pose pairs, and
-calculating the translational and rotational difference normalized by the
-distance or time that separated the poses. 1. Find pose pair separated by e.g.
-100 m in reference trajectory 2. Find corresponding pose pair in estimated
-trajectory 3. Compute relative translation and rotation between the reference
-pose pair 4. Compute relative translation and rotation between the estimated
-pose pair 5. Compute translational and rotational difference between 3) and 4)
-6. Divide 5) by the distance or the time that separated both poses (e.g. 100
-m). Units are m/m: %, deg/m for distance based comparison and m/s, deg/s for
-time-based comparison. Pose distances can be set in the settings of the
-corresponding trajectory. Furthermore, the user can choose to either use
-consecutive pose pairs (non-overlapping) or all posible pairs (overlapping). ##
-Spatial Sorting When dealing with repeated trajectories, it may be useful to
-spatially sort the trajectory for further analysis. This reconstructs the point
-order as a function of the trajectory length. Trajectopy uses a combination of
-an iterative voxel-based moving least-squares approximation and a minimum
-spanning tree to solve this problem. The point cloud is divided into voxels of
-a given size. Then, for each point, a number of neighboring voxels are
-requested. A 3D line is estimated using the points within these voxels.
-Finally, the current point is projected onto the line to obtain the
-approximated point. The spatial sorting of this MLS approximation is
-reconstructed using a minimum spanning tree. Depending on the algorithm,
-colinear points are discarded in this step. ## Approximation The trajectory can
-be approximated using piecewise cubic polynomials for the positions and sliding
-window based smoothing for the rotations. The window sizes and the minimum
-number of observations that should be within an interval can be set by the
-user. ## Sessions Sessions allow you to export all imported and computed
-trajectories and results into a folder. This folder can be imported again after
-restarting trajectopy, saving time and keeping related data together. ##
-Settings ### Plot Settings | Setting | Description | |---|---| | Position Unit
-| Affects deviation plots only | | Stair Histogram | If set to true, deviation
-histograms are not filled and only a stair is visible. (see also matplotlib
-documentation) | | Smoothing Window Width | For better visibility in the
-deviation plots, the deviations are smoothed with a sliding window of a certain
-width. Smoothing can be turned off by setting a width of 0.0 or -1.0 | | Show
-Mean Line | Toggles the visibility of a red mean line in deviation plots. | |
-Grid Megapixels | For every scatter plot, the trajectory data is divided into a
-grid with a certain number of pixels that can be set with this setting. This
-prevents slow plotting with large trajectories. | | RMS Window Width | Similar
-to the Smoothing Window Width, this parameter sets the width of a sliding
-window used to smooth the RMS values that are mapped onto the trajectory in
-scatter plots. Smoothing can be turned off by setting a width of 0.0 or -1.0 |
-| Show Zero-Crossing in Colorbars | Each scatter plot of deviations includes a
-colorbar, which can be toggled to show the zero-crossing explicitly. | |
-Colorbar Step Divisor, Clip Colorbar at X Sigma | The colorbar limits are
-determined by either the minimum or maximum values, or by the X-sigma range
-("Clip-Colorbar at X Sigma" Setting) around the mean deviation, depending on
-which limit is more restrictive. Starting at the lower bound, the colorbar
-ticks are placed at positions each separated by the total colorbar range
-divided by the colorbar step divisor. | | No axis | Toggles the visibility of
-axes in scatter plots | | Rotate Scatter Plots to Main Axis | When set to true,
-the scatter plot trajectories will be rotated to align their main axis of
-extension (determined through principal component analysis) with the x-axis.
-This can be beneficial for elongated trajectories. | #### Custom Matplotlib
-Style You can use a custom plotting style by placing a `custom.mplstyle` file
-in the directory you launched trajectopy in. For instructions on how to define
-custom plotting styles, please see https://matplotlib.org/stable/tutorials/
-introductory/customizing.html. Below you can see the default style of
-trajectopy ```python figure.figsize: 8, 6 figure.facecolor: white font.size: 14
-font.family: serif axes.prop_cycle: cycler("color", ["1E88E5", "#FFC107",
-"#004D40", "#D81B60", "#2bd2bb", "#a3bbf1", "#3c41fd", "#cc5510", "#3b0732",
-"#88122b", "#bccb70", "dc9c54"]) axes.facecolor: E2E2E2 axes.edgecolor: white
-axes.grid: True grid.color: white grid.linewidth: 0.3 axes.grid.which: major
-axes.axisbelow: True legend.facecolor: white lines.linestyle: - lines.marker: .
-savefig.dpi: 1500 savefig.format: pdf ```
+rotation - Similarity scale - (small) Time shift - Lever arm x - Lever arm y -
+Lever arm z Both trajectories should be roughly synchronized to improve
+trajectory matching before alignment. ## Comparing Trajectories This toolbox
+allows the comparison of two trajectories using absolute and relative metrics.
+Before comparison, both trajectories to be compared must be matched. After
+this, either absolute or relative metrics can be computed. ### Matching There
+are three different types of trajectory matching implemented in trajectopy: *
+Matching via interpolation: Poses are matched by interpolating one trajectory
+onto the timestamps of the other. * Matching via Nearest Temporal Neighbor:
+Poses are matched using their timestamps while considering some pre-defined
+tolerance. * Matching via Nearest Spatial Neighbor: Poses are matched using
+their nearest neighbors while considering some pre-defined distance tolerance.
+Matching tolerances can be set in the settings of the corresponding trajectory.
+### Absolute This metric is often referred to as Absolute Trajectory Error
+(ATE). It measures the translational and rotational difference between two
+matched poses. By default, trajectopy splits the deviations into vertical
+cross-track, horizontal cross-track, and along-track deviations to simplify
+interpretation. This behavior can be turned off. ### Relative For this metric,
+relative pose-pair differences are compared. The distance between two poses can
+be specified by the user and can be either time- or distance-based. The
+comparison involves finding pose pairs separated by a specific distance or time
+interval, computing the relative translation and rotation between the reference
+and estimated pose pairs, and calculating the translational and rotational
+difference normalized by the distance or time that separated the poses. 1. Find
+pose pair separated by e.g. 100 m in reference trajectory 2. Find corresponding
+pose pair in estimated trajectory 3. Compute relative translation and rotation
+between the reference pose pair 4. Compute relative translation and rotation
+between the estimated pose pair 5. Compute translational and rotational
+difference between 3) and 4) 6. Divide 5) by the distance or the time that
+separated both poses (e.g. 100 m). Units are m/m: %, deg/m for distance based
+comparison and m/s, deg/s for time-based comparison. Pose distances can be set
+in the settings of the corresponding trajectory. Furthermore, the user can
+choose to either use consecutive pose pairs (non-overlapping) or all posible
+pairs (overlapping). ## Spatial Sorting When dealing with repeated
+trajectories, it may be useful to spatially sort the trajectory for further
+analysis. This reconstructs the point order as a function of the trajectory
+length. Trajectopy uses a combination of an iterative voxel-based moving least-
+squares approximation and a minimum spanning tree to solve this problem. The
+point cloud is divided into voxels of a given size. Then, for each point, a
+number of neighboring voxels are requested. A 3D line is estimated using the
+points within these voxels. Finally, the current point is projected onto the
+line to obtain the approximated point. The spatial sorting of this MLS
+approximation is reconstructed using a minimum spanning tree. Depending on the
+algorithm, colinear points are discarded in this step. ## Approximation The
+trajectory can be approximated using piecewise cubic polynomials for the
+positions and sliding window based smoothing for the rotations. The window
+sizes and the minimum number of observations that should be within an interval
+can be set by the user. ## Sessions Sessions allow you to export all imported
+and computed trajectories and results into a folder. This folder can be
+imported again after restarting trajectopy, saving time and keeping related
+data together. ## Settings ### Plot Settings | Setting | Description | |---|---
+| | Position Unit | Affects deviation plots only | | Stair Histogram | If set
+to true, deviation histograms are not filled and only a stair is visible. (see
+also matplotlib documentation) | | Smoothing Window Width | For better
+visibility in the deviation plots, the deviations are smoothed with a sliding
+window of a certain width. Smoothing can be turned off by setting a width of
+0.0 or -1.0 | | Show Mean Line | Toggles the visibility of a red mean line in
+deviation plots. | | Grid Megapixels | For every scatter plot, the trajectory
+data is divided into a grid with a certain number of pixels that can be set
+with this setting. This prevents slow plotting with large trajectories. | | RMS
+Window Width | Similar to the Smoothing Window Width, this parameter sets the
+width of a sliding window used to smooth the RMS values that are mapped onto
+the trajectory in scatter plots. Smoothing can be turned off by setting a width
+of 0.0 or -1.0 | | Show Zero-Crossing in Colorbars | Each scatter plot of
+deviations includes a colorbar, which can be toggled to show the zero-crossing
+explicitly. | | Colorbar Step Divisor, Clip Colorbar at X Sigma | The colorbar
+limits are determined by either the minimum or maximum values, or by the X-
+sigma range ("Clip-Colorbar at X Sigma" Setting) around the mean deviation,
+depending on which limit is more restrictive. Starting at the lower bound, the
+colorbar ticks are placed at positions each separated by the total colorbar
+range divided by the colorbar step divisor. | | No axis | Toggles the
+visibility of axes in scatter plots | | Rotate Scatter Plots to Main Axis |
+When set to true, the scatter plot trajectories will be rotated to align their
+main axis of extension (determined through principal component analysis) with
+the x-axis. This can be beneficial for elongated trajectories. | #### Custom
+Matplotlib Style You can use a custom plotting style by placing a
+`custom.mplstyle` file in the directory you launched trajectopy in. For
+instructions on how to define custom plotting styles, please see https://
+matplotlib.org/stable/tutorials/introductory/customizing.html. Below you can
+see the default style of trajectopy ```python figure.figsize: 8, 6
+figure.facecolor: white font.size: 14 font.family: serif axes.prop_cycle:
+cycler("color", ["1E88E5", "#FFC107", "#004D40", "#D81B60", "#2bd2bb",
+"#a3bbf1", "#3c41fd", "#cc5510", "#3b0732", "#88122b", "#bccb70", "dc9c54"])
+axes.facecolor: E2E2E2 axes.edgecolor: white axes.grid: True grid.color: white
+grid.linewidth: 0.3 axes.grid.which: major axes.axisbelow: True
+legend.facecolor: white lines.linestyle: - lines.marker: . savefig.dpi: 1500
+savefig.format: pdf ```
```

### Comparing `trajectopy-0.1.7/README.md` & `trajectopy-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,162 +1,201 @@
-# Trajectopy - Trajectory Evaluation in Python
-Welcome to Trajectopy, a Python package designed to simplify the alignment and comparison of trajectories using an intuitive graphical user interface (GUI).
-![](.images/main_gui.png)
-
-## Key Features
-
-Trajectopy offers a range of features, including:
-
-- Interactive GUI: A user-friendly interface that enables seamless interaction with your trajectory data, making it easy to visualize, align, and compare trajectories.
-- Alignment Algorithm: An advanced algorithm that can be tailored to the specific application and supports a similarity transformation, a leverarm and a time shift estimation.
-- Comparison Metrics: Absolute and relative comparison metrics that can be computed using various pose-matching methods
-- Data Import/Export: Support for importing and exporting data, ensuring compatibility with your existing workflows.
-- Customizable Visualization: A flexible visualization that allows users to customize plot styles, tailoring the output to their specific needs.
-
-## Installation
-Clone this repository using:
-```console
-$ git clone https://github.com/gereon-t/trajectopy.git
-```
-```console
-cd trajectopy
-```
-
-
-Install
-```
-python3 -m pip install -e .
-```
-
-Run
-```
-trajectopy
-```
-
-## Importing Trajectories
-Trajectories can be imported using the "Add" button below the trajectory table or by dragging files into the area of the trajectory table.
-Trajectory files must be ASCII files with a csv-like layout, by default, trajectopy filters for the ".traj" extension. The default column structure that can be read without any configuration is the following:
-
-| time | position x | position y | position z | quaternion x | quaternion y | quaternion z | quaternion w |
-|---|---|---|---|---|---|---|---|
-
-
-Columns are expected to be separated by commas by default.
-
-It is recommended to provide a header at the beginning of the trajectory file. Header entries always begin with a "#".
-Below you can find a table of all allowed header entries and their meaning.
-
-| Header | Description  |
-|---|---|
-| #name | The name provided here is displayed in the table view and in plots of the trajectory |
-| #epsg | [EPSG Code](https://epsg.io/) of the datum of the input positions. Required, if geodetic datum transformations are desired. Default: 0, meaning local coordinates without any known geodetic datum |
-| #fields | Describes the columns of the ASCII trajectory file. Separated with commas. <table>  <thead>  <th>field name</th>  <th>Meaning</th>  </tr>  </thead>  <tbody>  <tr>  <td>t</td>  <td>time</td>  </tr>  <tr>  <td>l</td>  <td>arc lengths in meters</td>  </tr>  <tr>  <td>px</td>  <td>position x / lat (degrees only)</td>  </tr>  <tr>  <td>py</td>  <td>position y / lon (degrees only) </td>  </tr>  <tr>  <td>pz</td>  <td>position z</td>  </tr> <tr>  <td>qx</td>  <td>quaternion x</td>  </tr> <tr>  <td>qy</td>  <td>quaternion y</td>  </tr> <tr>  <td>qz</td>  <td>quaternion z</td>  </tr> <tr>  <td>qw</td>  <td>quaternion w</td>  </tr> </tr> <tr>  <td>ex</td>  <td>euler angle x</td>  </tr> </tr> <tr>  <td>ey</td>  <td>euler angle y</td>  </tr> </tr> <tr>  <td>ez</td>  <td>euler angle z</td>  </tr> </tr> <tr>  <td>vx</td>  <td>speed x</td>  </tr> </tr> <tr>  <td>vy</td>  <td>speed y</td>  </tr> </tr> <tr>  <td>vz</td>  <td>speed z</td>  </tr> </tr> </tbody>  </table> Example: "#fields t,px,py,pz" Note: The only column that is allowed to appear multiple times is the "t" column. |
-| #delimiter | Delimiter used to separate the columns within the file. Default: "," |
-| #nframe | Definition of the navigation-frame the orientations of the trajectory refer to. Choices: "enu": East North Up or "ned": North East Down. Default: "enu" |
-| #rot_unit | Unit of the orientations. Choices: "deg": Degree, "rad": Radians. Default: "rad" |
-| #time_format | Format of the timestamps / dates. Choices: "unix": Unix timestamps (since 01-01-1970), "datetime": Human readable date-times. Default: "unix" |
-| #time_offset | Offset in seconds that is applied to the imported timestamps. Default: 0.0 |
-| #datetime_format | Format of the datetimes. Only relevant if "time_format" is "datetime". Default: "%Y-%m-%d %H:%M:%S.%f" |
-| #datetime_timezone | Time zone of the timestamps. During import, all timestamps are converted to UTC considering the input time zone. Choices: [Time zone](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) or "GPS" |
-| #sorting | Sorting of the input data. Choices: "chrono": Chronologically sorted data (usually the case), "spatial": Spatially sorted data, i.e. along the arc length. Default: "chrono" |
-| #state | States describing what processing steps the data already has passed. States: "approximated", "interpolated", "intersected", "aligned", "matched", "sorting_known" |
-
-## Aligning Trajectories
-The trajectories to be compared could be defined in different coordinate systems and/or refer to different positions on the same platform due to different mounting positions. There may also be a small synchronization offset. To solve this problem, trajectopy provides functionality to align two trajectories using least squares adjustment theory. This allows estimation of up to 11 parameters, all of which can be turned on or off individually to tailor the alignment to the sensor modalities. The alignment settings can be found in the right-click trajectory settings.
-
-### Alignment Settings
-| Setting | Description |
-|---|---|
-| Minimum Speed | If set to a value larger than 0.0, only poses with a speed higher than the specified value are used for alignment. This is only relevant for the time shift estimation where higher speed usually lead to better results. |
-| Time Start, Time End | Time range given in seconds relative to the start of the trajectory that should be aligned. If set to non-zero values, only poses in the specified time span are used for alignment. |
-| Error Probability | Used for stochastic tests. During the alignment, the functional relationship and the stochastic model are tested for consistency. Besides a global test, there are also tests for each observation group. Observation groups are:  xy_from, z_from, xy_to, z_to, roll_pitch, yaw, speed. |
-| Observation Standard Deviations | Standard deviations of the trajectory data involved. |
-| Estimation Of | Toggle for individual parameters that should be estimated. Furthermore, the user can specify which components of the 3d speed vector should be used for time shift estimation. |
-
-Parameters that can be estimated:
-- Similarity x translation
-- Similarity y translation
-- Similarity z translation
-- Similarity x rotation
-- Similarity y rotation
-- Similarity z rotation
-- Similarity scale
-- Time shift
-- Lever arm x
-- Lever arm y
-- Lever arm z
-
-
-## Comparing Trajectories
-This toolbox allows the comparison of two trajectories using absolute and relative metrics. Before comparison, both trajectories to be compared must be matched. After this, either absolute or relative metrics can be computed.
-
-### Matching
-There are three different types of trajectory matching implemented in trajectopy:
-* Matching via interpolation: Poses are matched by interpolating one trajectory onto the timestamps of the other.
-* Matching via Nearest Temporal Neighbor: Poses are matched using their timestamps while considering some pre-defined tolerance.
-* Matching via Nearest Spatial Neighbor: Poses are matched using their nearest neighbors while considering some pre-defined distance tolerance.
-
-Matching tolerances can be set in the settings of the corresponding trajectory.
-
-### Absolute
-This metric is often referred to as Absolute Trajectory Error (ATE). It measures the translational and rotational difference between two matched poses. By default, trajectopy splits the deviations into vertical cross-track, horizontal cross-track, and along-track deviations to simplify interpretation. This behavior can be turned off.
-
-### Relative
-For this metric, relative pose-pair differences are compared. The distance between two poses can be specified by the user and can be either time- or distance-based. The comparison involves finding pose pairs separated by a specific distance or time interval, computing the relative translation and rotation between the reference and estimated pose pairs, and calculating the translational and rotational difference normalized by the distance or time that separated the poses.
-
-1. Find pose pair separated by e.g. 100 m in reference trajectory
-2. Find corresponding pose pair in estimated trajectory
-3. Compute relative translation and rotation between the reference pose pair
-4. Compute relative translation and rotation between the estimated pose pair
-5. Compute translational and rotational difference between 3) and 4)
-6. Divide 5) by the distance or the time that separated both poses (e.g. 100 m).
-
-Units are m/m: %, deg/m for distance based comparison and m/s, deg/s for time-based comparison. Pose distances can be set in the settings of the corresponding trajectory. Furthermore, the user can choose to either use consecutive pose pairs (non-overlapping) or all posible pairs (overlapping).
-
-## Spatial Sorting
-When dealing with repeated trajectories, it may be useful to spatially sort the trajectory for further analysis. This reconstructs the point order as a function of the trajectory length. Trajectopy uses a combination of an iterative voxel-based moving least-squares approximation and a minimum spanning tree to solve this problem.
-
-The point cloud is divided into voxels of a given size. Then, for each point, a number of neighboring voxels are requested. A 3D line is estimated using the points within these voxels. Finally, the current point is projected onto the line to obtain the approximated point. The spatial sorting of this MLS approximation is reconstructed using a minimum spanning tree. Depending on the algorithm, colinear points are discarded in this step.
-
-## Approximation
-The trajectory can be approximated using piecewise cubic polynomials for the positions and sliding window based smoothing for the rotations. The window sizes and the minimum number of observations that should be within an interval can be set by the user.
-
-## Sessions
-Sessions allow you to export all imported and computed trajectories and results into a folder. This folder can be imported again after restarting trajectopy, saving time and keeping related data together.
-
-## Settings
-### Plot Settings
-| Setting | Description |
-|---|---|
-| Position Unit | Affects deviation plots only |
-| Stair Histogram | If set to true, deviation histograms are not filled and only a stair is visible. (see also matplotlib documentation) |
-| Smoothing Window Width | For better visibility in the deviation plots, the deviations are smoothed with a sliding window of a certain width. Smoothing can be turned off by setting a width of 0.0 or -1.0 |
-| Show Mean Line | Toggles the visibility of a red mean line in deviation plots. |
-| Grid Megapixels | For every scatter plot, the trajectory data is divided into a grid with a certain number of pixels that can be set with this setting. This prevents slow plotting with large trajectories. |
-| RMS Window Width | Similar to the Smoothing Window Width, this parameter sets the width of a sliding window used to smooth the RMS values that are mapped onto the trajectory in scatter plots. Smoothing can be turned off by setting a width of 0.0 or -1.0 |
-| Show Zero-Crossing in Colorbars | Each scatter plot of deviations includes a colorbar, which can be toggled to show the zero-crossing explicitly. |
-| Colorbar Step Divisor, Clip Colorbar at X Sigma | The colorbar limits are determined by either the minimum or maximum values, or by the X-sigma range ("Clip-Colorbar at X Sigma" Setting) around the mean deviation, depending on which limit is more restrictive. Starting at the lower bound, the colorbar ticks are placed at positions each separated by the total colorbar range divided by the colorbar step divisor. |
-| No axis | Toggles the visibility of axes in scatter plots |
-| Rotate Scatter Plots to Main Axis | When set to true, the scatter plot trajectories will be rotated to align their main axis of extension (determined through principal component analysis) with the x-axis. This can be beneficial for elongated trajectories. |
-
-#### Custom Matplotlib Style
-You can use a custom plotting style by placing a `custom.mplstyle` file in the directory you launched trajectopy in. For instructions on how to define custom plotting styles, please see https://matplotlib.org/stable/tutorials/introductory/customizing.html.
-Below you can see the default style of trajectopy
-```python
-figure.figsize: 8, 6
-figure.facecolor: white
-font.size: 14
-font.family: serif
-axes.prop_cycle: cycler("color", ["1E88E5", "#FFC107", "#004D40", "#D81B60", "#2bd2bb", "#a3bbf1", "#3c41fd", "#cc5510", "#3b0732", "#88122b", "#bccb70", "dc9c54"])
-axes.facecolor: E2E2E2
-axes.edgecolor: white
-axes.grid: True
-grid.color: white
-grid.linewidth: 0.3
-axes.grid.which: major
-axes.axisbelow: True
-legend.facecolor: white
-lines.linestyle: -
-lines.marker: .
-savefig.dpi: 1500
-savefig.format: pdf
-```
+Metadata-Version: 2.1
+Name: trajectopy
+Version: 0.1.8
+Summary: Trajectory Evaluation in Python
+Home-page: https://github.com/gereon-t/trajectopy
+License: GPLv3
+Keywords: trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics
+Author: Gereon Tombrink
+Author-email: tombrink@igg.uni-bonn.de
+Requires-Python: >=3.9,<3.12
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyQt6 (>=6.4.2)
+Requires-Dist: PyQt6-Qt6 (>=6.4.2)
+Requires-Dist: PyQt6-sip (>=13.4.1)
+Requires-Dist: PyYAML (>=6.0)
+Requires-Dist: autograd (>=1.5)
+Requires-Dist: matplotlib (>=3.6.3)
+Requires-Dist: networkx (>=3.0)
+Requires-Dist: numpy (>=1.24.1)
+Requires-Dist: pandas (>=1.5.3)
+Requires-Dist: pointset (>=0.1.5)
+Requires-Dist: scipy (>=1.10.0)
+Requires-Dist: seaborn (>=0.12.2)
+Project-URL: Repository, https://github.com/gereon-t/trajectopy.git
+Description-Content-Type: text/markdown
+
+# Trajectopy - Trajectory Evaluation in Python
+Welcome to Trajectopy, a Python package designed to simplify the alignment and comparison of trajectories using an intuitive graphical user interface (GUI).
+![](.images/main_gui.png)
+![](.images/evaluation_example.png)
+
+## Key Features
+
+Trajectopy offers a range of features, including:
+
+- Interactive GUI: A user-friendly interface that enables seamless interaction with your trajectory data, making it easy to visualize, align, and compare trajectories.
+- Alignment Algorithm: An advanced algorithm that can be tailored to the specific application and supports a similarity transformation, a leverarm and a time shift estimation.
+- Comparison Metrics: Absolute and relative comparison metrics that can be computed using various pose-matching methods
+- Data Import/Export: Support for importing and exporting data, ensuring compatibility with your existing workflows.
+- Customizable Visualization: A flexible visualization that allows users to customize plot styles, tailoring the output to their specific needs.
+
+## Installation
+Using pip:
+```console
+pip install trajectopy
+```
+
+Or using the repository:
+```console
+$ git clone https://github.com/gereon-t/trajectopy.git
+```
+```console
+cd trajectopy
+```
+
+
+Install
+```
+python3 -m pip install -e .
+```
+
+Run
+```
+trajectopy
+```
+
+## Importing Trajectories
+Trajectories can be imported using the "Add" button below the trajectory table or by dragging files into the area of the trajectory table.
+Trajectory files must be ASCII files with a csv-like layout, by default, trajectopy filters for the ".traj" extension. The default column structure that can be read without any configuration is the following:
+
+| time | position x | position y | position z | quaternion x | quaternion y | quaternion z | quaternion w |
+|---|---|---|---|---|---|---|---|
+
+
+Columns are expected to be separated by commas by default.
+
+It is recommended to provide a header at the beginning of the trajectory file. Header entries always begin with a "#".
+Below you can find a table of all allowed header entries and their meaning.
+
+| Header | Description  |
+|---|---|
+| #name | The name provided here is displayed in the table view and in plots of the trajectory |
+| #epsg | [EPSG Code](https://epsg.io/) of the datum of the input positions. Required, if geodetic datum transformations are desired. Default: 0, meaning local coordinates without any known geodetic datum |
+| #fields | Describes the columns of the ASCII trajectory file. Separated with commas. <table>  <thead>  <th>field name</th>  <th>Meaning</th>  </tr>  </thead>  <tbody>  <tr>  <td>t</td>  <td>time</td>  </tr>  <tr>  <td>l</td>  <td>arc lengths in meters</td>  </tr>  <tr>  <td>px</td>  <td>position x / lat (degrees only)</td>  </tr>  <tr>  <td>py</td>  <td>position y / lon (degrees only) </td>  </tr>  <tr>  <td>pz</td>  <td>position z</td>  </tr> <tr>  <td>qx</td>  <td>quaternion x</td>  </tr> <tr>  <td>qy</td>  <td>quaternion y</td>  </tr> <tr>  <td>qz</td>  <td>quaternion z</td>  </tr> <tr>  <td>qw</td>  <td>quaternion w</td>  </tr> </tr> <tr>  <td>ex</td>  <td>euler angle x</td>  </tr> </tr> <tr>  <td>ey</td>  <td>euler angle y</td>  </tr> </tr> <tr>  <td>ez</td>  <td>euler angle z</td>  </tr> </tr> <tr>  <td>vx</td>  <td>speed x</td>  </tr> </tr> <tr>  <td>vy</td>  <td>speed y</td>  </tr> </tr> <tr>  <td>vz</td>  <td>speed z</td>  </tr> </tr> </tbody>  </table> Example: "#fields t,px,py,pz" Note: The only column that is allowed to appear multiple times is the "t" column. |
+| #delimiter | Delimiter used to separate the columns within the file. Default: "," |
+| #nframe | Definition of the navigation-frame the orientations of the trajectory refer to. Choices: "enu": East North Up or "ned": North East Down. Default: "enu" |
+| #rot_unit | Unit of the orientations. Choices: "deg": Degree, "rad": Radians. Default: "rad" |
+| #time_format | Format of the timestamps / dates. Choices: "unix": Unix timestamps (since 01-01-1970), "datetime": Human readable date-times. Default: "unix" |
+| #time_offset | Offset in seconds that is applied to the imported timestamps. Default: 0.0 |
+| #datetime_format | Format of the datetimes. Only relevant if "time_format" is "datetime". Default: "%Y-%m-%d %H:%M:%S.%f" |
+| #datetime_timezone | Time zone of the timestamps. During import, all timestamps are converted to UTC considering the input time zone. Choices: [Time zone](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) or "GPS" |
+| #sorting | Sorting of the input data. Choices: "chrono": Chronologically sorted data (usually the case), "spatial": Spatially sorted data, i.e. along the arc length. Default: "chrono" |
+| #state | States describing what processing steps the data already has passed. States: "approximated", "interpolated", "intersected", "aligned", "matched", "sorting_known" |
+
+## Aligning Trajectories
+The trajectories to be compared could be defined in different coordinate systems and/or refer to different positions on the same platform due to different mounting positions. There may also be a small synchronization offset. To solve this problem, trajectopy provides functionality to align two trajectories using least squares adjustment theory. This allows estimation of up to 11 parameters, all of which can be turned on or off individually to tailor the alignment to the sensor modalities. The alignment settings can be found in the right-click trajectory settings.
+
+### Alignment Settings
+| Setting | Description |
+|---|---|
+| Minimum Speed | If set to a value larger than 0.0, only poses with a speed higher than the specified value are used for alignment. This is only relevant for the time shift estimation where higher speed usually lead to better results. |
+| Time Start, Time End | Time range given in seconds relative to the start of the trajectory that should be aligned. If set to non-zero values, only poses in the specified time span are used for alignment. |
+| Error Probability | Used for stochastic tests. During the alignment, the functional relationship and the stochastic model are tested for consistency. Besides a global test, there are also tests for each observation group. Observation groups are:  xy_from, z_from, xy_to, z_to, roll_pitch, yaw, speed. |
+| Observation Standard Deviations | Standard deviations of the trajectory data involved. |
+| Estimation Of | Toggle for individual parameters that should be estimated. Furthermore, the user can specify which components of the 3d speed vector should be used for time shift estimation. |
+
+Parameters that can be estimated:
+- Similarity x translation
+- Similarity y translation
+- Similarity z translation
+- Similarity x rotation
+- Similarity y rotation
+- Similarity z rotation
+- Similarity scale
+- (small) Time shift
+- Lever arm x
+- Lever arm y
+- Lever arm z
+
+Both trajectories should be roughly synchronized to improve trajectory matching before alignment.
+
+
+## Comparing Trajectories
+This toolbox allows the comparison of two trajectories using absolute and relative metrics. Before comparison, both trajectories to be compared must be matched. After this, either absolute or relative metrics can be computed.
+
+### Matching
+There are three different types of trajectory matching implemented in trajectopy:
+* Matching via interpolation: Poses are matched by interpolating one trajectory onto the timestamps of the other.
+* Matching via Nearest Temporal Neighbor: Poses are matched using their timestamps while considering some pre-defined tolerance.
+* Matching via Nearest Spatial Neighbor: Poses are matched using their nearest neighbors while considering some pre-defined distance tolerance.
+
+Matching tolerances can be set in the settings of the corresponding trajectory.
+
+### Absolute
+This metric is often referred to as Absolute Trajectory Error (ATE). It measures the translational and rotational difference between two matched poses. By default, trajectopy splits the deviations into vertical cross-track, horizontal cross-track, and along-track deviations to simplify interpretation. This behavior can be turned off.
+
+### Relative
+For this metric, relative pose-pair differences are compared. The distance between two poses can be specified by the user and can be either time- or distance-based. The comparison involves finding pose pairs separated by a specific distance or time interval, computing the relative translation and rotation between the reference and estimated pose pairs, and calculating the translational and rotational difference normalized by the distance or time that separated the poses.
+
+1. Find pose pair separated by e.g. 100 m in reference trajectory
+2. Find corresponding pose pair in estimated trajectory
+3. Compute relative translation and rotation between the reference pose pair
+4. Compute relative translation and rotation between the estimated pose pair
+5. Compute translational and rotational difference between 3) and 4)
+6. Divide 5) by the distance or the time that separated both poses (e.g. 100 m).
+
+Units are m/m: %, deg/m for distance based comparison and m/s, deg/s for time-based comparison. Pose distances can be set in the settings of the corresponding trajectory. Furthermore, the user can choose to either use consecutive pose pairs (non-overlapping) or all posible pairs (overlapping).
+
+## Spatial Sorting
+When dealing with repeated trajectories, it may be useful to spatially sort the trajectory for further analysis. This reconstructs the point order as a function of the trajectory length. Trajectopy uses a combination of an iterative voxel-based moving least-squares approximation and a minimum spanning tree to solve this problem.
+
+The point cloud is divided into voxels of a given size. Then, for each point, a number of neighboring voxels are requested. A 3D line is estimated using the points within these voxels. Finally, the current point is projected onto the line to obtain the approximated point. The spatial sorting of this MLS approximation is reconstructed using a minimum spanning tree. Depending on the algorithm, colinear points are discarded in this step.
+
+## Approximation
+The trajectory can be approximated using piecewise cubic polynomials for the positions and sliding window based smoothing for the rotations. The window sizes and the minimum number of observations that should be within an interval can be set by the user.
+
+## Sessions
+Sessions allow you to export all imported and computed trajectories and results into a folder. This folder can be imported again after restarting trajectopy, saving time and keeping related data together.
+
+## Settings
+### Plot Settings
+| Setting | Description |
+|---|---|
+| Position Unit | Affects deviation plots only |
+| Stair Histogram | If set to true, deviation histograms are not filled and only a stair is visible. (see also matplotlib documentation) |
+| Smoothing Window Width | For better visibility in the deviation plots, the deviations are smoothed with a sliding window of a certain width. Smoothing can be turned off by setting a width of 0.0 or -1.0 |
+| Show Mean Line | Toggles the visibility of a red mean line in deviation plots. |
+| Grid Megapixels | For every scatter plot, the trajectory data is divided into a grid with a certain number of pixels that can be set with this setting. This prevents slow plotting with large trajectories. |
+| RMS Window Width | Similar to the Smoothing Window Width, this parameter sets the width of a sliding window used to smooth the RMS values that are mapped onto the trajectory in scatter plots. Smoothing can be turned off by setting a width of 0.0 or -1.0 |
+| Show Zero-Crossing in Colorbars | Each scatter plot of deviations includes a colorbar, which can be toggled to show the zero-crossing explicitly. |
+| Colorbar Step Divisor, Clip Colorbar at X Sigma | The colorbar limits are determined by either the minimum or maximum values, or by the X-sigma range ("Clip-Colorbar at X Sigma" Setting) around the mean deviation, depending on which limit is more restrictive. Starting at the lower bound, the colorbar ticks are placed at positions each separated by the total colorbar range divided by the colorbar step divisor. |
+| No axis | Toggles the visibility of axes in scatter plots |
+| Rotate Scatter Plots to Main Axis | When set to true, the scatter plot trajectories will be rotated to align their main axis of extension (determined through principal component analysis) with the x-axis. This can be beneficial for elongated trajectories. |
+
+#### Custom Matplotlib Style
+You can use a custom plotting style by placing a `custom.mplstyle` file in the directory you launched trajectopy in. For instructions on how to define custom plotting styles, please see https://matplotlib.org/stable/tutorials/introductory/customizing.html.
+Below you can see the default style of trajectopy
+```python
+figure.figsize: 8, 6
+figure.facecolor: white
+font.size: 14
+font.family: serif
+axes.prop_cycle: cycler("color", ["1E88E5", "#FFC107", "#004D40", "#D81B60", "#2bd2bb", "#a3bbf1", "#3c41fd", "#cc5510", "#3b0732", "#88122b", "#bccb70", "dc9c54"])
+axes.facecolor: E2E2E2
+axes.edgecolor: white
+axes.grid: True
+grid.color: white
+grid.linewidth: 0.3
+axes.grid.which: major
+axes.axisbelow: True
+legend.facecolor: white
+lines.linestyle: -
+lines.marker: .
+savefig.dpi: 1500
+savefig.format: pdf
+```
+
```

#### html2text {}

```diff
@@ -1,39 +1,55 @@
-# Trajectopy - Trajectory Evaluation in Python Welcome to Trajectopy, a Python
-package designed to simplify the alignment and comparison of trajectories using
-an intuitive graphical user interface (GUI). ![](.images/main_gui.png) ## Key
-Features Trajectopy offers a range of features, including: - Interactive GUI: A
-user-friendly interface that enables seamless interaction with your trajectory
-data, making it easy to visualize, align, and compare trajectories. - Alignment
-Algorithm: An advanced algorithm that can be tailored to the specific
-application and supports a similarity transformation, a leverarm and a time
-shift estimation. - Comparison Metrics: Absolute and relative comparison
-metrics that can be computed using various pose-matching methods - Data Import/
-Export: Support for importing and exporting data, ensuring compatibility with
-your existing workflows. - Customizable Visualization: A flexible visualization
-that allows users to customize plot styles, tailoring the output to their
-specific needs. ## Installation Clone this repository using: ```console $ git
-clone https://github.com/gereon-t/trajectopy.git ``` ```console cd trajectopy
-``` Install ``` python3 -m pip install -e . ``` Run ``` trajectopy ``` ##
-Importing Trajectories Trajectories can be imported using the "Add" button
-below the trajectory table or by dragging files into the area of the trajectory
-table. Trajectory files must be ASCII files with a csv-like layout, by default,
-trajectopy filters for the ".traj" extension. The default column structure that
-can be read without any configuration is the following: | time | position x |
-position y | position z | quaternion x | quaternion y | quaternion z |
-quaternion w | |---|---|---|---|---|---|---|---| Columns are expected to be
-separated by commas by default. It is recommended to provide a header at the
-beginning of the trajectory file. Header entries always begin with a "#". Below
-you can find a table of all allowed header entries and their meaning. | Header
-| Description | |---|---| | #name | The name provided here is displayed in the
-table view and in plots of the trajectory | | #epsg | [EPSG Code](https://
-epsg.io/) of the datum of the input positions. Required, if geodetic datum
-transformations are desired. Default: 0, meaning local coordinates without any
-known geodetic datum | | #fields | Describes the columns of the ASCII
-trajectory file. Separated with commas.
+Metadata-Version: 2.1 Name: trajectopy Version: 0.1.8 Summary: Trajectory
+Evaluation in Python Home-page: https://github.com/gereon-t/trajectopy License:
+GPLv3 Keywords:
+trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics Author:
+Gereon Tombrink Author-email: tombrink@igg.uni-bonn.de Requires-Python:
+>=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: PyQt6 (>=6.4.2) Requires-
+Dist: PyQt6-Qt6 (>=6.4.2) Requires-Dist: PyQt6-sip (>=13.4.1) Requires-Dist:
+PyYAML (>=6.0) Requires-Dist: autograd (>=1.5) Requires-Dist: matplotlib
+(>=3.6.3) Requires-Dist: networkx (>=3.0) Requires-Dist: numpy (>=1.24.1)
+Requires-Dist: pandas (>=1.5.3) Requires-Dist: pointset (>=0.1.5) Requires-
+Dist: scipy (>=1.10.0) Requires-Dist: seaborn (>=0.12.2) Project-URL:
+Repository, https://github.com/gereon-t/trajectopy.git Description-Content-
+Type: text/markdown # Trajectopy - Trajectory Evaluation in Python Welcome to
+Trajectopy, a Python package designed to simplify the alignment and comparison
+of trajectories using an intuitive graphical user interface (GUI). ![](.images/
+main_gui.png) ![](.images/evaluation_example.png) ## Key Features Trajectopy
+offers a range of features, including: - Interactive GUI: A user-friendly
+interface that enables seamless interaction with your trajectory data, making
+it easy to visualize, align, and compare trajectories. - Alignment Algorithm:
+An advanced algorithm that can be tailored to the specific application and
+supports a similarity transformation, a leverarm and a time shift estimation. -
+Comparison Metrics: Absolute and relative comparison metrics that can be
+computed using various pose-matching methods - Data Import/Export: Support for
+importing and exporting data, ensuring compatibility with your existing
+workflows. - Customizable Visualization: A flexible visualization that allows
+users to customize plot styles, tailoring the output to their specific needs.
+## Installation Using pip: ```console pip install trajectopy ``` Or using the
+repository: ```console $ git clone https://github.com/gereon-t/trajectopy.git
+``` ```console cd trajectopy ``` Install ``` python3 -m pip install -e . ```
+Run ``` trajectopy ``` ## Importing Trajectories Trajectories can be imported
+using the "Add" button below the trajectory table or by dragging files into the
+area of the trajectory table. Trajectory files must be ASCII files with a csv-
+like layout, by default, trajectopy filters for the ".traj" extension. The
+default column structure that can be read without any configuration is the
+following: | time | position x | position y | position z | quaternion x |
+quaternion y | quaternion z | quaternion w | |---|---|---|---|---|---|---|---
+| Columns are expected to be separated by commas by default. It is recommended
+to provide a header at the beginning of the trajectory file. Header entries
+always begin with a "#". Below you can find a table of all allowed header
+entries and their meaning. | Header | Description | |---|---| | #name | The
+name provided here is displayed in the table view and in plots of the
+trajectory | | #epsg | [EPSG Code](https://epsg.io/) of the datum of the input
+positions. Required, if geodetic datum transformations are desired. Default: 0,
+meaning local coordinates without any known geodetic datum | | #fields |
+Describes the columns of the ASCII trajectory file. Separated with commas.
 t  time
 l  arc lengths in meters
 px position x / lat (degrees only)
 py position y / lon (degrees only)
 pz position z
 qx quaternion x
 qy quaternion y
@@ -84,92 +100,94 @@
 Observation groups are: xy_from, z_from, xy_to, z_to, roll_pitch, yaw, speed. |
 | Observation Standard Deviations | Standard deviations of the trajectory data
 involved. | | Estimation Of | Toggle for individual parameters that should be
 estimated. Furthermore, the user can specify which components of the 3d speed
 vector should be used for time shift estimation. | Parameters that can be
 estimated: - Similarity x translation - Similarity y translation - Similarity z
 translation - Similarity x rotation - Similarity y rotation - Similarity z
-rotation - Similarity scale - Time shift - Lever arm x - Lever arm y - Lever
-arm z ## Comparing Trajectories This toolbox allows the comparison of two
-trajectories using absolute and relative metrics. Before comparison, both
-trajectories to be compared must be matched. After this, either absolute or
-relative metrics can be computed. ### Matching There are three different types
-of trajectory matching implemented in trajectopy: * Matching via interpolation:
-Poses are matched by interpolating one trajectory onto the timestamps of the
-other. * Matching via Nearest Temporal Neighbor: Poses are matched using their
-timestamps while considering some pre-defined tolerance. * Matching via Nearest
-Spatial Neighbor: Poses are matched using their nearest neighbors while
-considering some pre-defined distance tolerance. Matching tolerances can be set
-in the settings of the corresponding trajectory. ### Absolute This metric is
-often referred to as Absolute Trajectory Error (ATE). It measures the
-translational and rotational difference between two matched poses. By default,
-trajectopy splits the deviations into vertical cross-track, horizontal cross-
-track, and along-track deviations to simplify interpretation. This behavior can
-be turned off. ### Relative For this metric, relative pose-pair differences are
-compared. The distance between two poses can be specified by the user and can
-be either time- or distance-based. The comparison involves finding pose pairs
-separated by a specific distance or time interval, computing the relative
-translation and rotation between the reference and estimated pose pairs, and
-calculating the translational and rotational difference normalized by the
-distance or time that separated the poses. 1. Find pose pair separated by e.g.
-100 m in reference trajectory 2. Find corresponding pose pair in estimated
-trajectory 3. Compute relative translation and rotation between the reference
-pose pair 4. Compute relative translation and rotation between the estimated
-pose pair 5. Compute translational and rotational difference between 3) and 4)
-6. Divide 5) by the distance or the time that separated both poses (e.g. 100
-m). Units are m/m: %, deg/m for distance based comparison and m/s, deg/s for
-time-based comparison. Pose distances can be set in the settings of the
-corresponding trajectory. Furthermore, the user can choose to either use
-consecutive pose pairs (non-overlapping) or all posible pairs (overlapping). ##
-Spatial Sorting When dealing with repeated trajectories, it may be useful to
-spatially sort the trajectory for further analysis. This reconstructs the point
-order as a function of the trajectory length. Trajectopy uses a combination of
-an iterative voxel-based moving least-squares approximation and a minimum
-spanning tree to solve this problem. The point cloud is divided into voxels of
-a given size. Then, for each point, a number of neighboring voxels are
-requested. A 3D line is estimated using the points within these voxels.
-Finally, the current point is projected onto the line to obtain the
-approximated point. The spatial sorting of this MLS approximation is
-reconstructed using a minimum spanning tree. Depending on the algorithm,
-colinear points are discarded in this step. ## Approximation The trajectory can
-be approximated using piecewise cubic polynomials for the positions and sliding
-window based smoothing for the rotations. The window sizes and the minimum
-number of observations that should be within an interval can be set by the
-user. ## Sessions Sessions allow you to export all imported and computed
-trajectories and results into a folder. This folder can be imported again after
-restarting trajectopy, saving time and keeping related data together. ##
-Settings ### Plot Settings | Setting | Description | |---|---| | Position Unit
-| Affects deviation plots only | | Stair Histogram | If set to true, deviation
-histograms are not filled and only a stair is visible. (see also matplotlib
-documentation) | | Smoothing Window Width | For better visibility in the
-deviation plots, the deviations are smoothed with a sliding window of a certain
-width. Smoothing can be turned off by setting a width of 0.0 or -1.0 | | Show
-Mean Line | Toggles the visibility of a red mean line in deviation plots. | |
-Grid Megapixels | For every scatter plot, the trajectory data is divided into a
-grid with a certain number of pixels that can be set with this setting. This
-prevents slow plotting with large trajectories. | | RMS Window Width | Similar
-to the Smoothing Window Width, this parameter sets the width of a sliding
-window used to smooth the RMS values that are mapped onto the trajectory in
-scatter plots. Smoothing can be turned off by setting a width of 0.0 or -1.0 |
-| Show Zero-Crossing in Colorbars | Each scatter plot of deviations includes a
-colorbar, which can be toggled to show the zero-crossing explicitly. | |
-Colorbar Step Divisor, Clip Colorbar at X Sigma | The colorbar limits are
-determined by either the minimum or maximum values, or by the X-sigma range
-("Clip-Colorbar at X Sigma" Setting) around the mean deviation, depending on
-which limit is more restrictive. Starting at the lower bound, the colorbar
-ticks are placed at positions each separated by the total colorbar range
-divided by the colorbar step divisor. | | No axis | Toggles the visibility of
-axes in scatter plots | | Rotate Scatter Plots to Main Axis | When set to true,
-the scatter plot trajectories will be rotated to align their main axis of
-extension (determined through principal component analysis) with the x-axis.
-This can be beneficial for elongated trajectories. | #### Custom Matplotlib
-Style You can use a custom plotting style by placing a `custom.mplstyle` file
-in the directory you launched trajectopy in. For instructions on how to define
-custom plotting styles, please see https://matplotlib.org/stable/tutorials/
-introductory/customizing.html. Below you can see the default style of
-trajectopy ```python figure.figsize: 8, 6 figure.facecolor: white font.size: 14
-font.family: serif axes.prop_cycle: cycler("color", ["1E88E5", "#FFC107",
-"#004D40", "#D81B60", "#2bd2bb", "#a3bbf1", "#3c41fd", "#cc5510", "#3b0732",
-"#88122b", "#bccb70", "dc9c54"]) axes.facecolor: E2E2E2 axes.edgecolor: white
-axes.grid: True grid.color: white grid.linewidth: 0.3 axes.grid.which: major
-axes.axisbelow: True legend.facecolor: white lines.linestyle: - lines.marker: .
-savefig.dpi: 1500 savefig.format: pdf ```
+rotation - Similarity scale - (small) Time shift - Lever arm x - Lever arm y -
+Lever arm z Both trajectories should be roughly synchronized to improve
+trajectory matching before alignment. ## Comparing Trajectories This toolbox
+allows the comparison of two trajectories using absolute and relative metrics.
+Before comparison, both trajectories to be compared must be matched. After
+this, either absolute or relative metrics can be computed. ### Matching There
+are three different types of trajectory matching implemented in trajectopy: *
+Matching via interpolation: Poses are matched by interpolating one trajectory
+onto the timestamps of the other. * Matching via Nearest Temporal Neighbor:
+Poses are matched using their timestamps while considering some pre-defined
+tolerance. * Matching via Nearest Spatial Neighbor: Poses are matched using
+their nearest neighbors while considering some pre-defined distance tolerance.
+Matching tolerances can be set in the settings of the corresponding trajectory.
+### Absolute This metric is often referred to as Absolute Trajectory Error
+(ATE). It measures the translational and rotational difference between two
+matched poses. By default, trajectopy splits the deviations into vertical
+cross-track, horizontal cross-track, and along-track deviations to simplify
+interpretation. This behavior can be turned off. ### Relative For this metric,
+relative pose-pair differences are compared. The distance between two poses can
+be specified by the user and can be either time- or distance-based. The
+comparison involves finding pose pairs separated by a specific distance or time
+interval, computing the relative translation and rotation between the reference
+and estimated pose pairs, and calculating the translational and rotational
+difference normalized by the distance or time that separated the poses. 1. Find
+pose pair separated by e.g. 100 m in reference trajectory 2. Find corresponding
+pose pair in estimated trajectory 3. Compute relative translation and rotation
+between the reference pose pair 4. Compute relative translation and rotation
+between the estimated pose pair 5. Compute translational and rotational
+difference between 3) and 4) 6. Divide 5) by the distance or the time that
+separated both poses (e.g. 100 m). Units are m/m: %, deg/m for distance based
+comparison and m/s, deg/s for time-based comparison. Pose distances can be set
+in the settings of the corresponding trajectory. Furthermore, the user can
+choose to either use consecutive pose pairs (non-overlapping) or all posible
+pairs (overlapping). ## Spatial Sorting When dealing with repeated
+trajectories, it may be useful to spatially sort the trajectory for further
+analysis. This reconstructs the point order as a function of the trajectory
+length. Trajectopy uses a combination of an iterative voxel-based moving least-
+squares approximation and a minimum spanning tree to solve this problem. The
+point cloud is divided into voxels of a given size. Then, for each point, a
+number of neighboring voxels are requested. A 3D line is estimated using the
+points within these voxels. Finally, the current point is projected onto the
+line to obtain the approximated point. The spatial sorting of this MLS
+approximation is reconstructed using a minimum spanning tree. Depending on the
+algorithm, colinear points are discarded in this step. ## Approximation The
+trajectory can be approximated using piecewise cubic polynomials for the
+positions and sliding window based smoothing for the rotations. The window
+sizes and the minimum number of observations that should be within an interval
+can be set by the user. ## Sessions Sessions allow you to export all imported
+and computed trajectories and results into a folder. This folder can be
+imported again after restarting trajectopy, saving time and keeping related
+data together. ## Settings ### Plot Settings | Setting | Description | |---|---
+| | Position Unit | Affects deviation plots only | | Stair Histogram | If set
+to true, deviation histograms are not filled and only a stair is visible. (see
+also matplotlib documentation) | | Smoothing Window Width | For better
+visibility in the deviation plots, the deviations are smoothed with a sliding
+window of a certain width. Smoothing can be turned off by setting a width of
+0.0 or -1.0 | | Show Mean Line | Toggles the visibility of a red mean line in
+deviation plots. | | Grid Megapixels | For every scatter plot, the trajectory
+data is divided into a grid with a certain number of pixels that can be set
+with this setting. This prevents slow plotting with large trajectories. | | RMS
+Window Width | Similar to the Smoothing Window Width, this parameter sets the
+width of a sliding window used to smooth the RMS values that are mapped onto
+the trajectory in scatter plots. Smoothing can be turned off by setting a width
+of 0.0 or -1.0 | | Show Zero-Crossing in Colorbars | Each scatter plot of
+deviations includes a colorbar, which can be toggled to show the zero-crossing
+explicitly. | | Colorbar Step Divisor, Clip Colorbar at X Sigma | The colorbar
+limits are determined by either the minimum or maximum values, or by the X-
+sigma range ("Clip-Colorbar at X Sigma" Setting) around the mean deviation,
+depending on which limit is more restrictive. Starting at the lower bound, the
+colorbar ticks are placed at positions each separated by the total colorbar
+range divided by the colorbar step divisor. | | No axis | Toggles the
+visibility of axes in scatter plots | | Rotate Scatter Plots to Main Axis |
+When set to true, the scatter plot trajectories will be rotated to align their
+main axis of extension (determined through principal component analysis) with
+the x-axis. This can be beneficial for elongated trajectories. | #### Custom
+Matplotlib Style You can use a custom plotting style by placing a
+`custom.mplstyle` file in the directory you launched trajectopy in. For
+instructions on how to define custom plotting styles, please see https://
+matplotlib.org/stable/tutorials/introductory/customizing.html. Below you can
+see the default style of trajectopy ```python figure.figsize: 8, 6
+figure.facecolor: white font.size: 14 font.family: serif axes.prop_cycle:
+cycler("color", ["1E88E5", "#FFC107", "#004D40", "#D81B60", "#2bd2bb",
+"#a3bbf1", "#3c41fd", "#cc5510", "#3b0732", "#88122b", "#bccb70", "dc9c54"])
+axes.facecolor: E2E2E2 axes.edgecolor: white axes.grid: True grid.color: white
+grid.linewidth: 0.3 axes.grid.which: major axes.axisbelow: True
+legend.facecolor: white lines.linestyle: - lines.marker: . savefig.dpi: 1500
+savefig.format: pdf ```
```

### Comparing `trajectopy-0.1.7/trajectopy/LICENSE` & `trajectopy-0.1.8/trajectopy/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/__main__.py` & `trajectopy-0.1.8/trajectopy/__main__.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/alignment/alignment.py` & `trajectopy-0.1.8/trajectopy/alignment/alignment.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/alignment/data.py` & `trajectopy-0.1.8/trajectopy/alignment/data.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/alignment/direct_helmert_transformation.py` & `trajectopy-0.1.8/trajectopy/alignment/direct_helmert_transformation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/alignment/direct_leverarm.py` & `trajectopy-0.1.8/trajectopy/alignment/direct_leverarm.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/alignment/direct_timeshift.py` & `trajectopy-0.1.8/trajectopy/alignment/direct_timeshift.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/alignment/functional_model/equations.py` & `trajectopy-0.1.8/trajectopy/alignment/functional_model/equations.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/alignment/functional_model/interface.py` & `trajectopy-0.1.8/trajectopy/alignment/functional_model/interface.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/alignment/parameters.py` & `trajectopy-0.1.8/trajectopy/alignment/parameters.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/alignment/util.py` & `trajectopy-0.1.8/trajectopy/alignment/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/approximation/cubic_approximation.py` & `trajectopy-0.1.8/trajectopy/approximation/cubic_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/approximation/mls_approximation.py` & `trajectopy-0.1.8/trajectopy/approximation/mls_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/approximation/rot_approximation.py` & `trajectopy-0.1.8/trajectopy/approximation/rot_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/approximation/trajectory_approximation.py` & `trajectopy-0.1.8/trajectopy/approximation/trajectory_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/approximation/util.py` & `trajectopy-0.1.8/trajectopy/approximation/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/approximation/voxelizer.py` & `trajectopy-0.1.8/trajectopy/approximation/voxelizer.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/evaluation/comparison.py` & `trajectopy-0.1.8/trajectopy/evaluation/comparison.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/evaluation/matching.py` & `trajectopy-0.1.8/trajectopy/evaluation/matching.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/evaluation/trajectory_deviations.py` & `trajectopy-0.1.8/trajectopy/evaluation/trajectory_deviations.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/main_window.py` & `trajectopy-0.1.8/trajectopy/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/managers/file_manager.py` & `trajectopy-0.1.8/trajectopy/gui/managers/file_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/managers/manager.py` & `trajectopy-0.1.8/trajectopy/gui/managers/manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/managers/plot_manager.py` & `trajectopy-0.1.8/trajectopy/gui/managers/plot_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 mail@gtombrink.de
 """
 import logging
 from trajectopy.gui.managers.manager import Manager
 from trajectopy.gui.models.entry import AbsoluteDeviationEntry
 from trajectopy.gui.requests.plot_requests import PlotRequest, PlotRequestType
 from trajectopy.gui.requests.ui_request import UIRequest, UIRequestType
-from trajectopy.plotting.image_request import TIMImageRequester
 from trajectopy.settings.plot_settings import PlotSettings
 
 from trajectopy.plotting.plot_tabs import PlotTabs
 from PyQt6.QtCore import pyqtSlot
 
 logger = logging.getLogger("root")
```

### Comparing `trajectopy-0.1.7/trajectopy/gui/managers/session_manager.py` & `trajectopy-0.1.8/trajectopy/gui/managers/session_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/managers/trajectory_manager.py` & `trajectopy-0.1.8/trajectopy/gui/managers/trajectory_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/managers/ui_manager.py` & `trajectopy-0.1.8/trajectopy/gui/managers/ui_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/models/entry.py` & `trajectopy-0.1.8/trajectopy/gui/models/entry.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/models/property_model.py` & `trajectopy-0.1.8/trajectopy/gui/models/property_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/models/result_model.py` & `trajectopy-0.1.8/trajectopy/gui/models/result_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/models/selection.py` & `trajectopy-0.1.8/trajectopy/gui/models/selection.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/models/table_model.py` & `trajectopy-0.1.8/trajectopy/gui/models/table_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/models/trajectory_model.py` & `trajectopy-0.1.8/trajectopy/gui/models/trajectory_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/requests/file_request.py` & `trajectopy-0.1.8/trajectopy/gui/requests/file_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/requests/plot_requests.py` & `trajectopy-0.1.8/trajectopy/gui/requests/plot_requests.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/requests/result_model_request.py` & `trajectopy-0.1.8/trajectopy/gui/requests/result_model_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/requests/trajectory_manager_request.py` & `trajectopy-0.1.8/trajectopy/gui/requests/trajectory_manager_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/requests/trajectory_model_request.py` & `trajectopy-0.1.8/trajectopy/gui/requests/trajectory_model_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/requests/ui_request.py` & `trajectopy-0.1.8/trajectopy/gui/requests/ui_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/resources/full-icon-poppins.png` & `trajectopy-0.1.8/trajectopy/gui/resources/full-icon-poppins.png`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/resources/icon.png` & `trajectopy-0.1.8/trajectopy/gui/resources/icon.png`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/util.py` & `trajectopy-0.1.8/trajectopy/gui/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/about_window.py` & `trajectopy-0.1.8/trajectopy/gui/views/about_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/alignment_edit_window.py` & `trajectopy-0.1.8/trajectopy/gui/views/alignment_edit_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/plot_settings_window.py` & `trajectopy-0.1.8/trajectopy/gui/views/plot_settings_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,85 +118,58 @@
         self.formLayout_general.setLabelAlignment(Qt.AlignmentFlag.AlignLeft)
         self.formLayout_general.setFormAlignment(Qt.AlignmentFlag.AlignRight)
         self.formLayout_general.setObjectName("formLayout_general")
         self.general_label = QtWidgets.QLabel(self.verticalLayoutWidget)
         self.general_label.setFont(font)
         self.general_label.setObjectName("label")
         self.formLayout_general.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.general_label)
-        self.request_image_label = QtWidgets.QLabel(self.verticalLayoutWidget)
-        self.request_image_label.setObjectName("request_image_label")
-        self.formLayout_general.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.request_image_label)
-        self.requestImageCheckBox = QtWidgets.QCheckBox(self.verticalLayoutWidget)
-        self.requestImageCheckBox.setText("")
-        self.requestImageCheckBox.setObjectName("requestImageCheckBox")
-        self.formLayout_general.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.requestImageCheckBox)
-        self.image_width_label = QtWidgets.QLabel(self.verticalLayoutWidget)
-        self.image_width_label.setObjectName("image_width_label")
-        self.formLayout_general.setWidget(2, QtWidgets.QFormLayout.ItemRole.LabelRole, self.image_width_label)
-        self.imagewidthSpinbox = QtWidgets.QSpinBox(self.verticalLayoutWidget)
-        self.imagewidthSpinbox.setMinimum(1)
-        self.imagewidthSpinbox.setMaximum(1000)
-        self.imagewidthSpinbox.setProperty("value", 100)
-        self.imagewidthSpinbox.setObjectName("imagewidthSpinbox")
-        self.formLayout_general.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.imagewidthSpinbox)
-        self.image_height_label = QtWidgets.QLabel(self.verticalLayoutWidget)
-        self.image_height_label.setObjectName("image_height_label")
-        self.formLayout_general.setWidget(3, QtWidgets.QFormLayout.ItemRole.LabelRole, self.image_height_label)
-        self.imageheightSpinBox = QtWidgets.QSpinBox(self.verticalLayoutWidget)
-        self.imageheightSpinBox.setMinimum(1)
-        self.imageheightSpinBox.setMaximum(1000)
-        self.imageheightSpinBox.setProperty("value", 100)
-        self.imageheightSpinBox.setObjectName("imageheightSpinBox")
-        self.formLayout_general.setWidget(3, QtWidgets.QFormLayout.ItemRole.FieldRole, self.imageheightSpinBox)
         self.positionUnitLabel = QtWidgets.QLabel(self.verticalLayoutWidget)
         self.positionUnitLabel.setObjectName("positionUnitLabel")
-        self.formLayout_general.setWidget(4, QtWidgets.QFormLayout.ItemRole.LabelRole, self.positionUnitLabel)
+        self.formLayout_general.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.positionUnitLabel)
         self.positionUnitComboBox = QtWidgets.QComboBox(self.verticalLayoutWidget)
         self.positionUnitComboBox.setObjectName("positionUnitComboBox")
         self.positionUnitComboBox.addItem("")
         self.positionUnitComboBox.addItem("")
-        self.formLayout_general.setWidget(4, QtWidgets.QFormLayout.ItemRole.FieldRole, self.positionUnitComboBox)
+        self.formLayout_general.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.positionUnitComboBox)
         self.stairHistogramLabel = QtWidgets.QLabel(self.verticalLayoutWidget)
         self.stairHistogramLabel.setObjectName("stairHistogramLabel")
-        self.formLayout_general.setWidget(5, QtWidgets.QFormLayout.ItemRole.LabelRole, self.stairHistogramLabel)
+        self.formLayout_general.setWidget(2, QtWidgets.QFormLayout.ItemRole.LabelRole, self.stairHistogramLabel)
         self.stairHistogramCheckBox = QtWidgets.QCheckBox(self.verticalLayoutWidget)
         self.stairHistogramCheckBox.setObjectName("stairHistogramCheckBox")
-        self.formLayout_general.setWidget(5, QtWidgets.QFormLayout.ItemRole.FieldRole, self.stairHistogramCheckBox)
+        self.formLayout_general.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.stairHistogramCheckBox)
         self.smoothingWindowWidthMLabel = QtWidgets.QLabel(self.verticalLayoutWidget)
         self.smoothingWindowWidthMLabel.setObjectName("smoothingWindowWidthMLabel")
-        self.formLayout_general.setWidget(
-            10, QtWidgets.QFormLayout.ItemRole.LabelRole, self.smoothingWindowWidthMLabel
-        )
+        self.formLayout_general.setWidget(3, QtWidgets.QFormLayout.ItemRole.LabelRole, self.smoothingWindowWidthMLabel)
         self.smoothingWindowWidthMDoubleSpinBox = QtWidgets.QDoubleSpinBox(self.verticalLayoutWidget)
         self.smoothingWindowWidthMDoubleSpinBox.setMaximum(1000.0)
         self.smoothingWindowWidthMDoubleSpinBox.setSingleStep(0.1)
         self.smoothingWindowWidthMDoubleSpinBox.setProperty("value", 1.0)
         self.smoothingWindowWidthMDoubleSpinBox.setObjectName("smoothingWindowWidthMDoubleSpinBox")
         self.formLayout_general.setWidget(
-            10, QtWidgets.QFormLayout.ItemRole.FieldRole, self.smoothingWindowWidthMDoubleSpinBox
+            3, QtWidgets.QFormLayout.ItemRole.FieldRole, self.smoothingWindowWidthMDoubleSpinBox
         )
         self.showMeanLineLabel = QtWidgets.QLabel(self.verticalLayoutWidget)
         self.showMeanLineLabel.setObjectName("showMeanLineLabel")
-        self.formLayout_general.setWidget(6, QtWidgets.QFormLayout.ItemRole.LabelRole, self.showMeanLineLabel)
+        self.formLayout_general.setWidget(4, QtWidgets.QFormLayout.ItemRole.LabelRole, self.showMeanLineLabel)
         self.showMeanLineCheckBox = QtWidgets.QCheckBox(self.verticalLayoutWidget)
         self.showMeanLineCheckBox.setObjectName("showMeanLineCheckBox")
-        self.formLayout_general.setWidget(6, QtWidgets.QFormLayout.ItemRole.FieldRole, self.showMeanLineCheckBox)
+        self.formLayout_general.setWidget(4, QtWidgets.QFormLayout.ItemRole.FieldRole, self.showMeanLineCheckBox)
         self.showDirectedDeviationsAlongCrossVerticalLabel = QtWidgets.QLabel(self.verticalLayoutWidget)
         self.showDirectedDeviationsAlongCrossVerticalLabel.setObjectName(
             "showDirectedDeviationsAlongCrossVerticalLabel"
         )
         self.formLayout_general.setWidget(
-            7, QtWidgets.QFormLayout.ItemRole.LabelRole, self.showDirectedDeviationsAlongCrossVerticalLabel
+            5, QtWidgets.QFormLayout.ItemRole.LabelRole, self.showDirectedDeviationsAlongCrossVerticalLabel
         )
         self.showDirectedDeviationsAlongCrossVerticalCheckBox = QtWidgets.QCheckBox(self.verticalLayoutWidget)
         self.showDirectedDeviationsAlongCrossVerticalCheckBox.setObjectName(
             "showDirectedDeviationsAlongCrossVerticalCheckBox"
         )
         self.formLayout_general.setWidget(
-            7, QtWidgets.QFormLayout.ItemRole.FieldRole, self.showDirectedDeviationsAlongCrossVerticalCheckBox
+            5, QtWidgets.QFormLayout.ItemRole.FieldRole, self.showDirectedDeviationsAlongCrossVerticalCheckBox
         )
         self.verticalLayout_general.addLayout(self.formLayout_general)
         spacerItem = QtWidgets.QSpacerItem(
             20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding
         )
         self.verticalLayout_general.addItem(spacerItem)
         self.horizontalLayout_forms.addLayout(self.verticalLayout_general)
@@ -319,17 +292,14 @@
         self.retranslateUi()
         QtCore.QMetaObject.connectSlotsByName(self)
 
     def retranslateUi(self):
         _translate = QtCore.QCoreApplication.translate
         self.setWindowTitle(_translate("MainWindow", "Plot Settings"))
         self.general_label.setText(_translate("MainWindow", "General Settings"))
-        self.request_image_label.setText(_translate("MainWindow", "Request Aerial Image:"))
-        self.image_width_label.setText(_translate("MainWindow", "Image Width [m]:"))
-        self.image_height_label.setText(_translate("MainWindow", "Image Height [m]:"))
         self.positionUnitLabel.setText(_translate("MainWindow", "Position Unit:"))
         self.positionUnitComboBox.setItemText(0, _translate("MainWindow", "mm"))
         self.positionUnitComboBox.setItemText(1, _translate("MainWindow", "m"))
         self.stairHistogramLabel.setText(_translate("MainWindow", "Stair Histogram:"))
         self.smoothingWindowWidthMLabel.setText(_translate("MainWindow", "Smoothing Window Width [m]:"))
         self.showMeanLineLabel.setText(_translate("MainWindow", "Show Mean Line:"))
         self.showDirectedDeviationsAlongCrossVerticalLabel.setText(
@@ -343,34 +313,28 @@
         self.clipColorbarAtXSigmaLabel.setText(_translate("MainWindow", "Clip Colorbar at X Sigma:"))
         self.doNotPlotAxisLabel.setText(_translate("MainWindow", "Do Not Plot Axis:"))
         self.rotateScatterPlotsToMainAxisLabel.setText(_translate("MainWindow", "Rotate Scatter Plots to Main Axis:"))
         self.cancelButton.setText(_translate("MainWindow", "Cancel"))
         self.okButton.setText(_translate("MainWindow", "OK"))
 
     def update_view(self) -> None:
-        self.requestImageCheckBox.setChecked(self.settings.request_aerial_image)
-        self.imageheightSpinBox.setValue(self.settings.image_height)
-        self.imagewidthSpinbox.setValue(self.settings.image_width)
         self.gridMegapixelsDoubleSpinBox.setValue(self.settings.grid_mp)
         self.rMSWindowWidthMDoubleSpinBox.setValue(self.settings.rms_window_width)
         self.smoothingWindowWidthMDoubleSpinBox.setValue(self.settings.smoothing_window_size)
         self.positionUnitComboBox.setCurrentIndex(0 if self.settings.unit_is_mm else 1)
         self.showZeroCrossingInColorbarsCheckBox.setChecked(self.settings.always_show_zero)
         self.colorbarStepDivisorSpinBox.setValue(self.settings.c_bar_step_divisor)
         self.clipColorbarAtXSigmaDoubleSpinBox.setValue(self.settings.scatter_sigma_factor)
         self.doNotPlotAxisCheckBox.setChecked(self.settings.scatter_no_axis)
         self.rotateScatterPlotsToMainAxisCheckBox.setChecked(self.settings.scatter_rotate)
         self.stairHistogramCheckBox.setChecked(self.settings.hist_as_stairs)
         self.showMeanLineCheckBox.setChecked(self.settings.show_mean_line)
         self.showDirectedDeviationsAlongCrossVerticalCheckBox.setChecked(self.settings.show_directed_devs)
 
     def update_model(self) -> None:
-        self.settings.request_aerial_image = self.requestImageCheckBox.isChecked()
-        self.settings.image_height = self.imageheightSpinBox.value()
-        self.settings.image_width = self.imagewidthSpinbox.value()
         self.settings.grid_mp = self.gridMegapixelsDoubleSpinBox.value()
         self.settings.rms_window_width = self.rMSWindowWidthMDoubleSpinBox.value()
         self.settings.smoothing_window_size = self.smoothingWindowWidthMDoubleSpinBox.value()
         self.settings.unit_is_mm = self.positionUnitComboBox.currentIndex() == 0
         self.settings.always_show_zero = self.showZeroCrossingInColorbarsCheckBox.isChecked()
         self.settings.c_bar_step_divisor = self.colorbarStepDivisorSpinBox.value()
         self.settings.scatter_sigma_factor = self.clipColorbarAtXSigmaDoubleSpinBox.value()
```

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/progress_window.py` & `trajectopy-0.1.8/trajectopy/gui/views/progress_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/properties_window.py` & `trajectopy-0.1.8/trajectopy/gui/views/properties_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/result_context_menu.py` & `trajectopy-0.1.8/trajectopy/gui/views/result_context_menu.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/result_selection_window.py` & `trajectopy-0.1.8/trajectopy/gui/views/result_selection_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/result_table_view.py` & `trajectopy-0.1.8/trajectopy/gui/views/result_table_view.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/settings_window.py` & `trajectopy-0.1.8/trajectopy/gui/views/settings_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/trajectory_context_menu.py` & `trajectopy-0.1.8/trajectopy/gui/views/trajectory_context_menu.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/gui/views/trajectory_table_view.py` & `trajectopy-0.1.8/trajectopy/gui/views/trajectory_table_view.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/plotting/alignment_plot.py` & `trajectopy-0.1.8/trajectopy/plotting/alignment_plot.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/plotting/deviation_plot.py` & `trajectopy-0.1.8/trajectopy/plotting/deviation_plot.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/plotting/plot_tabs.py` & `trajectopy-0.1.8/trajectopy/plotting/plot_tabs.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/plotting/trajectory_plot.py` & `trajectopy-0.1.8/trajectopy/plotting/trajectory_plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
 from typing import Tuple
 
 import numpy as np
 from matplotlib import pyplot as plt
-from trajectopy.plotting.image_request import TIMImageRequester
 from trajectopy.settings.plot_settings import PlotSettings
 from matplotlib.figure import Figure
 from trajectopy.trajectory import Sorting, Trajectory
 
 
 def plot_trajectories(
     trajectories: list[Trajectory],
@@ -38,28 +37,17 @@
         ax_pos.set_zlabel("z [m]")  # type: ignore
     else:
         raise ValueError(f"Unknown dimension: {dim}")
     ax_pos.set_xlabel("x [m]")
     ax_pos.set_ylabel("y [m]")
 
     legend_names = []
-    image_requester = TIMImageRequester()
-    for i, traj in enumerate(trajectories):
+    for traj in trajectories:
         legend_names.append(traj.name)
 
-        if plot_settings.request_aerial_image and dim == 2 and traj.pos.local_transformer is not None:
-            if i == 0:
-                image, extent = image_requester.request(
-                    pointset=traj.pos.mean(), width=plot_settings.image_width, height=plot_settings.image_height
-                )
-                plt.imshow(np.array(image), aspect="auto", extent=extent)
-                ax_pos.axis("equal")
-            traj = traj.copy()
-            traj.pos.to_epsg(target_epsg=image_requester.request_epsg, inplace=True)
-
         # pos fig
         if dim == 2:
             ax_pos.plot(traj.pos.x, traj.pos.y)
         elif dim == 3:
             ax_pos.plot(traj.pos.x, traj.pos.y, traj.pos.z)
 
     if dim == 3:
```

### Comparing `trajectopy-0.1.7/trajectopy/plotting/util.py` & `trajectopy-0.1.8/trajectopy/plotting/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/settings/alignment_settings.py` & `trajectopy-0.1.8/trajectopy/settings/alignment_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/settings/approximation_settings.py` & `trajectopy-0.1.8/trajectopy/settings/approximation_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/settings/comparison_settings.py` & `trajectopy-0.1.8/trajectopy/settings/comparison_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/settings/core.py` & `trajectopy-0.1.8/trajectopy/settings/core.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/settings/plot_settings.py` & `trajectopy-0.1.8/trajectopy/settings/plot_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,14 @@
     scatter_rotate: bool = False
     unit_is_mm: bool = False
     hist_as_stairs: bool = False
     smoothing_window_size: float = 1.0
     show_mean_line: bool = True
     heatmap_spacing: float = 1.0
     show_directed_devs: bool = True
-    request_aerial_image: bool = False
-    image_width: float = 200
-    image_height: float = 200
 
     @classmethod
     def from_config_dict(cls: "Settings", config_dict: dict) -> "Settings":
         return super().from_config_dict(config_dict)
 
     @property
     def unit_multiplier(self) -> float:
```

### Comparing `trajectopy-0.1.7/trajectopy/settings/processing_settings.py` & `trajectopy-0.1.8/trajectopy/settings/processing_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/settings/sorting_settings.py` & `trajectopy-0.1.8/trajectopy/settings/sorting_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/trajectory.py` & `trajectopy-0.1.8/trajectopy/trajectory.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/util/datahandling.py` & `trajectopy-0.1.8/trajectopy/util/datahandling.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/util/definitions.py` & `trajectopy-0.1.8/trajectopy/util/definitions.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/util/path.py` & `trajectopy-0.1.8/trajectopy/util/path.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/util/printing.py` & `trajectopy-0.1.8/trajectopy/util/printing.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/util/reading.py` & `trajectopy-0.1.8/trajectopy/util/reading.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/util/rotationset.py` & `trajectopy-0.1.8/trajectopy/util/rotationset.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/util/spatialsorter.py` & `trajectopy-0.1.8/trajectopy/util/spatialsorter.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.1.7/trajectopy/util/trajectory_processing_state.py` & `trajectopy-0.1.8/trajectopy/util/trajectory_processing_state.py`

 * *Files identical despite different names*

