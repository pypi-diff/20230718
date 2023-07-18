# Comparing `tmp/asreview-1.2.1.tar.gz` & `tmp/asreview-1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asreview-1.2.1.tar", last modified: Tue Jul 18 10:56:53 2023, max compression
+gzip compressed data, was "asreview-1.3a0.tar", last modified: Thu Jun  1 08:05:11 2023, max compression
```

## Comparing `asreview-1.2.1.tar` & `asreview-1.3a0.tar`

### file list

```diff
@@ -1,122 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.620917 asreview-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-07-18 10:54:50.000000 asreview-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-18 10:54:50.000000 asreview-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-18 10:56:53.620917 asreview-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-07-18 10:54:50.000000 asreview-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.620917 asreview-1.2.1/asreview/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-18 10:56:53.620917 asreview-1.2.1/asreview/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.612917 asreview-1.2.1/asreview/data/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/data/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.612917 asreview-1.2.1/asreview/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/entry_points/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/entry_points/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/entry_points/lab.py
--rw-r--r--   0 runner    (1001) docker     (123)    15252 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/entry_points/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/entry_points/state_inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.612917 asreview-1.2.1/asreview/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/io/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/io/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/io/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/io/paper_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/io/ris_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/io/ris_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/io/tsv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.612917 asreview-1.2.1/asreview/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.616917 asreview-1.2.1/asreview/models/balance/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/balance/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/balance/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/balance/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/balance/triple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/balance/undersample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/balance/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.616917 asreview-1.2.1/asreview/models/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/classifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/classifiers/logistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/classifiers/lstm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/classifiers/lstm_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/classifiers/nb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/classifiers/nn_2_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/classifiers/rf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/classifiers/svm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/classifiers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.616917 asreview-1.2.1/asreview/models/feature_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/feature_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/feature_extraction/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/feature_extraction/doc2vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/feature_extraction/embedding_idf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/feature_extraction/embedding_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/feature_extraction/sbert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/feature_extraction/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/feature_extraction/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.616917 asreview-1.2.1/asreview/models/query/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/query/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/query/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/query/mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/query/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/query/uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/models/query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22689 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.616917 asreview-1.2.1/asreview/review/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/review/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/review/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/review/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.616917 asreview-1.2.1/asreview/state/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.620917 asreview-1.2.1/asreview/state/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/legacy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/legacy/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/legacy/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/legacy/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/legacy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/sql_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    42032 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/sqlstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/state/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.620917 asreview-1.2.1/asreview/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/webapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52683 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/webapp/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/webapp/io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/webapp/run_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-18 10:54:50.000000 asreview-1.2.1/asreview/webapp/sqlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-07-18 10:54:51.000000 asreview-1.2.1/asreview/webapp/start_flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.620917 asreview-1.2.1/asreview/webapp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 10:54:51.000000 asreview-1.2.1/asreview/webapp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-18 10:54:51.000000 asreview-1.2.1/asreview/webapp/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-18 10:54:51.000000 asreview-1.2.1/asreview/webapp/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-18 10:54:51.000000 asreview-1.2.1/asreview/webapp/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-18 10:54:51.000000 asreview-1.2.1/asreview/webapp/tests/test_webapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-18 10:54:51.000000 asreview-1.2.1/asreview/webapp/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:56:53.612917 asreview-1.2.1/asreview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-18 10:56:53.000000 asreview-1.2.1/asreview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-18 10:56:53.000000 asreview-1.2.1/asreview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:56:53.000000 asreview-1.2.1/asreview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-18 10:56:53.000000 asreview-1.2.1/asreview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-18 10:56:53.000000 asreview-1.2.1/asreview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 10:56:53.000000 asreview-1.2.1/asreview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-18 10:56:53.620917 asreview-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-07-18 10:54:51.000000 asreview-1.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68612 2023-07-18 10:54:51.000000 asreview-1.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:11.000901 asreview-1.3a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-01 08:03:03.000000 asreview-1.3a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-01 08:03:03.000000 asreview-1.3a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-01 08:05:11.000901 asreview-1.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-01 08:03:03.000000 asreview-1.3a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:11.000901 asreview-1.3a0/asreview/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 08:05:11.000901 asreview-1.3a0/asreview/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.988901 asreview-1.3a0/asreview/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/data/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.988901 asreview-1.3a0/asreview/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/entry_points/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/entry_points/auth_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/entry_points/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/entry_points/lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/entry_points/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/entry_points/state_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.992901 asreview-1.3a0/asreview/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/io/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/io/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/io/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/io/paper_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/io/ris_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/io/ris_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/io/tsv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.992901 asreview-1.3a0/asreview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.992901 asreview-1.3a0/asreview/models/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/balance/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/balance/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/balance/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/balance/triple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/balance/undersample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/balance/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.992901 asreview-1.3a0/asreview/models/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/classifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/classifiers/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/classifiers/lstm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/classifiers/lstm_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/classifiers/nb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/classifiers/nn_2_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/classifiers/rf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/classifiers/svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/classifiers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.992901 asreview-1.3a0/asreview/models/feature_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/feature_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/feature_extraction/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/feature_extraction/doc2vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/feature_extraction/embedding_idf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/feature_extraction/embedding_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/feature_extraction/sbert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/feature_extraction/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/feature_extraction/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.996901 asreview-1.3a0/asreview/models/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/query/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/query/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/query/mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/query/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/query/uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/models/query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.996901 asreview-1.3a0/asreview/review/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/review/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/review/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/review/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.996901 asreview-1.3a0/asreview/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.996901 asreview-1.3a0/asreview/state/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/legacy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/legacy/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/legacy/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/legacy/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/legacy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22144 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/sql_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42551 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/sqlstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/state/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.996901 asreview-1.3a0/asreview/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.996901 asreview-1.3a0/asreview/webapp/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17893 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54904 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/api/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.996901 asreview-1.3a0/asreview/webapp/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/authentication/login_required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/authentication/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/authentication/oauth_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5204 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/run_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/sqlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/start_flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:11.000901 asreview-1.3a0/asreview/webapp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/temp_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/test_asreview_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/test_auth_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29221 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/test_project_api_authenticated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/test_project_api_unauthenticated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/test_webapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-01 08:03:03.000000 asreview-1.3a0/asreview/webapp/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:05:10.988901 asreview-1.3a0/asreview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-01 08:05:10.000000 asreview-1.3a0/asreview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-01 08:05:10.000000 asreview-1.3a0/asreview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:05:10.000000 asreview-1.3a0/asreview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-01 08:05:10.000000 asreview-1.3a0/asreview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-01 08:05:10.000000 asreview-1.3a0/asreview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 08:05:10.000000 asreview-1.3a0/asreview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-01 08:05:11.000901 asreview-1.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-06-01 08:03:03.000000 asreview-1.3a0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68752 2023-06-01 08:03:03.000000 asreview-1.3a0/versioneer.py
```

### Comparing `asreview-1.2.1/LICENSE` & `asreview-1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/PKG-INFO` & `asreview-1.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asreview
-Version: 1.2.1
+Version: 1.3a0
 Summary: ASReview LAB - A tool for AI-assisted systematic reviews
 Home-page: https://github.com/asreview/asreview
 Author: ASReview LAB developers
 Author-email: asreview@uu.nl
 Project-URL: Bug Reports, https://github.com/asreview/asreview/issues
 Project-URL: Source, https://github.com/asreview/asreview/
 Keywords: systematic review,machine-learning
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: General
 Classifier: Framework :: Flask
-Requires-Python: ~=3.8
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: sbert
 Provides-Extra: doc2vec
 Provides-Extra: tensorflow
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: all
@@ -68,15 +68,15 @@
   the performance of active learning models on fully labeled data. Simulations
   can be run in ASReview LAB or via the command line interface with more
   advanced options.
 
 
 ## Installation
 
-The ASReview software requires Python 3.8+. Detailed step-by-step instructions
+The ASReview software requires Python 3.7+. Detailed step-by-step instructions
 to install Python and ASReview are available for
 [Windows](https://asreview.ai/installation-guide-windows/) and
 [macOS](https://asreview.ai/installation-guide-macos/) users.
 
 ```bash
 pip install asreview
 ```
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: asreview Version: 1.2.1 Summary: ASReview LAB - A
+Metadata-Version: 2.1 Name: asreview Version: 1.3a0 Summary: ASReview LAB - A
 tool for AI-assisted systematic reviews Home-page: https://github.com/asreview/
 asreview Author: ASReview LAB developers Author-email: asreview@uu.nl Project-
 URL: Bug Reports, https://github.com/asreview/asreview/issues Project-URL:
 Source, https://github.com/asreview/asreview/ Keywords: systematic
 review,machine-learning Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
 Engineering :: Information Analysis Classifier: Topic :: Text Processing ::
-General Classifier: Framework :: Flask Requires-Python: ~=3.8 Description-
+General Classifier: Framework :: Flask Requires-Python: ~=3.7 Description-
 Content-Type: text/markdown Provides-Extra: sbert Provides-Extra: doc2vec
 Provides-Extra: tensorflow Provides-Extra: dev Provides-Extra: test Provides-
 Extra: all License-File: LICENSE
      [https://raw.githubusercontent.com/asreview/asreview-artwork/master/
               LogoASReview/SVG/GitHub_Repo_Card_Transparent.svg]
 ## ASReview: Active learning for Systematic Reviews [![PyPI version](https://
 badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build
@@ -45,15 +45,15 @@
 implements three different modes: - **Oracle** Screen textual data in
 interaction with the active learning model. The reviewer is the 'oracle',
 making the labeling decisions. - **Exploration** Explore or demonstrate
 ASReview LAB with a completely labeled dataset. This mode is suitable for
 teaching purposes. - **Simulation** Evaluate the performance of active learning
 models on fully labeled data. Simulations can be run in ASReview LAB or via the
 command line interface with more advanced options. ## Installation The ASReview
-software requires Python 3.8+. Detailed step-by-step instructions to install
+software requires Python 3.7+. Detailed step-by-step instructions to install
 Python and ASReview are available for [Windows](https://asreview.ai/
 installation-guide-windows/) and [macOS](https://asreview.ai/installation-
 guide-macos/) users. ```bash pip install asreview ``` Upgrade ASReview with the
 following command: ```bash pip install --upgrade asreview ``` To install
 ASReview LAB with Docker, see [Install with Docker](https://
 asreview.readthedocs.io/en/latest/installation.html). ## How it works [!
 [ASReview LAB explained - animation](https://img.youtube.com/vi/k-a2SCq-LtA/
```

### Comparing `asreview-1.2.1/README.md` & `asreview-1.3a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   the performance of active learning models on fully labeled data. Simulations
   can be run in ASReview LAB or via the command line interface with more
   advanced options.
 
 
 ## Installation
 
-The ASReview software requires Python 3.8+. Detailed step-by-step instructions
+The ASReview software requires Python 3.7+. Detailed step-by-step instructions
 to install Python and ASReview are available for
 [Windows](https://asreview.ai/installation-guide-windows/) and
 [macOS](https://asreview.ai/installation-guide-macos/) users.
 
 ```bash
 pip install asreview
 ```
```

#### html2text {}

```diff
@@ -30,15 +30,15 @@
 data in interaction with the active learning model. The reviewer is the
 'oracle', making the labeling decisions. - **Exploration** :triangular_ruler:
 Explore or demonstrate ASReview LAB with a completely labeled dataset. This
 mode is suitable for teaching purposes. - **Simulation** :
 chart_with_upwards_trend: Evaluate the performance of active learning models on
 fully labeled data. Simulations can be run in ASReview LAB or via the command
 line interface with more advanced options. ## Installation The ASReview
-software requires Python 3.8+. Detailed step-by-step instructions to install
+software requires Python 3.7+. Detailed step-by-step instructions to install
 Python and ASReview are available for [Windows](https://asreview.ai/
 installation-guide-windows/) and [macOS](https://asreview.ai/installation-
 guide-macos/) users. ```bash pip install asreview ``` Upgrade ASReview with the
 following command: ```bash pip install --upgrade asreview ``` To install
 ASReview LAB with Docker, see [Install with Docker](https://
 asreview.readthedocs.io/en/latest/installation.html). ## How it works [!
 [ASReview LAB explained - animation](https://img.youtube.com/vi/k-a2SCq-LtA/
```

### Comparing `asreview-1.2.1/asreview/__main__.py` & `asreview-1.3a0/asreview/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,27 +32,25 @@
 
 
 def main():
     # Get the available entry points.
     entry_points = get_entry_points("asreview.entry_points")
 
     if (
-        len(sys.argv) > 1 and
-        not sys.argv[1].startswith("-") and
-        sys.argv[1] not in entry_points
+        len(sys.argv) > 1
+        and not sys.argv[1].startswith("-")
+        and sys.argv[1] not in entry_points
     ):
         raise ValueError(f"'{sys.argv[1]}' is not a valid subcommand.")
 
     elif len(sys.argv) > 1 and sys.argv[1] in entry_points:
-
         entry = entry_points[sys.argv[1]]
         entry.load()().execute(sys.argv[2:])
 
     else:
-
         description_subcommands = ""
 
         for name, pkg_entry_points in groupby(
             pkg_resources.iter_entry_points("asreview.entry_points"),
             lambda entry: entry.dist,
         ):
             description = metadata.metadata(name.project_name)["Summary"]
```

### Comparing `asreview-1.2.1/asreview/compat.py` & `asreview-1.3a0/asreview/compat.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/data/__init__.py` & `asreview-1.3a0/asreview/data/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/data/base.py` & `asreview-1.3a0/asreview/data/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,39 +58,36 @@
     try:
         dataset_path = DatasetManager().find(name).filepath
         return ASReviewData.from_file(dataset_path, *args, **kwargs)
     except DatasetNotFoundError:
         pass
 
     # Could not find dataset, return None.
-    raise FileNotFoundError(
-        f"File, URL, or dataset does not exist: '{name}'")
+    raise FileNotFoundError(f"File, URL, or dataset does not exist: '{name}'")
 
 
 def _get_filename_from_url(url):
-
     if not is_url(url):
         raise ValueError(f"'{url}' is not a valid URL.")
 
     if Path(urlparse(url).path).suffix:
         return Path(urlparse(url).path).name, url
     else:
-
         try:
             return urlopen(url).headers.get_filename(), url
         except HTTPError as err:
             # 308 (Permanent Redirect) not supported
             # See https://bugs.python.org/issue40321
             if err.code == 308:
                 return _get_filename_from_url(err.headers.get("Location"))
             else:
                 raise err
 
 
-class ASReviewData():
+class ASReviewData:
     """Data object to the dataset with texts, labels, DOIs etc.
 
     Arguments
     ---------
     df: pandas.DataFrame
         Dataframe containing the data for the ASReview data object.
     column_spec: dict
@@ -125,17 +122,15 @@
     final_included: numpy.ndarray
         Pending deprecation! Returns an array with document inclusion markers.
     labels: numpy.ndarray
         Identical to included.
 
     """
 
-    def __init__(self,
-                 df=None,
-                 column_spec=None):
+    def __init__(self, df=None, column_spec=None):
         self.df = df
         self.prior_idx = np.array([], dtype=int)
 
         self.max_idx = max(df.index.values) + 1
 
         # Infer column specifications if it is not given.
         if column_spec is None:
@@ -159,21 +154,23 @@
         """Compute a hash from the dataset.
 
         Returns
         -------
         str:
             SHA1 hash, computed from the titles/abstracts of the dataframe.
         """
-        if ((len(self.df.index) < 1000 and self.bodies is not None) or
-                self.texts is None):
+        if (
+            len(self.df.index) < 1000 and self.bodies is not None
+        ) or self.texts is None:
             texts = " ".join(self.bodies)
         else:
             texts = " ".join(self.texts)
-        return hashlib.sha1(" ".join(texts).encode(
-            encoding='UTF-8', errors='ignore')).hexdigest()
+        return hashlib.sha1(
+            " ".join(texts).encode(encoding="UTF-8", errors="ignore")
+        ).hexdigest()
 
     @classmethod
     def from_file(cls, fp, reader=None):
         """Create instance from supported file format.
 
         It works in two ways; either manual control where the conversion
         functions are supplied or automatic, where it searches in the entry
@@ -197,16 +194,15 @@
             fn = Path(fp).name
 
         entry_points = get_entry_points(entry_name="asreview.readers")
 
         try:
             reader = entry_points[Path(fn).suffix].load()
         except Exception:
-            raise BadFileFormatError(
-                f"Importing file {fp} not possible.")
+            raise BadFileFormatError(f"Importing file {fp} not possible.")
 
         df, column_spec = reader.read_data(fp)
 
         return cls(df, column_spec=column_spec)
 
     def record(self, i, by_index=True):
         """Create a record from an index.
@@ -228,24 +224,27 @@
         if not is_iterable(i):
             index_list = [i]
         else:
             index_list = i
 
         if by_index:
             records = [
-                PaperRecord(**self.df.iloc[j],
-                            column_spec=self.column_spec,
-                            record_id=self.df.index.values[j])
+                PaperRecord(
+                    **self.df.iloc[j],
+                    column_spec=self.column_spec,
+                    record_id=self.df.index.values[j],
+                )
                 for j in index_list
             ]
         else:
             records = [
-                PaperRecord(**self.df.loc[j, :],
-                            record_id=j,
-                            column_spec=self.column_spec) for j in index_list
+                PaperRecord(
+                    **self.df.loc[j, :], record_id=j, column_spec=self.column_spec
+                )
+                for j in index_list
             ]
 
         if is_iterable(i):
             return records
         return records[0]
 
     @property
@@ -255,17 +254,18 @@
     @property
     def texts(self):
         if self.title is None:
             return self.abstract
         if self.abstract is None:
             return self.title
 
-        cur_texts = np.array([
-            self.title[i] + " " + self.abstract[i] for i in range(len(self))
-        ], dtype=object)
+        cur_texts = np.array(
+            [self.title[i] + " " + self.abstract[i] for i in range(len(self))],
+            dtype=object,
+        )
         return cur_texts
 
     @property
     def headings(self):
         return self.title
 
     @property
@@ -292,16 +292,15 @@
             return self.df[self.column_spec["notes"]].values
         except KeyError:
             return None
 
     @property
     def keywords(self):
         try:
-            return self.df[self.column_spec["keywords"]].apply(
-                convert_keywords).values
+            return self.df[self.column_spec["keywords"]].apply(convert_keywords).values
         except KeyError:
             return None
 
     @property
     def authors(self):
         try:
             return self.df[self.column_spec["authors"]].values
@@ -416,16 +415,18 @@
 
             for suffix, entry in entry_points.items():
                 if Path(fp).suffix == suffix:
                     if best_suffix is None or len(suffix) > len(best_suffix):
                         best_suffix = suffix
 
             if best_suffix is None:
-                raise BadFileFormatError(f"Error exporting file {fp}, no capabilities "
-                                         "for exporting such a file.")
+                raise BadFileFormatError(
+                    f"Error exporting file {fp}, no capabilities "
+                    "for exporting such a file."
+                )
 
             writer = entry_points[best_suffix].load()
             writer.write_data(df, fp, labels=labels, ranking=ranking)
 
     def to_dataframe(self, labels=None, ranking=None):
         """Create new dataframe with updated label (order).
 
@@ -466,15 +467,15 @@
         # replace labeled NA values by np.nan
         if col_label in list(result_df):
             result_df[col_label] = result_df[col_label].astype(object)
             result_df.loc[result_df[col_label] == LABEL_NA, col_label] = np.nan
 
         return result_df
 
-    def duplicated(self, pid='doi'):
+    def duplicated(self, pid="doi"):
         """Return boolean Series denoting duplicate rows.
 
         Identify duplicates based on titles and abstracts and if available,
         on a persistent identifier (PID) such as the Digital Object Identifier
         (`DOI <https://www.doi.org/>`_).
 
         Arguments
@@ -492,35 +493,39 @@
             # in case of strings, strip whitespaces and replace empty strings with None
             if is_string_dtype(self.df[pid]) or is_object_dtype(self.df[pid]):
                 s_pid = self.df[pid].str.strip().replace("", None)
             else:
                 s_pid = self.df[pid]
 
             # save boolean series for duplicates based on persistent identifiers
-            s_dups_pid = ((s_pid.duplicated()) & (s_pid.notnull()))
+            s_dups_pid = (s_pid.duplicated()) & (s_pid.notnull())
         else:
             s_dups_pid = None
 
         # get the texts, clean them and replace empty strings with None
-        s = pd.Series(self.texts) \
-            .str.replace("[^A-Za-z0-9]", "", regex=True) \
-            .str.lower().str.strip().replace("", None)
+        s = (
+            pd.Series(self.texts)
+            .str.replace("[^A-Za-z0-9]", "", regex=True)
+            .str.lower()
+            .str.strip()
+            .replace("", None)
+        )
 
         # save boolean series for duplicates based on titles/abstracts
-        s_dups_text = ((s.duplicated()) & (s.notnull()))
+        s_dups_text = (s.duplicated()) & (s.notnull())
 
         # final boolean series for all duplicates
         if s_dups_pid is not None:
             s_dups = s_dups_pid | s_dups_text
         else:
             s_dups = s_dups_text
 
         return s_dups
 
-    def drop_duplicates(self, pid='doi', inplace=False, reset_index=True):
+    def drop_duplicates(self, pid="doi", inplace=False, reset_index=True):
         """Drop duplicate records.
 
         Drop duplicates based on titles and abstracts and if available,
         on a persistent identifier (PID) such the Digital Object Identifier
         (`DOI <https://www.doi.org/>`_).
 
         Arguments
```

### Comparing `asreview-1.2.1/asreview/data/statistics.py` & `asreview-1.3a0/asreview/data/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     if data.labels is None:
         n_missing_included = None
     else:
         n_missing_included = 0
     for i in range(len(data.title)):
         if len(data.title[i]) == 0:
             n_missing += 1
-            if (data.labels is not None and data.labels[i] == 1):
+            if data.labels is not None and data.labels[i] == 1:
                 n_missing_included += 1
     return n_missing, n_missing_included
 
 
 def n_missing_abstract(data):
     """Return the number of records with missing abstracts.
 
@@ -133,15 +133,15 @@
         n_missing_included = None
     else:
         n_missing_included = 0
 
     for i in range(len(data.abstract)):
         if len(data.abstract[i]) == 0:
             n_missing += 1
-            if (data.labels is not None and data.labels[i] == 1):
+            if data.labels is not None and data.labels[i] == 1:
                 n_missing_included += 1
 
     return n_missing, n_missing_included
 
 
 def title_length(data):
     """Return the average length of the titles.
@@ -199,15 +199,15 @@
         The statistic
     """
     if data.keywords is None:
         return None
     return np.average([len(keywords) for keywords in data.keywords])
 
 
-def n_duplicates(data, pid='doi'):
+def n_duplicates(data, pid="doi"):
     """Number of duplicates.
 
     Duplicate detection can be a very challenging task. Multiple
     algorithms can be used and results can be vary.
 
     Arguments
     ---------
```

### Comparing `asreview-1.2.1/asreview/datasets.py` & `asreview-1.3a0/asreview/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,41 +37,40 @@
     except URLError as e:
         if isinstance(e.reason, socket.timeout):
             raise Exception("Connection time out.")
         raise e
 
     datasets = []
     for data in meta_data.values():
-
         # raise error on versioned datasets
         if "type" in data and data["type"] == "versioned":
             raise ValueError("Datasets of type 'versioned' are deprecated")
 
         datasets.append(BaseDataSet(**data))
 
     return datasets
 
 
-class BaseDataSet():
-
-    def __init__(self,
-                 dataset_id,
-                 filepath,
-                 title,
-                 description=None,
-                 authors=None,
-                 topic=None,
-                 link=None,
-                 reference=None,
-                 img_url=None,
-                 license=None,
-                 year=None,
-                 aliases=[],
-                 **kwargs
-                 ):
+class BaseDataSet:
+    def __init__(
+        self,
+        dataset_id,
+        filepath,
+        title,
+        description=None,
+        authors=None,
+        topic=None,
+        link=None,
+        reference=None,
+        img_url=None,
+        license=None,
+        year=None,
+        aliases=[],
+        **kwargs,
+    ):
         """Base class for metadata of dataset.
 
         A BaseDataSet is a class with metadata about a (labeled)
         dataset used in ASReview LAB. The dataset can be used via
         the frontend or via command line interface.
 
         In general, a BaseDataSet is part of a group (BaseDataGroup).
@@ -130,32 +129,33 @@
         self.license = license
         self.year = year
         self.img_url = img_url
         self.aliases = aliases
         self.kwargs = kwargs
 
     def __str__(self):
-        return f"<BaseDataSet dataset_id='{self.dataset_id}' title='{self.title}'>"  # noqa
+        return (
+            f"<BaseDataSet dataset_id='{self.dataset_id}' title='{self.title}'>"  # noqa
+        )
 
     def __dict__(self):
-
         return {
-            'dataset_id': self.dataset_id,
-            'filepath': self.filepath,
-            'title': self.title,
-            'description': self.description,
-            'authors': self.authors,
-            'topic': self.topic,
-            'link': self.link,
-            'reference': self.reference,
-            'license': self.license,
-            'year': self.year,
-            'img_url': self.img_url,
-            'aliases': self.aliases,
-            **self.kwargs
+            "dataset_id": self.dataset_id,
+            "filepath": self.filepath,
+            "title": self.title,
+            "description": self.description,
+            "authors": self.authors,
+            "topic": self.topic,
+            "link": self.link,
+            "reference": self.reference,
+            "license": self.license,
+            "year": self.year,
+            "img_url": self.img_url,
+            "aliases": self.aliases,
+            **self.kwargs,
         }
 
 
 class BaseDataGroup(ABC):
     def __init__(self, *datasets):
         """Group of datasets.
 
@@ -187,17 +187,15 @@
     def append(self, dataset):
         """Append dataset to group.
 
         dataset: asreview.datasets.BaseDataSet
             A asreview BaseDataSet-like object.
         """
         if not issubclass(dataset, BaseDataSet):
-            raise ValueError(
-                "Expected BaseDataSet or subclass of BaseDataSet."
-            )
+            raise ValueError("Expected BaseDataSet or subclass of BaseDataSet.")
         self.datasets.append(dataset)
 
     def find(self, dataset_id):
         """Find dataset in the group.
 
         Parameters
         ----------
@@ -208,36 +206,34 @@
         Returns
         -------
         asreview.datasets.BaseDataSet:
             Returns base dataset with the given dataset_id.
         """
         results = []
         for d in self.datasets:
-            if dataset_id.lower() == d.dataset_id.lower() or \
-                    dataset_id.lower() in [a.lower() for a in d.aliases]:
+            if dataset_id.lower() == d.dataset_id.lower() or dataset_id.lower() in [
+                a.lower() for a in d.aliases
+            ]:
                 results.append(d)
 
         if len(results) > 1:
             raise ValueError(
                 f"Broken dataset group '{self.group_id}' containing multiple"
-                f" datasets with the same name/alias '{dataset_id}'.")
+                f" datasets with the same name/alias '{dataset_id}'."
+            )
         elif len(results) == 1:
             return results[0]
 
-        raise DatasetNotFoundError(
-            f"Dataset {dataset_id} not found"
-        )
-
+        raise DatasetNotFoundError(f"Dataset {dataset_id} not found")
 
-class DatasetManager():
 
+class DatasetManager:
     @property
     def groups(self):
-
-        entry_points = get_entry_points('asreview.datasets')
+        entry_points = get_entry_points("asreview.datasets")
 
         return list(entry_points.keys())
 
     def find(self, dataset_id):
         """Find a dataset.
 
         Parameters
@@ -263,49 +259,46 @@
         # If dataset_id is a valid path, create a dataset from it.
         if Path(dataset_id).is_file():
             return BaseDataSet(dataset_id)
 
         dataset_id = str(dataset_id)
 
         # get installed dataset groups
-        dataset_groups = get_entry_points('asreview.datasets')
+        dataset_groups = get_entry_points("asreview.datasets")
 
         # Split into group/dataset if possible.
         split_dataset_id = dataset_id.split(":")
         if len(split_dataset_id) == 2:
             data_group = split_dataset_id[0]
             split_dataset_id = split_dataset_id[1]
             if data_group in self.groups:
-                return dataset_groups[data_group].load()() \
-                    .find(split_dataset_id)
+                return dataset_groups[data_group].load()().find(split_dataset_id)
 
         # Look through all available/installed groups for the name.
         all_results = {}
         for group_id, dataset_entry in dataset_groups.items():
             try:
-                all_results[group_id] = \
-                    dataset_entry.load()().find(dataset_id)
+                all_results[group_id] = dataset_entry.load()().find(dataset_id)
             except Exception:
                 # don't raise error on loading entry point
                 pass
 
         # If we have multiple results, throw an error.
         if len(all_results) > 1:
             raise ValueError(
                 f"Multiple datasets found: {list(all_results)}."
                 "Use DATAGROUP:DATASET format to specify which one"
-                " you want.")
+                " you want."
+            )
 
         if len(all_results) == 1:
             return list(all_results.values())[0]
 
         # Could not find dataset
-        raise DatasetNotFoundError(
-            f"Dataset {dataset_id} not found"
-        )
+        raise DatasetNotFoundError(f"Dataset {dataset_id} not found")
 
     def list(self, include=None, exclude=None, serialize=True, raise_on_error=False):
         """List the available datasets.
 
         Parameters
         ----------
         include: str, iterable
@@ -332,67 +325,66 @@
             groups = include
         elif exclude is not None:
             exclude = exclude if is_iterable(exclude) else [exclude]
             groups = list(set(self.groups) - set(exclude))
         else:
             groups = self.groups.copy()
 
-        dataset_groups = get_entry_points('asreview.datasets')
+        dataset_groups = get_entry_points("asreview.datasets")
 
         group_list = []
         for group in groups:
             try:
                 group_list.append(dataset_groups[group].load()())
             except Exception as err:
-
                 # don't raise error on loading entry point
                 if raise_on_error:
                     raise err
 
         if serialize:
             dataset_list_ser = []
             for data_group in group_list:
                 try:
                     group_ser = []
                     for dataset in data_group.datasets:
                         group_ser.append(dataset.__dict__())
-                    dataset_list_ser.append({
-                        "group_id": data_group.group_id,
-                        "description": data_group.description,
-                        "datasets": group_ser
-                    })
+                    dataset_list_ser.append(
+                        {
+                            "group_id": data_group.group_id,
+                            "description": data_group.description,
+                            "datasets": group_ser,
+                        }
+                    )
                 except Exception as err:
                     # don't raise error on loading entry point
                     if raise_on_error:
                         raise err
 
             return dataset_list_ser
 
         return group_list
 
 
 class BenchmarkDataGroup(BaseDataGroup):
     """Datasets available in the benchmark platform."""
+
     group_id = "benchmark"
     description = "Datasets available in the online benchmark platform"
 
     def __init__(self):
         meta_file = "https://raw.githubusercontent.com/asreview/systematic-review-datasets/master/index_v1.json"  # noqa
         datasets = _download_from_metadata(meta_file)
 
-        super(BenchmarkDataGroup, self).__init__(
-            *datasets
-        )
+        super(BenchmarkDataGroup, self).__init__(*datasets)
 
 
 class NaturePublicationDataGroup(BaseDataGroup):
     """Datasets used in the paper Van de Schoot et al. 2020."""
+
     group_id = "benchmark-nature"
     description = "Datasets used in the validation paper published in Nature Machine Intelligence (van de Schoot et al. 2021)"  # noqa
 
     def __init__(self):
         meta_file = "https://raw.githubusercontent.com/asreview/paper-asreview/master/index_v1.json"  # noqa
         datasets = _download_from_metadata(meta_file)
 
-        super(NaturePublicationDataGroup, self).__init__(
-            *datasets
-        )
+        super(NaturePublicationDataGroup, self).__init__(*datasets)
```

### Comparing `asreview-1.2.1/asreview/entry_points/__init__.py` & `asreview-1.3a0/asreview/entry_points/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from asreview.entry_points.algorithms import AlgorithmsEntryPoint
+from asreview.entry_points.auth_tool import AuthTool
 from asreview.entry_points.base import BaseEntryPoint
 from asreview.entry_points.lab import LABEntryPoint
 from asreview.entry_points.lab import WebRunModelEntryPoint
 from asreview.entry_points.simulate import SimulateEntryPoint
 from asreview.entry_points.state_inspect import StateInspectEntryPoint
 
 """Default entry points for asreview."""
```

### Comparing `asreview-1.2.1/asreview/entry_points/algorithms.py` & `asreview-1.3a0/asreview/entry_points/algorithms.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from asreview.models.balance import list_balance_strategies
 from asreview.models.classifiers import list_classifiers
 from asreview.models.feature_extraction import list_feature_extraction
 from asreview.models.query import list_query_strategies
 
 
 def _format_algorithm(values, name, description):
-
     s = f"  {name: <20}Available {description}:\n\n"
 
     result = []
 
     for x in values:
         if hasattr(x, "label"):
             result.append(
@@ -37,42 +36,42 @@
     s += "\n\n"
 
     return s
 
 
 class AlgorithmsEntryPoint(BaseEntryPoint):
     """Entry point to list available algorithms in ASReview LAB."""
+
     description = "Available active learning algorithms for ASReview."
 
     def execute(self, argv):
-
         s = "Available active learning algorithms for ASReview. \n\n"
 
         # feature_extraction
         s += _format_algorithm(
             values=list_feature_extraction(),
             name="feature_extraction",
-            description="feature extraction algorithms"
+            description="feature extraction algorithms",
         )
 
         # classifiers
         s += _format_algorithm(
             values=list_classifiers(),
             name="classifiers",
-            description="classification algorithms"
+            description="classification algorithms",
         )
 
         # query_strategies
         s += _format_algorithm(
             values=list_query_strategies(),
             name="query_strategies",
-            description="query strategies"
+            description="query strategies",
         )
 
         # balance_strategies
         s += _format_algorithm(
             values=list_balance_strategies(),
             name="balance_strategies",
-            description="balance strategies"
+            description="balance strategies",
         )
 
         print(s)
```

### Comparing `asreview-1.2.1/asreview/entry_points/base.py` & `asreview-1.3a0/asreview/entry_points/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,17 @@
     -------
     argparse.ArgumentParser
         Configured argparser.
     """
 
     # parse arguments if available
     parser = argparse.ArgumentParser(
-        prog=prog,
-        description=description,
-        formatter_class=RawTextHelpFormatter
+        prog=prog, description=description, formatter_class=RawTextHelpFormatter
     )
     parser.add_argument(
         "--embedding",
         type=str,
         default=None,
-        dest='embedding_fp',
-        help="File path of embedding matrix. Required for LSTM models."
+        dest="embedding_fp",
+        help="File path of embedding matrix. Required for LSTM models.",
     )
     return parser
```

### Comparing `asreview-1.2.1/asreview/entry_points/lab.py` & `asreview-1.3a0/asreview/entry_points/lab.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,105 +9,143 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
+
 from asreview.entry_points.base import BaseEntryPoint
 from asreview.entry_points.base import DeprecateAction
 from asreview.entry_points.base import _base_parser
 from asreview.webapp.run_model import main as main_run_model
 
 HOST_NAME = os.getenv("ASREVIEW_HOST")
 if HOST_NAME is None:
     HOST_NAME = "localhost"
 PORT_NUMBER = 5000
 
 
 def _lab_parser(prog="lab"):
     parser = _base_parser(
         prog=prog,
-        description="""ASReview LAB - Active learning for Systematic Reviews."""  # noqa
+        description="""ASReview LAB - Active learning for Systematic Reviews.""",  # noqa
     )
 
     parser.add_argument(
         "--clean-project",
         dest="clean_project",
         default=None,
         type=str,
-        help="Safe cleanup of temporary files in project.")
+        help="Safe cleanup of temporary files in project.",
+    )
 
     parser.add_argument(
         "--clean-all-projects",
         dest="clean_all_projects",
         default=None,
-        action='store_true',
-        help="Safe cleanup of temporary files in all projects.")
+        action="store_true",
+        help="Safe cleanup of temporary files in all projects.",
+    )
 
     parser.add_argument(
         "--ip",
         default=HOST_NAME,
         type=str,
-        help="The IP address the server will listen on.")
+        help="The IP address the server will listen on.",
+    )
 
     parser.add_argument(
         "--port",
         default=PORT_NUMBER,
         type=int,
-        help="The port the server will listen on.")
+        help="The port the server will listen on.",
+    )
+
+    parser.add_argument(
+        "--enable-auth",
+        dest="enable_authentication",
+        action="store_true",
+        help="Enable authentication.",
+    )
+
+    parser.add_argument(
+        "--secret-key",
+        default=None,
+        type=str,
+        help="Secret key for authentication.",
+    )
+
+    parser.add_argument(
+        "--salt",
+        default=None,
+        type=str,
+        help="When using authentication, a salt code is needed" "for hasing passwords.",
+    )
+
+    parser.add_argument(
+        "--flask-configfile",
+        default="",
+        type=str,
+        help="Full path to a JSON file containing Flask parameters"
+        "for authentication.",
+    )
 
     parser.add_argument(
         "--no-browser",
         dest="no_browser",
-        action='store_true',
-        help="Do not open ASReview LAB in a browser after startup.")
+        action="store_true",
+        help="Do not open ASReview LAB in a browser after startup.",
+    )
 
     parser.add_argument(
         "--port-retries",
         dest="port_retries",
         default=50,
         type=int,
         help="The number of additional ports to try if the"
-        "specified port is not available.")
+        "specified port is not available.",
+    )
 
     parser.add_argument(
         "--certfile",
         default="",
         type=str,
-        help="The full path to an SSL/TLS certificate file.")
+        help="The full path to an SSL/TLS certificate file.",
+    )
 
     parser.add_argument(
         "--keyfile",
         default="",
         type=str,
-        help="The full path to a private key file for usage with SSL/TLS.")
+        help="The full path to a private key file for usage with SSL/TLS.",
+    )
 
     parser.add_argument(
         "--config_file",
         type=str,
         default=None,
         help="Deprecated, see subcommand simulate.",
-        action=DeprecateAction
+        action=DeprecateAction,
     )
+
     parser.add_argument(
         "--seed",
         default=None,
         type=int,
         help="Deprecated, see subcommand simulate.",
-        action=DeprecateAction
+        action=DeprecateAction,
     )
     return parser
 
 
 class LABEntryPoint(BaseEntryPoint):
     """Entry point to start the ASReview LAB webapp."""
 
     def execute(self, argv):
-
         from asreview.webapp.start_flask import main
 
         main(argv)
 
 
 class WebRunModelEntryPoint(BaseEntryPoint):
     description = "Internal use only."
```

### Comparing `asreview-1.2.1/asreview/entry_points/simulate.py` & `asreview-1.3a0/asreview/entry_points/simulate.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,53 +14,36 @@
 """Simulation entry point and utils."""
 
 import logging
 import shutil
 from pathlib import Path
 
 from asreview.compat import convert_id_to_idx
-from asreview.config import ASCII_LOGO
 from asreview.config import DEFAULT_BALANCE_STRATEGY
 from asreview.config import DEFAULT_FEATURE_EXTRACTION
 from asreview.config import DEFAULT_MODEL
 from asreview.config import DEFAULT_N_INSTANCES
 from asreview.config import DEFAULT_N_PRIOR_EXCLUDED
 from asreview.config import DEFAULT_N_PRIOR_INCLUDED
 from asreview.config import DEFAULT_QUERY_STRATEGY
-from asreview.config import EMAIL_ADDRESS
-from asreview.config import GITHUB_PAGE
+from asreview.data import ASReviewData
 from asreview.data import load_data
 from asreview.entry_points.base import BaseEntryPoint
 from asreview.entry_points.base import _base_parser
 from asreview.models.balance.utils import get_balance_model
 from asreview.models.classifiers import get_classifier
 from asreview.models.feature_extraction import get_feature_model
 from asreview.models.query import get_query_model
 from asreview.project import ASReviewProject
 from asreview.project import ProjectExistsError
 from asreview.project import open_state
 from asreview.review.simulate import ReviewSimulate
 from asreview.settings import ASReviewSettings
 from asreview.types import type_n_queries
 from asreview.utils import get_random_state
-from asreview.webapp.io import read_data
-
-ASCII_MSG_SIMULATE = """
----------------------------------------------------------------------------------
-|                                                                                |
-|  Welcome to ASReview LAB - AI-assisted systematic reviews software.            |
-|  In simulation mode the computer will simulate how well ASReview LAB           |
-|  could have accelerate the systematic review of your dataset.                  |
-|  You can sit back and relax while the computer runs this simulation.           |
-|                                                                                |
-|  GitHub page:        {0: <58}|
-|  Questions/remarks:  {1: <58}|
-|                                                                                |
----------------------------------------------------------------------------------
-""".format(GITHUB_PAGE, EMAIL_ADDRESS)  # noqa
 
 
 def _get_dataset_path_from_args(args_dataset):
     """Remove 'benchmark:' from the dataset name and add .csv suffix.
 
     Parameters
     ----------
@@ -69,18 +52,18 @@
 
     Returns
     -------
     str
         Dataset name without 'benchmark:' if it started with that,
         and with .csv suffix.
     """
-    if args_dataset.startswith('benchmark:'):
+    if args_dataset.startswith("benchmark:"):
         args_dataset = args_dataset[10:]
 
-    return Path(args_dataset).with_suffix('.csv').name
+    return Path(args_dataset).with_suffix(".csv").name
 
 
 def _set_log_verbosity(verbose):
     if verbose == 0:
         logging.getLogger().setLevel(logging.WARNING)
     elif verbose == 1:
         logging.getLogger().setLevel(logging.INFO)
@@ -88,128 +71,133 @@
         logging.getLogger().setLevel(logging.DEBUG)
 
 
 class SimulateEntryPoint(BaseEntryPoint):
     """Entry point for simulation with ASReview LAB."""
 
     def execute(self, argv):  # noqa
-
         # parse arguments
         parser = _simulate_parser()
         args = parser.parse_args(argv)
 
         # change the verbosity
         _set_log_verbosity(args.verbose)
 
         # check for state file extension
         if args.state_file is None:
-            raise ValueError(
-                "Specify project file name (with .asreview extension).")
-
-        # print intro message
-        print(ASCII_LOGO + ASCII_MSG_SIMULATE)
+            raise ValueError("Specify project file name (with .asreview extension).")
 
         # for webapp
         if args.dataset == "":
-
             project = ASReviewProject(args.state_file)
 
             with open_state(args.state_file) as state:
                 settings = state.settings
 
                 # Check if there are new labeled records.
                 exist_new_labeled_records = state.exist_new_labeled_records
 
             # collect command line arguments and pass them to the reviewer
             if exist_new_labeled_records:
-                as_data = read_data(project)
+                fp_data = Path(
+                    project.project_path, "data", project.config["dataset_path"]
+                )
+                as_data = ASReviewData.from_file(fp_data)
                 prior_idx = args.prior_idx
 
             classifier_model = get_classifier(settings.model)
             query_model = get_query_model(settings.query_strategy)
             balance_model = get_balance_model(settings.balance_strategy)
             feature_model = get_feature_model(settings.feature_extraction)
 
         # for simulation CLI
         else:
-
             # do this check now and again when zipping.
             if Path(args.state_file).exists():
                 raise ProjectExistsError("Project already exists.")
 
             as_data = load_data(args.dataset)
 
             if len(as_data) == 0:
-                raise ValueError("Supply at least one dataset"
-                                 " with at least one record.")
+                raise ValueError(
+                    "Supply at least one dataset" " with at least one record."
+                )
 
             # create a project file
-            fp_tmp_simulation = Path(
-                args.state_file).with_suffix(".asreview.tmp")
+            fp_tmp_simulation = Path(args.state_file).with_suffix(".asreview.tmp")
 
             project = ASReviewProject.create(
                 fp_tmp_simulation,
                 project_id=Path(args.state_file).stem,
                 project_mode="simulate",
                 project_name=Path(args.state_file).stem,
                 project_description="Simulation created via ASReview via "
-                                    "command line interface"
+                "command line interface",
             )
 
             # Add the dataset to the project file.
             dataset_path = _get_dataset_path_from_args(args.dataset)
 
-            as_data.to_file(
-                Path(fp_tmp_simulation, 'data', dataset_path)
-            )
+            as_data.to_file(Path(fp_tmp_simulation, "data", dataset_path))
             # Update the project.json.
             project.update_config(dataset_path=dataset_path)
 
             # create a new settings object from arguments
             settings = ASReviewSettings(
                 model=args.model,
                 n_instances=args.n_instances,
                 stop_if=args.stop_if,
                 n_prior_included=args.n_prior_included,
                 n_prior_excluded=args.n_prior_excluded,
                 query_strategy=args.query_strategy,
                 balance_strategy=args.balance_strategy,
-                feature_extraction=args.feature_extraction)
+                feature_extraction=args.feature_extraction,
+            )
             settings.from_file(args.config_file)
 
             # Initialize models.
             random_state = get_random_state(args.seed)
-            classifier_model = get_classifier(settings.model,
-                                              random_state=random_state,
-                                              **settings.model_param)
-            query_model = get_query_model(settings.query_strategy,
-                                          random_state=random_state,
-                                          **settings.query_param)
-            balance_model = get_balance_model(settings.balance_strategy,
-                                              random_state=random_state,
-                                              **settings.balance_param)
-            feature_model = get_feature_model(settings.feature_extraction,
-                                              random_state=random_state,
-                                              **settings.feature_param)
+            classifier_model = get_classifier(
+                settings.model, random_state=random_state, **settings.model_param
+            )
+            query_model = get_query_model(
+                settings.query_strategy,
+                random_state=random_state,
+                **settings.query_param,
+            )
+            balance_model = get_balance_model(
+                settings.balance_strategy,
+                random_state=random_state,
+                **settings.balance_param,
+            )
+            feature_model = get_feature_model(
+                settings.feature_extraction,
+                random_state=random_state,
+                **settings.feature_param,
+            )
 
             # prior knowledge
-            if args.prior_idx is not None and args.prior_record_id is not None and \
-                    len(args.prior_idx) > 0 and len(args.prior_record_id) > 0:
+            if (
+                args.prior_idx is not None
+                and args.prior_record_id is not None
+                and len(args.prior_idx) > 0
+                and len(args.prior_record_id) > 0
+            ):
                 raise ValueError(
                     "Not possible to provide both prior_idx and prior_record_id"
                 )
 
             prior_idx = args.prior_idx
-            if args.prior_record_id is not None and len(
-                    args.prior_record_id) > 0:
+            if args.prior_record_id is not None and len(args.prior_record_id) > 0:
                 prior_idx = convert_id_to_idx(as_data, args.prior_record_id)
 
         if classifier_model.name.startswith("lstm-"):
-            classifier_model.embedding_matrix = feature_model.\
-                get_embedding_matrix(as_data.texts, args.embedding_fp)
+            classifier_model.embedding_matrix = feature_model.get_embedding_matrix(
+                as_data.texts, args.embedding_fp
+            )
 
         try:
             # Initialize the review class.
             reviewer = ReviewSimulate(
                 as_data,
                 project=project,
                 model=classifier_model,
@@ -219,43 +207,41 @@
                 n_papers=args.n_papers,
                 n_instances=args.n_instances,
                 stop_if=args.stop_if,
                 prior_indices=prior_idx,
                 n_prior_included=args.n_prior_included,
                 n_prior_excluded=args.n_prior_excluded,
                 init_seed=args.init_seed,
-                write_interval=args.write_interval)
+                write_interval=args.write_interval,
+            )
 
             # Start the review process.
             project.update_review(status="review")
 
             with open_state(project, read_only=True) as s:
-
                 prior_df = s.get_priors()
 
                 print("The following records are prior knowledge:\n")
                 for i, row in prior_df.iterrows():
-                    preview = as_data.record(row['record_id'])
+                    preview = as_data.record(row["record_id"])
                     print(preview)
 
             print("Simulation started\n")
             reviewer.review()
         except Exception as err:
-
             # save the error to the project
             project.set_error(err)
 
             raise err
 
         print("\nSimulation finished")
         project.mark_review_finished()
 
         # create .ASReview file out of simulation folder
         if args.dataset != "":
-
             project.export(args.state_file)
             shutil.rmtree(fp_tmp_simulation)
 
 
 DESCRIPTION_SIMULATE = """
 ASReview for simulation.
 
@@ -268,129 +254,145 @@
 def _simulate_parser(prog="simulate", description=DESCRIPTION_SIMULATE):
     parser = _base_parser(prog=prog, description=description)
     # Active learning parameters
     # File path to the data.
     parser.add_argument(
         "dataset",
         type=str,
-        help="File path to the dataset or one of the benchmark datasets.")
+        help="File path to the dataset or one of the benchmark datasets.",
+    )
     # Initial data (prior knowledge)
-    parser.add_argument("--n_prior_included",
-                        default=DEFAULT_N_PRIOR_INCLUDED,
-                        type=int,
-                        help="Sample n prior included papers. "
-                        "Only used when --prior_idx is not given. "
-                        f"Default {DEFAULT_N_PRIOR_INCLUDED}")
-
-    parser.add_argument("--n_prior_excluded",
-                        default=DEFAULT_N_PRIOR_EXCLUDED,
-                        type=int,
-                        help="Sample n prior excluded papers. "
-                        "Only used when --prior_idx is not given. "
-                        f"Default {DEFAULT_N_PRIOR_EXCLUDED}")
+    parser.add_argument(
+        "--n_prior_included",
+        default=DEFAULT_N_PRIOR_INCLUDED,
+        type=int,
+        help="Sample n prior included papers. "
+        "Only used when --prior_idx is not given. "
+        f"Default {DEFAULT_N_PRIOR_INCLUDED}",
+    )
+
+    parser.add_argument(
+        "--n_prior_excluded",
+        default=DEFAULT_N_PRIOR_EXCLUDED,
+        type=int,
+        help="Sample n prior excluded papers. "
+        "Only used when --prior_idx is not given. "
+        f"Default {DEFAULT_N_PRIOR_EXCLUDED}",
+    )
 
     parser.add_argument(
         "--prior_idx",
         default=[],
         nargs="*",
         type=int,
-        help="Prior indices by rownumber (0 is first rownumber).")
-    parser.add_argument("--prior_record_id",
-                        default=[],
-                        nargs="*",
-                        type=int,
-                        help="Prior indices by record_id.")
+        help="Prior indices by rownumber (0 is first rownumber).",
+    )
+    parser.add_argument(
+        "--prior_record_id",
+        default=[],
+        nargs="*",
+        type=int,
+        help="Prior indices by record_id.",
+    )
     # logging and verbosity
     parser.add_argument(
         "--state_file",
         "-s",
         default=None,
         type=str,
-        help="Location to ASReview project file of simulation.")
-    parser.add_argument("-m",
-                        "--model",
-                        type=str,
-                        default=DEFAULT_MODEL,
-                        help=f"The prediction model for Active Learning. "
-                        f"Default: '{DEFAULT_MODEL}'.")
-    parser.add_argument("-q",
-                        "--query_strategy",
-                        type=str,
-                        default=DEFAULT_QUERY_STRATEGY,
-                        help=f"The query strategy for Active Learning. "
-                        f"Default: '{DEFAULT_QUERY_STRATEGY}'.")
+        help="Location to ASReview project file of simulation.",
+    )
+    parser.add_argument(
+        "-m",
+        "--model",
+        type=str,
+        default=DEFAULT_MODEL,
+        help=f"The prediction model for Active Learning. "
+        f"Default: '{DEFAULT_MODEL}'.",
+    )
+    parser.add_argument(
+        "-q",
+        "--query_strategy",
+        type=str,
+        default=DEFAULT_QUERY_STRATEGY,
+        help=f"The query strategy for Active Learning. "
+        f"Default: '{DEFAULT_QUERY_STRATEGY}'.",
+    )
     parser.add_argument(
         "-b",
         "--balance_strategy",
         type=str,
         default=DEFAULT_BALANCE_STRATEGY,
         help="Data rebalancing strategy mainly for RNN methods. Helps against"
         " imbalanced dataset with few inclusions and many exclusions. "
-        f"Default: '{DEFAULT_BALANCE_STRATEGY}'")
+        f"Default: '{DEFAULT_BALANCE_STRATEGY}'",
+    )
     parser.add_argument(
         "-e",
         "--feature_extraction",
         type=str,
         default=DEFAULT_FEATURE_EXTRACTION,
         help="Feature extraction method. Some combinations of feature"
         " extraction method and prediction model are impossible/ill"
         " advised."
-        f"Default: '{DEFAULT_FEATURE_EXTRACTION}'")
+        f"Default: '{DEFAULT_FEATURE_EXTRACTION}'",
+    )
     parser.add_argument(
-        '--init_seed',
+        "--init_seed",
         default=None,
         type=int,
         help="Seed for setting the prior indices if the --prior_idx option is "
         "not used. If the option --prior_idx is used with one or more "
-        "index, this option is ignored.")
+        "index, this option is ignored.",
+    )
     parser.add_argument(
         "--seed",
         default=None,
         type=int,
         help="Seed for the model (classifiers, balance strategies, "
-             "feature extraction techniques, and query strategies)."
+        "feature extraction techniques, and query strategies).",
     )
     parser.add_argument(
         "--config_file",
         type=str,
         default=None,
-        help="Configuration file with model settings"
-             "and parameter values."
+        help="Configuration file with model settings" "and parameter values.",
+    )
+    parser.add_argument(
+        "--n_instances",
+        default=DEFAULT_N_INSTANCES,
+        type=int,
+        help="Number of papers queried each query." f"Default {DEFAULT_N_INSTANCES}.",
     )
-    parser.add_argument("--n_instances",
-                        default=DEFAULT_N_INSTANCES,
-                        type=int,
-                        help="Number of papers queried each query."
-                        f"Default {DEFAULT_N_INSTANCES}.")
     parser.add_argument(
         "--n_queries",
         type=type_n_queries,
         default="min",
-        help="Deprecated, use 'stop_if' instead.")
+        help="Deprecated, use 'stop_if' instead.",
+    )
     parser.add_argument(
         "--stop_if",
         type=type_n_queries,
         default="min",
         help="The number of label actions to simulate. Default, 'min' "
         "will stop simulating when all relevant records are found. Use -1 "
-        "to simulate all labels actions.")
+        "to simulate all labels actions.",
+    )
     parser.add_argument(
         "-n",
         "--n_papers",
         type=int,
         default=None,
-        help="Deprecated, use 'stop_if' instead.")
-    parser.add_argument("--verbose",
-                        "-v",
-                        default=0,
-                        type=int,
-                        help="Verbosity")
+        help="Deprecated, use 'stop_if' instead.",
+    )
+    parser.add_argument("--verbose", "-v", default=0, type=int, help="Verbosity")
     parser.add_argument(
         "--write_interval",
         "-w",
         default=None,
         type=int,
         help="The simulation data will be written after each set of this"
         "many labeled records. By default only writes data at the end"
-        "of the simulation to make it as fast as possible.")
+        "of the simulation to make it as fast as possible.",
+    )
 
     return parser
```

### Comparing `asreview-1.2.1/asreview/entry_points/state_inspect.py` & `asreview-1.3a0/asreview/entry_points/state_inspect.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 
 from asreview.entry_points.base import BaseEntryPoint
 from asreview.project import get_project_path
 from asreview.project import open_state
 
 
 def _parse_state_inspect_args():
-
     # parse arguments if available
-    parser = argparse.ArgumentParser(prog="state-inspect",
-                                     description="Inspect state file.")
+    parser = argparse.ArgumentParser(
+        prog="state-inspect", description="Inspect state file."
+    )
     parser.add_argument(
-        "project_id",
-        type=str,
-        help="Project_id or path to ASReview file.")
+        "project_id", type=str, help="Project_id or path to ASReview file."
+    )
     parser.add_argument(
         "table",
         type=str,
-        help="Table to view (e.g. results, record_table, last_ranking).")
+        help="Table to view (e.g. results, record_table, last_ranking).",
+    )
 
     return parser
 
 
 class StateInspectEntryPoint(BaseEntryPoint):
     """Entry point to inspect ASReview LAB review progress."""
```

### Comparing `asreview-1.2.1/asreview/exceptions.py` & `asreview-1.3a0/asreview/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 class BadFileFormatError(Exception):
     pass
```

### Comparing `asreview-1.2.1/asreview/io/__init__.py` & `asreview-1.3a0/asreview/io/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/io/csv_reader.py` & `asreview-1.3a0/asreview/io/csv_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 # limitations under the License.
 
 import pandas as pd
 
 from asreview.io.utils import _standardize_dataframe
 
 
-class CSVReader():
-    """CVS file reader.
-    """
+class CSVReader:
+    """CVS file reader."""
 
     read_format = [".csv", ".tab", ".tsv"]
     write_format = [".csv", ".tsv", ".xlsx"]
 
     @classmethod
     def read_data(cls, fp):
         """Import dataset.
@@ -36,19 +35,14 @@
         Returns
         -------
         list:
             List with entries.
         """
         for encoding in ["utf-8", "ISO-8859-1"]:
             try:
-                df = pd.read_csv(
-                    fp,
-                    sep=None,
-                    encoding=encoding,
-                    engine='python'
-                )
+                df = pd.read_csv(fp, sep=None, encoding=encoding, engine="python")
                 return _standardize_dataframe(df)
             except UnicodeDecodeError:
                 # if unicode error, go to next encoding
                 continue
 
         raise UnicodeDecodeError("The encoding of the file is not supported.")
```

### Comparing `asreview-1.2.1/asreview/io/csv_writer.py` & `asreview-1.3a0/asreview/io/csv_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-class CSVWriter():
-    """CSV file writer.
-    """
+
+class CSVWriter:
+    """CSV file writer."""
 
     name = "csv"
     label = "CSV (UTF-8)"
     write_format = ".csv"
 
     @classmethod
     def write_data(cls, df, fp, sep=",", labels=None, ranking=None):
```

### Comparing `asreview-1.2.1/asreview/io/excel_reader.py` & `asreview-1.3a0/asreview/io/excel_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 
 import pandas as pd
 
 from asreview.config import COLUMN_DEFINITIONS
 from asreview.io.utils import _standardize_dataframe
 
 
-class ExcelReader():
-    """Excel file reader.
-    """
+class ExcelReader:
+    """Excel file reader."""
 
     read_format = [".xlsx"]
     write_format = [".csv", ".tsv", ".xlsx"]
 
     @classmethod
     def read_data(cls, fp):
         """Import dataset.
```

### Comparing `asreview-1.2.1/asreview/io/excel_writer.py` & `asreview-1.3a0/asreview/io/excel_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-class ExcelWriter():
-    """Excel file writer.
-    """
+
+class ExcelWriter:
+    """Excel file writer."""
 
     name = "xlsx"
     label = "Excel"
     write_format = ".xlsx"
 
     @classmethod
     def write_data(cls, df, fp, labels=None, ranking=None):
```

### Comparing `asreview-1.2.1/asreview/io/paper_record.py` & `asreview-1.3a0/asreview/io/paper_record.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,22 +47,22 @@
     title_str = ""
     author_str = ""
     heading = record.title
     if heading is None:
         heading = record.abstract
     if heading is not None:
         if len(heading) > w_title:
-            title_str = heading[:w_title - 2] + ".."
+            title_str = heading[: w_title - 2] + ".."
         else:
             title_str = heading
 
     if record.authors is not None:
         cur_authors = format_to_str(record.authors)
         if len(cur_authors) > w_authors:
-            author_str = cur_authors[:w_authors - 2] + ".."
+            author_str = cur_authors[: w_authors - 2] + ".."
         else:
             author_str = cur_authors
     format_str = "{0: <" + str(w_title) + "}   " + "{1: <" + str(w_authors)
     format_str += "}"
     prev_str = format_str.format(title_str, author_str)
     return prev_str
 
@@ -106,18 +106,18 @@
     elif record.included == 1:
         label = "RELEVANT"
     else:
         label = ""
 
     header = f"---{record.record_id}---{label}---"
 
-    return (f"\n{header:-<60}\n{title}{authors}{abstract}")
+    return f"\n{header:-<60}\n{title}{authors}{abstract}"
 
 
-class PaperRecord():
+class PaperRecord:
     """A single record from a paper in a systematic review.
 
     Arguments
     ---------
     record_id: int
         Some identifier for this record.
     title: str
@@ -134,15 +134,14 @@
         Current label of the paper. No label is indicated by
         asreview.config.LABEL_NA (== -1).
     kwargs: dict
         Any extra keyword arguments will be put in self.extra_fields.
     """
 
     def __init__(self, record_id, column_spec={}, **kwargs):
-
         for attr in [
             "title",
             "abstract",
             "authors",
             "notes",
             "keywords",
             "doi",
```

### Comparing `asreview-1.2.1/asreview/io/ris_reader.py` & `asreview-1.3a0/asreview/io/ris_reader.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/io/ris_writer.py` & `asreview-1.3a0/asreview/io/ris_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pandas as pd
 import rispy
 
 
-class RISWriter():
-    """RIS file writer.
-    """
+class RISWriter:
+    """RIS file writer."""
+
     name = "ris"
     label = "RIS"
     caution = "Available only if you imported a RIS file when creating the project"
     write_format = ".ris"
 
     @classmethod
     def write_data(cls, df, fp, labels=None, ranking=None):
@@ -44,15 +44,15 @@
         Returns
         -------
         RIS file
             Dataframe of all available record data.
         """
 
         # Turn pandas DataFrame into records (list of dictionaries) for rispy
-        records = df.to_dict('records')
+        records = df.to_dict("records")
 
         # Create an array for storing modified records
         records_new = []
 
         # Iterate over all available records
         for rec in records:
 
@@ -71,17 +71,19 @@
                 except Exception:
                     rec_copy[m] = []
 
             # Get label for record if specified, if not specified set to -1
             included = rec_copy.pop("included", -1)
 
             # Map labels to notes
-            dict_note = {-1: "ASReview_not_seen",
-                         0: "ASReview_irrelevant",
-                         1: "ASReview_relevant"}
+            dict_note = {
+                -1: "ASReview_not_seen",
+                0: "ASReview_irrelevant",
+                1: "ASReview_relevant",
+            }
             rec_copy["notes"].insert(0, dict_note[included])
 
             # Append the deepcopied and updated record to a new array
             records_new.append(rec_copy)
 
         # From buffered dataframe
         if fp is None:
```

### Comparing `asreview-1.2.1/asreview/io/tsv_writer.py` & `asreview-1.3a0/asreview/io/tsv_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-class TSVWriter():
-    """TSV file writer.
-    """
+
+class TSVWriter:
+    """TSV file writer."""
 
     name = "tsv"
     label = "TSV (UTF-8)"
     write_format = ".tsv"
 
     @classmethod
     def write_data(cls, df, fp, sep="\t", labels=None, ranking=None):
```

### Comparing `asreview-1.2.1/asreview/io/utils.py` & `asreview-1.3a0/asreview/io/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,27 +59,24 @@
         new_split = keywords.split(splitter)
         if len(new_split) > len(current_best):
             current_best = new_split
     return current_best
 
 
 def _is_record_id_unique(s):
-
     if len(pd.unique(s)) != len(s.index):
         raise ValueError("Column 'record_id' contains duplicate values.")
 
 
 def _is_record_id_notnull(s):
-
     if s.isnull().any():
         raise ValueError("Column 'record_id' contains missing values.")
 
 
 def _is_record_id_int(s):
-
     try:
         pd.to_numeric(s).astype(int)
     except Exception:
         raise ValueError("Column 'record_id' should contain integer values.")
 
 
 def _standardize_dataframe(df, column_def={}):
```

### Comparing `asreview-1.2.1/asreview/models/__init__.py` & `asreview-1.3a0/asreview/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 from asreview.models.classifiers.lstm_pool import LSTMPoolClassifier
 from asreview.models.classifiers.nb import NaiveBayesClassifier
 from asreview.models.classifiers.nn_2_layer import NN2LayerClassifier
 from asreview.models.classifiers.rf import RandomForestClassifier
 from asreview.models.classifiers.svm import SVMClassifier
 from asreview.models.classifiers.utils import get_classifier
 from asreview.models.classifiers.utils import get_classifier_class
-from asreview.models.classifiers.utils import list_classifiers as _list_classifiers    # NOQA
+from asreview.models.classifiers.utils import list_classifiers as _list_classifiers
 
 """Active learning model components.
 
 Components like classifiers, query strategies, balance strategies, and
 feature_extraction techniques."""
```

### Comparing `asreview-1.2.1/asreview/models/balance/__init__.py` & `asreview-1.3a0/asreview/models/balance/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/balance/base.py` & `asreview-1.3a0/asreview/models/balance/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/balance/double.py` & `asreview-1.3a0/asreview/models/balance/double.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,20 +48,15 @@
         number of samples. Higher values means that larger samples are more
         strongly penalizing zeros.
     """
 
     name = "double"
     label = "Dynamic resampling (Double)"
 
-    def __init__(self,
-                 a=2.155,
-                 alpha=0.94,
-                 b=0.789,
-                 beta=1.0,
-                 random_state=None):
+    def __init__(self, a=2.155, alpha=0.94, b=0.789, beta=1.0, random_state=None):
         super(DoubleBalance, self).__init__()
         self.a = a
         self.alpha = alpha
         self.b = b
         self.beta = beta
         self.fallback_model = SimpleBalance()
         self._random_state = get_random_state(random_state)
@@ -97,51 +92,52 @@
 
         # Compute sampling weights.
         one_weight = _one_weight(n_one, n_zero, self.a, self.alpha)
         zero_weight = _zero_weight(n_one + n_zero, self.b, self.beta)
         tot_zo_weight = one_weight * n_one + zero_weight * n_zero
         # Number of inclusions to sample.
         n_one_train = random_round(
-            one_weight * n_one * n_train / tot_zo_weight, self._random_state)
+            one_weight * n_one * n_train / tot_zo_weight, self._random_state
+        )
         # Should be at least 1, and at least two spots should be for exclusions.
         n_one_train = max(1, min(n_train - 2, n_one_train))
         # Number of exclusions to sample
         n_zero_train = n_train - n_one_train
 
         # Sample records of ones and zeroes
         one_train_idx = fill_training(one_idx, n_one_train, self._random_state)
-        zero_train_idx = fill_training(zero_idx, n_zero_train,
-                                       self._random_state)
+        zero_train_idx = fill_training(zero_idx, n_zero_train, self._random_state)
         # Merge and shuffle.
         all_idx = np.concatenate([one_train_idx, zero_train_idx])
         self._random_state.shuffle(all_idx)
 
         # Return resampled feature matrix and labels.
         return X[all_idx], y[all_idx]
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         parameter_space = {
             "bal_a": hp.lognormal("bal_a", 0, 1),
             "bal_alpha": hp.uniform("bal_alpha", 0, 2),
             "bal_b": hp.uniform("bal_b", 0, 1),
             # "bal_beta": hp.uniform("bal_beta", 0, 2),
         }
         return parameter_space, {}
 
 
 def _one_weight(n_one, n_zero, a, alpha):
     """Get the weight of the ones."""
-    weight = a * (n_one / n_zero)**(-alpha)
+    weight = a * (n_one / n_zero) ** (-alpha)
     return weight
 
 
 def _zero_weight(n_read, b, beta):
     """Get the weight of the zeros."""
-    weight = 1 - (1 - b) * (1 + log(n_read))**(-beta)
+    weight = 1 - (1 - b) * (1 + log(n_read)) ** (-beta)
     return weight
 
 
 def random_round(value, random_state):
     """Round up or down, depending on how far the value is.
 
     For example: 8.1 would be rounded to 8, 90% of the time, and rounded
@@ -150,20 +146,20 @@
     base = int(floor(value))
     if random_state.rand() < value - base:
         base += 1
     return base
 
 
 def fill_training(src_idx, n_train, random_state):
-    """Copy/sample until there are n_train indices sampled/copied.
-    """
+    """Copy/sample until there are n_train indices sampled/copied."""
     # Number of copies needed.
     n_copy = int(n_train / len(src_idx))
     # For the remainder, use sampling.
     n_sample = n_train - n_copy * len(src_idx)
 
     # Copy indices
     dest_idx = np.tile(src_idx, n_copy).reshape(-1)
     # Add samples
-    dest_idx = np.append(dest_idx,
-                         random_state.choice(src_idx, n_sample, replace=False))
+    dest_idx = np.append(
+        dest_idx, random_state.choice(src_idx, n_sample, replace=False)
+    )
     return dest_idx
```

### Comparing `asreview-1.2.1/asreview/models/balance/simple.py` & `asreview-1.3a0/asreview/models/balance/simple.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/balance/triple.py` & `asreview-1.3a0/asreview/models/balance/triple.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,35 +62,38 @@
         Governs the scaling of the weight of the max samples as a function
         of the % of papers read. Higher values mean stronger scaling.
     """
 
     name = "triple"
     label = "Dynamic resampling (Triple)"
 
-    def __init__(self,
-                 a=2.155,
-                 alpha=0.94,
-                 b=0.789,
-                 beta=1.0,
-                 c=0.835,
-                 gamma=2.0,
-                 shuffle=True,
-                 random_state=None):
+    def __init__(
+        self,
+        a=2.155,
+        alpha=0.94,
+        b=0.789,
+        beta=1.0,
+        c=0.835,
+        gamma=2.0,
+        shuffle=True,
+        random_state=None,
+    ):
         """Initialize the triple balance strategy."""
 
         super(TripleBalance, self).__init__()
         self.a = a
         self.alpha = alpha
         self.b = b
         self.beta = beta
         self.c = c
         self.gamma = gamma
         self.shuffle = shuffle
         self.fallback_model = DoubleBalance(
-            a=a, alpha=alpha, b=b, beta=beta, random_state=random_state)
+            a=a, alpha=alpha, b=b, beta=beta, random_state=random_state
+        )
         self._random_state = get_random_state(random_state)
 
     def sample(self, X, y, train_idx, shared):
         """Resample the training data.
 
         Arguments
         ---------
@@ -117,58 +120,78 @@
         rand_idx = rand_idx.astype(int)
         # Write them back for next round.
         if self.shuffle:
             self._random_state.shuffle(rand_idx)
             self._random_state.shuffle(max_idx)
 
         if len(rand_idx) == 0 or len(max_idx) == 0:
-            logging.debug("Warning: trying to use triple balance, but unable"
-                          f" to, because we have {len(max_idx)} max samples "
-                          f"and {len(rand_idx)} random samples.")
+            logging.debug(
+                "Warning: trying to use triple balance, but unable"
+                f" to, because we have {len(max_idx)} max samples "
+                f"and {len(rand_idx)} random samples."
+            )
             return self.fallback_model.sample(X, y, train_idx, shared)
 
         # Split the idx into three groups: 1's, random 0's, max 0's.
         one_idx = train_idx[np.where(y[train_idx] == 1)]
         zero_max_idx = max_idx[np.where(y[max_idx] == 0)]
         zero_rand_idx = rand_idx[np.where(y[rand_idx] == 0)]
 
         if len(zero_rand_idx) == 0 or len(zero_max_idx) == 0:
-            logging.debug("Warning: trying to use triple balance, but unable "
-                          f"to, because we have {len(zero_max_idx)} zero max"
-                          f"samples and {len(zero_rand_idx)} random samples.")
+            logging.debug(
+                "Warning: trying to use triple balance, but unable "
+                f"to, because we have {len(zero_max_idx)} zero max"
+                f"samples and {len(zero_rand_idx)} random samples."
+            )
             return self.fallback_model.sample(X, y, train_idx, shared)
 
         n_one = len(one_idx)
         n_zero_rand = len(zero_rand_idx)
         n_zero_max = len(zero_max_idx)
         n_samples = len(y)
         n_train = len(train_idx)
 
         # Get the distribution of 1's, and random 0's and max 0's.
         n_one_train, n_zero_rand_train, n_zero_max_train = _get_triple_dist(
-            n_one, n_zero_rand, n_zero_max, n_samples, n_train, self.a,
-            self.alpha, self.b, self.beta, self.c, self.gamma,
-            self._random_state)
-        logging.debug(f"(1, 0_rand, 0_max) = ({n_one_train}, "
-                      f"{n_zero_rand_train}, {n_zero_max_train})")
+            n_one,
+            n_zero_rand,
+            n_zero_max,
+            n_samples,
+            n_train,
+            self.a,
+            self.alpha,
+            self.b,
+            self.beta,
+            self.c,
+            self.gamma,
+            self._random_state,
+        )
+        logging.debug(
+            f"(1, 0_rand, 0_max) = ({n_one_train}, "
+            f"{n_zero_rand_train}, {n_zero_max_train})"
+        )
 
         one_train_idx = fill_training(one_idx, n_one_train, self._random_state)
-        zero_rand_train_idx = fill_training(zero_rand_idx, n_zero_rand_train,
-                                            self._random_state)
-        zero_max_train_idx = fill_training(zero_max_idx, n_zero_max_train,
-                                           self._random_state)
+        zero_rand_train_idx = fill_training(
+            zero_rand_idx, n_zero_rand_train, self._random_state
+        )
+        zero_max_train_idx = fill_training(
+            zero_max_idx, n_zero_max_train, self._random_state
+        )
 
         all_idx = np.concatenate(
-            [one_train_idx, zero_rand_train_idx, zero_max_train_idx])
+            [one_train_idx, zero_rand_train_idx, zero_max_train_idx]
+        )
         self._random_state.shuffle(all_idx)
 
         return X[all_idx], y[all_idx]
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         parameter_space = {
             "bal_a": hp.lognormal("bal_a", 0, 1),
             "bal_alpha": hp.uniform("bal_alpha", 0, 2),
             "bal_b": hp.uniform("bal_b", 0, 1),
             # "bal_zero_beta": hp.uniform("bal_zero_beta", 0, 2),
             "bal_c": hp.uniform("bal_c", 0, 1),
             # "bal_zero_max_gamma": hp.uniform("bal_zero_max_gamma", 0.01, 2)
@@ -188,36 +211,48 @@
         Asymptotic ratio for infinite number of samples.
 
     Returns
     -------
     float:
         Weight ratio between 1's and 0's
     """
-    weight = 1 - (1 - c) * (1 - fraction_read)**gamma
+    weight = 1 - (1 - c) * (1 - fraction_read) ** gamma
     return weight
 
 
-def _get_triple_dist(n_one, n_zero_rand, n_zero_max, n_samples, n_train, one_a,
-                     one_alpha, zero_b, zero_beta, zero_max_c, zero_max_gamma,
-                     random_state):
-    " Get the number of 1's, random 0's and max 0's in each mini epoch. "
+def _get_triple_dist(
+    n_one,
+    n_zero_rand,
+    n_zero_max,
+    n_samples,
+    n_train,
+    one_a,
+    one_alpha,
+    zero_b,
+    zero_beta,
+    zero_max_c,
+    zero_max_gamma,
+    random_state,
+):
+    "Get the number of 1's, random 0's and max 0's in each mini epoch."
     n_zero = n_zero_rand + n_zero_max
     n_read = n_one + n_zero
     one_weight = _one_weight(n_one, n_zero, one_a, one_alpha)
     zero_weight = _zero_weight(n_read, zero_b, zero_beta)
-    zero_max_weight = _zero_max_weight(n_read / n_samples, zero_max_c,
-                                       zero_max_gamma)
+    zero_max_weight = _zero_max_weight(n_read / n_samples, zero_max_c, zero_max_gamma)
 
     tot_zo_weight = one_weight * n_one + zero_weight * n_zero
 
-    n_one_train = random_round(one_weight * n_one * n_train / tot_zo_weight,
-                               random_state)
+    n_one_train = random_round(
+        one_weight * n_one * n_train / tot_zo_weight, random_state
+    )
     n_one_train = max(1, min(n_train - 2, n_one_train))
     n_zero_train = n_train - n_one_train
 
     tot_rm_weight = 1 * n_zero_rand + zero_max_weight * n_zero_max
     n_zero_rand_train = random_round(
-        n_zero_train * 1 * n_zero_rand / tot_rm_weight, random_state)
+        n_zero_train * 1 * n_zero_rand / tot_rm_weight, random_state
+    )
     n_zero_rand_train = max(1, min(n_zero_rand - 1, n_zero_rand_train))
     n_zero_max_train = n_zero_train - n_zero_rand_train
 
     return n_one_train, n_zero_rand_train, n_zero_max_train
```

### Comparing `asreview-1.2.1/asreview/models/balance/undersample.py` & `asreview-1.3a0/asreview/models/balance/undersample.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,21 @@
 
         # If we don't have an excess of 0's, give back all training_samples.
         if n_one / n_zero >= self.ratio:
             shuf_ind = np.append(one_ind, zero_ind)
         else:
             n_zero_epoch = ceil(n_one / self.ratio)
             zero_under = self._random_state.choice(
-                np.arange(n_zero), n_zero_epoch, replace=False)
+                np.arange(n_zero), n_zero_epoch, replace=False
+            )
             shuf_ind = np.append(one_ind, zero_ind[zero_under])
 
         self._random_state.shuffle(shuf_ind)
         return X[shuf_ind], y[shuf_ind]
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         parameter_space = {
-            "bal_ratio": hp.lognormal('bal_ratio', 0, 1),
+            "bal_ratio": hp.lognormal("bal_ratio", 0, 1),
         }
         return parameter_space, {}
```

### Comparing `asreview-1.2.1/asreview/models/balance/utils.py` & `asreview-1.3a0/asreview/models/balance/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,15 @@
         Name of the model, e.g. 'simple', 'double' or 'undersample'.
 
     Returns
     -------
     BaseBalanceModel:
         Class corresponding to the name.
     """
-    return _model_class_from_entry_point(
-        name,
-        entry_name="asreview.models.balance")
+    return _model_class_from_entry_point(name, entry_name="asreview.models.balance")
 
 
 def get_balance_model(name, *args, random_state=None, **kwargs):
     """Get an instance of a balance model from a string.
 
     Arguments
     ---------
```

### Comparing `asreview-1.2.1/asreview/models/base.py` & `asreview-1.3a0/asreview/models/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/classifiers/__init__.py` & `asreview-1.3a0/asreview/models/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/classifiers/base.py` & `asreview-1.3a0/asreview/models/classifiers/base.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/classifiers/logistic.py` & `asreview-1.3a0/asreview/models/classifiers/logistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,29 +39,30 @@
         Number of CPU cores used.
     """
 
     name = "logistic"
     label = "Logistic regression"
 
     def __init__(self, C=1.0, class_weight=1.0, random_state=None, n_jobs=1):
-
         super(LogisticClassifier, self).__init__()
         self.C = C
         self.class_weight = class_weight
         self.n_jobs = n_jobs
 
         self._model = LogisticRegression(
             solver="liblinear",
             C=C,
             class_weight=_set_class_weight(class_weight),
             n_jobs=n_jobs,
-            random_state=random_state)
+            random_state=random_state,
+        )
         logging.debug(self._model)
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         hyper_choices = {}
         hyper_space = {
             "mdl_C": hp.lognormal("mdl_C", 0, 1),
             "mdl_class_weight": hp.lognormal("mdl_class_weight", 0, 1),
         }
         return hyper_space, hyper_choices
```

### Comparing `asreview-1.2.1/asreview/models/classifiers/lstm_base.py` & `asreview-1.3a0/asreview/models/classifiers/lstm_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,15 @@
 
 from asreview.models.classifiers.base import BaseTrainClassifier
 from asreview.models.classifiers.utils import _set_class_weight
 
 
 def _check_tensorflow():
     if not TF_AVAILABLE:
-        raise ImportError(
-            "Install tensorflow package to use"
-            " LSTM-base.")
+        raise ImportError("Install tensorflow package to use" " LSTM-base.")
 
 
 class LSTMBaseClassifier(BaseTrainClassifier):
     """LSTM-base classifier (``lstm-base``).
 
     LSTM model that consists of an embedding layer, LSTM layer with one
     output, dense layer, and a single sigmoid output node. Use the
@@ -86,27 +84,29 @@
     class_weight: float
         Class weight for the included papers.
     """
 
     name = "lstm-base"
     label = "LSTM classic"
 
-    def __init__(self,
-                 embedding_matrix=None,
-                 backwards=True,
-                 dropout=0.4,
-                 optimizer="rmsprop",
-                 lstm_out_width=20,
-                 learn_rate=1.0,
-                 dense_width=128,
-                 verbose=0,
-                 batch_size=32,
-                 epochs=35,
-                 shuffle=False,
-                 class_weight=30.0):
+    def __init__(
+        self,
+        embedding_matrix=None,
+        backwards=True,
+        dropout=0.4,
+        optimizer="rmsprop",
+        lstm_out_width=20,
+        learn_rate=1.0,
+        dense_width=128,
+        verbose=0,
+        batch_size=32,
+        epochs=35,
+        shuffle=False,
+        class_weight=30.0,
+    ):
         """Initialize the LSTM base model"""
         super(LSTMBaseClassifier, self).__init__()
         self.embedding_matrix = embedding_matrix
         self.backwards = backwards
         self.dropout = dropout
         self.optimizer = optimizer
         self.lstm_out_width = lstm_out_width
@@ -117,15 +117,14 @@
         self.epochs = epochs
         self.shuffle = shuffle
         self.class_weight = class_weight
         self._model = None
         self.sequence_length = None
 
     def fit(self, X, y):
-
         # check is tensorflow is available
         _check_tensorflow()
 
         if isspmatrix(X):
             X = X.toarray()
 
         sequence_length = X.shape[1]
@@ -136,26 +135,28 @@
                 backwards=self.backwards,
                 dropout=self.dropout,
                 optimizer=self.optimizer,
                 max_sequence_length=self.sequence_length,
                 lstm_out_width=self.lstm_out_width,
                 dense_width=self.dense_width,
                 learn_rate=self.learn_rate,
-                verbose=self.verbose)
+                verbose=self.verbose,
+            )
             print(keras_model)
             self._model = KerasClassifier(keras_model, verbose=self.verbose)
 
         self._model.fit(
             X,
             y,
             batch_size=self.batch_size,
             epochs=self.epochs,
             shuffle=self.shuffle,
             class_weight=_set_class_weight(self.class_weight),
-            verbose=self.verbose)
+            verbose=self.verbose,
+        )
 
     def predict_proba(self, X):
         """Get the inclusion probability for each sample.
 
         Arguments
         ---------
         X: numpy.ndarray
@@ -171,39 +172,42 @@
         if isspmatrix(X):
             X = X.toarray()
 
         return self._model.predict_proba(X)
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         hyper_choices = {}
         hyper_space = {
             "mdl_dropout": hp.uniform("mdl_dropout", 0, 0.9),
             "mdl_lstm_out_width": hp.quniform("mdl_lstm_out_width", 1, 50, 1),
             "mdl_dense_width": hp.quniform("mdl_dense_width", 1, 200, 1),
-            "mdl_learn_rate_mult": hp.lognormal("mdl_learn_rate_mult", 0, 1)
+            "mdl_learn_rate_mult": hp.lognormal("mdl_learn_rate_mult", 0, 1),
         }
         return hyper_space, hyper_choices
 
     @property
     def default_param(self):
         defaults = super(LSTMBaseClassifier, self).default_param
         defaults.pop("embedding_matrix")
         return defaults
 
 
-def _create_lstm_base_model(embedding_matrix,
-                            backwards=True,
-                            dropout=0.4,
-                            optimizer='rmsprop',
-                            max_sequence_length=1000,
-                            lstm_out_width=20,
-                            dense_width=128,
-                            learn_rate=1.0,
-                            verbose=1):
+def _create_lstm_base_model(
+    embedding_matrix,
+    backwards=True,
+    dropout=0.4,
+    optimizer="rmsprop",
+    max_sequence_length=1000,
+    lstm_out_width=20,
+    dense_width=128,
+    learn_rate=1.0,
+    verbose=1,
+):
     """Return callable lstm model.
     Returns
     -------
     callable:
         A function that return the Keras Sklearn model when
         called.
 
@@ -218,42 +222,46 @@
         # add first embedding layer with pretrained wikipedia weights
         model.add(
             Embedding(
                 embedding_matrix.shape[0],
                 embedding_matrix.shape[1],
                 weights=[embedding_matrix],
                 input_length=max_sequence_length,
-                trainable=False))
+                trainable=False,
+            )
+        )
 
         # add LSTM layer
         model.add(
             LSTM(
                 lstm_out_width,
-                input_shape=(max_sequence_length, ),
+                input_shape=(max_sequence_length,),
                 go_backwards=backwards,
                 dropout=dropout,
                 recurrent_dropout=dropout,
-            ))
+            )
+        )
 
         # add Dense layer with relu activation
-        model.add(Dense(
-            dense_width,
-            activation='relu',
-        ))
+        model.add(
+            Dense(
+                dense_width,
+                activation="relu",
+            )
+        )
 
         # add Dense layer
-        model.add(Dense(1, activation='sigmoid'))
+        model.add(Dense(1, activation="sigmoid"))
 
         optimizer_fn = _get_optimizer(optimizer, learn_rate)
 
         # Compile model
         model.compile(
-            loss='binary_crossentropy',
-            optimizer=optimizer_fn,
-            metrics=['acc'])
+            loss="binary_crossentropy", optimizer=optimizer_fn, metrics=["acc"]
+        )
 
         if verbose >= 1:
             model.summary(verbose=verbose)
 
         return model
 
     return model_wrapper
```

### Comparing `asreview-1.2.1/asreview/models/classifiers/lstm_pool.py` & `asreview-1.3a0/asreview/models/classifiers/lstm_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 from asreview.models.classifiers.base import BaseTrainClassifier
 from asreview.models.classifiers.lstm_base import _get_optimizer
 from asreview.models.classifiers.utils import _set_class_weight
 
 
 def _check_tensorflow():
     if not TF_AVAILABLE:
-        raise ImportError(
-            "Install tensorflow package to use"
-            " LSTM-pool.")
+        raise ImportError("Install tensorflow package to use" " LSTM-pool.")
 
 
 class LSTMPoolClassifier(BaseTrainClassifier):
     """
     LSTM-pool classifier (``lstm-pool``).
 
     LSTM model that consists of an embedding layer, LSTM layer with many
@@ -90,27 +88,29 @@
     class_weight: float
         Class weight for the included papers.
     """
 
     name = "lstm-pool"
     label = "LSTM with a max pooling layer"
 
-    def __init__(self,
-                 embedding_matrix=None,
-                 backwards=True,
-                 dropout=0.4,
-                 optimizer="rmsprop",
-                 lstm_out_width=20,
-                 lstm_pool_size=128,
-                 learn_rate=1.0,
-                 verbose=0,
-                 batch_size=32,
-                 epochs=35,
-                 shuffle=False,
-                 class_weight=30.0):
+    def __init__(
+        self,
+        embedding_matrix=None,
+        backwards=True,
+        dropout=0.4,
+        optimizer="rmsprop",
+        lstm_out_width=20,
+        lstm_pool_size=128,
+        learn_rate=1.0,
+        verbose=0,
+        batch_size=32,
+        epochs=35,
+        shuffle=False,
+        class_weight=30.0,
+    ):
         """Initialize the LSTM pool model."""
         super(LSTMPoolClassifier, self).__init__()
         self.embedding_matrix = embedding_matrix
         self.backwards = backwards
         self.dropout = dropout
         self.optimizer = optimizer
         self.lstm_out_width = lstm_out_width
@@ -121,15 +121,14 @@
         self.shuffle = shuffle
         self.class_weight = _set_class_weight(class_weight)
         self.lstm_pool_size = lstm_pool_size
         self._model = None
         self.sequence_length = None
 
     def fit(self, X, y):
-
         # check is tensorflow is available
         _check_tensorflow()
 
         if isspmatrix(X):
             X = X.toarray()
 
         sequence_length = X.shape[1]
@@ -139,24 +138,26 @@
                 embedding_matrix=self.embedding_matrix,
                 backwards=self.backwards,
                 dropout=self.dropout,
                 optimizer=self.optimizer,
                 max_sequence_length=sequence_length,
                 lstm_out_width=self.lstm_out_width,
                 learn_rate=self.learn_rate,
-                verbose=self.verbose)
+                verbose=self.verbose,
+            )
             self._model = KerasClassifier(keras_model, verbose=self.verbose)
         self._model.fit(
             X,
             y,
             batch_size=self.batch_size,
             epochs=self.epochs,
             shuffle=self.shuffle,
             class_weight=self.class_weight,
-            verbose=self.verbose)
+            verbose=self.verbose,
+        )
 
     def predict_proba(self, X):
         """Get the inclusion probability for each sample.
 
         Arguments
         ---------
         X: numpy.ndarray
@@ -178,34 +179,36 @@
         from hyperopt import hp
 
         hyper_choices = {}
         hyper_space = {
             "mdl_dropout": hp.uniform("mdl_dropout", 0, 0.9),
             "mdl_lstm_out_width": hp.quniform("mdl_lstm_out_width", 1, 50, 1),
             "mdl_dense_width": hp.quniform("mdl_dense_width", 1, 200, 1),
-            "mdl_learn_rate_mult": hp.lognormal("mdl_learn_rate_mult", 0, 1)
+            "mdl_learn_rate_mult": hp.lognormal("mdl_learn_rate_mult", 0, 1),
         }
         return hyper_space, hyper_choices
 
     @property
     def default_param(self):
         defaults = super(LSTMPoolClassifier, self).default_param
         defaults.pop("embedding_matrix")
         return defaults
 
 
-def _create_lstm_pool_model(embedding_matrix,
-                            backwards=True,
-                            dropout=0.4,
-                            optimizer='rmsprop',
-                            max_sequence_length=1000,
-                            lstm_out_width=20,
-                            lstm_pool_size=100,
-                            learn_rate=1.0,
-                            verbose=1):
+def _create_lstm_pool_model(
+    embedding_matrix,
+    backwards=True,
+    dropout=0.4,
+    optimizer="rmsprop",
+    max_sequence_length=1000,
+    lstm_out_width=20,
+    lstm_pool_size=100,
+    learn_rate=1.0,
+    verbose=1,
+):
     """Return callable lstm model.
     Returns
     -------
     callable:
         A function that return the Keras Sklearn model when
         called.
 
@@ -222,41 +225,47 @@
         # add first embedding layer with pretrained wikipedia weights
         model.add(
             Embedding(
                 embedding_matrix.shape[0],
                 embedding_matrix.shape[1],
                 weights=[embedding_matrix],
                 input_length=max_sequence_length,
-                trainable=False))
+                trainable=False,
+            )
+        )
 
         # add LSTM layer
         model.add(
             LSTM(
                 lstm_out_width,
-                input_shape=(max_sequence_length, ),
+                input_shape=(max_sequence_length,),
                 go_backwards=backwards,
                 dropout=dropout,
                 recurrent_dropout=dropout,
                 return_sequences=True,
                 kernel_constraint=MaxNorm(),
-            ))
+            )
+        )
 
-        model.add(MaxPooling1D(pool_size=lstm_pool_size, ))
+        model.add(
+            MaxPooling1D(
+                pool_size=lstm_pool_size,
+            )
+        )
         model.add(Flatten())
 
         # Add output layer
-        model.add(Dense(1, activation='sigmoid'))
+        model.add(Dense(1, activation="sigmoid"))
 
         optimizer_fn = _get_optimizer(optimizer, learn_rate)
 
         # Compile model
         model.compile(
-            loss='binary_crossentropy',
-            optimizer=optimizer_fn,
-            metrics=['acc'])
+            loss="binary_crossentropy", optimizer=optimizer_fn, metrics=["acc"]
+        )
 
         if verbose >= 1:
             model.summary()
 
         return model
 
     return model_wrapper
```

### Comparing `asreview-1.2.1/asreview/models/classifiers/nb.py` & `asreview-1.3a0/asreview/models/classifiers/nb.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,20 @@
         (0 for no smoothing).
     """
 
     name = "nb"
     label = "Naive Bayes"
 
     def __init__(self, alpha=3.822):
-
         super(NaiveBayesClassifier, self).__init__()
         self.alpha = alpha
         self._model = MultinomialNB(alpha=alpha)
         logging.debug(self._model)
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         hyper_choices = {}
         hyper_space = {
             "mdl_alpha": hp.lognormal("mdl_alpha", 0, 1),
         }
         return hyper_space, hyper_choices
```

### Comparing `asreview-1.2.1/asreview/models/classifiers/nn_2_layer.py` & `asreview-1.3a0/asreview/models/classifiers/nn_2_layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 from asreview.models.classifiers.utils import _set_class_weight
 
 
 def _check_tensorflow():
     if not TF_AVAILABLE:
         raise ImportError(
             "Install tensorflow package to use"
-            " Fully connected neural network (2 hidden layers).")
+            " Fully connected neural network (2 hidden layers)."
+        )
 
 
 class NN2LayerClassifier(BaseTrainClassifier):
     """Fully connected neural network (2 hidden layers) classifier (``nn-2-layer``).
 
     Neural network with two hidden, dense layers of the same size.
 
@@ -83,24 +84,26 @@
     class_weight: float
         Class weights for inclusions (1's).
     """
 
     name = "nn-2-layer"
     label = "Fully connected neural network (2 hidden layers)"
 
-    def __init__(self,
-                 dense_width=128,
-                 optimizer='rmsprop',
-                 learn_rate=1.0,
-                 regularization=0.01,
-                 verbose=0,
-                 epochs=35,
-                 batch_size=32,
-                 shuffle=False,
-                 class_weight=30.0):
+    def __init__(
+        self,
+        dense_width=128,
+        optimizer="rmsprop",
+        learn_rate=1.0,
+        regularization=0.01,
+        verbose=0,
+        epochs=35,
+        batch_size=32,
+        shuffle=False,
+        class_weight=30.0,
+    ):
         """Initialize the 2-layer neural network model."""
         super(NN2LayerClassifier, self).__init__()
         self.dense_width = int(dense_width)
         self.optimizer = optimizer
         self.learn_rate = learn_rate
         self.regularization = regularization
         self.verbose = verbose
@@ -109,69 +112,71 @@
         self.shuffle = shuffle
         self.class_weight = class_weight
 
         self._model = None
         self.input_dim = None
 
     def fit(self, X, y):
-
         # check is tensorflow is available
         _check_tensorflow()
 
         if scipy.sparse.issparse(X):
             X = X.toarray()
         if self._model is None or X.shape[1] != self.input_dim:
             self.input_dim = X.shape[1]
             keras_model = _create_dense_nn_model(
-                self.input_dim, self.dense_width, self.optimizer,
-                self.learn_rate, self.regularization, self.verbose)
+                self.input_dim,
+                self.dense_width,
+                self.optimizer,
+                self.learn_rate,
+                self.regularization,
+                self.verbose,
+            )
             self._model = KerasClassifier(keras_model, verbose=self.verbose)
 
         self._model.fit(
             X,
             y,
             batch_size=self.batch_size,
             epochs=self.epochs,
             shuffle=self.shuffle,
             verbose=self.verbose,
-            class_weight=_set_class_weight(self.class_weight))
+            class_weight=_set_class_weight(self.class_weight),
+        )
 
     def predict_proba(self, X):
         if scipy.sparse.issparse(X):
             X = X.toarray()
         return super(NN2LayerClassifier, self).predict_proba(X)
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         hyper_choices = {
             "mdl_optimizer": ["sgd", "rmsprop", "adagrad", "adam", "nadam"]
         }
         hyper_space = {
-            "mdl_dense_width":
-            hp.quniform("mdl_dense_width", 2, 100, 1),
-            "mdl_epochs":
-            hp.quniform("mdl_epochs", 20, 60, 1),
-            "mdl_optimizer":
-            hp.choice("mdl_optimizer", hyper_choices["mdl_optimizer"]),
-            "mdl_learn_rate":
-            hp.lognormal("mdl_learn_rate", 0, 1),
-            "mdl_class_weight":
-            hp.lognormal("mdl_class_weight", 3, 1),
-            "mdl_regularization":
-            hp.lognormal("mdl_regularization", -4, 2),
+            "mdl_dense_width": hp.quniform("mdl_dense_width", 2, 100, 1),
+            "mdl_epochs": hp.quniform("mdl_epochs", 20, 60, 1),
+            "mdl_optimizer": hp.choice("mdl_optimizer", hyper_choices["mdl_optimizer"]),
+            "mdl_learn_rate": hp.lognormal("mdl_learn_rate", 0, 1),
+            "mdl_class_weight": hp.lognormal("mdl_class_weight", 3, 1),
+            "mdl_regularization": hp.lognormal("mdl_regularization", -4, 2),
         }
         return hyper_space, hyper_choices
 
 
-def _create_dense_nn_model(vector_size=40,
-                           dense_width=128,
-                           optimizer='rmsprop',
-                           learn_rate_mult=1.0,
-                           regularization=0.01,
-                           verbose=1):
+def _create_dense_nn_model(
+    vector_size=40,
+    dense_width=128,
+    optimizer="rmsprop",
+    learn_rate_mult=1.0,
+    regularization=0.01,
+    verbose=1,
+):
     """Return callable lstm model.
 
     Returns
     -------
     callable:
         A function that return the Keras Sklearn model when
         called.
@@ -186,36 +191,37 @@
 
         model.add(
             Dense(
                 dense_width,
                 input_dim=vector_size,
                 kernel_regularizer=regularizers.l2(regularization),
                 activity_regularizer=regularizers.l1(regularization),
-                activation='relu',
-            ))
+                activation="relu",
+            )
+        )
 
         # add Dense layer with relu activation
         model.add(
             Dense(
                 dense_width,
                 kernel_regularizer=regularizers.l2(regularization),
                 activity_regularizer=regularizers.l1(regularization),
-                activation='relu',
-            ))
+                activation="relu",
+            )
+        )
 
         # add Dense layer
-        model.add(Dense(1, activation='sigmoid'))
+        model.add(Dense(1, activation="sigmoid"))
 
         optimizer_fn = _get_optimizer(optimizer, learn_rate_mult)
 
         # Compile model
         model.compile(
-            loss='binary_crossentropy',
-            optimizer=optimizer_fn,
-            metrics=['acc'])
+            loss="binary_crossentropy", optimizer=optimizer_fn, metrics=["acc"]
+        )
 
         if verbose >= 1:
             model.summary()
 
         return model
 
     return model_wrapper
```

### Comparing `asreview-1.2.1/asreview/models/classifiers/rf.py` & `asreview-1.3a0/asreview/models/classifiers/rf.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,37 +34,37 @@
     class_weight: float, default=1.0
         Class weight of the inclusions.
     random_state : int or RandomState, default=None
         Controls both the randomness of the bootstrapping of the samples used
         when building trees and the sampling of the features to consider when
         looking for the best split at each node.
     """
+
     name = "rf"
     label = "Random forest"
 
-    def __init__(self,
-                 n_estimators=100,
-                 max_features=10,
-                 class_weight=1.0,
-                 random_state=None):
-
+    def __init__(
+        self, n_estimators=100, max_features=10, class_weight=1.0, random_state=None
+    ):
         super(RandomForestClassifier, self).__init__()
         self.n_estimators = int(n_estimators)
         self.max_features = int(max_features)
         self.class_weight = class_weight
         self._random_state = random_state
 
         self._model = SKRandomForestClassifier(
             n_estimators=self.n_estimators,
             max_features=self.max_features,
             class_weight=_set_class_weight(class_weight),
-            random_state=random_state)
+            random_state=random_state,
+        )
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         hyper_choices = {}
         hyper_space = {
             "mdl_n_estimators": hp.quniform("mdl_n_estimators", 10, 100, 1),
             "mdl_max_features": hp.quniform("mdl_max_features", 6, 10, 1),
-            "mdl_class_weight": hp.lognormal('mdl_class_weight', 0, 1),
+            "mdl_class_weight": hp.lognormal("mdl_class_weight", 0, 1),
         }
         return hyper_space, hyper_choices
```

### Comparing `asreview-1.2.1/asreview/models/classifiers/svm.py` & `asreview-1.3a0/asreview/models/classifiers/svm.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,42 +38,46 @@
     random_state: int, RandomState
         State of the RNG.
     """
 
     name = "svm"
     label = "Support vector machine"
 
-    def __init__(self,
-                 gamma="auto",
-                 class_weight=0.249,
-                 C=15.4,
-                 kernel="linear",
-                 random_state=None):
+    def __init__(
+        self,
+        gamma="auto",
+        class_weight=0.249,
+        C=15.4,
+        kernel="linear",
+        random_state=None,
+    ):
         super(SVMClassifier, self).__init__()
         self.gamma = gamma
         self.class_weight = class_weight
         self.C = C
         self.kernel = kernel
         self._random_state = random_state
 
         self._model = SVC(
             kernel=kernel,
             C=C,
             class_weight=_set_class_weight(class_weight),
             random_state=random_state,
             gamma=gamma,
-            probability=True)
+            probability=True,
+        )
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         hyper_choices = {
             "mdl_gamma": ["auto", "scale"],
-            "mdl_kernel": ["linear", "rbf", "poly", "sigmoid"]
+            "mdl_kernel": ["linear", "rbf", "poly", "sigmoid"],
         }
 
         hyper_space = {
-            "mdl_gamma": hp.choice('mdl_gamma', hyper_choices["mdl_gamma"]),
-            "mdl_kernel": hp.choice('mdl_kernel', hyper_choices["mdl_kernel"]),
-            "mdl_C": hp.lognormal('mdl_C', 0, 2),
-            "mdl_class_weight": hp.lognormal('mdl_class_weight', 0, 1)
+            "mdl_gamma": hp.choice("mdl_gamma", hyper_choices["mdl_gamma"]),
+            "mdl_kernel": hp.choice("mdl_kernel", hyper_choices["mdl_kernel"]),
+            "mdl_C": hp.lognormal("mdl_C", 0, 2),
+            "mdl_class_weight": hp.lognormal("mdl_class_weight", 0, 1),
         }
         return hyper_space, hyper_choices
```

### Comparing `asreview-1.2.1/asreview/models/classifiers/utils.py` & `asreview-1.3a0/asreview/models/classifiers/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/feature_extraction/__init__.py` & `asreview-1.3a0/asreview/models/feature_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/feature_extraction/base.py` & `asreview-1.3a0/asreview/models/feature_extraction/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from scipy.sparse import issparse
 
 from asreview.models.base import BaseModel
 
 
 class BaseFeatureExtraction(BaseModel):
     """Base class for feature extraction methods."""
+
     name = "base-feature"
 
     def __init__(self, split_ta=0, use_keywords=0):
         self.split_ta = split_ta
         self.use_keywords = use_keywords
 
     def fit_transform(self, texts, titles=None, abstracts=None, keywords=None):
@@ -41,16 +42,17 @@
         -------
         numpy.ndarray
             Feature matrix representing the texts.
         """
         self.fit(texts)
         if self.split_ta > 0:
             if titles is None or abstracts is None:
-                raise ValueError("Error: if splitting titles and abstracts,"
-                                 " supply them!")
+                raise ValueError(
+                    "Error: if splitting titles and abstracts," " supply them!"
+                )
             X_titles = self.transform(titles)
             X_abstracts = self.transform(abstracts)
             if issparse(X_titles) and issparse(X_abstracts):
                 X = hstack([X_titles, X_abstracts]).tocsr()
             else:
                 X = np.concatenate((X_titles, X_abstracts), axis=1)
         else:
@@ -93,13 +95,14 @@
         numpy.ndarray
             Feature matrix representing the texts.
         """
         raise NotImplementedError
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         hyper_choices = {}
         hyper_space = {
             "fex_split_ta": hp.randint("fex_split_ta", 2),
             "fex_use_keywords": hp.randint("fex_use_keywords", 2),
         }
         return hyper_space, hyper_choices
```

### Comparing `asreview-1.2.1/asreview/models/feature_extraction/doc2vec.py` & `asreview-1.3a0/asreview/models/feature_extraction/doc2vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,28 @@
 
 import numpy as np
 
 try:
     from gensim.models.doc2vec import Doc2Vec as GenSimDoc2Vec
     from gensim.models.doc2vec import TaggedDocument
     from gensim.utils import simple_preprocess
+
     GENSIM_AVAILABLE = True
 except ImportError:
     GENSIM_AVAILABLE = False
 
 from asreview.models.feature_extraction.base import BaseFeatureExtraction
 
 
 def _check_gensim():
     if not GENSIM_AVAILABLE:
-        raise ImportError(
-            "Install gensim package to use"
-            " Doc2Vec.")
+        raise ImportError("Install gensim package to use" " Doc2Vec.")
 
 
 def _train_model(corpus, *args, **kwargs):
-
     model = GenSimDoc2Vec(*args, **kwargs)
     model.build_vocab(corpus)
     model.train(corpus, total_examples=model.corpus_count, epochs=model.epochs)
     return model
 
 
 def _transform_text(model, corpus):
@@ -89,25 +87,27 @@
     dbow_words: int
         Whether to train the word vectors using the skipgram method.
     """
 
     name = "doc2vec"
     label = "Doc2Vec"
 
-    def __init__(self,
-                 *args,
-                 vector_size=40,
-                 epochs=33,
-                 min_count=1,
-                 n_jobs=1,
-                 window=7,
-                 dm_concat=0,
-                 dm=2,
-                 dbow_words=0,
-                 **kwargs):
+    def __init__(
+        self,
+        *args,
+        vector_size=40,
+        epochs=33,
+        min_count=1,
+        n_jobs=1,
+        window=7,
+        dm_concat=0,
+        dm=2,
+        dbow_words=0,
+        **kwargs
+    ):
         """Initialize the doc2vec model."""
         super(Doc2Vec, self).__init__(*args, **kwargs)
         self.vector_size = int(vector_size)
         self.epochs = int(epochs)
         self.min_count = int(min_count)
         self.n_jobs = int(n_jobs)
         self.window = int(window)
@@ -115,76 +115,68 @@
         self.dm = int(dm)
         self.dbow_words = int(dbow_words)
         self._model = None
         self._model_dm = None
         self._model_dbow = None
 
     def fit(self, texts):
-
         # check is gensim is available
         _check_gensim()
 
         model_param = {
             "vector_size": self.vector_size,
             "epochs": self.epochs,
             "min_count": self.min_count,
             "workers": self.n_jobs,
             "window": self.window,
             "dm_concat": self.dm_concat,
             "dbow_words": self.dbow_words,
         }
 
         corpus = [
-            TaggedDocument(simple_preprocess(text), [i])
-            for i, text in enumerate(texts)
+            TaggedDocument(simple_preprocess(text), [i]) for i, text in enumerate(texts)
         ]
 
         # If self.dm is 2, train both models and concatenate the feature
         # vectors later. Resulting vector size should be the same.
         if self.dm == 2:
             model_param["vector_size"] = int(model_param["vector_size"] / 2)
             self.model_dm = _train_model(corpus, **model_param, dm=1)
             self.model_dbow = _train_model(corpus, **model_param, dm=0)
         else:
             self.model = _train_model(corpus, **model_param, dm=self.dm)
 
     def transform(self, texts):
-
         # check is gensim is available
         _check_gensim()
 
         corpus = [
-            TaggedDocument(simple_preprocess(text), [i])
-            for i, text in enumerate(texts)
+            TaggedDocument(simple_preprocess(text), [i]) for i, text in enumerate(texts)
         ]
 
         if self.dm == 2:
             X_dm = _transform_text(self.model_dm, corpus)
             X_dbow = _transform_text(self.model_dbow, corpus)
             X = np.concatenate((X_dm, X_dbow), axis=1)
         else:
             X = _transform_text(self.model, corpus)
         return X
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         eps = 1e-7
 
         hyper_space, hyper_choices = super(Doc2Vec, self).full_hyper_space()
-        hyper_space.update({
-            "fex_vector_size":
-            hp.quniform("fex_vector_size", 31.5, 127.5 - eps, 8),
-            "fex_epochs":
-            hp.quniform("fex_epochs", 20, 50, 1),
-            "fex_min_count":
-            hp.quniform("fex_min_count", 0.5, 2.499999, 1),
-            "fex_window":
-            hp.quniform("fex_window", 4.5, 9.4999999, 1),
-            "fex_dm_concat":
-            hp.randint("fex_dm_concat", 2),
-            "fex_dm":
-            hp.randint("fex_dm", 3),
-            "fex_dbow_words":
-            hp.randint("fex_dbow_words", 2),
-        })
+        hyper_space.update(
+            {
+                "fex_vector_size": hp.quniform("fex_vector_size", 31.5, 127.5 - eps, 8),
+                "fex_epochs": hp.quniform("fex_epochs", 20, 50, 1),
+                "fex_min_count": hp.quniform("fex_min_count", 0.5, 2.499999, 1),
+                "fex_window": hp.quniform("fex_window", 4.5, 9.4999999, 1),
+                "fex_dm_concat": hp.randint("fex_dm_concat", 2),
+                "fex_dm": hp.randint("fex_dm", 3),
+                "fex_dbow_words": hp.randint("fex_dbow_words", 2),
+            }
+        )
 
         return hyper_space, hyper_choices
```

### Comparing `asreview-1.2.1/asreview/models/feature_extraction/embedding_idf.py` & `asreview-1.3a0/asreview/models/feature_extraction/embedding_idf.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,17 +33,15 @@
 from asreview.models.feature_extraction.base import BaseFeatureExtraction
 from asreview.models.feature_extraction.embedding_lstm import load_embedding
 from asreview.utils import get_random_state
 
 
 def _check_tensorflow():
     if not TF_AVAILABLE:
-        raise ImportError(
-            "Install tensorflow package to use"
-            " Embedding IDF.")
+        raise ImportError("Install tensorflow package to use" " Embedding IDF.")
 
 
 class EmbeddingIdf(BaseFeatureExtraction):
     """Embedding IDF feature extraction technique (``embedding-idf``).
 
     This model averages the weighted word vectors of all the words in the
     text, in order to get a single feature vector for each text. The weights
@@ -69,28 +67,25 @@
         """Initialize the Embedding-Idf model."""
         super(EmbeddingIdf, self).__init__(*args, **kwargs)
         self.embedding_fp = embedding_fp
         self.embedding = None
         self._random_state = get_random_state(random_state)
 
     def transform(self, texts):
-
         # check is tensorflow is available
         _check_tensorflow()
 
         if self.embedding is None:
             if self.embedding_fp is None:
-                raise ValueError(
-                    "Error: need embedding to train Embeddingdf model.")
+                raise ValueError("Error: need embedding to train Embeddingdf model.")
             self.embedding = load_embedding(self.embedding_fp, n_jobs=-1)
 
         text_counts = _get_freq_dict(texts)
         idf = _get_idf(text_counts)
-        X = _get_X_from_dict(text_counts, idf, self.embedding,
-                             self._random_state)
+        X = _get_X_from_dict(text_counts, idf, self.embedding, self._random_state)
         return X
 
 
 def _get_freq_dict(all_text):
     text_dicts = []
     for text in all_text:
         cur_dict = {}
```

### Comparing `asreview-1.2.1/asreview/models/feature_extraction/embedding_lstm.py` & `asreview-1.3a0/asreview/models/feature_extraction/embedding_lstm.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,15 @@
     TF_AVAILABLE = False
 else:
     TF_AVAILABLE = True
 
 
 def _check_tensorflow():
     if not TF_AVAILABLE:
-        raise ImportError(
-            "Install tensorflow package to use"
-            " Embedding LSTM.")
+        raise ImportError("Install tensorflow package to use" " Embedding LSTM.")
 
 
 class EmbeddingLSTM(BaseFeatureExtraction):
     """Embedding LSTM feature extraction technique (``embedding-lstm``).
 
     Feature extraction technique for
     :class:`asreview.models.classifiers.LSTMBaseClassifier` and
@@ -72,80 +70,78 @@
     n_jobs:
         Number of processors used in reading the embedding matrix.
     """
 
     name = "embedding-lstm"
     label = "Embedding LSTM"
 
-    def __init__(self,
-                 *args,
-                 loop_sequence=1,
-                 num_words=20000,
-                 max_sequence_length=1000,
-                 padding='post',
-                 truncating='post',
-                 n_jobs=1,
-                 **kwargs):
+    def __init__(
+        self,
+        *args,
+        loop_sequence=1,
+        num_words=20000,
+        max_sequence_length=1000,
+        padding="post",
+        truncating="post",
+        n_jobs=1,
+        **kwargs,
+    ):
         """Initialize the embedding matrix feature extraction."""
         super(EmbeddingLSTM, self).__init__(*args, **kwargs)
         self.embedding = None
         self.num_words = num_words
         self.max_sequence_length = max_sequence_length
         self.padding = padding
         self.truncating = truncating
         self.n_jobs = n_jobs
         self.loop_sequence = loop_sequence
 
     def transform(self, texts):
-
         _check_tensorflow()
 
         self.X, self.word_index = text_to_features(
             texts,
             loop_sequence=self.loop_sequence,
             num_words=self.num_words,
             max_sequence_length=self.max_sequence_length,
             padding=self.padding,
-            truncating=self.truncating)
+            truncating=self.truncating,
+        )
         return self.X
 
     def get_embedding_matrix(self, texts, embedding_fp):
-
         _check_tensorflow()
 
         self.fit_transform(texts)
         if embedding_fp is None:
-            embedding_fp = Path(get_data_home(),
-                                EMBEDDING_EN["name"]).expanduser()
+            embedding_fp = Path(get_data_home(), EMBEDDING_EN["name"]).expanduser()
 
             if not embedding_fp.exists():
-                logging.warning("Warning: will start to download large "
-                                "embedding file in 10 seconds.")
+                logging.warning(
+                    "Warning: will start to download large "
+                    "embedding file in 10 seconds."
+                )
                 time.sleep(10)
                 download_embedding()
-        logging.info("Loading embedding matrix. "
-                     "This can take several minutes.")
+        logging.info("Loading embedding matrix. " "This can take several minutes.")
 
         embedding = load_embedding(embedding_fp, n_jobs=self.n_jobs)
         return sample_embedding(embedding, self.word_index)
 
     def full_hyper_space(self):
         from hyperopt import hp
 
-        hyper_space, hyper_choices = super(EmbeddingLSTM,
-                                           self).full_hyper_space()
-        hyper_space.update(
-            {"fex_loop_sequences": hp.randint("fex_loop_sequences", 2)})
+        hyper_space, hyper_choices = super(EmbeddingLSTM, self).full_hyper_space()
+        hyper_space.update({"fex_loop_sequences": hp.randint("fex_loop_sequences", 2)})
         return hyper_space, hyper_choices
 
 
 EMBEDDING_EN = {
-    "url":
-    "https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/cc.en.300.vec.gz",  # noqa
-    "name": 'fasttext.cc.en.300.vec'
+    "url": "https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/cc.en.300.vec.gz",  # noqa
+    "name": "fasttext.cc.en.300.vec",
 }
 
 
 def loop_sequences(X, max_sequence_length=1000):
     # Loop the sequences instead of padding.
     for i, old_x in enumerate(X):
         nz = max_sequence_length - 1
@@ -157,26 +153,28 @@
         nz += 1
         new_x = old_x.copy()
 
         j = 1
         # Copy the old data to the new matrix.
         while nz * j < max_sequence_length:
             cp_len = min(nz * (j + 1), max_sequence_length) - nz * j
-            new_x[nz * j:nz * j + cp_len] = old_x[0:cp_len]
+            new_x[nz * j : nz * j + cp_len] = old_x[0:cp_len]
             j += 1
         X[i] = new_x
     return X
 
 
-def text_to_features(sequences,
-                     loop_sequence=1,
-                     num_words=20000,
-                     max_sequence_length=1000,
-                     padding='post',
-                     truncating='post'):
+def text_to_features(
+    sequences,
+    loop_sequence=1,
+    num_words=20000,
+    max_sequence_length=1000,
+    padding="post",
+    truncating="post",
+):
     """Convert text data into features.
 
     Arguments
     ---------
     sequences: list, numpy.ndarray, pandas.Series
         The sequences to convert into features.
     num_words: int
@@ -192,45 +190,41 @@
     tokenizer = Tokenizer(num_words=num_words)
     tokenizer.fit_on_texts(sequences)
 
     # tokenize sequences
     tokens = tokenizer.texts_to_sequences(sequences)
 
     # Pad sequences with zeros.
-    x = pad_sequences(tokens,
-                      maxlen=max_sequence_length,
-                      padding=padding,
-                      truncating=truncating)
+    x = pad_sequences(
+        tokens, maxlen=max_sequence_length, padding=padding, truncating=truncating
+    )
 
     if loop_sequence == 1:
         x = loop_sequences(x, max_sequence_length)
     # word index hack. see issue
     # https://github.com/keras-team/keras/issues/8092
-    word_index = {
-        e: i
-        for e, i in tokenizer.word_index.items() if i <= num_words
-    }
+    word_index = {e: i for e, i in tokenizer.word_index.items() if i <= num_words}
 
     return x, word_index
 
 
 def _embedding_reader(filename, input_queue, block_size=1000):
-    """ Process that reads the word embeddings from a file.
+    """Process that reads the word embeddings from a file.
 
     Parameters
     ----------
     filename: str
         File of trained embedding vectors.
     input_queue: Queue
         Queue to store jobs in.
     block_size: int
         Number of lines for each job.
     """
 
-    with open(filename, 'r', encoding='utf-8', newline='\n') as f:
+    with open(filename, "r", encoding="utf-8", newline="\n") as f:
         # Throw away the first line, since we don't care about the dimensions.
         f.readline()
 
         i_line = 0
         buffer = []
         # Read the embedding file line by line.
         for line in f:
@@ -247,15 +241,15 @@
     # Put the string "DONE" in the queue, to ensure that the
     # worker processes finish.
 
     input_queue.put("DONE")
 
 
 def _embedding_worker(input_queue, output_queue, emb_vec_dim, word_index=None):
-    """ Process that reads the word embeddings from a file.
+    """Process that reads the word embeddings from a file.
 
     Parameters
     ----------
     input_queue: Queue
         Queue in which the jobs are submitted.
     output_queue: Queue
         Queue to store the embedding in dictionary form.
@@ -271,27 +265,27 @@
         embedding = {}
         buffer = input_queue.get()
         if buffer == "DONE":
             break
 
         for line in buffer:
             line = line.rstrip()
-            values = line.split(' ')
+            values = line.split(" ")
 
             if len(values) != emb_vec_dim + 1:
                 if not bad_input:
                     print("Error: bad input in embedding vector.")
                 bad_input = True
                 bad_values = values
                 break
 
             word = values[0]
             if word_index is not None and word not in word_index:
                 continue
-            coefs = values[1:emb_vec_dim + 1]
+            coefs = values[1 : emb_vec_dim + 1]
 
             # store the results
             embedding[word] = np.asarray(coefs, dtype=np.float32)
         output_queue.put(embedding)
 
     # We removed the "DONE" from the input queue, so put it back in for
     # the other processes.
@@ -300,15 +294,15 @@
     # Store the results in the output queue
     if bad_input:
         output_queue.put({"ErrorBadInputValues": bad_values})
     output_queue.put("DONE")
 
 
 def _embedding_aggregator(output_queue, n_worker):
-    """ Process that aggregates the results of the workers.
+    """Process that aggregates the results of the workers.
         This should be the main/original process.
 
     Parameters
     ----------
     output_queue: Queue
         This queue is the output queue of the workers.
     n_worker: int
@@ -328,17 +322,17 @@
             num_done += 1
         else:
             embedding.update(new_embedding)
 
     return embedding
 
 
-def download_embedding(url=EMBEDDING_EN['url'],
-                       name=EMBEDDING_EN['name'],
-                       data_home=None):
+def download_embedding(
+    url=EMBEDDING_EN["url"], name=EMBEDDING_EN["name"], data_home=None
+):
     """Download word embedding file.
 
     Download word embedding file, unzip the file and save to the
     file system.
 
     Parameters
     ----------
@@ -353,24 +347,24 @@
     """
 
     if data_home is None:
         data_home = get_data_home()
 
     out_fp = Path(data_home, name)
 
-    logging.info(f'Start downloading: {url}')
+    logging.info(f"Start downloading: {url}")
 
     r = urlopen(url)
     compressed_file = io.BytesIO(r.read())
 
-    logging.info(f'Save embedding to {out_fp}')
+    logging.info(f"Save embedding to {out_fp}")
 
     decompressed_file = gzip.GzipFile(fileobj=compressed_file)
 
-    with open(out_fp, 'wb') as out_file:
+    with open(out_fp, "wb") as out_file:
         for line in decompressed_file:
             out_file.write(line)
 
 
 def load_embedding(fp, word_index=None, n_jobs=None):
     """Load embedding matrix from file.
 
@@ -404,26 +398,28 @@
         n_jobs = 1
     elif n_jobs == -1:
         n_jobs = cpu_count() - 1
 
     input_queue = Queue(queue_size)
     output_queue = Queue()
 
-    with open(fp, 'r', encoding='utf-8', newline='\n') as f:
-        n_words, emb_vec_dim = list(map(int, f.readline().split(' ')))
+    with open(fp, "r", encoding="utf-8", newline="\n") as f:
+        n_words, emb_vec_dim = list(map(int, f.readline().split(" ")))
 
     logging.debug(f"Reading {n_words} vectors with {emb_vec_dim} dimensions.")
 
     worker_procs = []
     p = Process(target=_embedding_reader, args=(fp, input_queue), daemon=True)
     worker_procs.append(p)
     for _ in range(n_jobs):
-        p = Process(target=_embedding_worker,
-                    args=(input_queue, output_queue, emb_vec_dim, word_index),
-                    daemon=True)
+        p = Process(
+            target=_embedding_worker,
+            args=(input_queue, output_queue, emb_vec_dim, word_index),
+            daemon=True,
+        )
         worker_procs.append(p)
 
     # Start workers.
     for proc in worker_procs:
         proc.start()
     embedding = _embedding_aggregator(output_queue, n_jobs)
 
@@ -459,20 +455,21 @@
     (np.ndarray, list):
         The embedding weights strored in a two dimensional
         numpy array and a list with the corresponding words.
     """
 
     n_words, emb_vec_dim = len(word_index), len(next(iter(embedding.values())))
 
-    logging.debug(f"Creating matrix with {n_words} vectors "
-                  f"with dimension {emb_vec_dim}.")
+    logging.debug(
+        f"Creating matrix with {n_words} vectors " f"with dimension {emb_vec_dim}."
+    )
 
     # n+1 because 0 is preserved in the tokenizing process.
     embedding_matrix = np.zeros((n_words + 1, emb_vec_dim))
 
     for word, i in word_index.items():
         coefs = embedding.get(word)
         if coefs is not None:
             embedding_matrix[i] = coefs
-    logging.debug(f'Shape of embedding matrix: {embedding_matrix.shape}')
+    logging.debug(f"Shape of embedding matrix: {embedding_matrix.shape}")
 
     return embedding_matrix
```

### Comparing `asreview-1.2.1/asreview/models/feature_extraction/tfidf.py` & `asreview-1.3a0/asreview/models/feature_extraction/tfidf.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,43 +32,45 @@
     ngram_max: int
         Can use up to ngrams up to ngram_max. For example in the case of
         ngram_max=2, monograms and bigrams could be used.
     stop_words: str
         When set to 'english', use stopwords. If set to None or 'none',
         do not use stop words.
     """
+
     name = "tfidf"
     label = "TF-IDF"
 
     def __init__(self, *args, ngram_max=1, stop_words="english", **kwargs):
-        """Initialize tfidf class.
-        """
+        """Initialize tfidf class."""
         super(Tfidf, self).__init__(*args, **kwargs)
         self.ngram_max = ngram_max
         self.stop_words = stop_words
         if stop_words is None or stop_words.lower() == "none":
             sklearn_stop_words = None
         else:
             sklearn_stop_words = self.stop_words
-        self._model = TfidfVectorizer(ngram_range=(1, ngram_max),
-                                      stop_words=sklearn_stop_words)
+        self._model = TfidfVectorizer(
+            ngram_range=(1, ngram_max), stop_words=sklearn_stop_words
+        )
 
     def fit(self, texts):
         self._model.fit(texts)
 
     def transform(self, texts):
         X = self._model.transform(texts).tocsr()
         return X
 
     def full_hyper_space(self):
         from hyperopt import hp
 
         hyper_space, hyper_choices = super(Tfidf, self).full_hyper_space()
-        hyper_choices.update({
-            "fex_stop_words": ["english", "none"]
-        })
-        hyper_space.update({
-            "fex_ngram_max": hp.uniformint("fex_ngram_max", 1, 3),
-            "fex_stop_words": hp.choice('fex_stop_words',
-                                        hyper_choices["fex_stop_words"]),
-        })
+        hyper_choices.update({"fex_stop_words": ["english", "none"]})
+        hyper_space.update(
+            {
+                "fex_ngram_max": hp.uniformint("fex_ngram_max", 1, 3),
+                "fex_stop_words": hp.choice(
+                    "fex_stop_words", hyper_choices["fex_stop_words"]
+                ),
+            }
+        )
         return hyper_space, hyper_choices
```

### Comparing `asreview-1.2.1/asreview/models/feature_extraction/utils.py` & `asreview-1.3a0/asreview/models/feature_extraction/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/query/__init__.py` & `asreview-1.3a0/asreview/models/query/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/query/base.py` & `asreview-1.3a0/asreview/models/query/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,15 @@
 
 class BaseQueryStrategy(BaseModel):
     """Abstract class for query strategies."""
 
     name = "base-query"
 
     @abstractmethod
-    def query(self,
-              X,
-              classifier=None,
-              n_instances=None,
-              **kwargs):
+    def query(self, X, classifier=None, n_instances=None, **kwargs):
         """Query new instances.
 
         Arguments
         ---------
         X: numpy.ndarray
             Feature matrix to choose samples from.
         classifier: SKLearnModel
@@ -50,16 +46,15 @@
         raise NotImplementedError
 
 
 class ProbaQueryStrategy(BaseQueryStrategy):
     name = "proba"
 
     def query(self, X, classifier, n_instances=None, **kwargs):
-        """Query method for strategies which use class probabilities.
-        """
+        """Query method for strategies which use class probabilities."""
         if n_instances is None:
             n_instances = X.shape[0]
 
         predictions = classifier.predict_proba(X)
 
         query_idx = self._query(predictions, n_instances, X)
```

### Comparing `asreview-1.2.1/asreview/models/query/cluster.py` & `asreview-1.3a0/asreview/models/query/cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,57 +36,52 @@
     random_state: int, RandomState
         State/seed of the RNG.
     """
 
     name = "cluster"
     label = "Clustering"
 
-    def __init__(self,
-                 cluster_size=350,
-                 update_interval=200,
-                 random_state=None):
-        """Initialize the clustering strategy.
-
-        """
+    def __init__(self, cluster_size=350, update_interval=200, random_state=None):
+        """Initialize the clustering strategy."""
         super(ClusterQuery, self).__init__()
         self.cluster_size = cluster_size
         self.update_interval = update_interval
         self.last_update = None
         self.fallback_model = MaxQuery()
         self._random_state = get_random_state(random_state)
 
     def _query(self, predictions, n_instances, X):
         n_samples = X.shape[0]
 
         last_update = self.last_update
-        if (last_update is None or self.update_interval is None or
-                last_update - n_samples >= self.update_interval):
+        if (
+            last_update is None
+            or self.update_interval is None
+            or last_update - n_samples >= self.update_interval
+        ):
             n_clusters = round(n_samples / self.cluster_size)
             if n_clusters <= 1:
-                return self.fallback_model._query(
-                    predictions, n_instances, X)
+                return self.fallback_model._query(predictions, n_instances, X)
             model = KMeans(
-                n_clusters=n_clusters,
-                n_init=1,
-                random_state=self._random_state)
+                n_clusters=n_clusters, n_init=1, random_state=self._random_state
+            )
             self.clusters = model.fit_predict(X)
             self.last_update = n_samples
 
         clusters = {}
         for idx in np.arange(n_samples):
             cluster_id = self.clusters[idx]
             if cluster_id in clusters:
                 clusters[cluster_id].append((idx, predictions[idx, 1]))
             else:
                 clusters[cluster_id] = [(idx, predictions[idx, 1])]
 
         for cluster_id in clusters:
             try:
-                clusters[cluster_id] = sorted(
-                    clusters[cluster_id], key=lambda x: x[1])
+                clusters[cluster_id] = sorted(clusters[cluster_id], key=lambda x: x[1])
             except ValueError:
                 raise
 
         clust_idx = []
         cluster_ids = list(clusters)
         for _ in range(n_instances):
             cluster_id = self._random_state.choice(cluster_ids, 1)[0]
@@ -97,13 +92,13 @@
 
         clust_idx = np.array(clust_idx, dtype=int)
 
         return clust_idx
 
     def full_hyper_space(self):
         from hyperopt import hp
+
         parameter_space = {
-            "qry_cluster_size": hp.quniform('qry_cluster_size', 50, 1000, 1),
-            "qry_update_interval": hp.quniform('qry_update_interval', 100, 300,
-                                               1),
+            "qry_cluster_size": hp.quniform("qry_cluster_size", 50, 1000, 1),
+            "qry_update_interval": hp.quniform("qry_update_interval", 100, 300, 1),
         }
         return parameter_space, {}
```

### Comparing `asreview-1.2.1/asreview/models/query/max.py` & `asreview-1.3a0/asreview/models/query/max.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/query/mixed.py` & `asreview-1.3a0/asreview/models/query/mixed.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,18 @@
 
 from asreview.models.query.base import BaseQueryStrategy
 from asreview.models.query.utils import get_query_model
 from asreview.utils import get_random_state
 
 
 def _parse_mixed_kwargs(kwargs, strategy_name):
-
     kwargs_new = {}
     for key, value in kwargs.items():
         if key.startswith(strategy_name):
-            new_key = key[len(strategy_name) + 1:]
+            new_key = key[len(strategy_name) + 1 :]
             kwargs_new[new_key] = value
 
     return kwargs_new
 
 
 class MixedQuery(BaseQueryStrategy):
     """Mixed query strategy.
@@ -56,20 +55,22 @@
         Seed for the numpy random number generator.
     **kwargs: dict
         Keyword arguments for the two strategy. To specify which of the
         strategies the argument is for, prepend with the name of the query
         strategy and an underscore, e.g. 'max' for maximal sampling.
     """
 
-    def __init__(self,
-                 strategy_1="max",
-                 strategy_2="random",
-                 mix_ratio=0.95,
-                 random_state=None,
-                 **kwargs):
+    def __init__(
+        self,
+        strategy_1="max",
+        strategy_2="random",
+        mix_ratio=0.95,
+        random_state=None,
+        **kwargs
+    ):
         """Initialize the Mixed query strategy."""
         super(MixedQuery, self).__init__()
 
         self.strategy_1 = strategy_1
         self.strategy_2 = strategy_2
 
         self.mix_ratio = mix_ratio
@@ -77,57 +78,51 @@
 
         self.kwargs_1 = _parse_mixed_kwargs(kwargs, strategy_1)
         self.kwargs_2 = _parse_mixed_kwargs(kwargs, strategy_2)
 
         self.query_model1 = get_query_model(strategy_1, **self.kwargs_1)
         if "random_state" in self.query_model1.default_param:
             self.query_model1 = get_query_model(
-                strategy_1, random_state=self._random_state, **self.kwargs_1)
+                strategy_1, random_state=self._random_state, **self.kwargs_1
+            )
 
         self.query_model2 = get_query_model(strategy_2, **self.kwargs_2)
         if "random_state" in self.query_model2.default_param:
             self.query_model2 = get_query_model(
-                strategy_2, random_state=self._random_state, **self.kwargs_2)
+                strategy_2, random_state=self._random_state, **self.kwargs_2
+            )
 
     def query(self, X, classifier, n_instances=None, **kwargs):
-
         # set the number of instances to len(X) if None
         if n_instances is None:
             n_instances = X.shape[0]
 
         # compute the predictions
         predictions = classifier.predict_proba(X)
 
         # Perform the query with strategy 1.
         try:
-            query_idx_1 = self.query_model1._query(
-                predictions,
-                n_instances=n_instances)
+            query_idx_1 = self.query_model1._query(predictions, n_instances=n_instances)
         except AttributeError:
             # for random for example
-            query_idx_1 = self.query_model1.query(
-                X, classifier, n_instances)
+            query_idx_1 = self.query_model1.query(X, classifier, n_instances)
 
         # Perform the query with strategy 2.
         try:
-            query_idx_2 = self.query_model2._query(
-                predictions,
-                n_instances=n_instances)
+            query_idx_2 = self.query_model2._query(predictions, n_instances=n_instances)
         except AttributeError:
             # for random for example
-            query_idx_2 = self.query_model2.query(
-                X, classifier, n_instances)
+            query_idx_2 = self.query_model2.query(X, classifier, n_instances)
 
         # mix the 2 query strategies into one list
         query_idx_mix = []
         i = 0
         j = 0
 
         while i < len(query_idx_1) and j < len(query_idx_2):
-
             if self._random_state.rand() < self.mix_ratio:
                 query_idx_mix.append(query_idx_1[i])
                 i = i + 1
             else:
                 query_idx_mix.append(query_idx_2[j])
                 j = j + 1
 
@@ -168,43 +163,39 @@
     query strategy after which the remaining 5% would be sampled with
     the random query strategy.
     """
 
     name = "max_random"
     label = "Mixed (95% Maximum and 5% Random)"
 
-    def __init__(self,
-                 mix_ratio=0.95,
-                 random_state=None,
-                 **kwargs):
+    def __init__(self, mix_ratio=0.95, random_state=None, **kwargs):
         """Initialize the Mixed (Maximum and Random) query strategy."""
         super(MaxRandomQuery, self).__init__(
             strategy_1="max",
             strategy_2="random",
             mix_ratio=mix_ratio,
             random_state=random_state,
-            **kwargs)
+            **kwargs
+        )
 
 
 class MaxUncertaintyQuery(MixedQuery):
     """Mixed (95% Maximum and 5% Uncertainty) query strategy (``max_uncertainty``).
 
     A mix of maximum and random query strategies with a mix ratio of 0.95.
     At each query 95% of the instances would be sampled with the maximum
     query strategy after which the remaining 5% would be sampled with
     the uncertainty query strategy.
     """
 
     name = "max_uncertainty"
     label = "Mixed (95% Maximum and 5% Uncertainty)"
 
-    def __init__(self,
-                 mix_ratio=0.95,
-                 random_state=None,
-                 **kwargs):
+    def __init__(self, mix_ratio=0.95, random_state=None, **kwargs):
         """Initialize the Mixed (Maximum and Uncertainty) query strategy."""
         super(MaxUncertaintyQuery, self).__init__(
             strategy_1="max",
             strategy_2="uncertainty",
             mix_ratio=mix_ratio,
             random_state=random_state,
-            **kwargs)
+            **kwargs
+        )
```

### Comparing `asreview-1.2.1/asreview/models/query/random.py` & `asreview-1.3a0/asreview/models/query/random.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,22 +25,24 @@
     Randomly select samples with no regard to model assigned probabilities.
 
     .. warning::
         Selecting this option means your review is not going to be
         accelerated by ASReview.
 
     """
+
     name = "random"
     label = "Random"
 
     def __init__(self, random_state=None):
         super(RandomQuery, self).__init__()
         self._random_state = get_random_state(random_state)
 
     def query(self, X, classifier=None, n_instances=None, **kwargs):
         if n_instances is None:
             n_instances = X.shape[0]
 
         query_idx = self._random_state.choice(
-            np.arange(X.shape[0]), n_instances, replace=False)
+            np.arange(X.shape[0]), n_instances, replace=False
+        )
 
         return query_idx
```

### Comparing `asreview-1.2.1/asreview/models/query/uncertainty.py` & `asreview-1.3a0/asreview/models/query/uncertainty.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/models/query/utils.py` & `asreview-1.3a0/asreview/models/query/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,15 @@
     -------
     class
         Class corresponding to the name name.
     """
 
     # Try to split the query strategy if the string wasn't found.
     try:
-        return _model_class_from_entry_point(
-            name,
-            entry_name="asreview.models.query")
+        return _model_class_from_entry_point(name, entry_name="asreview.models.query")
     except ValueError:
         raise ValueError(f"Error: query name '{name}' is not implemented.")
 
 
 def get_query_model(name, *args, random_state=None, **kwargs):
     """Get an instance of the query strategy.
```

### Comparing `asreview-1.2.1/asreview/project.py` & `asreview-1.3a0/asreview/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,116 +21,120 @@
 import zipfile
 from contextlib import contextmanager
 from datetime import datetime
 from functools import wraps
 from pathlib import Path
 from uuid import uuid4
 
-from filelock import FileLock
 import jsonschema
 import numpy as np
+from filelock import FileLock
 from scipy.sparse import csr_matrix
 from scipy.sparse import load_npz
 from scipy.sparse import save_npz
 
 from asreview._version import get_versions
 from asreview.config import LABEL_NA
-from asreview.config import PROJECT_MODES
 from asreview.config import PROJECT_MODE_SIMULATE
+from asreview.config import PROJECT_MODES
 from asreview.config import SCHEMA
+from asreview.data import ASReviewData
 from asreview.state.errors import StateNotFoundError
 from asreview.state.sqlstate import SQLiteState
 from asreview.utils import asreview_path
-from asreview.webapp.io import read_data
 
 PATH_PROJECT_CONFIG = "project.json"
 PATH_PROJECT_CONFIG_LOCK = "project.json.lock"
-PATH_FEATURE_MATRICES = 'feature_matrices'
+PATH_FEATURE_MATRICES = "feature_matrices"
 
 
 class ProjectError(Exception):
     pass
 
 
 class ProjectExistsError(Exception):
     pass
 
 
 class ProjectNotFoundError(Exception):
     pass
 
 
-def get_project_path(project_id, asreview_dir=None):
+def get_project_path(folder_id):
     """Get the project directory.
 
     Arguments
     ---------
-    project_id: str
-        The id of the current project.
+    folder_id: str
+        The id of the folder containing a project. If there is no
+        authentication, the folder_id is equal to the project_id. Otherwise,
+        this is equal to {project_owner_id}_{project_id}.
     """
-
-    if asreview_dir is None:
-        asreview_dir = asreview_path()
-
-    return Path(asreview_dir, project_id)
+    return Path(asreview_path(), folder_id)
 
 
 def project_from_id(f):
+    """Decorator function that takes a user account as parameter,
+    the user account is used to get the correct sub folder in which
+    the projects is
+    """
 
     @wraps(f)
     def decorated_function(project_id, *args, **kwargs):
-
         project_path = get_project_path(project_id)
+        if not is_project(project_path):
+            raise ProjectNotFoundError(f"Project '{project_id}' not found")
         project = ASReviewProject(project_path, project_id=project_id)
         return f(project, *args, **kwargs)
 
     return decorated_function
 
 
-def list_asreview_projects():
-    """List the projects in the asreview path"""
+def get_projects(project_paths=None):
+    """Get the ASReview projects at the given paths.
 
-    file_list = []
-    for x in asreview_path().iterdir():
-        if x.is_dir():
-            try:
-                project = ASReviewProject(x)
-                project.project_id = project.config["id"]
-                file_list.append(project)
-            except Exception:
-                pass
-    return file_list
+    Arguments
+    ---------
+    project_paths : list[Path], optional
+        List of paths to projects. By default all the projects in the asreview
+        folder are used, by default None
+
+    Returns
+    -------
+    list[ASReviewProject]
+        Projects at the given project paths.
+    """
+    if project_paths is None:
+        project_paths = [path for path in asreview_path().iterdir() if path.is_dir()]
+
+    return [ASReviewProject(project_path) for project_path in project_paths]
 
 
 def _create_project_id(name):
     """Create project id from input name."""
 
-    if isinstance(name, str) \
-            and len(name) > 0 \
-            and not name[0].isalnum():
-        raise ValueError("First character should be alphabet"
-                         " letter (a-z) or number (0-9).")
-
-    if not name \
-            and not isinstance(name, str) \
-            and len(name) >= 3:
+    if isinstance(name, str) and len(name) > 0 and not name[0].isalnum():
+        raise ValueError(
+            "First character should be alphabet" " letter (a-z) or number (0-9)."
+        )
+
+    if not name and not isinstance(name, str) and len(name) >= 3:
         raise ValueError("Project name should be at least 3 characters.")
 
     project_id = ""
     for c in name.lower():
         if c.isalnum():
             project_id += c
         elif len(project_id) > 0 and project_id[-1] != "-":
             project_id += "-"
 
     return project_id
 
 
 def is_project(project_path):
-
     project_path = Path(project_path) / PATH_PROJECT_CONFIG
 
     return project_path.exists()
 
 
 def is_v0_project(project_path):
     """Check if a project file is of a ASReview version 0 project."""
@@ -156,107 +160,106 @@
     -------
     SQLiteState
     """
 
     # Unzip the ASReview data if needed.
     if isinstance(asreview_obj, ASReviewProject):
         project = asreview_obj
-    elif zipfile.is_zipfile(asreview_obj) and Path(
-            asreview_obj).suffix == ".asreview":
-
+    elif zipfile.is_zipfile(asreview_obj) and Path(asreview_obj).suffix == ".asreview":
         if not read_only:
-            raise ValueError(
-                "ASReview files do not support not read only files.")
+            raise ValueError("ASReview files do not support not read only files.")
 
         # work from a temp dir
         tmpdir = tempfile.TemporaryDirectory()
         project = ASReviewProject.load(asreview_obj, tmpdir.name)
     else:
         project = ASReviewProject(asreview_obj)
 
     # init state class
     state = SQLiteState(read_only=read_only)
 
     try:
         if len(project.reviews) > 0:
             if review_id is None:
-                review_id = project.config['reviews'][0]['id']
+                review_id = project.config["reviews"][0]["id"]
             logging.debug(f"Opening review {review_id}.")
             state._restore(project.project_path, review_id)
         elif len(project.reviews) == 0 and not read_only:
             review_id = uuid4().hex
             logging.debug(f"Create new review (state) with id {review_id}.")
             state._create_new_state_file(project.project_path, review_id)
             project.add_review(review_id)
         else:
-            raise StateNotFoundError("State file does not exist, and in "
-                                     "read only mode.")
+            raise StateNotFoundError(
+                "State file does not exist, and in " "read only mode."
+            )
         yield state
     finally:
         try:
             state.close()
         except AttributeError:
             # file seems to be closed, do nothing
             pass
 
 
-class ASReviewProject():
+class ASReviewProject:
     """Project class for ASReview project files."""
 
     def __init__(self, project_path, project_id=None):
         self.project_path = Path(project_path)
         self.project_id = project_id
 
     @classmethod
-    def create(cls,
-               project_path,
-               project_id=None,
-               project_mode="oracle",
-               project_name=None,
-               project_description=None,
-               project_authors=None):
+    def create(
+        cls,
+        project_path,
+        project_id=None,
+        project_mode="oracle",
+        project_name=None,
+        project_description=None,
+        project_authors=None,
+    ):
         """Initialize the necessary files specific to the web app."""
 
         project_path = Path(project_path)
 
         if is_project(project_path):
             raise ProjectExistsError("Project already exists.")
 
         if project_mode not in PROJECT_MODES:
-            raise ValueError(f"Project mode '{project_mode}' is not in "
-                             f"{PROJECT_MODES}.")
+            raise ValueError(
+                f"Project mode '{project_mode}' is not in " f"{PROJECT_MODES}."
+            )
 
         if project_id is None:
             project_id = project_path.stem
 
         if project_name is None:
             project_name = project_path.stem
 
         if project_path.is_dir():
-            raise IsADirectoryError(
-                f'Project folder {project_path} already exists.')
+            raise IsADirectoryError(f"Project folder {project_path} already exists.")
 
         try:
-            project_path.mkdir(exist_ok=True)
+            project_path.mkdir(parents=True, exist_ok=True)
             Path(project_path, "data").mkdir(exist_ok=True)
             Path(project_path, PATH_FEATURE_MATRICES).mkdir(exist_ok=True)
             Path(project_path, "reviews").mkdir(exist_ok=True)
 
             config = {
-                'version':
-                get_versions()['version'],
-                'id': project_id,
-                'mode': project_mode,
-                'name': project_name,
-                'description': project_description,
-                'authors': project_authors,
-                'created_at_unix': int(time.time()),
-                'datetimeCreated': str(datetime.now()),
-                'reviews': [],
-                'feature_matrices': []
+                "version": get_versions()["version"],
+                "id": project_id,
+                "mode": project_mode,
+                "name": project_name,
+                "description": project_description,
+                "authors": project_authors,
+                "created_at_unix": int(time.time()),
+                "datetimeCreated": str(datetime.now()),
+                "reviews": [],
+                "feature_matrices": [],
             }
 
             # validate new config before storing
             jsonschema.validate(instance=config, schema=SCHEMA)
 
             project_fp = Path(project_path, PATH_PROJECT_CONFIG)
             project_fp_lock = Path(project_path, PATH_PROJECT_CONFIG_LOCK)
@@ -272,42 +275,35 @@
             shutil.rmtree(project_path)
             raise err
 
         return cls(project_path, project_id=project_id)
 
     @property
     def config(self):
-
         try:
             return self._config
         except AttributeError:
-
             project_fp = Path(self.project_path, PATH_PROJECT_CONFIG)
             project_fp_lock = Path(self.project_path, PATH_PROJECT_CONFIG_LOCK)
             lock = FileLock(project_fp_lock, timeout=3)
 
             try:
-
                 with lock:
-
                     # read the file with project info
                     with open(project_fp, "r") as fp:
-
                         config = json.load(fp)
                         self._config = config
 
                         return config
 
             except FileNotFoundError:
-                raise ProjectNotFoundError(
-                    f"Project '{self.project_path}' not found")
+                raise ProjectNotFoundError(f"Project '{self.project_path}' not found")
 
     @config.setter
     def config(self, config):
-
         project_fp = Path(self.project_path, PATH_PROJECT_CONFIG)
         project_fp_lock = Path(self.project_path, PATH_PROJECT_CONFIG_LOCK)
         lock = FileLock(project_fp_lock, timeout=3)
 
         with lock:
             with open(project_fp, "w") as f:
                 json.dump(config, f)
@@ -323,119 +319,114 @@
             del kwargs_copy["name"]
             logging.info(
                 "Update project name is ignored, use 'rename_project' function."
             )
 
         # validate schema
         if "mode" in kwargs_copy and kwargs_copy["mode"] not in PROJECT_MODES:
-            raise ValueError("Project mode '{}' not found.".format(
-                kwargs_copy["mode"]))
+            raise ValueError("Project mode '{}' not found.".format(kwargs_copy["mode"]))
 
         # update project file
         config = self.config
         config.update(kwargs_copy)
 
         # validate new config before storing
         jsonschema.validate(instance=config, schema=SCHEMA)
 
         self.config = config
         return config
 
-    def rename(self, project_name_new):
+    def rename(self, new_project_data={}):
         """Rename a project id.
 
         This function only works for projects in ASReview LAB  web interface.
         This is the result of the file storage in
         asreview.webapp.utils.project_path.asreview_path.
 
         Arguments
         ---------
-        project_id: str
-            The current project_id.
-        project_name_new: str
-            The new project name to be converted into a new
-            project_id.
+        new_project_data: dict
+            Dictionary that contains a new name, id and project path
 
         Returns
         -------
-        str:
-            The new project_id.
+        ASReviewProject:
+            The updated project
         """
+        # get all data
+        new_project_name = new_project_data.get("name", None)
+        new_project_id = new_project_data.get("project_id", None)
+        new_project_path = new_project_data.get("project_path", None)
 
-        # create a new project_id from project name
-        project_id_new = _create_project_id(project_name_new)
-        project_path_new = Path(asreview_path(), project_id_new)
-
-        if (self.project_path == project_path_new):
+        if self.project_id == new_project_id:
             # nothing to do
             return self
 
-        if (self.project_path !=
-                project_path_new) & is_project(project_path_new):
-            raise ValueError(f"Project '{project_path_new}' already exists.")
-
-        self.project_path.rename(project_path_new)
-        self.project_path = project_path_new
-        self.project_id = project_id_new
+        if (self.project_path != new_project_path) and is_project(new_project_path):
+            raise ValueError(f"Project '{new_project_path}' already exists.")
+
+        self.project_path.rename(new_project_path)
+        self.project_path = new_project_path
+        self.project_id = new_project_id
 
         # update the project file
         config = self.config
 
-        config["id"] = project_id_new
-        config["name"] = project_name_new
+        config["id"] = new_project_id
+        config["name"] = new_project_name
 
         self.config = config
         self._config = config
 
         return self
 
     def add_dataset(self, file_name):
         """Add file path to the project file.
 
         Add file to data subfolder and fill the pool of iteration 0.
         """
         self.update_config(dataset_path=file_name)
 
         # fill the pool of the first iteration
-        as_data = read_data(self)
+        fp_data = Path(self.project_path, "data", self.config["dataset_path"])
+        as_data = ASReviewData.from_file(fp_data)
 
         with open_state(self.project_path, read_only=False) as state:
-
             # save the record ids in the state file
             state.add_record_table(as_data.record_ids)
 
             # if the data contains labels, add them to the state file
-            if self.config["mode"] != PROJECT_MODE_SIMULATE and \
-                    as_data.labels is not None:
-
+            if (
+                self.config["mode"] != PROJECT_MODE_SIMULATE
+                and as_data.labels is not None
+            ):
                 labeled_indices = np.where(as_data.labels != LABEL_NA)[0]
                 labels = as_data.labels[labeled_indices].tolist()
-                labeled_record_ids = as_data.record_ids[
-                    labeled_indices].tolist()
+                labeled_record_ids = as_data.record_ids[labeled_indices].tolist()
 
                 # add the labels as prior data
                 state.add_labeling_data(
                     record_ids=labeled_record_ids,
                     labels=labels,
                     notes=[None for _ in labeled_record_ids],
-                    prior=True)
+                    prior=True,
+                )
 
     def remove_dataset(self):
-        """Remove dataset from project.
-
-        """
+        """Remove dataset from project."""
         # reset dataset_path
         self.update_config(dataset_path=None)
 
         # remove datasets from project
         shutil.rmtree(Path(self.project_path, "data"))
 
         # remove state file if present
-        if Path(self.project_path, "reviews").is_dir() and \
-                any(Path(self.project_path, "reviews").iterdir()):
+        if Path(self.project_path, "reviews").is_dir() and any(
+            Path(self.project_path, "reviews").iterdir()
+        ):
             self.delete_review()
 
     def clean_tmp_files(self):
         """Clean temporary files in a project.
 
         Arguments
         ---------
@@ -449,15 +440,15 @@
                 os.remove(f_pickle)
             except OSError as e:
                 print(f"Error: {f_pickle} : {e.strerror}")
 
     @property
     def feature_matrices(self):
         try:
-            return self.config['feature_matrices']
+            return self.config["feature_matrices"]
         except Exception:
             return []
 
     def add_feature_matrix(self, feature_matrix, feature_extraction_method):
         """Add feature matrix to project file.
 
         Arguments
@@ -469,26 +460,29 @@
         """
         # Make sure the feature matrix is in csr format.
         if isinstance(feature_matrix, np.ndarray):
             feature_matrix = csr_matrix(feature_matrix)
         if not isinstance(feature_matrix, csr_matrix):
             raise ValueError(
                 "The feature matrix should be convertible to type "
-                "scipy.sparse.csr.csr_matrix.")
+                "scipy.sparse.csr.csr_matrix."
+            )
 
-        matrix_filename = f'{feature_extraction_method}_feature_matrix.npz'
-        save_npz(Path(self.project_path, PATH_FEATURE_MATRICES,
-                      matrix_filename), feature_matrix)
+        matrix_filename = f"{feature_extraction_method}_feature_matrix.npz"
+        save_npz(
+            Path(self.project_path, PATH_FEATURE_MATRICES, matrix_filename),
+            feature_matrix,
+        )
 
         # Add the feature matrix to the project config.
         config = self.config
 
         feature_matrix_config = {
             "id": feature_extraction_method,
-            "filename": matrix_filename
+            "filename": matrix_filename,
         }
 
         # Add container for feature matrices.
         if "feature_matrices" not in config:
             config["feature_matrices"] = []
 
         config["feature_matrices"].append(feature_matrix_config)
@@ -504,22 +498,21 @@
             Name of the feature extraction method for which to get the matrix.
 
         Returns
         -------
         scipy.sparse.csr_matrix:
             Feature matrix in sparse format.
         """
-        matrix_filename = f'{feature_extraction_method}_feature_matrix.npz'
-        return load_npz(Path(self.project_path, PATH_FEATURE_MATRICES,
-                             matrix_filename))
+        matrix_filename = f"{feature_extraction_method}_feature_matrix.npz"
+        return load_npz(Path(self.project_path, PATH_FEATURE_MATRICES, matrix_filename))
 
     @property
     def reviews(self):
         try:
-            return self.config['reviews']
+            return self.config["reviews"]
         except Exception:
             return []
 
     def add_review(self, review_id, start_time=None, status="setup"):
         """Add new review metadata.
 
         Arguments
@@ -572,97 +565,89 @@
 
         # read the file with project info
         config = self.config
 
         if review_id is None:
             review_index = 0
         else:
-            review_index = [x['id'] for x in self.config['reviews']
-                            ].index(review_id)
+            review_index = [x["id"] for x in self.config["reviews"]].index(review_id)
 
         review_config = config["reviews"][review_index]
         review_config.update(kwargs)
 
         config["reviews"][review_index] = review_config
 
         # update the file with project info
         self.config = config
 
     def delete_review(self, remove_folders=False):
-
         try:
             # remove the folder tree
             shutil.rmtree(Path(self.project_path, PATH_FEATURE_MATRICES))
 
             # recreate folder structure if True
             if not remove_folders:
-                Path(self.project_path,
-                     PATH_FEATURE_MATRICES).mkdir(exist_ok=True)
+                Path(self.project_path, PATH_FEATURE_MATRICES).mkdir(exist_ok=True)
         except Exception:
             print("Failed to remove feature matrices.")
 
         try:
-            path_review = Path(self.project_path, 'reviews')
+            path_review = Path(self.project_path, "reviews")
             shutil.rmtree(path_review)
             if not remove_folders:
-                Path(self.project_path, 'reviews').mkdir(exist_ok=True)
+                Path(self.project_path, "reviews").mkdir(exist_ok=True)
         except Exception:
             print("Failed to remove sql database.")
 
         # update the config
-        self.update_config(**{
-            'reviews': [],
-            'feature_matrices': []
-        })
+        self.update_config(**{"reviews": [], "feature_matrices": []})
 
     def mark_review_finished(self, review_id=None):
         """Mark a review in the project as finished.
 
         If no review_id is given, mark the first review as finished.
 
         Arguments
         ---------
         review_id: str
             Identifier of the review to mark as finished.
         """
 
-        self.update_review(review_id=review_id,
-                           status="finished",
-                           end_time=str(datetime.now()))
+        self.update_review(
+            review_id=review_id, status="finished", end_time=str(datetime.now())
+        )
 
     def export(self, export_fp):
-
         if Path(export_fp).suffix != ".asreview":
             raise ValueError("Export file should have .asreview extension.")
 
         if Path(export_fp) == Path(self.project_path):
-            raise ValueError(
-                "export_fp should not be identical to project path.")
+            raise ValueError("export_fp should not be identical to project path.")
 
         export_fp_tmp = Path(export_fp).with_suffix(".asreview.zip")
 
         # copy the source tree, but ignore pickle files
-        shutil.copytree(self.project_path,
-                        export_fp_tmp,
-                        ignore=shutil.ignore_patterns('*.pickle', '*.lock'))
+        shutil.copytree(
+            self.project_path,
+            export_fp_tmp,
+            ignore=shutil.ignore_patterns("*.pickle", "*.lock"),
+        )
 
         # create the archive
         shutil.make_archive(export_fp_tmp, "zip", root_dir=export_fp_tmp)
 
         # remove the unzipped folder and move zip
         shutil.rmtree(export_fp_tmp)
-        shutil.move(f'{export_fp_tmp}.zip', export_fp)
+        shutil.move(f"{export_fp_tmp}.zip", export_fp)
 
     @classmethod
     def load(cls, asreview_file, project_path, safe_import=False):
-
         tmpdir = tempfile.TemporaryDirectory().name
 
         try:
-
             # Unzip the project file
             with zipfile.ZipFile(asreview_file, "r") as zip_obj:
                 zip_filenames = zip_obj.namelist()
 
                 # raise error if no ASReview project file
                 if PATH_PROJECT_CONFIG not in zip_filenames:
                     raise ValueError("Project file is not valid project.")
@@ -675,53 +660,48 @@
         except zipfile.BadZipFile:
             raise ValueError("File is not an ASReview file.")
 
         with open(Path(tmpdir, PATH_PROJECT_CONFIG), "r") as f:
             project_config = json.load(f)
 
         if safe_import:
-
             # If the uploaded project already exists,
             # then overwrite project.json with a copy suffix.
             while Path(
-                    project_path,
-                    project_config["id"],
-                    PATH_PROJECT_CONFIG
+                project_path, project_config["id"], PATH_PROJECT_CONFIG
             ).exists():
                 # project update
                 project_config["id"] = f"{project_config['id']}-copy"
-                project_config[
-                    "name"] = f"{project_config['name']} copy"
+                project_config["name"] = f"{project_config['name']} copy"
             else:
                 with open(Path(tmpdir, PATH_PROJECT_CONFIG), "r+") as f:
                     # write to file
                     f.seek(0)
                     json.dump(project_config, f)
                     f.truncate()
 
         # location to copy file to
         # Move the project from the temp folder to the projects folder.
         os.replace(tmpdir, Path(project_path, project_config["id"]))
 
         return cls(Path(project_path, project_config["id"]))
 
     def set_error(self, err, save_error_message=True):
-
         err_type = type(err).__name__
         self.update_review(status="error")
 
         # write error to file if label method is prior (first iteration)
         if save_error_message:
             message = {
                 "message": f"{err_type}: {err}",
                 "type": f"{err_type}",
-                "datetime": str(datetime.now())
+                "datetime": str(datetime.now()),
             }
 
-            with open(Path(self.project_path, "error.json"), 'w') as f:
+            with open(Path(self.project_path, "error.json"), "w") as f:
                 json.dump(message, f)
 
     def remove_error(self, status):
         error_path = self.project_path / "error.json"
         if error_path.exists():
             try:
                 os.remove(error_path)
```

### Comparing `asreview-1.2.1/asreview/review/__init__.py` & `asreview-1.3a0/asreview/review/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/review/base.py` & `asreview-1.3a0/asreview/review/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,64 +96,65 @@
             if self.record_table.empty:
                 state.add_record_table(as_data.record_ids)
                 self.record_table = state.get_record_table()
 
             # Retrieve feature matrix from the project file or create
             # one from scratch.
             try:
-                self.X = self.project.get_feature_matrix(
-                    self.feature_extraction.name)
+                self.X = self.project.get_feature_matrix(self.feature_extraction.name)
             except FileNotFoundError:
                 self.X = self.feature_extraction.fit_transform(
-                    as_data.texts,
-                    as_data.headings,
-                    as_data.bodies,
-                    as_data.keywords
+                    as_data.texts, as_data.headings, as_data.bodies, as_data.keywords
                 )
 
                 # check if the number of records after the transform equals
                 # the number of records in the dataset
                 if self.X.shape[0] != len(as_data):
                     raise ValueError(
                         "Dataset has {} records while feature "
-                        "extractor returns {} records"
-                        .format(len(as_data), self.X.shape[0]))
+                        "extractor returns {} records".format(
+                            len(as_data), self.X.shape[0]
+                        )
+                    )
 
-                self.project.add_feature_matrix(self.X,
-                                                self.feature_extraction.name)
+                self.project.add_feature_matrix(self.X, self.feature_extraction.name)
 
             # Check if the number or records in the feature matrix matches the
             # length of the dataset.
             if self.X.shape[0] != len(self.data_labels):
-                raise ValueError("The state file does not correspond to the "
-                                 "given data file, please use another state "
-                                 "file or dataset.")
+                raise ValueError(
+                    "The state file does not correspond to the "
+                    "given data file, please use another state "
+                    "file or dataset."
+                )
 
             # Make sure the priors are labeled.
             self._label_priors()
 
     @property
     def settings(self):
         """Get an ASReview settings object"""
         extra_kwargs = {}
-        if hasattr(self, 'n_prior_included'):
-            extra_kwargs['n_prior_included'] = self.n_prior_included
-        if hasattr(self, 'n_prior_excluded'):
-            extra_kwargs['n_prior_excluded'] = self.n_prior_excluded
-        return ASReviewSettings(model=self.classifier.name,
-                                query_strategy=self.query_strategy.name,
-                                balance_strategy=self.balance_model.name,
-                                feature_extraction=self.feature_extraction.name,
-                                n_instances=self.n_instances,
-                                stop_if=self.stop_if,
-                                model_param=self.classifier.param,
-                                query_param=self.query_strategy.param,
-                                balance_param=self.balance_model.param,
-                                feature_param=self.feature_extraction.param,
-                                **extra_kwargs)
+        if hasattr(self, "n_prior_included"):
+            extra_kwargs["n_prior_included"] = self.n_prior_included
+        if hasattr(self, "n_prior_excluded"):
+            extra_kwargs["n_prior_excluded"] = self.n_prior_excluded
+        return ASReviewSettings(
+            model=self.classifier.name,
+            query_strategy=self.query_strategy.name,
+            balance_strategy=self.balance_model.name,
+            feature_extraction=self.feature_extraction.name,
+            n_instances=self.n_instances,
+            stop_if=self.stop_if,
+            model_param=self.classifier.param,
+            query_param=self.query_strategy.param,
+            balance_param=self.balance_model.param,
+            feature_param=self.feature_extraction.param,
+            **extra_kwargs
+        )
 
     def review(self):
         """Do a full review."""
         # Label any pending records.
 
         with open_state(self.project, read_only=False) as s:
             pending = s.get_pending()
@@ -162,20 +163,20 @@
 
             labels_prior = s.get_labels()
 
         # progress bars
         pbar_rel = tqdm(
             initial=sum(labels_prior),
             total=sum(self.as_data.labels),
-            desc="Relevant records found"
+            desc="Relevant records found",
         )
         pbar_total = tqdm(
             initial=len(labels_prior),
             total=len(self.as_data),
-            desc="Records labeled       "
+            desc="Records labeled       ",
         )
 
         # While the stopping condition has not been met:
         while not self._stop_review():
             # Train a new model.
             self.train()
 
@@ -195,16 +196,17 @@
             pbar_total.close()
             self._write_to_state()
 
     def _label_priors(self):
         """Make sure the prior records are labeled."""
         with open_state(self.project, read_only=False) as state:
             labeled = state.get_labeled()
-            unlabeled_priors = [x for x in self.prior_indices
-                                if x not in labeled['record_id'].to_list()]
+            unlabeled_priors = [
+                x for x in self.prior_indices if x not in labeled["record_id"].to_list()
+            ]
             self._label(unlabeled_priors, prior=True)
 
     def _stop_review(self):
         """Check if the review should be stopped according to stopping rule
         obtained from the settings.
 
         Returns
@@ -220,15 +222,15 @@
 
         # if the pool is empty, always stop
         if pool.empty:
             stop = True
 
         # If stop_if is set to min, stop when all papers in the pool are
         # irrelevant.
-        if self.stop_if == 'min' and (self.data_labels[pool] == 0).all():
+        if self.stop_if == "min" and (self.data_labels[pool] == 0).all():
             stop = True
         # Otherwise, stop when reaching stop_if (if provided)
         elif self.stop_if is not None:
             with open_state(self.project) as state:
                 training_sets = state.get_training_sets()
                 # There is one query per trained model. We subtract 1
                 # for the priors.
@@ -272,44 +274,46 @@
             s.add_labeling_data(record_ids, labels, prior=prior)
 
     def train(self):
         """Train a new model on the labeled data."""
         # Check if both labels are available.
         with open_state(self.project) as state:
             labeled = state.get_labeled()
-            labels = labeled['label'].to_list()
+            labels = labeled["label"].to_list()
             training_set = len(labeled)
             if not (0 in labels and 1 in labels):
-                raise ValueError('Not both labels available. '
-                                 'Stopped training the model')
+                raise ValueError(
+                    "Not both labels available. " "Stopped training the model"
+                )
 
         # TODO: Simplify balance model input.
         # Use the balance model to sample the trainings data.
-        y_sample_input = pd.DataFrame(self.record_table).\
-            merge(labeled, how='left', on='record_id').\
-            loc[:, 'label'].\
-            fillna(LABEL_NA).\
-            to_numpy()
+        y_sample_input = (
+            pd.DataFrame(self.record_table)
+            .merge(labeled, how="left", on="record_id")
+            .loc[:, "label"]
+            .fillna(LABEL_NA)
+            .to_numpy()
+        )
         train_idx = np.where(y_sample_input != LABEL_NA)[0]
 
-        X_train, y_train = self.balance_model.sample(
-            self.X,
-            y_sample_input,
-            train_idx
-        )
+        X_train, y_train = self.balance_model.sample(self.X, y_sample_input, train_idx)
 
         # Fit the classifier on the trainings data.
         self.classifier.fit(X_train, y_train)
 
         # Use the query strategy to produce a ranking.
-        ranked_record_ids = \
-            self.query_strategy.query(self.X, classifier=self.classifier)
+        ranked_record_ids = self.query_strategy.query(
+            self.X, classifier=self.classifier
+        )
 
         # TODO: Also log the probablities.
         # Log the ranking in the state.
         with open_state(self.project, read_only=False) as state:
-            state.add_last_ranking(ranked_record_ids,
-                                   self.classifier.name,
-                                   self.query_strategy.name,
-                                   self.balance_model.name,
-                                   self.feature_extraction.name,
-                                   training_set)
+            state.add_last_ranking(
+                ranked_record_ids,
+                self.classifier.name,
+                self.query_strategy.name,
+                self.balance_model.name,
+                self.feature_extraction.name,
+                training_set,
+            )
```

### Comparing `asreview-1.2.1/asreview/review/simulate.py` & `asreview-1.3a0/asreview/review/simulate.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from asreview.project import open_state
 from asreview.review import BaseReview
 from asreview.review.base import LABEL_NA
 from asreview.utils import get_random_state
 
 
 def sample_prior_knowledge(
-        labels, n_prior_included=10,
-        n_prior_excluded=10, random_state=None):
+    labels, n_prior_included=10, n_prior_excluded=10, random_state=None
+):
     """Function to sample prelabelled articles.
 
     Arguments
     ---------
     labels: np.ndarray
         Array of labels, with 1 -> included, 0 -> excluded.
     n_prior_included: int
@@ -54,25 +54,25 @@
     included_idx = np.where(labels == 1)[0]
     excluded_idx = np.where(labels == 0)[0]
 
     if len(included_idx) < n_prior_included:
         raise ValueError(
             f"Number of included priors requested ({n_prior_included})"
             f" is bigger than number of included papers "
-            f"({len(included_idx)}).")
+            f"({len(included_idx)})."
+        )
     if len(excluded_idx) < n_prior_excluded:
         raise ValueError(
             f"Number of excluded priors requested ({n_prior_excluded})"
             f" is bigger than number of excluded papers "
-            f"({len(excluded_idx)}).")
+            f"({len(excluded_idx)})."
+        )
     # select randomly from included and excluded papers
-    included_indexes_sample = r.choice(
-        included_idx, n_prior_included, replace=False)
-    excluded_indexes_sample = r.choice(
-        excluded_idx, n_prior_excluded, replace=False)
+    included_indexes_sample = r.choice(included_idx, n_prior_included, replace=False)
+    excluded_indexes_sample = r.choice(excluded_idx, n_prior_excluded, replace=False)
 
     init = np.append(included_indexes_sample, excluded_indexes_sample)
 
     return init
 
 
 class ReviewSimulate(BaseReview):
@@ -119,24 +119,25 @@
     write_interval: int
         After how many labeled records to write the simulation data to the
         state.
     """
 
     name = "simulate"
 
-    def __init__(self,
-                 as_data,
-                 *args,
-                 n_prior_included=0,
-                 n_prior_excluded=0,
-                 prior_indices=None,
-                 init_seed=None,
-                 write_interval=None,
-                 **kwargs):
-
+    def __init__(
+        self,
+        as_data,
+        *args,
+        n_prior_included=0,
+        n_prior_excluded=0,
+        prior_indices=None,
+        init_seed=None,
+        write_interval=None,
+        **kwargs,
+    ):
         self.n_prior_included = n_prior_included
         self.n_prior_excluded = n_prior_excluded
 
         self.write_interval = write_interval
 
         # check for partly labeled data
         labels = as_data.labels
@@ -145,64 +146,80 @@
             raise ValueError("Expected fully labeled dataset.")
 
         if prior_indices is not None and len(prior_indices) != 0:
             start_idx = prior_indices
         else:
             start_idx = as_data.prior_data_idx
             if len(start_idx) == 0 and n_prior_included + n_prior_excluded > 0:
-                start_idx = sample_prior_knowledge(labels,
-                                                   n_prior_included,
-                                                   n_prior_excluded,
-                                                   random_state=init_seed)
-        super(ReviewSimulate, self).__init__(as_data,
-                                             *args,
-                                             start_idx=start_idx,
-                                             **kwargs)
+                start_idx = sample_prior_knowledge(
+                    labels, n_prior_included, n_prior_excluded, random_state=init_seed
+                )
+        super(ReviewSimulate, self).__init__(
+            as_data, *args, start_idx=start_idx, **kwargs
+        )
 
         # Setup the reviewer attributes that take over the role of state
         # functions.
         with open_state(self.project) as state:
             # Check if there is already a ranking stored in the state.
             if state.model_has_trained:
                 self.last_ranking = state.get_last_ranking()
             else:
                 self.last_ranking = None
 
             self.labeled = state.get_labeled()
-            self.pool = pd.Series([
-                record_id for record_id in self.record_table if record_id
-                not in self.labeled['record_id'].values])
+            self.pool = pd.Series(
+                [
+                    record_id
+                    for record_id in self.record_table
+                    if record_id not in self.labeled["record_id"].values
+                ]
+            )
             self.training_set = len(self.labeled)
 
             # Get the number of queries.
             training_sets = state.get_training_sets()
             # There is one query per trained model. We subtract 1
             # for the priors.
             self.total_queries = len(set(training_sets)) - 1
 
             # Check that both labels are available.
-            if (0 not in self.labeled['label'].values) or \
-                    (1 not in self.labeled['label'].values):
-                raise ValueError("Not both labels available Make sure there"
-                                 " is an included and excluded record in "
-                                 "the priors.")
-
-        self.results = pd.DataFrame([], columns=[
-            'record_id', 'label', 'classifier', 'query_strategy',
-            'balance_strategy', 'feature_extraction', 'training_set',
-            'labeling_time', 'notes'])
+            if (0 not in self.labeled["label"].values) or (
+                1 not in self.labeled["label"].values
+            ):
+                raise ValueError(
+                    "Not both labels available Make sure there"
+                    " is an included and excluded record in "
+                    "the priors."
+                )
+
+        self.results = pd.DataFrame(
+            [],
+            columns=[
+                "record_id",
+                "label",
+                "classifier",
+                "query_strategy",
+                "balance_strategy",
+                "feature_extraction",
+                "training_set",
+                "labeling_time",
+                "notes",
+            ],
+        )
 
     def _label_priors(self):
         """Make sure all the priors are labeled as well as the pending
         labels."""
         with open_state(self.project, read_only=False) as state:
             # Make sure the prior records are labeled.
             labeled = state.get_labeled()
-            unlabeled_priors = [x for x in self.prior_indices
-                                if x not in labeled['record_id'].to_list()]
+            unlabeled_priors = [
+                x for x in self.prior_indices if x not in labeled["record_id"].to_list()
+            ]
             labels = self.data_labels[unlabeled_priors]
 
             with open_state(self.project, read_only=False) as s:
                 s.add_labeling_data(unlabeled_priors, labels, prior=True)
 
             # Make sure the pending records are labeled.
             pending = state.get_pending()
@@ -215,118 +232,121 @@
 
         # if the pool is empty, always stop
         if self.pool.empty:
             return True
 
         # If stop_if is set to min, stop when all papers in the pool are
         # irrelevant.
-        if self.stop_if == 'min' and (self.data_labels[self.pool] == 0).all():
+        if self.stop_if == "min" and (self.data_labels[self.pool] == 0).all():
             return True
 
         # Stop when reaching stop_if (if provided)
         if isinstance(self.stop_if, int) and self.total_queries >= self.stop_if:
             return True
 
         return False
 
     def train(self):
         """Train a new model on the labeled data."""
         # Check if both labels are available is done in init for simulation.
         # Use the balance model to sample the trainings data.
         new_training_set = len(self.labeled)
 
-        y_sample_input = pd.DataFrame(self.record_table). \
-            merge(self.labeled, how='left', on='record_id'). \
-            loc[:, 'label']. \
-            fillna(LABEL_NA). \
-            to_numpy()
+        y_sample_input = (
+            pd.DataFrame(self.record_table)
+            .merge(self.labeled, how="left", on="record_id")
+            .loc[:, "label"]
+            .fillna(LABEL_NA)
+            .to_numpy()
+        )
         train_idx = np.where(y_sample_input != LABEL_NA)[0]
 
-        X_train, y_train = self.balance_model.sample(
-            self.X,
-            y_sample_input,
-            train_idx
-        )
+        X_train, y_train = self.balance_model.sample(self.X, y_sample_input, train_idx)
 
         # Fit the classifier on the trainings data.
         self.classifier.fit(X_train, y_train)
 
         # Use the query strategy to produce a ranking.
-        ranked_record_ids = \
-            self.query_strategy.query(self.X, classifier=self.classifier)
+        ranked_record_ids = self.query_strategy.query(
+            self.X, classifier=self.classifier
+        )
 
-        self.last_ranking = \
-            pd.concat([pd.Series(ranked_record_ids),
-                      pd.Series(range(len(ranked_record_ids)))], axis=1)
-        self.last_ranking.columns = ['record_id', 'label']
+        self.last_ranking = pd.concat(
+            [pd.Series(ranked_record_ids), pd.Series(range(len(ranked_record_ids)))],
+            axis=1,
+        )
+        self.last_ranking.columns = ["record_id", "label"]
 
         self.training_set = new_training_set
 
     def _query(self, n):
         """In simulation mode, the query function should get the n highest
         ranked unlabeled records, without writing the model data to the results
-        table. The """
+        table. The"""
         unlabeled_ranking = self.last_ranking[
-            self.last_ranking['record_id'].isin(self.pool)]
+            self.last_ranking["record_id"].isin(self.pool)
+        ]
 
         self.total_queries += 1
 
-        return unlabeled_ranking['record_id'].iloc[:n].to_list()
+        return unlabeled_ranking["record_id"].iloc[:n].to_list()
 
     def _label(self, record_ids, prior=False):
         """In simulation mode, the label function should also add the model
         data to the results table."""
 
         labels = self.data_labels[record_ids]
         labeling_time = datetime.now()
 
         results = []
         for record_id, label in zip(record_ids, labels):
-            results.append({
-                'record_id': int(record_id),
-                'label': int(label),
-                'classifier': self.classifier.name,
-                'query_strategy': self.query_strategy.name,
-                'balance_strategy': self.balance_model.name,
-                'feature_extraction': self.feature_extraction.name,
-                'training_set': int(self.training_set),
-                'labeling_time': str(labeling_time),
-                'notes': None
-            })
-
-        self.results = pd.concat([
-            self.results,
-            pd.DataFrame(results)
-        ], ignore_index=True)
+            results.append(
+                {
+                    "record_id": int(record_id),
+                    "label": int(label),
+                    "classifier": self.classifier.name,
+                    "query_strategy": self.query_strategy.name,
+                    "balance_strategy": self.balance_model.name,
+                    "feature_extraction": self.feature_extraction.name,
+                    "training_set": int(self.training_set),
+                    "labeling_time": str(labeling_time),
+                    "notes": None,
+                }
+            )
+
+        self.results = pd.concat(
+            [self.results, pd.DataFrame(results)], ignore_index=True
+        )
 
         # Add the record ids to the labeled and remove from the pool.
-        new_labeled_data = pd.DataFrame(zip(record_ids, labels),
-                                        columns=['record_id', 'label'])
-        self.labeled = pd.concat(
-            [self.labeled, new_labeled_data], ignore_index=True)
+        new_labeled_data = pd.DataFrame(
+            zip(record_ids, labels), columns=["record_id", "label"]
+        )
+        self.labeled = pd.concat([self.labeled, new_labeled_data], ignore_index=True)
         self.pool = self.pool[~self.pool.isin(record_ids)]
 
-        if (self.write_interval is not None) and \
-                (len(self.results) >= self.write_interval):
+        if (self.write_interval is not None) and (
+            len(self.results) >= self.write_interval
+        ):
             self._write_to_state()
 
         return labels
 
     def _write_to_state(self):
         """Write the data that has not yet been written to the state."""
         # Write the data to the state.
         if len(self.results) > 0:
-            rows = [tuple(self.results.iloc[i])
-                    for i in range(len(self.results))]
+            rows = [tuple(self.results.iloc[i]) for i in range(len(self.results))]
             with open_state(self.project, read_only=False) as state:
                 state._add_labeling_data_simulation_mode(rows)
 
                 state.add_last_ranking(
-                    self.last_ranking['record_id'].to_numpy(),
+                    self.last_ranking["record_id"].to_numpy(),
                     self.classifier.name,
                     self.query_strategy.name,
                     self.balance_model.name,
                     self.feature_extraction.name,
-                    self.training_set)
+                    self.training_set,
+                )
 
             # Empty the results table in memory.
             self.results.drop(self.results.index, inplace=True)
```

### Comparing `asreview-1.2.1/asreview/search.py` & `asreview-1.3a0/asreview/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,24 +102,21 @@
         if all_authors is not None:
             match_list.append(format_to_str(all_authors[i]))
 
         # add keywords if present
         if all_keywords is not None:
             match_list.append(format_to_str(all_keywords[i]))
 
-        match_str[i, ] = " ".join(match_list)
+        match_str[i,] = " ".join(match_list)
     return match_str
 
 
-def fuzzy_find(as_data,
-               keywords,
-               threshold=60,
-               max_return=10,
-               exclude=None,
-               by_index=True):
+def fuzzy_find(
+    as_data, keywords, threshold=60, max_return=10, exclude=None, by_index=True
+):
     """Find a record using keywords.
 
     It looks for keywords in the title/authors/keywords
     (for as much is available). Using the diflib package it creates
     a ranking based on token set matching.
 
     Arguments
@@ -146,16 +143,19 @@
     """
     new_ranking = _get_fuzzy_scores(keywords, _match_string(as_data))
     sorted_idx = np.argsort(-new_ranking)
     best_idx = []
     if exclude is None:
         exclude = np.array([], dtype=int)
     for idx in sorted_idx:
-        if ((not by_index and as_data.df.index.values[idx] in exclude) or
-                by_index and idx in exclude):
+        if (
+            (not by_index and as_data.df.index.values[idx] in exclude)
+            or by_index
+            and idx in exclude
+        ):
             continue
         if len(best_idx) >= max_return:
             break
         if len(best_idx) > 0 and new_ranking[idx] < threshold:
             break
         best_idx.append(idx)
     fuzz_idx = np.array(best_idx, dtype=int)
```

### Comparing `asreview-1.2.1/asreview/settings.py` & `asreview-1.3a0/asreview/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,72 +38,71 @@
     "query_param": dict,
     "feature_param": dict,
     "balance_param": dict,
 }
 
 
 def _map_settings_type(name, value):
-
     if value is None:
         return None
 
     try:
         return SETTINGS_TYPE_DICT[name](value)
     except TypeError:
-        raise TypeError(
-            f"Can't convert setting '{name}' to {SETTINGS_TYPE_DICT[name]}"
-        )
+        raise TypeError(f"Can't convert setting '{name}' to {SETTINGS_TYPE_DICT[name]}")
 
 
 def _convert_types(par_defaults, param):
     """Convert strings from the config file to the appropriate type."""
     for par in param:
         try:
             par_type = type(par_defaults[par])
             if par_type == bool:
                 param[par] = param[par] in ["True", "true", "T", "t", True]
             else:
                 try:
                     param[par] = par_type(param[par])
                 except TypeError:
-                    raise TypeError(
-                        f"Error converting key in config file: {par}")
+                    raise TypeError(f"Error converting key in config file: {par}")
         except KeyError:
-            logging.warning(f"Parameter {par} does not have a default.\n"
-                            f"Defaults: {par_defaults}.")
+            logging.warning(
+                f"Parameter {par} does not have a default.\n"
+                f"Defaults: {par_defaults}."
+            )
 
 
 class ASReviewSettings(object):
     """Object to store the configuration of a review session.
 
     The main difference being that it type checks (some)
     of its contents.
     """
-    def __init__(self,
-                 model,
-                 query_strategy,
-                 balance_strategy,
-                 feature_extraction,
-                 n_instances=DEFAULT_N_INSTANCES,
-                 stop_if=None,
-                 n_prior_included=None,
-                 n_prior_excluded=None,
-                 as_data=None,
-                 model_param={},
-                 query_param={},
-                 balance_param={},
-                 feature_param={},
-                 data_fp=None,
-                 n_queries=None,
-                 abstract_only=False,  # deprecated
-                 mode=None,  # deprecated
-                 n_papers=None,  # deprecated
-                 data_name=None  # deprecated
-                 ):
 
+    def __init__(
+        self,
+        model,
+        query_strategy,
+        balance_strategy,
+        feature_extraction,
+        n_instances=DEFAULT_N_INSTANCES,
+        stop_if=None,
+        n_prior_included=None,
+        n_prior_excluded=None,
+        as_data=None,
+        model_param={},
+        query_param={},
+        balance_param={},
+        feature_param={},
+        data_fp=None,
+        n_queries=None,
+        abstract_only=False,  # deprecated
+        mode=None,  # deprecated
+        n_papers=None,  # deprecated
+        data_name=None,  # deprecated
+    ):
         self.model = model
         self.query_strategy = query_strategy
         self.balance_strategy = balance_strategy
         self.feature_extraction = feature_extraction
         self.n_instances = n_instances
         self.stop_if = stop_if
         self.n_prior_included = n_prior_included
@@ -123,25 +122,20 @@
         self.balance_param = balance_param
         self.feature_param = feature_param
 
     def __str__(self):
         return pretty_format(self.to_dict())
 
     def __setattr__(self, name, value):
-
         try:
             super(ASReviewSettings, self).__setattr__(
-                name,
-                _map_settings_type(name, value)
+                name, _map_settings_type(name, value)
             )
         except KeyError:
-            super(ASReviewSettings, self).__setattr__(
-                name,
-                value
-            )
+            super(ASReviewSettings, self).__setattr__(name, value)
 
     def to_dict(self):
         """Export default settings to dict."""
         info_dict = {}
         for attrib in SETTINGS_TYPE_DICT:
             value = getattr(self, attrib, None)
             if value is not None:
@@ -169,25 +163,31 @@
         # Read the each of the sections.
         for sect in config:
             if sect == "global_settings":
                 for key, value in config.items(sect):
                     try:
                         setattr(self, key, SETTINGS_TYPE_DICT[key](value))
                     except (KeyError, TypeError):
-                        print(f"Warning: value with key '{key}' is ignored "
-                              "(spelling mistake, wrong type?).")
+                        print(
+                            f"Warning: value with key '{key}' is ignored "
+                            "(spelling mistake, wrong type?)."
+                        )
 
             elif sect in [
-                    "model_param", "query_param", "balance_param",
-                    "feature_param"
+                "model_param",
+                "query_param",
+                "balance_param",
+                "feature_param",
             ]:
                 setattr(self, sect, dict(config.items(sect)))
             elif sect != "DEFAULT":
-                print(f"Warning: section [{sect}] is ignored in "
-                      f"config file {config_file}")
+                print(
+                    f"Warning: section [{sect}] is ignored in "
+                    f"config file {config_file}"
+                )
 
         model = get_classifier(self.model)
         _convert_types(model.default_param, self.model_param)
         balance_model = get_balance_model(self.balance_strategy)
         _convert_types(balance_model.default_param, self.balance_param)
         query_model = get_query_model(self.query_strategy)
         _convert_types(query_model.default_param, self.query_param)
```

### Comparing `asreview-1.2.1/asreview/state/__init__.py` & `asreview-1.3a0/asreview/state/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/state/base.py` & `asreview-1.3a0/asreview/state/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,17 +79,23 @@
         ---------
         probabilities: list-like.
             List containing the probabilities for every record.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def add_last_ranking(self, ranked_record_ids, classifier,
-                         query_strategy, balance_strategy, feature_extraction,
-                         training_set):
+    def add_last_ranking(
+        self,
+        ranked_record_ids,
+        classifier,
+        query_strategy,
+        balance_strategy,
+        feature_extraction,
+        training_set,
+    ):
         """Save the ranking of the last iteration of the model, in the ranking
         order.
 
         Arguments
         ---------
         ranked_record_ids: list, numpy.ndarray
             A list of records ids in the order that they were ranked.
@@ -116,16 +122,15 @@
             Series with name 'proba' containing the probabilities.
         """
         raise NotImplementedError
 
     @property
     @abstractmethod
     def settings(self):
-        """Get settings from the state.
-        """
+        """Get settings from the state."""
         raise NotImplementedError
 
     @abstractmethod
     def add_note(self, note, record_id):
         """Add a text note to save with a labeled record.
 
         Arguments
@@ -299,15 +304,15 @@
         -------
         pd.Series:
             Series containing the training set on which the classifier was
             fit at each labeling moment.
         """
         raise NotImplementedError
 
-    def get_labeling_times(self, time_format='int'):
+    def get_labeling_times(self, time_format="int"):
         """Get the time of labeling the state file.
 
         Arguments
         ---------
         time_format: 'int' or 'datetime'
             Format of the return value. If it is 'int' you get a UTC timestamp,
             if it is 'datetime' you get datetime instead of an integer.
@@ -318,26 +323,21 @@
             If format='int' you get a UTC timestamp (integer number of
             microseconds), if it is 'datetime' you get datetime format.
         """
         raise NotImplementedError
 
     @abstractmethod
     def close(self):
-        """Close the files opened by the state.
-
-        """
+        """Close the files opened by the state."""
         raise NotImplementedError
 
     def to_dict(self):
         """Convert state to dictionary.
 
         Returns
         -------
         dict:
             Dictionary with all settings and results.
         """
         state_data = self.get_dataset()
-        state_dict = {
-            'settings': vars(self.settings),
-            'data': state_data.to_dict()
-        }
+        state_dict = {"settings": vars(self.settings), "data": state_data.to_dict()}
         return state_dict
```

### Comparing `asreview-1.2.1/asreview/state/errors.py` & `asreview-1.3a0/asreview/state/errors.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/state/legacy/base.py` & `asreview-1.3a0/asreview/state/legacy/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,15 @@
             The last known queries, with {query_idx: query_method}.
         """
         raise NotImplementedError
 
     @property
     @abstractmethod
     def settings(self):
-        """Get settings from state
-        """
+        """Get settings from state"""
         raise NotImplementedError
 
     @abstractmethod
     def add_classification(self, idx, labels, methods, query_i):
         """Add training indices and their labels.
         Arguments
         ---------
@@ -241,16 +240,20 @@
             "query_i": query_i,
             "query_i_classified": query_i_classified,
         }
         return startup_vals
 
     def review_state(self):
         startup = self.startup_vals()
-        return (startup["labals"], startup["train_idx"], startup["query_src"],
-                startup["query_i"])
+        return (
+            startup["labals"],
+            startup["train_idx"],
+            startup["query_src"],
+            startup["query_i"],
+        )
 
     @property
     def pred_proba(self):
         """Get last predicted probabilities."""
         for query_i in reversed(range(self.n_queries())):
             try:
                 proba = self.get("proba", query_i=query_i)
@@ -308,20 +311,25 @@
         for dataset in global_datasets:
             try:
                 state_dict[dataset] = self.get(dataset).tolist()
             except KeyError:
                 pass
 
         query_datasets = [
-            "label_methods", "label_idx", "inclusions", "proba", "pool_idx",
-            "train_idx"
+            "label_methods",
+            "label_idx",
+            "inclusions",
+            "proba",
+            "pool_idx",
+            "train_idx",
         ]
         state_dict["results"] = []
         for query_i in range(self.n_queries()):
             state_dict["results"].append({})
             for dataset in query_datasets:
                 try:
                     state_dict["results"][query_i][dataset] = self.get(
-                        dataset, query_i).tolist()
+                        dataset, query_i
+                    ).tolist()
                 except (KeyError, IndexError):
                     pass
         return state_dict
```

### Comparing `asreview-1.2.1/asreview/state/legacy/dict.py` & `asreview-1.3a0/asreview/state/legacy/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     if dtype is not None:
         array = list(map(dtype, array))
     return array
 
 
 class DictState(BaseState):
     """Class for storing the state of a review with no permanent storage."""
+
     version = "1.1"
     read_only = False
 
     def __init__(self, state_fp, *_, **__):
         super(DictState, self).__init__(state_fp)
         self.read_only = False
 
@@ -112,16 +113,15 @@
 
         return state_str
 
     def _add_to_state(self, new_dict, i, append_result=False):
         # Find the first number that has not yet been used.
         results = self._state_dict["results"]
         if i is None:
-            if (len(results) > 0 and
-                    set(new_dict.keys()).isdisjoint(results[-1])):
+            if len(results) > 0 and set(new_dict.keys()).isdisjoint(results[-1]):
                 i = len(results) - 1
             else:
                 i = len(results)
 
         while i >= len(results):
             results.append({})
 
@@ -147,15 +147,15 @@
         if isinstance(feature_matrix, np.ndarray):
             encoded_X = feature_matrix.tolist()
             matrix_type = "ndarray"
         elif isinstance(feature_matrix, csr_matrix):
             with BytesIO() as f:
                 save_npz(f, feature_matrix)
                 f.seek(0)
-                encoded_X = b64encode(f.read()).decode('ascii')
+                encoded_X = b64encode(f.read()).decode("ascii")
             matrix_type = "csr_matrix"
         else:
             encoded_X = feature_matrix
             matrix_type = "unknown"
         data_properties[data_hash]["feature_matrix"] = encoded_X
         data_properties[data_hash]["matrix_type"] = matrix_type
 
@@ -199,15 +199,15 @@
 
     def add_classification(self, idx, labels, methods, query_i):
         # Ensure that variables are serializable
         idx = get_serial_list(idx, int)
         labels = get_serial_list(labels, int)
         methods = get_serial_list(methods, str)
 
-        new_dict = {'labelled': list(zip(idx, labels, methods))}
+        new_dict = {"labelled": list(zip(idx, labels, methods))}
         self._add_to_state(new_dict, query_i, append_result=True)
 
     def add_proba(self, pool_idx, train_idx, proba, query_i):
         new_dict = {
             "pool_idx": get_serial_list(pool_idx, int),
             "train_idx": get_serial_list(train_idx, int),
             "proba": get_serial_list(proba, float),
@@ -225,16 +225,15 @@
         label_vars = ["label_idx", "inclusions", "label_methods"]
         if variable in label_vars:
             array_id = label_vars.index(variable)
             if variable == "label_methods":
                 dtype = str
             else:
                 dtype = int
-            array = np.array([x[array_id] for x in res["labelled"]],
-                             dtype=dtype)
+            array = np.array([x[array_id] for x in res["labelled"]], dtype=dtype)
         elif variable == "labels":
             array = np.array(self._state_dict["labels"], dtype=int)
         elif variable == "final_labels":
             array = np.array(self._state_dict["final_labels"], dtype=int)
         elif variable == "proba":
             array = np.array(res["proba"], dtype=float)
         elif variable == "train_idx":
@@ -248,23 +247,24 @@
         return array
 
     def delete_last_query(self):
         self._state_dict["results"].pop()
 
     def initialize_structure(self):
         from asreview import __version__ as asr_version
-        self._state_dict = OrderedDict({
-            "time": {
-                "start_time": str(datetime.now())
-            },
-            "version": self.version,
-            "software_version": asr_version,
-            "settings": {},
-            "results": [],
-        })
+
+        self._state_dict = OrderedDict(
+            {
+                "time": {"start_time": str(datetime.now())},
+                "version": self.version,
+                "software_version": asr_version,
+                "settings": {},
+                "results": [],
+            }
+        )
 
     def close(self):
         if not self.read_only:
             self.save()
 
     def save(self):
         print(self)
```

### Comparing `asreview-1.2.1/asreview/state/legacy/hdf5.py` & `asreview-1.3a0/asreview/state/legacy/hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,115 +15,111 @@
 import json
 from datetime import datetime
 from pathlib import Path
 
 try:
     import h5py
 except ImportError:
-    raise ImportError("To use the legacy hdf5 state file, downgrade ASReview "
-                      "to version 0.x and make sure package h5py is installed.")
+    raise ImportError(
+        "To use the legacy hdf5 state file, downgrade ASReview "
+        "to version 0.x and make sure package h5py is installed."
+    )
 import numpy as np
 from scipy.sparse import csr_matrix
 
 from asreview.settings import ASReviewSettings
 from asreview.state.legacy.base import BaseState
 
 
 def _append_to_dataset(name, values, g, dtype):
     if name not in g:
-        g.create_dataset(name, (len(values), ),
-                         dtype=dtype,
-                         maxshape=(None, ),
-                         chunks=True)
+        g.create_dataset(
+            name, (len(values),), dtype=dtype, maxshape=(None,), chunks=True
+        )
     else:
-        g[name].resize((len(g[name]) + len(values), ))
+        g[name].resize((len(g[name]) + len(values),))
     dataset = g[name]
-    dataset[len(g[name]) - len(values):] = values
+    dataset[len(g[name]) - len(values) :] = values
 
 
 def _result_group(f, query_i):
     try:
-        g = f[f'/results/{query_i}']
+        g = f[f"/results/{query_i}"]
     except KeyError:
-        g = f.create_group(f'/results/{query_i}')
-        g.attrs['creation_time'] = np.string_(datetime.now())
+        g = f.create_group(f"/results/{query_i}")
+        g.attrs["creation_time"] = np.string_(datetime.now())
     return g
 
 
 class HDF5StateLegacy(BaseState):
     """Class for storing the review state with HDF5 storage."""
+
     version = "1.1"
 
     def __init__(self, state_fp, read_only=False):
         super(HDF5StateLegacy, self).__init__(state_fp, read_only=read_only)
 
     def set_labels(self, y):
         if "labels" not in self.f:
             self.f.create_dataset("labels", y.shape, dtype=int, data=y)
         else:
             self.f["labels"][...] = y
 
     def set_final_labels(self, y):
         if "final_labels" not in self.f:
-            self.f.create_dataset("final_labels",
-                                  y.shape,
-                                  dtype=int,
-                                  data=y)
+            self.f.create_dataset("final_labels", y.shape, dtype=int, data=y)
         else:
             self.f["final_labels"][...] = y
 
     def set_current_queries(self, current_queries):
-        str_queries = {
-            str(key): value
-            for key, value in current_queries.items()
-        }
+        str_queries = {str(key): value for key, value in current_queries.items()}
         data = np.string_(json.dumps(str_queries))
         self.f.attrs.pop("current_queries", None)
         self.f.attrs["current_queries"] = data
 
     def get_current_queries(self):
         str_queries = json.loads(self.f.attrs["current_queries"])
         return {int(key): value for key, value in str_queries.items()}
 
     def add_classification(self, idx, labels, methods, query_i):
         g = _result_group(self.f, query_i)
         if "new_labels" not in g:
             g.create_group("new_labels")
 
-        g = g['new_labels']
+        g = g["new_labels"]
 
         np_methods = np.array(list(map(np.string_, methods)))
-        _append_to_dataset('idx', idx, g, dtype=int)
-        _append_to_dataset('labels', labels, g, dtype=int)
-        _append_to_dataset('methods', np_methods, g, dtype='S20')
+        _append_to_dataset("idx", idx, g, dtype=int)
+        _append_to_dataset("labels", labels, g, dtype=int)
+        _append_to_dataset("methods", np_methods, g, dtype="S20")
 
     def add_proba(self, pool_idx, train_idx, proba, query_i):
         g = _result_group(self.f, query_i)
         g.create_dataset("pool_idx", data=pool_idx, dtype=int)
         g.create_dataset("train_idx", data=train_idx, dtype=int)
         g.create_dataset("proba", data=proba, dtype=float)
 
     @property
     def settings(self):
-        settings = self.f.attrs.get('settings', None)
+        settings = self.f.attrs.get("settings", None)
         if settings is None:
             return None
         settings_dict = json.loads(settings)
         return ASReviewSettings(**settings_dict)
 
     @settings.setter
     def settings(self, settings):
-        self.f.attrs.pop('settings', None)
-        self.f.attrs['settings'] = np.string_(json.dumps(vars(settings)))
+        self.f.attrs.pop("settings", None)
+        self.f.attrs["settings"] = np.string_(json.dumps(vars(settings)))
 
     def n_queries(self):
-        return len(self.f['results'].keys())
+        return len(self.f["results"].keys())
 
     def save(self):
-        self.f['end_time'] = str(datetime.now())
+        self.f["end_time"] = str(datetime.now())
         self.f.flush()
 
     def _add_as_data(self, as_data, feature_matrix=None):
         record_table = as_data.record_ids
         data_hash = as_data.hash()
         try:
             data_group = self.f["/data_properties"]
@@ -140,50 +136,51 @@
 
         if feature_matrix is None:
             return
         if isinstance(feature_matrix, np.ndarray):
             if "feature_matrix" in as_data_group:
                 return
             as_data_group.create_dataset("feature_matrix", data=feature_matrix)
-            as_data_group.attrs['matrix_type'] = np.string_("ndarray")
+            as_data_group.attrs["matrix_type"] = np.string_("ndarray")
         elif isinstance(feature_matrix, csr_matrix):
             if "indptr" in as_data_group:
                 return
             as_data_group.create_dataset("indptr", data=feature_matrix.indptr)
-            as_data_group.create_dataset("indices",
-                                         data=feature_matrix.indices)
-            as_data_group.create_dataset("shape",
-                                         data=feature_matrix.shape,
-                                         dtype=int)
+            as_data_group.create_dataset("indices", data=feature_matrix.indices)
+            as_data_group.create_dataset("shape", data=feature_matrix.shape, dtype=int)
             as_data_group.create_dataset("data", data=feature_matrix.data)
             as_data_group.attrs["matrix_type"] = np.string_("csr_matrix")
         else:
             as_data_group.create_dataset("feature_matrix", data=feature_matrix)
             as_data_group.attrs["matrix_type"] = np.string_("unknown")
 
     def get_feature_matrix(self, data_hash):
         as_data_group = self.f[f"/data_properties/{data_hash}"]
 
         matrix_type = as_data_group.attrs["matrix_type"].decode("ascii")
         if matrix_type == "ndarray":
             return np.array(as_data_group["feature_matrix"])
         elif matrix_type == "csr_matrix":
             feature_matrix = csr_matrix(
-                (as_data_group["data"], as_data_group["indices"],
-                 as_data_group["indexptr"]),
-                shape=as_data_group["shape"])
+                (
+                    as_data_group["data"],
+                    as_data_group["indices"],
+                    as_data_group["indexptr"],
+                ),
+                shape=as_data_group["shape"],
+            )
             return feature_matrix
         return as_data_group["feature_matrix"]
 
     def get(self, variable, query_i=None, idx=None):
         if query_i is not None:
             g = self.f[f"/results/{query_i}"]
         array = None
         if variable == "label_methods":
-            array = np.array(g["new_labels"]["methods"]).astype('U20')
+            array = np.array(g["new_labels"]["methods"]).astype("U20")
         if variable == "label_idx":
             array = np.array(g["new_labels"]["idx"], dtype=int)
         if variable == "inclusions":
             array = np.array(g["new_labels"]["labels"], dtype=int)
         if variable == "proba":
             array = np.array(g["proba"], dtype=float)
         if variable == "labels":
@@ -202,33 +199,34 @@
 
     def delete_last_query(self):
         query_i_last = self.n_queries() - 1
         del self.f[f"/results/{query_i_last}"]
 
     def restore(self, fp):
         if self.read_only:
-            mode = 'r'
+            mode = "r"
         else:
-            mode = 'a'
+            mode = "a"
 
         Path(fp).parent.mkdir(parents=True, exist_ok=True)
         self.f = h5py.File(fp, mode)
         try:
-            state_version = self.f.attrs['version'].decode("ascii")
+            state_version = self.f.attrs["version"].decode("ascii")
             if state_version != self.version:
                 raise ValueError(
                     f"State cannot be read: state version {self.version}, "
-                    f"state file version {state_version}.")
+                    f"state file version {state_version}."
+                )
         except KeyError:
             self.initialize_structure()
 
     def initialize_structure(self):
-        self.f.attrs['start_time'] = np.string_(datetime.now())
-        self.f.attrs['end_time'] = np.string_(datetime.now())
-        self.f.attrs['settings'] = np.string_("{}")
-        self.f.attrs['version'] = np.string_(self.version)
-        self.f.create_group('results')
+        self.f.attrs["start_time"] = np.string_(datetime.now())
+        self.f.attrs["end_time"] = np.string_(datetime.now())
+        self.f.attrs["settings"] = np.string_("{}")
+        self.f.attrs["version"] = np.string_(self.version)
+        self.f.create_group("results")
 
     def close(self):
         if not self.read_only:
-            self.f.attrs['end_time'] = np.string_(datetime.now())
+            self.f.attrs["end_time"] = np.string_(datetime.now())
         self.f.close()
```

### Comparing `asreview-1.2.1/asreview/state/legacy/json.py` & `asreview-1.3a0/asreview/state/legacy/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,39 +19,41 @@
 
 from asreview.settings import ASReviewSettings
 from asreview.state.legacy.dict import DictState
 
 
 class JSONState(DictState):
     """Class for storing the state of a Systematic Review using JSON files."""
+
     version = "2.1"
 
     def __init__(self, state_fp, read_only=False):
         super(JSONState, self).__init__(state_fp)
         self.read_only = read_only
 
     def save(self):
         if self.read_only:
-            raise ValueError("State error: trying to save when opened file"
-                             " in read_only mode.")
+            raise ValueError(
+                "State error: trying to save when opened file" " in read_only mode."
+            )
         self._state_dict["time"]["end_time"] = str(datetime.now())
         fp = Path(self.state_fp)
 
         if fp.is_file:
             fp.parent.mkdir(parents=True, exist_ok=True)
 
         try:
             self._state_dict["current_queries"] = {
                 str(key): val
                 for key, val in self._state_dict["current_queries"].items()
             }
         except KeyError:
             pass
 
-        with fp.open('w') as outfile:
+        with fp.open("w") as outfile:
             json.dump(self._state_dict, outfile, indent=2)
 
         try:
             self._state_dict["current_queries"] = {
                 int(key): val
                 for key, val in self._state_dict["current_queries"].items()
             }
@@ -62,19 +64,19 @@
         try:
             with open(fp, "r") as f:
                 self._state_dict = OrderedDict(json.load(f))
             state_version = self._state_dict["version"]
             if state_version != self.version:
                 raise ValueError(
                     f"State cannot be read: state version {self.version}, "
-                    f"state file version {state_version}.")
+                    f"state file version {state_version}."
+                )
             self.settings = ASReviewSettings(**self._state_dict["settings"])
             try:
                 self._state_dict["current_queries"] = {
                     int(key): val
-                    for key, val in
-                    self._state_dict["current_queries"].items()
+                    for key, val in self._state_dict["current_queries"].items()
                 }
             except KeyError:
                 pass
         except FileNotFoundError:
             self.initialize_structure()
```

### Comparing `asreview-1.2.1/asreview/state/legacy/utils.py` & `asreview-1.3a0/asreview/state/legacy/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,23 +21,26 @@
 
 from asreview.config import LEGACY_STATE_EXTENSIONS
 
 
 def _get_state_class(fp):
     "Get state class from file extension."
     from asreview.state.legacy.dict import DictState
+
     if fp is None:
         return DictState
 
     state_ext = Path(fp).suffix
-    if state_ext in ['.h5', '.hdf5', '.he5']:
+    if state_ext in [".h5", ".hdf5", ".he5"]:
         from asreview.state.legacy.hdf5 import HDF5StateLegacy
+
         state_class = HDF5StateLegacy
-    elif state_ext in ['.json']:
+    elif state_ext in [".json"]:
         from asreview.state.legacy.json import JSONState
+
         state_class = JSONState
     else:
         state_class = None
     return state_class
 
 
 @contextmanager
@@ -57,17 +60,19 @@
         - [.h5, .hdf5, .he5] -> HDF5state.
         - None -> Dictstate (doesn't store anything permanently).
         - Anything else -> JSONstate.
     """
     state_class = _get_state_class(fp)
 
     if state_class is None:
-        raise ValueError("Bad state file extension, choose one of the"
-                         f" following:\n   "
-                         f"{', '.join(LEGACY_STATE_EXTENSIONS)}")
+        raise ValueError(
+            "Bad state file extension, choose one of the"
+            f" following:\n   "
+            f"{', '.join(LEGACY_STATE_EXTENSIONS)}"
+        )
 
     # init state class
     state = state_class(state_fp=fp, *args, read_only=read_only, **kwargs)
 
     try:
         yield state
     finally:
@@ -124,19 +129,20 @@
     if not Path(data_fp).is_file():
         logging.error(f"File {data_fp} does not exist, cannot create state.")
         return None
 
     if Path(data_fp).suffix == ".asreview":
         base_state = state_from_asreview_file(data_fp)
     elif Path(data_fp).suffix in LEGACY_STATE_EXTENSIONS:
-        base_state = _get_state_class(data_fp)(state_fp=data_fp,
-                                               read_only=True)
+        base_state = _get_state_class(data_fp)(state_fp=data_fp, read_only=True)
     else:
-        raise ValueError(f"Expected ASReview file or file {data_fp} with "
-                         f"extension {LEGACY_STATE_EXTENSIONS}.")
+        raise ValueError(
+            f"Expected ASReview file or file {data_fp} with "
+            f"extension {LEGACY_STATE_EXTENSIONS}."
+        )
 
     state = {os.path.basename(os.path.normpath(data_fp)): base_state}
     return state
 
 
 def state_from_asreview_file(data_fp):
     """Obtain the state from a .asreview file.
@@ -146,18 +152,18 @@
         Path to .asreview file.
     Returns
     -------
     BaseState:
         The same type of state file as in the .asreview file, which at the moment
         is JSONState.
     """
-    if not Path(data_fp).suffix == '.asreview':
+    if not Path(data_fp).suffix == ".asreview":
         raise ValueError(f"file {data_fp} does not end with '.asreview'.")
 
     # Name of the state file in the .asreview file.
-    state_fp_in_zip = 'result.json'
+    state_fp_in_zip = "result.json"
     with zipfile.ZipFile(data_fp, "r") as zipObj:
         tmpdir = tempfile.TemporaryDirectory()
         zipObj.extract(state_fp_in_zip, tmpdir.name)
         fp = Path(tmpdir.name, state_fp_in_zip)
         state = _get_state_class(fp)(state_fp=fp, read_only=True)
         return state
```

### Comparing `asreview-1.2.1/asreview/state/sql_converter.py` & `asreview-1.3a0/asreview/state/sql_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,33 +29,32 @@
 from scipy.sparse import save_npz
 
 from asreview._version import get_versions
 from asreview.state.errors import StateError
 from asreview.state.legacy.utils import open_state as open_state_legacy
 
 SQLSTATE_VERSION = "1.0"
-ASREVIEW_FILE_EXTENSION = '.asreview'
+ASREVIEW_FILE_EXTENSION = ".asreview"
 
 
 class StateConversionException(Exception):
     pass
 
 
 def is_old_project(fp):
     """Check if state file is old version."""
-    if Path(fp, 'reviews').is_dir():
+    if Path(fp, "reviews").is_dir():
         return False
     else:
         return True
 
 
 def get_old_project_status(config):
-
     # project is marked as finished
-    if config.get('reviewFinished', False):
+    if config.get("reviewFinished", False):
         return "finished"
 
     # project init is not ready
     if "projectInitReady" in config and not config["projectInitReady"]:
         return "setup"
 
     # project init flag is not available
@@ -93,39 +92,41 @@
     Returns
     -------
     Converts the data in the project to the new format
     and adds it to the folder in place."""
 
     if from_version != 0 and to_version != 1:
         raise ValueError(
-            f"Not possible to upgrade from v{from_version} to v{to_version}.")
+            f"Not possible to upgrade from v{from_version} to v{to_version}."
+        )
 
     # Check if it is indeed an old format project.
     if not is_old_project(fp):
-        raise ValueError(f"There already is a 'reviews' folder at {fp}. "
-                         f"This project seems to be in new format.")
+        raise ValueError(
+            f"There already is a 'reviews' folder at {fp}. "
+            f"This project seems to be in new format."
+        )
 
     # Current Paths
     fp = Path(fp)
-    legacy_fp = Path(fp, 'legacy')
+    legacy_fp = Path(fp, "legacy")
     move_old_files_to_legacy_folder(fp)
 
     try:
         # Current paths.
-        json_fp = Path(legacy_fp, 'result.json')
-        labeled_json_fp = Path(legacy_fp, 'labeled.json')
-        pool_fp = Path(legacy_fp, 'pool.json')
-        kwargs_fp = Path(legacy_fp, 'kwargs.json')
+        json_fp = Path(legacy_fp, "result.json")
+        labeled_json_fp = Path(legacy_fp, "labeled.json")
+        pool_fp = Path(legacy_fp, "pool.json")
+        kwargs_fp = Path(legacy_fp, "kwargs.json")
         review_id = str(uuid4().hex)
 
         # Create the reviews folder and the paths for the results and settings.
-        Path(fp, 'reviews', review_id).mkdir(parents=True)
-        sql_fp = str(Path(fp, 'reviews', review_id, 'results.sql'))
-        settings_metadata_fp = Path(fp, 'reviews', review_id,
-                                    'settings_metadata.json')
+        Path(fp, "reviews", review_id).mkdir(parents=True)
+        sql_fp = str(Path(fp, "reviews", review_id, "results.sql"))
+        settings_metadata_fp = Path(fp, "reviews", review_id, "settings_metadata.json")
 
         # Create the path for the feature matrix.
 
         # Create sqlite table with the results of the review.
         convert_json_results_to_sql(sql_fp, json_fp, labeled_json_fp)
 
         # Create sqlite tables 'last_probabilities'.
@@ -140,38 +141,42 @@
         # Create decision changes table.
         create_decision_changes_table(sql_fp)
 
         # Create json for settings.
         convert_json_settings_metadata(settings_metadata_fp, json_fp)
 
         # Create file for the feature matrix.
-        with open(kwargs_fp, 'r') as f:
+        with open(kwargs_fp, "r") as f:
             kwargs_dict = json.load(f)
-            feature_extraction_method = kwargs_dict['feature_extraction']
-        feature_matrix_fp = convert_json_feature_matrix(fp, json_fp,
-                                                        feature_extraction_method)
+            feature_extraction_method = kwargs_dict["feature_extraction"]
+        feature_matrix_fp = convert_json_feature_matrix(
+            fp, json_fp, feature_extraction_method
+        )
 
         # --- Upgrade the project.json file.
 
         # extract the start time from the state json
-        with open(json_fp, 'r') as f:
-            start_time = json.load(f)['time']['start_time']
+        with open(json_fp, "r") as f:
+            start_time = json.load(f)["time"]["start_time"]
             start_time = datetime.strptime(start_time, "%Y-%m-%d %H:%M:%S.%f")
 
         # open the project json and upgrade
-        with open(Path(fp, 'project.json'), 'r') as f:
+        with open(Path(fp, "project.json"), "r") as f:
             project_config_old = json.load(f)
 
-        project_config_new = upgrade_project_config(project_config_old, review_id,
-                                                    start_time,
-                                                    Path(feature_matrix_fp).name,
-                                                    feature_extraction_method)
+        project_config_new = upgrade_project_config(
+            project_config_old,
+            review_id,
+            start_time,
+            Path(feature_matrix_fp).name,
+            feature_extraction_method,
+        )
 
         # dump the project json
-        with open(Path(fp, 'project.json'), 'w') as f:
+        with open(Path(fp, "project.json"), "w") as f:
             json.dump(project_config_new, f)
     except Exception as e:
         rollback_conversion(fp, check_is_converted=False)
         raise StateConversionException(
             f"An error occurred during conversion of state "
             f"from {from_version} to {to_version}."
         ) from e
@@ -191,34 +196,36 @@
     this legacy folder, and keeps a copy of 'project.json' and the data folder
     at the original place.
     """
 
     project_content = list(fp.iterdir())
 
     # copy to legacy folder
-    shutil.copytree(fp, Path(fp, 'legacy'))
+    shutil.copytree(fp, Path(fp, "legacy"))
 
     # remove files and folders
-    files_to_keep = ['project.json', 'data', 'lock.sqlite']
+    files_to_keep = ["project.json", "data", "lock.sqlite"]
 
     for f in project_content:
         if f.name not in files_to_keep:
             if f.is_file():
                 f.unlink()
             elif f.is_dir():
                 shutil.rmtree(f)
             else:
                 pass
 
 
-def upgrade_project_config(config,
-                           review_id=None,
-                           start_time=None,
-                           feature_matrix_name=None,
-                           feature_extraction_method=None):
+def upgrade_project_config(
+    config,
+    review_id=None,
+    start_time=None,
+    feature_matrix_name=None,
+    feature_extraction_method=None,
+):
     """Update the project.json file to contain the review information , the
     feature matrix information and the new state version number.
 
     Arguments
     ---------
     config: str/path
         Path to the project json file.
@@ -231,39 +238,38 @@
     feature_extraction_method: str
         Name of the feature extraction method.
     """
 
     start_time_s = str(start_time) if start_time else None
 
     # Add the review information.
-    config['reviews'] = [{
-        'id': review_id,
-        'start_time': start_time_s,
-        'status': get_old_project_status(config)
-    }]
+    config["reviews"] = [
+        {
+            "id": review_id,
+            "start_time": start_time_s,
+            "status": get_old_project_status(config),
+        }
+    ]
 
     # Add the feature matrix information.
-    config['feature_matrices'] = [{
-        'id': feature_extraction_method,
-        'filename': feature_matrix_name
-    }]
+    config["feature_matrices"] = [
+        {"id": feature_extraction_method, "filename": feature_matrix_name}
+    ]
 
     # Add the project mode.
-    config['mode'] = config.get('mode', 'oracle')
+    config["mode"] = config.get("mode", "oracle")
 
     # Update the state version.
-    config['version'] = get_versions()['version']
-    config['state_version'] = SQLSTATE_VERSION
+    config["version"] = get_versions()["version"]
+    config["state_version"] = SQLSTATE_VERSION
 
     # set created_at_unix to start time (empty: None)
     if "created_at_unix" not in config:
         try:
-            config["created_at_unix"] = time.mktime(
-                start_time.timetuple()
-            )
+            config["created_at_unix"] = time.mktime(start_time.timetuple())
         except Exception:
             config["created_at_unix"] = None
 
     config["datetimeCreated"] = start_time_s
 
     # delete deprecated metadata
     config.pop("projectInitReady", None)
@@ -282,27 +288,26 @@
     fp: str/path
         Path where to save the json file.
     json_fp: str/path
         Path to the json state file.
     """
     data_dict = {}
     with open_state_legacy(json_fp) as json_state:
-        data_dict['settings'] = json_state._state_dict['settings']
+        data_dict["settings"] = json_state._state_dict["settings"]
         # The 'triple' balance strategy is no longer implemented.
-        if data_dict['settings']['balance_strategy'] == 'triple':
-            data_dict['settings']['balance_strategy'] = 'double'
-        data_dict['state_version'] = SQLSTATE_VERSION
-        data_dict['software_version'] = json_state._state_dict[
-            'software_version']
-        data_dict['model_has_trained'] = True
+        if data_dict["settings"]["balance_strategy"] == "triple":
+            data_dict["settings"]["balance_strategy"] = "double"
+        data_dict["state_version"] = SQLSTATE_VERSION
+        data_dict["software_version"] = json_state._state_dict["software_version"]
+        data_dict["model_has_trained"] = True
 
         # remove the outdated mode
         data_dict.pop("mode", None)
 
-    with open(fp, 'w') as f:
+    with open(fp, "w") as f:
         json.dump(data_dict, f)
 
 
 def create_last_ranking_table(sql_fp, pool_fp, kwargs_fp, json_fp):
     """Create the table which will contain the ranking of the last iteration of
     the model.
 
@@ -311,56 +316,67 @@
     sql_fp: str/path
         Path where to save the record table. Should be a .sql file.
     """
 
     with open(pool_fp) as f_pool:
         pool_ranking = json.load(f_pool)
 
-    with open(kwargs_fp, 'r') as f_kwargs:
+    with open(kwargs_fp, "r") as f_kwargs:
         kwargs_dict = json.load(f_kwargs)
 
     # Add the record_ids not found in the pool to the end of the ranking.
     with open_state_legacy(json_fp) as json_state:
         record_table = get_json_record_table(json_state)
     records_not_in_pool = [
-        record_id for record_id in record_table
-        if record_id not in pool_ranking
+        record_id for record_id in record_table if record_id not in pool_ranking
     ]
     pool_ranking += records_not_in_pool
 
     # Convert the records in the pool to the new record ids (starting from 0).
-    old_to_new_record_ids = {old_id: idx
-                             for idx, old_id in enumerate(record_table)}
+    old_to_new_record_ids = {old_id: idx for idx, old_id in enumerate(record_table)}
     pool_ranking = [old_to_new_record_ids[record] for record in pool_ranking]
 
     # Set the training set to -1 (prior) for records from old pool.
     training_set = -1
     time = None
 
-    last_ranking = [(v, i, kwargs_dict['model'], kwargs_dict['query_strategy'],
-                     kwargs_dict['balance_strategy'],
-                     kwargs_dict['feature_extraction'], training_set, time)
-                    for i, v in enumerate(pool_ranking)]
+    last_ranking = [
+        (
+            v,
+            i,
+            kwargs_dict["model"],
+            kwargs_dict["query_strategy"],
+            kwargs_dict["balance_strategy"],
+            kwargs_dict["feature_extraction"],
+            training_set,
+            time,
+        )
+        for i, v in enumerate(pool_ranking)
+    ]
 
     with sqlite3.connect(sql_fp) as con:
         cur = con.cursor()
 
         # Create the last_ranking table.
-        cur.execute('''CREATE TABLE last_ranking
+        cur.execute(
+            """CREATE TABLE last_ranking
                         (record_id INTEGER,
                         ranking INT,
                         classifier TEXT,
                         query_strategy TEXT,
                         balance_strategy TEXT,
                         feature_extraction TEXT,
                         training_set INTEGER,
-                        time INTEGER)''')
+                        time INTEGER)"""
+        )
         cur.executemany(
             """INSERT INTO last_ranking VALUES
-                                    (?, ?, ?, ?, ?, ?, ?, ?)""", last_ranking)
+                                    (?, ?, ?, ?, ?, ?, ?, ?)""",
+            last_ranking,
+        )
         con.commit()
 
 
 def convert_json_last_probabilities(sql_fp, json_fp):
     """Get the last ranking from a json state and save it as the table
     'last_probabilities' in the .sql file at the location of sql_fp.
 
@@ -373,37 +389,40 @@
     """
     with open_state_legacy(json_fp) as json_state:
         # Get the last predicted probabilities from the state file.
         # Also get the number of record labeled and the classifier.
         last_probabilities = json_state.pred_proba
 
         # Put them in the format for input in the sqlite database.
-        last_probabilities = [(proba, ) for proba in last_probabilities]
+        last_probabilities = [(proba,) for proba in last_probabilities]
 
         with sqlite3.connect(sql_fp) as con:
             cur = con.cursor()
-            cur.execute("""CREATE TABLE last_probabilities
-                            (proba REAL)""")
+            cur.execute(
+                """CREATE TABLE last_probabilities
+                            (proba REAL)"""
+            )
             cur.executemany(
                 """INSERT INTO last_probabilities VALUES
-                                        (?)""", last_probabilities)
+                                        (?)""",
+                last_probabilities,
+            )
 
             con.commit()
 
 
 def get_json_state_data_hash(json_state):
     """Get the data hash from a json state."""
-    return list(json_state._state_dict['data_properties'].keys())[0]
+    return list(json_state._state_dict["data_properties"].keys())[0]
 
 
 def get_json_record_table(json_state):
     """Get the record table from a json state."""
     data_hash = get_json_state_data_hash(json_state)
-    record_table = json_state._state_dict['data_properties'][data_hash][
-        'record_table']
+    record_table = json_state._state_dict["data_properties"][data_hash]["record_table"]
     return record_table
 
 
 def convert_json_feature_matrix(fp, json_fp, feature_extraction_method):
     """Get the feature matrix from a json state file. Save it in the feature
     matrices folder. Format is .npz if the matrix is sparse and .npy if the
     matrix is dense.
@@ -418,27 +437,29 @@
         Name of the feature extraction method.
 
     Returns
     -------
     pathlib.Path
         Path where the feature matrix is saved.
     """
-    feature_matrices_fp = Path(fp, 'feature_matrices')
+    feature_matrices_fp = Path(fp, "feature_matrices")
     feature_matrices_fp.mkdir()
 
     with open_state_legacy(json_fp) as json_state:
         data_hash = get_json_state_data_hash(json_state)
         feature_matrix = decode_feature_matrix(json_state, data_hash)
         if issparse(feature_matrix):
-            save_fp = Path(feature_matrices_fp,
-                           f'{feature_extraction_method}_feature_matrix.npz')
+            save_fp = Path(
+                feature_matrices_fp, f"{feature_extraction_method}_feature_matrix.npz"
+            )
             save_npz(save_fp, feature_matrix)
         else:
-            save_fp = Path(feature_matrices_fp,
-                           f'{feature_extraction_method}_feature_matrix.npy')
+            save_fp = Path(
+                feature_matrices_fp, f"{feature_extraction_method}_feature_matrix.npy"
+            )
             np.save(save_fp, feature_matrix)
 
     return save_fp
 
 
 def convert_json_record_table(sql_fp, json_fp):
     """Get the record table and save as the table 'record_table'
@@ -452,92 +473,102 @@
         Path to the json state file.
     """
 
     with open_state_legacy(json_fp) as json_state:
         record_table = get_json_record_table(json_state)
 
     # Convert record_table to list of tuples.
-    record_table = [(record_id, ) for record_id in range(len(record_table))]
+    record_table = [(record_id,) for record_id in range(len(record_table))]
 
     con = sqlite3.connect(sql_fp)
     cur = con.cursor()
-    cur.execute('''CREATE TABLE record_table
-                    (record_id INT)''')
+    cur.execute(
+        """CREATE TABLE record_table
+                    (record_id INT)"""
+    )
     cur.executemany(
         """INSERT INTO record_table VALUES
-                                (?)""", record_table)
+                                (?)""",
+        record_table,
+    )
     con.commit()
     con.close()
 
 
 def convert_json_results_to_sql(sql_fp, json_fp, labeled_json_fp):
     """Convert the result of a json state file to a sqlite database."""
     with open_state_legacy(json_fp, read_only=True) as sf:
         with sqlite3.connect(sql_fp) as con:
-            with open(labeled_json_fp, 'r') as file:
+            with open(labeled_json_fp, "r") as file:
                 labeled_json = json.load(file)
 
             cur = con.cursor()
 
             # Create the results table.
-            cur.execute('''CREATE TABLE results
+            cur.execute(
+                """CREATE TABLE results
                             (record_id INTEGER,
                             label INTEGER,
                             classifier TEXT,
                             query_strategy TEXT,
                             balance_strategy TEXT,
                             feature_extraction TEXT,
                             training_set INTEGER,
                             labeling_time INTEGER,
-                            notes TEXT)''')
+                            notes TEXT)"""
+            )
 
             record_table = get_json_record_table(sf)
-            record_id_to_row_number = {record_table[i]: i
-                                       for i in range(len(record_table))}
+            record_id_to_row_number = {
+                record_table[i]: i for i in range(len(record_table))
+            }
             old_record_ids = [x[0] for x in labeled_json]
-            sf_indices = [record_id_to_row_number[record_id]
-                          for record_id in old_record_ids]
+            sf_indices = [
+                record_id_to_row_number[record_id] for record_id in old_record_ids
+            ]
 
             sf_labels = [x[1] for x in labeled_json]
 
             # query strategy.
             old_query_strategy = [
                 sample_data[2]
-                for query in range(len(sf._state_dict['results']))
-                for sample_data in sf._state_dict['results'][query]['labelled']
+                for query in range(len(sf._state_dict["results"]))
+                for sample_data in sf._state_dict["results"][query]["labelled"]
             ]
 
-            n_priors = old_query_strategy.count('prior')
+            n_priors = old_query_strategy.count("prior")
             n_records_labeled = len(sf_indices)
             n_non_prior_records = n_records_labeled - n_priors
 
-            query_strategy = sf.settings.to_dict()['query_strategy']
-            sf_query_strategy = ['prior'] * n_priors + \
-                                [query_strategy] * n_non_prior_records
+            query_strategy = sf.settings.to_dict()["query_strategy"]
+            sf_query_strategy = ["prior"] * n_priors + [
+                query_strategy
+            ] * n_non_prior_records
 
             # classifier.
-            classifier = sf.settings.to_dict()['model']
+            classifier = sf.settings.to_dict()["model"]
             sf_classifiers = [None] * n_priors + [
-                f'{classifier}' for _ in range(n_non_prior_records)
+                f"{classifier}" for _ in range(n_non_prior_records)
             ]
 
             # training set.
             sf_training_sets = [-1] * n_priors + list(
-                range(n_priors, n_records_labeled))
+                range(n_priors, n_records_labeled)
+            )
 
             # feature extraction.
-            feature_extraction = sf.settings.to_dict()['feature_extraction']
+            feature_extraction = sf.settings.to_dict()["feature_extraction"]
             sf_feature_extraction = [None] * n_priors + [
-                f'{feature_extraction}' for _ in range(n_non_prior_records)
+                f"{feature_extraction}" for _ in range(n_non_prior_records)
             ]
 
             # balance strategy.
-            balance_strategy = sf.settings.to_dict()['balance_strategy']
+            balance_strategy = sf.settings.to_dict()["balance_strategy"]
             sf_balance_strategy = [None] * n_priors + [
-                f'{balance_strategy}' for _ in range(n_non_prior_records)
+                f"{balance_strategy}" for _ in range(n_non_prior_records)
             ]
 
             # Labeling time.
             sf_time = [0 for _ in range(n_records_labeled)]
 
             # No notes were saved before.
             sf_notes = [None for _ in range(n_records_labeled)]
@@ -548,97 +579,105 @@
                 len(sf_labels),
                 len(sf_classifiers),
                 len(sf_training_sets),
                 len(sf_query_strategy),
                 len(sf_time),
                 len(sf_feature_extraction),
                 len(sf_balance_strategy),
-                len(sf_notes)
+                len(sf_notes),
             ]
             if not all([length == n_records_labeled for length in lengths]):
-                raise StateError(
-                    "All datasets should have the same number of entries.")
+                raise StateError("All datasets should have the same number of entries.")
 
             # Create the database rows.
-            db_rows = [(sf_indices[i], sf_labels[i], sf_classifiers[i],
-                        sf_query_strategy[i], sf_balance_strategy[i],
-                        sf_feature_extraction[i], sf_training_sets[i],
-                        sf_time[i], sf_notes[i])
-                       for i in range(n_records_labeled)]
+            db_rows = [
+                (
+                    sf_indices[i],
+                    sf_labels[i],
+                    sf_classifiers[i],
+                    sf_query_strategy[i],
+                    sf_balance_strategy[i],
+                    sf_feature_extraction[i],
+                    sf_training_sets[i],
+                    sf_time[i],
+                    sf_notes[i],
+                )
+                for i in range(n_records_labeled)
+            ]
             cur.executemany(
                 """INSERT INTO results VALUES
-                            (?, ?, ?, ?, ?, ?, ?, ?, ?)""", db_rows)
+                            (?, ?, ?, ?, ?, ?, ?, ?, ?)""",
+                db_rows,
+            )
             con.commit()
 
 
 def create_decision_changes_table(sql_fp):
     """Create an emtpy table that will contain the record_ids and new labels
     of the records whose label was changed after the original labeling action.
     Also contains the time at which the label was changed."""
     with sqlite3.connect(sql_fp) as con:
         cur = con.cursor()
 
-        cur.execute('''CREATE TABLE decision_changes
+        cur.execute(
+            """CREATE TABLE decision_changes
                                     (record_id INTEGER,
                                     new_label INTEGER,
-                                    time INTEGER)''')
+                                    time INTEGER)"""
+        )
 
         con.commit()
 
 
 # Disable is_converted_check.
-def rollback_conversion(fp,
-                        from_version=1,
-                        to_version=0,
-                        check_is_converted=True):
+def rollback_conversion(fp, from_version=1, to_version=0, check_is_converted=True):
     if from_version != 1 and to_version != 0:
         raise ValueError(
             f"Not possible to roll back conversion from v{from_version} "
             f"to v{to_version}."
         )
 
     if check_is_converted and not is_converted_project(fp):
-        raise ValueError(f"Project file at {fp} is not a converted "
-                         f"project file.")
+        raise ValueError(f"Project file at {fp} is not a converted " f"project file.")
 
     fp = Path(fp)
-    legacy_fp = Path(fp, 'legacy')
+    legacy_fp = Path(fp, "legacy")
 
     # Delete everything other than the legacy folder.
     for item in fp.iterdir():
         if item.is_file():
             item.unlink()
-        elif item.is_dir() and (item.name != 'legacy'):
+        elif item.is_dir() and (item.name != "legacy"):
             shutil.rmtree(item)
         else:
             pass
 
     # Copy from legacy folder and delete it after.
     shutil.copytree(legacy_fp, fp, dirs_exist_ok=True)
     shutil.rmtree(legacy_fp)
 
 
 def is_converted_project(fp):
     """Check if asreview file has been converter from v0 to v1."""
     # Check if there is a legacy project.json and it has v0.
     try:
-        with open(Path(fp, 'legacy', 'project.json'), 'r') as f:
+        with open(Path(fp, "legacy", "project.json"), "r") as f:
             project_config_old = json.load(f)
     except FileNotFoundError:
         return False
 
-    if project_config_old['version'][0] != '0':
+    if project_config_old["version"][0] != "0":
         return False
 
     # Check if the current project.json has 'state_version' == 1.
-    with open(Path(fp, 'project.json'), 'r') as f:
+    with open(Path(fp, "project.json"), "r") as f:
         project_config_current = json.load(f)
 
     try:
-        current_state_version = project_config_current['state_version']
+        current_state_version = project_config_current["state_version"]
     except KeyError:
         return False
 
     if current_state_version[0] == "1":
         return True
     else:
         return False
```

### Comparing `asreview-1.2.1/asreview/state/sqlstate.py` & `asreview-1.3a0/asreview/state/sqlstate.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,23 +31,34 @@
     # the mapping of record identifiers to row numbers
     "record_table",
     # the latest probabilities.
     "last_probabilities",
     # the latest ranking.
     "last_ranking",
     # the record ids whose labeling decision was changed.
-    "decision_changes"
+    "decision_changes",
 ]
 
 RESULTS_TABLE_COLUMNS = [
-    "record_id", "label", "classifier", "query_strategy", "balance_strategy",
-    "feature_extraction", "training_set", "labeling_time", "notes"
+    "record_id",
+    "label",
+    "classifier",
+    "query_strategy",
+    "balance_strategy",
+    "feature_extraction",
+    "training_set",
+    "labeling_time",
+    "notes",
+]
+SETTINGS_METADATA_KEYS = [
+    "settings",
+    "state_version",
+    "software_version",
+    "model_has_trained",
 ]
-SETTINGS_METADATA_KEYS = ["settings", "state_version", "software_version",
-                          "model_has_trained"]
 
 
 class SQLiteState(BaseState):
     """Class for storing the review state.
 
     The results are stored in a sqlite database.
 
@@ -70,46 +81,46 @@
         Number of priors. If priors have not been selected returns None.
     exist_new_labeled_records: bool
         Have there been labeled records added to the state since the last time
         a model ranking was added to the state?
     model_has_trained: bool
         Has the ranking by a model been added to the state?
     """
+
     def __init__(self, read_only=True):
         super(SQLiteState, self).__init__(read_only=read_only)
 
-# INTERNAL PATHS AND CONNECTIONS
+    # INTERNAL PATHS AND CONNECTIONS
 
     def _connect_to_sql(self):
         """Get a connection to the SQLite database.
 
         Returns
         -------
         sqlite3.Connection
             Connection to the the SQLite database.
             The connection is read only if self.read_only is true.
         """
         if self.read_only:
-            con = sqlite3.connect(f"file:{str(self._sql_fp)}?mode=ro",
-                                  uri=True)
+            con = sqlite3.connect(f"file:{str(self._sql_fp)}?mode=ro", uri=True)
         else:
             con = sqlite3.connect(str(self._sql_fp))
         return con
 
     @property
     def _sql_fp(self):
         """Get the path to the sqlite database."""
 
-        return Path(self.review_dir, 'results.sql')
+        return Path(self.review_dir, "results.sql")
 
     @property
     def _settings_metadata_fp(self):
         """Get the path to the settings and metadata json file."""
 
-        return Path(self.review_dir, 'settings_metadata.json')
+        return Path(self.review_dir, "settings_metadata.json")
 
     def _create_new_state_file(self, working_dir, review_id):
         """Create the files for storing a new state given an review_id.
 
         Stages:
         1: create result structure
         2: create model settings
@@ -121,74 +132,84 @@
             Review folder location.
         review_id: str
             Identifier of the review.
         """
         if self.read_only:
             raise ValueError("Can't create new state file in read_only mode.")
 
-        self.review_dir = Path(working_dir, 'reviews', review_id)
+        self.review_dir = Path(working_dir, "reviews", review_id)
 
         # create folder in the folder `results` with the name of result_id
         self._sql_fp.parent.mkdir(parents=True, exist_ok=True)
 
         # Create results table.
         con = self._connect_to_sql()
         try:
             cur = con.cursor()
 
             # Create the results table.
-            cur.execute("""CREATE TABLE results
+            cur.execute(
+                """CREATE TABLE results
                                 (record_id INTEGER,
                                 label INTEGER,
                                 classifier TEXT,
                                 query_strategy TEXT,
                                 balance_strategy TEXT,
                                 feature_extraction TEXT,
                                 training_set INTEGER,
                                 labeling_time INTEGER,
-                                notes TEXT)""")
+                                notes TEXT)"""
+            )
 
             # Create the record table.
-            cur.execute("""CREATE TABLE record_table
-                                (record_id INT)""")
+            cur.execute(
+                """CREATE TABLE record_table
+                                (record_id INT)"""
+            )
 
             # Create the last_probabilities table.
-            cur.execute("""CREATE TABLE last_probabilities
-                                (proba REAL)""")
+            cur.execute(
+                """CREATE TABLE last_probabilities
+                                (proba REAL)"""
+            )
 
             # Create the last_ranking table.
-            cur.execute('''CREATE TABLE last_ranking
+            cur.execute(
+                """CREATE TABLE last_ranking
                                 (record_id INTEGER,
                                 ranking INT,
                                 classifier TEXT,
                                 query_strategy TEXT,
                                 balance_strategy TEXT,
                                 feature_extraction TEXT,
                                 training_set INTEGER,
-                                time INTEGER)''')
+                                time INTEGER)"""
+            )
 
             # Create the table of changed decisions.
-            cur.execute('''CREATE TABLE decision_changes
+            cur.execute(
+                """CREATE TABLE decision_changes
                                 (record_id INTEGER,
                                 new_label INTEGER,
-                                time INTEGER)''')
+                                time INTEGER)"""
+            )
 
             con.commit()
             con.close()
         except sqlite3.Error as e:
             con.close()
             raise e
 
         # Create settings_metadata.json file
         # content of the settings is added later
         self.settings_metadata = {
             "settings": None,
             "state_version": "1",
-            "software_version": get_versions()['version'],
-            "model_has_trained": False
+            "software_version": get_versions()["version"],
+            "model_has_trained": False,
         }
 
         with open(self._settings_metadata_fp, "w") as f:
             json.dump(self.settings_metadata, f)
 
     def _restore(self, working_dir, review_id):
         """
@@ -198,81 +219,90 @@
         ---------
         review_dir: str, pathlib.Path
             Review folder location.
         review_id: str
             Identifier of the review.
         """
         # store filepath
-        self.review_dir = Path(working_dir, 'reviews', review_id)
+        self.review_dir = Path(working_dir, "reviews", review_id)
 
         # If state already exist
         if not working_dir.is_dir():
             raise StateNotFoundError(f"Project {working_dir} doesn't exist.")
 
         if not self._sql_fp.parent.is_dir():
-            raise StateNotFoundError(
-                f"Review with id {review_id} doesn't exist.")
+            raise StateNotFoundError(f"Review with id {review_id} doesn't exist.")
 
         # Cache the settings.
         try:
             with open(self._settings_metadata_fp, "r") as f:
                 self.settings_metadata = json.load(f)
         except FileNotFoundError:
             raise AttributeError(
-                "'settings_metadata.json' not found in the state file.")
+                "'settings_metadata.json' not found in the state file."
+            )
 
         try:
             if not self._is_valid_version():
                 raise ValueError(
                     f"State cannot be read: state version {self.version}, "
-                    f"state file version {self.version}.")
+                    f"state file version {self.version}."
+                )
         except AttributeError as err:
-            raise ValueError(
-                f"Unexpected error when opening state file: {err}")
+            raise ValueError(f"Unexpected error when opening state file: {err}")
 
         self._is_valid_state()
 
     def _is_valid_state(self):
         con = self._connect_to_sql()
         cur = con.cursor()
         column_names = cur.execute("PRAGMA table_info(results)").fetchall()
         table_names = cur.execute(
-            "SELECT name FROM sqlite_master WHERE type='table';").fetchall()
+            "SELECT name FROM sqlite_master WHERE type='table';"
+        ).fetchall()
         con.close()
 
         # Check if all required tables are present.
         table_names = [tup[0] for tup in table_names]
-        missing_tables = [table for table in REQUIRED_TABLES
-                          if table not in table_names]
+        missing_tables = [
+            table for table in REQUIRED_TABLES if table not in table_names
+        ]
         if missing_tables:
             raise StateError(
                 f"The SQL file should contain tables named "
-                f"'{' '.join(missing_tables)}'.")
+                f"'{' '.join(missing_tables)}'."
+            )
 
         # Check if all required columns are present in results.
         column_names = [tup[1] for tup in column_names]
-        missing_columns = [col for col in RESULTS_TABLE_COLUMNS
-                           if col not in column_names]
+        missing_columns = [
+            col for col in RESULTS_TABLE_COLUMNS if col not in column_names
+        ]
         if missing_columns:
             raise StateError(
                 f"The results table does not contain the columns "
-                f"{' '.join(missing_columns)}.")
+                f"{' '.join(missing_columns)}."
+            )
 
         # Check settings_metadata contains the required keys.
-        missing_keys = [key for key in SETTINGS_METADATA_KEYS
-                        if key not in self.settings_metadata.keys()]
+        missing_keys = [
+            key
+            for key in SETTINGS_METADATA_KEYS
+            if key not in self.settings_metadata.keys()
+        ]
         if missing_keys:
             raise StateError(
                 f"The keys {' '.join(missing_keys)} were not found in "
-                f"settings_metadata.")
+                f"settings_metadata."
+            )
 
     def close(self):
         pass
 
-# PROPERTIES
+    # PROPERTIES
 
     def _is_valid_version(self):
         """Check compatibility of state version."""
         return self.version[0] == "1"
 
     @property
     def version(self):
@@ -284,15 +314,16 @@
             Returns the version of the state.
 
         """
         try:
             return self.settings_metadata["state_version"]
         except KeyError:
             raise AttributeError(
-                "'settings_metadata.json' does not contain 'state_version'.")
+                "'settings_metadata.json' does not contain 'state_version'."
+            )
 
     @property
     def settings(self):
         """Settings of the ASReview pipeline.
 
         Example
         -------
@@ -313,26 +344,25 @@
             'mix_ratio': 0.95}
             feature_param     : {}
             balance_param     : {'a': 2.155, 'alpha': 0.94, ... 'gamma': 2.0,
             'shuffle': True}
             abstract_only     : False
 
         """
-        settings = self.settings_metadata['settings']
+        settings = self.settings_metadata["settings"]
         if settings is None:
             return None
         return ASReviewSettings(**settings)
 
     @settings.setter
     def settings(self, settings):
         if isinstance(settings, ASReviewSettings):
             self._add_settings_metadata("settings", settings.to_dict())
         else:
-            raise ValueError(
-                "'settings' should be an ASReviewSettings object.")
+            raise ValueError("'settings' should be an ASReviewSettings object.")
 
     @property
     def n_records(self):
         """Number of records in the loop.
 
         Returns
         -------
@@ -366,16 +396,15 @@
         Returns
         -------
         int
             Number of records which were added as prior knowledge.
         """
         con = self._connect_to_sql()
         cur = con.cursor()
-        cur.execute(
-            "SELECT COUNT (*) FROM results WHERE query_strategy='prior'")
+        cur.execute("SELECT COUNT (*) FROM results WHERE query_strategy='prior'")
         n = cur.fetchone()
         con.close()
         n = n[0]
 
         if n == 0:
             return None
         return n
@@ -385,24 +414,24 @@
         """Return True if there are new labeled records.
 
         Return True if there are any record labels added since the last time
         the model ranking was added to the state. Also returns True if no
         model was trained yet, but priors have been added.
         """
         labeled = self.get_labeled()
-        last_training_set = self.get_last_ranking()['training_set']
+        last_training_set = self.get_last_ranking()["training_set"]
         if last_training_set.empty:
             return len(labeled) > 0
         else:
             return len(labeled) > last_training_set.iloc[0]
 
     @property
     def model_has_trained(self):
         """Return True if there is data of a trained model in the state."""
-        return self.settings_metadata['model_has_trained']
+        return self.settings_metadata["model_has_trained"]
 
     def _add_settings_metadata(self, key, value):
         """Add information to the settings_metadata dictionary."""
         if self.read_only:
             raise ValueError("Can't change settings in read only mode.")
         self.settings_metadata[key] = value
 
@@ -413,56 +442,62 @@
         """Add the record table to the state.
 
         Arguments
         ---------
         record_ids: list, np.array
             List containing all record ids of the dataset.
         """
-        record_sql_input = [(int(record_id), ) for record_id in record_ids]
+        record_sql_input = [(int(record_id),) for record_id in record_ids]
 
         con = self._connect_to_sql()
         cur = con.cursor()
         cur.execute("DELETE FROM record_table")
         cur.executemany(
-            "INSERT INTO record_table (record_id) VALUES (?)",
-            record_sql_input
+            "INSERT INTO record_table (record_id) VALUES (?)", record_sql_input
         )
         con.commit()
 
     def add_last_probabilities(self, probabilities):
         """Save the probabilities produced by the last classifier.
 
         Arguments
         ---------
         probabilities: list, np.array
             List containing the probabilities for every record.
         """
-        proba_sql_input = [(proba, ) for proba in probabilities]
+        proba_sql_input = [(proba,) for proba in probabilities]
 
         con = self._connect_to_sql()
         cur = con.cursor()
 
         # Check that the number of rows in the table is 0 (if the table is not
         # yet populated), or that it's equal to len(probabilities).
         cur.execute("SELECT COUNT (*) FROM last_probabilities")
         proba_length = cur.fetchone()[0]
         if not ((proba_length == 0) or (proba_length == len(proba_sql_input))):
             raise ValueError(
                 f"There are {proba_length} probabilities in the database, "
-                f"but 'probabilities' has length {len(probabilities)}")
+                f"but 'probabilities' has length {len(probabilities)}"
+            )
 
         cur.execute("""DELETE FROM last_probabilities""")
         cur.executemany(
-            "INSERT INTO last_probabilities (proba) VALUES (?)",
-            proba_sql_input
+            "INSERT INTO last_probabilities (proba) VALUES (?)", proba_sql_input
         )
         con.commit()
 
-    def add_last_ranking(self, ranked_record_ids, classifier, query_strategy,
-                         balance_strategy, feature_extraction, training_set):
+    def add_last_ranking(
+        self,
+        ranked_record_ids,
+        classifier,
+        query_strategy,
+        balance_strategy,
+        feature_extraction,
+        training_set,
+    ):
         """Save the ranking of the last iteration of the model.
 
         Save the ranking of the last iteration of the model, in the ranking
         order, so the record on row 0 is ranked first by the model.
 
         Arguments
         ---------
@@ -478,61 +513,74 @@
             Name of the feature extraction method of the model.
         training_set: int
             Number of labeled records available at the time of training.
         """
         record_ids = self.get_record_table()
 
         if len(record_ids) != len(ranked_record_ids):
-            raise ValueError("The ranking should have the same length as the "
-                             "record table.")
+            raise ValueError(
+                "The ranking should have the same length as the " "record table."
+            )
 
         ranking = range(len(record_ids))
         classifiers = [classifier for _ in record_ids]
         query_strategies = [query_strategy for _ in record_ids]
         balance_strategies = [balance_strategy for _ in record_ids]
         feature_extractions = [feature_extraction for _ in record_ids]
         training_sets = [int(training_set) for _ in record_ids]
         ranking_times = [datetime.now()] * len(record_ids)
 
         # Create the database rows.
-        db_rows = [(int(ranked_record_ids[i]), int(ranking[i]), classifiers[i],
-                    query_strategies[i], balance_strategies[i],
-                    feature_extractions[i], training_sets[i], ranking_times[i])
-                   for i in range(len(record_ids))]
+        db_rows = [
+            (
+                int(ranked_record_ids[i]),
+                int(ranking[i]),
+                classifiers[i],
+                query_strategies[i],
+                balance_strategies[i],
+                feature_extractions[i],
+                training_sets[i],
+                ranking_times[i],
+            )
+            for i in range(len(record_ids))
+        ]
 
         con = self._connect_to_sql()
         cur = con.cursor()
         cur.execute("DELETE FROM last_ranking")
         cur.executemany(
-            ("INSERT INTO last_ranking (record_id, ranking, classifier, "
-             "query_strategy, balance_strategy, feature_extraction, "
-             "training_set, time) VALUES (?, ?, ?, ?, ?, ?, ?, ?)"),
-            db_rows
+            (
+                "INSERT INTO last_ranking (record_id, ranking, classifier, "
+                "query_strategy, balance_strategy, feature_extraction, "
+                "training_set, time) VALUES (?, ?, ?, ?, ?, ?, ?, ?)"
+            ),
+            db_rows,
         )
         con.commit()
         con.close()
 
         # If it's the first ranking table to be added, set model_has_trained.
         if not self.model_has_trained:
-            self._add_settings_metadata('model_has_trained', True)
+            self._add_settings_metadata("model_has_trained", True)
 
     def add_note(self, note, record_id):
         """Add a text note to save with a labeled record.
 
         Arguments
         ---------
         note: str
             Text note to save.
         record_id: int
             Identifier of the record to which the note should be added.
         """
         con = self._connect_to_sql()
         cur = con.cursor()
-        cur.execute("UPDATE results SET notes = ? WHERE record_id = ?",
-                    (note, record_id))
+        cur.execute(
+            "UPDATE results SET notes = ? WHERE record_id = ?", (note, record_id)
+        )
         con.commit()
         con.close()
 
     def add_labeling_data(self, record_ids, labels, notes=None, prior=False):
         """Add the data corresponding to a labeling action to the state file.
 
         Arguments
@@ -562,41 +610,56 @@
         n_records_labeled = len(record_ids)
 
         pool, _, pending = self.get_pool_labeled_pending()
 
         if prior:
             # Check that the record_ids are in the pool.
             if not all(record_id in pool.values for record_id in record_ids):
-                raise ValueError("Labeling priors, but not all "
-                                 "record_ids were found in the pool.")
+                raise ValueError(
+                    "Labeling priors, but not all " "record_ids were found in the pool."
+                )
 
-            query_strategies = ['prior' for _ in record_ids]
+            query_strategies = ["prior" for _ in record_ids]
             training_sets = [-1 for _ in record_ids]
-            data = [(int(record_ids[i]), int(labels[i]), query_strategies[i],
-                     training_sets[i], labeling_times[i], notes[i])
-                    for i in range(n_records_labeled)]
+            data = [
+                (
+                    int(record_ids[i]),
+                    int(labels[i]),
+                    query_strategies[i],
+                    training_sets[i],
+                    labeling_times[i],
+                    notes[i],
+                )
+                for i in range(n_records_labeled)
+            ]
 
             # If prior, we need to insert new records into the database.
-            query = ("INSERT INTO results (record_id, label, query_strategy, "
-                     "training_set, labeling_time, notes) "
-                     "VALUES (?, ?, ?, ?, ?, ?)")
+            query = (
+                "INSERT INTO results (record_id, label, query_strategy, "
+                "training_set, labeling_time, notes) "
+                "VALUES (?, ?, ?, ?, ?, ?)"
+            )
 
         else:
             # Check that the record_ids are pending.
-            if not all(record_id in pending.values
-                       for record_id in record_ids):
-                raise ValueError("Labeling records, but not all "
-                                 "record_ids were pending.")
+            if not all(record_id in pending.values for record_id in record_ids):
+                raise ValueError(
+                    "Labeling records, but not all " "record_ids were pending."
+                )
 
-            data = [(int(labels[i]), labeling_times[i], notes[i],
-                     int(record_ids[i])) for i in range(n_records_labeled)]
+            data = [
+                (int(labels[i]), labeling_times[i], notes[i], int(record_ids[i]))
+                for i in range(n_records_labeled)
+            ]
 
             # If not prior, we need to update records.
-            query = ("UPDATE results SET label=?, labeling_time=?, "
-                     "notes=? WHERE record_id=?")
+            query = (
+                "UPDATE results SET label=?, labeling_time=?, "
+                "notes=? WHERE record_id=?"
+            )
 
         # Add the rows to the database.
         con = self._connect_to_sql()
         cur = con.cursor()
         cur.executemany(query, data)
         con.commit()
         con.close()
@@ -611,18 +674,20 @@
         Arguments
         ----------
         rows : list of tuples
             List of tuples (record_id: int, label: int, classifier: str,
             query_strategy: str, balance_strategy: str, feature_extraction: str,
              training_set: int, labeling_time: int, notes: str).
         """
-        query = ("INSERT INTO results (record_id, label, classifier, "
-                 "query_strategy, balance_strategy, feature_extraction, "
-                 "training_set, labeling_time, notes) "
-                 "VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?)")
+        query = (
+            "INSERT INTO results (record_id, label, classifier, "
+            "query_strategy, balance_strategy, feature_extraction, "
+            "training_set, labeling_time, notes) "
+            "VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?)"
+        )
 
         con = self._connect_to_sql()
         cur = con.cursor()
         cur.executemany(query, rows)
         con.commit()
         con.close()
 
@@ -639,22 +704,26 @@
             Note to add to the record.
         """
 
         con = self._connect_to_sql()
         cur = con.cursor()
 
         # Change the label.
-        cur.execute("UPDATE results SET label = ?, notes = ? "
-                    "WHERE record_id = ?", (label, note, record_id))
+        cur.execute(
+            "UPDATE results SET label = ?, notes = ? " "WHERE record_id = ?",
+            (label, note, record_id),
+        )
 
         # Add the change to the decision changes table.
         cur.execute(
-            ("INSERT INTO decision_changes (record_id, new_label, time) "
-             "VALUES (?, ?, ?)"),
-            (record_id, label, datetime.now())
+            (
+                "INSERT INTO decision_changes (record_id, new_label, time) "
+                "VALUES (?, ?, ?)"
+            ),
+            (record_id, label, datetime.now()),
         )
 
         con.commit()
         con.close()
 
     def delete_record_labeling_data(self, record_id):
         """Delete the labeling data for the given record id.
@@ -665,21 +734,23 @@
             Identifier of the record to delete.
 
         """
         current_time = datetime.now()
 
         con = self._connect_to_sql()
         cur = con.cursor()
-        cur.execute('DELETE FROM results WHERE record_id=?', (record_id, ))
+        cur.execute("DELETE FROM results WHERE record_id=?", (record_id,))
 
         # Add the change to the decision changes table.
         cur.execute(
-            ("INSERT INTO decision_changes (record_id, new_label, time) "
-             "VALUES (?,?, ?)"),
-            (record_id, None, current_time)
+            (
+                "INSERT INTO decision_changes (record_id, new_label, time) "
+                "VALUES (?,?, ?)"
+            ),
+            (record_id, None, current_time),
         )
         con.commit()
         con.close()
 
     def get_decision_changes(self):
         """Get the record ids for any decision changes.
 
@@ -689,59 +760,58 @@
         Returns
         -------
         pd.DataFrame
             Dataframe with columns 'record_id', 'new_label', and 'time' for
             each record of which the labeling decision was changed.
         """
         con = self._connect_to_sql()
-        change_table = pd.read_sql_query('SELECT * FROM decision_changes', con)
+        change_table = pd.read_sql_query("SELECT * FROM decision_changes", con)
         con.close()
         return change_table
 
     def get_record_table(self):
         """Get the record table of the state.
 
         Returns
         -------
         pd.Series:
             Series with name 'record_id' containing the record ids.
         """
         con = self._connect_to_sql()
-        record_table = pd.read_sql_query('SELECT * FROM record_table', con)
-        record_table = record_table['record_id']
+        record_table = pd.read_sql_query("SELECT * FROM record_table", con)
+        record_table = record_table["record_id"]
         con.close()
         return record_table
 
     def get_last_probabilities(self):
         """Get the probabilities produced by the last classifier.
 
         Returns
         -------
         pd.Series:
             Series with name 'proba' containing the probabilities.
         """
         con = self._connect_to_sql()
-        last_probabilities = pd.read_sql_query(
-            'SELECT * FROM last_probabilities', con)
+        last_probabilities = pd.read_sql_query("SELECT * FROM last_probabilities", con)
         con.close()
-        return last_probabilities['proba']
+        return last_probabilities["proba"]
 
     def get_last_ranking(self):
         """Get the ranking from the state.
 
         Returns
         -------
         pd.DataFrame
             Dataframe with columns 'record_id', 'ranking', 'classifier',
             'query_strategy', 'balance_strategy', 'feature_extraction',
             'training_set' and 'time'. It has one row for each record in the
             dataset, and is ordered by ranking.
         """
         con = self._connect_to_sql()
-        last_ranking = pd.read_sql_query('SELECT * FROM last_ranking', con)
+        last_ranking = pd.read_sql_query("SELECT * FROM last_ranking", con)
         con.close()
         return last_ranking
 
     def _move_ranking_data_to_results(self, record_ids):
         """Move data from the ranking to the results table.
 
         Move the data with the given record_ids from the last_ranking table
@@ -750,29 +820,30 @@
         Arguments
         ---------
         record_ids: list
             List of record ids in last ranking whose model data should be added
             to the results table.
         """
         if self.model_has_trained:
-            record_list = [(record_id, ) for record_id in record_ids]
+            record_list = [(record_id,) for record_id in record_ids]
             con = self._connect_to_sql()
             cur = con.cursor()
             cur.executemany(
                 """INSERT INTO results (record_id, classifier, query_strategy,
                 balance_strategy, feature_extraction, training_set)
                 SELECT record_id, classifier, query_strategy,
                 balance_strategy, feature_extraction, training_set
                 FROM last_ranking
-                WHERE record_id=?""", record_list)
+                WHERE record_id=?""",
+                record_list,
+            )
             con.commit()
             con.close()
         else:
-            raise StateError("Save trained model data "
-                             "before using this function.")
+            raise StateError("Save trained model data " "before using this function.")
 
     def query_top_ranked(self, n):
         """Get the top ranked records from the ranking table.
 
         Get the top n instances from the pool according to the last ranking.
         Add the model data to the results table.
 
@@ -787,20 +858,19 @@
             List of record_ids of the top n ranked records.
         """
         if self.model_has_trained:
             pool = self.get_pool()
             top_n_records = pool[:n].to_list()
             self._move_ranking_data_to_results(top_n_records)
         else:
-            raise StateError("Save trained model data "
-                             "before using this function.")
+            raise StateError("Save trained model data " "before using this function.")
 
         return top_n_records
 
-# GET FUNCTIONS
+    # GET FUNCTIONS
     def get_data_by_query_number(self, query, columns=None):
         """Get the data of a specific query from the results table.
 
         Arguments
         ---------
         query: int
             Number of the query of which you want the data. query=0 corresponds
@@ -813,23 +883,26 @@
         pd.DataFrame
             Dataframe containing the data from the results table with the given
             query number and columns.
         """
         if columns is not None:
             if not type(columns) == list:
                 raise ValueError("The columns argument should be a list.")
-        col_query_string = '*' if columns is None else ','.join(columns)
+        col_query_string = "*" if columns is None else ",".join(columns)
 
         if query == 0:
-            sql_query = f"SELECT {col_query_string} FROM results WHERE " \
-                        f"query_strategy='prior'"
+            sql_query = (
+                f"SELECT {col_query_string} FROM results WHERE "
+                f"query_strategy='prior'"
+            )
         else:
             rowid = query + self.n_priors
-            sql_query = f"SELECT {col_query_string} FROM results WHERE " \
-                        f"rowid={rowid}"
+            sql_query = (
+                f"SELECT {col_query_string} FROM results WHERE " f"rowid={rowid}"
+            )
 
         con = self._connect_to_sql()
         data = pd.read_sql_query(sql_query, con)
         con.close()
         return data
 
     def get_data_by_record_id(self, record_id, columns=None):
@@ -844,20 +917,20 @@
 
         Returns
         -------
         pd.DataFrame
             Dataframe containing the data from the results table with the given
             record_id and columns.
         """
-        query_string = '*' if columns is None else ','.join(columns)
+        query_string = "*" if columns is None else ",".join(columns)
 
         con = self._connect_to_sql()
         data = pd.read_sql_query(
-            f'SELECT {query_string} FROM results WHERE record_id={record_id}',
-            con)
+            f"SELECT {query_string} FROM results WHERE record_id={record_id}", con
+        )
         con.close()
         return data
 
     def get_dataset(self, columns=None, priors=True, pending=False):
         """Get a subset from the results table.
 
         Can be used to get any column subset from the results table.
@@ -886,25 +959,26 @@
         if (not priors) or (not pending):
             sql_where = []
             if not priors:
                 sql_where.append("query_strategy is not 'prior'")
             if not pending:
                 sql_where.append("label is not NULL")
 
-            sql_where_str = f'WHERE {sql_where[0]}'
+            sql_where_str = f"WHERE {sql_where[0]}"
             if len(sql_where) == 2:
-                sql_where_str += f' AND {sql_where[1]}'
+                sql_where_str += f" AND {sql_where[1]}"
         else:
             sql_where_str = ""
 
         # Query the database.
-        query_string = '*' if columns is None else ','.join(columns)
+        query_string = "*" if columns is None else ",".join(columns)
         con = self._connect_to_sql()
         data = pd.read_sql_query(
-            f'SELECT {query_string} FROM results {sql_where_str}', con)
+            f"SELECT {query_string} FROM results {sql_where_str}", con
+        )
         con.close()
 
         return data
 
     def get_order_of_labeling(self, priors=True, pending=False):
         """Get full array of record id's in order that they were labeled.
 
@@ -916,32 +990,34 @@
             Whether to keep the records are pending a labeling decision.
 
         Returns
         -------
         pd.Series:
             The record_id's in the order that they were labeled.
         """
-        return self.get_dataset('record_id', priors=priors,
-                                pending=pending)['record_id']
+        return self.get_dataset("record_id", priors=priors, pending=pending)[
+            "record_id"
+        ]
 
     def get_priors(self, columns=["record_id"]):
         """Get the record ids of the priors.
 
         Returns
         -------
         pd.Series:
             The record_id's of the priors in the order they were added.
         """
 
-        query_string = '*' if columns is None else ','.join(columns)
+        query_string = "*" if columns is None else ",".join(columns)
 
         con = self._connect_to_sql()
         data = pd.read_sql_query(
-            f"SELECT {query_string} FROM results"
-            " WHERE query_strategy is 'prior'", con)
+            f"SELECT {query_string} FROM results" " WHERE query_strategy is 'prior'",
+            con,
+        )
         con.close()
 
         return data
 
     def get_labels(self, priors=True, pending=False):
         """Get the labels from the state.
 
@@ -954,16 +1030,15 @@
 
         Returns
         -------
         pd.Series:
             Series containing the labels at each labelling moment.
         """
 
-        return self.get_dataset('label', priors=priors,
-                                pending=pending)['label']
+        return self.get_dataset("label", priors=priors, pending=pending)["label"]
 
     def get_classifiers(self, priors=True, pending=False):
         """Get the classifiers from the state.
 
         Arguments
         ---------
         priors: bool
@@ -972,16 +1047,17 @@
             Whether to keep the records which are pending a labeling decision.
 
         Returns
         -------
         pd.Series:
             Series containing the classifier used at each labeling moment.
         """
-        return self.get_dataset('classifier', priors=priors,
-                                pending=pending)['classifier']
+        return self.get_dataset("classifier", priors=priors, pending=pending)[
+            "classifier"
+        ]
 
     def get_query_strategies(self, priors=True, pending=False):
         """Get the query strategies from the state.
 
         Arguments
         ---------
         priors: bool
@@ -991,16 +1067,17 @@
 
         Returns
         -------
         pd.Series:
             Series containing the query strategy used to get the record to
             query at each labeling moment.
         """
-        return self.get_dataset('query_strategy', priors=priors,
-                                pending=pending)['query_strategy']
+        return self.get_dataset("query_strategy", priors=priors, pending=pending)[
+            "query_strategy"
+        ]
 
     def get_balance_strategies(self, priors=True, pending=False):
         """Get the balance strategies from the state.
 
         Arguments
         ---------
         priors: bool
@@ -1010,16 +1087,17 @@
 
         Returns
         -------
         pd.Series:
             Series containing the balance strategy used to get the training
             data at each labeling moment.
         """
-        return self.get_dataset('balance_strategy', priors=priors,
-                                pending=pending)['balance_strategy']
+        return self.get_dataset("balance_strategy", priors=priors, pending=pending)[
+            "balance_strategy"
+        ]
 
     def get_feature_extraction(self, priors=True, pending=False):
         """Get the query strategies from the state.
 
         Arguments
         ---------
         priors: bool
@@ -1029,16 +1107,17 @@
 
         Returns
         -------
         pd.Series:
             Series containing the feature extraction method used for the
             classifier input at each labeling moment.
         """
-        return self.get_dataset('feature_extraction', priors=priors,
-                                pending=pending)['feature_extraction']
+        return self.get_dataset("feature_extraction", priors=priors, pending=pending)[
+            "feature_extraction"
+        ]
 
     def get_training_sets(self, priors=True, pending=False):
         """Get the training_sets from the state.
 
         Arguments
         ---------
         priors: bool
@@ -1048,19 +1127,19 @@
 
         Returns
         -------
         pd.Series:
             Series containing the training set on which the classifier was fit
             at each labeling moment.
         """
-        return self.get_dataset('training_set', priors=priors,
-                                pending=pending)['training_set']
+        return self.get_dataset("training_set", priors=priors, pending=pending)[
+            "training_set"
+        ]
 
-    def get_labeling_times(self, time_format='int', priors=True,
-                           pending=False):
+    def get_labeling_times(self, time_format="int", priors=True, pending=False):
         """Get the time of labeling from the state.
 
         Arguments
         ---------
         time_format: 'int' or 'datetime'
             Format of the return value. If it is 'int' you get a UTC timestamp,
             if it is 'datetime' you get datetime instead of an integer.
@@ -1071,26 +1150,26 @@
 
         Returns
         -------
         pd.Series:
             If format='int' you get a UTC timestamp (integer number of
             microseconds), if it is 'datetime' you get datetime format.
         """
-        times = self.get_dataset('labeling_time', priors=priors,
-                                 pending=pending)['labeling_time']
+        times = self.get_dataset("labeling_time", priors=priors, pending=pending)[
+            "labeling_time"
+        ]
 
         # Convert time to datetime format.
-        if time_format == 'datetime':
-            times = times.applymap(
-                lambda x: datetime.utcfromtimestamp(x / 10**6))
+        if time_format == "datetime":
+            times = times.applymap(lambda x: datetime.utcfromtimestamp(x / 10**6))
 
         return times
 
-# Get pool, labeled and pending in slightly more optimized way than via
-# get_dataset.
+    # Get pool, labeled and pending in slightly more optimized way than via
+    # get_dataset.
     def get_pool(self):
         """Get the unlabeled, not-pending records in ranking order.
 
         Get the pool of unlabeled records, not pending a labeling decision,
         in the ranking order. If you only want the records in the pool, this
         is more efficient than via 'get_pool_labeled_pending'.
 
@@ -1120,15 +1199,15 @@
                     LEFT JOIN results
                     ON record_table.record_id = results.record_id
                     WHERE results.query_strategy is null
                     """
             df = pd.read_sql_query(query, con)
 
         con.close()
-        return df['record_id']
+        return df["record_id"]
 
     def get_labeled(self):
         """Get the labeled records in order of labeling.
 
         Get the record_ids and labels of the labeled records in order of
         labeling. If you only want the labeled records, this is more efficient
         than via 'get_pool_labeled_pending'.
@@ -1158,15 +1237,15 @@
             A series containing the record_ids of the records whose label is
             pending.
         """
         con = self._connect_to_sql()
         query = """SELECT record_id FROM results WHERE label is null"""
         df = pd.read_sql_query(query, con)
         con.close()
-        return df['record_id']
+        return df["record_id"]
 
     def get_pool_labeled_pending(self):
         """Return the unlabeled pool, labeled and pending records.
 
         Convenience function to get the pool, labeled and pending records in
         one SQL query. If you only want one of these, it is more efficient to
         use the methods 'get_pool', 'get_labeled' or 'get_pending'.
@@ -1192,16 +1271,16 @@
                 LEFT JOIN last_ranking
                 ON record_table.record_id=last_ranking.record_id
                 ORDER BY label_order, ranking
                 """
 
         df = pd.read_sql_query(query, con)
         con.close()
-        labeled = df.loc[~df['label'].isna()] \
-            .loc[:, ['record_id', 'label']] \
-            .astype(int)
-        pool = df.loc[df['label_order'].isna(), 'record_id'].astype(int)
-        pending = df.loc[df['label'].isna() & ~df['query_strategy'].isna()] \
-            .loc[:, 'record_id'] \
+        labeled = df.loc[~df["label"].isna()].loc[:, ["record_id", "label"]].astype(int)
+        pool = df.loc[df["label_order"].isna(), "record_id"].astype(int)
+        pending = (
+            df.loc[df["label"].isna() & ~df["query_strategy"].isna()]
+            .loc[:, "record_id"]
             .astype(int)
+        )
 
         return pool, labeled, pending
```

### Comparing `asreview-1.2.1/asreview/state/utils.py` & `asreview-1.3a0/asreview/state/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 
 def is_zipped_project_file(fp):
     """Check if it is a zipped asreview project file."""
     if Path(fp).is_file():
         state_ext = Path(fp).suffix
 
-        if state_ext in ['.h5', '.hdf5', '.he5', '.json']:
+        if state_ext in [".h5", ".hdf5", ".he5", ".json"]:
             raise ValueError(
-                f'State file with extension {state_ext} is no longer '
-                f'supported. Migrate to the new format or '
-                'use an older version of ASReview. See LINK.')
-        elif state_ext == '.asreview':
+                f"State file with extension {state_ext} is no longer "
+                f"supported. Migrate to the new format or "
+                "use an older version of ASReview. See LINK."
+            )
+        elif state_ext == ".asreview":
             return True
         else:
-            raise ValueError(f'State file extension {state_ext} is not '
-                             f'recognized.')
+            raise ValueError(f"State file extension {state_ext} is not " f"recognized.")
     else:
         return False
 
 
 def is_valid_project_folder(fp):
     """Check of the folder contains an asreview project."""
-    if not Path(fp, 'reviews').is_dir() \
-            or not Path(fp, 'feature_matrices').is_dir():
+    if not Path(fp, "reviews").is_dir() or not Path(fp, "feature_matrices").is_dir():
         raise StateNotFoundError(
             f"There does not seem to be a valid project folder at {fp}. The "
-            f"'reviews' or 'feature_matrices' folder is missing.")
+            f"'reviews' or 'feature_matrices' folder is missing."
+        )
     else:
         return
```

### Comparing `asreview-1.2.1/asreview/types.py` & `asreview-1.3a0/asreview/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 def type_n_queries(value):
     """Custom type used for --n_queries argument.
 
     Parameters
     ----------
     value: str
         The argument value for --n_queries
 
     Returns
     -------
     type_n_queries:
         A string containing 'min' or an integer.
     """
-    if value == 'min':
+    if value == "min":
         return value
     else:
         try:
             value_i = int(value)
 
             # convert -1 to None
             if value_i == -1:
```

### Comparing `asreview-1.2.1/asreview/utils.py` & `asreview-1.3a0/asreview/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 
 def asreview_path():
     """Get the location where projects are stored.
 
     Overwrite this location by specifying the ASREVIEW_PATH enviroment
     variable.
     """
-
     if os.environ.get("ASREVIEW_PATH", None):
         asreview_path = Path(os.environ["ASREVIEW_PATH"])
     else:
         asreview_path = Path("~", ".asreview").expanduser()
 
     asreview_path.mkdir(parents=True, exist_ok=True)
 
@@ -133,16 +132,15 @@
     Parameters
     ----------
     data_home : str | None
         The path to scikit-learn data dir.
 
     """
     if data_home is None:
-        data_home = os.environ.get('ASR_DATA',
-                                   Path('~', 'asr_data'))
+        data_home = os.environ.get("ASR_DATA", Path("~", "asr_data"))
     data_home = Path(data_home).expanduser()
 
     if not data_home.exists():
         data_home.mkdir(parents=True, exist_ok=True)
 
     return data_home
 
@@ -201,68 +199,70 @@
 
     Returns
     -------
     dict:
         Dictionary with the name of the entry point as key
         and the entry point as value.
     """
-    return {
-        entry.name: entry
-        for entry in pkg_resources.iter_entry_points(entry_name)
-    }
+    return {entry.name: entry for entry in pkg_resources.iter_entry_points(entry_name)}
 
 
 def _model_class_from_entry_point(method, entry_name="asreview.models"):
     entry_points = get_entry_points(entry_name)
     try:
         return entry_points[method].load()
     except KeyError:
         raise ValueError(
             f"Error: method '{method}' is not implemented for entry point "
-            f"{entry_name}.")
+            f"{entry_name}."
+        )
     except ImportError as e:
         raise ValueError(
             f"Failed to import '{method}' model ({entry_name}) "
-            f"with the following error:\n{e}")
+            f"with the following error:\n{e}"
+        )
 
 
 def _reader_class_from_entry_point(suffix, entry_name="asreview.readers"):
     entry_points = get_entry_points(entry_name)
     try:
         return entry_points[suffix].load()
     except KeyError:
         raise ValueError(
             f"Error: suffix '{suffix}' is not implemented for entry point "
-            f"{entry_name}.")
+            f"{entry_name}."
+        )
     except ImportError as e:
         raise ValueError(
             f"Failed to import '{suffix}' reader ({entry_name}) "
-            f"with the following error:\n{e}")
+            f"with the following error:\n{e}"
+        )
 
 
 def _writer_class_from_entry_point(suffix, entry_name="asreview.writers"):
     entry_points = get_entry_points(entry_name)
     try:
         return entry_points[suffix].load()
     except KeyError:
         raise ValueError(
             f"Error: suffix '{suffix}' is not implemented for entry point "
-            f"{entry_name}.")
+            f"{entry_name}."
+        )
     except ImportError as e:
         raise ValueError(
             f"Failed to import '{suffix}' writer ({entry_name}) "
-            f"with the following error:\n{e}")
+            f"with the following error:\n{e}"
+        )
 
 
 def is_url(url):
     """Check if object is a valid url."""
     try:
         result = urlparse(url)
-        return all(getattr(result, x) != ""
-                   for x in ["scheme", "netloc", "path"])
+        return all(getattr(result, x) != "" for x in ["scheme", "netloc", "path"])
     except Exception:
         return False
 
 
 def get_random_state(random_state):
     """Create a RandomState instance.
 
@@ -279,8 +279,8 @@
 
     return random_state
 
 
 def _get_executable():
     """Get the Python executable"""
 
-    return sys.executable if sys.executable else 'python'
+    return sys.executable if sys.executable else "python"
```

### Comparing `asreview-1.2.1/asreview/webapp/__init__.py` & `asreview-1.3a0/asreview/webapp/api/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/webapp/api.py` & `asreview-1.3a0/asreview/webapp/api/projects.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,26 +13,32 @@
 # limitations under the License.
 
 import json
 import logging
 import shutil
 import subprocess
 import tempfile
+from functools import wraps
 from pathlib import Path
 from urllib.request import urlretrieve
+from uuid import NAMESPACE_URL
+from uuid import uuid5
 
 import datahugger
+import numpy as np
+import pandas as pd
 from flask import Blueprint
 from flask import abort
+from flask import current_app
 from flask import jsonify
 from flask import request
 from flask import send_file
 from flask_cors import CORS
-import numpy as np
-import pandas as pd
+from flask_login import current_user
+from sqlalchemy import and_
 from werkzeug.exceptions import InternalServerError
 from werkzeug.utils import secure_filename
 
 from asreview.config import DEFAULT_BALANCE_STRATEGY
 from asreview.config import DEFAULT_FEATURE_EXTRACTION
 from asreview.config import DEFAULT_MODEL
 from asreview.config import DEFAULT_QUERY_STRATEGY
@@ -53,53 +59,121 @@
 from asreview.models.feature_extraction import list_feature_extraction
 from asreview.models.query import get_query_model
 from asreview.models.query import list_query_strategies
 from asreview.project import ASReviewProject
 from asreview.project import ProjectNotFoundError
 from asreview.project import _create_project_id
 from asreview.project import get_project_path
-from asreview.project import is_project
+from asreview.project import get_projects
 from asreview.project import is_v0_project
-from asreview.project import list_asreview_projects
 from asreview.project import open_state
 from asreview.project import project_from_id
 from asreview.search import SearchError
 from asreview.search import fuzzy_find
 from asreview.settings import ASReviewSettings
 from asreview.state.errors import StateError
 from asreview.state.errors import StateNotFoundError
 from asreview.state.sql_converter import upgrade_asreview_project_file
 from asreview.state.sql_converter import upgrade_project_config
 from asreview.utils import _get_executable
 from asreview.utils import asreview_path
 from asreview.utils import list_reader_names
+from asreview.webapp import DB
+from asreview.webapp.authentication.login_required import asreview_login_required
+from asreview.webapp.authentication.models import Project
 from asreview.webapp.io import read_data
 
-bp = Blueprint('api', __name__, url_prefix='/api')
-CORS(bp, resources={r"*": {"origins": "*"}})
+bp = Blueprint("api", __name__, url_prefix="/api")
+CORS(
+    bp,
+    resources={
+        r"*": {
+            "origins": [
+                "http://localhost:3000",
+                "http://127.0.0.1:3000",
+                "localhost:3000",
+            ]
+        }
+    },
+    supports_credentials=True,
+)
 
-# error handlers
 
+# helper function that indicates if app is authenticated
+def app_is_authenticated(app):
+    """Checks is app is authenticated"""
+    return app.config.get("AUTHENTICATION_ENABLED", False)
 
-@bp.errorhandler(ProjectNotFoundError)
-def project_not_found(e):
 
-    message = str(e) if str(e) else "Project not found."
-    logging.error(message)
-    return jsonify(message=message), 400
+# helper functions for generating a unique uuid for an authenticated
+# project id and folder name in the asreview folder
+def _get_project_uuid(project_id, user_id=""):
+    user_uuid = uuid5(NAMESPACE_URL, str(user_id)).hex
+    return uuid5(NAMESPACE_URL, project_id + user_uuid).hex
+
+
+def _get_authenticated_folder_id(project_id, user):
+    # if we do authentication, then the project must be
+    # registered in the database
+    project_from_db = Project.query.filter(
+        Project.project_id == project_id
+    ).one_or_none()
+
+    # project exists and user -is- owner OR this is a new project
+    if (project_from_db and user == project_from_db.owner) or (project_from_db is None):
+        project_uuid = _get_project_uuid(project_id, user.id)
+
+    # project exists but user is a collaborator
+    elif project_from_db and user in project_from_db.collaborators:
+        project_uuid = _get_project_uuid(project_id, project_from_db.owner_id)
+
+    # default to project_id
+    else:
+        project_uuid = _get_project_uuid(project_id)
+
+    return project_uuid
+
+
+def project_authorization(f):
+    """Decorator function that checks if current user can access
+    a project in an authenticated situation"""
+
+    @wraps(f)
+    def decorated_function(project_id, *args, **kwargs):
+        if app_is_authenticated(current_app):
+            # find the project
+            project = Project.query.filter(
+                Project.project_id == project_id
+            ).one_or_none()
+            if project is None:
+                return jsonify({"message": "project not found"}), 404
+            # if there is a project, check if
+            all_users = set([project.owner] + project.collaborators)
+            if current_user not in all_users:
+                return jsonify({"message": "no permission"}), 403
+        return f(project_id, *args, **kwargs)
+
+    return decorated_function
 
 
 @bp.errorhandler(ValueError)
 def value_error(e):
-
     message = str(e) if str(e) else "Incorrect value."
     logging.error(message)
     return jsonify(message=message), 400
 
 
+# error handlers
+@bp.errorhandler(ProjectNotFoundError)
+def project_not_found(e):
+    message = str(e) if str(e) else "Project not found."
+    logging.error(message)
+    return jsonify(message=message), 404
+
+
 @bp.errorhandler(InternalServerError)
 def error_500(e):
     original = getattr(e, "original_exception", None)
 
     if original is None or str(e.original_exception) == "":
         # direct 500 error, such as abort(500)
         logging.error(e)
@@ -107,187 +181,261 @@
 
     # wrapped unhandled error
     logging.error(e.original_exception)
     return jsonify(message=str(e.original_exception)), 500
 
 
 # routes
-@bp.route('/projects', methods=["GET"])
+@bp.route("/projects", methods=["GET"])
+@asreview_login_required
 def api_get_projects():  # noqa: F401
-    """Get info on the article"""
-
+    """"""
     project_info = []
-    for project in list_asreview_projects():
 
-        try:
+    if app_is_authenticated(current_app):
+        # authenticated with User accounts
+        user_db_projects = list(current_user.projects) + list(current_user.involved_in)
+        project_paths = [project.project_path for project in user_db_projects]
+        owner_ids = [project.owner_id for project in user_db_projects]
+        projects = get_projects(project_paths)
+    else:
+        # force get_projects to list the .asreview folder
+        projects = get_projects(None)
+        owner_ids = [None for p in projects]
 
+    for project, owner_id in zip(projects, owner_ids):
+        try:
             project_config = project.config
 
             # upgrade info of v0 projects
             if project_config["version"].startswith("0"):
                 project_config = upgrade_project_config(project_config)
                 project_config["projectNeedsUpgrade"] = True
 
+            # add ownership information if authentication is enabled
+            if app_is_authenticated(current_app):
+                project_config["owner_id"] = owner_id
+
             logging.info("Project found: {}".format(project_config["id"]))
             project_info.append(project_config)
 
         except Exception as err:
             logging.error(err)
 
     # sort the projects based on created_at_unix
     project_info = sorted(
         project_info,
         key=lambda y: (y["created_at_unix"] is not None, y["created_at_unix"]),
-        reverse=True)
+        reverse=True,
+    )
 
     response = jsonify({"result": project_info})
-    response.headers.add('Access-Control-Allow-Origin', '*')
 
     return response
 
 
-@bp.route('/projects/stats', methods=["GET"])
+@bp.route("/projects/stats", methods=["GET"])
+@asreview_login_required
 def api_get_projects_stats():  # noqa: F401
     """Get dashboard statistics of all projects"""
 
-    stats_counter = {
-        "n_in_review": 0,
-        "n_finished": 0,
-        "n_setup": 0
-    }
+    stats_counter = {"n_in_review": 0, "n_finished": 0, "n_setup": 0}
 
-    for project in list_asreview_projects():
+    if app_is_authenticated(current_app):
+        user_db_projects = list(current_user.projects) + list(current_user.involved_in)
+        project_paths = [project.project_path for project in user_db_projects]
+    else:
+        # force get_projects to list the .asreview folder
+        project_paths = None
 
-        try:
-            project_config = project.config
+    for project in get_projects(project_paths):
+        project_config = project.config
 
-            # upgrade info of v0 projects
-            if project_config["version"].startswith("0"):
-                project_config = upgrade_project_config(project_config)
-                project_config["projectNeedsUpgrade"] = True
+        # upgrade info of v0 projects
+        if project_config["version"].startswith("0"):
+            project_config = upgrade_project_config(project_config)
+            project_config["projectNeedsUpgrade"] = True
 
-            # get dashboard statistics
-            try:
-                if project_config["reviews"][0]["status"] == "review":
-                    stats_counter["n_in_review"] += 1
-                elif project_config["reviews"][0]["status"] == "finished":
-                    stats_counter["n_finished"] += 1
-                else:
-                    stats_counter["n_setup"] += 1
-            except Exception:
+        # get dashboard statistics
+        try:
+            if project_config["reviews"][0]["status"] == "review":
+                stats_counter["n_in_review"] += 1
+            elif project_config["reviews"][0]["status"] == "finished":
+                stats_counter["n_finished"] += 1
+            else:
                 stats_counter["n_setup"] += 1
-
-        except Exception as err:
-            logging.error(err)
-            return jsonify(message=f"Failed to load dashboard statistics. {err}"), 500
+        except Exception:
+            stats_counter["n_setup"] += 1
 
     response = jsonify({"result": stats_counter})
-    response.headers.add('Access-Control-Allow-Origin', '*')
 
     return response
 
 
-@bp.route('/projects/info', methods=["POST"])
+@bp.route("/projects/info", methods=["POST"])
+@asreview_login_required
 def api_init_project():  # noqa: F401
-    """Get info on the article"""
+    """"""
 
-    project_mode = request.form['mode']
-    project_name = request.form['name']
-    project_description = request.form['description']
-    project_authors = request.form['authors']
+    project_mode = request.form["mode"]
+    project_name = request.form["name"]
+    project_description = request.form["description"]
+    project_authors = request.form["authors"]
+
+    plaintext_project_id = _create_project_id(project_name)
+
+    if (
+        not plaintext_project_id
+        and not isinstance(plaintext_project_id, str)
+        and len(plaintext_project_id) >= 3
+    ):
+        raise ValueError("Project name should be at least 3 characters.")
 
-    project_id = _create_project_id(project_name)
+    # generate a project path
+    if app_is_authenticated(current_app):
+        project_id = _get_authenticated_folder_id(plaintext_project_id, current_user)
+    else:
+        project_id = plaintext_project_id
 
-    if not project_id and not isinstance(project_id, str) \
-            and len(project_id) >= 3:
-        raise ValueError("Project name should be at least 3 characters.")
+    # get path of this project
+    project_path = get_project_path(project_id)
 
-    project = ASReviewProject.create(get_project_path(project_id),
-                                     project_id=project_id,
-                                     project_mode=project_mode,
-                                     project_name=project_name,
-                                     project_description=project_description,
-                                     project_authors=project_authors)
+    project = ASReviewProject.create(
+        project_path,
+        project_id=project_id,
+        project_mode=project_mode,
+        project_name=project_name,
+        project_description=project_description,
+        project_authors=project_authors,
+    )
+
+    # create a database entry for this project
+    if app_is_authenticated(current_app):
+        current_user.projects.append(Project(project_id=project_id))
+        DB.session.commit()
 
     response = jsonify(project.config)
 
     return response, 201
 
 
-@bp.route('/projects/<project_id>/upgrade_if_old', methods=["GET"])
+@bp.route("/projects/<project_id>/upgrade_if_old", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_upgrade_project_if_old(project):
     """Get upgrade project if it is v0.x"""
 
     if not project.config["version"].startswith("0"):
-        response = jsonify(
-            message="Can only convert v0.x projects.")
-        response.headers.add('Access-Control-Allow-Origin', '*')
+        response = jsonify(message="Can only convert v0.x projects.")
         return response, 400
 
     # errors are handled by the InternalServerError
     upgrade_asreview_project_file(project.project_path)
 
-    response = jsonify({'success': True})
-    response.headers.add('Access-Control-Allow-Origin', '*')
+    response = jsonify({"success": True})
     return response
 
 
-@bp.route('/projects/<project_id>/info', methods=["GET"])
+@bp.route("/projects/<project_id>/info", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_get_project_info(project):  # noqa: F401
-    """Get info on the article"""
-
+    """"""
     project_config = project.config
 
     # upgrade info of v0 projects
     if project_config["version"].startswith("0"):
         project_config = upgrade_project_config(project_config)
         project_config["projectNeedsUpgrade"] = True
 
+    # add user_id of owner to response if authenticated
+    if app_is_authenticated(current_app):
+        db_project = Project.query.filter(
+            Project.project_id == project.config.get("id", 0)
+        ).one_or_none()
+        if db_project:
+            project_config["ownerId"] = db_project.owner_id
+
     return jsonify(project_config)
 
 
-@bp.route('/projects/<project_id>/info', methods=["PUT"])
+@bp.route("/projects/<project_id>/info", methods=["PUT"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_update_project_info(project):  # noqa: F401
-    """Get info on the article"""
-
+    """"""
     # rename the project if project name is changed
-    if request.form.get('name', None) is not None:
-        project.rename(request.form['name'])
+    if request.form.get("name", None) is not None:
+        # get new name
+        new_project_name = request.form.get("name")
+        # if the name has been changed, process changes
+        if project.config["name"] != new_project_name:
+            old_project_id = project.config["id"]
+            plaintext_new_project_id = _create_project_id(new_project_name)
+
+            if app_is_authenticated(current_app):
+                new_project_id = _get_authenticated_folder_id(
+                    plaintext_new_project_id, current_user
+                )
+            else:
+                new_project_id = plaintext_new_project_id
+
+            new_project_path = get_project_path(new_project_id)
+            project.rename(
+                {
+                    "name": new_project_name,
+                    "project_id": new_project_id,
+                    "project_path": new_project_path,
+                }
+            )
+
+            # update project in the database
+            # ==============================
+            if app_is_authenticated(current_app):
+                Project.query.filter(
+                    and_(
+                        Project.owner_id == current_user.id,
+                        Project.project_id == old_project_id,
+                    )
+                ).update({"project_id": new_project_id})
+                DB.session.commit()
 
     # update the project info
-    project.update_config(mode=request.form['mode'],
-                          description=request.form['description'],
-                          authors=request.form['authors'])
+    project.update_config(
+        mode=request.form["mode"],
+        description=request.form["description"],
+        authors=request.form["authors"],
+    )
 
     return api_get_project_info(project.project_id)
 
 
-@bp.route('/datasets', methods=["GET"])
+@bp.route("/datasets", methods=["GET"])
+@asreview_login_required
 def api_demo_data_project():  # noqa: F401
-    """Get info on the article"""
+    """"""
 
-    subset = request.args.get('subset', None)
+    subset = request.args.get("subset", None)
 
     manager = DatasetManager()
 
     if subset == "plugin":
-
         try:
             result_datasets = manager.list(
-                exclude=["builtin", "benchmark", "benchmark-nature"])
+                exclude=["builtin", "benchmark", "benchmark-nature"]
+            )
 
         except Exception as err:
             logging.error(err)
             return jsonify(message="Failed to load plugin datasets."), 500
 
     elif subset == "benchmark":
-
         try:
             # collect the datasets metadata
             result_datasets = manager.list(include=["benchmark-nature", "benchmark"])
 
         except Exception as err:
             logging.error(err)
             return jsonify(message="Failed to load benchmark datasets."), 500
@@ -295,133 +443,130 @@
     else:
         response = jsonify(message="demo-data-loading-failed")
 
         return response, 400
 
     payload = {"result": result_datasets}
     response = jsonify(payload)
-    response.headers.add('Access-Control-Allow-Origin', '*')
     return response
 
 
-@bp.route('/projects/<project_id>/data', methods=["POST", "PUT"])
+@bp.route("/projects/<project_id>/data", methods=["POST", "PUT"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_upload_data_to_project(project):  # noqa: F401
-    """Get info on the article"""
+    """"""
 
     # get the project config to modify behavior of dataset
     project_config = project.config
 
     # remove old dataset if present
-    if "dataset_path" in project_config and \
-            project_config["dataset_path"] is not None:
+    if "dataset_path" in project_config and project_config["dataset_path"] is not None:
         logging.warning("Removing old dataset and adding new dataset.")
         project.remove_dataset()
 
     # create dataset folder if not present
     Path(project.project_path, "data").mkdir(exist_ok=True)
 
-    if request.form.get('plugin', None):
-        url = DatasetManager().find(request.form['plugin']).filepath
+    if request.form.get("plugin", None):
+        url = DatasetManager().find(request.form["plugin"]).filepath
         filename, url = _get_filename_from_url(url)
 
-    if request.form.get('benchmark', None):
-        url = DatasetManager().find(request.form['benchmark']).filepath
+    if request.form.get("benchmark", None):
+        url = DatasetManager().find(request.form["benchmark"]).filepath
         filename, url = _get_filename_from_url(url)
 
-    if request.form.get('url', None):
-
-        url = request.form.get('url')
+    if request.form.get("url", None):
+        url = request.form.get("url")
 
         # check if url value is actually DOI without netloc
         if url.startswith("10."):
             url = f"https://doi.org/{url}"
 
         filename, url = _get_filename_from_url(url)
 
-        if bool(request.form.get('validate', None)):
-
+        if bool(request.form.get("validate", None)):
             reader_keys = list_reader_names()
 
-            if filename and Path(filename).suffix and \
-                    Path(filename).suffix in reader_keys:
+            if (
+                filename
+                and Path(filename).suffix
+                and Path(filename).suffix in reader_keys
+            ):
                 return jsonify(files=[{"link": url, "name": filename}]), 201
             elif filename and not Path(filename).suffix:
                 raise BadFileFormatError("Can't determine file format.")
             else:
                 try:
                     # get file list from datahugger
                     dh = datahugger.info(url)
                     files = dh.files.copy()
 
                     for i, f in enumerate(files):
-                        files[i]["disabled"] = Path(
-                            files[i]["name"]).suffix not in reader_keys
+                        files[i]["disabled"] = (
+                            Path(files[i]["name"]).suffix not in reader_keys
+                        )
 
                     return jsonify(files=files), 201
                 except Exception:
                     raise BadFileFormatError("Can't retrieve files.")
 
-    if request.form.get('plugin', None) or request.form.get(
-            'benchmark', None) or request.form.get('url', None):
+    if (
+        request.form.get("plugin", None)
+        or request.form.get("benchmark", None)
+        or request.form.get("url", None)
+    ):
         try:
             urlretrieve(url, Path(project.project_path, "data") / filename)
-
         except Exception as err:
-
             logging.error(err)
             message = f"Can't retrieve data from URL {url}."
 
             return jsonify(message=message), 400
 
-    elif 'file' in request.files:
-
-        data_file = request.files['file']
+    elif "file" in request.files:
+        data_file = request.files["file"]
 
         # check the file is file is in a correct format
         # check_dataset(data_file)
         try:
-
             filename = secure_filename(data_file.filename)
             fp_data = Path(project.project_path, "data") / filename
 
             # save the file
             data_file.save(str(fp_data))
 
         except Exception as err:
-
             logging.error(err)
 
-            response = jsonify(
-                message=f"Failed to upload file '{filename}'. {err}")
+            response = jsonify(message=f"Failed to upload file '{filename}'. {err}")
 
             return response, 400
     else:
         response = jsonify(message="No file or dataset found to upload.")
         return response, 400
 
     if project_config["mode"] == PROJECT_MODE_EXPLORE:
-
         data_path_raw = Path(project.project_path, "data") / filename
-        data_path = data_path_raw.with_suffix('.csv')
+        data_path = data_path_raw.with_suffix(".csv")
 
         data = ASReviewData.from_file(data_path_raw)
 
         if data.labels is None:
             raise ValueError("Upload fully labeled dataset.")
 
-        data.df.rename({data.column_spec["included"]: "debug_label"},
-                       axis=1,
-                       inplace=True)
+        data.df.rename(
+            {data.column_spec["included"]: "debug_label"}, axis=1, inplace=True
+        )
         data.to_file(data_path)
 
     elif project_config["mode"] == PROJECT_MODE_SIMULATE:
-
         data_path_raw = Path(project.project_path, "data") / filename
-        data_path = data_path_raw.with_suffix('.csv')
+        data_path = data_path_raw.with_suffix(".csv")
 
         data = ASReviewData.from_file(data_path_raw)
 
         if data.labels is None:
             raise ValueError("Upload fully labeled dataset.")
 
         data.df["debug_label"] = data.df[data.column_spec["included"]]
@@ -435,314 +580,287 @@
         project.add_dataset(data_path.name)
 
     # Bad format. TODO{Jonathan} Return informative message with link.
     except BadFileFormatError as err:
         message = f"Failed to upload file '{filename}'. {err}"
         return jsonify(message=message), 400
 
-    response = jsonify({'success': True})
-    response.headers.add('Access-Control-Allow-Origin', '*')
+    response = jsonify({"success": True})
 
     return response
 
 
-@bp.route('/projects/<project_id>/data', methods=["GET"])
+@bp.route("/projects/<project_id>/data", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_get_project_data(project):  # noqa: F401
-    """Get info on the article"""
-
-    if not is_project(project.project_path):
-        response = jsonify(message="Project not found.")
-        return response, 404
+    """"""
 
     try:
-
         # get statistics of the dataset
         as_data = read_data(project)
 
         statistics = {
             "n_rows": as_data.df.shape[0],
             "n_cols": as_data.df.shape[1],
             "n_duplicates": n_duplicates(as_data),
             "filename": Path(project.config["dataset_path"]).stem,
         }
 
     except FileNotFoundError as err:
         logging.info(err)
         statistics = {"filename": None}
 
-    except Exception as err:
-        logging.error(err)
-        message = f"Failed to get file. {err}"
-        return jsonify(message=message), 400
+    return jsonify(statistics)
 
-    response = jsonify(statistics)
-    response.headers.add('Access-Control-Allow-Origin', '*')
-    return response
 
-
-@bp.route('/projects/<project_id>/dataset_writer', methods=["GET"])
+@bp.route("/projects/<project_id>/dataset_writer", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_list_dataset_writers(project):
     """List the name and label of available dataset writer"""
 
     fp_data = Path(project.config["dataset_path"])
 
-    try:
-        readers = list_readers()
-        writers = list_writers()
+    readers = list_readers()
+    writers = list_writers()
 
-        # get write format for the data file
-        write_format = None
-        for c in readers:
-            if fp_data.suffix in c.read_format:
-                if write_format is None:
-                    write_format = c.write_format
+    # get write format for the data file
+    write_format = None
+    for c in readers:
+        if fp_data.suffix in c.read_format:
+            if write_format is None:
+                write_format = c.write_format
 
-        # get available writers
-        payload = {"result": []}
-        for c in writers:
-            payload["result"].append({
+    # get available writers
+    payload = {"result": []}
+    for c in writers:
+        payload["result"].append(
+            {
                 "enabled": True if c.write_format in write_format else False,
                 "name": c.name,
                 "label": c.label,
-                "caution": c.caution if hasattr(c, "caution") else None
-            })
-
-        if not payload["result"]:
-            return jsonify(
-                message=f"No dataset writer available for {fp_data.suffix} file."
-            ), 500
-
-        # remove duplicate writers
-        payload["result"] = [
-            i for n, i in enumerate(payload["result"])
-            if i not in payload["result"][n + 1:]
-        ]
+                "caution": c.caution if hasattr(c, "caution") else None,
+            }
+        )
 
-    except Exception as err:
-        logging.error(err)
-        return jsonify(message=f"Failed to retrieve dataset writers. {err}"), 500
+    if not payload["result"]:
+        return (
+            jsonify(message=f"No dataset writer available for {fp_data.suffix} file."),
+            500,
+        )
 
-    response = jsonify(payload)
-    response.headers.add('Access-Control-Allow-Origin', '*')
-    return response
+    # remove duplicate writers
+    payload["result"] = [
+        i
+        for n, i in enumerate(payload["result"])
+        if i not in payload["result"][(n + 1) :]
+    ]
+
+    return jsonify(payload)
 
 
-@bp.route('/projects/<project_id>/search', methods=["GET"])
+@bp.route("/projects/<project_id>/search", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_search_data(project):  # noqa: F401
-    """Search for papers
-    """
-    q = request.args.get('q', default=None, type=str)
-    max_results = request.args.get('n_max', default=10, type=int)
+    """Search for papers"""
+    q = request.args.get("q", default=None, type=str)
+    max_results = request.args.get("n_max", default=10, type=int)
 
     project_mode = project.config["mode"]
 
-    try:
-        payload = {"result": []}
-        if q:
-
-            # read the dataset
-            as_data = read_data(project)
+    payload = {"result": []}
+    if q:
+        # read the dataset
+        as_data = read_data(project)
 
-            # read record_ids of labels from state
-            with open_state(project.project_path) as s:
-                labeled_record_ids = s.get_dataset(["record_id"
-                                                    ])["record_id"].to_list()
+        # read record_ids of labels from state
+        with open_state(project.project_path) as s:
+            labeled_record_ids = s.get_dataset(["record_id"])["record_id"].to_list()
 
+        try:
             # search for the keywords
-            result_idx = fuzzy_find(as_data,
-                                    q,
-                                    max_return=max_results,
-                                    exclude=labeled_record_ids,
-                                    by_index=True)
-
-            for record in as_data.record(result_idx):
-
-                debug_label = record.extra_fields.get("debug_label", None)
-                debug_label = int(debug_label) if pd.notnull(
-                    debug_label) else None
-
-                if project_mode == PROJECT_MODE_SIMULATE:
-                    # ignore existing labels
-                    included = -1
-                else:
-                    included = int(record.included)
+            result_idx = fuzzy_find(
+                as_data,
+                q,
+                max_return=max_results,
+                exclude=labeled_record_ids,
+                by_index=True,
+            )
+        except SearchError as err:
+            raise ValueError(err) from err
 
-                payload["result"].append({
+        for record in as_data.record(result_idx):
+            debug_label = record.extra_fields.get("debug_label", None)
+            debug_label = int(debug_label) if pd.notnull(debug_label) else None
+
+            if project_mode == PROJECT_MODE_SIMULATE:
+                # ignore existing labels
+                included = -1
+            else:
+                included = int(record.included)
+
+            payload["result"].append(
+                {
                     "id": int(record.record_id),
                     "title": record.title,
                     "abstract": record.abstract,
                     "authors": record.authors,
                     "keywords": record.keywords,
                     "included": included,
-                    "_debug_label": debug_label
-                })
-
-    except SearchError as search_err:
-        logging.error(search_err)
-        return jsonify(message=f"Error: {search_err}"), 500
+                    "_debug_label": debug_label,
+                }
+            )
 
-    except Exception as err:
-        logging.error(err)
-        return jsonify(message="Failed to load search results."), 500
-
-    response = jsonify(payload)
-    response.headers.add('Access-Control-Allow-Origin', '*')
-    return response
+    return jsonify(payload)
 
 
-@bp.route('/projects/<project_id>/labeled', methods=["GET"])
+@bp.route("/projects/<project_id>/labeled", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_get_labeled(project):  # noqa: F401
-    """Get all papers classified as labeled documents
-    """
+    """Get all papers classified as labeled documents"""
 
     page = request.args.get("page", default=None, type=int)
     per_page = request.args.get("per_page", default=20, type=int)
     subset = request.args.getlist("subset")
     latest_first = request.args.get("latest_first", default=1, type=int)
 
-    try:
+    with open_state(project.project_path) as s:
+        data = s.get_dataset(["record_id", "label", "query_strategy", "notes"])
+        data["prior"] = (data["query_strategy"] == "prior").astype(int)
+
+    if any(s in subset for s in ["relevant", "included"]):
+        data = data[data["label"] == 1]
+    elif any(s in subset for s in ["irrelevant", "excluded"]):
+        data = data[data["label"] == 0]
+    else:
+        data = data[~data["label"].isnull()]
 
-        with open_state(project.project_path) as s:
-            data = s.get_dataset(
-                ["record_id", "label", "query_strategy", "notes"])
-            data["prior"] = (data["query_strategy"] == "prior").astype(int)
-
-        if any(s in subset for s in ["relevant", "included"]):
-            data = data[data["label"] == 1]
-        elif any(s in subset for s in ["irrelevant", "excluded"]):
-            data = data[data["label"] == 0]
-        else:
-            data = data[~data["label"].isnull()]
+    if "note" in subset:
+        data = data[~data["notes"].isnull()]
 
-        if "note" in subset:
-            data = data[~data["notes"].isnull()]
+    if "prior" in subset:
+        data = data[data["prior"] == 1]
 
-        if "prior" in subset:
-            data = data[data["prior"] == 1]
+    if latest_first == 1:
+        data = data.iloc[::-1]
 
-        if latest_first == 1:
-            data = data.iloc[::-1]
-
-        # count labeled records and max pages
-        count = len(data)
-        if count == 0:
-            payload = {
-                "count": 0,
-                "next_page": None,
-                "previous_page": None,
-                "result": [],
-            }
-            response = jsonify(payload)
-            response.headers.add('Access-Control-Allow-Origin', '*')
-            return response
-
-        max_page_calc = divmod(count, per_page)
-        if max_page_calc[1] == 0:
-            max_page = max_page_calc[0]
-        else:
-            max_page = max_page_calc[0] + 1
+    # count labeled records and max pages
+    count = len(data)
+    if count == 0:
+        payload = {
+            "count": 0,
+            "next_page": None,
+            "previous_page": None,
+            "result": [],
+        }
+        response = jsonify(payload)
 
-        if page is not None:
-            # slice out records on specific page
-            if page <= max_page:
-                idx_start = page * per_page - per_page
-                idx_end = page * per_page
-                data = data.iloc[idx_start:idx_end, :].copy()
-            else:
-                return abort(404)
+        return response
 
-            # set next & previous page
-            if page < max_page:
-                next_page = page + 1
-                if page > 1:
-                    previous_page = page - 1
-                else:
-                    previous_page = None
-            else:
-                next_page = None
+    max_page_calc = divmod(count, per_page)
+    if max_page_calc[1] == 0:
+        max_page = max_page_calc[0]
+    else:
+        max_page = max_page_calc[0] + 1
+
+    if page is not None:
+        # slice out records on specific page
+        if page <= max_page:
+            idx_start = page * per_page - per_page
+            idx_end = page * per_page
+            data = data.iloc[idx_start:idx_end, :].copy()
+        else:
+            return abort(404)
+
+        # set next & previous page
+        if page < max_page:
+            next_page = page + 1
+            if page > 1:
                 previous_page = page - 1
+            else:
+                previous_page = None
         else:
             next_page = None
-            previous_page = None
-
-        records = read_data(project).record(data["record_id"])
+            previous_page = page - 1
+    else:
+        next_page = None
+        previous_page = None
 
-        payload = {
-            "count": count,
-            "next_page": next_page,
-            "previous_page": previous_page,
-            "result": [],
-        }
-        for i, record in zip(data.index.tolist(), records):
+    records = read_data(project).record(data["record_id"])
 
-            payload["result"].append({
+    payload = {
+        "count": count,
+        "next_page": next_page,
+        "previous_page": previous_page,
+        "result": [],
+    }
+    for i, record in zip(data.index.tolist(), records):
+        payload["result"].append(
+            {
                 "id": int(record.record_id),
                 "title": record.title,
                 "abstract": record.abstract,
                 "authors": record.authors,
                 "keywords": record.keywords,
                 "doi": record.doi,
                 "url": record.url,
                 "included": int(data.loc[i, "label"]),
                 "note": data.loc[i, "notes"],
-                "prior": int(data.loc[i, "prior"])
-            })
-
-    except Exception as err:
-        logging.error(err)
-        return jsonify(message=f"{err}"), 500
+                "prior": int(data.loc[i, "prior"]),
+            }
+        )
 
-    response = jsonify(payload)
-    response.headers.add('Access-Control-Allow-Origin', '*')
-    return response
+    return jsonify(payload)
 
 
-@bp.route('/projects/<project_id>/labeled_stats', methods=["GET"])
+@bp.route("/projects/<project_id>/labeled_stats", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_get_labeled_stats(project):  # noqa: F401
-    """Get all papers classified as prior documents
-    """
+    """Get all papers classified as prior documents"""
 
     try:
-
         with open_state(project.project_path) as s:
             data = s.get_dataset(["label", "query_strategy"])
             data_prior = data[data["query_strategy"] == "prior"]
 
-        response = jsonify({
-            "n": len(data),
-            "n_inclusions": sum(data['label'] == 1),
-            "n_exclusions": sum(data['label'] == 0),
-            "n_prior": len(data_prior),
-            "n_prior_inclusions": sum(data_prior['label'] == 1),
-            "n_prior_exclusions": sum(data_prior['label'] == 0)
-        })
+        return jsonify(
+            {
+                "n": len(data),
+                "n_inclusions": sum(data["label"] == 1),
+                "n_exclusions": sum(data["label"] == 0),
+                "n_prior": len(data_prior),
+                "n_prior_inclusions": sum(data_prior["label"] == 1),
+                "n_prior_exclusions": sum(data_prior["label"] == 0),
+            }
+        )
     except StateNotFoundError:
-        response = jsonify({
-            "n": 0,
-            "n_inclusions": 0,
-            "n_exclusions": 0,
-            "n_prior": 0,
-            "n_prior_inclusions": 0,
-            "n_prior_exclusions": 0
-        })
-
-    except Exception as err:
-        logging.error(err)
-        return jsonify(message="Failed to load prior information."), 500
-
-    response.headers.add('Access-Control-Allow-Origin', '*')
-    return response
+        return jsonify(
+            {
+                "n": 0,
+                "n_inclusions": 0,
+                "n_exclusions": 0,
+                "n_prior": 0,
+                "n_prior_inclusions": 0,
+                "n_prior_exclusions": 0,
+            }
+        )
 
 
-@bp.route('/projects/<project_id>/prior_random', methods=["GET"])
+@bp.route("/projects/<project_id>/prior_random", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_random_prior_papers(project):  # noqa: F401
     """Get a selection of random records.
 
     This set of records is extracted from the pool, but without
     the already labeled items.
     """
@@ -756,34 +874,32 @@
         pool = state.get_pool().values
 
     as_data = read_data(project)
 
     payload = {"result": []}
 
     if subset in ["relevant", "included"]:
-        rel_indices = as_data.df[
-            as_data.df["debug_label"] == 1].index.values
+        rel_indices = as_data.df[as_data.df["debug_label"] == 1].index.values
         rel_indices_pool = np.intersect1d(pool, rel_indices)
 
         if len(rel_indices_pool) == 0:
             return jsonify(payload)
         elif n > len(rel_indices_pool):
             rand_pool_relevant = np.random.choice(
-                rel_indices_pool, len(rel_indices_pool), replace=False)
+                rel_indices_pool, len(rel_indices_pool), replace=False
+            )
         else:
             rand_pool = np.random.choice(pool, n, replace=False)
-            rand_pool_relevant = np.random.choice(
-                rel_indices_pool, n, replace=False)
+            rand_pool_relevant = np.random.choice(rel_indices_pool, n, replace=False)
 
         try:
             relevant_records = as_data.record(rand_pool_relevant)
         except Exception as err:
             logging.error(err)
-            return jsonify(
-                message=f"Failed to load random records. {err}"), 500
+            return jsonify(message=f"Failed to load random records. {err}"), 500
 
         for rr in relevant_records:
             payload["result"].append(
                 {
                     "id": int(rr.record_id),
                     "title": rr.title,
                     "abstract": rr.abstract,
@@ -791,33 +907,33 @@
                     "keywords": rr.keywords,
                     "included": None,
                     "_debug_label": 1,
                 }
             )
 
     elif subset in ["irrelevant", "excluded"]:
-        irrel_indices = as_data.df[
-            as_data.df["debug_label"] == 0].index.values
+        irrel_indices = as_data.df[as_data.df["debug_label"] == 0].index.values
         irrel_indices_pool = np.intersect1d(pool, irrel_indices)
 
         if len(irrel_indices_pool) == 0:
             return jsonify(payload)
         elif n > len(irrel_indices_pool):
             rand_pool_irrelevant = np.random.choice(
-                irrel_indices_pool, len(irrel_indices_pool), replace=False)
+                irrel_indices_pool, len(irrel_indices_pool), replace=False
+            )
         else:
             rand_pool_irrelevant = np.random.choice(
-                irrel_indices_pool, n, replace=False)
+                irrel_indices_pool, n, replace=False
+            )
 
         try:
             irrelevant_records = as_data.record(rand_pool_irrelevant)
         except Exception as err:
             logging.error(err)
-            return jsonify(
-                message=f"Failed to load random records. {err}"), 500
+            return jsonify(message=f"Failed to load random records. {err}"), 500
 
         for ir in irrelevant_records:
             payload["result"].append(
                 {
                     "id": int(ir.record_id),
                     "title": ir.title,
                     "abstract": ir.abstract,
@@ -836,112 +952,96 @@
         else:
             rand_pool = np.random.choice(pool, n, replace=False)
 
         try:
             records = as_data.record(rand_pool)
         except Exception as err:
             logging.error(err)
-            return jsonify(
-                message=f"Failed to load random records. {err}"), 500
+            return jsonify(message=f"Failed to load random records. {err}"), 500
 
         for r in records:
             payload["result"].append(
                 {
                     "id": int(r.record_id),
                     "title": r.title,
                     "abstract": r.abstract,
                     "authors": r.authors,
                     "keywords": r.keywords,
                     "included": None,
                     "_debug_label": None,
                 }
             )
 
-    response = jsonify(payload)
-    response.headers.add('Access-Control-Allow-Origin', '*')
-    return response
+    return jsonify(payload)
 
 
-@bp.route('/algorithms', methods=["GET"])
+@bp.route("/algorithms", methods=["GET"])
+@asreview_login_required
 def api_list_algorithms():
     """List the names and labels of available algorithms"""
 
-    try:
-        classes = [
-            list_balance_strategies(),
-            list_classifiers(),
-            list_feature_extraction(),
-            list_query_strategies()
-        ]
-
-        payload = {
-            "balance_strategy": [],
-            "classifier": [],
-            "feature_extraction": [],
-            "query_strategy": [],
-        }
-
-        for c, key in zip(classes, payload.keys()):
-            for method in c:
-                if hasattr(method, "label"):
-                    payload[key].append({
-                        "name": method.name,
-                        "label": method.label
-                    })
-                else:
-                    payload[key].append({
-                        "name": method.name,
-                        "label": method.name
-                    })
+    classes = [
+        list_balance_strategies(),
+        list_classifiers(),
+        list_feature_extraction(),
+        list_query_strategies(),
+    ]
+
+    payload = {
+        "balance_strategy": [],
+        "classifier": [],
+        "feature_extraction": [],
+        "query_strategy": [],
+    }
 
-    except Exception as err:
-        logging.error(err)
-        return jsonify(message="Failed to retrieve algorithms."), 500
+    for c, key in zip(classes, payload.keys()):
+        for method in c:
+            if hasattr(method, "label"):
+                payload[key].append({"name": method.name, "label": method.label})
+            else:
+                payload[key].append({"name": method.name, "label": method.name})
 
-    response = jsonify(payload)
-    response.headers.add('Access-Control-Allow-Origin', '*')
-    return response
+    return jsonify(payload)
 
 
-@bp.route('/projects/<project_id>/algorithms', methods=["GET"])
+@bp.route("/projects/<project_id>/algorithms", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_get_algorithms(project):  # noqa: F401
-
     default_payload = {
         "model": DEFAULT_MODEL,
         "feature_extraction": DEFAULT_FEATURE_EXTRACTION,
         "query_strategy": DEFAULT_QUERY_STRATEGY,
-        "balance_strategy": DEFAULT_BALANCE_STRATEGY
+        "balance_strategy": DEFAULT_BALANCE_STRATEGY,
     }
 
     # check if there were algorithms stored in the state file
     try:
-
         with open_state(project.project_path) as state:
             if state.settings is not None:
                 payload = {
                     "model": state.settings.model,
                     "feature_extraction": state.settings.feature_extraction,
                     "query_strategy": state.settings.query_strategy,
-                    "balance_strategy": state.settings.balance_strategy
+                    "balance_strategy": state.settings.balance_strategy,
                 }
             else:
                 payload = default_payload
-    except (StateNotFoundError):
+    except StateNotFoundError:
         payload = default_payload
 
-    response = jsonify(payload)
-    response.headers.add('Access-Control-Allow-Origin', '*')
-    return response
+    return jsonify(payload)
 
 
-@bp.route('/projects/<project_id>/algorithms', methods=["POST"])
+@bp.route("/projects/<project_id>/algorithms", methods=["POST"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_set_algorithms(project):  # noqa: F401
-
     # TODO@{Jonathan} validate model choice on server side
     ml_model = request.form.get("model", None)
     ml_query_strategy = request.form.get("query_strategy", None)
     ml_balance_strategy = request.form.get("balance_strategy", None)
     ml_feature_extraction = request.form.get("feature_extraction", None)
 
     # create a new settings object from arguments
@@ -950,76 +1050,80 @@
         model=ml_model,
         query_strategy=ml_query_strategy,
         balance_strategy=ml_balance_strategy,
         feature_extraction=ml_feature_extraction,
         model_param=get_classifier(ml_model).param,
         query_param=get_query_model(ml_query_strategy).param,
         balance_param=get_balance_model(ml_balance_strategy).param,
-        feature_param=get_feature_model(ml_feature_extraction).param
+        feature_param=get_feature_model(ml_feature_extraction).param,
     )
 
     # save the new settings to the state file
     with open_state(project.project_path, read_only=False) as state:
         state.settings = asreview_settings
 
-    response = jsonify({'success': True})
-    response.headers.add('Access-Control-Allow-Origin', '*')
+    response = jsonify({"success": True})
+
     return response
 
 
-@bp.route('/projects/<project_id>/start', methods=["POST"])
+@bp.route("/projects/<project_id>/start", methods=["POST"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_start(project):  # noqa: F401
-    """Start training of first model or simulation.
-    """
+    """Start training of first model or simulation."""
 
     # the project is a simulation project
     if project.config["mode"] == PROJECT_MODE_SIMULATE:
-
         # get priors
         with open_state(project.project_path) as s:
             priors = s.get_priors()["record_id"].tolist()
 
         logging.info("Start simulation")
 
         try:
             datafile = project.config["dataset_path"]
             logging.info("Project data file found: {}".format(datafile))
 
             # start simulation
             py_exe = _get_executable()
-            run_command = [
-                # get executable
-                py_exe,
-                # get module
-                "-m",
-                "asreview",
-                # run simulation via cli
-                "simulate",
-                # specify dataset
-                "",
-                # specify prior indices
-                "--prior_idx"
-            ] + list(map(str, priors)) + [
-                # specify state file
-                "--state_file",
-                str(project.project_path),
-                # specify write interval
-                "--write_interval", "100"
-            ]
+            run_command = (
+                [
+                    # get executable
+                    py_exe,
+                    # get module
+                    "-m",
+                    "asreview",
+                    # run simulation via cli
+                    "simulate",
+                    # specify dataset
+                    "",
+                    # specify prior indices
+                    "--prior_idx",
+                ]
+                + list(map(str, priors))
+                + [
+                    # specify state file
+                    "--state_file",
+                    str(project.project_path),
+                    # specify write interval
+                    "--write_interval",
+                    "100",
+                ]
+            )
             subprocess.Popen(run_command)
 
         except Exception as err:
             logging.error(err)
             message = f"Failed to get data file. {err}"
             return jsonify(message=message), 400
 
     # the project is an oracle or explore project
     else:
-
         logging.info("Train first iteration of model")
         try:
             # start training the model
             py_exe = _get_executable()
             run_command = [
                 # get executable
                 py_exe,
@@ -1029,53 +1133,56 @@
                 # train the model via cli
                 "web_run_model",
                 # specify project id
                 str(project.project_path),
                 # output the error of the first model
                 "--output_error",
                 # mark the first run for status update
-                "--first_run"
+                "--first_run",
             ]
             subprocess.Popen(run_command)
 
         except Exception as err:
             logging.error(err)
             return jsonify(message="Failed to train the model."), 500
 
-    response = jsonify({'success': True})
-    response.headers.add('Access-Control-Allow-Origin', '*')
+    response = jsonify({"success": True})
+
     return response
 
 
-@bp.route('/projects/<project_id>/status', methods=["GET"])
+@bp.route("/projects/<project_id>/status", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_get_status(project):  # noqa: F401
-    """Check the status of the review
-    """
+    """Check the status of the review"""
 
     try:
-        status = project.reviews[0]['status']
+        status = project.reviews[0]["status"]
     except Exception:
         status = None
 
     if status == "error":
         error_path = project.project_path / "error.json"
         if error_path.exists():
             logging.error("Error on training")
             with open(error_path, "r") as f:
                 error_message = json.load(f)["message"]
 
             raise Exception(error_message)
 
-    response = jsonify({'status': status})
-    response.headers.add('Access-Control-Allow-Origin', '*')
+    response = jsonify({"status": status})
+
     return response
 
 
-@bp.route('/projects/<project_id>/status', methods=["PUT"])
+@bp.route("/projects/<project_id>/status", methods=["PUT"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_status_update(project):
     """Update the status of the review.
 
     The following status updates are allowed for
     oracle and explore:
     - `review` to `finished`
@@ -1094,60 +1201,61 @@
 
     current_status = project.config["reviews"][0]["status"]
     mode = project.config["mode"]
 
     if current_status == "error" and status == "setup":
         project.remove_error(status=status)
 
-        response = jsonify({'success': True})
-        response.headers.add('Access-Control-Allow-Origin', '*')
+        response = jsonify({"success": True})
+
         return response
 
     if mode == PROJECT_MODE_SIMULATE:
-        raise ValueError(
-            "Not possible to update status of simulation project.")
+        raise ValueError("Not possible to update status of simulation project.")
     else:
         if current_status == "review" and status == "finished":
             project.update_review(status=status)
         elif current_status == "finished" and status == "review":
             project.update_review(status=status)
             # ideally, also check here for empty pool
         else:
             raise ValueError(
-                f"Not possible to update status from {current_status} to {status}")
+                f"Not possible to update status from {current_status} to {status}"
+            )
+
+        response = jsonify({"success": True})
 
-        response = jsonify({'success': True})
-        response.headers.add('Access-Control-Allow-Origin', '*')
         return response
 
 
-@bp.route('/projects/import_project', methods=["POST"])
+@bp.route("/projects/import_project", methods=["POST"])
+@asreview_login_required
 def api_import_project():
     """Import uploaded project"""
 
     # raise error if file not given
-    if 'file' not in request.files:
+    if "file" not in request.files:
         response = jsonify(message="No ASReview file found to upload.")
         return response, 400
 
     try:
         project = ASReviewProject.load(
-            request.files['file'],
-            asreview_path(),
-            safe_import=True
+            request.files["file"], asreview_path(), safe_import=True
         )
 
     except Exception as err:
         logging.error(err)
         raise ValueError("Failed to import project.")
 
     return jsonify(project.config)
 
 
-@bp.route('/projects/<project_id>/export_dataset', methods=["GET"])
+@bp.route("/projects/<project_id>/export_dataset", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_export_dataset(project):
     """Export dataset with relevant/irrelevant labels"""
 
     # get the export args
     file_format = request.args.get("file_format", None)
     dataset_label = request.args.get("dataset_label", default="all")
@@ -1159,25 +1267,27 @@
     try:
         # get labels and ranking from state file
         with open_state(project.project_path) as s:
             pool, labeled, pending = s.get_pool_labeled_pending()
             # get state dataset for accessing notes
             state_df = s.get_dataset().set_index("record_id")
 
-        included = labeled[labeled['label'] == 1]
-        excluded = labeled[labeled['label'] != 1]
+        included = labeled[labeled["label"] == 1]
+        excluded = labeled[labeled["label"] != 1]
 
         if dataset_label == "relevant":
-            export_order = included['record_id'].to_list()
+            export_order = included["record_id"].to_list()
             labeled = included
         else:
-            export_order = included['record_id'].to_list() + \
-                pending.to_list() + \
-                pool.to_list() + \
-                excluded['record_id'].to_list()
+            export_order = (
+                included["record_id"].to_list()
+                + pending.to_list()
+                + pool.to_list()
+                + excluded["record_id"].to_list()
+            )
 
         # get writer corresponding to specified file format
         writers = list_writers()
         writer = None
         for c in writers:
             if writer is None:
                 if c.name == file_format:
@@ -1196,409 +1306,397 @@
                 try:
                     screening = int(col.split("_")[2])
                 except IndexError:
                     screening = 0
         screening += 1
 
         state_df.rename(
-            columns={"notes": f"exported_notes_{screening}", },
+            columns={
+                "notes": f"exported_notes_{screening}",
+            },
             inplace=True,
         )
 
         as_data.df = as_data.df.join(
-            state_df[f"exported_notes_{screening}"],
-            on="record_id"
+            state_df[f"exported_notes_{screening}"], on="record_id"
         )
 
         as_data.to_file(
             fp=tmp_path_dataset,
             labels=labeled.values.tolist(),
             ranking=export_order,
-            writer=writer)
+            writer=writer,
+        )
 
         return send_file(
             tmp_path_dataset,
             as_attachment=True,
             download_name=f"asreview_dataset_{project.project_id}.{file_format}",
-            max_age=0)
+            max_age=0,
+        )
 
     except Exception as err:
         raise Exception(f"Failed to export the {file_format} dataset. {err}")
 
 
-@bp.route('/projects/<project_id>/export_project', methods=["GET"])
+@bp.route("/projects/<project_id>/export_project", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def export_project(project):
     """Export the project file.
 
     The ASReview project file is a file with .asreview extension.
     The ASReview project file is a zipped file and contains
     all information to continue working on the project as well
-    as the orginal dataset.
+    as the original dataset.
     """
 
     # create a temp folder to zip
     tmpdir = tempfile.TemporaryDirectory()
     tmpfile = Path(tmpdir.name, project.project_id).with_suffix(".asreview")
 
-    logging.info("Saving project (temporary) to", tmpfile)
+    logging.info("Saving project (temporary) to %s", tmpfile)
     project.export(tmpfile)
 
-    return send_file(tmpfile,
-                     as_attachment=True,
-                     download_name=f"{project.project_id}.asreview",
-                     max_age=0)
+    return send_file(
+        tmpfile,
+        as_attachment=True,
+        download_name=f"{project.project_id}.asreview",
+        max_age=0,
+    )
 
 
 def _get_stats(project, include_priors=False):
+    if is_v0_project(project.project_path):
+        json_fp = Path(project.project_path, "result.json")
 
-    try:
-
-        if is_v0_project(project.project_path):
-            json_fp = Path(project.project_path, 'result.json')
-
-            # Check if the v0 project is in review.
-            if json_fp.exists():
-
-                with open(json_fp, 'r') as f:
-                    s = json.load(f)
-
-                # Get the labels.
-                labels = np.array([
-                    int(sample_data[1]) for query in range(len(s['results']))
-                    for sample_data in s['results'][query]['labelled']
-                ])
+        # Check if the v0 project is in review.
+        if json_fp.exists():
+            with open(json_fp, "r") as f:
+                s = json.load(f)
+
+            # Get the labels.
+            labels = np.array(
+                [
+                    int(sample_data[1])
+                    for query in range(len(s["results"]))
+                    for sample_data in s["results"][query]["labelled"]
+                ]
+            )
 
-                # Get the record table.
-                data_hash = list(s['data_properties'].keys())[0]
-                record_table = s['data_properties'][data_hash]['record_table']
+            # Get the record table.
+            data_hash = list(s["data_properties"].keys())[0]
+            record_table = s["data_properties"][data_hash]["record_table"]
 
-                n_records = len(record_table)
+            n_records = len(record_table)
 
-            # No result found.
-            else:
-                labels = np.array([])
-                n_records = 0
+        # No result found.
         else:
-            # Check if there is a review started in the project.
-            try:
-                # get label history
-                with open_state(project.project_path) as s:
-
-                    if project.config["reviews"][0]["status"] == "finished" \
-                            and project.config["mode"] == PROJECT_MODE_SIMULATE:
-                        labels = _get_labels(s, priors=include_priors)
-                    else:
-                        labels = s.get_labels(priors=include_priors)
-
-                    n_records = len(s.get_record_table())
-
-            # No state file found or not init.
-            except (StateNotFoundError, StateError):
-                labels = np.array([])
-                n_records = 0
+            labels = np.array([])
+            n_records = 0
+    else:
+        # Check if there is a review started in the project.
+        try:
+            # get label history
+            with open_state(project.project_path) as s:
+                if (
+                    project.config["reviews"][0]["status"] == "finished"
+                    and project.config["mode"] == PROJECT_MODE_SIMULATE
+                ):
+                    labels = _get_labels(s, priors=include_priors)
+                else:
+                    labels = s.get_labels(priors=include_priors)
 
-        n_included = int(sum(labels == 1))
-        n_excluded = int(sum(labels == 0))
+                n_records = len(s.get_record_table())
 
-        if n_included > 0:
-            n_since_last_relevant = int(labels.tolist()[::-1].index(1))
-        else:
-            n_since_last_relevant = 0
+        # No state file found or not init.
+        except (StateNotFoundError, StateError):
+            labels = np.array([])
+            n_records = 0
 
-    except Exception as err:
-        logging.error(err)
-        return jsonify(message="Failed to load progress statistics."), 500
+    n_included = int(sum(labels == 1))
+    n_excluded = int(sum(labels == 0))
+
+    if n_included > 0:
+        n_since_last_relevant = int(labels.tolist()[::-1].index(1))
+    else:
+        n_since_last_relevant = 0
 
     return {
         "n_included": n_included,
         "n_excluded": n_excluded,
         "n_since_last_inclusion": n_since_last_relevant,
         "n_papers": n_records,
-        "n_pool": n_records - n_excluded - n_included
+        "n_pool": n_records - n_excluded - n_included,
     }
 
 
 def _get_labels(state_obj, priors=False):
-
     # get the number of records
     n_records = state_obj.n_records
 
     # get the labels
     labels = state_obj.get_labels(priors=priors).to_list()
 
     # if less labels than records, fill with 0
     if len(labels) < n_records:
         labels += [0] * (n_records - len(labels))
         labels = pd.Series(labels)
 
     return labels
 
 
-@bp.route('/projects/<project_id>/progress', methods=["GET"])
+@bp.route("/projects/<project_id>/progress", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_get_progress_info(project):  # noqa: F401
     """Get progress statistics of a project"""
 
-    include_priors = request.args.get('priors', True, type=bool)
+    include_priors = request.args.get("priors", True, type=bool)
 
     response = jsonify(_get_stats(project, include_priors=include_priors))
-    response.headers.add('Access-Control-Allow-Origin', '*')
 
     # return a success response to the client.
     return response
 
 
-@bp.route('/projects/<project_id>/progress_density', methods=["GET"])
+@bp.route("/projects/<project_id>/progress_density", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_get_progress_density(project):
     """Get progress density of a project"""
 
-    include_priors = request.args.get('priors', False, type=bool)
+    include_priors = request.args.get("priors", False, type=bool)
 
-    try:
-        # get label history
-        with open_state(project.project_path) as s:
+    # get label history
+    with open_state(project.project_path) as s:
+        if (
+            project.config["reviews"][0]["status"] == "finished"
+            and project.config["mode"] == PROJECT_MODE_SIMULATE
+        ):
+            data = _get_labels(s, priors=include_priors)
+        else:
+            data = s.get_labels(priors=include_priors)
 
-            if project.config["reviews"][0]["status"] == "finished" \
-                    and project.config["mode"] == PROJECT_MODE_SIMULATE:
-                data = _get_labels(s, priors=include_priors)
-            else:
-                data = s.get_labels(priors=include_priors)
+    # create a dataset with the rolling mean of every 10 papers
+    df = (
+        data.to_frame(name="Relevant")
+        .reset_index(drop=True)
+        .rolling(10, min_periods=1)
+        .mean()
+    )
+    df["Total"] = df.index + 1
 
-        # create a dataset with the rolling mean of every 10 papers
-        df = data \
-            .to_frame(name="Relevant") \
-            .reset_index(drop=True) \
-            .rolling(10, min_periods=1) \
-            .mean()
-        df["Total"] = df.index + 1
-
-        # transform mean(percentage) to number
-        for i in range(0, len(df)):
-            if df.loc[i, "Total"] < 10:
-                df.loc[i, "Irrelevant"] = (
-                    1 - df.loc[i, "Relevant"]) * df.loc[i, "Total"]
-                df.loc[i,
-                       "Relevant"] = df.loc[i, "Total"] - df.loc[i,
-                                                                 "Irrelevant"]
-            else:
-                df.loc[i, "Irrelevant"] = (1 - df.loc[i, "Relevant"]) * 10
-                df.loc[i, "Relevant"] = 10 - df.loc[i, "Irrelevant"]
+    # transform mean(percentage) to number
+    for i in range(0, len(df)):
+        if df.loc[i, "Total"] < 10:
+            df.loc[i, "Irrelevant"] = (1 - df.loc[i, "Relevant"]) * df.loc[i, "Total"]
+            df.loc[i, "Relevant"] = df.loc[i, "Total"] - df.loc[i, "Irrelevant"]
+        else:
+            df.loc[i, "Irrelevant"] = (1 - df.loc[i, "Relevant"]) * 10
+            df.loc[i, "Relevant"] = 10 - df.loc[i, "Irrelevant"]
 
-        df = df.round(1).to_dict(orient="records")
-        for d in df:
-            d["x"] = d.pop("Total")
-
-        df_relevant = [{k: v
-                        for k, v in d.items() if k != "Irrelevant"}
-                       for d in df]
-        for d in df_relevant:
-            d["y"] = d.pop("Relevant")
-
-        df_irrelevant = [{k: v
-                          for k, v in d.items() if k != "Relevant"}
-                         for d in df]
-        for d in df_irrelevant:
-            d["y"] = d.pop("Irrelevant")
+    df = df.round(1).to_dict(orient="records")
+    for d in df:
+        d["x"] = d.pop("Total")
 
-        payload = {"relevant": df_relevant, "irrelevant": df_irrelevant}
+    df_relevant = [{k: v for k, v in d.items() if k != "Irrelevant"} for d in df]
+    for d in df_relevant:
+        d["y"] = d.pop("Relevant")
 
-    except Exception as err:
-        logging.error(err)
-        return jsonify(message="Failed to load progress density."), 500
+    df_irrelevant = [{k: v for k, v in d.items() if k != "Relevant"} for d in df]
+    for d in df_irrelevant:
+        d["y"] = d.pop("Irrelevant")
 
-    response = jsonify(payload)
-    response.headers.add('Access-Control-Allow-Origin', '*')
+    payload = {"relevant": df_relevant, "irrelevant": df_irrelevant}
 
-    return response
+    return jsonify(payload)
 
 
-@bp.route('/projects/<project_id>/progress_recall', methods=["GET"])
+@bp.route("/projects/<project_id>/progress_recall", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_get_progress_recall(project):
     """Get cumulative number of inclusions by ASReview/at random"""
 
-    include_priors = request.args.get('priors', False, type=bool)
+    include_priors = request.args.get("priors", False, type=bool)
 
-    try:
-        with open_state(project.project_path) as s:
+    with open_state(project.project_path) as s:
+        if (
+            project.config["reviews"][0]["status"] == "finished"
+            and project.config["mode"] == PROJECT_MODE_SIMULATE
+        ):
+            data = _get_labels(s, priors=include_priors)
+        else:
+            data = s.get_labels(priors=include_priors)
 
-            if project.config["reviews"][0]["status"] == "finished" \
-                    and project.config["mode"] == PROJECT_MODE_SIMULATE:
-                data = _get_labels(s, priors=include_priors)
-            else:
-                data = s.get_labels(priors=include_priors)
+        n_records = len(s.get_record_table())
 
-            n_records = len(s.get_record_table())
+    # create a dataset with the cumulative number of inclusions
+    df = data.to_frame(name="Relevant").reset_index(drop=True).cumsum()
+    df["Total"] = df.index + 1
+    df["Random"] = (df["Total"] * (df["Relevant"][-1:] / n_records).values).round()
 
-        # create a dataset with the cumulative number of inclusions
-        df = data \
-            .to_frame(name="Relevant") \
-            .reset_index(drop=True) \
-            .cumsum()
-        df["Total"] = df.index + 1
-        df["Random"] = (df["Total"] *
-                        (df["Relevant"][-1:] / n_records).values).round()
-
-        df = df.round(1).to_dict(orient="records")
-        for d in df:
-            d["x"] = d.pop("Total")
-
-        df_asreview = [{k: v
-                        for k, v in d.items() if k != "Random"} for d in df]
-        for d in df_asreview:
-            d["y"] = d.pop("Relevant")
-
-        df_random = [{k: v
-                      for k, v in d.items() if k != "Relevant"} for d in df]
-        for d in df_random:
-            d["y"] = d.pop("Random")
+    df = df.round(1).to_dict(orient="records")
+    for d in df:
+        d["x"] = d.pop("Total")
 
-        payload = {"asreview": df_asreview, "random": df_random}
+    df_asreview = [{k: v for k, v in d.items() if k != "Random"} for d in df]
+    for d in df_asreview:
+        d["y"] = d.pop("Relevant")
 
-    except Exception as err:
-        logging.error(err)
-        return jsonify(message="Failed to load progress recall."), 500
+    df_random = [{k: v for k, v in d.items() if k != "Relevant"} for d in df]
+    for d in df_random:
+        d["y"] = d.pop("Random")
 
-    response = jsonify(payload)
-    response.headers.add('Access-Control-Allow-Origin', '*')
+    payload = {"asreview": df_asreview, "random": df_random}
 
-    return response
+    return jsonify(payload)
 
 
-@bp.route('/projects/<project_id>/record/<doc_id>', methods=["POST", "PUT"])
+@bp.route("/projects/<project_id>/record/<doc_id>", methods=["POST", "PUT"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_classify_instance(project, doc_id):  # noqa: F401
     """Label item
 
     This request handles the document identifier and the corresponding label.
     The result is stored in a temp location. If this storage exceeds a certain
     amount of values, then the model is triggered. The values of the location
     are passed to the model and the storaged is cleared. This model will run
     in the background.
     """
     # return the combination of document_id and label.
-    record_id = int(request.form.get('doc_id'))
-    label = int(request.form.get('label'))
-    note = request.form.get('note', type=str)
+    record_id = int(request.form.get("doc_id"))
+    label = int(request.form.get("label"))
+    note = request.form.get("note", type=str)
     if not note:
         note = None
 
-    is_prior = request.form.get('is_prior', default=False)
+    is_prior = request.form.get("is_prior", default=False)
 
     retrain_model = False if is_prior == "1" else True
     prior = True if is_prior == "1" else False
 
-    if request.method == 'POST':
-
+    if request.method == "POST":
         with open_state(project.project_path, read_only=False) as state:
-
             # add the labels as prior data
-            state.add_labeling_data(record_ids=[record_id],
-                                    labels=[label],
-                                    notes=[note],
-                                    prior=prior)
-
-    elif request.method == 'PUT':
+            state.add_labeling_data(
+                record_ids=[record_id], labels=[label], notes=[note], prior=prior
+            )
 
+    elif request.method == "PUT":
         with open_state(project.project_path, read_only=False) as state:
-
             if label in [0, 1]:
                 state.update_decision(record_id, label, note=note)
             elif label == -1:
                 state.delete_record_labeling_data(record_id)
 
     if retrain_model:
-
         # retrain model
-        subprocess.Popen([
-            _get_executable(), "-m", "asreview", "web_run_model",
-            str(project.project_path)
-        ])
+        subprocess.Popen(
+            [
+                _get_executable(),
+                "-m",
+                "asreview",
+                "web_run_model",
+                str(project.project_path),
+            ]
+        )
 
-    response = jsonify({'success': True})
-    response.headers.add('Access-Control-Allow-Origin', '*')
+    response = jsonify({"success": True})
 
     return response
 
 
-@bp.route('/projects/<project_id>/get_document', methods=["GET"])
+@bp.route("/projects/<project_id>/get_document", methods=["GET"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_get_document(project):  # noqa: F401
     """Retrieve documents in order of review.
 
     After these documents were retrieved, the queue on the client side is
     updated.
     This request can get triggered after each document classification.
     Although it might be better to call this function after 20 requests on the
     client side.
     """
-    try:
-
-        with open_state(project.project_path, read_only=False) as state:
-            # First check if there is a pending record.
-            _, _, pending = state.get_pool_labeled_pending()
-            if not pending.empty:
-                record_ids = pending.to_list()
-            # Else query for a new record.
-            else:
-                record_ids = state.query_top_ranked(1)
-
-        if len(record_ids) > 0:
-            new_instance = record_ids[0]
-
-            as_data = read_data(project)
-            record = as_data.record(int(new_instance))
+    with open_state(project.project_path, read_only=False) as state:
+        # First check if there is a pending record.
+        _, _, pending = state.get_pool_labeled_pending()
+        if not pending.empty:
+            record_ids = pending.to_list()
+        # Else query for a new record.
+        else:
+            record_ids = state.query_top_ranked(1)
 
-            item = {}
-            item['title'] = record.title
-            item['authors'] = record.authors
-            item['abstract'] = record.abstract
-            item['doi'] = record.doi
-            item['url'] = record.url
+    if len(record_ids) > 0:
+        new_instance = record_ids[0]
 
-            # return the debug label
-            debug_label = record.extra_fields.get("debug_label", None)
-            item['_debug_label'] = \
-                int(debug_label) if pd.notnull(debug_label) else None
+        as_data = read_data(project)
+        record = as_data.record(int(new_instance))
 
-            item["doc_id"] = new_instance
-            pool_empty = False
-        else:
-            # end of pool
-            project.update_review(status="finished")
-            item = None
-            pool_empty = True
+        item = {}
+        item["title"] = record.title
+        item["authors"] = record.authors
+        item["abstract"] = record.abstract
+        item["doi"] = record.doi
+        item["url"] = record.url
+
+        # return the debug label
+        debug_label = record.extra_fields.get("debug_label", None)
+        item["_debug_label"] = int(debug_label) if pd.notnull(debug_label) else None
 
-    except Exception as err:
-        logging.error(err)
-        return jsonify(message=f"Failed to retrieve new records. {err}."), 500
+        item["doc_id"] = new_instance
+        pool_empty = False
+    else:
+        # end of pool
+        project.update_review(status="finished")
+        item = None
+        pool_empty = True
 
-    response = jsonify({"result": item, "pool_empty": pool_empty})
-    response.headers.add('Access-Control-Allow-Origin', '*')
-    return response
+    return jsonify({"result": item, "pool_empty": pool_empty})
 
 
-@bp.route('/projects/<project_id>/delete', methods=["DELETE"])
+@bp.route("/projects/<project_id>/delete", methods=["DELETE"])
+@asreview_login_required
+@project_authorization
 @project_from_id
 def api_delete_project(project):  # noqa: F401
-    """Get info on the article"""
-
-    # some checks to check if there is a project to delete
-    if project.project_id == "" or project.project_id is None:
-        response = jsonify(message="project-delete-failure")
-        return response, 500
+    """"""
 
     if project.project_path.exists() and project.project_path.is_dir():
         try:
+            # remove from database if applicable
+            if app_is_authenticated(current_app):
+                project = Project.query.filter(
+                    and_(
+                        Project.project_id == project.project_id,
+                        Project.owner_id == current_user.id,
+                    )
+                ).one_or_none()
+
+                if project is not None:
+                    DB.session.delete(project)
+                    DB.session.commit()
+                else:
+                    return jsonify(message="Failed to delete project in DB."), 500
+
+            # and remove the folder
             shutil.rmtree(project.project_path)
+
         except Exception as err:
             logging.error(err)
             return jsonify(message="Failed to delete project."), 500
 
-        response = jsonify({'success': True})
-        response.headers.add('Access-Control-Allow-Origin', '*')
+        response = jsonify({"success": True})
+
         return response
 
     response = jsonify(message="project-delete-failure")
     return response, 500
```

### Comparing `asreview-1.2.1/asreview/webapp/io.py` & `asreview-1.3a0/asreview/webapp/io.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,41 +17,40 @@
 import pickle
 from pathlib import Path
 
 import pandas as pd
 
 from asreview._version import get_versions
 from asreview.data import ASReviewData
+from asreview.project import ProjectNotFoundError
+from asreview.project import is_project
 
 
 class CacheDataError(Exception):
     pass
 
 
 def _get_cache_data_path(fp_data):
-
-    return Path(fp_data) \
-        .with_suffix(fp_data.suffix + ".pickle")
+    return Path(fp_data).with_suffix(fp_data.suffix + ".pickle")
 
 
 def _read_data_from_cache(fp_data, version_check=True):
-
     fp_data_pickle = _get_cache_data_path(fp_data)
 
     try:
         # get the pickle data
-        with open(fp_data_pickle, 'rb') as f_pickle_read:
+        with open(fp_data_pickle, "rb") as f_pickle_read:
             data_obj, data_obj_version = pickle.load(f_pickle_read)
 
         # validate data object
         if not isinstance(data_obj.df, pd.DataFrame):
             raise ValueError()
 
         # drop cache files generated by older versions
-        if (not version_check) or (get_versions()['version'] == data_obj_version):
+        if (not version_check) or (get_versions()["version"] == data_obj_version):
             return data_obj
 
     except FileNotFoundError:
         # file not available
         pass
     except Exception as err:
         # problem loading pickle file or outdated
@@ -62,20 +61,19 @@
         except FileNotFoundError:
             pass
 
     raise CacheDataError()
 
 
 def _write_data_to_cache(fp_data, data_obj):
-
     fp_data_pickle = _get_cache_data_path(fp_data)
 
     logging.info("Store a copy of the data in a pickle file.")
-    with open(fp_data_pickle, 'wb') as f_pickle:
-        pickle.dump((data_obj, get_versions()['version']), f_pickle)
+    with open(fp_data_pickle, "wb") as f_pickle:
+        pickle.dump((data_obj, get_versions()["version"]), f_pickle)
 
 
 def read_data(project, use_cache=True, save_cache=True):
     """Get ASReviewData object from file.
 
     Parameters
     ----------
@@ -89,17 +87,19 @@
     Returns
     -------
     ASReviewData:
         The data object for internal use in ASReview.
 
     """
 
+    if not is_project(project.project_path):
+        raise ProjectNotFoundError()
+
     try:
-        fp_data = Path(
-            project.project_path, "data", project.config["dataset_path"])
+        fp_data = Path(project.project_path, "data", project.config["dataset_path"])
     except Exception:
         raise FileNotFoundError("Dataset not found")
 
     # use cache file
     if use_cache:
         try:
             return _read_data_from_cache(fp_data)
```

### Comparing `asreview-1.2.1/asreview/webapp/run_model.py` & `asreview-1.3a0/asreview/webapp/run_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 from asreview.project import ASReviewProject
 from asreview.project import open_state
 from asreview.review.base import BaseReview
 from asreview.webapp.io import read_data
 from asreview.webapp.sqlock import SQLiteLock
 
 
-def get_lab_reviewer(as_data,
-                     project,
-                     embedding_fp=None,
-                     verbose=0,
-                     prior_idx=None,
-                     prior_record_id=None,
-                     seed=None,
-                     **kwargs):
-    """Get a review object from arguments.
-    """
+def get_lab_reviewer(
+    as_data,
+    project,
+    embedding_fp=None,
+    verbose=0,
+    prior_idx=None,
+    prior_record_id=None,
+    seed=None,
+    **kwargs,
+):
+    """Get a review object from arguments."""
 
     if len(as_data) == 0:
-        raise ValueError("Supply at least one dataset"
-                         " with at least one record.")
+        raise ValueError("Supply at least one dataset" " with at least one record.")
 
     with open_state(project) as state:
         settings = state.settings
 
     # TODO: Set random seed.
     # Initialize models.
     # random_state = get_random_state(seed)
@@ -53,30 +53,35 @@
     query_model = get_query_model(settings.query_strategy)
     balance_model = get_balance_model(settings.balance_strategy)
     feature_model = get_feature_model(settings.feature_extraction)
 
     # LSTM models need embedding matrices.
     if classifier_model.name.startswith("lstm-"):
         classifier_model.embedding_matrix = feature_model.get_embedding_matrix(
-            as_data.texts, embedding_fp)
-
-    # prior knowledge
-    if prior_idx is not None and prior_record_id is not None and \
-            len(prior_idx) > 0 and len(prior_record_id) > 0:
-        raise ValueError(
-            "Not possible to provide both prior_idx and prior_record_id"
+            as_data.texts, embedding_fp
         )
 
-    reviewer = BaseReview(as_data,
-                          project,
-                          model=classifier_model,
-                          query_model=query_model,
-                          balance_model=balance_model,
-                          feature_model=feature_model,
-                          **kwargs)
+    # prior knowledge
+    if (
+        prior_idx is not None
+        and prior_record_id is not None
+        and len(prior_idx) > 0
+        and len(prior_record_id) > 0
+    ):
+        raise ValueError("Not possible to provide both prior_idx and prior_record_id")
+
+    reviewer = BaseReview(
+        as_data,
+        project,
+        model=classifier_model,
+        query_model=query_model,
+        balance_model=balance_model,
+        feature_model=feature_model,
+        **kwargs,
+    )
     return reviewer
 
 
 def train_model(project):
     """Add the new labels to the review and do the modeling.
 
     It uses a lock to ensure only one model is running at the same time.
@@ -89,21 +94,22 @@
 
     # get file locations
     lock_file = Path(project.project_path, "lock.sqlite")
 
     # Lock so that only one training run is running at the same time.
     # It doesn't lock the flask server/client.
     with SQLiteLock(
-            lock_file, blocking=False, lock_name="training",
-            project_id=project.project_id) as lock:
-
+        lock_file, blocking=False, lock_name="training", project_id=project.project_id
+    ) as lock:
         # If the lock is not acquired, another training instance is running.
         if not lock.locked():
-            logging.info(f"Project {project.project_path} - "
-                         "Cannot acquire lock, other instance running.")
+            logging.info(
+                f"Project {project.project_path} - "
+                "Cannot acquire lock, other instance running."
+            )
             return
 
         # Check if there are new labeled records.
         with open_state(project.project_path) as state:
             exist_new_labeled_records = state.exist_new_labeled_records
 
         if exist_new_labeled_records:
@@ -112,50 +118,50 @@
 
             reviewer = get_lab_reviewer(as_data, project)
 
             # Train the model.
             reviewer.train()
         else:
             logging.info(
-                f"Project {project.project_path} - No new labels since last run.")
+                f"Project {project.project_path} - No new labels since last run."
+            )
             return
 
 
 def main(argv):
-
     # parse arguments
     parser = argparse.ArgumentParser()
     parser.add_argument("project_path", type=str, help="Project id")
     parser.add_argument(
         "--output_error",
-        dest='output_error',
-        action='store_true',
-        help="Save training error message to file.")
+        dest="output_error",
+        action="store_true",
+        help="Save training error message to file.",
+    )
     parser.add_argument(
         "--first_run",
-        dest='first_run',
-        action='store_true',
-        help="After first run, status is updated.")
+        dest="first_run",
+        action="store_true",
+        help="After first run, status is updated.",
+    )
     args = parser.parse_args(argv)
 
     project = ASReviewProject(args.project_path)
 
     try:
         train_model(project)
 
         # change the project status to review
         project.update_review(status="review")
 
     except Exception as err:
-
         # save the error to the project
         project.set_error(err, save_error_message=args.output_error)
 
         # raise the error for full traceback
         raise err
     else:
         project.update_review(status="review")
 
 
 if __name__ == "__main__":
-
     main(sys.argv)
```

### Comparing `asreview-1.2.1/asreview/webapp/sqlock.py` & `asreview-1.3a0/asreview/webapp/sqlock.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,81 +23,85 @@
     if project_id is not None:
         return f"Project {project_id} - {msg}"
 
     return msg
 
 
 def get_db(db_file):
-    db = sqlite3.connect(str(db_file), detect_types=sqlite3.PARSE_DECLTYPES)
+    db = sqlite3.connect(
+        str(db_file), check_same_thread=False, detect_types=sqlite3.PARSE_DECLTYPES
+    )
     db.row_factory = sqlite3.Row
     return db
 
 
 def release_all_locks(db_file):
     db = get_db(db_file)
-    db.execute('DELETE FROM locks;')
+    db.execute("DELETE FROM locks;")
     db.close()
 
 
-class SQLiteLock():
-    def __init__(self,
-                 db_file,
-                 lock_name="global",
-                 blocking=False,
-                 timeout=30,
-                 polling_rate=0.4,
-                 project_id=None):
+class SQLiteLock:
+    def __init__(
+        self,
+        db_file,
+        lock_name="global",
+        blocking=False,
+        timeout=30,
+        polling_rate=0.4,
+        project_id=None,
+    ):
         self.db_file = db_file
         self.lock_name = lock_name
         self.lock_acquired = False
         self.timeout = timeout
         self.polling_rate = polling_rate
         self.project_id = project_id
 
         # acquire
-        self.acquire(
-            blocking=blocking, timeout=timeout, polling_rate=polling_rate)
+        self.acquire(blocking=blocking, timeout=timeout, polling_rate=polling_rate)
 
     def acquire(self, blocking=False, timeout=30, polling_rate=0.4):
         if self.lock_acquired:
             return
 
         if not os.path.isfile(self.db_file):
             self.init_db()
 
         cur_timeout = 0
         while True and not self.lock_acquired:
             db = get_db(self.db_file)
             try:
-                db.isolation_level = 'EXCLUSIVE'
-                db.execute('BEGIN EXCLUSIVE')
-                lock_entry = db.execute('SELECT * FROM locks WHERE name = ?',
-                                        (self.lock_name, )).fetchone()
+                db.isolation_level = "EXCLUSIVE"
+                db.execute("BEGIN EXCLUSIVE")
+                lock_entry = db.execute(
+                    "SELECT * FROM locks WHERE name = ?", (self.lock_name,)
+                ).fetchone()
                 if lock_entry is None:
-                    db.execute('INSERT INTO locks (name) VALUES (?)',
-                               (self.lock_name, ))
+                    db.execute("INSERT INTO locks (name) VALUES (?)", (self.lock_name,))
                     self.lock_acquired = True
                     logging.debug(
-                        _log_msg(f"Acquired lock {self.lock_name}",
-                                 self.project_id))
+                        _log_msg(f"Acquired lock {self.lock_name}", self.project_id)
+                    )
                 db.commit()
             except sqlite3.OperationalError as e:
                 logging.error(
-                    _log_msg(f"Encountering operational error {e}",
-                             self.project_id))
+                    _log_msg(f"Encountering operational error {e}", self.project_id)
+                )
             db.close()
             if self.lock_acquired or not blocking:
                 break
             cur_timeout += polling_rate
             sleep(polling_rate)
 
     def init_db(self):
         db = get_db(self.db_file)
-        db.executescript('DROP TABLE IF EXISTS locks; '
-                         'CREATE TABLE locks (name TEXT NOT NULL);')
+        db.executescript(
+            "DROP TABLE IF EXISTS locks; " "CREATE TABLE locks (name TEXT NOT NULL);"
+        )
         db.close()
 
     def locked(self):
         return self.lock_acquired
 
     def __enter__(self):
         return self
@@ -107,19 +111,17 @@
 
     def release(self):
         if not self.locked():
             return
         while True:
             db = get_db(self.db_file)
             try:
-                db.execute('DELETE FROM locks WHERE name = ?',
-                           (self.lock_name, ))
+                db.execute("DELETE FROM locks WHERE name = ?", (self.lock_name,))
                 db.commit()
                 db.close()
                 break
             except sqlite3.OperationalError:
                 pass
             db.close()
             sleep(0.4)
-        logging.debug(
-            _log_msg(f"Released lock {self.lock_name}", self.project_id))
+        logging.debug(_log_msg(f"Released lock {self.lock_name}", self.project_id))
         self.lock_acquired = False
```

### Comparing `asreview-1.2.1/asreview/webapp/tests/__init__.py` & `asreview-1.3a0/asreview/webapp/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `asreview-1.2.1/asreview/webapp/tests/test_project.py` & `asreview-1.3a0/asreview/webapp/tests/test_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     # change default folder for projects
     os.environ["ASREVIEW_PATH"] = str(tmp_path)
 
     # Test import uploaded project
     with urlopen(url) as project_file:
         response_import = client.post(
             "/api/projects/import_project",
-            data={"file": (BytesIO(project_file.read()), "project.asreview")})
+            data={"file": (BytesIO(project_file.read()), "project.asreview")},
+        )
     json_data_import = response_import.get_json()
     assert response_import.status_code == 200
 
     project_id = json_data_import["id"]
     api_url = f"/api/projects/{project_id}"
 
     # Test get dashboard analytics
@@ -51,16 +52,15 @@
     assert "n_finished" in json_data_stats["result"]
     assert isinstance(json_data_stats["result"], dict)
 
     # Test get projects
     response_projects = client.get("/api/projects")
     json_data_projects = response_projects.get_json()
     assert "result" in json_data_projects
-    assert any(item["id"] == project_id
-               for item in json_data_projects["result"])
+    assert any(item["id"] == project_id for item in json_data_projects["result"])
 
     # Test export project before upgrade
     response_export_old_project = client.get(f"{api_url}/export_project")
     assert response_export_old_project.status_code == 200
 
     # Test upgrade project if old
     response_upgrade_if_old = client.get(f"{api_url}/upgrade_if_old")
@@ -73,22 +73,23 @@
 
     # Test get dataset writer
     response_get_writer = client.get(f"{api_url}/dataset_writer")
     json_data_get_writer = response_get_writer.get_json()
     assert isinstance(json_data_get_writer["result"], list)
 
     # Test update info of the project
-    response_update_info = client.put(f"{api_url}/info",
-                                      data={
-                                          "mode": "explore",
-                                          "name": json_data_get_info["name"],
-                                          "authors":
-                                          json_data_get_info["authors"],
-                                          "description": "Hoi Elas"
-                                      })
+    response_update_info = client.put(
+        f"{api_url}/info",
+        data={
+            "mode": "explore",
+            "name": json_data_get_info["name"],
+            "authors": json_data_get_info["authors"],
+            "description": "Hoi Elas",
+        },
+    )
     assert response_update_info.status_code == 200
 
     # Test get progress info on the article
     response_progress = client.get(f"{api_url}/progress")
     json_data_progress = response_progress.get_json()
     assert isinstance(json_data_progress, dict)
 
@@ -112,42 +113,45 @@
     assert "result" in json_data_get_document
     assert isinstance(json_data_get_document, dict)
 
     # get doc_id from the queue and label the item
     doc_id = json_data_get_document["result"]["doc_id"]
 
     # Test retrieve classification result
-    response_classify_instance = client.post(f"{api_url}/record/{doc_id}",
-                                             data={
-                                                 "doc_id": doc_id,
-                                                 "label": 1,
-                                             })
+    response_classify_instance = client.post(
+        f"{api_url}/record/{doc_id}",
+        data={
+            "doc_id": doc_id,
+            "label": 1,
+        },
+    )
     assert response_classify_instance.status_code == 200
 
     # Test update classification result
-    response_update_classify = client.put(f"{api_url}/record/{doc_id}",
-                                          data={
-                                              "doc_id": doc_id,
-                                              "label": 0,
-                                          })
+    response_update_classify = client.put(
+        f"{api_url}/record/{doc_id}",
+        data={
+            "doc_id": doc_id,
+            "label": 0,
+        },
+    )
     assert response_update_classify.status_code == 200
 
     # Test retrieve review history
     response_prior = client.get(f"{api_url}/labeled")
     json_data_prior = response_prior.get_json()
     assert "result" in json_data_prior
     assert isinstance(json_data_prior["result"], list)
 
     # Test export result
-    response_export_result_csv = client.get(
-        f"{api_url}/export_dataset?file_format=csv")
-    response_export_result_tsv = client.get(
-        f"{api_url}/export_dataset?file_format=tsv")
+    response_export_result_csv = client.get(f"{api_url}/export_dataset?file_format=csv")
+    response_export_result_tsv = client.get(f"{api_url}/export_dataset?file_format=tsv")
     response_export_result_excel = client.get(
-        f"{api_url}/export_dataset?file_format=xlsx")
+        f"{api_url}/export_dataset?file_format=xlsx"
+    )
     assert response_export_result_csv.status_code == 200
     assert response_export_result_tsv.status_code == 200
     assert response_export_result_excel.status_code == 200
 
     # Test export project
     response_export_project = client.get(f"{api_url}/export_project")
     assert response_export_project.status_code == 200
@@ -155,14 +159,13 @@
     # Test get project status
     response_status = client.get(f"{api_url}/status")
     json_data_status = response_status.get_json()
     assert "status" in json_data_status
     assert isinstance(json_data_status, dict)
 
     # Test mark project as finished
-    response_finish = client.put(f"{api_url}/status",
-                                 data={"status": "finished"})
+    response_finish = client.put(f"{api_url}/status", data={"status": "finished"})
     assert response_finish.status_code == 200
 
     # Test delete project
     response_delete = client.delete(f"{api_url}/delete")
     assert response_delete.status_code == 200
```

### Comparing `asreview-1.2.1/asreview/webapp/tests/test_webapp.py` & `asreview-1.3a0/asreview/webapp/tests/test_webapp.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 
     This test will fail if build is missing. Please run
     `python setup.py compile_assets` first.
     """
     response = client.get("/")
     html = response.data.decode()
 
-    assert "<title>ASReview LAB - A tool for AI-assisted systematic reviews</title>" in html  # noqa
+    assert (
+        "<title>ASReview LAB - A tool for AI-assisted systematic reviews</title>"
+        in html
+    )  # noqa
 
 
 def test_boot(client):
     """Test if version number is available on boot."""
     response = client.get("/boot")
     json_data = response.get_json()
```

### Comparing `asreview-1.2.1/asreview/webapp/tests/utils.py` & `asreview-1.3a0/asreview/webapp/tests/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 
 import json
 from urllib.request import urlopen
 
 
 def retrieve_project_url_github(major=None):
-    '''Retrieve .asreview file url from
-    asreview-project-files-testing GitHub repository'''
+    """Retrieve .asreview file url from
+    asreview-project-files-testing GitHub repository"""
 
     repo = "/asreview/asreview-project-files-testing"
     repo_api_url = "https://api.github.com/repos" + repo + "/git/trees/master"
     repo_url = "https://github.com" + repo + "/blob/master"
     file_type = "startreview.asreview?raw=true"
 
     json_file = json.loads(urlopen(repo_api_url).read().decode("utf-8"))["tree"]
```

### Comparing `asreview-1.2.1/asreview.egg-info/PKG-INFO` & `asreview-1.3a0/asreview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asreview
-Version: 1.2.1
+Version: 1.3a0
 Summary: ASReview LAB - A tool for AI-assisted systematic reviews
 Home-page: https://github.com/asreview/asreview
 Author: ASReview LAB developers
 Author-email: asreview@uu.nl
 Project-URL: Bug Reports, https://github.com/asreview/asreview/issues
 Project-URL: Source, https://github.com/asreview/asreview/
 Keywords: systematic review,machine-learning
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: General
 Classifier: Framework :: Flask
-Requires-Python: ~=3.8
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: sbert
 Provides-Extra: doc2vec
 Provides-Extra: tensorflow
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: all
@@ -68,15 +68,15 @@
   the performance of active learning models on fully labeled data. Simulations
   can be run in ASReview LAB or via the command line interface with more
   advanced options.
 
 
 ## Installation
 
-The ASReview software requires Python 3.8+. Detailed step-by-step instructions
+The ASReview software requires Python 3.7+. Detailed step-by-step instructions
 to install Python and ASReview are available for
 [Windows](https://asreview.ai/installation-guide-windows/) and
 [macOS](https://asreview.ai/installation-guide-macos/) users.
 
 ```bash
 pip install asreview
 ```
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: asreview Version: 1.2.1 Summary: ASReview LAB - A
+Metadata-Version: 2.1 Name: asreview Version: 1.3a0 Summary: ASReview LAB - A
 tool for AI-assisted systematic reviews Home-page: https://github.com/asreview/
 asreview Author: ASReview LAB developers Author-email: asreview@uu.nl Project-
 URL: Bug Reports, https://github.com/asreview/asreview/issues Project-URL:
 Source, https://github.com/asreview/asreview/ Keywords: systematic
 review,machine-learning Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
 Engineering :: Information Analysis Classifier: Topic :: Text Processing ::
-General Classifier: Framework :: Flask Requires-Python: ~=3.8 Description-
+General Classifier: Framework :: Flask Requires-Python: ~=3.7 Description-
 Content-Type: text/markdown Provides-Extra: sbert Provides-Extra: doc2vec
 Provides-Extra: tensorflow Provides-Extra: dev Provides-Extra: test Provides-
 Extra: all License-File: LICENSE
      [https://raw.githubusercontent.com/asreview/asreview-artwork/master/
               LogoASReview/SVG/GitHub_Repo_Card_Transparent.svg]
 ## ASReview: Active learning for Systematic Reviews [![PyPI version](https://
 badge.fury.io/py/asreview.svg)](https://badge.fury.io/py/asreview) [![Build
@@ -45,15 +45,15 @@
 implements three different modes: - **Oracle** Screen textual data in
 interaction with the active learning model. The reviewer is the 'oracle',
 making the labeling decisions. - **Exploration** Explore or demonstrate
 ASReview LAB with a completely labeled dataset. This mode is suitable for
 teaching purposes. - **Simulation** Evaluate the performance of active learning
 models on fully labeled data. Simulations can be run in ASReview LAB or via the
 command line interface with more advanced options. ## Installation The ASReview
-software requires Python 3.8+. Detailed step-by-step instructions to install
+software requires Python 3.7+. Detailed step-by-step instructions to install
 Python and ASReview are available for [Windows](https://asreview.ai/
 installation-guide-windows/) and [macOS](https://asreview.ai/installation-
 guide-macos/) users. ```bash pip install asreview ``` Upgrade ASReview with the
 following command: ```bash pip install --upgrade asreview ``` To install
 ASReview LAB with Docker, see [Install with Docker](https://
 asreview.readthedocs.io/en/latest/installation.html). ## How it works [!
 [ASReview LAB explained - animation](https://img.youtube.com/vi/k-a2SCq-LtA/
```

### Comparing `asreview-1.2.1/asreview.egg-info/SOURCES.txt` & `asreview-1.3a0/asreview.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 asreview/__init__.py
 asreview/__main__.py
+asreview/_deprecated.py
 asreview/_version.py
 asreview/compat.py
 asreview/config.py
 asreview/datasets.py
 asreview/exceptions.py
 asreview/project.py
 asreview/search.py
@@ -23,14 +24,15 @@
 asreview.egg-info/requires.txt
 asreview.egg-info/top_level.txt
 asreview/data/__init__.py
 asreview/data/base.py
 asreview/data/statistics.py
 asreview/entry_points/__init__.py
 asreview/entry_points/algorithms.py
+asreview/entry_points/auth_tool.py
 asreview/entry_points/base.py
 asreview/entry_points/lab.py
 asreview/entry_points/simulate.py
 asreview/entry_points/state_inspect.py
 asreview/io/__init__.py
 asreview/io/csv_reader.py
 asreview/io/csv_writer.py
@@ -88,18 +90,31 @@
 asreview/state/legacy/__init__.py
 asreview/state/legacy/base.py
 asreview/state/legacy/dict.py
 asreview/state/legacy/hdf5.py
 asreview/state/legacy/json.py
 asreview/state/legacy/utils.py
 asreview/webapp/__init__.py
-asreview/webapp/api.py
 asreview/webapp/io.py
 asreview/webapp/run_model.py
 asreview/webapp/sqlock.py
 asreview/webapp/start_flask.py
+asreview/webapp/api/__init__.py
+asreview/webapp/api/auth.py
+asreview/webapp/api/projects.py
+asreview/webapp/api/team.py
+asreview/webapp/authentication/__init__.py
+asreview/webapp/authentication/login_required.py
+asreview/webapp/authentication/models.py
+asreview/webapp/authentication/oauth_handler.py
 asreview/webapp/tests/__init__.py
 asreview/webapp/tests/conftest.py
-asreview/webapp/tests/test_api.py
+asreview/webapp/tests/temp_env_var.py
+asreview/webapp/tests/test_asreview_database.py
+asreview/webapp/tests/test_auth.py
+asreview/webapp/tests/test_auth_conversion.py
 asreview/webapp/tests/test_project.py
+asreview/webapp/tests/test_project_api_authenticated.py
+asreview/webapp/tests/test_project_api_unauthenticated.py
+asreview/webapp/tests/test_teams_api.py
 asreview/webapp/tests/test_webapp.py
 asreview/webapp/tests/utils.py
```

### Comparing `asreview-1.2.1/asreview.egg-info/entry_points.txt` & `asreview-1.3a0/asreview.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [asreview.datasets]
 benchmark = asreview.datasets:BenchmarkDataGroup
 benchmark-nature = asreview.datasets:NaturePublicationDataGroup
 
 [asreview.entry_points]
 algorithms = asreview.entry_points:AlgorithmsEntryPoint
+auth-tool = asreview.entry_points:AuthTool
 lab = asreview.entry_points:LABEntryPoint
 simulate = asreview.entry_points:SimulateEntryPoint
 state-inspect = asreview.entry_points:StateInspectEntryPoint
 web_run_model = asreview.entry_points:WebRunModelEntryPoint
 
 [asreview.models.balance]
 double = asreview.models.balance:DoubleBalance
```

### Comparing `asreview-1.2.1/setup.py` & `asreview-1.3a0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,45 +15,46 @@
 # based on https://github.com/pypa/sampleproject - MIT License
 
 # Always prefer setuptools over distutils
 import re
 import subprocess
 from io import open
 from os import path
+from pathlib import Path
 
 from setuptools import Command
 from setuptools import find_packages
 from setuptools import setup
 
 import versioneer
 
 
 def get_long_description():
     """Get project description based on README."""
     here = path.abspath(path.dirname(__file__))
 
     # Get the long description from the README file
-    with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+    with open(path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = f.read()
 
     # remove emoji
     long_description = re.sub(r"\:[a-z_]+\:", "", long_description)
 
     return long_description
 
 
 DEPS = {
-    "sbert": ['sentence_transformers'],
-    "doc2vec": ['gensim'],
-    "tensorflow": ['tensorflow>=2.0,<2.13.0'],
-    "dev": ['check-manifest'],
-    'test': ['coverage', 'pytest'],
+    "sbert": ["sentence_transformers"],
+    "doc2vec": ["gensim"],
+    "tensorflow": ["tensorflow~=2.0"],
+    "dev": ["black", "check-manifest", "flake8", "flake8-isort", "isort"],
+    "test": ["coverage", "pytest"],
 }
-DEPS['all'] = DEPS['sbert'] + DEPS['doc2vec'] + DEPS['dev']
-DEPS['all'] += DEPS['tensorflow']
+DEPS["all"] = DEPS["sbert"] + DEPS["doc2vec"]
+DEPS["all"] += DEPS["tensorflow"]
 
 
 class CompileAssets(Command):
     """
     Compile and build the frontend assets using npm and webpack.
 
     Registered as cmdclass in setup() so it can be called with
@@ -67,131 +68,141 @@
         """Set default values for options."""
 
     def finalize_options(self):
         """Set final values for options."""
 
     def run(self):
         """Run a command to compile and build assets."""
-        subprocess.check_call('sh ./asreview/webapp/compile_assets.sh',
-                              shell=True)
+
+        path_webapp = Path(__file__).parent / "asreview" / "webapp"
+
+        subprocess.check_call(["npm", "install"], cwd=str(path_webapp))
+        subprocess.check_call(["npm", "run-script", "build"], cwd=str(path_webapp))
 
 
 def get_cmdclass():
     cmdclass = versioneer.get_cmdclass()
     cmdclass["compile_assets"] = CompileAssets
     return cmdclass
 
 
 setup(
-    name='asreview',
+    name="asreview",
     version=versioneer.get_version(),
     cmdclass=get_cmdclass(),
-    description='ASReview LAB - A tool for AI-assisted systematic reviews',
+    description="ASReview LAB - A tool for AI-assisted systematic reviews",
     long_description=get_long_description(),
-    long_description_content_type='text/markdown',
-    url='https://github.com/asreview/asreview',
-    author='ASReview LAB developers',
-    author_email='asreview@uu.nl',
+    long_description_content_type="text/markdown",
+    url="https://github.com/asreview/asreview",
+    author="ASReview LAB developers",
+    author_email="asreview@uu.nl",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Scientific/Engineering :: Artificial Intelligence',
-        'Topic :: Scientific/Engineering :: Information Analysis',
-        'Topic :: Text Processing :: General',
-        'Framework :: Flask',
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Text Processing :: General",
+        "Framework :: Flask",
     ],
-    keywords=['systematic review', 'machine-learning'],
-    packages=find_packages(exclude=['contrib', 'docs', 'tests']),
-    package_data={'asreview': [
-        'webapp/build/*',
-        'webapp/build/static/*/*',
-    ]},
-    python_requires='~=3.8',
+    keywords=["systematic review", "machine-learning"],
+    packages=find_packages(exclude=["contrib", "docs", "tests"]),
+    package_data={
+        "asreview": [
+            "webapp/build/*",
+            "webapp/build/static/*/*",
+        ]
+    },
+    python_requires="~=3.7",
     install_requires=[
-        'numpy',
-        'scikit-learn',
-        'pandas>=1,<3',
-        'rispy~=0.7.0',
-        'dill',
-        'xlrd>=1.0.0',
-        'setuptools',
-        'flask>=2.0',
-        'flask_cors',
-        'openpyxl',
-        'gevent>=20',
-        'jsonschema',
-        'filelock',
-        'tqdm',
-        'datahugger>=0.2'
+        "numpy",
+        "pandas>=1,<3",
+        "scikit-learn",
+        "rispy~=0.7.0",
+        "dill",
+        "xlrd>=1.0.0",
+        "setuptools",
+        "flask>=2.0",
+        "flask_cors",
+        "flask-login",
+        "flask-mail",
+        "openpyxl",
+        "jsonschema",
+        "filelock",
+        "Flask-SQLAlchemy>=3.0.2",
+        "requests",
+        "tqdm",
+        "gevent>=20",
+        "datahugger>=0.2",
     ],
     extras_require=DEPS,
     entry_points={
-        'console_scripts': [
-            'asreview=asreview.__main__:main',
+        "console_scripts": [
+            "asreview=asreview.__main__:main",
         ],
-        'asreview.entry_points': [
-            'lab=asreview.entry_points:LABEntryPoint',
-            'web_run_model = asreview.entry_points:WebRunModelEntryPoint',
-            'simulate=asreview.entry_points:SimulateEntryPoint',
-            'algorithms = asreview.entry_points:AlgorithmsEntryPoint',
-            'state-inspect = asreview.entry_points:StateInspectEntryPoint'
-        ],
-        'asreview.readers': [
-            '.csv = asreview.io:CSVReader',
-            '.tab = asreview.io:CSVReader',
-            '.tsv = asreview.io:CSVReader',
-            '.ris = asreview.io:RISReader',
-            '.txt = asreview.io:RISReader',
-            '.xlsx = asreview.io:ExcelReader',
-        ],
-        'asreview.writers': [
-            '.csv = asreview.io:CSVWriter',
-            '.tab = asreview.io:TSVWriter',
-            '.tsv = asreview.io:TSVWriter',
-            '.ris = asreview.io:RISWriter',
-            '.txt = asreview.io:RISWriter',
-            '.xlsx = asreview.io:ExcelWriter',
-        ],
-        'asreview.datasets': [
-            'benchmark = asreview.datasets:BenchmarkDataGroup',
-            'benchmark-nature = asreview.datasets:NaturePublicationDataGroup',
-        ],
-        'asreview.models.classifiers': [
-            'svm = asreview.models.classifiers:SVMClassifier',
-            'nb = asreview.models.classifiers:NaiveBayesClassifier',
-            'rf = asreview.models.classifiers:RandomForestClassifier',
-            'nn-2-layer = asreview.models.classifiers:NN2LayerClassifier',
-            'logistic = asreview.models.classifiers:LogisticClassifier',
-            'lstm-base = asreview.models.classifiers:LSTMBaseClassifier',
-            'lstm-pool = asreview.models.classifiers:LSTMPoolClassifier',
-        ],
-        'asreview.models.feature_extraction': [
-            'doc2vec = asreview.models.feature_extraction:Doc2Vec',
-            'embedding-idf = asreview.models.feature_extraction:EmbeddingIdf',
-            'embedding-lstm = asreview.models.feature_extraction:EmbeddingLSTM',
-            'sbert = asreview.models.feature_extraction:SBERT',
-            'tfidf = asreview.models.feature_extraction:Tfidf',
+        "asreview.entry_points": [
+            "lab=asreview.entry_points:LABEntryPoint",
+            "web_run_model=asreview.entry_points:WebRunModelEntryPoint",
+            "simulate=asreview.entry_points:SimulateEntryPoint",
+            "algorithms=asreview.entry_points:AlgorithmsEntryPoint",
+            "state-inspect=asreview.entry_points:StateInspectEntryPoint",
+            "auth-tool=asreview.entry_points:AuthTool",
+        ],
+        "asreview.readers": [
+            ".csv = asreview.io:CSVReader",
+            ".tab = asreview.io:CSVReader",
+            ".tsv = asreview.io:CSVReader",
+            ".ris = asreview.io:RISReader",
+            ".txt = asreview.io:RISReader",
+            ".xlsx = asreview.io:ExcelReader",
+        ],
+        "asreview.writers": [
+            ".csv = asreview.io:CSVWriter",
+            ".tab = asreview.io:TSVWriter",
+            ".tsv = asreview.io:TSVWriter",
+            ".ris = asreview.io:RISWriter",
+            ".txt = asreview.io:RISWriter",
+            ".xlsx = asreview.io:ExcelWriter",
+        ],
+        "asreview.datasets": [
+            "benchmark = asreview.datasets:BenchmarkDataGroup",
+            "benchmark-nature = asreview.datasets:NaturePublicationDataGroup",
+        ],
+        "asreview.models.classifiers": [
+            "svm = asreview.models.classifiers:SVMClassifier",
+            "nb = asreview.models.classifiers:NaiveBayesClassifier",
+            "rf = asreview.models.classifiers:RandomForestClassifier",
+            "nn-2-layer = asreview.models.classifiers:NN2LayerClassifier",
+            "logistic = asreview.models.classifiers:LogisticClassifier",
+            "lstm-base = asreview.models.classifiers:LSTMBaseClassifier",
+            "lstm-pool = asreview.models.classifiers:LSTMPoolClassifier",
+        ],
+        "asreview.models.feature_extraction": [
+            "doc2vec = asreview.models.feature_extraction:Doc2Vec",
+            "embedding-idf = asreview.models.feature_extraction:EmbeddingIdf",
+            "embedding-lstm = asreview.models.feature_extraction:EmbeddingLSTM",
+            "sbert = asreview.models.feature_extraction:SBERT",
+            "tfidf = asreview.models.feature_extraction:Tfidf",
         ],
-        'asreview.models.balance': [
+        "asreview.models.balance": [
             "simple = asreview.models.balance:SimpleBalance",
             "double = asreview.models.balance:DoubleBalance",
             # "triple = asreview.models.balance:TripleBalance",  # Broken, only via API
             "undersample = asreview.models.balance:UndersampleBalance",
         ],
-        'asreview.models.query': [
+        "asreview.models.query": [
             "max = asreview.models.query.max:MaxQuery",
             "random = asreview.models.query.random:RandomQuery",
             "uncertainty = asreview.models.query.uncertainty:UncertaintyQuery",
             "cluster = asreview.models.query.cluster:ClusterQuery",
             "max_random = asreview.models.query.mixed:MaxRandomQuery",
             "max_uncertainty = asreview.models.query.mixed:MaxUncertaintyQuery",
-        ]
+        ],
     },
     project_urls={
-        'Bug Reports': 'https://github.com/asreview/asreview/issues',
-        'Source': 'https://github.com/asreview/asreview/',
+        "Bug Reports": "https://github.com/asreview/asreview/issues",
+        "Source": "https://github.com/asreview/asreview/",
     },
 )
```

### Comparing `asreview-1.2.1/versioneer.py` & `asreview-1.3a0/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -273,14 +272,15 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
+
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -304,33 +304,37 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         me = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(me), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
@@ -344,14 +348,15 @@
         parser.readfp(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
+
     cfg = VersioneerConfig()
     cfg.VCS = VCS
     cfg.style = get(parser, "style") or ""
     cfg.versionfile_source = get(parser, "versionfile_source")
     cfg.versionfile_build = get(parser, "versionfile_build")
     cfg.tag_prefix = get(parser, "tag_prefix")
     if cfg.tag_prefix in ("''", '""'):
@@ -368,36 +373,40 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            p = subprocess.Popen(
+                [c] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+            )
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -414,15 +423,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY[
+    "git"
+] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by github's download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -989,71 +1000,86 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = set([r for r in refs if re.search(r"\d", r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = run_command(
+        GITS,
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            "%s*" % tag_prefix,
+        ],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1068,54 +1094,55 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
         pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
+        0
+    ].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
@@ -1163,24 +1190,30 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         else:
             rootdirs.append(root)
             root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1201,29 +1234,30 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+    )
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+        )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1247,16 +1281,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
@@ -1362,19 +1395,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-pre":
@@ -1386,17 +1421,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1411,16 +1450,17 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert (
+        cfg.versionfile_source is not None
+    ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1466,17 +1506,21 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1517,14 +1561,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1549,22 +1594,23 @@
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1577,25 +1623,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
             from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1606,21 +1656,25 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
@@ -1639,16 +1693,18 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(
+                target_versionfile, self._versioneer_generated_versions
+            )
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1695,36 +1751,41 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (
+        EnvironmentError,
+        configparser.NoSectionError,
+        configparser.NoOptionError,
+    ) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except EnvironmentError:
             old = ""
         if INIT_PY_SNIPPET not in old:
@@ -1758,16 +1819,18 @@
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
         with open(manifest_in, "a") as f:
             f.write("include versioneer.py\n")
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
+        print(
+            " appending versionfile_source ('%s') to MANIFEST.in"
+            % cfg.versionfile_source
+        )
         with open(manifest_in, "a") as f:
             f.write("include %s\n" % cfg.versionfile_source)
     else:
         print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
```

