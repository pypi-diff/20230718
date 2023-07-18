# Comparing `tmp/jupysql-0.7.9.tar.gz` & `tmp/jupysql-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupysql-0.7.9.tar", last modified: Mon Jun 19 15:52:22 2023, max compression
+gzip compressed data, was "jupysql-0.8.0.tar", last modified: Tue Jul 18 14:57:10 2023, max compression
```

## Comparing `jupysql-0.7.9.tar` & `jupysql-0.8.0.tar`

### file list

```diff
@@ -1,58 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-06-19 15:52:03.000000 jupysql-0.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-19 15:52:03.000000 jupysql-0.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-19 15:52:22.880631 jupysql-0.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-19 15:52:03.000000 jupysql-0.7.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 15:52:03.000000 jupysql-0.7.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-19 15:52:22.880631 jupysql-0.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-19 15:52:03.000000 jupysql-0.7.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.872631 jupysql-0.7.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.876631 jupysql-0.7.9/src/jupysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-19 15:52:22.000000 jupysql-0.7.9/src/jupysql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.876631 jupysql-0.7.9/src/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/column_guesser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/ggplot/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/facet_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/ggplot/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/geom/geom_boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/geom/geom_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/ggplot/ggplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/magic_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/magic_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    25298 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/query_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/sqlcmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/widgets/table_widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/table_widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/widgets/table_widget/css/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/table_widget/css/tableWidget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:22.880631 jupysql-0.7.9/src/sql/widgets/table_widget/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/table_widget/js/tableWidget.js
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/table_widget/table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-19 15:52:03.000000 jupysql-0.7.9/src/sql/widgets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-07-18 14:56:54.000000 jupysql-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-18 14:56:54.000000 jupysql-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-18 14:57:10.742658 jupysql-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-18 14:56:54.000000 jupysql-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 14:56:54.000000 jupysql-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 14:57:10.742658 jupysql-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-18 14:56:54.000000 jupysql-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.734658 jupysql-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.734658 jupysql-0.8.0/src/jupysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 14:57:10.000000 jupysql-0.8.0/src/jupysql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.738658 jupysql-0.8.0/src/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.738658 jupysql-0.8.0/src/sql/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/cmd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/cmd/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/column_guesser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.738658 jupysql-0.8.0/src/sql/ggplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/facet_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/src/sql/ggplot/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/geom/geom_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/geom/geom_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/ggplot/ggplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21240 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/magic_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/magic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/query_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24152 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/src/sql/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/src/sql/widgets/table_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/table_widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/src/sql/widgets/table_widget/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/table_widget/css/tableWidget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:57:10.742658 jupysql-0.8.0/src/sql/widgets/table_widget/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/table_widget/js/tableWidget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/table_widget/table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-18 14:56:54.000000 jupysql-0.8.0/src/sql/widgets/utils.py
```

### Comparing `jupysql-0.7.9/LICENSE` & `jupysql-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/PKG-INFO` & `jupysql-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.9
+Version: 0.8.0
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.9 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.8.0 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.9/README.md` & `jupysql-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/pyproject.toml` & `jupysql-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/setup.py` & `jupysql-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 ]
 
 DEV = [
     "flake8",
     "pytest",
     "pandas",
     "polars==0.17.2",  # 04/18/23 this breaks our CI
+    "pyarrow",
     "invoke",
     "pkgmt",
     "twine",
     # tests
     "duckdb<0.8.0",
     "duckdb-engine",
     "pyodbc",
```

### Comparing `jupysql-0.7.9/src/jupysql.egg-info/PKG-INFO` & `jupysql-0.8.0/src/jupysql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.9
+Version: 0.8.0
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.9 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.8.0 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.9/src/jupysql.egg-info/SOURCES.txt` & `jupysql-0.8.0/src/jupysql.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,18 +23,26 @@
 src/sql/magic.py
 src/sql/magic_cmd.py
 src/sql/magic_plot.py
 src/sql/parse.py
 src/sql/plot.py
 src/sql/query_util.py
 src/sql/run.py
-src/sql/sqlcmd.py
 src/sql/store.py
 src/sql/telemetry.py
 src/sql/util.py
+src/sql/warnings.py
+src/sql/cmd/__init__.py
+src/sql/cmd/cmd_utils.py
+src/sql/cmd/columns.py
+src/sql/cmd/explore.py
+src/sql/cmd/profile.py
+src/sql/cmd/snippets.py
+src/sql/cmd/tables.py
+src/sql/cmd/test.py
 src/sql/ggplot/__init__.py
 src/sql/ggplot/aes.py
 src/sql/ggplot/facet_wrap.py
 src/sql/ggplot/ggplot.py
 src/sql/ggplot/geom/__init__.py
 src/sql/ggplot/geom/geom.py
 src/sql/ggplot/geom/geom_boxplot.py
```

### Comparing `jupysql-0.7.9/src/jupysql.egg-info/requires.txt` & `jupysql-0.8.0/src/jupysql.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ipython<=8.12.0
 
 [dev]
 flake8
 pytest
 pandas
 polars==0.17.2
+pyarrow
 invoke
 pkgmt
 twine
 duckdb<0.8.0
 duckdb-engine
 pyodbc
 matplotlib
@@ -32,25 +33,25 @@
 jupysql-plugin
 
 [integration]
 flake8
 pytest
 pandas
 polars==0.17.2
+pyarrow
 invoke
 pkgmt
 twine
 duckdb<0.8.0
 duckdb-engine
 pyodbc
 matplotlib
 black
 ipywidgets
 js2py
 jupysql-plugin
 dockerctx
-pyarrow
 psycopg2-binary
 pymysql
 pgspecial==2.0.1
 snowflake-sqlalchemy
 oracledb
```

### Comparing `jupysql-0.7.9/src/sql/_patch.py` & `jupysql-0.8.0/src/sql/_patch.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/src/sql/_testing.py` & `jupysql-0.8.0/src/sql/_testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,31 @@
-from dockerctx import new_container
 from contextlib import contextmanager
 import sys
 import time
-import docker
-from docker import errors
+
 from sqlalchemy.engine import URL
 import os
 import sqlalchemy
 
+from ploomber_core.dependencies import requires
+
+# SQLite and DuckDB do not require Docker, so we make docker packages optional
+# in case we want to run those tests
+
+try:
+    from dockerctx import new_container
+except ModuleNotFoundError:
+    new_container = None
+
+try:
+    import docker
+except ModuleNotFoundError:
+    docker = None
+
+
 TMP_DIR = "tmp"
 
 
 class DatabaseConfigHelper:
     @staticmethod
     def get_database_config(database):
         return databaseConfig[database]
@@ -113,15 +127,15 @@
         "alias": "MSSQLTest",
     },
     "Snowflake": {
         "drivername": "snowflake",
         "username": os.getenv("SF_USERNAME"),
         "password": os.getenv("SF_PASSWORD"),
         # database/schema
-        "database": os.getenv("SF_DATABASE"),
+        "database": os.getenv("SF_DATABASE", "JUPYSQL_INTEGRATION_TESTING/GENERAL"),
         "host": "lpb17716.us-east-1",
         "port": None,
         "alias": "snowflakeTest",
         "docker_ct": None,
         "query": {
             "warehouse": "COMPUTE_WH",
             "role": "SYSADMIN",
@@ -158,17 +172,14 @@
         host=databaseConfig[database]["host"],
         port=databaseConfig[database]["port"],
         database=databaseConfig[database]["database"],
         query=databaseConfig[database]["query"],
     ).render_as_string(hide_password=False)
 
 
-client = docker.from_env()
-
-
 def database_ready(
     database,
     timeout=60,
     poll_freq=0.5,
 ):
     """Wait until the container is ready to receive connections.
 
@@ -204,24 +215,25 @@
 def get_docker_client():
     return docker.from_env(
         version="auto", environment={"DOCKER_HOST": os.getenv("DOCKER_HOST")}
     )
 
 
 @contextmanager
+@requires(["docker", "dockerctx"])
 def postgres(is_bypass_init=False):
     if is_bypass_init:
         yield None
         return
     db_config = DatabaseConfigHelper.get_database_config("postgreSQL")
     try:
         client = get_docker_client()
         container = client.containers.get(db_config["docker_ct"]["name"])
         yield container
-    except errors.NotFound:
+    except docker.errors.NotFound:
         print("Creating new container: postgreSQL")
         with new_container(
             new_container_name=db_config["docker_ct"]["name"],
             image_name=db_config["docker_ct"]["image"],
             ports=db_config["docker_ct"]["ports"],
             environment={
                 "POSTGRES_DB": db_config["database"],
@@ -236,24 +248,25 @@
                 "retries": 5,
             },
         ) as container:
             yield container
 
 
 @contextmanager
+@requires(["docker", "dockerctx"])
 def mysql(is_bypass_init=False):
     if is_bypass_init:
         yield None
         return
     db_config = DatabaseConfigHelper.get_database_config("mySQL")
     try:
         client = get_docker_client()
         container = client.containers.get(db_config["docker_ct"]["name"])
         yield container
-    except errors.NotFound:
+    except docker.errors.NotFound:
         print("Creating new container: mysql")
         with new_container(
             new_container_name=db_config["docker_ct"]["name"],
             image_name=db_config["docker_ct"]["image"],
             ports=db_config["docker_ct"]["ports"],
             environment={
                 "MYSQL_DATABASE": db_config["database"],
@@ -276,24 +289,25 @@
                 "timeout": 5000000000,
             },
         ) as container:
             yield container
 
 
 @contextmanager
+@requires(["docker", "dockerctx"])
 def mariadb(is_bypass_init=False):
     if is_bypass_init:
         yield None
         return
     db_config = DatabaseConfigHelper.get_database_config("mariaDB")
     try:
         client = get_docker_client()
         curr = client.containers.get(db_config["docker_ct"]["name"])
         yield curr
-    except errors.NotFound:
+    except docker.errors.NotFound:
         print("Creating new container: mariaDB")
         with new_container(
             new_container_name=db_config["docker_ct"]["name"],
             image_name=db_config["docker_ct"]["image"],
             ports=db_config["docker_ct"]["ports"],
             environment={
                 "MYSQL_DATABASE": db_config["database"],
@@ -316,24 +330,25 @@
                 "timeout": 5000000000,
             },
         ) as container:
             yield container
 
 
 @contextmanager
+@requires(["docker", "dockerctx"])
 def mssql(is_bypass_init=False):
     if is_bypass_init:
         yield None
         return
     db_config = DatabaseConfigHelper.get_database_config("MSSQL")
     try:
         client = get_docker_client()
         curr = client.containers.get(db_config["docker_ct"]["name"])
         yield curr
-    except errors.NotFound:
+    except docker.errors.NotFound:
         print("Creating new container: MSSQL")
         with new_container(
             new_container_name=db_config["docker_ct"]["name"],
             image_name=db_config["docker_ct"]["image"],
             ports=db_config["docker_ct"]["ports"],
             environment={
                 "MSSQL_DATABASE": db_config["database"],
@@ -349,24 +364,25 @@
                 "timeout": 5000000000,
             },
         ) as container:
             yield container
 
 
 @contextmanager
+@requires(["docker", "dockerctx"])
 def oracle(is_bypass_init=False):
     if is_bypass_init:
         yield None
         return
     db_config = DatabaseConfigHelper.get_database_config("oracle")
     try:
         client = get_docker_client()
         curr = client.containers.get(db_config["docker_ct"]["name"])
         yield curr
-    except errors.NotFound:
+    except docker.errors.NotFound:
         print("Creating new container: oracle")
         with new_container(
             new_container_name=db_config["docker_ct"]["name"],
             image_name=db_config["docker_ct"]["image"],
             ports=db_config["docker_ct"]["ports"],
             environment={
                 "APP_USER": db_config["username"],
```

### Comparing `jupysql-0.7.9/src/sql/column_guesser.py` & `jupysql-0.8.0/src/sql/column_guesser.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/src/sql/command.py` & `jupysql-0.8.0/src/sql/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,26 +24,24 @@
         self._cell = cell
 
         self.args = parse.magic_args(magic.execute, line)
         # self.args.line (everything that appears after %sql/%%sql in the first line)
         # is split in tokens (delimited by spaces), this checks if we have one arg
         one_arg = len(self.args.line) == 1
 
-        is_custom_connection_ = (
-            Connection.is_custom_connection(user_ns.get(self.args.line[0], False))
+        is_dbapi_connection_ = (
+            Connection.is_dbapi_connection(user_ns.get(self.args.line[0], False))
             if len(self.args.line) > 0
             else False
         )
 
         if (
             one_arg
             and self.args.line[0] in user_ns
-            and (
-                isinstance(user_ns[self.args.line[0]], Engine) or is_custom_connection_
-            )
+            and (isinstance(user_ns[self.args.line[0]], Engine) or is_dbapi_connection_)
         ):
             line_for_command = []
             add_conn = True
         else:
             line_for_command = self.args.line
             add_conn = False
 
@@ -67,14 +65,18 @@
 
         if add_conn:
             self.parsed["connection"] = user_ns[self.args.line[0]]
 
         if add_alias:
             self.parsed["connection"] = self.args.line[0]
 
+        if self.args.with_:
+            final = store.render(self.parsed["sql"], with_=self.args.with_)
+            self.parsed["sql"] = str(final)
+
     @property
     def sql(self):
         """
         Returns the SQL query to execute, without any other options or arguments
         """
         return self.parsed["sql"]
```

### Comparing `jupysql-0.7.9/src/sql/connection.py` & `jupysql-0.8.0/src/sql/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,21 +355,21 @@
         """
         Set the current database connection. This method is called from the magic to
         determine which connection to use (either use an existing one or open a new one)
         """
         connect_args = connect_args or {}
 
         if descriptor:
-            is_custom_connection_ = Connection.is_custom_connection(descriptor)
+            is_dbapi_connection_ = Connection.is_dbapi_connection(descriptor)
             if isinstance(descriptor, Connection):
                 cls.current = descriptor
             elif isinstance(descriptor, Engine):
                 cls.current = Connection(descriptor, alias=alias)
-            elif is_custom_connection_:
-                cls.current = CustomConnection(descriptor, alias=alias)
+            elif is_dbapi_connection_:
+                cls.current = DBAPIConnection(descriptor, alias=alias)
             else:
                 existing = rough_dict_get(cls.connections, descriptor)
                 # NOTE: I added one indentation level, otherwise
                 # the "existing" variable would not exist if
                 # passing an engine object as descriptor.
                 # Since I never saw this breaking, my guess
                 # is that we're missing some unit tests
@@ -485,41 +485,41 @@
     def close_all(cls, verbose=False):
         """Close all active connections"""
         connections = Connection.connections.copy()
         for key, conn in connections.items():
             conn.close(key)
 
             if verbose:
-                print(f"Closing {key}")
+                display.message(f"Closing {key}")
 
         cls.connections = {}
 
-    def is_custom_connection(conn=None) -> bool:
+    def is_dbapi_connection(conn=None) -> bool:
         """
         Checks if given connection is custom
         """
-        is_custom_connection_ = False
+        is_dbapi_connection_ = False
 
         if conn is None:
             if not Connection.current:
                 raise exceptions.RuntimeError("No active connection")
             else:
                 conn = Connection.current.session
 
-        if isinstance(conn, (CustomConnection, CustomSession)):
-            is_custom_connection_ = True
+        if isinstance(conn, (DBAPIConnection, DBAPISession)):
+            is_dbapi_connection_ = True
         else:
             if isinstance(
                 conn, (sqlalchemy.engine.base.Connection, Connection)
             ) or not (is_pep249_compliant(conn)):
-                is_custom_connection_ = False
+                is_dbapi_connection_ = False
             else:
-                is_custom_connection_ = True
+                is_dbapi_connection_ = True
 
-        return is_custom_connection_
+        return is_dbapi_connection_
 
     def _get_curr_sqlalchemy_connection_info(self):
         """Get the dialect, driver, and database server version info of current
         connected dialect
 
         Returns
         -------
@@ -538,14 +538,15 @@
 
         return {
             "dialect": getattr(engine.dialect, "name", None),
             "driver": getattr(engine.dialect, "driver", None),
             "server_version_info": getattr(engine.dialect, "server_version_info", None),
         }
 
+    # TODO: we have self.dialect and we also have this, which is confusing, see #732
     def _get_curr_sqlglot_dialect(self):
         """Get the dialect name in sqlglot package scope
 
         Returns
         -------
         str
             Available dialect in sqlglot package, see more:
@@ -592,15 +593,15 @@
                     cur_dialect
                 ).Tokenizer.IDENTIFIERS
 
                 identifiers = [*set(identifiers + identifiers_)]
         except ValueError:
             pass
         except AttributeError:
-            # this might be a custom connection..
+            # this might be a DBAPI connection
             pass
 
         return identifiers
 
     def _transpile_query(self, query):
         """Translate the given SQL clause that's compatible to current connected
         dialect by sqlglot
@@ -635,15 +636,15 @@
             The key to use in with sql clause
         """
         if with_:
             query = str(store.render(query, with_=with_))
 
         query = self._transpile_query(query)
 
-        if self.is_custom_connection():
+        if self.is_dbapi_connection():
             query = str(query)
         else:
             query = sqlalchemy.sql.text(query)
 
         return query
 
     def execute(self, query, with_=None):
@@ -653,54 +654,66 @@
         query = self._prepare_query(query, with_)
         return self.session.execute(query)
 
 
 atexit.register(Connection.close_all, verbose=True)
 
 
-class CustomSession(sqlalchemy.engine.base.Connection):
+class DBAPISession(sqlalchemy.engine.base.Connection):
     """
-    Custom sql alchemy session
+    A session object for generic DBAPI connections
     """
 
     def __init__(self, connection, engine):
         self.engine = engine
         self.dialect = dict(
             {
                 "name": connection.dialect,
                 "driver": connection.dialect,
                 "server_version_info": connection.dialect,
             }
         )
 
+    # TODO: this will fail when using a duck native connection and a tmp
+    # table since the table will only be visible to the cursor
     def execute(self, query):
         cur = self.engine.cursor()
         cur.execute(query)
         return cur
 
 
-class CustomConnection(Connection):
+class DBAPIConnection(Connection):
     """
-    Custom connection for unsupported drivers in sqlalchemy
+    A connection object for generic DBAPI connections
     """
 
-    @telemetry.log_call("CustomConnection", payload=True)
+    @telemetry.log_call("DBAPIConnection", payload=True)
     def __init__(self, payload, engine=None, alias=None):
         try:
             payload["engine"] = type(engine)
         except Exception as e:
             payload["engine_parsing_error"] = str(e)
 
         if engine is None:
             raise ValueError("Engine cannot be None")
 
-        connection_name_ = "custom_driver"
+        # detect if the engine is a native duckdb connection
+        _is_duckdb_native = _check_if_duckdb_dbapi_connection(engine)
+        connection_name_ = "duckdb" if _is_duckdb_native else "custom_driver"
+
         self.url = str(engine)
         self.name = connection_name_
         self.dialect = connection_name_
-        self.session = CustomSession(self, engine)
+        self.session = DBAPISession(self, engine)
 
         self.connections[alias or connection_name_] = self
 
         self.connect_args = None
         self.alias = alias
         Connection.current = self
+
+
+def _check_if_duckdb_dbapi_connection(conn):
+    """Check if the connection is a native duckdb connection"""
+    # NOTE: duckdb defines df and pl to efficiently convert results to
+    # pandas.DataFrame and polars.DataFrame respectively
+    return hasattr(conn, "df") and hasattr(conn, "pl")
```

### Comparing `jupysql-0.7.9/src/sql/display.py` & `jupysql-0.8.0/src/sql/display.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/src/sql/exceptions.py` & `jupysql-0.8.0/src/sql/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/src/sql/ggplot/facet_wrap.py` & `jupysql-0.8.0/src/sql/ggplot/facet_wrap.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/src/sql/ggplot/geom/geom_histogram.py` & `jupysql-0.8.0/src/sql/ggplot/geom/geom_histogram.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/src/sql/ggplot/ggplot.py` & `jupysql-0.8.0/src/sql/ggplot/ggplot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/src/sql/magic.py` & `jupysql-0.8.0/src/sql/magic.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from sql import display, exceptions
 from sql.store import store
 from sql.command import SQLCommand
 from sql.magic_plot import SqlPlotMagic
 from sql.magic_cmd import SqlCmdMagic
 from sql._patch import patch_ipython_usage_error
 from sql import query_util
-from sql.util import get_suggestions_message, show_deprecation_warning
+from sql.util import get_suggestions_message, pretty_print
 from ploomber_core.dependencies import check_installed
 
 from sql.error_message import detail
 from traitlets.config.configurable import Configurable
 from traitlets import Bool, Int, TraitError, Unicode, Dict, observe, validate
 
 
@@ -68,14 +68,21 @@
         help="Use a saved query",
         action="append",
         dest="with_",
     )
     @telemetry.log_call("sqlrender")
     def sqlrender(self, line):
         args = parse_argstring(self.sqlrender, line)
+        warnings.warn(
+            "\n'%sqlrender' will be deprecated soon, "
+            f"please use '%sqlcmd snippets {args.line[0]}' instead. "
+            "\n\nFor documentation, follow this link : "
+            "https://jupysql.ploomber.io/en/latest/api/magic-snippets.html#id1",
+            FutureWarning,
+        )
         return str(store[args.line[0]])
 
 
 @magics_class
 class SqlMagic(Magics, Configurable):
     """Runs SQL statement on a database, specified by SQLAlchemy connect string.
 
@@ -99,15 +106,15 @@
     )
     short_errors = Bool(
         True,
         config=True,
         help="Don't display the full traceback on SQL Programming Error",
     )
     displaylimit = Int(
-        sql.run.DEFAULT_DISPLAYLIMIT_VALUE,
+        10,
         config=True,
         allow_none=True,
         help=(
             "Automatically limit the number of rows "
             "displayed (full result set is still stored)"
         ),
     )
@@ -157,15 +164,15 @@
     # If:
     #   None -> We treat it as 0 (no limit)
     #   Positive Integer -> Pass
     #   Negative Integer -> raise Error
     @validate("displaylimit")
     def _valid_displaylimit(self, proposal):
         if proposal["value"] is None:
-            print("displaylimit: Value None will be treated as 0 (no limit)")
+            display.message("displaylimit: Value None will be treated as 0 (no limit)")
             return 0
         try:
             value = int(proposal["value"])
             if value < 0:
                 raise TraitError(
                     "{}: displaylimit cannot be a negative integer".format(value)
                 )
@@ -177,15 +184,17 @@
     def _mutex_autopandas_autopolars(self, change):
         # When enabling autopandas or autopolars, automatically disable the
         # other one in case it was enabled and print a warning
         if change["new"]:
             other = "autopolars" if change["name"] == "autopandas" else "autopandas"
             if getattr(self, other):
                 setattr(self, other, False)
-                print(f"Disabled '{other}' since '{change['name']}' was enabled.")
+                display.message(
+                    f"Disabled '{other}' since '{change['name']}' was enabled."
+                )
 
     def check_random_arguments(self, line="", cell=""):
         # check only for cell magic
         if cell != "":
             tokens = shlex.split(line, posix=False)
             arguments = []
 
@@ -203,14 +212,43 @@
             declared_argument = _option_strings_from_parser(SqlMagic.execute.parser)
             for check_argument in arguments:
                 if check_argument not in declared_argument:
                     raise exceptions.UsageError(
                         "Unrecognized argument(s): {}".format(check_argument)
                     )
 
+    def _error_handling(self, e, query):
+        detailed_msg = detail(e)
+        if self.short_errors:
+            if detailed_msg is not None:
+                err = exceptions.UsageError(detailed_msg)
+                raise err
+                # TODO: move to error_messages.py
+                # Added here due to circular dependency issue (#545)
+            elif "no such table" in str(e):
+                tables = query_util.extract_tables_from_query(query)
+                for table in tables:
+                    suggestions = get_close_matches(table, list(self._store))
+                    err_message = f"There is no table with name {table!r}."
+                    # with_message = "Alternatively, please specify table
+                    # name using --with argument"
+                    if len(suggestions) > 0:
+                        suggestions_message = get_suggestions_message(suggestions)
+                        raise exceptions.TableNotFoundError(
+                            f"{err_message}{suggestions_message}"
+                        )
+                display.message(str(e))
+            else:
+                display.message(str(e))
+        else:
+            if detailed_msg is not None:
+                display.message(detailed_msg)
+            e.modify_exception = True
+            raise e
+
     @no_var_expand
     @needs_local_scope
     @line_magic("sql")
     @cell_magic("sql")
     @line_magic("jupysql")
     @cell_magic("jupysql")
     @magic_arguments()
@@ -353,28 +391,33 @@
         user_ns.update(local_ns)
 
         command = SQLCommand(self, user_ns, line, cell)
         # args.line: contains the line after the magic with all options removed
 
         args = command.args
 
-        with_ = self._store.infer_dependencies(command.sql_original, args.save)
-        if with_:
-            command.set_sql_with(with_)
-            print(f"Generating CTE with stored snippets : {', '.join(with_)}")
+        if args.with_:
+            with_ = args.with_
         else:
-            with_ = None
+            with_ = self._store.infer_dependencies(command.sql_original, args.save)
+            if with_:
+                command.set_sql_with(with_)
+                display.message(
+                    f"Generating CTE with stored snippets : {pretty_print(with_)}"
+                )
+            else:
+                with_ = None
 
         # Create the interactive slider
         if args.interact and not is_interactive_mode:
             check_installed(["ipywidgets"], "--interactive argument")
             interactive_dict = {}
             for key in args.interact:
                 interactive_dict[key] = local_ns[key]
-            print(
+            display.message(
                 "Interactive mode, please interact with below "
                 "widget(s) to control the variable"
             )
             interact(interactive_execute_wrapper, **interactive_dict)
             return
         if args.connections:
             return sql.connection.Connection.connections_table()
@@ -394,15 +437,15 @@
                     targets = ['"', "'"]
                     head = raw_args[0]
                     tail = raw_args[-1]
                     if head in targets and head == tail:
                         raw_args = raw_args[1:-1]
                 args.connection_arguments = json.loads(raw_args)
             except Exception as e:
-                print(e)
+                display.message(str(e))
                 raise e
         else:
             args.connection_arguments = {}
         if args.creator:
             args.creator = user_ns[args.creator]
 
         # this creates a new connection or use an existing one
@@ -447,16 +490,15 @@
         if args.append:
             return self._persist_dataframe(
                 command.sql, conn, user_ns, append=True, index=not args.no_index
             )
 
         if not command.sql:
             return
-        if args.with_:
-            show_deprecation_warning()
+
         # store the query if needed
         if args.save:
             if "-" in args.save:
                 warnings.warn(
                     "Using hyphens will be deprecated soon, "
                     "please use "
                     + str(args.save.replace("-", "_"))
@@ -483,15 +525,15 @@
                 if self.autopandas or self.autopolars:
                     keys = result.keys()
                 else:
                     keys = result.keys
                     result = result.dict()
 
                 if self.feedback:
-                    print(
+                    display.message(
                         "Returning data to local variables [{}]".format(", ".join(keys))
                     )
 
                 self.shell.user_ns.update(result)
 
                 return None
             else:
@@ -503,38 +545,20 @@
 
                 # Return results into the default ipython _ variable
                 return result
 
         # JA: added DatabaseError for MySQL
         except (ProgrammingError, OperationalError, DatabaseError) as e:
             # Sqlite apparently return all errors as OperationalError :/
-            detailed_msg = detail(e, command.sql)
-            if self.short_errors:
-                if detailed_msg is not None:
-                    err = exceptions.UsageError(detailed_msg)
-                    raise err
-                    # TODO: move to error_messages.py
-                    # Added here due to circular dependency issue (#545)
-                elif "no such table" in str(e):
-                    tables = query_util.extract_tables_from_query(command.sql)
-                    for table in tables:
-                        suggestions = get_close_matches(table, list(self._store))
-                        if len(suggestions) > 0:
-                            err_message = f"There is no table with name {table!r}."
-                            suggestions_message = get_suggestions_message(suggestions)
-                            raise exceptions.TableNotFoundError(
-                                f"{err_message}{suggestions_message}"
-                            )
-                    print(e)
-                else:
-                    print(e)
+            self._error_handling(e, command.sql)
+        except Exception as e:
+            # handle DuckDB exceptions
+            if "Catalog Error" in str(e):
+                self._error_handling(e, command.sql)
             else:
-                if detailed_msg is not None:
-                    print(detailed_msg)
-                e.modify_exception = True
                 raise e
 
     legal_sql_identifier = re.compile(r"^[A-Za-z0-9#_$]+")
 
     @modify_exceptions
     def _persist_dataframe(
         self, raw, conn, user_ns, append=False, index=True, replace=False
@@ -581,17 +605,15 @@
             if_exists = "replace"
         elif append:
             if_exists = "append"
         else:
             if_exists = "fail"
 
         try:
-            frame.to_sql(
-                table_name, conn.session.engine, if_exists=if_exists, index=index
-            )
+            frame.to_sql(table_name, conn.session, if_exists=if_exists, index=index)
         except ValueError:
             raise exceptions.ValueError(
                 f"""Table {table_name!r} already exists. Consider using \
 --persist-replace to drop the table before persisting the data frame"""
             )
 
         display.message_success(f"Success! Persisted {table_name} to the database.")
```

### Comparing `jupysql-0.7.9/src/sql/magic_plot.py` & `jupysql-0.8.0/src/sql/magic_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,62 +76,61 @@
             plot_str = util.pretty_print(SUPPORTED_PLOTS, last_delimiter="or")
             raise exceptions.UsageError(
                 "Missing the first argument, must be any of: "
                 f"{plot_str}\n"
                 "Example: %sqlplot histogram"
             )
 
+        if cmd.args.line[0] not in SUPPORTED_PLOTS + ["hist", "box"]:
+            plot_str = util.pretty_print(SUPPORTED_PLOTS, last_delimiter="or")
+            raise exceptions.UsageError(
+                f"Unknown plot {cmd.args.line[0]!r}. Must be any of: " f"{plot_str}"
+            )
+
         column = util.sanitize_identifier(column)
         table = util.sanitize_identifier(cmd.args.table)
 
         if cmd.args.with_:
-            util.show_deprecation_warning()
-        if cmd.args.line[0] in {"box", "boxplot"}:
+            with_ = cmd.args.with_
+        else:
             with_ = self._check_table_exists(table)
 
+        if cmd.args.line[0] in {"box", "boxplot"}:
             return plot.boxplot(
                 table=table,
                 column=column,
                 with_=with_,
                 orient=cmd.args.orient,
                 conn=None,
             )
         elif cmd.args.line[0] in {"hist", "histogram"}:
-            with_ = self._check_table_exists(table)
             return plot.histogram(
                 table=table,
                 column=column,
                 bins=cmd.args.bins,
                 with_=with_,
                 conn=None,
             )
         elif cmd.args.line[0] in {"bar"}:
-            with_ = self._check_table_exists(table)
             return plot.bar(
                 table=table,
                 column=column,
                 with_=with_,
                 orient=cmd.args.orient,
                 show_num=cmd.args.show_numbers,
                 conn=None,
             )
         elif cmd.args.line[0] in {"pie"}:
-            with_ = self._check_table_exists(table)
             return plot.pie(
                 table=table,
                 column=column,
                 with_=with_,
                 show_num=cmd.args.show_numbers,
                 conn=None,
             )
-        else:
-            plot_str = util.pretty_print(SUPPORTED_PLOTS, last_delimiter="or")
-            raise exceptions.UsageError(
-                f"Unknown plot {cmd.args.line[0]!r}. Must be any of: " f"{plot_str}"
-            )
 
     @staticmethod
     def _check_table_exists(table):
         with_ = None
         if util.is_saved_snippet(table):
             with_ = [table]
         else:
```

### Comparing `jupysql-0.7.9/src/sql/parse.py` & `jupysql-0.8.0/src/sql/parse.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     Please don't add any more syntax requiring
     special parsing.
     Instead, add @arguments to SqlMagic.execute.
 
     We're grandfathering the
     connection string and `<<` operator in.
     """
-
     result = {
         "connection": "",
         "sql": "",
         "result_var": None,
         "return_result_var": False,
     }
 
@@ -50,27 +49,28 @@
         return result
     result["connection"] = _connection_string(pieces[0], config)
     if result["connection"]:
         if len(pieces) == 1:
             return result
         cell = pieces[1]
 
-    pieces = cell.split(None, 2)
-    if len(pieces) > 1 and pieces[1] == "<<":
-        if pieces[0].endswith("="):
-            result["result_var"] = pieces[0][:-1]
+    pointer = cell.find("<<")
+    if pointer != -1:
+        left = cell[:pointer].replace(" ", "").replace("\n", "")
+        right = cell[pointer + 2 :].strip(" ")
+
+        if "=" in left:
+            result["result_var"] = left[:-1]
             result["return_result_var"] = True
         else:
-            result["result_var"] = pieces[0]
-
-        if len(pieces) == 2:
-            return result
-        cell = pieces[2]
+            result["result_var"] = left
 
-    result["sql"] = cell
+        result["sql"] = right
+    else:
+        result["sql"] = cell
     return result
 
 
 def _option_strings_from_parser(parser):
     """Extracts the expected option strings (-a, --append, etc) from argparse parser
 
     Thanks Martijn Pieters
```

### Comparing `jupysql-0.7.9/src/sql/plot.py` & `jupysql-0.8.0/src/sql/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from ploomber_core.dependencies import requires
 from ploomber_core.exceptions import modify_exceptions
 from jinja2 import Template
 
 from sql.util import flatten
 from sqlalchemy.exc import ProgrammingError
-from sql import exceptions
+from sql import exceptions, display
 
 try:
     import matplotlib.pyplot as plt
     from matplotlib.colors import Normalize
 except ModuleNotFoundError:
     plt = None
     Normalize = None
@@ -662,15 +662,15 @@
                 " on which group by and count is applied or"
                 " two columns: labels and size"
             )
 
         x_ = column[0]
         height_ = column[1]
 
-        print(f"Removing NULLs, if there exists any from {x_} and {height_}")
+        display.message(f"Removing NULLs, if there exists any from {x_} and {height_}")
         template_ = """
             select "{{x_}}" as x,
             "{{height_}}" as height
             from "{{table}}"
             where "{{x_}}" is not null
             and "{{height_}}" is not null;
             """
@@ -681,15 +681,15 @@
         if use_backticks:
             template_ = template_.replace('"', "`")
 
         template = Template(template_)
         query = template.render(table=table, x_=x_, height_=height_)
 
     else:
-        print(f"Removing NULLs, if there exists any from {column}")
+        display.message(f"Removing NULLs, if there exists any from {column}")
         template_ = """
                 select "{{column}}" as x,
                 count("{{column}}") as height
                 from "{{table}}"
                 where "{{column}}" is not null
                 group by "{{column}}";
                 """
@@ -846,30 +846,32 @@
                 " on which group by and count is applied or"
                 " two columns: labels and size"
             )
 
         labels_ = column[0]
         size_ = column[1]
 
-        print(f"Removing NULLs, if there exists any from {labels_} and {size_}")
+        display.message(
+            f"Removing NULLs, if there exists any from {labels_} and {size_}"
+        )
         template_ = """
                 select "{{labels_}}" as labels,
                 "{{size_}}" as size
                 from "{{table}}"
                 where "{{labels_}}" is not null
                 and "{{size_}}" is not null;
                 """
         if use_backticks:
             template_ = template_.replace('"', "`")
 
         template = Template(template_)
         query = template.render(table=table, labels_=labels_, size_=size_)
 
     else:
-        print(f"Removing NULLs, if there exists any from {column}")
+        display.message(f"Removing NULLs, if there exists any from {column}")
         template_ = """
                 select "{{column}}" as x,
                 count("{{column}}") as height
                 from "{{table}}"
                 where "{{column}}" is not null
                 group by "{{column}}";
                 """
```

### Comparing `jupysql-0.7.9/src/sql/query_util.py` & `jupysql-0.8.0/src/sql/query_util.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/src/sql/run.py` & `jupysql-0.8.0/src/sql/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 from io import StringIO
 import html
 
 import prettytable
 import sqlalchemy
 import sqlparse
 from sql.connection import Connection
+from sqlalchemy.exc import ResourceClosedError
 from sql import exceptions, display
 from .column_guesser import ColumnGuesserMixin
+from sql.warnings import JupySQLDataFramePerformanceWarning
 
 try:
     from pgspecial.main import PGSpecial
 except ModuleNotFoundError:
     PGSpecial = None
 from sqlalchemy.orm import Session
 
 from sql.telemetry import telemetry
 import logging
 import warnings
 from collections.abc import Iterable
 
-DEFAULT_DISPLAYLIMIT_VALUE = 10
-
 
 def unduplicate_field_names(field_names):
     """Append a number to duplicate field names to make them unique."""
     res = []
     for k in field_names:
         if k in res:
             i = 1
@@ -100,92 +100,174 @@
 
 
 _cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
 
 
 class ResultSet(ColumnGuesserMixin):
     """
-    Results of a SQL query.
-
-    Can access rows listwise, or by string value of leftmost column.
+    Results of a SQL query. Fetches rows lazily (only the necessary rows to show the
+    preview based on the current configuration)
     """
 
-    def __init__(self, sqlaproxy, config):
+    # user to overcome a duckdb-engine limitation, see @sqlaproxy for details
+    LAST_BY_CONNECTION = {}
+
+    def __init__(self, sqlaproxy, config, statement=None, conn=None):
+        ResultSet.LAST_BY_CONNECTION[conn] = self
+
         self.config = config
-        self.keys = {}
+        self.truncated = False
+        self.statement = statement
+
+        self._sqlaproxy = sqlaproxy
+        self._conn = conn
+        self._dialect = conn._get_curr_sqlglot_dialect()
+        self._keys = None
+        self._field_names = None
         self._results = []
+
         # https://peps.python.org/pep-0249/#description
-        is_dbapi_results = hasattr(sqlaproxy, "description")
+        self.is_dbapi_results = hasattr(sqlaproxy, "description")
 
-        self.pretty = None
+        # note that calling this will fetch the keys
+        self.pretty_table = self._init_table()
 
-        if is_dbapi_results:
-            should_try_fetch_results = True
+        self._mark_fetching_as_done = False
+
+        if self.config.autolimit == 1:
+            # if autolimit is 1, we only want to fetch one row
+            self.fetchmany(size=1)
+            self._done_fetching()
         else:
-            should_try_fetch_results = sqlaproxy.returns_rows
+            # in all other cases, 2 allows us to know if there are more rows
+            # for example when creating a table, the results contains one row, in
+            # such case, fetching 2 rows will tell us that there are no more rows
+            # and can set the _mark_fetching_as_done flag to True
+            self.fetchmany(size=2)
+
+        self._finished_init = True
+
+    @property
+    def sqlaproxy(self):
+        # there is a problem when using duckdb + sqlalchemy: duckdb-engine doesn't
+        # create separate cursors, so whenever we have >1 ResultSet, the old ones
+        # become outdated and fetching their results will return the results from
+        # the last ResultSet. To fix this, we have to re-issue the query
+        is_last_result = ResultSet.LAST_BY_CONNECTION.get(self._conn) is self
+        is_duckdb_sqlalchemy = (
+            self._dialect == "duckdb" and not self._conn.is_dbapi_connection()
+        )
 
-        if should_try_fetch_results:
-            # sql alchemy results
-            if not is_dbapi_results:
-                self.keys = sqlaproxy.keys()
-            elif isinstance(sqlaproxy.description, Iterable):
-                self.keys = [i[0] for i in sqlaproxy.description]
-            else:
-                self.keys = []
-
-            if len(self.keys) > 0:
-                if isinstance(config.autolimit, int) and config.autolimit > 0:
-                    self._results = sqlaproxy.fetchmany(size=config.autolimit)
-                else:
-                    self._results = sqlaproxy.fetchall()
+        if (
+            # skip this if we're initializing the object (we're running __init__)
+            hasattr(self, "_finished_init")
+            # this only applies to duckdb + sqlalchemy with outdated results
+            and is_duckdb_sqlalchemy
+            and not is_last_result
+        ):
+            self._sqlaproxy = self._conn.session.execute(self.statement)
+            self._sqlaproxy.fetchmany(size=len(self._results))
+
+            ResultSet.LAST_BY_CONNECTION[self._conn] = self
+
+        return self._sqlaproxy
+
+    def _extend_results(self, elements):
+        """Store the DB fetched results into the internal list of results"""
+        to_add = self.config.displaylimit - len(self._results)
+        self._results.extend(elements)
+        self.pretty_table.add_rows(elements[:to_add])
+
+    def mark_fetching_as_done(self):
+        self._mark_fetching_as_done = True
+        # NOTE: don't close the connection here (self.sqlaproxy.close()),
+        # because we need to keep it open for the next query
+
+    def _done_fetching(self):
+        return self._mark_fetching_as_done
+
+    @property
+    def field_names(self):
+        if self._field_names is None:
+            self._field_names = unduplicate_field_names(self.keys)
 
-                self.field_names = unduplicate_field_names(self.keys)
+        return self._field_names
 
-                _style = None
+    @property
+    def keys(self):
+        """
+        Return the keys of the results (the column names)
+        """
+        if self._keys is not None:
+            return self._keys
 
-                self.pretty = PrettyTable(self.field_names)
+        if not self.is_dbapi_results:
+            try:
+                self._keys = self.sqlaproxy.keys()
+            # sqlite raises this error when running a script that doesn't return rows
+            # e.g, 'CREATE TABLE' but others don't (e.g., duckdb)
+            except ResourceClosedError:
+                self._keys = []
+                return self._keys
 
-                if isinstance(config.style, str):
-                    _style = prettytable.__dict__[config.style.upper()]
-                    self.pretty.set_style(_style)
+        elif isinstance(self.sqlaproxy.description, Iterable):
+            self._keys = [i[0] for i in self.sqlaproxy.description]
+        else:
+            self._keys = []
+
+        return self._keys
 
     def _repr_html_(self):
+        self.fetch_for_repr_if_needed()
+
         _cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
-        if self.pretty:
-            self.pretty.add_rows(self)
-            result = self.pretty.get_html_string()
-            # to create clickable links
-            result = html.unescape(result)
-            result = _cell_with_spaces_pattern.sub(_nonbreaking_spaces, result)
-            if len(self) > self.pretty.row_count:
-                HTML = (
-                    '%s\n<span style="font-style:italic;text-align:center;">'
-                    "%d rows, truncated to displaylimit of %d</span>"
-                    "<br>"
-                    '<span style="font-style:italic;text-align:center;">'
-                    "If you want to see more, please visit "
-                    '<a href="https://jupysql.ploomber.io/en/latest/api/configuration.html#displaylimit">displaylimit</a>'  # noqa: E501
-                    " configuration</span>"
-                )
-                result = HTML % (result, len(self), self.pretty.row_count)
-            return result
-        else:
-            return None
+
+        result = self.pretty_table.get_html_string()
+
+        HTML = (
+            "%s\n<span style='font-style:italic;font-size:11px'>"
+            "<code>ResultSet</code> : to convert to pandas, call <a href="
+            "'https://jupysql.ploomber.io/en/latest/integrations/pandas.html'>"
+            "<code>.DataFrame()</code></a> or to polars, call <a href="
+            "'https://jupysql.ploomber.io/en/latest/integrations/polars.html'>"
+            "<code>.PolarsDataFrame()</code></a></span><br>"
+        )
+        result = HTML % (result)
+
+        # to create clickable links
+        result = html.unescape(result)
+        result = _cell_with_spaces_pattern.sub(_nonbreaking_spaces, result)
+
+        if self.config.displaylimit != 0 and not self._done_fetching():
+            HTML = (
+                '%s\n<span style="font-style:italic;text-align:center;">'
+                "Truncated to displaylimit of %d</span>"
+                "<br>"
+                '<span style="font-style:italic;text-align:center;">'
+                "If you want to see more, please visit "
+                '<a href="https://jupysql.ploomber.io/en/latest/api/configuration.html#displaylimit">displaylimit</a>'  # noqa: E501
+                " configuration</span>"
+            )
+            result = HTML % (result, self.config.displaylimit)
+        return result
 
     def __len__(self):
+        self.fetchall()
+
         return len(self._results)
 
     def __iter__(self):
+        self.fetchall()
+
         for result in self._results:
             yield result
 
-    def __str__(self, *arg, **kwarg):
-        if self.pretty:
-            self.pretty.add_rows(self)
-        return str(self.pretty or "")
+    def __str__(self):
+        self.fetch_for_repr_if_needed()
+        return str(self.pretty_table)
 
     def __repr__(self) -> str:
         return str(self)
 
     def __eq__(self, another: object) -> bool:
         return self._results == another
 
@@ -200,45 +282,49 @@
             result = [row for row in self if row[0] == key]
             if not result:
                 raise KeyError(key)
             if len(result) > 1:
                 raise KeyError('%d results for "%s"' % (len(result), key))
             return result[0]
 
+    def __getattr__(self, attr):
+        err_msg = (
+            f"'{attr}' is not a valid operation, you can convert this "
+            "into a pandas data frame by calling '.DataFrame()' or a "
+            "polars data frame by calling '.PolarsDataFrame()'"
+        )
+        raise AttributeError(err_msg)
+
     def dict(self):
         """Returns a single dict built from the result set
 
         Keys are column names; values are a tuple"""
         return dict(zip(self.keys, zip(*self)))
 
     def dicts(self):
         "Iterator yielding a dict for each row"
         for row in self:
             yield dict(zip(self.keys, row))
 
     @telemetry.log_call("data-frame", payload=True)
     def DataFrame(self, payload):
-        "Returns a Pandas DataFrame instance built from the result set."
+        """Returns a Pandas DataFrame instance built from the result set."""
+        payload["connection_info"] = self._conn._get_curr_sqlalchemy_connection_info()
         import pandas as pd
 
-        frame = pd.DataFrame(self, columns=(self and self.keys) or [])
-        payload[
-            "connection_info"
-        ] = Connection.current._get_curr_sqlalchemy_connection_info()
-        return frame
+        kwargs = {"columns": (self and self.keys) or []}
+        return _convert_to_data_frame(self, "df", pd.DataFrame, kwargs)
 
     @telemetry.log_call("polars-data-frame")
     def PolarsDataFrame(self, **polars_dataframe_kwargs):
-        "Returns a Polars DataFrame instance built from the result set."
+        """Returns a Polars DataFrame instance built from the result set."""
         import polars as pl
 
-        frame = pl.DataFrame(
-            (tuple(row) for row in self), schema=self.keys, **polars_dataframe_kwargs
-        )
-        return frame
+        polars_dataframe_kwargs["schema"] = self.keys
+        return _convert_to_data_frame(self, "pl", pl.DataFrame, polars_dataframe_kwargs)
 
     @telemetry.log_call("pie")
     def pie(self, key_word_sep=" ", title=None, **kwargs):
         """Generates a pylab pie chart from the result set.
 
         ``matplotlib`` must be installed, and in an
         IPython Notebook, inlining must be on::
@@ -341,17 +427,14 @@
         ax.set_ylabel(self.ys[0].name)
         return ax
 
     @telemetry.log_call("generate-csv")
     def csv(self, filename=None, **format_params):
         """Generate results in comma-separated form.  Write to ``filename`` if given.
         Any other parameters will be passed on to csv.writer."""
-        if not self.pretty:
-            return None  # no results
-        self.pretty.add_rows(self)
         if filename:
             encoding = format_params.get("encoding", "utf-8")
             outfile = open(filename, "w", newline="", encoding=encoding)
         else:
             outfile = StringIO()
 
         writer = UnicodeWriter(outfile, **format_params)
@@ -360,14 +443,60 @@
             writer.writerow(row)
         if filename:
             outfile.close()
             return CsvResultDescriptor(filename)
         else:
             return outfile.getvalue()
 
+    def fetchmany(self, size):
+        """Fetch n results and add it to the results"""
+        if not self._done_fetching():
+            try:
+                returned = self.sqlaproxy.fetchmany(size=size)
+            # sqlite raises this error when running a script that doesn't return rows
+            # e.g, 'CREATE TABLE' but others don't (e.g., duckdb)
+            except ResourceClosedError:
+                self.mark_fetching_as_done()
+                return
+
+            self._extend_results(returned)
+
+            if len(returned) < size:
+                self.mark_fetching_as_done()
+
+            if (
+                self.config.autolimit is not None
+                and self.config.autolimit != 0
+                and len(self._results) >= self.config.autolimit
+            ):
+                self.mark_fetching_as_done()
+
+    def fetch_for_repr_if_needed(self):
+        if self.config.displaylimit == 0:
+            self.fetchall()
+
+        missing = self.config.displaylimit - len(self._results)
+
+        if missing > 0:
+            self.fetchmany(missing)
+
+    def fetchall(self):
+        if not self._done_fetching():
+            self._extend_results(self.sqlaproxy.fetchall())
+            self.mark_fetching_as_done()
+
+    def _init_table(self):
+        pretty = CustomPrettyTable(self.field_names)
+
+        if isinstance(self.config.style, str):
+            _style = prettytable.__dict__[self.config.style.upper()]
+            pretty.set_style(_style)
+
+        return pretty
+
 
 def display_affected_rowcount(rowcount):
     if rowcount > 0:
         display.message_success(f"{rowcount} rows affected.")
 
 
 class FakeResultProxy(object):
@@ -429,15 +558,15 @@
     )
 
     if _should_commit:
         try:
             with Session(conn.session) as session:
                 session.commit()
         except sqlalchemy.exc.OperationalError:
-            print("The database does not support the COMMIT command")
+            display.message("The database does not support the COMMIT command")
 
 
 def is_postgres_or_redshift(dialect):
     """Checks if dialect is postgres or redshift"""
     return "postgres" in str(dialect) or "redshift" in str(dialect)
 
 
@@ -504,18 +633,14 @@
 
     sql : str
         SQL query to execution
 
     config
         Configuration object
     """
-    info = conn._get_curr_sqlalchemy_connection_info()
-
-    duckdb_autopandas = info and info.get("dialect") == "duckdb" and config.autopandas
-
     if not sql.strip():
         # returning only when sql is empty string
         return "Connected: %s" % conn.name
 
     for statement in sqlparse.split(sql):
         first_word = sql.strip().split()[0].lower()
         manual_commit = False
@@ -527,65 +652,93 @@
         # postgres metacommand
         if first_word.startswith("\\") and is_postgres_or_redshift(conn.dialect):
             result = handle_postgres_special(conn, statement)
 
         # regular query
         else:
             manual_commit = set_autocommit(conn, config)
-            is_custom_connection = Connection.is_custom_connection(conn)
+            is_dbapi_connection = Connection.is_dbapi_connection(conn)
 
             # if regular sqlalchemy, pass a text object
-            if not is_custom_connection:
+            if not is_dbapi_connection:
                 statement = sqlalchemy.sql.text(statement)
 
-            if duckdb_autopandas:
-                conn = conn.engine.raw_connection()
-                cursor = conn.cursor()
-                cursor.execute(str(statement))
-
-            else:
-                result = conn.session.execute(statement)
-                _commit(conn=conn, config=config, manual_commit=manual_commit)
-
-                if result and config.feedback:
-                    if hasattr(result, "rowcount"):
-                        display_affected_rowcount(result.rowcount)
-
-    # bypass ResultSet and use duckdb's native method to return a pandas data frame
-    if duckdb_autopandas:
-        df = cursor.df()
-        conn.close()
-        return df
-    else:
-        resultset = ResultSet(result, config)
-        return select_df_type(resultset, config)
+            result = conn.session.execute(statement)
+            _commit(conn=conn, config=config, manual_commit=manual_commit)
+
+            if result and config.feedback:
+                if hasattr(result, "rowcount"):
+                    display_affected_rowcount(result.rowcount)
+
+    resultset = ResultSet(result, config, statement, conn)
+    return select_df_type(resultset, config)
 
 
 def raw_run(conn, sql):
     return conn.session.execute(sqlalchemy.sql.text(sql))
 
 
-class PrettyTable(prettytable.PrettyTable):
-    def __init__(self, *args, **kwargs):
-        self.row_count = 0
-        self.displaylimit = DEFAULT_DISPLAYLIMIT_VALUE
-        return super(PrettyTable, self).__init__(*args, **kwargs)
-
+class CustomPrettyTable(prettytable.PrettyTable):
     def add_rows(self, data):
-        if self.row_count and (data.config.displaylimit == self.displaylimit):
-            return  # correct number of rows already present
-        self.clear_rows()
-        self.displaylimit = data.config.displaylimit
-        if self.displaylimit == 0:
-            self.displaylimit = None
-        if self.displaylimit in (None, 0):
-            self.row_count = len(data)
-        else:
-            self.row_count = min(len(data), self.displaylimit)
-        for row in data[: self.displaylimit]:
+        for row in data:
             formatted_row = []
             for cell in row:
                 if isinstance(cell, str) and cell.startswith("http"):
                     formatted_row.append("<a href={}>{}</a>".format(cell, cell))
                 else:
                     formatted_row.append(cell)
             self.add_row(formatted_row)
+
+
+def _statement_is_select(statement):
+    statement_ = statement.lower().strip()
+    # duckdb also allows FROM without SELECT
+    return statement_.startswith("select") or statement_.startswith("from")
+
+
+def _convert_to_data_frame(
+    result_set, converter_name, constructor, constructor_kwargs=None
+):
+    constructor_kwargs = constructor_kwargs or {}
+    has_converter_method = hasattr(result_set.sqlaproxy, converter_name)
+
+    # native duckdb connection
+    if hasattr(result_set.sqlaproxy, converter_name):
+        # we need to re-execute the statement because if we fetched some rows
+        # already, .df() will return None. But only if it's a select statement
+        # otherwise we might end up re-execute INSERT INTO or CREATE TABLE
+        # statements
+        is_select = _statement_is_select(result_set.statement)
+
+        if is_select:
+            result_set.sqlaproxy.execute(result_set.statement)
+
+        return getattr(result_set.sqlaproxy, converter_name)()
+    else:
+        frame = constructor(
+            (tuple(row) for row in result_set),
+            **constructor_kwargs,
+        )
+
+        # NOTE: in JupySQL 0.7.9, we were opening a raw new connection so people
+        # using SQLALchemy still had the native performance to convert to data frames
+        # but this led to other problems because the native connection didn't
+        # have the same state as the SQLAlchemy connection, yielding confusing
+        # errors. So we decided to remove this and just warn the user that
+        # performance might be slow and they could use a native connection
+        if (
+            result_set._dialect == "duckdb"
+            and not has_converter_method
+            and len(frame) >= 1_000
+        ):
+            DOCS = "https://jupysql.ploomber.io/en/latest/integrations/duckdb.html"
+            WARNINGS = "https://jupysql.ploomber.io/en/latest/tutorials/duckdb-native-sqlalchemy.html#supress-warnings"  # noqa: E501
+
+            warnings.warn(
+                "It looks like you're using DuckDB with SQLAlchemy. "
+                "For faster conversions, use "
+                f" a DuckDB native connection. Docs: {DOCS}."
+                f" to suppress this warning, see: {WARNINGS}",
+                category=JupySQLDataFramePerformanceWarning,
+            )
+
+        return frame
```

### Comparing `jupysql-0.7.9/src/sql/sqlcmd.py` & `jupysql-0.8.0/src/sql/cmd/snippets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from sql.magic_cmd import CmdParser
 from sql import util
 from sql.exceptions import UsageError
+from sql.cmd.cmd_utils import CmdParser
+from sql.store import store
+from sql.display import Table, Message
 
 
 def _modify_display_msg(key, remaining_keys, dependent_keys=None):
     """
 
     Parameters
     ----------
@@ -26,23 +28,27 @@
     if remaining_keys:
         msg = f"{msg}Stored snippets : {', '.join(remaining_keys)}"
     else:
         msg = f"{msg}There are no stored snippets"
     return msg
 
 
-def sqlcmd_snippets(others):
+def snippets(others):
     """
-
-    Parameters
-    ----------
+    Implementation of `%sqlcmd snippets`
     This function handles all the arguments related to %sqlcmd snippets, namely
     listing stored snippets, and delete/ force delete/ force delete a snippet and
     all its dependent snippets.
 
+
+    Parameters
+    ----------
+    others : str,
+        A string containing the command line arguments.
+
     """
     parser = CmdParser()
     parser.add_argument(
         "-d", "--delete", type=str, help="Delete stored snippet", required=False
     )
     parser.add_argument(
         "-D",
@@ -54,18 +60,36 @@
     parser.add_argument(
         "-A",
         "--delete-force-all",
         type=str,
         help="Force delete all stored snippets",
         required=False,
     )
+    all_snippets = util.get_all_keys()
+    if len(others) == 1:
+        if others[0] in all_snippets:
+            return str(store[others[0]])
+
+        base_err_msg = f"'{others[0]}' is not a snippet. "
+        if len(all_snippets) == 0:
+            err_msg = "%sThere is no available snippet."
+        else:
+            err_msg = "%sAvailable snippets are " f"{util.pretty_print(all_snippets)}."
+        err_msg = err_msg % (base_err_msg)
+
+        raise UsageError(err_msg)
+
     args = parser.parse_args(others)
     SNIPPET_ARGS = [args.delete, args.delete_force, args.delete_force_all]
     if SNIPPET_ARGS.count(None) == len(SNIPPET_ARGS):
-        return ", ".join(util.get_all_keys())
+        if len(all_snippets) == 0:
+            return Message("No snippets stored")
+        else:
+            return Table(["Stored snippets"], [[snippet] for snippet in all_snippets])
+
     if args.delete:
         deps = util.get_key_dependents(args.delete)
         if deps:
             deps = ", ".join(deps)
             raise UsageError(
                 f"The following tables are dependent on {args.delete}: {deps}.\n"
                 f"Pass --delete-force to only delete {args.delete}.\n"
```

### Comparing `jupysql-0.7.9/src/sql/store.py` & `jupysql-0.8.0/src/sql/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,17 @@
 {{ "," if not loop.last }}{% endfor %}{{query}}"""
         )
         is_use_backtick = sql.connection.Connection.current.is_use_backtick_template()
         with_all = _get_dependencies(self._store, self._with_)
         template = (
             with_clause_template_backtick if is_use_backtick else with_clause_template
         )
+        # return query without 'with' when no dependency exists
+        if len(with_all) == 0:
+            return self._query.strip()
         return template.render(
             query=self._query,
             saved=self._store._data,
             with_=with_all,
             rts=_remove_trailing_semicolon,
         )
```

### Comparing `jupysql-0.7.9/src/sql/util.py` & `jupysql-0.8.0/src/sql/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import warnings
 import sql
 from sql import inspect
 import difflib
 from sql.connection import Connection
 from sql.store import store, _get_dependents_for_key
-from sql import exceptions
+from sql import exceptions, display
 import json
 
 SINGLE_QUOTE = "'"
 DOUBLE_QUOTE = '"'
 
 
 def sanitize_identifier(identifier):
@@ -98,15 +98,15 @@
     else:
         table_ = table
 
     _is_exist = _is_table_exists(table_, conn)
 
     if not _is_exist:
         if not ignore_error:
-            try_find_suggestions = not Connection.is_custom_connection(conn)
+            try_find_suggestions = not Connection.is_dbapi_connection(conn)
             expected = []
             existing_schemas = []
             existing_tables = []
 
             if try_find_suggestions:
                 existing_schemas = inspect.get_schema_names()
 
@@ -125,20 +125,23 @@
                     f"There is no table with name {table!r} in schema {schema!r}"
                 )
             else:
                 err_message = (
                     f"There is no table with name {table!r} in the default schema"
                 )
 
-            suggestions = difflib.get_close_matches(invalid_input, expected)
-            suggestions_store = difflib.get_close_matches(invalid_input, list(store))
-            suggestions.extend(suggestions_store)
-            suggestions_message = get_suggestions_message(suggestions)
-            if suggestions_message:
-                err_message = f"{err_message}{suggestions_message}"
+            if table not in list(store):
+                suggestions = difflib.get_close_matches(invalid_input, expected)
+                suggestions_store = difflib.get_close_matches(
+                    invalid_input, list(store)
+                )
+                suggestions.extend(suggestions_store)
+                suggestions_message = get_suggestions_message(suggestions)
+                if suggestions_message:
+                    err_message = f"{err_message}{suggestions_message}"
             raise exceptions.TableNotFoundError(err_message)
 
     return _is_exist
 
 
 def _get_list_of_existing_tables() -> list:
     """
@@ -175,15 +178,15 @@
     Trims characters from the start and end of the string
     """
     return string.translate(str.maketrans("", "", chars))
 
 
 def is_saved_snippet(table: str) -> bool:
     if table in list(store):
-        print(f"Plotting using saved snippet : {table}")
+        display.message(f"Plotting using saved snippet : {table}")
         return True
     return False
 
 
 def _is_table_exists(table: str, conn) -> bool:
     """
     Runs a SQL query to check if table exists
@@ -243,16 +246,19 @@
     return process_list
 
 
 def support_only_sql_alchemy_connection(command):
     """
     Throws a sql.exceptions.RuntimeError if connection is not SQLAlchemy
     """
-    if Connection.is_custom_connection():
-        raise exceptions.RuntimeError(f"{command} is not supported for a custom engine")
+    if Connection.is_dbapi_connection():
+        raise exceptions.RuntimeError(
+            f"{command} is only supported with SQLAlchemy "
+            "connections, not with DBAPI connections"
+        )
 
 
 def fetch_sql_with_pagination(
     table, offset, n_rows, sort_column=None, sort_order=None
 ) -> tuple:
     """
     Returns next n_rows and columns from table starting at the offset
```

### Comparing `jupysql-0.7.9/src/sql/widgets/table_widget/js/tableWidget.js` & `jupysql-0.8.0/src/sql/widgets/table_widget/js/tableWidget.js`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/src/sql/widgets/table_widget/table_widget.py` & `jupysql-0.8.0/src/sql/widgets/table_widget/table_widget.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.9/src/sql/widgets/utils.py` & `jupysql-0.8.0/src/sql/widgets/utils.py`

 * *Files identical despite different names*

