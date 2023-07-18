# Comparing `tmp/SpiNNUtilities-1!7.0.0a6.tar.gz` & `tmp/SpiNNUtilities-4.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpiNNUtilities-1!7.0.0a6.tar", last modified: Tue Jul 18 11:15:08 2023, max compression
+gzip compressed data, was "dist\SpiNNUtilities-4.0.0a1.tar", last modified: Tue Apr 25 20:43:35 2017, max compression
```

## Comparing `SpiNNUtilities-1!7.0.0a6.tar` & `SpiNNUtilities-4.0.0a1.tar`

### file list

```diff
@@ -1,95 +1,24 @@
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:08.726704 SpiNNUtilities-1!7.0.0a6/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5086 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/CITATION.cff
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/LICENSE
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      959 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/LICENSE_POLICY.md
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       56 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/MANIFEST.in
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     4142 2023-07-18 11:15:08.726704 SpiNNUtilities-1!7.0.0a6/PKG-INFO
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2998 2023-07-18 11:15:05.000000 SpiNNUtilities-1!7.0.0a6/README.md
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:08.718705 SpiNNUtilities-1!7.0.0a6/SpiNNUtilities.egg-info/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     4142 2023-07-18 11:15:08.000000 SpiNNUtilities-1!7.0.0a6/SpiNNUtilities.egg-info/PKG-INFO
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2935 2023-07-18 11:15:08.000000 SpiNNUtilities-1!7.0.0a6/SpiNNUtilities.egg-info/SOURCES.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-07-18 11:15:08.000000 SpiNNUtilities-1!7.0.0a6/SpiNNUtilities.egg-info/dependency_links.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       79 2023-07-18 11:15:08.000000 SpiNNUtilities-1!7.0.0a6/SpiNNUtilities.egg-info/requires.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       16 2023-07-18 11:15:08.000000 SpiNNUtilities-1!7.0.0a6/SpiNNUtilities.egg-info/top_level.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-07-18 11:15:08.000000 SpiNNUtilities-1!7.0.0a6/SpiNNUtilities.egg-info/zip-safe
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      679 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/pyproject.toml
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1406 2023-07-18 11:15:08.730704 SpiNNUtilities-1!7.0.0a6/setup.cfg
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1316 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/setup.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:08.722705 SpiNNUtilities-1!7.0.0a6/spinn_utilities/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      842 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      734 2023-07-18 11:15:05.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/_version.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     4098 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/abstract_base.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1640 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/abstract_context_manager.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1725 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/bytestring_utils.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:08.722705 SpiNNUtilities-1!7.0.0a6/spinn_utilities/citation/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      855 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/citation/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    17912 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/citation/citation_aggregator.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    13284 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/citation/citation_updater_and_doi_generator.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1309 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/classproperty.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     9630 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/conf_loader.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    13262 2023-07-11 09:03:01.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/config_holder.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1262 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/config_setup.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:08.722705 SpiNNUtilities-1!7.0.0a6/spinn_utilities/configs/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1060 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/configs/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     4057 2023-07-18 07:37:27.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/configs/camel_case_config_parser.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      818 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/configs/case_sensitive_parser.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      723 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/configs/config_template_exception.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      705 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/configs/no_config_found_exception.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      729 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/configs/unexpected_config_exception.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:08.726704 SpiNNUtilities-1!7.0.0a6/spinn_utilities/data/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      720 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/data/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1743 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/data/data_status.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1020 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/data/reset_status.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1319 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/data/run_status.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    21132 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/data/utils_data_view.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    10655 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/data/utils_data_writer.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3334 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/exceptions.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     6430 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/executable_finder.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2798 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/find_max_success.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2872 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/helpful_functions.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      994 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/index_is_value.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    10561 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/log.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1622 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/log_store.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1692 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/logger_utils.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:08.726704 SpiNNUtilities-1!7.0.0a6/spinn_utilities/make_tools/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      738 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/make_tools/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2900 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/make_tools/converter.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2263 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/make_tools/db.sql
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    25114 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/make_tools/file_converter.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     8464 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/make_tools/log_sqllite_database.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3564 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/make_tools/replacer.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:08.726704 SpiNNUtilities-1!7.0.0a6/spinn_utilities/matrix/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      842 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/matrix/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1066 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/matrix/abstract_matrix.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1071 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/matrix/demo_matrix.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2235 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/matrix/double_dict.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1008 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/matrix/x_view.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1008 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/matrix/y_view.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2609 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ordered_set.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5813 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/overrides.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     4556 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/package_loader.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2321 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ping.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    12297 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/progress_bar.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1323 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/progress_bar.txt
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:08.726704 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1366 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     9982 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/abstract_dict.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    27485 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/abstract_list.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     9413 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/abstract_sized.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3178 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/abstract_view.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2071 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/ids_view.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      989 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/multiple_values_exception.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    16416 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/range_dictionary.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    21378 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/ranged_list.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1789 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/ranged_list_of_lists.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1976 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/single_view.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2650 2023-07-05 08:30:24.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/ranged/slice_view.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2912 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/require_subclass.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3102 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/safe_eval.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2230 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/see.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3504 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/socket_address.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      189 2023-05-04 07:53:36.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/spinn_utilities.cfg
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:08.726704 SpiNNUtilities-1!7.0.0a6/spinn_utilities/testing/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      597 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/testing/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5450 2023-07-18 07:37:27.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/testing/log_checker.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3113 2023-05-24 09:16:16.000000 SpiNNUtilities-1!7.0.0a6/spinn_utilities/timer.py
+drwxrwxrwx   0        0        0        0 2017-04-25 20:43:35.000000 SpiNNUtilities-4.0.0a1/
+-rw-rw-rw-   0        0        0      295 2017-04-25 20:43:35.000000 SpiNNUtilities-4.0.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2017-04-25 20:43:35.000000 SpiNNUtilities-4.0.0a1/setup.cfg
+-rw-rw-rw-   0        0        0     1259 2017-04-25 20:42:21.000000 SpiNNUtilities-4.0.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2017-04-25 20:43:35.000000 SpiNNUtilities-4.0.0a1/SpiNNUtilities.egg-info/
+-rw-rw-rw-   0        0        0        1 2017-04-25 20:43:35.000000 SpiNNUtilities-4.0.0a1/SpiNNUtilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      295 2017-04-25 20:43:35.000000 SpiNNUtilities-4.0.0a1/SpiNNUtilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2017-04-25 20:43:35.000000 SpiNNUtilities-4.0.0a1/SpiNNUtilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      600 2017-04-25 20:43:35.000000 SpiNNUtilities-4.0.0a1/SpiNNUtilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       16 2017-04-25 20:43:35.000000 SpiNNUtilities-4.0.0a1/SpiNNUtilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2017-04-25 20:43:35.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/
+-rw-rw-rw-   0        0        0     2717 2017-03-31 08:16:22.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/abstract_base.py
+-rw-rw-rw-   0        0        0     4870 2017-03-21 12:19:48.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/conf_loader.py
+-rw-rw-rw-   0        0        0     1950 2017-03-21 12:19:49.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/executable_finder.py
+-rw-rw-rw-   0        0        0     8032 2017-03-14 12:07:22.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/helpful_functions.py
+-rw-rw-rw-   0        0        0     2894 2017-03-21 12:19:48.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/log.py
+-rw-rw-rw-   0        0        0     3054 2017-03-21 12:19:49.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/ordered_set.py
+-rw-rw-rw-   0        0        0     4439 2017-03-21 12:19:48.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/overrides.py
+-rw-rw-rw-   0        0        0     2421 2017-04-06 09:26:34.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/package_loader.py
+-rw-rw-rw-   0        0        0     5986 2017-04-19 12:27:39.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/progress_bar.py
+-rw-rw-rw-   0        0        0     1886 2017-04-07 13:16:53.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/safe_eval.py
+-rw-rw-rw-   0        0        0     1070 2017-03-14 12:07:22.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/socket_address.py
+-rw-rw-rw-   0        0        0      880 2017-03-21 12:19:49.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/timer.py
+-rw-rw-rw-   0        0        0        0 2017-03-14 12:07:22.000000 SpiNNUtilities-4.0.0a1/spinn_utilities/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

