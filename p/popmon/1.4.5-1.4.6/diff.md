# Comparing `tmp/popmon-1.4.5.tar.gz` & `tmp/popmon-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popmon-1.4.5.tar", last modified: Thu Jul  6 14:54:25 2023, max compression
+gzip compressed data, was "popmon-1.4.6.tar", last modified: Tue Jul 18 10:21:18 2023, max compression
```

## Comparing `popmon-1.4.5.tar` & `popmon-1.4.6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.011726 popmon-1.4.5/
--rw-r--r--   0 root         (0) root         (0)     1071 2023-07-06 14:54:14.000000 popmon-1.4.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       75 2023-07-06 14:54:14.000000 popmon-1.4.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3792 2023-07-06 14:54:14.000000 popmon-1.4.5/NOTICE
--rw-r--r--   0 root         (0) root         (0)    23345 2023-07-06 14:54:25.011726 popmon-1.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21523 2023-07-06 14:54:14.000000 popmon-1.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.987726 popmon-1.4.5/popmon/
--rw-r--r--   0 root         (0) root         (0)     1893 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.987726 popmon-1.4.5/popmon/alerting/
--rw-r--r--   0 root         (0) root         (0)     1627 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/alerting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4219 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/alerting/alerts_summary.py
--rw-r--r--   0 root         (0) root         (0)    18853 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/alerting/compute_tl_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.991726 popmon-1.4.5/popmon/analysis/
--rw-r--r--   0 root         (0) root         (0)     1280 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13919 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/apply_func.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.991726 popmon-1.4.5/popmon/analysis/comparison/
--rw-r--r--   0 root         (0) root         (0)     1589 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/comparison/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8823 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/comparison/comparisons.py
--rw-r--r--   0 root         (0) root         (0)    15744 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/comparison/hist_comparer.py
--rw-r--r--   0 root         (0) root         (0)    19472 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/functions.py
--rw-r--r--   0 root         (0) root         (0)    18777 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/hist_numpy.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/merge_statistics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.991726 popmon-1.4.5/popmon/analysis/profiling/
--rw-r--r--   0 root         (0) root         (0)     1490 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/profiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8254 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/profiling/hist_profiler.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/profiling/profiles.py
--rw-r--r--   0 root         (0) root         (0)    11482 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/profiling/pull_calculator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.991726 popmon-1.4.5/popmon/base/
--rw-r--r--   0 root         (0) root         (0)     1224 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7096 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/base/module.py
--rw-r--r--   0 root         (0) root         (0)     3018 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/base/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     4833 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/base/registry.py
--rw-r--r--   0 root         (0) root         (0)    14549 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/decorators/
--rw-r--r--   0 root         (0) root         (0)     1215 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/decorators/pandas.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/decorators/spark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/extensions/
--rw-r--r--   0 root         (0) root         (0)     1190 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/extensions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/extensions/extension.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/extensions/profile_diptest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/hist/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/hist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/hist/filling/
--rw-r--r--   0 root         (0) root         (0)     1745 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/hist/filling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6638 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/hist/hist_splitter.py
--rw-r--r--   0 root         (0) root         (0)    10961 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/hist/hist_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/io/
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/io/file_reader.py
--rw-r--r--   0 root         (0) root         (0)     3301 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/io/file_writer.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/io/json_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/notebooks/
--rw-r--r--   0 root         (0) root         (0)    19461 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/notebooks/popmon_tutorial_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)     5777 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/notebooks/popmon_tutorial_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    11902 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/notebooks/popmon_tutorial_incremental_data.ipynb
--rw-r--r--   0 root         (0) root         (0)    11762 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/notebooks/popmon_tutorial_reports.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.999726 popmon-1.4.5/popmon/pipeline/
--rw-r--r--   0 root         (0) root         (0)     1108 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2425 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/amazing_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     5208 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/dataset_splitter.py
--rw-r--r--   0 root         (0) root         (0)     7116 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/metrics.py
--rw-r--r--   0 root         (0) root         (0)    16532 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/metrics_pipelines.py
--rw-r--r--   0 root         (0) root         (0)    11282 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/report.py
--rw-r--r--   0 root         (0) root         (0)     9162 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/report_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/timing.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.999726 popmon-1.4.5/popmon/stats/
--rw-r--r--   0 root         (0) root         (0)     1218 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/stats/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11243 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/stats/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.999726 popmon-1.4.5/popmon/stitching/
--rw-r--r--   0 root         (0) root         (0)     1234 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/stitching/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20246 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/stitching/hist_stitcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.003726 popmon-1.4.5/popmon/test_data/
--rw-r--r--   0 root         (0) root         (0)    73043 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/data_generator_hists.json.gz
--rw-r--r--   0 root         (0) root         (0)      128 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/example.json
--rw-r--r--   0 root         (0) root         (0)    15152 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/example_histogram.json
--rw-r--r--   0 root         (0) root         (0)   696816 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/flight_delays.csv.gz
--rw-r--r--   0 root         (0) root         (0)   692782 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/flight_delays_reference.csv.gz
--rw-r--r--   0 root         (0) root         (0)    79082 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/synthetic_histograms.json
--rw-r--r--   0 root         (0) root         (0)    64368 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/test.csv.gz
--rw-r--r--   0 root         (0) root         (0)     2712 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/utils.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-07-06 14:54:15.000000 popmon-1.4.5/popmon/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.003726 popmon-1.4.5/popmon/visualization/
--rw-r--r--   0 root         (0) root         (0)     1645 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6321 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/alert_section_generator.py
--rw-r--r--   0 root         (0) root         (0)    15385 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/histogram_section.py
--rw-r--r--   0 root         (0) root         (0)     8532 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/overview_section.py
--rw-r--r--   0 root         (0) root         (0)     3094 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/report_generator.py
--rw-r--r--   0 root         (0) root         (0)    10860 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/section_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.007726 popmon-1.4.5/popmon/visualization/templates/
--rw-r--r--   0 root         (0) root         (0)      835 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/aggregated-overview.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.983726 popmon-1.4.5/popmon/visualization/templates/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.007726 popmon-1.4.5/popmon/visualization/templates/assets/css/
--rw-r--r--   0 root         (0) root         (0)   155712 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)     2090 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/css/custom-style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.011726 popmon-1.4.5/popmon/visualization/templates/assets/js/
--rw-r--r--   0 root         (0) root         (0)    78586 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)     2943 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/custom-script.js
--rwxr-xr-x   0 root         (0) root         (0)     2532 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/jquery.easing.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)  3682474 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/plotly.js
--rw-r--r--   0 root         (0) root         (0)      927 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/scrolling-nav.js
--rw-r--r--   0 root         (0) root         (0)     2482 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/card.html
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/core.html
--rw-r--r--   0 root         (0) root         (0)      941 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/footer.html
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/header.html
--rw-r--r--   0 root         (0) root         (0)      988 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/modal-popup.html
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/notebook_iframe.html
--rw-r--r--   0 root         (0) root         (0)     2753 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/section.html
--rw-r--r--   0 root         (0) root         (0)     1401 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/table.html
--rw-r--r--   0 root         (0) root         (0)     7317 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/traffic_light_section_generator.py
--rw-r--r--   0 root         (0) root         (0)    26880 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.987726 popmon-1.4.5/popmon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23345 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3410 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      289 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5119 2023-07-06 14:54:14.000000 popmon-1.4.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      144 2023-07-06 14:54:14.000000 popmon-1.4.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 14:54:25.011726 popmon-1.4.5/setup.cfg
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.288368 popmon-1.4.6/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1071 2023-05-25 15:53:00.000000 popmon-1.4.6/LICENSE
+-rw-r--r--   0 AF57BI     (503) staff       (20)       75 2022-09-09 09:01:39.000000 popmon-1.4.6/MANIFEST.in
+-rw-r--r--   0 AF57BI     (503) staff       (20)     3792 2022-09-09 09:01:39.000000 popmon-1.4.6/NOTICE
+-rw-r--r--   0 AF57BI     (503) staff       (20)    23345 2023-07-18 10:21:18.287776 popmon-1.4.6/PKG-INFO
+-rw-r--r--   0 AF57BI     (503) staff       (20)    21523 2023-05-25 15:53:00.000000 popmon-1.4.6/README.rst
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.043680 popmon-1.4.6/popmon/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1893 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/__init__.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.064459 popmon-1.4.6/popmon/alerting/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1627 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/alerting/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     4219 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/alerting/alerts_summary.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    18853 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/alerting/compute_tl_bounds.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.082950 popmon-1.4.6/popmon/analysis/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1280 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/analysis/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    13919 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/analysis/apply_func.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.090415 popmon-1.4.6/popmon/analysis/comparison/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1589 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/analysis/comparison/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     8823 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/analysis/comparison/comparisons.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    15744 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/analysis/comparison/hist_comparer.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    19472 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/analysis/functions.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    18303 2023-07-18 10:11:39.000000 popmon-1.4.6/popmon/analysis/hist_numpy.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     2492 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/analysis/merge_statistics.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.095414 popmon-1.4.6/popmon/analysis/profiling/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1490 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/analysis/profiling/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     8254 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/analysis/profiling/hist_profiler.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     6805 2023-07-06 13:52:44.000000 popmon-1.4.6/popmon/analysis/profiling/profiles.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    11482 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/analysis/profiling/pull_calculator.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.098056 popmon-1.4.6/popmon/base/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1224 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/base/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     7096 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/base/module.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     3018 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/base/pipeline.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     4833 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/base/registry.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    14549 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/config.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.106230 popmon-1.4.6/popmon/decorators/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1215 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/decorators/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1689 2023-07-06 13:52:44.000000 popmon-1.4.6/popmon/decorators/pandas.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1728 2023-07-06 13:52:44.000000 popmon-1.4.6/popmon/decorators/spark.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.109988 popmon-1.4.6/popmon/extensions/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1190 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/extensions/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1229 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/extensions/extension.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     2456 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/extensions/profile_diptest.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.120753 popmon-1.4.6/popmon/hist/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1189 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/hist/__init__.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.125570 popmon-1.4.6/popmon/hist/filling/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1745 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/hist/filling/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     6638 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/hist/hist_splitter.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    10961 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/hist/hist_utils.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.137574 popmon-1.4.6/popmon/io/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1299 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/io/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     2940 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/io/file_reader.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     3301 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/io/file_writer.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1729 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/io/json_reader.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.176997 popmon-1.4.6/popmon/notebooks/
+-rw-r--r--   0 AF57BI     (503) staff       (20)    19461 2022-10-19 14:09:16.000000 popmon-1.4.6/popmon/notebooks/popmon_tutorial_advanced.ipynb
+-rw-r--r--   0 AF57BI     (503) staff       (20)     5777 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/notebooks/popmon_tutorial_basic.ipynb
+-rw-r--r--   0 AF57BI     (503) staff       (20)    11902 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/notebooks/popmon_tutorial_incremental_data.ipynb
+-rw-r--r--   0 AF57BI     (503) staff       (20)    11762 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/notebooks/popmon_tutorial_reports.ipynb
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.210782 popmon-1.4.6/popmon/pipeline/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1108 2023-05-25 15:53:00.000000 popmon-1.4.6/popmon/pipeline/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     2425 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/pipeline/amazing_pipeline.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     5208 2023-07-06 13:41:43.000000 popmon-1.4.6/popmon/pipeline/dataset_splitter.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     7116 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/pipeline/metrics.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    16532 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/pipeline/metrics_pipelines.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    11282 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/pipeline/report.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     9162 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/pipeline/report_pipelines.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1760 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/pipeline/timing.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     4530 2023-07-18 10:11:39.000000 popmon-1.4.6/popmon/resources.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.211794 popmon-1.4.6/popmon/stats/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1218 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/stats/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    11243 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/stats/numpy.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.215286 popmon-1.4.6/popmon/stitching/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1234 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/stitching/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    20246 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/stitching/hist_stitcher.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.249846 popmon-1.4.6/popmon/test_data/
+-rw-r--r--   0 AF57BI     (503) staff       (20)    73043 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/test_data/data_generator_hists.json.gz
+-rw-r--r--   0 AF57BI     (503) staff       (20)      128 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/test_data/example.json
+-rw-r--r--   0 AF57BI     (503) staff       (20)    15152 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/test_data/example_histogram.json
+-rw-r--r--   0 AF57BI     (503) staff       (20)   696816 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/test_data/flight_delays.csv.gz
+-rw-r--r--   0 AF57BI     (503) staff       (20)   692782 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/test_data/flight_delays_reference.csv.gz
+-rw-r--r--   0 AF57BI     (503) staff       (20)    79082 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/test_data/synthetic_histograms.json
+-rw-r--r--   0 AF57BI     (503) staff       (20)    64368 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/test_data/test.csv.gz
+-rw-r--r--   0 AF57BI     (503) staff       (20)     2712 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/utils.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1127 2023-07-18 10:21:00.000000 popmon-1.4.6/popmon/version.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.269459 popmon-1.4.6/popmon/visualization/
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1645 2023-07-06 13:51:42.000000 popmon-1.4.6/popmon/visualization/__init__.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     6321 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/visualization/alert_section_generator.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    15249 2023-07-18 10:11:39.000000 popmon-1.4.6/popmon/visualization/histogram_section.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     8532 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/visualization/overview_section.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)     3094 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/visualization/report_generator.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    10860 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/visualization/section_generator.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.276509 popmon-1.4.6/popmon/visualization/templates/
+-rw-r--r--   0 AF57BI     (503) staff       (20)      835 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/aggregated-overview.html
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.021234 popmon-1.4.6/popmon/visualization/templates/assets/
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.277609 popmon-1.4.6/popmon/visualization/templates/assets/css/
+-rw-r--r--   0 AF57BI     (503) staff       (20)   155712 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/assets/css/bootstrap.min.css
+-rw-r--r--   0 AF57BI     (503) staff       (20)     2090 2022-10-19 14:00:27.000000 popmon-1.4.6/popmon/visualization/templates/assets/css/custom-style.css
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.287205 popmon-1.4.6/popmon/visualization/templates/assets/js/
+-rw-r--r--   0 AF57BI     (503) staff       (20)    78586 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js
+-rw-r--r--   0 AF57BI     (503) staff       (20)     2943 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/assets/js/custom-script.js
+-rwxr-xr-x   0 AF57BI     (503) staff       (20)     2532 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/assets/js/jquery.easing.min.js
+-rw-r--r--   0 AF57BI     (503) staff       (20)    88145 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/assets/js/jquery.min.js
+-rw-r--r--   0 AF57BI     (503) staff       (20)  3682474 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/assets/js/plotly.js
+-rw-r--r--   0 AF57BI     (503) staff       (20)      927 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/assets/js/scrolling-nav.js
+-rw-r--r--   0 AF57BI     (503) staff       (20)     2482 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/visualization/templates/card.html
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1010 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/visualization/templates/core.html
+-rw-r--r--   0 AF57BI     (503) staff       (20)      941 2023-05-25 15:53:00.000000 popmon-1.4.6/popmon/visualization/templates/footer.html
+-rw-r--r--   0 AF57BI     (503) staff       (20)      782 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/header.html
+-rw-r--r--   0 AF57BI     (503) staff       (20)      988 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/modal-popup.html
+-rw-r--r--   0 AF57BI     (503) staff       (20)      178 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/notebook_iframe.html
+-rw-r--r--   0 AF57BI     (503) staff       (20)     2753 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/visualization/templates/section.html
+-rw-r--r--   0 AF57BI     (503) staff       (20)     1401 2022-09-09 09:01:39.000000 popmon-1.4.6/popmon/visualization/templates/table.html
+-rw-r--r--   0 AF57BI     (503) staff       (20)     7317 2023-07-06 14:57:08.000000 popmon-1.4.6/popmon/visualization/traffic_light_section_generator.py
+-rw-r--r--   0 AF57BI     (503) staff       (20)    26846 2023-07-18 10:11:39.000000 popmon-1.4.6/popmon/visualization/utils.py
+drwxr-xr-x   0 AF57BI     (503) staff       (20)        0 2023-07-18 10:21:18.059937 popmon-1.4.6/popmon.egg-info/
+-rw-r--r--   0 AF57BI     (503) staff       (20)    23345 2023-07-18 10:21:17.000000 popmon-1.4.6/popmon.egg-info/PKG-INFO
+-rw-r--r--   0 AF57BI     (503) staff       (20)     3410 2023-07-18 10:21:17.000000 popmon-1.4.6/popmon.egg-info/SOURCES.txt
+-rw-r--r--   0 AF57BI     (503) staff       (20)        1 2023-07-18 10:21:17.000000 popmon-1.4.6/popmon.egg-info/dependency_links.txt
+-rw-r--r--   0 AF57BI     (503) staff       (20)       68 2023-07-18 10:21:17.000000 popmon-1.4.6/popmon.egg-info/entry_points.txt
+-rw-r--r--   0 AF57BI     (503) staff       (20)      289 2023-07-18 10:21:17.000000 popmon-1.4.6/popmon.egg-info/requires.txt
+-rw-r--r--   0 AF57BI     (503) staff       (20)        7 2023-07-18 10:21:17.000000 popmon-1.4.6/popmon.egg-info/top_level.txt
+-rw-r--r--   0 AF57BI     (503) staff       (20)     5180 2023-07-18 10:11:39.000000 popmon-1.4.6/pyproject.toml
+-rw-r--r--   0 AF57BI     (503) staff       (20)      144 2023-02-15 17:18:57.000000 popmon-1.4.6/requirements.txt
+-rw-r--r--   0 AF57BI     (503) staff       (20)       38 2023-07-18 10:21:18.288456 popmon-1.4.6/setup.cfg
```

### Comparing `popmon-1.4.5/LICENSE` & `popmon-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/NOTICE` & `popmon-1.4.6/NOTICE`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/PKG-INFO` & `popmon-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popmon
-Version: 1.4.5
+Version: 1.4.6
 Summary: Monitor the stability of a pandas or spark dataset
 Author-email: ING Analytics Wholesale Banking <wbaa@ing.com>
 License: Copyright 2023 ING Analytics Wholesale Banking
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without restriction, including without limitation
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
```

### Comparing `popmon-1.4.5/README.rst` & `popmon-1.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/__init__.py` & `popmon-1.4.6/popmon/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/alerting/__init__.py` & `popmon-1.4.6/popmon/alerting/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/alerting/alerts_summary.py` & `popmon-1.4.6/popmon/alerting/alerts_summary.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/alerting/compute_tl_bounds.py` & `popmon-1.4.6/popmon/alerting/compute_tl_bounds.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/__init__.py` & `popmon-1.4.6/popmon/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/apply_func.py` & `popmon-1.4.6/popmon/analysis/apply_func.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/comparison/__init__.py` & `popmon-1.4.6/popmon/analysis/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/comparison/comparisons.py` & `popmon-1.4.6/popmon/analysis/comparison/comparisons.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/comparison/hist_comparer.py` & `popmon-1.4.6/popmon/analysis/comparison/hist_comparer.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/functions.py` & `popmon-1.4.6/popmon/analysis/functions.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/hist_numpy.py` & `popmon-1.4.6/popmon/analysis/hist_numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -378,19 +378,15 @@
     :param bool check_type: if true, also check type consistency of histograms (besides n-dim and datatype).
     :return: bool indicating if lists are similar
     """
     if len(hist_list) < 1:
         return True
     for hist in hist_list:
         if not isinstance(hist, assert_type):
-            raise TypeError(
-                "Input histogram type {htype} not of {htypes}.".format(
-                    htype=type(hist), htypes=assert_type
-                )
-            )
+            raise TypeError(f"Input histogram type {type(hist)} not of {assert_type}.")
     # perform similarity checks on:
     # - number of dimensions
     # - histogram type
     # - datatypes
     # - Bin attributes
     # - SparselyBin attributes
     # - all above for sub-histograms in case of n-dim > 1
@@ -407,64 +403,50 @@
     # Check generic attributes
     if check_type:
         # E.g. histogrammar.specialized.CategorizeHistogramMethods and
         # histogrammar.primitives.categorize.Categorize are both of type hg.Categorize
         # Make this consistent first.
         types = [get_contentType(hist) for hist in hist_list]
         if types.count(types[0]) != len(types):
-            warnings.warn(
-                "Input histograms have inconsistent class types: {types}".format(
-                    types=types
-                )
-            )
+            warnings.warn(f"Input histograms have inconsistent class types: {types}")
             return False
 
     # Check Bin attributes
     if isinstance(hist_list[0], histogrammar.Bin):
         nums = [hist.num for hist in hist_list]
         if nums.count(nums[0]) != len(nums):
             warnings.warn(
-                "Input Bin histograms have inconsistent num attributes: {types}".format(
-                    types=nums
-                )
+                f"Input Bin histograms have inconsistent num attributes: {nums}"
             )
             return False
         lows = [hist.low for hist in hist_list]
         if lows.count(lows[0]) != len(lows):
             warnings.warn(
-                "Input Bin histograms have inconsistent low attributes: {types}".format(
-                    types=lows
-                )
+                f"Input Bin histograms have inconsistent low attributes: {lows}"
             )
             return False
         highs = [hist.high for hist in hist_list]
         if highs.count(highs[0]) != len(highs):
             warnings.warn(
-                "Input histograms have inconsistent high attributes: {types}".format(
-                    types=highs
-                )
+                f"Input histograms have inconsistent high attributes: {highs}"
             )
             return False
 
     # Check SparselyBin attributes
     if isinstance(hist_list[0], histogrammar.SparselyBin):
         origins = [hist.origin for hist in hist_list]
         if origins.count(origins[0]) != len(origins):
             warnings.warn(
-                "Input SparselyBin histograms have inconsistent origin attributes: {types}".format(
-                    types=origins
-                )
+                f"Input SparselyBin histograms have inconsistent origin attributes: {origins}"
             )
             return False
         bws = [hist.binWidth for hist in hist_list]
         if bws.count(bws[0]) != len(bws):
             warnings.warn(
-                "Input SparselyBin histograms have inconsistent binWidth attributes: {types}".format(
-                    types=bws
-                )
+                f"Input SparselyBin histograms have inconsistent binWidth attributes: {bws}"
             )
             return False
 
     # Check sub-histogram attributes
     if n_d[0] > 1:
         sub_hist_list = []
         # Categorize and SparselyBin
```

### Comparing `popmon-1.4.5/popmon/analysis/merge_statistics.py` & `popmon-1.4.6/popmon/analysis/merge_statistics.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/profiling/__init__.py` & `popmon-1.4.6/popmon/analysis/profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/profiling/hist_profiler.py` & `popmon-1.4.6/popmon/analysis/profiling/hist_profiler.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/profiling/profiles.py` & `popmon-1.4.6/popmon/analysis/profiling/profiles.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/analysis/profiling/pull_calculator.py` & `popmon-1.4.6/popmon/analysis/profiling/pull_calculator.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/base/__init__.py` & `popmon-1.4.6/popmon/base/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/base/module.py` & `popmon-1.4.6/popmon/base/module.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/base/pipeline.py` & `popmon-1.4.6/popmon/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/base/registry.py` & `popmon-1.4.6/popmon/base/registry.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/config.py` & `popmon-1.4.6/popmon/config.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/decorators/__init__.py` & `popmon-1.4.6/popmon/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/decorators/pandas.py` & `popmon-1.4.6/popmon/decorators/pandas.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/decorators/spark.py` & `popmon-1.4.6/popmon/decorators/spark.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/extensions/__init__.py` & `popmon-1.4.6/popmon/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/extensions/extension.py` & `popmon-1.4.6/popmon/extensions/extension.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/extensions/profile_diptest.py` & `popmon-1.4.6/popmon/extensions/profile_diptest.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/hist/__init__.py` & `popmon-1.4.6/popmon/hist/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/hist/filling/__init__.py` & `popmon-1.4.6/popmon/hist/filling/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/hist/hist_splitter.py` & `popmon-1.4.6/popmon/hist/hist_splitter.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/hist/hist_utils.py` & `popmon-1.4.6/popmon/hist/hist_utils.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/io/__init__.py` & `popmon-1.4.6/popmon/io/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/io/file_reader.py` & `popmon-1.4.6/popmon/io/file_reader.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/io/file_writer.py` & `popmon-1.4.6/popmon/io/file_writer.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/io/json_reader.py` & `popmon-1.4.6/popmon/io/json_reader.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/notebooks/popmon_tutorial_advanced.ipynb` & `popmon-1.4.6/popmon/notebooks/popmon_tutorial_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/notebooks/popmon_tutorial_basic.ipynb` & `popmon-1.4.6/popmon/notebooks/popmon_tutorial_basic.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/notebooks/popmon_tutorial_incremental_data.ipynb` & `popmon-1.4.6/popmon/notebooks/popmon_tutorial_incremental_data.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/notebooks/popmon_tutorial_reports.ipynb` & `popmon-1.4.6/popmon/notebooks/popmon_tutorial_reports.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/pipeline/__init__.py` & `popmon-1.4.6/popmon/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/pipeline/amazing_pipeline.py` & `popmon-1.4.6/popmon/pipeline/amazing_pipeline.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/pipeline/dataset_splitter.py` & `popmon-1.4.6/popmon/pipeline/dataset_splitter.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/pipeline/metrics.py` & `popmon-1.4.6/popmon/pipeline/metrics.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/pipeline/metrics_pipelines.py` & `popmon-1.4.6/popmon/pipeline/metrics_pipelines.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/pipeline/report.py` & `popmon-1.4.6/popmon/pipeline/report.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/pipeline/report_pipelines.py` & `popmon-1.4.6/popmon/pipeline/report_pipelines.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/pipeline/timing.py` & `popmon-1.4.6/popmon/pipeline/timing.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/resources.py` & `popmon-1.4.6/popmon/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,17 +90,15 @@
     """
     full_path = _RESOURCES[resource_type].get(name, None)
 
     if full_path and full_path.exists():
         return str(full_path)
 
     raise FileNotFoundError(
-        'Could not find {resource_type} "{name!s}"! Does it exist?'.format(
-            resource_type=resource_type, name=name
-        )
+        f'Could not find {resource_type} "{name!s}"! Does it exist?'
     )
 
 
 def data(name: str) -> str:
     """Return the full path filename of a shipped data file.
 
     :param str name: The name of the data.
```

### Comparing `popmon-1.4.5/popmon/stats/__init__.py` & `popmon-1.4.6/popmon/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/stats/numpy.py` & `popmon-1.4.6/popmon/stats/numpy.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/stitching/__init__.py` & `popmon-1.4.6/popmon/stitching/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/stitching/hist_stitcher.py` & `popmon-1.4.6/popmon/stitching/hist_stitcher.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/test_data/data_generator_hists.json.gz` & `popmon-1.4.6/popmon/test_data/data_generator_hists.json.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/test_data/example_histogram.json` & `popmon-1.4.6/popmon/test_data/example_histogram.json`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/test_data/flight_delays.csv.gz` & `popmon-1.4.6/popmon/test_data/flight_delays.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/test_data/flight_delays_reference.csv.gz` & `popmon-1.4.6/popmon/test_data/flight_delays_reference.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/test_data/synthetic_histograms.json` & `popmon-1.4.6/popmon/test_data/synthetic_histograms.json`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/test_data/test.csv.gz` & `popmon-1.4.6/popmon/test_data/test.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/utils.py` & `popmon-1.4.6/popmon/utils.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/version.py` & `popmon-1.4.6/popmon/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-version = "1.4.5"
+version = "1.4.6"
```

### Comparing `popmon-1.4.5/popmon/visualization/__init__.py` & `popmon-1.4.6/popmon/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/alert_section_generator.py` & `popmon-1.4.6/popmon/visualization/alert_section_generator.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/histogram_section.py` & `popmon-1.4.6/popmon/visualization/histogram_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                 ]
             if len(hist_names) == 0:
                 self.logger.debug(
                     f"for feature {feature} no histograms found. skipping."
                 )
                 continue
 
-            # base64 heatmap plot for each metric
+            # heatmap plot for each metric
             dates = [short_date(date) for date in df.index[:]]
             hists = [
                 df[hist_names].iloc[-i].values
                 for i in reversed(range(1, len(dates) + 1))
             ]
 
             # compute heatmaps
@@ -229,22 +229,22 @@
         )
     # filter out Nones (e.g. can happen with empty rolling hist)
     none_hists = [i for i, hc in enumerate(hc_list) if hc is None]
     hc_list = [hc for i, hc in enumerate(hc_list) if i not in none_hists]
     hist_names = [hn for i, hn in enumerate(hist_names) if i not in none_hists]
     # more basic checks
     if len(hc_list) == 0:
-        return {"name": date, "description": "", "plot": ""}
+        return {}
     assert_similar_hists(hc_list)
 
     # make plot. note: slow!
     if hc_list[0].n_dim == 1:
         if all(h.entries == 0 for h in hc_list):
             # triviality checks, skip all histograms empty
-            return {"name": date, "description": "", "plot": ""}
+            return {}
 
         props = get_hist_props(hc_list[0])
         is_num = props["is_num"]
         is_ts = props["is_ts"]
         y_label = "Bin count" if len(hc_list) == 1 else "Bin probability"
 
         if is_num:
@@ -255,15 +255,15 @@
             # categorical
             entries_list, bins = get_consistent_numpy_entries(
                 hc_list, get_bin_labels=True
             )  # bins = bin-labels
 
         # skip histograms with too many bins to plot (default more than 1000)
         if len(bins) > max_nbins:
-            return {"name": date, "description": "", "plot": ""}
+            return {}
 
         # normalize histograms for plotting (comparison!) in case there is more than one.
         if len(hc_list) >= 2:
             entries_list = [
                 el / hc.entries if hc.entries > 0 else el
                 for el, hc in zip(entries_list, hc_list)
             ]
```

### Comparing `popmon-1.4.5/popmon/visualization/overview_section.py` & `popmon-1.4.6/popmon/visualization/overview_section.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/report_generator.py` & `popmon-1.4.6/popmon/visualization/report_generator.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/section_generator.py` & `popmon-1.4.6/popmon/visualization/section_generator.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/aggregated-overview.html` & `popmon-1.4.6/popmon/visualization/templates/aggregated-overview.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/assets/css/bootstrap.min.css` & `popmon-1.4.6/popmon/visualization/templates/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/assets/css/custom-style.css` & `popmon-1.4.6/popmon/visualization/templates/assets/css/custom-style.css`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js` & `popmon-1.4.6/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/assets/js/custom-script.js` & `popmon-1.4.6/popmon/visualization/templates/assets/js/custom-script.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/assets/js/jquery.easing.min.js` & `popmon-1.4.6/popmon/visualization/templates/assets/js/jquery.easing.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/assets/js/jquery.min.js` & `popmon-1.4.6/popmon/visualization/templates/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/assets/js/plotly.js` & `popmon-1.4.6/popmon/visualization/templates/assets/js/plotly.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/assets/js/scrolling-nav.js` & `popmon-1.4.6/popmon/visualization/templates/assets/js/scrolling-nav.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/card.html` & `popmon-1.4.6/popmon/visualization/templates/card.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/core.html` & `popmon-1.4.6/popmon/visualization/templates/core.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/footer.html` & `popmon-1.4.6/popmon/visualization/templates/footer.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/header.html` & `popmon-1.4.6/popmon/visualization/templates/header.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/modal-popup.html` & `popmon-1.4.6/popmon/visualization/templates/modal-popup.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/section.html` & `popmon-1.4.6/popmon/visualization/templates/section.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/templates/table.html` & `popmon-1.4.6/popmon/visualization/templates/table.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/traffic_light_section_generator.py` & `popmon-1.4.6/popmon/visualization/traffic_light_section_generator.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/popmon/visualization/utils.py` & `popmon-1.4.6/popmon/visualization/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -758,17 +758,15 @@
 
     # plot categories
     else:
         labels = hist_bins
         values = hist_values
         assert len(labels) == len(
             values
-        ), "labels and values have different array lengths: {:d} vs {:d}. {}".format(
-            len(labels), len(values), x_label
-        )
+        ), f"labels and values have different array lengths: {len(labels):d} vs {len(values):d}. {x_label}"
 
         # plot histogram
         fig = px.imshow(
             values,
             labels={"x": "Time Bins", "y": x_label, "color": y_label},
             x=date,
             y=[xtick(lab, top) for lab in labels],
```

### Comparing `popmon-1.4.5/popmon.egg-info/PKG-INFO` & `popmon-1.4.6/popmon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popmon
-Version: 1.4.5
+Version: 1.4.6
 Summary: Monitor the stability of a pandas or spark dataset
 Author-email: ING Analytics Wholesale Banking <wbaa@ing.com>
 License: Copyright 2023 ING Analytics Wholesale Banking
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without restriction, including without limitation
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
```

### Comparing `popmon-1.4.5/popmon.egg-info/SOURCES.txt` & `popmon-1.4.6/popmon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `popmon-1.4.5/pyproject.toml` & `popmon-1.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,16 @@
     "INP001",
 
     # Copyright
     "CPY001",
 ]
 
 "popmon/config.py" = [
-    "RUF012", # Mutable class attributes should be annotated with `typing.ClassVar`
+    "RUF012", # Mutable class attributes should be annotated with `typing.ClassVar`,
+    "FA100", # Missing `from __future__ import annotations`
 ]
 
 # Notebooks & NBQA
 "popmon/notebooks/*" = [
     # Imports cannot be checked properly with NBQA
     # (It splits each cell into a .py file)
     "INP001", "E401", "E402", "F401", "I001",
```

