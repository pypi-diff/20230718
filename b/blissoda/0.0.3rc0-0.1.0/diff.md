# Comparing `tmp/blissoda-0.0.3rc0.tar.gz` & `tmp/blissoda-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blissoda-0.0.3rc0.tar", last modified: Tue Mar 28 06:55:02 2023, max compression
+gzip compressed data, was "dist/blissoda-0.1.0.tar", last modified: Tue Jul 18 15:52:01 2023, max compression
```

## Comparing `blissoda-0.0.3rc0.tar` & `blissoda-0.1.0.tar`

### file list

```diff
@@ -1,97 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2015 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1722 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/app/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/app/cli_log_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1875 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/app/workflow_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/bm02/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/bm02/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/bm02/xrpd_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/bm23/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/bm23/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/bm23/exafs_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/demo/
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/exafs_plotter.py
--rw-rw-rw-   0 root         (0) root         (0)     3383 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/id11.py
--rw-rw-rw-   0 root         (0) root         (0)     5001 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/streamline_scanner.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/stscan_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/demo/user_scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/demo/user_scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/user_scripts/bm02.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/user_scripts/bm23.py
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/user_scripts/id11.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/user_scripts/id22.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/user_scripts/id31.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/user_scripts/streamline.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/xrpd_plotter.py
--rw-rw-rw-   0 root         (0) root         (0)     1883 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/demo/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/exafs_plotting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/exafs_plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/exafs_plotting/exafs_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    12341 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/exafs_plotting/exafs_plotter.py
--rw-rw-rw-   0 root         (0) root         (0)    12683 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/exafs_plotting/exafs_plotter_old.py
--rw-rw-rw-   0 root         (0) root         (0)     9917 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/exafs_plotting/exafs_widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/id11/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/id11/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9879 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/id11/xrpd_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/id22/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/id22/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30283 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/id22/stscan_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/id31/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/id31/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/id31/streamline_scanner.py
--rw-rw-rw-   0 root         (0) root         (0)     6705 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/id31/xrpd_processor.py
--rw-rw-rw-   0 root         (0) root         (0)     6135 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/persistent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/resources/bm23/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/resources/bm23/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/resources/bm23/bm23.ows
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/resources/demo/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/resources/demo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/resources/id11/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/resources/id11/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3687 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/resources/id11/integrate_scan.ows
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/resources/streamline/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/resources/streamline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2965 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/resources/streamline/reprocess.py
--rw-rw-rw-   0 root         (0) root         (0)    10202 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/resources/streamline/streamline_with_calib.ows
--rw-rw-rw-   0 root         (0) root         (0)     7356 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/resources/streamline/streamline_without_calib.ows
--rw-rw-rw-   0 root         (0) root         (0)     3758 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/resources/streamline/time_record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/seslab/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/seslab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/seslab/streamline_scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/streamline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/streamline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20320 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/streamline/streamline_scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1146 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    11229 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/tests/test_id22.py
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/tests/test_persistent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/utils/directories.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/utils/info.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/utils/pyfai.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda/xrpd_plotter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 06:54:57.000000 blissoda-0.0.3rc0/src/blissoda/xrpd_plotter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9048 2023-03-28 06:52:53.000000 blissoda-0.0.3rc0/src/blissoda/xrpd_plotter/xrpd_plotter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2015 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2586 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      886 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-28 06:55:02.000000 blissoda-0.0.3rc0/src/blissoda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-18 15:49:49.000000 blissoda-0.1.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-07-18 15:52:01.000000 blissoda-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-07-18 15:49:49.000000 blissoda-0.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-18 15:49:49.000000 blissoda-0.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-07-18 15:52:01.000000 blissoda-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-18 15:49:49.000000 blissoda-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/app/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/app/cli_log_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/app/workflow_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/bm02/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/bm02/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/bm02/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/bm23/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/bm23/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/bm23/exafs_plotter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/demo/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/exafs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3373 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/example.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/id22.py
+-rw-rw-rw-   0 root         (0) root         (0)     4990 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/streamline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/demo/user_scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/demo/user_scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/user_scripts/all.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/user_scripts/exafs.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/user_scripts/id22.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/user_scripts/streamline.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/user_scripts/xrpd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/demo/xrpd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/exafs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/exafs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/exafs/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    12568 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/exafs/plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9917 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/exafs/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/flint/
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/flint/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/id09/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/id09/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/id09/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/id11/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/id11/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/id11/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/id22/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/id22/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32384 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/id22/stscan_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/id22/xrpd_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/id31/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/id31/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5940 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/id31/optimize_exposure.py
+-rw-rw-rw-   0 root         (0) root         (0)     4684 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/id31/streamline_scanner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3306 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/id31/xrpd_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7328 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/id31/xrpd_processor_old.py
+-rw-rw-rw-   0 root         (0) root         (0)     6933 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/persistent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/resources/demo/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/demo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/resources/exafs/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/exafs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/exafs/exafs.ows
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/resources/streamline/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/streamline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/streamline/reprocess.py
+-rw-rw-rw-   0 root         (0) root         (0)     7835 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/streamline/streamline_with_calib.json
+-rw-rw-rw-   0 root         (0) root         (0)     5685 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/streamline/streamline_without_calib.json
+-rw-rw-rw-   0 root         (0) root         (0)     3758 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/streamline/time_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/resources/xrpd/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/xrpd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/xrpd/integrate_scan_with_saving.json
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/resources/xrpd/integrate_scan_without_saving.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/seslab/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/seslab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/seslab/streamline_scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/streamline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/streamline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20948 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/streamline/scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/tests/mock_id31/
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/tests/mock_id31/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/tests/mock_id31/attenuator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3273 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/tests/mock_id31/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/tests/mock_id31/lima_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/tests/mock_id31/setup_globals.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/tests/mock_id31/simulate.py
+-rw-rw-rw-   0 root         (0) root         (0)    13518 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/tests/test_id22.py
+-rw-rw-rw-   0 root         (0) root         (0)     1844 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/tests/test_id31.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/tests/test_persistent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/utils/directories.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/utils/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/utils/pyfai.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda/xrpd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:51:55.000000 blissoda-0.1.0/src/blissoda/xrpd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5167 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/xrpd/data.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/xrpd/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     6619 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/xrpd/plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    15944 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/xrpd/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2734 2023-07-18 15:49:49.000000 blissoda-0.1.0/src/blissoda/xrpd/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-18 15:52:01.000000 blissoda-0.1.0/src/blissoda.egg-info/top_level.txt
```

### Comparing `blissoda-0.0.3rc0/LICENSE.md` & `blissoda-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blissoda-0.0.3rc0/PKG-INFO` & `blissoda-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissoda
-Version: 0.0.3rc0
+Version: 0.1.0
 Summary: Utilities for ewoks developers
 Home-page: https://gitlab.esrf.fr/bliss/blissoda/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/bliss/blissoda/
 Project-URL: Documentation, https://blissoda.readthedocs.io/
@@ -13,19 +13,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: submit
 Provides-Extra: server
 Provides-Extra: id22
-Provides-Extra: streamline
-Provides-Extra: bm23
+Provides-Extra: id09
 Provides-Extra: id31
 Provides-Extra: bm02
 Provides-Extra: id11
+Provides-Extra: streamline
+Provides-Extra: bm23
 Provides-Extra: democlient
 Provides-Extra: demoworker
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE.md
```

### Comparing `blissoda-0.0.3rc0/README.md` & `blissoda-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `blissoda-0.0.3rc0/src/blissoda/app/__main__.py` & `blissoda-0.1.0/src/blissoda/app/__main__.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.0.3rc0/src/blissoda/app/cli_log_utils.py` & `blissoda-0.1.0/src/blissoda/app/cli_log_utils.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.0.3rc0/src/blissoda/app/workflow_server.py` & `blissoda-0.1.0/src/blissoda/app/workflow_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from gevent import monkey
 
 monkey.patch_all()
 
 import logging  # noqa E402
 import json  # noqa E402
-from typing import Mapping  # noqa E402
+from typing import Mapping, Optional  # noqa E402
 
 from blissdata.data.node import get_session_node  # noqa E402
 from ewoksjob.client import submit  # noqa E402
 
 logger = logging.getLogger(__name__)
 
 
@@ -25,32 +25,30 @@
                 continue
             filename = info.get("filename")
             scan_nb = info.get("scan_nb")
             for wfname, nxprocess in workflows.items():
                 if not isinstance(nxprocess, Mapping):
                     continue
                 try:
-                    config = nxprocess["configuration"]
                     job_id = submit_scan_workflow(
-                        config["data"], options=config.get("options")
+                        **json.loads(nxprocess["configuration"]["data"])
                     )
                 except Exception:
                     logger.exception(
-                        f"Error when submitting workflow {wfname} for scan {scan_nb} of file {filename}"
+                        f"Error when submitting workflow '{wfname}' for scan {scan_nb} of file '{filename}'"
                     )
                 else:
-                    logger.info(
-                        f"Submitted workflow '{wfname}' (JOB ID {job_id}) for scan {scan_nb} of file {filename}"
-                    )
+                    if job_id is not None:
+                        logger.info(
+                            f"Submitted workflow '{wfname}' (JOB ID {job_id}) for scan {scan_nb} of file '{filename}'"
+                        )
 
 
-def submit_scan_workflow(workflow, options=None):
-    if options:
-        kwargs = json.loads(options)
-    else:
-        kwargs = None
+def submit_scan_workflow(workflow=None, **kwargs) -> Optional[str]:
+    if not workflow:
+        return
     future = submit(args=(workflow,), kwargs=kwargs)
     return future.task_id
 
 
-def main(args):
+def main(args) -> None:
     session_watcher(args.session)
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/bm23/exafs_plotter.py` & `blissoda-0.1.0/src/blissoda/bm23/exafs_plotter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..exafs_plotting.exafs_plotter import ExafsPlotter
+from ..exafs.plotter import ExafsPlotter
 
 
 class Bm23ExafsPlotter(ExafsPlotter):
     def __init__(self) -> None:
         super().__init__()
         self._set_parameter_default("workflow", "/users/opd23/ewoks/online.ows")
         self._set_parameter_default("_scan_type", "cont")
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/demo/exafs_plotter.py` & `blissoda-0.1.0/src/blissoda/demo/exafs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 
 try:
     from bliss import setup_globals
 except ImportError:
     setup_globals = None
-from ..exafs_plotting.exafs_plotter import ExafsPlotter
-from ..resources.bm23 import RESOURCE_ROOT
+from ..exafs.plotter import ExafsPlotter
+from ..resources.exafs import RESOURCE_ROOT
 
 
 class DemoExafsPlotter(ExafsPlotter):
     def __init__(self) -> None:
         super().__init__()
-        self._set_parameter_default("workflow", os.path.join(RESOURCE_ROOT, "bm23.ows"))
+        self._set_parameter_default(
+            "workflow", os.path.join(RESOURCE_ROOT, "exafs.ows")
+        )
         self._set_parameter_default("_scan_type", "any")
         self._counters.setdefault(
             "any",
             {
                 "mu_name": "mu",
                 "energy_name": "energy",
                 "energy_unit": "eV",
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/demo/example.py` & `blissoda-0.1.0/src/blissoda/demo/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,8 +99,8 @@
     else:
         assert len(result_event) == 1
         result_event = result_event[0]
 
         # Get access to all output variables of "task1"
         if varinfo.get("root_uri"):
             results = result_event["outputs"]
-            assert results.variable_values["return_value"] == 3
+            assert results["return_value"].value == 3
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/demo/streamline_scanner.py` & `blissoda-0.1.0/src/blissoda/demo/streamline.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from contextlib import contextmanager
 
 try:
     from bliss import setup_globals
 except ImportError:
     setup_globals = None
 
-from ..streamline.streamline_scanner import StreamlineScanner
+from ..streamline.scanner import StreamlineScanner
 
 
 def energy_wavelength(x):
     """keV to m and vice versa"""
     return 12.398419843320026 * 1e-10 / x
 
 
@@ -23,29 +23,29 @@
     "rot2": 0,  # 0 deg
     "rot3": 0,  # 0 deg
     "wavelength": energy_wavelength(12),  # 12 keV
     "detector": "Pilatus1M",
 }
 
 
-class StreamlineDemoScanner(StreamlineScanner):
+class DemoStreamlineScanner(StreamlineScanner):
     def __init__(self):
         super().__init__()
         self._set_parameter_default("detector_name", "difflab6")
         self._set_parameter_default("calibrant", "LaB6")
         self._set_parameter_default("sample_changer_name", "streamline_sc")
         self._set_parameter("image_slice", "0,0:-1,0:-1")
         self._set_parameter_default(
             "integration_options",
             {
                 "method": "no_csr_cython",
                 "integrator_name": "sigma_clip_ng",
                 "extra_options": {"max_iter": 3, "thres": 0},
                 "error_model": "azimuthal",  # hybrid gives weird results
-                "nbpt_rad": 1024,
+                "nbpt_rad": 4096,
                 "unit": "q_nm^-1",
             },
         )
 
     def measure_sample(self, *args, **kwargs):
         return setup_globals.sct(*args, setup_globals.difflab6, **kwargs)
 
@@ -167,10 +167,10 @@
 
 
 if setup_globals is None:
     streamline_scanner = None
     streamline_sc = None
     streamline_translation = None
 else:
-    streamline_scanner = StreamlineDemoScanner()
+    streamline_scanner = DemoStreamlineScanner()
     streamline_sc = MockSampleChanger()
     streamline_translation = MockSampleTranslation()
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/demo/stscan_processor.py` & `blissoda-0.1.0/src/blissoda/demo/id22.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     from bliss import setup_globals
 except ImportError:
     setup_globals = None
 from ..id22.stscan_processor import StScanProcessor
 
 
-class StScanDemoProcessor(StScanProcessor):
+class DemoStScanProcessor(StScanProcessor):
     def __init__(self) -> None:
         super().__init__(
             convert_workflow="/tmp/demo/convert.json",
             rebinsum_workflow="/tmp/demo/rebinsum.json",
             extract_workflow="/tmp/demo/extract.json",
         )
 
@@ -23,8 +23,8 @@
         print("Options:")
         pprint(kw)
 
 
 if setup_globals is None:
     stscan_processor = None
 else:
-    stscan_processor = StScanDemoProcessor()
+    stscan_processor = DemoStScanProcessor()
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/demo/user_scripts/streamline.py` & `blissoda-0.1.0/src/blissoda/demo/user_scripts/streamline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from blissoda.demo.streamline_scanner import streamline_sc
-from blissoda.demo.streamline_scanner import streamline_scanner
+from blissoda.demo.streamline import streamline_sc
+from blissoda.demo.streamline import streamline_scanner
 
 
 def streamline_demo(with_calibration=False):
     # Nothing loaded and 2 holders in the tray:
     streamline_scanner.eject()
     streamline_sc.fill_tray(2)
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/demo/xrpd_plotter.py` & `blissoda-0.1.0/src/blissoda/demo/xrpd.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import numpy
 import json
+from typing import Optional, List
 
 try:
     from bliss import setup_globals
 except ImportError:
     setup_globals = None
-from ..xrpd_plotter.xrpd_plotter import XrpdPlotter
+
+from ..xrpd.processor import XrpdProcessor
+from ..persistent import ParameterInfo
 
 
 def energy_wavelength(x):
     """keV to m and vice versa"""
     return 12.398419843320026 * 1e-10 / x
 
 
@@ -21,51 +24,61 @@
     "rot2": 0,  # 0 deg
     "rot3": 0,  # 0 deg
     "wavelength": energy_wavelength(12),  # 12 keV
     "detector": "Pilatus1M",
 }
 
 
-class DemoXrpdPlotter(XrpdPlotter):
+class DemoXrpdProcessor(
+    XrpdProcessor,
+    parameters=[
+        ParameterInfo("config_filename", category="PyFai"),
+        ParameterInfo("integration_options", category="PyFai"),
+    ],
+):
     def __init__(self) -> None:
         super().__init__()
+        self._set_parameter_default("lima_names", ["difflab6"])
         self._set_parameter_default(
             "integration_options",
             {
                 "method": "no_csr_cython",
-                "nbpt_rad": 1024,
+                "nbpt_rad": 4096,
                 "radial_range_min": 1,
                 "unit": "q_nm^-1",
             },
         )
-        self._ensure_pyfai_config()
+        self._ensure_config_filename()
 
-    def _get_inputs(self, pyfai_config, db_name):
-        self._ensure_pyfai_config()
-        lst = super()._get_inputs(pyfai_config, db_name)
-        lst += [{"id": "load_image", "name": "demo", "value": True}]
-        return lst
+    def get_integrate_inputs(
+        self, scan, lima_name: str, task_identifier: str
+    ) -> List[dict]:
+        self._ensure_config_filename()
+        inputs = super().get_integrate_inputs(scan, lima_name, task_identifier)
+        inputs.append(
+            {"task_identifier": task_identifier, "name": "demo", "value": True}
+        )
+        return inputs
 
-    def _ensure_pyfai_config(self):
+    def _ensure_config_filename(self):
+        if self.config_filename:
+            return
         cfgfile = "/tmp/test.json"
-        self.pyfai_configurations["difflab6"] = cfgfile
         poni = _DEFAULT_CALIB
         with open(cfgfile, "w") as f:
             json.dump(poni, f)
+        self.config_filename = cfgfile
 
-    def test(self, npoints=100, expo=0.1):
-        setup_globals.loopscan(
-            npoints,
-            expo,
-            setup_globals.difflab6,
-            setup_globals.diode1,
-            setup_globals.diode2,
-        )
+    def get_config_filename(self, lima_name: str) -> Optional[str]:
+        return self.config_filename
+
+    def get_integration_options(self, lima_name: str) -> Optional[dict]:
+        return self.integration_options.to_dict()
 
 
 if setup_globals is None:
-    xrpd_plotter = None
+    xrpd_processor = None
 else:
     try:
-        xrpd_plotter = DemoXrpdPlotter()
+        xrpd_processor = DemoXrpdProcessor()
     except ImportError:
-        xrpd_plotter = None
+        xrpd_processor = None
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/exafs_plotting/exafs_plots.py` & `blissoda-0.1.0/src/blissoda/exafs/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     from bliss.flint.client.plots import BasePlot
 except ImportError:
     BasePlot = object
 
 
 class ExafsPlot(BasePlot):
-    WIDGET = "blissoda.exafs_plotting.exafs_widgets.ExafsWidget"
+    WIDGET = "blissoda.exafs.widgets.ExafsWidget"
 
     def clear(self):
         self.submit("clear")
 
     def remove_scan(self, legend):
         self.submit("remove_scan", legend)
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/exafs_plotting/exafs_plotter.py` & `blissoda-0.1.0/src/blissoda/exafs/plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """Workflow execution and Flint EXAFS plotting during a scan"""
 
 import time
 import os
 import logging
 import gevent
 from collections import OrderedDict
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Dict
 
 from silx.io.h5py_utils import top_level_names
 
 try:
     from bliss.common.plot import get_flint
     from bliss.flint.client.proxy import FlintClient
 except ImportError:
     get_flint = None
     FlintClient = None
 
 from ewoksjob.client import submit
 from ewoksjob.client import get_future
 
-from ..utils.info import format_info
 from ..persistent import WithPersistentParameters
-from .exafs_plots import ExafsPlot
+from .plots import ExafsPlot
+from ..persistent import ParameterInfo
 
 
 logger = logging.getLogger(__name__)
 
 
 class ExafsPlotter(
     WithPersistentParameters,
     parameters=[
-        "refresh_period",
-        "max_scans",
-        "enabled",
-        "workflow",
-        "_counters",
-        "_scan_type",
-        "_color_index",
+        ParameterInfo("refresh_period"),
+        ParameterInfo("max_scans"),
+        ParameterInfo("enabled"),
+        ParameterInfo("workflow"),
+        ParameterInfo("_counters"),
+        ParameterInfo("_scan_type"),
+        ParameterInfo("_color_index"),
     ],
 ):
     """Run a scan, execute a workflow every x seconds during the scan
     and plot the results in Flint. A fixed number of n scans stay plotted.
     """
 
     def __init__(self) -> None:
@@ -64,45 +64,46 @@
 
         # Runtime data
         self._scans = OrderedDict()  # scan_id -> scan_info
         self._plot: Optional[ExafsPlot] = None
         self._client = None
 
     @property
-    def counters(self):
-        return self._counters[self.scan_type]
+    def counters(self) -> dict:
+        return self._counters.get(self.scan_type, dict())
 
     @property
     def scan_type(self):
         return self._scan_type
 
     @scan_type.setter
     def scan_type(self, value):
-        assert value in self._counters
+        if value not in self._counters:
+            raise ValueError(f"Valid scan types are: {list(self._counters)}")
         self._scan_type = value
 
     @property
-    def mu_name(self):
-        return self.counters["mu_name"]
+    def mu_name(self) -> Optional[str]:
+        return self.counters.get("mu_name")
 
     @mu_name.setter
     def mu_name(self, value):
         self.counters["mu_name"] = value
 
     @property
-    def energy_name(self):
-        return self.counters["energy_name"]
+    def energy_name(self) -> Optional[str]:
+        return self.counters.get("energy_name")
 
     @energy_name.setter
     def energy_name(self, value):
         self.counters["energy_name"] = value
 
     @property
-    def energy_unit(self):
-        return self.counters["energy_unit"]
+    def energy_unit(self) -> Optional[str]:
+        return self.counters.get("energy_unit")
 
     @energy_unit.setter
     def energy_unit(self, value):
         self.counters["energy_unit"] = value
 
     def _scan_type_from_scan(self, scan) -> str:
         raise NotImplementedError
@@ -348,37 +349,36 @@
             }
         )
         future = submit(args=(self.workflow,), kwargs={"inputs": inputs})
         scan_info["future"] = future
         scan_info["job_id"] = future.task_id
         scan_info["result"] = None
 
-    def __info__(self) -> str:
-        return f"Parameters:\n {self._param_info()}\n\nProcessing:\n {self._process_info()}"
+    def _info_categories(self) -> Dict[str, dict]:
+        return {"parameters": self._param_info(), "processing": self._process_info()}
 
     def _process_info(self) -> str:
-        return "\n ".join(
-            [
-                f"Scan {scan_info['scan_name']}, Job {scan_info['job_id']}, Processed = {bool(scan_info['previous_result'])}"
-                for scan_info in self._scans.values()
-            ]
-        )
+        return {
+            scan_info[
+                "scan_name"
+            ]: f"Job {scan_info['job_id']}, Processed = {bool(scan_info['previous_result'])}"
+            for scan_info in self._scans.values()
+        }
 
-    def _param_info(self) -> str:
-        info = {
+    def _param_info(self) -> dict:
+        return {
             "enabled": self.enabled,
             "scan_type": self.scan_type,
             "workflow": self.workflow,
             "mu": self.mu_name,
             "energy": self.energy_name,
             "energy_unit": self.energy_unit,
             "refresh_period": self.refresh_period,
             "max_scans": self.max_scans,
         }
-        return format_info(info)
 
     @property
     def _n_colors(self):
         return min(len(self._COLOR_PALETTE), self.max_scans + 1)
 
     _COLOR_PALETTE = [
         (87, 81, 212),
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/exafs_plotting/exafs_widgets.py` & `blissoda-0.1.0/src/blissoda/exafs/widgets.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.0.3rc0/src/blissoda/id11/xrpd_processor.py` & `blissoda-0.1.0/src/blissoda/id31/xrpd_processor_old.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,281 +1,203 @@
+"""Automatic pyfai integration for every scan with saving and plotting"""
+
 import os
 import json
-import logging
-import tempfile
-from glob import glob
-from typing import Optional, List, MutableMapping
+from typing import Dict, Optional, Sequence
 
 try:
     from bliss.scanning import scan_meta
     from bliss import current_session
 except ImportError:
     scan_meta = None
     current_session = None
 
-from ewoksjob.client import submit, convert_workflow
-
 from ..persistent import WithPersistentParameters
-from ..resources.id11 import RESOURCE_ROOT
-from ..utils.directories import get_processed_dir, get_collection_dir
-from ..utils.pyfai import read_config
-from ..utils.info import format_info
-
-logger = logging.getLogger(__name__)
-
-
-_WORKERS = "lid11eiger2lima", "lid11detector"
+from ..utils.directories import get_processed_dir
 
 
 class XrpdProcessor(
     WithPersistentParameters,
     parameters=[
-        "enabled",
-        "workflow",
+        "_enabled",
         "detector_name",
         "counter_names",
-        "pyfai_config_directory",
-        "_integration_options",
+        "pyfai_config",
+        "integration_options",
         "retry_timeout",
         "monitor_name",
         "reference",
-        "worker",
     ],
 ):
     def __init__(self) -> None:
         super().__init__()
         if current_session is None:
             raise ImportError("blissdata")
-        self._set_parameter_default("enabled", False)
-        self._set_parameter_default("_integration_options", dict())
-        self._set_parameter_default("pyfai_config_directory", tempfile.gettempdir())
-        default_workflow = os.path.join(RESOURCE_ROOT, "integrate_scan.ows")
-        self._set_parameter_default("workflow", default_workflow)
+        self._set_parameter_default("_enabled", False)
+        self._set_parameter_default(
+            "integration_options",
+            {
+                "method": "no_csr_ocl_gpu",
+                "nbpt_rad": 4096,
+                "unit": "q_nm^-1",
+            },
+        )
         self._sync_scan_metadata()
 
-    def _modify_info(self, info: dict) -> None:
-        if self.detector_name:
-            info["integration_options"] = self._format_info("... (see below)")
-
-    def __info__(self):
-        s = super().__info__()
-        if not self.detector_name:
-            return s
-        info = {
-            "1. JSON file": self._detector_config_filename(".json"),
-            "2. PONI file": self._detector_config_filename(".poni"),
-            "3. User": self._format_info(self.integration_options),
-            "Merged": self._format_info(self._merged_integration_options),
-        }
-        return f"{s}\n\nPyFai integration:\n " + format_info(info)
-
-    @property
-    def integration_options(self) -> Optional[MutableMapping]:
-        detector_name = self.detector_name
-        if not detector_name:
-            return
-        return self._integration_options.setdefault(detector_name, dict())
-
-    @property
-    def _merged_integration_options(self) -> dict:
-        """Options from user, latest pyfai json file and latest pyfai poni file.
-        The user parameters take priority over the poni parameters which take priority over the json parameters.
-        """
-        options = self._default_azint_options()
-        options.update(self._default_calib_options())
-        if self.detector_name:
-            integration_options = self.integration_options
-            if integration_options:
-                options.update(integration_options.to_dict())
-        return options
-
-    def enable(self, detector) -> None:
-        self.enabled = True
-        self.detector_name = detector.name
+    def _info_categories(self) -> Dict[str, dict]:
+        categories = super()._info_categories()
+        categories["status"] = {"Enabled": self._enabled}
+        return categories
+
+    def enable(
+        self,
+        detector_name: str,
+        counter_names: Optional[Sequence[str]],
+        pyfai_config: Optional[str] = None,
+        integration_options: Optional[Dict] = None,
+    ):
+        self._enabled = True
+        self.detector_name = detector_name
+        self.counter_names = counter_names
+        if pyfai_config is not None:
+            self.pyfai_config = pyfai_config
+        if integration_options is not None:
+            self.integration_options = integration_options
         self._sync_scan_metadata()
 
-    def disable(self) -> None:
-        self.enabled = False
-        self.detector_name = None
+    def disable(self):
+        self._enabled = False
         self._sync_scan_metadata()
 
-    def _detector_config_filename(self, ext: str) -> Optional[str]:
-        detector_name = self.detector_name
-        if not detector_name:
-            return
-        pyfai_config_directory = self.pyfai_config_directory
-        if not pyfai_config_directory:
-            pyfai_config_directory = tempfile.gettempdir()
-        pattern = os.path.join(pyfai_config_directory, detector_name, f"*{ext}")
-        files = sorted(glob(pattern))
-        if not files:
-            return
-        return files[-1]
-
-    def _default_azint_options(self) -> dict:
-        filename = self._detector_config_filename(".json")
-        return read_config(filename)
-
-    def _default_calib_options(self) -> dict:
-        filename = self._detector_config_filename(".poni")
-        return read_config(filename)
-
     def _sync_scan_metadata(self):
         scan_meta_obj = scan_meta.get_user_scan_meta()
-        if self.enabled:
+        if self._enabled:
             if "workflows" not in scan_meta_obj.used_categories_names():
                 scan_meta_obj.add_categories({"workflows"})
             scan_meta_obj.workflows.timing = scan_meta.META_TIMING.START
             scan_meta_obj.workflows.set("@NX_class", {"@NX_class": "NXcollection"})
-            scan_meta_obj.workflows.set("nxprocess1", self._get_nxprocess1_content)
+            scan_meta_obj.workflows.set("nxprocess1", self.get_nxprocess1_content)
         else:
+            try:
+                # Before Bliss 1.11
+                keys = list(scan_meta_obj._metadata.keys())
+                for key in keys:
+                    if key.name.lower() == "workflows":
+                        scan_meta_obj._metadata.pop(key)
+            except Exception:
+                pass
+            # Since Bliss 1.11
             scan_meta_obj.remove_categories({"workflows"})
 
-    def _get_nxprocess1_content(self, scan) -> Optional[dict]:
+    def get_nxprocess1_content(self, scan):
         if not scan.scan_info.get("save"):
             return
-        filename = scan.scan_info.get("filename")
-        if not filename:
+        if not scan.scan_info.get("filename"):
             return
-        scan_nb = scan.scan_info.get("scan_nb")
-        if not scan_nb:
+        if not scan.scan_info.get("scan_nb"):
             return
         detector_name = self.detector_name
-        if not detector_name:
-            return
+        assert detector_name, "detector name is missing"
         detector_info = scan.scan_info.get("channels", dict()).get(
             f"{detector_name}:image"
         )
         if not detector_info:
             return None
-
-        nxprocess_name = os.path.splitext(os.path.basename(self.workflow))[0]
-        future = convert_workflow(args=(self.workflow, None), queue=self._queue)
-        workflow = future.get(timeout=10)
-        inputs = self._get_inputs(scan, workflow)
-        nxprocess1 = {
-            nxprocess_name: {
+        return {
+            "xrpd_data_reduction": {
                 "@NX_class": "NXprocess",
                 "program": "ewoks",
-                "workflow": json.dumps(workflow),
-                "inputs": json.dumps(inputs),
+                "configuration": self.get_configuration(scan),
             }
         }
 
-        convert_destination = self._save_workflow_filename(filename, scan_nb)
-        submit(
-            args=(self.workflow,),
-            kwargs={
-                "convert_destination": convert_destination,
-                "save_options": {"indent": 2},
-                "inputs": inputs,
-            },
-            queue=self._queue,
-        )
-        return nxprocess1
-
-    @property
-    def _queue(self):
-        if self.worker not in _WORKERS:
-            return None
-        return self.worker
-
-    def _integrate_node(self, workflow: dict) -> str:
-        for nodeattrs in workflow["nodes"]:
-            if ".integrate." in nodeattrs["task_identifier"]:
-                return nodeattrs["task_identifier"]
-        return "IntegrateBlissScan"
-
-    def _save_nexus_node(self, workflow: dict) -> str:
-        for nodeattrs in workflow["nodes"]:
-            if ".nexus." in nodeattrs["task_identifier"]:
-                return nodeattrs["task_identifier"]
-        return "SaveNexusIntegrated"
-
-    def _save_nexus_url(self, filename: str, scan_nb: str) -> str:
-        root = get_processed_dir(filename)
-        subdir = os.path.basename(get_collection_dir(filename))
-        basename = os.path.basename(filename)
-        filename = os.path.join(root, subdir, basename)
-        return f"silx://{filename}::{scan_nb}.1"
-
-    def _save_workflow_filename(self, filename: str, scan_nb: str) -> str:
-        root = get_processed_dir(filename)
-        subdir = os.path.basename(get_collection_dir(filename))
-        basename = os.path.splitext(os.path.basename(filename))[0]
-        basename = f"{basename}_{scan_nb}.json"
-        return os.path.join(root, subdir, "workflows", basename)
+    def get_configuration(self, scan):
+        data = {"workflow": self.get_workflow(), "inputs": self.get_inputs(scan)}
+        return {
+            "@NX_class": "NXnote",
+            "type": "application/json",
+            "data": json.dumps(data),
+        }
 
-    def _get_inputs(self, scan, workflow: dict) -> List[dict]:
-        detector_name = self.detector_name
+    def get_inputs(self, scan):
         filename = scan.scan_info.get("filename")
         scan_nb = scan.scan_info.get("scan_nb")
+        scan_memory_url = f"{scan.root_node.db_name}:{scan._node_name}"
+        output_filename = os.path.join(
+            get_processed_dir(filename), os.path.basename(filename)
+        )
+        pyfai_config = self.pyfai_config
+        assert pyfai_config, "pyfai configuration is missing"
+        detector_name = self.detector_name
+        assert detector_name, "detector name is missing"
+
+        integration_options = self.integration_options
         counter_names = self.counter_names
         retry_timeout = self.retry_timeout
         monitor_name = self.monitor_name
         reference = self.reference
-        integration_options = self._merged_integration_options
-        integrate_identifier = self._integrate_node(workflow)
-        inputs = [
-            {
-                "task_identifier": integrate_identifier,
-                "name": "filename",
-                "value": filename,
-            },
-            {
-                "task_identifier": integrate_identifier,
-                "name": "scan",
-                "value": scan_nb,
-            },
-            {
-                "task_identifier": integrate_identifier,
-                "name": "detector_name",
-                "value": detector_name,
-            },
-            {
-                "task_identifier": integrate_identifier,
-                "name": "monitor_name",
-                "value": monitor_name,
-            },
-            {
-                "task_identifier": integrate_identifier,
-                "name": "reference",
-                "value": reference,
-            },
-            {
-                "task_identifier": integrate_identifier,
-                "name": "maximum_persistent_workers",
-                "value": 1,
-            },
+
+        lst = [
+            {"id": "config", "name": "filename", "value": pyfai_config},
+            {"id": "integrate", "name": "filename", "value": filename},
+            {"id": "integrate", "name": "scan", "value": scan_nb},
+            {"id": "integrate", "name": "scan_memory_url", "value": scan_memory_url},
+            {"id": "integrate", "name": "detector_name", "value": detector_name},
+            {"id": "integrate", "name": "output_filename", "value": output_filename},
+            {"id": "integrate", "name": "monitor_name", "value": monitor_name},
+            {"id": "integrate", "name": "reference", "value": reference},
+            {"id": "integrate", "name": "maximum_persistent_workers", "value": 1},
         ]
-        if counter_names:
-            inputs.append(
+        if integration_options:
+            lst.append(
                 {
-                    "task_identifier": integrate_identifier,
-                    "name": "counter_names",
-                    "value": counter_names,
+                    "id": "config",
+                    "name": "integration_options",
+                    "value": integration_options.to_dict(),
                 }
             )
+        if counter_names:
+            lst.append(
+                {"id": "integrate", "name": "counter_names", "value": counter_names}
+            )
         if retry_timeout:
-            inputs.append(
-                {
-                    "task_identifier": integrate_identifier,
-                    "name": "retry_timeout",
-                    "value": retry_timeout,
-                }
+            lst.append(
+                {"id": "integrate", "name": "retry_timeout", "value": retry_timeout}
             )
-        if integration_options:
-            inputs.append(
+        return lst
+
+    def get_workflow(self):
+        return {
+            "graph": {"id": "xrpd_data_reduction"},
+            "nodes": [
                 {
-                    "task_identifier": "PyFaiConfig",
-                    "name": "integration_options",
-                    "value": integration_options,
+                    "id": "config",
+                    "task_type": "class",
+                    "task_identifier": "ewoksxrpd.tasks.pyfaiconfig.PyFaiConfig",
+                },
+                {
+                    "id": "integrate",
+                    "task_type": "class",
+                    "task_identifier": "ewoksxrpd.tasks.integrate.IntegrateBlissScan",
+                },
+            ],
+            "links": [
+                {
+                    "source": "config",
+                    "target": "integrate",
+                    "data_mapping": [
+                        {"source_output": "energy", "target_input": "energy"},
+                        {"source_output": "detector", "target_input": "detector"},
+                        {
+                            "source_output": "detector_config",
+                            "target_input": "detector_config",
+                        },
+                        {"source_output": "geometry", "target_input": "geometry"},
+                        {"source_output": "mask", "target_input": "mask"},
+                        {
+                            "source_output": "integration_options",
+                            "target_input": "integration_options",
+                        },
+                    ],
                 }
-            )
-        inputs.append(
-            {
-                "task_identifier": self._save_nexus_node(workflow),
-                "name": "url",
-                "value": self._save_nexus_url(filename, scan_nb),
-            }
-        )
-        return inputs
+            ],
+        }
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/id22/stscan_processor.py` & `blissoda-0.1.0/src/blissoda/id22/stscan_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,42 +4,43 @@
     DEMO_SESSION [1]: from blissoda.demo.stscan_processor import stscan_processor
     DEMO_SESSION [2]: stscan_processor
     DEMO_SESSION [3]: stscan_processor.submit_workflows()
 """
 
 import os
 import json
+from typing import Dict, List
 from contextlib import contextmanager
 
 try:
     from bliss import current_session
 except ImportError:
     current_session = None
 
 from ewoksjob.client import submit
 from ..persistent import WithPersistentParameters
-from ..utils.info import format_info
 from ..utils.directories import get_processed_dir
+from ..persistent import ParameterInfo
 
 
 class _NoRepr:
     def __repr__(self):
         return ""
 
 
 _NOREPR = _NoRepr()
 
 
 class StScanProcessor(
     WithPersistentParameters,
     parameters=[
-        "_convert_workflow",
-        "_rebinsum_workflow",
-        "_extract_workflow",
-        "session_in_outprefix",
+        ParameterInfo("_convert_workflow"),
+        ParameterInfo("_rebinsum_workflow"),
+        ParameterInfo("_extract_workflow"),
+        ParameterInfo("session_in_outprefix"),
     ],
 ):
     """Submit data processing workflows on stscan results
 
     StScanProcessor().submit_workflows()
     """
 
@@ -94,93 +95,93 @@
             with self._extract_context():
                 self._extract_workflow = value
         else:
             self._extract_workflow = value
             with self._extract_context():
                 pass
 
-    def __info__(self) -> str:
+    def _info_categories(self) -> Dict[str, dict]:
         with self._convert_context():
             with self._rebinsum_context():
                 with self._extract_context():
-                    info = [
-                        f"Workflows:\n {self._workflows_info()}",
-                        f"Execution:\n {self._execution_info()}",
-                        f"Convert:\n {self._convert_info()}",
-                        f"Rebin:\n {self._rebin_info()}",
-                        f"Sum:\n {self._sum_info()}",
-                        f"Extract:\n {self._extract_info()}",
-                    ]
-                    return "\n\n".join(info)
+                    return {
+                        "workflows": self._workflows_info(),
+                        "execution": self._execution_info(),
+                        "convert": self._convert_info(),
+                        "rebin": self._rebin_info(),
+                        "sum": self._sum_info(),
+                        "extract": self._extract_info(),
+                    }
 
-    def _execution_info(self) -> str:
+    def _execution_info(self) -> dict:
         info = dict()
         info["session_in_outprefix"] = self.session_in_outprefix
-        return format_info(info)
+        return info
 
-    def _workflows_info(self) -> str:
+    def _workflows_info(self) -> dict:
         info = dict()
         info["convert"] = self.convert_workflow
         info["rebin/sum"] = self.rebinsum_workflow
         info["extract"] = self.extract_workflow
-        return format_info(info)
+        return info
 
-    def _convert_info(self) -> str:
+    def _convert_info(self) -> dict:
         info = dict()
         info["do_convert"] = self.do_convert
         info["Results:"] = _NOREPR
         info.update(self._outdirs_info(self.convertdirs))
         info[" include_proposal_outdir"] = self.convert_include_proposal_outdir
-        return format_info(info)
+        return info
 
-    def _rebin_info(self) -> str:
+    def _rebin_info(self) -> dict:
         info = dict()
         info["do_rebin"] = self.do_rebin
 
         info["Parameters:"] = _NOREPR
         info[" range"] = self.range
         info[" delta2theta"] = self.delta2theta
         info[" startp"] = self.startp
         info[" parsfile"] = self.parsfile
 
         info["Results:"] = _NOREPR
         info.update(self._outdirs_info(self.rebindirs))
         info[" include_proposal_outdir"] = self.rebin_include_proposal_outdir
 
-        return format_info(info)
+        return info
 
-    def _sum_info(self) -> str:
+    def _sum_info(self) -> dict:
         info = dict()
-        info["do_sum"] = self.do_sum
+        info["do_sum_single"] = self.do_sum_single
+        info["do_sum_all"] = self.do_sum_all
 
         info["Parameters:"] = _NOREPR
         info[" binsize"] = self.binsize
         info[" resfile"] = self.resfile
 
         info["Results:"] = _NOREPR
         info[" include_proposal_outdir"] = self.sum_include_proposal_outdir
 
-        return format_info(info)
+        return info
 
-    def _extract_info(self) -> str:
+    def _extract_info(self) -> dict:
         info = dict()
         info["do_extract"] = self.do_extract
 
         info["Parameters:"] = _NOREPR
         info[" tth_min"] = self.tth_min
         info[" tth_max"] = self.tth_max
         info[" full_tth"] = self.full_tth
         info[" startp"] = self.startp
         info[" inp_file"] = self.inp_file
         info[" inp_step"] = self.inp_step
 
         info["Results:"] = _NOREPR
         info[" include_proposal_outdir"] = self.extract_include_proposal_outdir
 
-        return format_info(info)
+        return info
 
     @property
     def convertdirs(self):
         with self._convert_context() as workflow:
             return self._get_node_parameter(workflow, "convert", "outdirs")
 
     @convertdirs.setter
@@ -231,28 +232,55 @@
             if self.session_in_outprefix:
                 outprefix = f"{current_session.scan_saving.proposal_name}_{current_session.scan_saving.proposal_session_name}"
             else:
                 outprefix = current_session.scan_saving.proposal_name
         if filename is None:
             filename = current_session.scan_saving.filename
         if self.do_convert:
-            self._submit_convert_workflow(filename, entries, outprefix, list())
+            convert_destination = self._convert_destination(
+                "convert", filename, scan=scannr
+            )
+            self._submit_convert_workflow(
+                filename, entries, outprefix, list(), convert_destination
+            )
         if extract:
-            self._submit_extract_workflow(filename, entries, outprefix, list())
+            convert_destination = self._convert_destination(
+                "extract", filename, scan=scannr
+            )
+            self._submit_extract_workflow(
+                filename, entries, outprefix, list(), convert_destination
+            )
         elif self.do_rebin:
-            for inputs in self._iter_rebinsum_parameters():
-                self._submit_rebinsum_workflow(filename, entries, outprefix, inputs)
+            for inputs, kw in self._iter_rebinsum_parameters():
+                convert_destination = self._convert_destination(
+                    "rebinsum", filename, scan=scannr, **kw
+                )
+                self._submit_rebinsum_workflow(
+                    filename, entries, outprefix, inputs, convert_destination
+                )
 
     def _iter_rebinsum_parameters(self):
         for binsize in self.binsize:
             for delta2theta in self.delta2theta:
-                yield [
+                inputs = [
                     {"id": "rebin", "name": "delta2theta", "value": delta2theta},
                     {"id": "sum", "name": "binsize", "value": binsize},
                 ]
+                convert_destination = {"w": delta2theta, "b": binsize}
+                yield inputs, convert_destination
+
+    def _convert_destination(self, workflowname, filename, **kw):
+        dirname = os.path.join(get_processed_dir(filename), "workflows", workflowname)
+        basename = os.path.splitext(os.path.basename(filename))[0]
+        for name, value in kw.items():
+            if value is None:
+                continue
+            value = str(value).replace(".", "")
+            basename += f"_{name}{value}"
+        return os.path.join(dirname, basename + ".json")
 
     @property
     def delta2theta(self):
         with self._rebinsum_context() as workflow:
             delta2theta_list = self._get_node_parameter(
                 workflow, "rebin", "delta2theta", dest="for_bliss"
             )
@@ -417,57 +445,94 @@
             self._set_node_parameter(workflow, "rebin", "do", value, dest="for_bliss")
 
     @property
     def do_convert(self):
         return True
 
     @property
-    def do_sum(self):
+    def do_sum_single(self):
         with self._rebinsum_context() as workflow:
-            sum_single = self._get_node_parameter(workflow, "sum", "sum_single")
-            sum_all = self._get_node_parameter(workflow, "sum", "sum_all")
-            return sum_single or sum_all
+            return self._get_node_parameter(workflow, "sum", "sum_single")
 
-    @do_sum.setter
-    def do_sum(self, value):
+    @do_sum_single.setter
+    def do_sum_single(self, value):
         with self._rebinsum_context() as workflow:
             self._set_node_parameter(workflow, "sum", "sum_single", value)
+        if value:
+            self.do_rebin = True
+
+    @property
+    def do_sum_all(self):
+        with self._rebinsum_context() as workflow:
+            return self._get_node_parameter(workflow, "sum", "sum_all")
+
+    @do_sum_all.setter
+    def do_sum_all(self, value):
+        with self._rebinsum_context() as workflow:
             self._set_node_parameter(workflow, "sum", "sum_all", value)
         if value:
-            self.do_rebin = bool(value)
+            self.do_rebin = True
 
     @property
     def do_extract(self):
         return "< from command stscan(..., extract=False) >"
 
-    def _submit_convert_workflow(self, filename, entries, outprefix, inputs):
-        workflow = self.convert_workflow
+    def _submit_convert_workflow(
+        self,
+        filename: str,
+        entries: List[str],
+        outprefix: str,
+        inputs: List[dict],
+        convert_destination: str,
+    ):
+        with self._convert_context() as workflow:
+            pass
         primary_outdir = get_processed_dir(filename)
         self._add_wait_convert_inputs(inputs, filename, entries)
         self._add_convert_inputs(inputs, outprefix, primary_outdir)
-        self._submit_job(workflow, inputs, queue="solo1")
+        self._submit_job(workflow, inputs, convert_destination, queue="solo1")
 
-    def _submit_rebinsum_workflow(self, filename, entries, outprefix, inputs):
-        workflow = self.rebinsum_workflow
+    def _submit_rebinsum_workflow(
+        self,
+        filename: str,
+        entries: List[str],
+        outprefix: str,
+        inputs: List[dict],
+        convert_destination: str,
+    ):
+        with self._rebinsum_context() as workflow:
+            pass
         primary_outdir = get_processed_dir(filename)
         self._add_wait_rebin_inputs(inputs, filename, entries)
         self._add_rebin_inputs(inputs, outprefix, primary_outdir)
         self._add_convertrebin_inputs(inputs, primary_outdir)
         self._add_sum_inputs(inputs, primary_outdir)
-        self._submit_job(workflow, inputs, queue="solo2")
+        self._submit_job(workflow, inputs, convert_destination, queue="solo2")
 
-    def _submit_extract_workflow(self, filename, entries, outprefix, inputs):
-        workflow = self.extract_workflow
+    def _submit_extract_workflow(
+        self,
+        filename: str,
+        entries: List[str],
+        outprefix: str,
+        inputs: List[dict],
+        convert_destination: str,
+    ):
+        with self._extract_context() as workflow:
+            pass
         primary_outdir = get_processed_dir(filename)
         self._add_wait_extract_inputs(inputs, filename, entries)
         self._add_extract_inputs(inputs, outprefix, primary_outdir)
-        self._submit_job(workflow, inputs, queue="solo2")
+        self._submit_job(workflow, inputs, convert_destination, queue="solo2")
 
-    def _submit_job(self, workflow, inputs, **kw):
-        submit(args=(workflow,), kwargs={"inputs": inputs}, **kw)
+    def _submit_job(self, workflow, inputs, convert_destination, **kw):
+        submit(
+            args=(workflow,),
+            kwargs={"inputs": inputs, "convert_destination": convert_destination},
+            **kw,
+        )
 
     def _save_default_convert_workflow(self):
         workflow = self._convert_graph()
         self._add_wait_convert_default_inputs(workflow)
         self._add_convert_default_inputs(workflow)
         self._save_workflow(self.convert_workflow, workflow)
         return workflow
@@ -734,15 +799,15 @@
         node_attrs = self._get_node_attrs(workflow, "rebin")
         node_attrs["for_bliss"] = [{"name": "do", "value": False}]
         node_attrs["default_inputs"] = [
             {
                 "name": "parsfile",
                 "value": "/data/id22/inhouse/CD_GC_PDF/advanced_50keV/patterns/for_wout/out7.pars",
             },
-            {"name": "range", "value": [0.0, float("inf")]},
+            {"name": "range", "value": [float("nan"), float("nan")]},
             {"name": "delta2theta", "value": 0.003},
             {"name": "startp", "value": 31},
             {"name": "device", "value": 0},
             {
                 "name": "outdirs",
                 "value": {
                     "primary": "opid22@diffract22new:/users/opid22/data1/",
@@ -767,14 +832,15 @@
                 "value": {
                     "primary": "opid22@diffract22new:/users/opid22/data1/",
                     # "secondary": "opid22@diffract22bliss:/users/opid22/data1/",
                     "backup": "opid22@diffract22bliss:/data/id22/backup/data22/",
                 },
             },
             {"name": "retry_timeout", "value": 30},
+            {"name": "ascii_extension", "value": ".adv"},
         ]
 
     def _add_sum_inputs(self, inputs: list, primary_outdir: str):
         if self.sum_include_proposal_outdir:
             inputs += [{"id": "sum", "name": "primary_outdir", "value": primary_outdir}]
 
     def _add_sum_default_inputs(self, workflow: dict):
@@ -784,14 +850,15 @@
                 "name": "resfile",
                 "value": "/data/id22/inhouse/CD_GC_PDF/advanced_50keV/patterns/for_wout/temp.res",
             },
             {"name": "binsize", "value": 0.002},
             {"name": "sum_single", "value": False},
             {"name": "sum_all", "value": False},
             {"name": "retry_timeout", "value": 30},
+            {"name": "ascii_extension", "value": ".adv"},
         ]
 
     def _add_convert_inputs(self, inputs: list, outprefix: str, primary_outdir: str):
         if self.convert_include_proposal_outdir:
             inputs += [
                 {"id": "convert", "name": "outprefix", "value": outprefix},
                 {
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/persistent.py` & `blissoda-0.1.0/src/blissoda/persistent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections.abc import MutableMapping
-from typing import Callable, Any, Iterator, Mapping, Iterable
+from dataclasses import dataclass
+from typing import Callable, Any, Iterator, Mapping, Iterable, Dict, Optional
 
 try:
     from bliss import current_session
 except ImportError:
     current_session = None
 try:
     from bliss.common.utils import autocomplete_property
@@ -15,68 +16,87 @@
     try:
         from bliss.config import settings
     except ImportError:
         settings = None
 from .utils.info import format_info
 
 
+@dataclass
+class ParameterInfo:
+    name: str
+    category: str = "parameters"
+    hidden: Optional[bool] = None
+
+    def __post_init__(self):
+        if self.hidden is None:
+            self.hidden = self.name.startswith("_")
+
+
 class WithPersistentParameters:
     """Adds parameters as properties that will be stored in Redis
 
     .. code:: python
 
         class MyClass(WithPersistentParameters, parameters=["a", "b"])
             pass
 
         myobj = MyClass()
         myobj.a = 10
         myobj.b = None  # remove
     """
 
-    _PARAMETERS = list()
+    _PARAMETERS: Dict[str, ParameterInfo] = dict()
 
     def __init__(self) -> None:
-        if settings is None:
+        if current_session is None:
             raise ModuleNotFoundError("No module named 'bliss'")
         self._parameters = settings.HashObjSetting(
             f"blissoda:{current_session.name}:{self.__class__.__name__}"
         )
 
     def __init_subclass__(cls, parameters=None, **kw) -> None:
         super().__init_subclass__(**kw)
-        if parameters is None:
-            parameters = list()
+        if parameters:
+            extra_parameters = list()
+            for p in parameters:
+                if isinstance(p, str):
+                    p = ParameterInfo(name=p)
+                elif isinstance(p, Mapping):
+                    p = ParameterInfo(**p)
+                extra_parameters.append(p)
+            extra_parameters = {p.name: p for p in extra_parameters}
         else:
-            parameters = [p for p in parameters if p not in cls._PARAMETERS]
-        cls._PARAMETERS = cls._PARAMETERS + parameters
-        for name in parameters:
+            extra_parameters = dict()
+        cls._PARAMETERS = {**cls._PARAMETERS, **extra_parameters}
+        for name in extra_parameters:
             add_parameter_property(cls, name)
 
     def __dir__(self) -> Iterable[str]:
         return list(super().__dir__()) + [
-            s for s in self._PARAMETERS if not s.startswith("_")
+            name for name, param in self._PARAMETERS.items() if not param.hidden
         ]
 
-    def __info__(self):
-        info = self._parameters.get_all()
-        info = {
-            k: self._format_info(info.get(k, None))
-            for k in self._PARAMETERS
-            if not k.startswith("_")
-        }
-        self._modify_info(info)
-        return "Parameters:\n " + format_info(info)
-
-    def _format_info(self, value):
-        if isinstance(value, RemoteDictWrapper):
-            return value.to_dict()
-        return value
-
-    def _modify_info(self, info: dict) -> None:
-        pass
+    def _info_categories(self) -> Dict[str, dict]:
+        categories = dict()
+        all_values = self._parameters.get_all()
+        for name, param in self._PARAMETERS.items():
+            if param.hidden:
+                continue
+            category = categories.setdefault(param.category, dict())
+            category[name] = all_values.get(name)
+        return categories
+
+    def __info__(self) -> str:
+        return "\n\n".join(
+            [
+                f"{name.capitalize()}:\n {format_info(category)}"
+                for name, category in self._info_categories().items()
+                if category
+            ]
+        )
 
     def _get_parameter(self, name):
         v = self._parameters.get(name)
         if isinstance(v, dict):
             return RedisDictWrapper(name, self._parameters.get, self._set_parameter)
         return v
 
@@ -95,14 +115,16 @@
     def _raise_when_missing(self, *names):
         for name in names:
             if self._get_parameter(name) is None:
                 raise AttributeError(f"parameter '{name}' is not set")
 
 
 def add_parameter_property(cls, name):
+    if hasattr(cls, name):
+        return
     method = autocomplete_property(lambda self: self._get_parameter(name))
     setattr(cls, name, method)
     method = getattr(cls, name).setter(
         lambda self, value: self._set_parameter(name, value)
     )
     setattr(cls, name, method)
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/resources/bm23/bm23.ows` & `blissoda-0.1.0/src/blissoda/resources/exafs/exafs.ows`

 * *Files identical despite different names*

### Comparing `blissoda-0.0.3rc0/src/blissoda/resources/streamline/time_record.py` & `blissoda-0.1.0/src/blissoda/resources/streamline/time_record.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.0.3rc0/src/blissoda/seslab/streamline_scanner.py` & `blissoda-0.1.0/src/blissoda/seslab/streamline_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 try:
     from bliss import setup_globals
 except ImportError:
     setup_globals = None
 
 from streamline_changer.sample_changer import SampleChanger
-from ..streamline.streamline_scanner import StreamlineScanner
+from ..streamline.scanner import StreamlineScanner
 
 
 class StreamlineSesScanner(StreamlineScanner):
     def __init__(self):
         super().__init__()
         self._set_parameter_default("sample_changer_name", "streamline_sc")
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/streamline/streamline_scanner.py` & `blissoda-0.1.0/src/blissoda/streamline/scanner.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 import os
 import re
 import shutil
 from numbers import Number
 from contextlib import contextmanager
-from typing import Optional, NamedTuple, Tuple
+from typing import Optional, NamedTuple, Tuple, Dict
 import numpy
 
 try:
     from bliss import current_session
     from bliss import setup_globals
     from bliss.common.logtools import user_warning, user_info, elog_print
 except ImportError:
@@ -27,58 +27,72 @@
     user_info = print
     elog_print = print
 
 try:
     from ewoksjob.client import submit
 except ImportError:
     submit = None
+
 from ..persistent import WithPersistentParameters
-from ..resources.streamline import RESOURCE_ROOT
-from ..utils.info import format_info
-from ..utils.directories import get_processed_dir
+from ..persistent import ParameterInfo
+from ..utils import directories
+from ..resources.xrpd import RESOURCE_ROOT
 
 
 class ScanInfo(NamedTuple):
     filename: str
     scan_nb: int
 
     @property
     def url(self):
         return f"{self.filename}::/{self.scan_nb}.1"
 
 
 class StreamlineScanner(
     WithPersistentParameters,
     parameters=[
-        "workflow",
-        "sample_changer_name",
-        "detector_name",
-        "energy_name",
-        "calibrations",
-        "calibration_motor",
-        "image_slice",
-        "integration_options",
-        "pyfai_config",
-        "calibrant",
-        "trigger_workflows",
+        ParameterInfo("workflow", category="data processing"),
+        ParameterInfo("sample_changer_name", category="names"),
+        ParameterInfo("detector_name", category="names"),
+        ParameterInfo("energy_name", category="names"),
+        ParameterInfo("calibrations", category="calibration"),
+        ParameterInfo("calibration_motor", category="calibration"),
+        ParameterInfo("image_slice", category="PyFai"),
+        ParameterInfo("integration_options", category="PyFai"),
+        ParameterInfo("pyfai_config", category="PyFai"),
+        ParameterInfo("calibrant", category="calibration"),
+        ParameterInfo("trigger_workflows", category="data processing"),
+        ParameterInfo("vibration_speed_during_scan", category="sample changer"),
     ],
 ):
     def __init__(self) -> None:
         super().__init__()
         self._set_parameter_default("image_slice", 0)
         self._set_parameter_default("trigger_workflows", True)
+        self._set_parameter_default("vibration_speed_during_scan", 40)
 
-    def __info__(self):
-        s = super().__info__()
-        info = {
-            "# sample holders": self.sample_changer.number_of_remaining_baguettes,
-            "selected sample": int(self.sample_changer.translation.position),
-            "vibration speed (%)": self.sample_changer.vibration_speed,
+    def _info_categories(self) -> Dict[str, dict]:
+        categories = super()._info_categories()
+        try:
+            sample_changer = self.sample_changer
+        except (AttributeError, KeyError):
+            return categories
+        categories["status"] = {
+            "# sample holders left": sample_changer.number_of_remaining_baguettes,
+            "selected sample": int(sample_changer.translation.position),
+            "vibration speed (%)": sample_changer.vibration_speed,
+            "automatic calibration": self.workflow_has_calib,
+            "calibration": "OFF",
+            "flat-field": "OFF",
         }
-        return f"{s}\n\nStatus:\n " + format_info(info)
+        if self.workflow_has_calib:
+            categories["status"]["calibration"] = self._get_calibration().get("image")
+        if self.workflow_has_flatfield:
+            categories["status"]["flat-field"] = "ON"
+        return categories
 
     def measure_sample(self, *args, **kwargs):
         return setup_globals.sct(*args, **kwargs)
 
     @property
     def sample_changer(self):
         self._raise_when_missing("sample_changer_name")
@@ -172,34 +186,37 @@
 
     def select_sample(self, sample_index: int):
         self.sample_changer.translation.on()
         return self.sample_changer.select_sample(sample_index)
 
     def init_workflow(self, with_calibration: bool = False):
         if with_calibration:
-            filename = "streamline_with_calib.ows"
+            basename = "streamline_with_calib"
         else:
-            filename = "streamline_without_calib.ows"
-        basename = os.path.splitext(filename)[0]
-        source = os.path.join(RESOURCE_ROOT, filename)
+            basename = "streamline_without_calib"
+        filename = f"{basename}.json"
+
         dirname = self._get_workflows_dirname(current_session.scan_saving.filename)
-        os.makedirs(dirname, exist_ok=True)
-        destination = os.path.join(dirname, f"{basename}.ows")
-        i = 1
-        while os.path.exists(destination):
-            destination = os.path.join(dirname, f"{basename}{i}.ows")
-            i += 1
-        shutil.copyfile(source, destination)
+        destination = os.path.join(dirname, filename)
+        if not os.path.exists(destination):
+            os.makedirs(dirname, exist_ok=True)
+            source = os.path.join(RESOURCE_ROOT, filename)
+            shutil.copyfile(source, destination)
+
         self.workflow = destination
         user_info(f"Active data processing workflow: {destination}")
 
     @property
     def workflow_has_calib(self):
         return self.workflow and "with_calib" in self.workflow
 
+    @property
+    def workflow_has_flatfield(self):
+        return self.workflow and "with_flat" in self.workflow
+
     def _set_calibration_scan(self, scan_info: ScanInfo):
         if not scan_info.filename:
             user_warning("Cannot use as calibration because no data was collected")
             return
         info = {
             "image": self._get_image_url(scan_info),
             "gallery_directory": self._get_gallery_directory(scan_info.filename),
@@ -215,15 +232,15 @@
             return
         args, kwargs = self._job_arguments(scan_info, processed_metadata)
         submit(args=args, kwargs=kwargs)
 
     @contextmanager
     def run_context(self):
         self.sample_changer.translation.on()
-        self.sample_changer.vibration_speed = 100
+        self.sample_changer.vibration_speed = self.vibration_speed_during_scan
         elog_print("Start streamline run")
         try:
             yield
         finally:
             self.sample_changer.vibration_speed = 0
             elog_print("End streamline run")
 
@@ -303,25 +320,25 @@
         metadata["Sample_name"] = current_session.scan_saving.dataset["Sample_name"]
         return metadata
 
     def _get_calibration_position(self) -> Optional[Number]:
         if self.calibration_motor:
             return getattr(setup_globals, self.calibration_motor).position
 
-    def _get_calibration(self) -> Optional[dict]:
+    def _get_calibration(self) -> dict:
         calibrations = self.calibrations
         if not calibrations:
-            return None
+            return dict()
         position = self._get_calibration_position()
         if position is not None:
             positions = [p for p in calibrations if p is not None]
             if positions:
                 idx = (numpy.abs(numpy.array(positions) - position)).argmin()
                 position = positions[idx]
-        return calibrations.get(position)
+        return calibrations.get(position, dict())
 
     def _get_scan_info(self, scan) -> ScanInfo:
         if scan is None:
             return ScanInfo(filename="", scan_nb=0)
         if isinstance(scan, ScanInfo):
             return scan
         filename = scan.scan_info.get("filename")
@@ -334,21 +351,20 @@
         if image_slice is not None:
             image_slice = str(image_slice)
             image_slice = re.sub(r"[\s\(\)]+", "", image_slice)
             url = f"{url}&slice={image_slice}"
         return url
 
     def _get_output_dir(self, dataset_filename: str) -> str:
-        return os.path.join(get_processed_dir(dataset_filename), "streamline")
+        return os.path.join(
+            directories.get_processed_dir(dataset_filename), "streamline"
+        )
 
     def _get_transient_dirname(self, dataset_filename: str) -> str:
-        return os.path.join(get_processed_dir(dataset_filename), "_nobackup")
-
-    def _get_workflows_dirname(self, dataset_filename: str) -> str:
-        return os.path.join(get_processed_dir(dataset_filename), "workflows")
+        return directories.get_nobackup_dir(dataset_filename)
 
     def _get_output_dirname(self, dataset_filename: str) -> str:
         filename = os.path.basename(dataset_filename)
         return os.path.join(
             self._get_output_dir(dataset_filename), os.path.splitext(filename)[0]
         )
 
@@ -396,23 +412,14 @@
             self._raise_when_missing("calibrations", "calibrant")
 
         inputs = list()
 
         integrate_image_url = self._get_image_url(scan_info)
 
         # Configuration
-        if self.energy_name:
-            energy = getattr(setup_globals, self.energy_name).position
-            inputs.append(
-                {
-                    "task_identifier": "PyFaiConfig",
-                    "name": "energy",
-                    "value": energy,
-                }
-            )
         if self.integration_options:
             inputs.append(
                 {
                     "task_identifier": "PyFaiConfig",
                     "name": "integration_options",
                     "value": self.integration_options.to_dict(),
                 }
@@ -433,15 +440,15 @@
                     "value": self.calibrant,
                 }
             )
 
         # Calibration
         if self.workflow_has_calib:
             calibration = self._get_calibration()
-            if calibration is None:
+            if not calibration:
                 raise RuntimeError("no valid calibration found")
 
             inputs += [
                 {
                     "task_identifier": "CalibrateSingle",
                     "name": "image",
                     "value": calibration["image"],
@@ -461,15 +468,15 @@
                     "name": "image",
                     "value": calibration["image"],
                 },
                 {
                     "task_identifier": "DiagnoseCalibrateSingleResults",
                     "name": "filename",
                     "value": os.path.join(
-                        calibration["gallery_directory"], "ring_detection.png"
+                        calibration["gallery_directory"], "ring_detection.svg"
                     ),
                 },
             ]
 
             if calibration["image"] == integrate_image_url and self.calibrant:
                 inputs += [
                     {
@@ -533,15 +540,15 @@
 
         inputs += [
             {
                 "task_identifier": "DiagnoseIntegrate1D",
                 "name": "filename",
                 "value": os.path.join(
                     self._get_gallery_directory(scan_info.filename),
-                    "integrate.png",
+                    "integrate.svg",
                 ),
             },
         ]
 
         # Job arguments
         args = (self.workflow,)
         convert_destination = self._get_workflow_save_filename(scan_info.filename)
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/tests/conftest.py` & `blissoda-0.1.0/src/blissoda/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.0.3rc0/src/blissoda/tests/test_id22.py` & `blissoda-0.1.0/src/blissoda/tests/test_id22.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import json
 import pytest
 from unittest import mock
 from ..id22.stscan_processor import StScanProcessor
 
 _FILENAME = os.path.abspath(
     "/data/visitor/id000000/id00/20230227/raw/Blank/Blank_0001/Blank_0001.h5"
 )
@@ -73,230 +74,285 @@
 
 
 def test_info(stscan_processor):
     assert stscan_processor.__info__()
 
 
 def test_submit_convert(stscan_processor, submit_mock, tmpdir):
-    stscan_processor.submit_workflows()
+    stscan_processor.submit_workflows(scannr=1)
 
     calls = [
         mock.call(
-            args=(str(tmpdir / "convert.json"),),
+            args=(_read_workflow(tmpdir / "convert.json"),),
             kwargs={
                 "inputs": [
                     {"id": "wait", "name": "filename", "value": _FILENAME},
-                    {"id": "wait", "name": "entries", "value": []},
+                    {"id": "wait", "name": "entries", "value": ["1.1", "1.2"]},
                     {"id": "convert", "name": "outprefix", "value": "id000000"},
                     {
                         "id": "convert",
                         "name": "primary_outdir",
                         "value": _PROCESSED_DIR,
                     },
-                ]
+                ],
+                "convert_destination": os.path.join(
+                    _PROCESSED_DIR, "workflows", "convert", "Blank_0001_scan1.json"
+                ),
             },
             queue="solo1",
         )
     ]
 
     submit_mock.assert_has_calls(calls)
 
 
 def test_submit_rebin(stscan_processor, submit_mock, tmpdir):
     stscan_processor.do_rebin = True
     stscan_processor.submit_workflows()
 
     calls = [
         mock.call(
-            args=(str(tmpdir / "convert.json"),),
+            args=(_read_workflow(tmpdir / "convert.json"),),
             kwargs={
                 "inputs": [
                     {"id": "wait", "name": "filename", "value": _FILENAME},
                     {"id": "wait", "name": "entries", "value": []},
                     {"id": "convert", "name": "outprefix", "value": "id000000"},
                     {
                         "id": "convert",
                         "name": "primary_outdir",
                         "value": _PROCESSED_DIR,
                     },
-                ]
+                ],
+                "convert_destination": os.path.join(
+                    _PROCESSED_DIR, "workflows", "convert", "Blank_0001.json"
+                ),
             },
             queue="solo1",
         ),
         mock.call(
-            args=(str(tmpdir / "rebinsum.json"),),
+            args=(_read_workflow(tmpdir / "rebinsum.json"),),
             kwargs={
                 "inputs": [
                     {"id": "rebin", "name": "delta2theta", "value": 0.003},
                     {"id": "sum", "name": "binsize", "value": 0.002},
                     {"id": "wait", "name": "filename", "value": _FILENAME},
                     {"id": "wait", "name": "entries", "value": []},
                     {"id": "rebin", "name": "outprefix", "value": "id000000"},
                     {"id": "rebin", "name": "primary_outdir", "value": _PROCESSED_DIR},
                     {
                         "id": "convert",
                         "name": "primary_outdir",
                         "value": _PROCESSED_DIR,
                     },
                     {"id": "sum", "name": "primary_outdir", "value": _PROCESSED_DIR},
-                ]
+                ],
+                "convert_destination": os.path.join(
+                    _PROCESSED_DIR,
+                    "workflows",
+                    "rebinsum",
+                    "Blank_0001_w0003_b0002.json",
+                ),
             },
             queue="solo2",
         ),
     ]
 
     submit_mock.assert_has_calls(calls)
 
 
 def test_submit_sum(stscan_processor, submit_mock, tmpdir):
-    stscan_processor.do_sum = True
+    stscan_processor.do_sum_single = True
+    stscan_processor.do_sum_all = True
     stscan_processor.submit_workflows()
 
     calls = [
         mock.call(
-            args=(str(tmpdir / "convert.json"),),
+            args=(_read_workflow(tmpdir / "convert.json"),),
             kwargs={
                 "inputs": [
                     {"id": "wait", "name": "filename", "value": _FILENAME},
                     {"id": "wait", "name": "entries", "value": []},
                     {"id": "convert", "name": "outprefix", "value": "id000000"},
                     {
                         "id": "convert",
                         "name": "primary_outdir",
                         "value": _PROCESSED_DIR,
                     },
-                ]
+                ],
+                "convert_destination": os.path.join(
+                    _PROCESSED_DIR, "workflows", "convert", "Blank_0001.json"
+                ),
             },
             queue="solo1",
         ),
         mock.call(
-            args=(str(tmpdir / "rebinsum.json"),),
+            args=(_read_workflow(tmpdir / "rebinsum.json"),),
             kwargs={
                 "inputs": [
                     {"id": "rebin", "name": "delta2theta", "value": 0.003},
                     {"id": "sum", "name": "binsize", "value": 0.002},
                     {"id": "wait", "name": "filename", "value": _FILENAME},
                     {"id": "wait", "name": "entries", "value": []},
                     {"id": "rebin", "name": "outprefix", "value": "id000000"},
                     {"id": "rebin", "name": "primary_outdir", "value": _PROCESSED_DIR},
                     {
                         "id": "convert",
                         "name": "primary_outdir",
                         "value": _PROCESSED_DIR,
                     },
                     {"id": "sum", "name": "primary_outdir", "value": _PROCESSED_DIR},
-                ]
+                ],
+                "convert_destination": os.path.join(
+                    _PROCESSED_DIR,
+                    "workflows",
+                    "rebinsum",
+                    "Blank_0001_w0003_b0002.json",
+                ),
             },
             queue="solo2",
         ),
     ]
 
     submit_mock.assert_has_calls(calls)
 
 
 def test_submit_sum_multiparams(stscan_processor, submit_mock, tmpdir):
-    stscan_processor.do_sum = True
+    stscan_processor.do_sum_single = True
+    stscan_processor.do_sum_all = True
     stscan_processor.binsize = [0.002, 0.003]
     stscan_processor.delta2theta = [0.004, 0.005]
 
     stscan_processor.submit_workflows()
 
     calls = [
         mock.call(
-            args=(str(tmpdir / "convert.json"),),
+            args=(_read_workflow(tmpdir / "convert.json"),),
             kwargs={
                 "inputs": [
                     {"id": "wait", "name": "filename", "value": _FILENAME},
                     {"id": "wait", "name": "entries", "value": []},
                     {"id": "convert", "name": "outprefix", "value": "id000000"},
                     {
                         "id": "convert",
                         "name": "primary_outdir",
                         "value": _PROCESSED_DIR,
                     },
-                ]
+                ],
+                "convert_destination": os.path.join(
+                    _PROCESSED_DIR, "workflows", "convert", "Blank_0001.json"
+                ),
             },
             queue="solo1",
         ),
         mock.call(
-            args=(str(tmpdir / "rebinsum.json"),),
+            args=(_read_workflow(tmpdir / "rebinsum.json"),),
             kwargs={
                 "inputs": [
                     {"id": "rebin", "name": "delta2theta", "value": 0.004},
                     {"id": "sum", "name": "binsize", "value": 0.002},
                     {"id": "wait", "name": "filename", "value": _FILENAME},
                     {"id": "wait", "name": "entries", "value": []},
                     {"id": "rebin", "name": "outprefix", "value": "id000000"},
                     {"id": "rebin", "name": "primary_outdir", "value": _PROCESSED_DIR},
                     {
                         "id": "convert",
                         "name": "primary_outdir",
                         "value": _PROCESSED_DIR,
                     },
                     {"id": "sum", "name": "primary_outdir", "value": _PROCESSED_DIR},
-                ]
+                ],
+                "convert_destination": os.path.join(
+                    _PROCESSED_DIR,
+                    "workflows",
+                    "rebinsum",
+                    "Blank_0001_w0004_b0002.json",
+                ),
             },
             queue="solo2",
         ),
         mock.call(
-            args=(str(tmpdir / "rebinsum.json"),),
+            args=(_read_workflow(tmpdir / "rebinsum.json"),),
             kwargs={
                 "inputs": [
                     {"id": "rebin", "name": "delta2theta", "value": 0.005},
                     {"id": "sum", "name": "binsize", "value": 0.002},
                     {"id": "wait", "name": "filename", "value": _FILENAME},
                     {"id": "wait", "name": "entries", "value": []},
                     {"id": "rebin", "name": "outprefix", "value": "id000000"},
                     {"id": "rebin", "name": "primary_outdir", "value": _PROCESSED_DIR},
                     {
                         "id": "convert",
                         "name": "primary_outdir",
                         "value": _PROCESSED_DIR,
                     },
                     {"id": "sum", "name": "primary_outdir", "value": _PROCESSED_DIR},
-                ]
+                ],
+                "convert_destination": os.path.join(
+                    _PROCESSED_DIR,
+                    "workflows",
+                    "rebinsum",
+                    "Blank_0001_w0005_b0002.json",
+                ),
             },
             queue="solo2",
         ),
         mock.call(
-            args=(str(tmpdir / "rebinsum.json"),),
+            args=(_read_workflow(tmpdir / "rebinsum.json"),),
             kwargs={
                 "inputs": [
                     {"id": "rebin", "name": "delta2theta", "value": 0.004},
                     {"id": "sum", "name": "binsize", "value": 0.003},
                     {"id": "wait", "name": "filename", "value": _FILENAME},
                     {"id": "wait", "name": "entries", "value": []},
                     {"id": "rebin", "name": "outprefix", "value": "id000000"},
                     {"id": "rebin", "name": "primary_outdir", "value": _PROCESSED_DIR},
                     {
                         "id": "convert",
                         "name": "primary_outdir",
                         "value": _PROCESSED_DIR,
                     },
                     {"id": "sum", "name": "primary_outdir", "value": _PROCESSED_DIR},
-                ]
+                ],
+                "convert_destination": os.path.join(
+                    _PROCESSED_DIR,
+                    "workflows",
+                    "rebinsum",
+                    "Blank_0001_w0004_b0003.json",
+                ),
             },
             queue="solo2",
         ),
         mock.call(
-            args=(str(tmpdir / "rebinsum.json"),),
+            args=(_read_workflow(tmpdir / "rebinsum.json"),),
             kwargs={
                 "inputs": [
                     {"id": "rebin", "name": "delta2theta", "value": 0.005},
                     {"id": "sum", "name": "binsize", "value": 0.003},
                     {"id": "wait", "name": "filename", "value": _FILENAME},
                     {"id": "wait", "name": "entries", "value": []},
                     {"id": "rebin", "name": "outprefix", "value": "id000000"},
                     {"id": "rebin", "name": "primary_outdir", "value": _PROCESSED_DIR},
                     {
                         "id": "convert",
                         "name": "primary_outdir",
                         "value": _PROCESSED_DIR,
                     },
                     {"id": "sum", "name": "primary_outdir", "value": _PROCESSED_DIR},
-                ]
+                ],
+                "convert_destination": os.path.join(
+                    _PROCESSED_DIR,
+                    "workflows",
+                    "rebinsum",
+                    "Blank_0001_w0005_b0003.json",
+                ),
             },
             queue="solo2",
         ),
     ]
 
     submit_mock.assert_has_calls(calls)
+
+
+def _read_workflow(filename):
+    with open(filename, "r") as f:
+        return json.load(f)
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/tests/test_persistent.py` & `blissoda-0.1.0/src/blissoda/tests/test_persistent.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.0.3rc0/src/blissoda/utils/directories.py` & `blissoda-0.1.0/src/blissoda/utils/directories.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Tuple
 import os
 
 
 def get_dataset_dir(dataset_filename: str) -> str:
     return os.path.dirname(os.path.abspath(dataset_filename))
 
 
@@ -19,24 +20,45 @@
         # version 2
         return _abs_join(dirname, "..")
     # version 1: proposal == raw
     return dirname
 
 
 def get_processed_dir(dataset_filename: str) -> str:
-    dirname = get_raw_dir(dataset_filename)
-    if os.path.basename(dirname) == "RAW_DATA":
-        # version 3
+    version, dirname = get_directory_version(dataset_filename)
+    if version == 3:
         return _abs_join(dirname, "..", "PROCESSED_DATA")
-    if os.path.basename(dirname) == "raw":
-        # version 2
+    if version == 2:
         return _abs_join(dirname, "..", "processed")
-    # version 1: proposal == raw
     return _abs_join(dirname, "processed")
 
 
+def get_workflows_dir(dataset_filename: str) -> str:
+    return os.path.join(get_processed_dir(dataset_filename), "workflows")
+
+
+def get_nobackup_dir(dataset_filename: str) -> str:
+    version, dirname = get_directory_version(dataset_filename)
+    if version == 3:
+        return _abs_join(dirname, "..", "NOBACKUP")
+    if version == 2:
+        return _abs_join(dirname, "..", "_nobackup")
+    return _abs_join(dirname, "_nobackup")
+
+
+def get_directory_version(dataset_filename: str) -> Tuple[int, str]:
+    """Returns directory structure version number and the raw data directory"""
+    dirname = get_raw_dir(dataset_filename)
+    if os.path.basename(dirname) == "RAW_DATA":
+        return 3, dirname
+    if os.path.basename(dirname) == "raw":
+        return 2, dirname
+    # proposal == raw
+    return 1, dirname
+
+
 def get_session_dir(dataset_filename: str) -> str:
     return _abs_join(get_proposal_dir(dataset_filename), "..")
 
 
 def _abs_join(*args):
     return os.path.abspath(os.path.join(*args))
```

### Comparing `blissoda-0.0.3rc0/src/blissoda/utils/pyfai.py` & `blissoda-0.1.0/src/blissoda/utils/pyfai.py`

 * *Files identical despite different names*

### Comparing `blissoda-0.0.3rc0/src/blissoda.egg-info/PKG-INFO` & `blissoda-0.1.0/src/blissoda.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissoda
-Version: 0.0.3rc0
+Version: 0.1.0
 Summary: Utilities for ewoks developers
 Home-page: https://gitlab.esrf.fr/bliss/blissoda/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/bliss/blissoda/
 Project-URL: Documentation, https://blissoda.readthedocs.io/
@@ -13,19 +13,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: submit
 Provides-Extra: server
 Provides-Extra: id22
-Provides-Extra: streamline
-Provides-Extra: bm23
+Provides-Extra: id09
 Provides-Extra: id31
 Provides-Extra: bm02
 Provides-Extra: id11
+Provides-Extra: streamline
+Provides-Extra: bm23
 Provides-Extra: democlient
 Provides-Extra: demoworker
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE.md
```

### Comparing `blissoda-0.0.3rc0/src/blissoda.egg-info/SOURCES.txt` & `blissoda-0.1.0/src/blissoda.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,62 +12,76 @@
 src/blissoda.egg-info/requires.txt
 src/blissoda.egg-info/top_level.txt
 src/blissoda/app/__init__.py
 src/blissoda/app/__main__.py
 src/blissoda/app/cli_log_utils.py
 src/blissoda/app/workflow_server.py
 src/blissoda/bm02/__init__.py
-src/blissoda/bm02/xrpd_plotter.py
+src/blissoda/bm02/xrpd_processor.py
 src/blissoda/bm23/__init__.py
 src/blissoda/bm23/exafs_plotter.py
 src/blissoda/demo/__init__.py
-src/blissoda/demo/exafs_plotter.py
+src/blissoda/demo/exafs.py
 src/blissoda/demo/example.py
-src/blissoda/demo/id11.py
-src/blissoda/demo/streamline_scanner.py
-src/blissoda/demo/stscan_processor.py
-src/blissoda/demo/xrpd_plotter.py
-src/blissoda/demo/xrpd_processor.py
+src/blissoda/demo/id22.py
+src/blissoda/demo/streamline.py
+src/blissoda/demo/xrpd.py
 src/blissoda/demo/user_scripts/__init__.py
-src/blissoda/demo/user_scripts/bm02.py
-src/blissoda/demo/user_scripts/bm23.py
-src/blissoda/demo/user_scripts/id11.py
+src/blissoda/demo/user_scripts/all.py
+src/blissoda/demo/user_scripts/exafs.py
 src/blissoda/demo/user_scripts/id22.py
-src/blissoda/demo/user_scripts/id31.py
 src/blissoda/demo/user_scripts/streamline.py
-src/blissoda/exafs_plotting/__init__.py
-src/blissoda/exafs_plotting/exafs_plots.py
-src/blissoda/exafs_plotting/exafs_plotter.py
-src/blissoda/exafs_plotting/exafs_plotter_old.py
-src/blissoda/exafs_plotting/exafs_widgets.py
+src/blissoda/demo/user_scripts/xrpd.py
+src/blissoda/exafs/__init__.py
+src/blissoda/exafs/plots.py
+src/blissoda/exafs/plotter.py
+src/blissoda/exafs/widgets.py
+src/blissoda/flint/__init__.py
+src/blissoda/id09/__init__.py
+src/blissoda/id09/xrpd_processor.py
 src/blissoda/id11/__init__.py
 src/blissoda/id11/xrpd_processor.py
 src/blissoda/id22/__init__.py
 src/blissoda/id22/stscan_processor.py
+src/blissoda/id22/xrpd_processor.py
 src/blissoda/id31/__init__.py
+src/blissoda/id31/optimize_exposure.py
 src/blissoda/id31/streamline_scanner.py
 src/blissoda/id31/xrpd_processor.py
+src/blissoda/id31/xrpd_processor_old.py
 src/blissoda/resources/__init__.py
-src/blissoda/resources/bm23/__init__.py
-src/blissoda/resources/bm23/bm23.ows
 src/blissoda/resources/demo/__init__.py
-src/blissoda/resources/id11/__init__.py
-src/blissoda/resources/id11/integrate_scan.ows
+src/blissoda/resources/exafs/__init__.py
+src/blissoda/resources/exafs/exafs.ows
 src/blissoda/resources/streamline/__init__.py
 src/blissoda/resources/streamline/reprocess.py
-src/blissoda/resources/streamline/streamline_with_calib.ows
-src/blissoda/resources/streamline/streamline_without_calib.ows
+src/blissoda/resources/streamline/streamline_with_calib.json
+src/blissoda/resources/streamline/streamline_without_calib.json
 src/blissoda/resources/streamline/time_record.py
+src/blissoda/resources/xrpd/__init__.py
+src/blissoda/resources/xrpd/integrate_scan_with_saving.json
+src/blissoda/resources/xrpd/integrate_scan_without_saving.json
 src/blissoda/seslab/__init__.py
 src/blissoda/seslab/streamline_scanner.py
 src/blissoda/streamline/__init__.py
-src/blissoda/streamline/streamline_scanner.py
+src/blissoda/streamline/scanner.py
 src/blissoda/tests/__init__.py
 src/blissoda/tests/conftest.py
 src/blissoda/tests/test_id22.py
+src/blissoda/tests/test_id31.py
 src/blissoda/tests/test_persistent.py
+src/blissoda/tests/mock_id31/__init__.py
+src/blissoda/tests/mock_id31/attenuator.py
+src/blissoda/tests/mock_id31/controllers.py
+src/blissoda/tests/mock_id31/lima_image.py
+src/blissoda/tests/mock_id31/setup_globals.py
+src/blissoda/tests/mock_id31/simulate.py
 src/blissoda/utils/__init__.py
 src/blissoda/utils/directories.py
 src/blissoda/utils/info.py
 src/blissoda/utils/pyfai.py
-src/blissoda/xrpd_plotter/__init__.py
-src/blissoda/xrpd_plotter/xrpd_plotter.py
+src/blissoda/xrpd/__init__.py
+src/blissoda/xrpd/data.py
+src/blissoda/xrpd/plots.py
+src/blissoda/xrpd/plotter.py
+src/blissoda/xrpd/processor.py
+src/blissoda/xrpd/widgets.py
```

### Comparing `blissoda-0.0.3rc0/src/blissoda.egg-info/requires.txt` & `blissoda-0.1.0/src/blissoda.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,82 @@
 
 [bm02]
 ewoksjob
+silx>=1.1.0
+blissdata>=0.2.5
 
 [bm23]
 ewoksjob
 silx>=1.1.0
 
 [democlient]
 ewoksjob
 
 [demoworker]
 ewoksjob
-blissdata
-ewoksjob[blissworker]
-ewoksxrpd>=0.2
+blissdata>=0.2.5
+ewoksjob[blissworker]>=0.2.1
+ewoksxrpd>=0.3
 est[full]
 orange3
 
 [dev]
 pytest>=7
 mock
 pytest-mock
 ewoksjob
-silx
-streamline_changer@ git+https://gitlab.esrf.fr/bliss/streamline_changer.git
+blissdata>=0.2.5
 silx>=1.1.0
-ewoks
-blissdata
+streamline_changer@ git+https://gitlab.esrf.fr/bliss/streamline_changer.git
 black>=22
 flake8>=4
 
 [doc]
 pytest>=7
 mock
 pytest-mock
 ewoksjob
-silx
-streamline_changer@ git+https://gitlab.esrf.fr/bliss/streamline_changer.git
+blissdata>=0.2.5
 silx>=1.1.0
-ewoks
-blissdata
+streamline_changer@ git+https://gitlab.esrf.fr/bliss/streamline_changer.git
 sphinx>=4.5
 sphinx-autodoc-typehints>=1.16
 
+[id09]
+ewoksjob
+silx>=1.1.0
+blissdata>=0.2.5
+
 [id11]
 ewoksjob
+silx>=1.1.0
+blissdata>=0.2.5
 
 [id22]
 ewoksjob
+silx>=1.1.0
+blissdata>=0.2.5
 
 [id31]
 ewoksjob
-ewoks
+silx>=1.1.0
+blissdata>=0.2.5
 
 [server]
 ewoksjob
-blissdata
+blissdata>=0.2.5
 
 [streamline]
 ewoksjob
-silx
 streamline_changer@ git+https://gitlab.esrf.fr/bliss/streamline_changer.git
 
 [submit]
 ewoksjob
 
 [test]
 pytest>=7
 mock
 pytest-mock
 ewoksjob
-silx
-streamline_changer@ git+https://gitlab.esrf.fr/bliss/streamline_changer.git
+blissdata>=0.2.5
 silx>=1.1.0
-ewoks
-blissdata
+streamline_changer@ git+https://gitlab.esrf.fr/bliss/streamline_changer.git
```

