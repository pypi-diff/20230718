# Comparing `tmp/sflkit-0.2.0.tar.gz` & `tmp/sflkit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sflkit-0.2.0.tar", last modified: Wed Jun 28 11:12:49 2023, max compression
+gzip compressed data, was "sflkit-0.2.1.tar", last modified: Tue Jul 18 09:34:38 2023, max compression
```

## Comparing `sflkit-0.2.0.tar` & `sflkit-0.2.1.tar`

### file list

```diff
@@ -1,74 +1,70 @@
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.632706 sflkit-0.2.0/
--rw-r--r--   0 marius     (501) staff       (20)     1112 2023-03-23 09:55:10.000000 sflkit-0.2.0/LICENSE
--rw-r--r--   0 marius     (501) staff       (20)     4817 2023-06-28 11:12:49.632827 sflkit-0.2.0/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)     4062 2023-03-24 13:14:28.000000 sflkit-0.2.0/README.md
--rw-r--r--   0 marius     (501) staff       (20)      809 2023-06-28 11:07:58.000000 sflkit-0.2.0/pyproject.toml
--rw-r--r--   0 marius     (501) staff       (20)     1242 2023-06-28 11:12:49.633424 sflkit-0.2.0/setup.cfg
--rw-r--r--   0 marius     (501) staff       (20)       39 2023-03-23 09:55:13.000000 sflkit-0.2.0/setup.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.609956 sflkit-0.2.0/src/
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.615006 sflkit-0.2.0/src/SFLKit.egg-info/
--rw-r--r--   0 marius     (501) staff       (20)     4817 2023-06-28 11:12:49.000000 sflkit-0.2.0/src/SFLKit.egg-info/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)     1939 2023-06-28 11:12:49.000000 sflkit-0.2.0/src/SFLKit.egg-info/SOURCES.txt
--rw-r--r--   0 marius     (501) staff       (20)        1 2023-06-28 11:12:49.000000 sflkit-0.2.0/src/SFLKit.egg-info/dependency_links.txt
--rw-r--r--   0 marius     (501) staff       (20)       43 2023-06-28 11:12:49.000000 sflkit-0.2.0/src/SFLKit.egg-info/entry_points.txt
--rw-r--r--   0 marius     (501) staff       (20)      277 2023-06-28 11:12:49.000000 sflkit-0.2.0/src/SFLKit.egg-info/requires.txt
--rw-r--r--   0 marius     (501) staff       (20)        7 2023-06-28 11:12:49.000000 sflkit-0.2.0/src/SFLKit.egg-info/top_level.txt
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.616270 sflkit-0.2.0/src/sflkit/
--rw-r--r--   0 marius     (501) staff       (20)     1808 2023-06-28 11:08:12.000000 sflkit-0.2.0/src/sflkit/__init__.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.620717 sflkit-0.2.0/src/sflkit/analysis/
--rw-r--r--   0 marius     (501) staff       (20)      161 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/analysis/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     3331 2023-03-24 10:29:50.000000 sflkit-0.2.0/src/sflkit/analysis/analysis_type.py
--rw-r--r--   0 marius     (501) staff       (20)     2228 2023-03-23 17:28:40.000000 sflkit-0.2.0/src/sflkit/analysis/analyzer.py
--rw-r--r--   0 marius     (501) staff       (20)    13816 2023-03-24 11:51:43.000000 sflkit-0.2.0/src/sflkit/analysis/factory.py
--rw-r--r--   0 marius     (501) staff       (20)     1511 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/analysis/mapping.py
--rw-r--r--   0 marius     (501) staff       (20)    10720 2023-03-24 10:26:59.000000 sflkit-0.2.0/src/sflkit/analysis/predicate.py
--rw-r--r--   0 marius     (501) staff       (20)     1045 2023-03-24 10:29:08.000000 sflkit-0.2.0/src/sflkit/analysis/similarity.py
--rw-r--r--   0 marius     (501) staff       (20)    17367 2023-03-24 11:47:15.000000 sflkit-0.2.0/src/sflkit/analysis/spectra.py
--rw-r--r--   0 marius     (501) staff       (20)     1224 2023-03-23 15:58:48.000000 sflkit-0.2.0/src/sflkit/analysis/suggestion.py
--rw-r--r--   0 marius     (501) staff       (20)     3174 2023-03-23 17:38:06.000000 sflkit-0.2.0/src/sflkit/cli.py
--rw-r--r--   0 marius     (501) staff       (20)     3432 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/color.py
--rw-r--r--   0 marius     (501) staff       (20)    10870 2023-03-24 10:53:42.000000 sflkit-0.2.0/src/sflkit/config.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.621266 sflkit-0.2.0/src/sflkit/events/
--rw-r--r--   0 marius     (501) staff       (20)      362 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/events/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)    16791 2023-03-24 10:34:43.000000 sflkit-0.2.0/src/sflkit/events/event.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.622495 sflkit-0.2.0/src/sflkit/instrumentation/
--rw-r--r--   0 marius     (501) staff       (20)      665 2023-03-24 09:12:31.000000 sflkit-0.2.0/src/sflkit/instrumentation/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     3437 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/instrumentation/dir_instrumentation.py
--rw-r--r--   0 marius     (501) staff       (20)      446 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/instrumentation/file_instrumentation.py
--rw-r--r--   0 marius     (501) staff       (20)     4947 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/instrumentation/lib.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.624596 sflkit-0.2.0/src/sflkit/language/
--rw-r--r--   0 marius     (501) staff       (20)      151 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/language/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      353 2023-03-24 09:13:32.000000 sflkit-0.2.0/src/sflkit/language/extract.py
--rw-r--r--   0 marius     (501) staff       (20)      654 2023-03-23 15:08:14.000000 sflkit-0.2.0/src/sflkit/language/finder.py
--rw-r--r--   0 marius     (501) staff       (20)     3794 2023-03-23 14:04:24.000000 sflkit-0.2.0/src/sflkit/language/language.py
--rw-r--r--   0 marius     (501) staff       (20)     4063 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/language/meta.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.626186 sflkit-0.2.0/src/sflkit/language/python/
--rw-r--r--   0 marius     (501) staff       (20)        0 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/language/python/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     8599 2023-03-23 15:16:00.000000 sflkit-0.2.0/src/sflkit/language/python/extract.py
--rw-r--r--   0 marius     (501) staff       (20)    26809 2023-03-23 14:19:50.000000 sflkit-0.2.0/src/sflkit/language/python/factory.py
--rw-r--r--   0 marius     (501) staff       (20)     2990 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/language/python/finder.py
--rw-r--r--   0 marius     (501) staff       (20)     6119 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/language/python/visitor.py
--rw-r--r--   0 marius     (501) staff       (20)     1085 2023-03-24 09:09:17.000000 sflkit-0.2.0/src/sflkit/language/visitor.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.627575 sflkit-0.2.0/src/sflkit/model/
--rw-r--r--   0 marius     (501) staff       (20)      163 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/model/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      803 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/model/event_file.py
--rw-r--r--   0 marius     (501) staff       (20)     2073 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/model/model.py
--rw-r--r--   0 marius     (501) staff       (20)     1007 2023-03-23 09:55:13.000000 sflkit-0.2.0/src/sflkit/model/scope.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.628236 sflkit-0.2.0/src/sflkit/runners/
--rw-r--r--   0 marius     (501) staff       (20)      293 2023-06-28 09:49:26.000000 sflkit-0.2.0/src/sflkit/runners/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     7338 2023-06-28 09:49:26.000000 sflkit-0.2.0/src/sflkit/runners/run.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-28 11:12:49.632465 sflkit-0.2.0/tests/
--rw-r--r--   0 marius     (501) staff       (20)     7986 2023-03-23 09:55:13.000000 sflkit-0.2.0/tests/test_analysis_objects.py
--rw-r--r--   0 marius     (501) staff       (20)     2057 2023-03-23 18:03:53.000000 sflkit-0.2.0/tests/test_cli.py
--rw-r--r--   0 marius     (501) staff       (20)     1025 2023-03-24 09:19:40.000000 sflkit-0.2.0/tests/test_color.py
--rw-r--r--   0 marius     (501) staff       (20)     6241 2023-03-24 10:54:37.000000 sflkit-0.2.0/tests/test_config.py
--rw-r--r--   0 marius     (501) staff       (20)    14051 2023-03-23 17:37:39.000000 sflkit-0.2.0/tests/test_events.py
--rw-r--r--   0 marius     (501) staff       (20)     1318 2023-03-23 17:37:40.000000 sflkit-0.2.0/tests/test_execution.py
--rw-r--r--   0 marius     (501) staff       (20)     5100 2023-03-23 17:37:39.000000 sflkit-0.2.0/tests/test_instrumentation.py
--rw-r--r--   0 marius     (501) staff       (20)     8849 2023-03-23 17:37:40.000000 sflkit-0.2.0/tests/test_language.py
--rw-r--r--   0 marius     (501) staff       (20)     2773 2023-03-23 09:55:13.000000 sflkit-0.2.0/tests/test_predicates.py
--rw-r--r--   0 marius     (501) staff       (20)     6061 2023-06-28 09:49:26.000000 sflkit-0.2.0/tests/test_runner.py
--rw-r--r--   0 marius     (501) staff       (20)      615 2023-03-23 15:20:53.000000 sflkit-0.2.0/tests/test_scope.py
--rw-r--r--   0 marius     (501) staff       (20)     4277 2023-03-24 10:31:44.000000 sflkit-0.2.0/tests/test_spectra.py
--rw-r--r--   0 marius     (501) staff       (20)    11301 2023-03-24 12:11:43.000000 sflkit-0.2.0/tests/test_suggestions.py
--rw-r--r--   0 marius     (501) staff       (20)     1912 2023-03-23 09:55:13.000000 sflkit-0.2.0/tests/test_visitors.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.050030 sflkit-0.2.1/
+-rw-r--r--   0 marius     (501) staff       (20)     1112 2023-03-23 09:55:10.000000 sflkit-0.2.1/LICENSE
+-rw-r--r--   0 marius     (501) staff       (20)     4817 2023-07-18 09:34:38.050166 sflkit-0.2.1/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)     4062 2023-03-24 13:14:28.000000 sflkit-0.2.1/README.md
+-rw-r--r--   0 marius     (501) staff       (20)      809 2023-07-18 08:52:29.000000 sflkit-0.2.1/pyproject.toml
+-rw-r--r--   0 marius     (501) staff       (20)     1278 2023-07-18 09:34:38.051113 sflkit-0.2.1/setup.cfg
+-rw-r--r--   0 marius     (501) staff       (20)       39 2023-03-23 09:55:13.000000 sflkit-0.2.1/setup.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.023363 sflkit-0.2.1/src/
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.029558 sflkit-0.2.1/src/SFLKit.egg-info/
+-rw-r--r--   0 marius     (501) staff       (20)     4817 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)     1848 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/SOURCES.txt
+-rw-r--r--   0 marius     (501) staff       (20)        1 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/dependency_links.txt
+-rw-r--r--   0 marius     (501) staff       (20)       43 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/entry_points.txt
+-rw-r--r--   0 marius     (501) staff       (20)      311 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/requires.txt
+-rw-r--r--   0 marius     (501) staff       (20)        7 2023-07-18 09:34:38.000000 sflkit-0.2.1/src/SFLKit.egg-info/top_level.txt
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.031857 sflkit-0.2.1/src/sflkit/
+-rw-r--r--   0 marius     (501) staff       (20)     2330 2023-07-18 09:25:52.000000 sflkit-0.2.1/src/sflkit/__init__.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.036781 sflkit-0.2.1/src/sflkit/analysis/
+-rw-r--r--   0 marius     (501) staff       (20)      161 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/analysis/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     3331 2023-03-24 10:29:50.000000 sflkit-0.2.1/src/sflkit/analysis/analysis_type.py
+-rw-r--r--   0 marius     (501) staff       (20)     2228 2023-03-23 17:28:40.000000 sflkit-0.2.1/src/sflkit/analysis/analyzer.py
+-rw-r--r--   0 marius     (501) staff       (20)    13819 2023-07-18 09:22:13.000000 sflkit-0.2.1/src/sflkit/analysis/factory.py
+-rw-r--r--   0 marius     (501) staff       (20)     1511 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/analysis/mapping.py
+-rw-r--r--   0 marius     (501) staff       (20)    10727 2023-07-18 09:22:13.000000 sflkit-0.2.1/src/sflkit/analysis/predicate.py
+-rw-r--r--   0 marius     (501) staff       (20)     1045 2023-03-24 10:29:08.000000 sflkit-0.2.1/src/sflkit/analysis/similarity.py
+-rw-r--r--   0 marius     (501) staff       (20)    17373 2023-07-18 09:22:46.000000 sflkit-0.2.1/src/sflkit/analysis/spectra.py
+-rw-r--r--   0 marius     (501) staff       (20)     1224 2023-03-23 15:58:48.000000 sflkit-0.2.1/src/sflkit/analysis/suggestion.py
+-rw-r--r--   0 marius     (501) staff       (20)     3643 2023-07-18 08:52:29.000000 sflkit-0.2.1/src/sflkit/cli.py
+-rw-r--r--   0 marius     (501) staff       (20)     3432 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/color.py
+-rw-r--r--   0 marius     (501) staff       (20)    10920 2023-07-18 09:25:52.000000 sflkit-0.2.1/src/sflkit/config.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.038086 sflkit-0.2.1/src/sflkit/instrumentation/
+-rw-r--r--   0 marius     (501) staff       (20)      661 2023-07-18 09:22:46.000000 sflkit-0.2.1/src/sflkit/instrumentation/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     3382 2023-07-18 09:23:43.000000 sflkit-0.2.1/src/sflkit/instrumentation/dir_instrumentation.py
+-rw-r--r--   0 marius     (501) staff       (20)      446 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/instrumentation/file_instrumentation.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.041049 sflkit-0.2.1/src/sflkit/language/
+-rw-r--r--   0 marius     (501) staff       (20)      151 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/language/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      353 2023-03-24 09:13:32.000000 sflkit-0.2.1/src/sflkit/language/extract.py
+-rw-r--r--   0 marius     (501) staff       (20)      654 2023-03-23 15:08:14.000000 sflkit-0.2.1/src/sflkit/language/finder.py
+-rw-r--r--   0 marius     (501) staff       (20)     3798 2023-07-18 09:25:18.000000 sflkit-0.2.1/src/sflkit/language/language.py
+-rw-r--r--   0 marius     (501) staff       (20)     4066 2023-07-18 09:24:46.000000 sflkit-0.2.1/src/sflkit/language/meta.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.042765 sflkit-0.2.1/src/sflkit/language/python/
+-rw-r--r--   0 marius     (501) staff       (20)        0 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/language/python/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     8602 2023-07-18 09:24:46.000000 sflkit-0.2.1/src/sflkit/language/python/extract.py
+-rw-r--r--   0 marius     (501) staff       (20)    26800 2023-07-18 09:31:57.000000 sflkit-0.2.1/src/sflkit/language/python/factory.py
+-rw-r--r--   0 marius     (501) staff       (20)     2990 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/language/python/finder.py
+-rw-r--r--   0 marius     (501) staff       (20)     6119 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/language/python/visitor.py
+-rw-r--r--   0 marius     (501) staff       (20)     1085 2023-07-18 08:52:29.000000 sflkit-0.2.1/src/sflkit/language/visitor.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.044432 sflkit-0.2.1/src/sflkit/model/
+-rw-r--r--   0 marius     (501) staff       (20)      163 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/model/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      806 2023-07-18 09:25:18.000000 sflkit-0.2.1/src/sflkit/model/event_file.py
+-rw-r--r--   0 marius     (501) staff       (20)     2073 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/model/model.py
+-rw-r--r--   0 marius     (501) staff       (20)     1007 2023-03-23 09:55:13.000000 sflkit-0.2.1/src/sflkit/model/scope.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.045379 sflkit-0.2.1/src/sflkit/runners/
+-rw-r--r--   0 marius     (501) staff       (20)      293 2023-06-28 09:49:26.000000 sflkit-0.2.1/src/sflkit/runners/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     7338 2023-07-18 08:52:29.000000 sflkit-0.2.1/src/sflkit/runners/run.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-18 09:34:38.049704 sflkit-0.2.1/tests/
+-rw-r--r--   0 marius     (501) staff       (20)     7993 2023-07-18 09:27:16.000000 sflkit-0.2.1/tests/test_analysis_objects.py
+-rw-r--r--   0 marius     (501) staff       (20)     2057 2023-03-23 18:03:53.000000 sflkit-0.2.1/tests/test_cli.py
+-rw-r--r--   0 marius     (501) staff       (20)     1025 2023-03-24 09:19:40.000000 sflkit-0.2.1/tests/test_color.py
+-rw-r--r--   0 marius     (501) staff       (20)     6194 2023-07-18 09:28:33.000000 sflkit-0.2.1/tests/test_config.py
+-rw-r--r--   0 marius     (501) staff       (20)    14215 2023-07-18 09:30:53.000000 sflkit-0.2.1/tests/test_events.py
+-rw-r--r--   0 marius     (501) staff       (20)     1318 2023-03-23 17:37:40.000000 sflkit-0.2.1/tests/test_execution.py
+-rw-r--r--   0 marius     (501) staff       (20)     5090 2023-07-18 09:32:50.000000 sflkit-0.2.1/tests/test_instrumentation.py
+-rw-r--r--   0 marius     (501) staff       (20)     8856 2023-07-18 09:28:00.000000 sflkit-0.2.1/tests/test_language.py
+-rw-r--r--   0 marius     (501) staff       (20)     2773 2023-03-23 09:55:13.000000 sflkit-0.2.1/tests/test_predicates.py
+-rw-r--r--   0 marius     (501) staff       (20)     6061 2023-06-28 09:49:26.000000 sflkit-0.2.1/tests/test_runner.py
+-rw-r--r--   0 marius     (501) staff       (20)      615 2023-03-23 15:20:53.000000 sflkit-0.2.1/tests/test_scope.py
+-rw-r--r--   0 marius     (501) staff       (20)     4279 2023-07-18 09:27:50.000000 sflkit-0.2.1/tests/test_spectra.py
+-rw-r--r--   0 marius     (501) staff       (20)    11301 2023-03-24 12:11:43.000000 sflkit-0.2.1/tests/test_suggestions.py
+-rw-r--r--   0 marius     (501) staff       (20)     1912 2023-03-23 09:55:13.000000 sflkit-0.2.1/tests/test_visitors.py
```

### Comparing `sflkit-0.2.0/LICENSE` & `sflkit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/PKG-INFO` & `sflkit-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sflkit
-Version: 0.2.0
+Version: 0.2.1
 Summary: SFLKit: : A Workbench for Statistical Fault Localization
 Home-page: https://github.com/uds-se/sflkit
 Author: Marius Smytzek & Andreas Zeller
 Author-email: Marius Smytzek <marius.smytzek@cispa.de>
 Project-URL: Homepage, https://github.com/uds-se/sflkit/
 Project-URL: Bug Tracker, https://github.com/uds-se/sflkit/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sflkit-0.2.0/README.md` & `sflkit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/pyproject.toml` & `sflkit-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=67.6.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sflkit"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "Marius Smytzek", email = "marius.smytzek@cispa.de" },
 ]
 description = "SFLKit: : A Workbench for Statistical Fault Localization"
 readme = "README.md"
 license = { file = "COPYING" }
 requires-python = ">=3.10"
```

### Comparing `sflkit-0.2.0/setup.cfg` & `sflkit-0.2.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,31 +20,33 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 install_requires = 
+	sflkitlib>=0.0.1
 	astor>=0.8.1
-	numpy>=1.24.0
-	matplotlib>=3.4.3
+	numpy==1.25.1
+	matplotlib==3.7.2
 	sortedcollections>=2.1.0
 	parameterized>=0.8.1
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test = 
+	sflkitlib>=0.0.1
 	astor>=0.8.1
-	numpy>=1.24.0
-	matplotlib>=3.4.3
+	numpy==1.25.1
+	matplotlib==3.7.2
 	sortedcollections>=2.1.0
 	pytest>=7.2.2
-	pytest-cov>=4.0.0
+	pytest-cov>=4.1.0
 	pytest-html>=3.2.0
 	pytest-rerunfailures>=11.1.2
 	parameterized>=0.8.1
 dev = 
 
 [options.entry_points]
 console_scripts =
```

### Comparing `sflkit-0.2.0/src/SFLKit.egg-info/PKG-INFO` & `sflkit-0.2.1/src/SFLKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sflkit
-Version: 0.2.0
+Version: 0.2.1
 Summary: SFLKit: : A Workbench for Statistical Fault Localization
 Home-page: https://github.com/uds-se/sflkit
 Author: Marius Smytzek & Andreas Zeller
 Author-email: Marius Smytzek <marius.smytzek@cispa.de>
 Project-URL: Homepage, https://github.com/uds-se/sflkit/
 Project-URL: Bug Tracker, https://github.com/uds-se/sflkit/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sflkit-0.2.0/src/SFLKit.egg-info/SOURCES.txt` & `sflkit-0.2.1/src/SFLKit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,17 @@
 src/sflkit/analysis/analyzer.py
 src/sflkit/analysis/factory.py
 src/sflkit/analysis/mapping.py
 src/sflkit/analysis/predicate.py
 src/sflkit/analysis/similarity.py
 src/sflkit/analysis/spectra.py
 src/sflkit/analysis/suggestion.py
-src/sflkit/events/__init__.py
-src/sflkit/events/event.py
 src/sflkit/instrumentation/__init__.py
 src/sflkit/instrumentation/dir_instrumentation.py
 src/sflkit/instrumentation/file_instrumentation.py
-src/sflkit/instrumentation/lib.py
 src/sflkit/language/__init__.py
 src/sflkit/language/extract.py
 src/sflkit/language/finder.py
 src/sflkit/language/language.py
 src/sflkit/language/meta.py
 src/sflkit/language/visitor.py
 src/sflkit/language/python/__init__.py
```

### Comparing `sflkit-0.2.0/src/sflkit/analysis/analysis_type.py` & `sflkit-0.2.1/src/sflkit/analysis/analysis_type.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/analysis/analyzer.py` & `sflkit-0.2.1/src/sflkit/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/analysis/factory.py` & `sflkit-0.2.1/src/sflkit/analysis/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from abc import abstractmethod
 from typing import List, Type, Set
 
+from sflkitlib.events import EventType
+
 from sflkit.analysis.analysis_type import AnalysisObject, AnalysisType
 from sflkit.analysis.predicate import (
     Branch,
     Condition,
     Comp,
     ScalarPair,
     VariablePredicate,
@@ -13,15 +15,14 @@
     EmptyStringPredicate,
     IsAsciiPredicate,
     ContainsDigitPredicate,
     ContainsSpecialPredicate,
     EmptyBytesPredicate,
 )
 from sflkit.analysis.spectra import Line, Function, Loop, DefUse
-from sflkit.events import EventType
 from sflkit.model.scope import Scope
 
 
 class AnalysisFactory:
     def __init__(self):
         self.objects = dict()
 
@@ -153,15 +154,14 @@
                     self.objects[key] = DefUse(self.id_to_def[event.var_id], event)
                 return [self.objects[key]]
 
 
 class ConditionFactory(AnalysisFactory):
     def get_analysis(self, event, scope: Scope = None) -> List[AnalysisObject]:
         if event.event_type == EventType.CONDITION:
-
             key = (Condition.analysis_type(), event.file, event.line, event.condition)
             if key not in self.objects:
                 self.objects[key] = Condition(event.file, event.line, event.condition)
             return [self.objects[key]]
 
 
 class ScalarPairFactory(AnalysisFactory):
```

### Comparing `sflkit-0.2.0/src/sflkit/analysis/mapping.py` & `sflkit-0.2.1/src/sflkit/analysis/mapping.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/analysis/predicate.py` & `sflkit-0.2.1/src/sflkit/analysis/predicate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import enum
 from abc import ABC
 from typing import Tuple, Callable, Optional
 
+from sflkitlib.events import EventType
+from sflkitlib.events.event import BranchEvent, FunctionExitEvent, DefEvent
+
 from sflkit.analysis.analysis_type import AnalysisType
 from sflkit.analysis.spectra import Spectrum
 from sflkit.analysis.suggestion import Suggestion, Location
-from sflkit.events import EventType
-from sflkit.events.event import BranchEvent, FunctionExitEvent, DefEvent
 from sflkit.model import scope
 
 
 class Predicate(Spectrum, ABC):
     def __init__(self, file, line):
         super().__init__(file, line)
         self.true_relevant = 0
```

### Comparing `sflkit-0.2.0/src/sflkit/analysis/similarity.py` & `sflkit-0.2.1/src/sflkit/analysis/similarity.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/analysis/spectra.py` & `sflkit-0.2.1/src/sflkit/analysis/spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import math
 from abc import ABC
 from typing import Callable, Optional
 
 import numpy
-
-from sflkit.analysis.analysis_type import AnalysisObject, AnalysisType
-from sflkit.analysis.suggestion import Suggestion, Location
-from sflkit.events import EventType
-from sflkit.events.event import (
+from sflkitlib.events import EventType
+from sflkitlib.events.event import (
     LineEvent,
     FunctionEnterEvent,
     LoopEndEvent,
     LoopBeginEvent,
     LoopHitEvent,
     DefEvent,
     UseEvent,
 )
+
+from sflkit.analysis.analysis_type import AnalysisObject, AnalysisType
+from sflkit.analysis.suggestion import Suggestion, Location
 from sflkit.model.scope import Scope
 
 
 class Spectrum(AnalysisObject, ABC):
     def __init__(
         self,
         file: str,
```

### Comparing `sflkit-0.2.0/src/sflkit/analysis/suggestion.py` & `sflkit-0.2.1/src/sflkit/analysis/suggestion.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/cli.py` & `sflkit-0.2.1/src/sflkit/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 from typing import Any
 
 import sflkit
 from sflkit.analysis.suggestion import Suggestion, Location
 
 INSTRUMENT = "instrument"
+RUN = "run"
 ANALYZE = "analyze"
 
 
 class ResultEncoder(json.JSONEncoder):
     def default(self, o: Any) -> Any:
         if isinstance(o, Suggestion):
             return {
@@ -26,14 +27,16 @@
 def main(args):
     if args.debug:
         logging.getLogger().setLevel(logging.DEBUG)
     else:
         logging.getLogger().setLevel(logging.INFO)
     if args.command == INSTRUMENT:
         sflkit.instrument(args.config, args.events)
+    elif args.command == RUN:
+        sflkit.run(args.config, args.out)
     elif args.command == ANALYZE:
         results = sflkit.analyze(args.config, args.analysis)
         with open(args.out, "w") as output:
             json.dump(results, output, cls=ResultEncoder, indent=4)
 
 
 def parse_args(args=None, namespace=None):
@@ -92,12 +95,25 @@
     analyze_parser.add_argument(
         "-o",
         "--out",
         dest="out",
         default="out.json",
         help="The report of the final results, i.e. the suggestions sorted by analysis",
     )
+
+    analyze_parser = commands.add_parser(
+        RUN,
+        description="The run command executes the tests of the subject and creates the event files.",
+        help="execute the tests and collect predicates",
+    )
+    analyze_parser.add_argument(
+        "-o",
+        "--out",
+        dest="out",
+        default=None,
+        help="The output path of the event files.",
+    )
     return arg_parser.parse_args(args=args, namespace=namespace)
 
 
 if __name__ == "__main__":
     main(parse_args())
```

### Comparing `sflkit-0.2.0/src/sflkit/color.py` & `sflkit-0.2.1/src/sflkit/color.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/config.py` & `sflkit-0.2.1/src/sflkit/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import configparser
 import csv
 import os.path
 import queue
+from pathlib import Path
 from typing import List, Callable, Union
 
-from sflkit.analysis.predicate import Predicate
+from sflkitlib.events import EventType
+
 from sflkit.analysis.analysis_type import AnalysisType
 from sflkit.analysis.factory import (
     analysis_factory_mapping,
     CombinationFactory,
     AnalysisFactory,
 )
 from sflkit.analysis.mapping import analysis_mapping
+from sflkit.analysis.predicate import Predicate
 from sflkit.analysis.spectra import Spectrum
-from sflkit.events import EventType
 from sflkit.language.language import Language
 from sflkit.language.meta import (
     CombinationVisitor,
     IDGenerator,
     TmpGenerator,
     MetaVisitor,
 )
@@ -72,18 +74,17 @@
         if path:
             if isinstance(path, configparser.ConfigParser):
                 config = path
             else:
                 config = configparser.ConfigParser()
                 config.read(path)
             try:
-
                 # target section
                 target = config["target"]
-                self.target_path = target["path"]
+                self.target_path = Path(target["path"])
                 self.language = Language[target["language"].upper()]
                 self.language.setup()
 
                 # events section
                 events = config["events"]
                 if "predicates" in events:
                     # get the predicates
@@ -145,15 +146,15 @@
                     )
                 # instrumentation section
                 instrument = config["instrumentation"]
                 if "exclude" in instrument:
                     self.instrument_exclude = list(csv.reader([instrument["exclude"]]))[
                         0
                     ]
-                self.instrument_working = instrument["path"]
+                self.instrument_working = Path(instrument["path"])
 
                 # test section
                 if "test" in config:
                     test = config["test"]
                     if "runner" in test and test["runner"] != "None":
                         self.runner = RunnerType[test["runner"].upper()]
 
@@ -264,29 +265,29 @@
         conf = configparser.ConfigParser()
         conf["target"] = dict()
         conf["events"] = dict()
         conf["instrumentation"] = dict()
         conf["test"] = dict()
 
         if self.target_path:
-            conf["target"]["path"] = self.target_path
+            conf["target"]["path"] = str(self.target_path)
         if self.language:
             conf["target"]["language"] = self.language.name
         if self.events:
             conf["events"]["events"] = ",".join(e.name for e in self.events)
         if self.predicates:
             conf["events"]["predicates"] = ",".join(p.name for p in self.predicates)
         if self.metrics:
             conf["events"]["metrics"] = ",".join(m.__name__ for m in self.metrics)
         if self.passing:
             conf["events"]["passing"] = ",".join(e.path for e in self.passing)
         if self.failing:
             conf["events"]["failing"] = ",".join(e.path for e in self.failing)
         if self.instrument_working:
-            conf["instrumentation"]["path"] = self.instrument_working
+            conf["instrumentation"]["path"] = str(self.instrument_working)
         if self.instrument_exclude:
             conf["instrumentation"]["exclude"] = ",".join(self.instrument_exclude)
         if self.runner:
             conf["test"]["runner"] = self.runner.name
 
         with open(path, "w") as fp:
             conf.write(fp)
```

### Comparing `sflkit-0.2.0/src/sflkit/instrumentation/__init__.py` & `sflkit-0.2.1/src/sflkit/instrumentation/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from abc import abstractmethod
 from typing import List
 
-from sflkit.events import event
+from sflkitlib.events import event
 from sflkit.language.visitor import ASTVisitor
 
 
 class Instrumentation:
     def __init__(self, visitor: ASTVisitor):
         self.visitor = visitor
         self.events = list()
@@ -18,8 +18,8 @@
         raise NotImplementedError()
 
     def dump_events(self, out_file):
         with open(out_file, "w") as fp:
             json.dump(self.events, fp, cls=event.EventEncoder)
 
 
-__all__ = ["dir_instrumentation", "file_instrumentation", "lib", "Instrumentation"]
+__all__ = ["dir_instrumentation", "file_instrumentation", "Instrumentation"]
```

### Comparing `sflkit-0.2.0/src/sflkit/instrumentation/dir_instrumentation.py` & `sflkit-0.2.1/src/sflkit/instrumentation/dir_instrumentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-import atexit
 import logging
 import os
 import queue
 import re
 import shutil
 from typing import List
 
-from sflkit.instrumentation import lib, Instrumentation
+from sflkit.instrumentation import Instrumentation
 from sflkit.instrumentation.file_instrumentation import FileInstrumentation
 from sflkit.language.visitor import ASTVisitor
 
-atexit.unregister(lib.dump_events)
-
 
 class DirInstrumentation(Instrumentation):
     def __init__(self, visitor: ASTVisitor):
         super().__init__(visitor)
         self.file_instrumentation = FileInstrumentation(visitor)
 
     def instrument(
```

### Comparing `sflkit-0.2.0/src/sflkit/language/finder.py` & `sflkit-0.2.1/src/sflkit/language/finder.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/language/language.py` & `sflkit-0.2.1/src/sflkit/language/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import enum
 from typing import List, Dict, Type
 
+from sflkitlib.events import EventType
+
 import sflkit.language.python.factory as python_factory
 from sflkit.analysis.analysis_type import AnalysisObject
-from sflkit.events import EventType
 from sflkit.language.extract import VariableExtract, ConditionExtract
 from sflkit.language.finder import BranchFinder, LoopFinder, FunctionFinder
 from sflkit.language.meta import MetaVisitor
 from sflkit.language.python.extract import PythonVarExtract, PythonConditionExtract
 from sflkit.language.python.finder import (
     PythonFunctionFinder,
     PythonLoopFinder,
```

### Comparing `sflkit-0.2.0/src/sflkit/language/meta.py` & `sflkit-0.2.1/src/sflkit/language/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 from abc import ABC
 from typing import List, Type, Any
 
-from sflkit.events.event import Event
+from sflkitlib.events.event import Event
 
 
 class Injection:
     def __init__(
         self,
         pre: List = None,
         body: List = None,
```

### Comparing `sflkit-0.2.0/src/sflkit/language/python/extract.py` & `sflkit-0.2.1/src/sflkit/language/python/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 from typing import Any, Union
 
+from sflkitlib.events.event import ConditionEvent
 from sortedcollections import OrderedSet
 
-from sflkit.events.event import ConditionEvent
 from sflkit.language.extract import VariableExtract, ConditionExtract
 
 
 class PythonIsDoc(ast.NodeVisitor):
     def generic_visit(self, node: ast.AST) -> bool:
         return False
```

### Comparing `sflkit-0.2.0/src/sflkit/language/python/factory.py` & `sflkit-0.2.1/src/sflkit/language/python/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import ast
 import typing
 from ast import *
 
-from sflkit.events.event import (
+from sflkitlib.events.event import (
     LineEvent,
     Event,
     BranchEvent,
     DefEvent,
     FunctionEnterEvent,
     FunctionErrorEvent,
     FunctionExitEvent,
     LoopBeginEvent,
     LoopHitEvent,
     LoopEndEvent,
     UseEvent,
     ConditionEvent,
 )
+
 from sflkit.language.meta import MetaVisitor, Injection, IDGenerator, TmpGenerator
 
-python_lib = "sflkit.instrumentation.lib"
+python_lib = "sflkitlib.lib"
 
 
 def get_call(function, *args) -> Expr:
     return Expr(
         value=Call(
             func=Attribute(
                 value=Name(
```

### Comparing `sflkit-0.2.0/src/sflkit/language/python/finder.py` & `sflkit-0.2.1/src/sflkit/language/python/finder.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/language/python/visitor.py` & `sflkit-0.2.1/src/sflkit/language/python/visitor.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/language/visitor.py` & `sflkit-0.2.1/src/sflkit/language/visitor.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/model/event_file.py` & `sflkit-0.2.1/src/sflkit/model/event_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import csv
 
-from sflkit.events import event
+from sflkitlib.events import event
 
 
 class EventFile(object):
     def __init__(self, path: str, run_id: int, failing: bool = False):
         self.path = path
         self.run_id = run_id
         self.failing = failing
```

### Comparing `sflkit-0.2.0/src/sflkit/model/model.py` & `sflkit-0.2.1/src/sflkit/model/model.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/model/scope.py` & `sflkit-0.2.1/src/sflkit/model/scope.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/src/sflkit/runners/run.py` & `sflkit-0.2.1/src/sflkit/runners/run.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/tests/test_analysis_objects.py` & `sflkit-0.2.1/tests/test_analysis_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+from sflkitlib.events import EventType
+from sflkitlib.events.event import (
+    LineEvent,
+    BranchEvent,
+    FunctionEnterEvent,
+    LoopBeginEvent,
+    DefEvent,
+    UseEvent,
+    FunctionExitEvent,
+)
+
 from sflkit.analysis.analysis_type import AnalysisType
 from sflkit.analysis.predicate import (
     Branch,
     Condition,
     ScalarPair,
     Comp,
     VariablePredicate,
@@ -10,24 +21,14 @@
     EmptyStringPredicate,
     EmptyBytesPredicate,
     IsAsciiPredicate,
     ContainsDigitPredicate,
     ContainsSpecialPredicate,
 )
 from sflkit.analysis.spectra import Line, Function, Loop, DefUse
-from sflkit.events import EventType
-from sflkit.events.event import (
-    LineEvent,
-    BranchEvent,
-    FunctionEnterEvent,
-    LoopBeginEvent,
-    DefEvent,
-    UseEvent,
-    FunctionExitEvent,
-)
 from utils import BaseTest
 
 
 class TestAnalysisObjects(BaseTest):
     def test_line(self):
         obj = Line(LineEvent(self.ACCESS, 1, 0))
         self.assertEqual(self.ACCESS, obj.file)
```

### Comparing `sflkit-0.2.0/tests/test_cli.py` & `sflkit-0.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/tests/test_color.py` & `sflkit-0.2.1/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/tests/test_config.py` & `sflkit-0.2.1/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import os.path
 import unittest
+from pathlib import Path
+
+from sflkitlib.events import EventType
 
 from sflkit import instrument, analyze
 from sflkit.analysis.analysis_type import AnalysisType
 from sflkit.analysis.factory import DefUseFactory
 from sflkit.analysis.spectra import Spectrum
 from sflkit.analysis.suggestion import Location
 from sflkit.config import Config, write_config
-from sflkit.events import EventType
 from sflkit.language.language import Language
 from sflkit.language.python.factory import LineEventFactory, BranchEventFactory
 from utils import BaseTest
 
 
 class ConfigTests(unittest.TestCase):
     def test_config(self):
         config = Config.create(
             path=os.path.join("test", "path"),
             language="Python",
             events="Line,Branch",
             working=os.path.join("instrumentation", "path"),
             exclude="test,test2",
         )
-        self.assertEqual(os.path.join("test", "path"), config.target_path)
+        self.assertEqual(Path("test", "path"), config.target_path)
         self.assertEqual(Language.PYTHON, config.language)
         self.assertEqual(2, len(config.events))
         self.assertIn(EventType.LINE, config.events)
         self.assertIn(EventType.BRANCH, config.events)
         self.assertEqual(0, len(config.predicates))
         self.assertEqual(2, len(config.meta_visitor.visitors))
         self.assertTrue(
@@ -41,42 +43,38 @@
             any(
                 map(
                     lambda v: isinstance(v, BranchEventFactory),
                     config.meta_visitor.visitors,
                 )
             )
         )
-        self.assertEqual(
-            os.path.join("instrumentation", "path"), config.instrument_working
-        )
+        self.assertEqual(Path("instrumentation", "path"), config.instrument_working)
         self.assertEqual(2, len(config.instrument_exclude))
         self.assertIn("test", config.instrument_exclude)
         self.assertIn("test2", config.instrument_exclude)
         self.assertIsNone(config.runner)
 
     def test_overwrite_predicates(self):
         config = Config.create(
             path=os.path.join("test", "path"),
             language="Python",
             events="Line,Branch",
             predicates="Def_Use",
             working=os.path.join("instrumentation", "path"),
         )
-        self.assertEqual(os.path.join("test", "path"), config.target_path)
+        self.assertEqual(Path("test", "path"), config.target_path)
         self.assertEqual(Language.PYTHON, config.language)
         self.assertEqual(2, len(config.events))
         self.assertIn(EventType.DEF, config.events)
         self.assertIn(EventType.USE, config.events)
         self.assertEqual(1, len(config.predicates))
         self.assertIn(AnalysisType.DEF_USE, config.predicates)
         self.assertEqual(1, len(config.factory.factories))
         self.assertIsInstance(config.factory.factories[0], DefUseFactory)
-        self.assertEqual(
-            os.path.join("instrumentation", "path"), config.instrument_working
-        )
+        self.assertEqual(Path("instrumentation", "path"), config.instrument_working)
         self.assertEqual(0, len(config.instrument_exclude))
         self.assertIsNone(config.runner)
 
     def test_create_config(self):
         config = Config.create(
             path=os.path.join("test", "path"),
             language="Python",
```

### Comparing `sflkit-0.2.0/tests/test_events.py` & `sflkit-0.2.1/tests/test_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import subprocess
 
 from parameterized import parameterized
+from sflkitlib.events import event
 
 from sflkit import instrument_config
 from sflkit.config import Config
-from sflkit.events import event
 from utils import BaseTest
 
 
 class EventTests(BaseTest):
     def test_lines(self):
         config = Config.create(
             path=os.path.join(self.TEST_RESOURCES, self.TEST_LINES),
@@ -52,14 +52,15 @@
                 self.assertEqual(self.ACCESS, e.file, f"{e} has not correct file")
                 self.assertEqual(lines[line_i], e.line, f"{e} has not correct line")
                 line_i += 1
             elif e.event_type == event.EventType.BRANCH:
                 self.assertIsInstance(
                     e, event.BranchEvent, f"{e} is not a condition event"
                 )
+                e: event.BranchEvent
                 self.assertEqual(self.ACCESS, e.file, f"{e} has not correct file")
                 self.assertEqual(
                     branch_lines[branch_i], e.line, f"{e} has not correct line"
                 )
                 if first_branch:
                     self.assertGreater(
                         e.then_id, e.else_id, f"{e} has not correct branch ids"
@@ -130,23 +131,25 @@
         function_exit_i = 0
         for e in events:
             if e.event_type == event.EventType.FUNCTION_ENTER:
                 line, function = function_enter[function_enter_i]
                 self.assertIsInstance(
                     e, event.FunctionEnterEvent, f"{e} is not a line event"
                 )
+                e: event.FunctionEnterEvent
                 self.assertEqual(BaseTest.ACCESS, e.file, f"{e} has not correct file")
                 self.assertEqual(line, e.line, f"{e} has not correct line")
                 self.assertEqual(function, e.function, f"{e} has not correct function")
                 function_enter_i += 1
             elif e.event_type == event.EventType.FUNCTION_EXIT:
                 line, function, value = function_exit[function_exit_i]
                 self.assertIsInstance(
                     e, event.FunctionExitEvent, f"{e} is not a line event"
                 )
+                e: event.FunctionExitEvent
                 self.assertEqual(BaseTest.ACCESS, e.file, f"{e} has not correct file")
                 self.assertEqual(line, e.line, f"{e} has not correct line")
                 self.assertEqual(function, e.function, f"{e} has not correct function")
                 self.assertEqual(value, e.return_value, f"{e} has not correct function")
                 function_exit_i += 1
 
     def test_branch(self):
@@ -159,14 +162,15 @@
             )
         )
         branches_i = 0
         for e in events:
             if e.event_type == event.EventType.BRANCH:
                 line, mod = branches[branches_i]
                 self.assertIsInstance(e, event.BranchEvent, f"{e} is not a line event")
+                e: event.BranchEvent
                 self.assertEqual(BaseTest.ACCESS, e.file, f"{e} has not correct file")
                 self.assertEqual(line, e.line, f"{e} has not correct line")
                 if mod < 0:
                     self.assertLess(
                         e.then_id,
                         e.else_id,
                         f"{e} has not correct branch ids",
```

### Comparing `sflkit-0.2.0/tests/test_execution.py` & `sflkit-0.2.1/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/tests/test_instrumentation.py` & `sflkit-0.2.1/tests/test_instrumentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import atexit
 import os
 from pathlib import Path
 
 from parameterized import parameterized
+from sflkitlib.events import event, EventType
 
 from sflkit import instrument_config, Config
-from sflkit.events import event, EventType
 from utils import BaseTest
 
 
 class TestInstrumentation(BaseTest):
     def test_complex_structure(self):
         config = Config.create(
             path=os.path.join(BaseTest.TEST_RESOURCES, "test_instrumentation"),
@@ -89,15 +89,15 @@
                 s_content, d_content, f"{d} has the same content then {s}"
             )
 
 
 class TestLib(BaseTest):
     @classmethod
     def setUpClass(cls) -> None:
-        from sflkit.instrumentation import lib
+        from sflkitlib import lib
 
         atexit.unregister(lib.dump_events)
         cls.lib = lib
         cls.event_type_map = {
             EventType.DEF: lib.add_def_event,
             EventType.USE: lib.add_use_event,
             EventType.LINE: lib.add_line_event,
```

### Comparing `sflkit-0.2.0/tests/test_language.py` & `sflkit-0.2.1/tests/test_language.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
 from typing import List
 
-from sflkit import Config, instrument_config
-from sflkit.events import EventType
-from sflkit.events.event import (
+from sflkitlib.events import EventType
+from sflkitlib.events.event import (
     LineEvent,
     Event,
     load_json,
     BranchEvent,
     DefEvent,
     UseEvent,
     ConditionEvent,
     FunctionEnterEvent,
     FunctionExitEvent,
     FunctionErrorEvent,
     LoopBeginEvent,
     LoopHitEvent,
     LoopEndEvent,
 )
+
+from sflkit import Config, instrument_config
 from sflkit.language.language import Language
 from utils import BaseTest
 
 
 class LanguageTests(BaseTest):
     def test_python_equals_python3(self):
         self.assertEqual(Language.PYTHON, Language.PYTHON3)
```

### Comparing `sflkit-0.2.0/tests/test_predicates.py` & `sflkit-0.2.1/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/tests/test_runner.py` & `sflkit-0.2.1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/tests/test_scope.py` & `sflkit-0.2.1/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/tests/test_spectra.py` & `sflkit-0.2.1/tests/test_spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 from parameterized import parameterized
+from sflkitlib.events.event import LineEvent
 
 from sflkit.analysis import similarity
 from sflkit.analysis.spectra import Line
-from sflkit.events.event import LineEvent
 from utils import BaseTest
 
 
 class TestSimilarityCoefficient(BaseTest):
     @classmethod
     def setUpClass(cls) -> None:
         analysis = cls.run_analysis(
@@ -68,15 +68,14 @@
             "Wong2": 0,
             "Wong3": 0,
             "Zoltar": 0.5,
         }
 
     @parameterized.expand(similarity.similarity_coefficients)
     def test_coefficient(self, metric):
-
         result = getattr(self.line, metric)()
 
         self.assertAlmostEqual(
             self.expected_results.get(metric, 1),
             result,
             msg=f"The results for {metric} are not correct",
             delta=self.delta,
```

### Comparing `sflkit-0.2.0/tests/test_suggestions.py` & `sflkit-0.2.1/tests/test_suggestions.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.0/tests/test_visitors.py` & `sflkit-0.2.1/tests/test_visitors.py`

 * *Files identical despite different names*

