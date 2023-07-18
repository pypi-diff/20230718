# Comparing `tmp/lino_react-23.7.1.tar.gz` & `tmp/lino_react-23.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino_react-23.7.1.tar", last modified: Thu Jul 13 12:30:04 2023, max compression
+gzip compressed data, was "lino_react-23.7.2.tar", last modified: Tue Jul 18 09:52:38 2023, max compression
```

## Comparing `lino_react-23.7.1.tar` & `lino_react-23.7.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:30:04.859869 lino_react-23.7.1/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.7.1/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.7.1/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-07-13 12:30:04.859869 lino_react-23.7.1/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.7.1/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:30:04.851868 lino_react-23.7.1/lino_react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.7.1/lino_react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:30:04.851868 lino_react-23.7.1/lino_react/react/
--rw-rw-r--   0 luc       (1000) www-data    (33)     4628 2023-06-13 10:30:58.000000 lino_react-23.7.1/lino_react/react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:30:04.851868 lino_react-23.7.1/lino_react/react/__pycache__/
--rw-rw-r--   0 luc       (1000) www-data    (33)     3362 2023-06-23 05:20:50.000000 lino_react-23.7.1/lino_react/react/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)     4010 2023-07-05 02:47:39.000000 lino_react-23.7.1/lino_react/react/__pycache__/icons.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)      140 2023-06-23 05:20:51.000000 lino_react-23.7.1/lino_react/react/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)    18458 2023-07-12 14:38:05.000000 lino_react-23.7.1/lino_react/react/__pycache__/renderer.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)    20595 2023-06-23 08:10:05.000000 lino_react-23.7.1/lino_react/react/__pycache__/views.cpython-310.pyc
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:30:04.851868 lino_react-23.7.1/lino_react/react/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:30:04.851868 lino_react-23.7.1/lino_react/react/config/react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.7.1/lino_react/react/config/react/linoweb.json
--rw-rw-r--   0 luc       (1000) www-data    (33)     1910 2023-06-11 12:10:21.000000 lino_react-23.7.1/lino_react/react/config/react/main.html
--rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.7.1/lino_react/react/config/react/service-worker.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3952 2023-07-05 02:47:35.000000 lino_react-23.7.1/lino_react/react/icons.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.7.1/lino_react/react/index.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.7.1/lino_react/react/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    29400 2023-07-11 17:44:12.000000 lino_react-23.7.1/lino_react/react/renderer.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:30:04.851868 lino_react-23.7.1/lino_react/react/static/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:30:04.855868 lino_react-23.7.1/lino_react/react/static/media/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.7.1/lino_react/react/static/media/color.6441e63a.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.7.1/lino_react/react/static/media/color.c7a33805.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.7.1/lino_react/react/static/media/line.567f5738.gif
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.7.1/lino_react/react/static/media/primeicons.2d2afb27.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.7.1/lino_react/react/static/media/primeicons.3a0d4a58.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.7.1/lino_react/react/static/media/primeicons.66ee0deb.woff
--rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.7.1/lino_react/react/static/media/primeicons.c55d94a2.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.7.1/lino_react/react/static/media/primeicons.df0140f8.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.7.1/lino_react/react/static/media/primeicons.dfbfef2d.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.7.1/lino_react/react/static/media/primeicons.e5e0e944.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.7.1/lino_react/react/static/media/primeicons.e61f3495.woff
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:30:04.859869 lino_react-23.7.1/lino_react/react/static/react/
--rw-rw-r--   0 luc       (1000) www-data    (33)  1789476 2023-07-11 17:44:12.000000 lino_react-23.7.1/lino_react/react/static/react/main.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.7.1/lino_react/react/static/react/main.js.LICENSE.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.7.1/lino_react/react/views.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-07-13 12:29:35.000000 lino_react-23.7.1/lino_react/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-13 12:30:04.851868 lino_react-23.7.1/lino_react.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-07-13 12:30:04.000000 lino_react-23.7.1/lino_react.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1522 2023-07-13 12:30:04.000000 lino_react-23.7.1/lino_react.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-07-13 12:30:04.000000 lino_react-23.7.1/lino_react.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.7.1/lino_react.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-07-13 12:30:04.000000 lino_react-23.7.1/lino_react.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-07-13 12:30:04.000000 lino_react-23.7.1/lino_react.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-07-13 12:30:04.859869 lino_react-23.7.1/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.7.1/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.7.1/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.892101 lino_react-23.7.2/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.7.2/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.7.2/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-07-18 09:52:38.892101 lino_react-23.7.2/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.7.2/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.7.2/lino_react/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/react/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4628 2023-06-13 10:30:58.000000 lino_react-23.7.2/lino_react/react/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/react/__pycache__/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3362 2023-06-23 05:20:50.000000 lino_react-23.7.2/lino_react/react/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4010 2023-07-05 02:47:39.000000 lino_react-23.7.2/lino_react/react/__pycache__/icons.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)      140 2023-06-23 05:20:51.000000 lino_react-23.7.2/lino_react/react/__pycache__/models.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)    18481 2023-07-18 09:49:19.000000 lino_react-23.7.2/lino_react/react/__pycache__/renderer.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)    20595 2023-06-23 08:10:05.000000 lino_react-23.7.2/lino_react/react/__pycache__/views.cpython-310.pyc
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/react/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/react/config/react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.7.2/lino_react/react/config/react/linoweb.json
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1910 2023-06-11 12:10:21.000000 lino_react-23.7.2/lino_react/react/config/react/main.html
+-rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.7.2/lino_react/react/config/react/service-worker.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3952 2023-07-05 02:47:35.000000 lino_react-23.7.2/lino_react/react/icons.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.7.2/lino_react/react/index.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.7.2/lino_react/react/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    29449 2023-07-18 09:49:16.000000 lino_react-23.7.2/lino_react/react/renderer.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react/react/static/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.892101 lino_react-23.7.2/lino_react/react/static/media/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.7.2/lino_react/react/static/media/color.6441e63a.png
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.7.2/lino_react/react/static/media/color.c7a33805.png
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.7.2/lino_react/react/static/media/line.567f5738.gif
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.2d2afb27.eot
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.3a0d4a58.ttf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.66ee0deb.woff
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.c55d94a2.svg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.df0140f8.ttf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.dfbfef2d.eot
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.e5e0e944.svg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.7.2/lino_react/react/static/media/primeicons.e61f3495.woff
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.892101 lino_react-23.7.2/lino_react/react/static/react/
+-rw-rw-r--   0 luc       (1000) www-data    (33)  1789571 2023-07-18 09:49:16.000000 lino_react-23.7.2/lino_react/react/static/react/main.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.7.2/lino_react/react/static/react/main.js.LICENSE.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.7.2/lino_react/react/views.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-07-18 09:52:15.000000 lino_react-23.7.2/lino_react/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-07-18 09:52:38.888101 lino_react-23.7.2/lino_react.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-07-18 09:52:38.000000 lino_react-23.7.2/lino_react.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1522 2023-07-18 09:52:38.000000 lino_react-23.7.2/lino_react.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-07-18 09:52:38.000000 lino_react-23.7.2/lino_react.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.7.2/lino_react.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-07-18 09:52:38.000000 lino_react-23.7.2/lino_react.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-07-18 09:52:38.000000 lino_react-23.7.2/lino_react.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-07-18 09:52:38.892101 lino_react-23.7.2/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.7.2/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.7.2/tasks.py
```

### Comparing `lino_react-23.7.1/COPYING` & `lino_react-23.7.2/COPYING`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/PKG-INFO` & `lino_react-23.7.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino_react
-Version: 23.7.1
+Version: 23.7.2
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier:   Programming Language :: Python
```

### Comparing `lino_react-23.7.1/lino_react/react/__init__.py` & `lino_react-23.7.2/lino_react/react/__init__.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/__pycache__/__init__.cpython-310.pyc` & `lino_react-23.7.2/lino_react/react/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/__pycache__/icons.cpython-310.pyc` & `lino_react-23.7.2/lino_react/react/__pycache__/icons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/__pycache__/renderer.cpython-310.pyc` & `lino_react-23.7.2/lino_react/react/__pycache__/renderer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul 11 17:44:12 2023 UTC, .py size: 29400 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ec94 ad64 d872 0000  o..........d.r..
+00000000: 6f0d 0d0a 0000 0000 1c60 b664 0973 0000  o........`.d.s..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ae01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -127,1028 +127,1030 @@
 000007e0: 7079 326a 735f 636f 6e76 6572 7465 7229  py2js_converter)
 000007f0: 02da 0473 656c 66da 0966 726f 6e74 5f65  ...self..front_e
 00000800: 6e64 a901 da09 5f5f 636c 6173 735f 5f72  nd....__class__r
 00000810: 3700 0000 7238 0000 0072 3d00 0000 4600  7...r8...r=...F.
 00000820: 0000 7304 0000 000c 0110 017a 1152 656e  ..s........z.Ren
 00000830: 6465 7265 722e 5f5f 696e 6974 5f5f 6302  derer.__init__c.
 00000840: 0000 0000 0000 0000 0000 000c 0000 0008  ................
-00000850: 0000 0003 0000 0073 7202 0000 6401 6402  .......sr...d.d.
+00000850: 0000 0003 0000 0073 7002 0000 6401 6402  .......sp...d.d.
 00000860: 8400 7400 6a01 a002 a100 4400 8301 7d02  ..t.j.....D...}.
 00000870: 7403 8300 7d03 8800 6a04 4400 5d14 7d04  t...}...j.D.].}.
 00000880: 7c04 a005 a100 4400 5d0d 7d05 7c05 6a06  |.....D.].}.|.j.
 00000890: 7c03 7601 7223 7c03 a007 7c05 6a06 a101  |.v.r#|...|.j...
 000008a0: 0100 7116 7110 6403 8800 5f08 7409 6a0a  ..q.q.d..._.t.j.
 000008b0: 6a0b 7d06 740c 8700 6601 6404 6402 8408  j.}.t...f.d.d...
 000008c0: 7c03 4400 8301 7409 6a0a a00d 740e 8300  |.D...t.j...t...
 000008d0: a101 7c06 6a0f 6a10 7409 6a0a 6a11 8800  ..|.j.j.t.j.j...
 000008e0: 6a12 6a13 6405 7501 6406 6402 8400 7409  j.j.d.u.d.d...t.
 000008f0: 6a0a 6a14 4400 8301 6407 8d06 7d07 7409  j.j.D...d...}.t.
 00000900: 6a0a a015 6408 a101 7264 7c07 6a16 7417  j...d...rd|.j.t.
 00000910: 7c06 6a18 6a19 6a1a a01b a100 8301 6409  |.j.j.j.......d.
 00000920: 8d01 0100 7c07 6a16 7409 6a0a 6a00 6a1c  ....|.j.t.j.j.j.
-00000930: 640a 8d01 0100 7a13 7c07 6a16 741d a01e  d.....z.|.j.t...
-00000940: 741f 7409 6a20 8301 640b 1b00 640c 1b00  t.t.j ..d...d...
-00000950: a101 6a21 640d 8d01 0100 5700 6e09 0400  ..j!d.....W.n...
-00000960: 7422 7989 0100 0100 0100 5900 6e01 7700  t"y.......Y.n.w.
-00000970: 7423 7409 6a0a 640e 8302 7298 7c07 6a16  t#t.j.d...r.|.j.
-00000980: 7409 6a0a 6a24 640f 8d01 0100 7409 6a0a  t.j.j$d.....t.j.
-00000990: 6a25 6405 6b02 72a5 7c07 6a16 6403 6410  j%d.k.r.|.j.d.d.
-000009a0: 8d01 0100 6e0e 7423 7c06 6a26 6411 8302  ....n.t#|.j&d...
-000009b0: 72b3 7c07 6a16 7c06 6a26 6a27 6412 8d01  r.|.j.|.j&j'd...
-000009c0: 0100 7409 6a0a a015 6413 a101 72c5 7c07  ..t.j...d...r.|.
-000009d0: 6a16 7c06 6a28 6a29 6fc2 7409 6a0a 6a2a  j.|.j(j)o.t.j.j*
-000009e0: 6414 8d01 0100 6900 7d08 8800 6a2b 4400  d.....i.}...j+D.
-000009f0: 5d2f 7d09 8800 a02c 7c09 a101 7c08 7c09  ]/}....,|...|.|.
-00000a00: 6a2d 3c00 7423 7c09 6415 8302 72f9 6416  j-<.t#|.d...r.d.
-00000a10: 7c09 6a2d 7600 72f9 742e 7c02 6417 1900  |.j-v.r.t.|.d...
-00000a20: 8301 4400 5d14 5c02 7d0a 7d0b 7c0b 6418  ..D.].\.}.}.|.d.
-00000a30: 1900 7c09 6a2f 6b02 72f8 7c09 6a2d 7c02  ..|.j/k.r.|.j-|.
-00000a40: 6417 1900 7c0a 1900 6419 3c00 71e4 71ca  d...|...d.<.q.q.
-00000a50: 8800 6a30 4400 5d0a 7d09 8800 a02c 7c09  ..j0D.].}....,|.
-00000a60: a101 7c08 7c09 6a2d 3c00 71fd 8800 6a31  ..|.|.j-<.q...j1
-00000a70: 4400 5d0b 7d09 8800 a02c 7c09 a101 7c08  D.].}....,|...|.
-00000a80: 7c09 6a2d 3c00 9001 710b 8800 6a32 4400  |.j-<...q...j2D.
-00000a90: 5d0b 7d09 8800 a02c 7c09 a101 7c08 7c09  ].}....,|...|.|.
-00000aa0: 6a2d 3c00 9001 711a 7c07 6a16 7c08 7c02  j-<...q.|.j.|.|.
-00000ab0: 641a 8d02 0100 7c01 a033 7434 7c07 8301  d.....|..3t4|...
-00000ac0: a101 0100 641b 8800 5f08 641c 5300 291d  ....d..._.d.S.).
-00000ad0: 7a86 0a20 2020 2020 2020 2043 7265 6174  z..        Creat
-00000ae0: 6573 2077 6861 7420 6973 206b 6e6f 776e  es what is known
-00000af0: 2061 7320 7769 6e64 6f77 2e41 7070 2e73   as window.App.s
-00000b00: 7461 7465 2e73 6974 655f 6461 7461 2069  tate.site_data i
-00000b10: 6e20 5265 6163 7420 636f 6465 2e0a 0a20  n React code... 
-00000b20: 2020 2020 2020 203a 7061 7261 6d20 663a         :param f:
-00000b30: 2046 696c 6520 6f62 6a65 6374 0a20 2020   File object.   
-00000b40: 2020 2020 203a 7265 7475 726e 3a20 310a       :return: 1.
-00000b50: 2020 2020 2020 2020 6301 0000 0000 0000          c.......
-00000b60: 0000 0000 0003 0000 0006 0000 0053 0000  .............S..
-00000b70: 0073 2400 0000 6900 7c00 5d0e 5c02 7d01  .s$...i.|.].\.}.
-00000b80: 7d02 7c01 6400 6401 8400 7c02 a000 a100  }.|.d.d...|.....
-00000b90: 4400 8301 9302 7102 5300 2902 6301 0000  D.....q.S.).c...
-00000ba0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00000bb0: 0053 0000 0073 2400 0000 6700 7c00 5d0e  .S...s$...g.|.].
-00000bc0: 7d01 7c01 6400 1900 6a00 7401 7c01 6401  }.|.d...j.t.|.d.
-00000bd0: 1900 8301 6402 9c02 9102 7102 5300 2903  ....d.....q.S.).
-00000be0: 7201 0000 0072 2d00 0000 2902 da05 7661  r....r-...)...va
-00000bf0: 6c75 65da 0474 6578 7429 0272 4400 0000  lue..text).rD...
-00000c00: da03 7374 7229 02da 022e 30da 0163 7237  ..str)....0..cr7
-00000c10: 0000 0072 3700 0000 7238 0000 00da 0a3c  ...r7...r8.....<
-00000c20: 6c69 7374 636f 6d70 3e53 0000 0073 0200  listcomp>S...s..
-00000c30: 0000 2400 7a35 5265 6e64 6572 6572 2e77  ..$.z5Renderer.w
-00000c40: 7269 7465 5f6c 696e 6f5f 6a73 2e3c 6c6f  rite_lino_js.<lo
-00000c50: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
-00000c60: 2e3c 6c69 7374 636f 6d70 3e29 01da 0b67  .<listcomp>)...g
-00000c70: 6574 5f63 686f 6963 6573 2903 7247 0000  et_choices).rG..
-00000c80: 00da 0249 44da 0263 6c72 3700 0000 7237  ...ID..clr7...r7
-00000c90: 0000 0072 3800 0000 da0a 3c64 6963 7463  ...r8.....<dictc
-00000ca0: 6f6d 703e 5100 0000 7308 0000 0006 0006  omp>Q...s.......
-00000cb0: 0312 ff06 fe7a 2a52 656e 6465 7265 722e  .....z*Renderer.
-00000cc0: 7772 6974 655f 6c69 6e6f 5f6a 732e 3c6c  write_lino_js.<l
-00000cd0: 6f63 616c 733e 2e3c 6469 6374 636f 6d70  ocals>.<dictcomp
-00000ce0: 3e54 6301 0000 0000 0000 0000 0000 0002  >Tc.............
-00000cf0: 0000 0006 0000 0013 0000 0073 1a00 0000  ...........s....
-00000d00: 6900 7c00 5d09 7d01 7c01 6a00 8800 a001  i.|.].}.|.j.....
-00000d10: 7c01 a101 9302 7102 5300 7237 0000 0029  |.....q.S.r7...)
-00000d20: 02da 0b61 6374 696f 6e5f 6e61 6d65 da0b  ...action_name..
-00000d30: 6163 7469 6f6e 326a 736f 6e29 0272 4700  action2json).rG.
-00000d40: 0000 da01 61a9 0172 4000 0000 7237 0000  ....a..r@...r7..
-00000d50: 0072 3800 0000 724d 0000 0060 0000 0073  .r8...rM...`...s
-00000d60: 0200 0000 1a00 4e63 0100 0000 0000 0000  ......Nc........
-00000d70: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00000d80: 7316 0000 0069 007c 005d 077d 017c 016a  s....i.|.].}.|.j
-00000d90: 007c 016a 0193 0271 0253 0072 3700 0000  .|.j...q.S.r7...
-00000da0: 2902 da0b 646a 616e 676f 5f63 6f64 65da  )...django_code.
-00000db0: 046e 616d 6529 0272 4700 0000 da04 6c61  .name).rG.....la
-00000dc0: 6e67 7237 0000 0072 3700 0000 7238 0000  ngr7...r7...r8..
-00000dd0: 0072 4d00 0000 6600 0000 7302 0000 0016  .rM...f...s.....
-00000de0: 0029 06da 0761 6374 696f 6e73 da04 6d65  .)...actions..me
-00000df0: 6e75 da15 7573 655f 6461 7368 626f 6172  nu..use_dashboar
-00000e00: 645f 6c61 796f 7574 73da 0a73 6974 655f  d_layouts..site_
-00000e10: 7469 746c 65da 1065 6469 7469 6e67 5f66  title..editing_f
-00000e20: 726f 6e74 656e 64da 096c 616e 6775 6167  rontend..languag
-00000e30: 6573 da04 6d65 6d6f 2901 da0a 7375 6767  es..memo)...sugg
-00000e40: 6573 746f 7273 2901 da0f 7265 7669 7369  estors)...revisi
-00000e50: 6f6e 5f6e 756d 6265 72da 0572 6561 6374  on_number..react
-00000e60: 7a07 6d61 696e 2e6a 7329 01da 0d6d 6a73  z.main.js)...mjs
-00000e70: 5f74 696d 6573 7461 6d70 da0a 7468 656d  _timestamp..them
-00000e80: 655f 6e61 6d65 2901 7260 0000 0029 01da  e_name).r`...)..
-00000e90: 0d6e 6f5f 7573 6572 5f6d 6f64 656c da19  .no_user_model..
-00000ea0: 616c 6c6f 775f 6f6e 6c69 6e65 5f72 6567  allow_online_reg
-00000eb0: 6973 7472 6174 696f 6e29 0172 6200 0000  istration).rb...
-00000ec0: da06 6e6f 7469 6679 2901 da0c 7573 655f  ..notify)...use_
-00000ed0: 7075 7368 5f61 7069 da0b 6368 6f69 6365  push_api..choice
-00000ee0: 5f6e 616d 657a 1073 7973 7465 6d2e 4461  _namez.system.Da
-00000ef0: 7368 626f 6172 647a 1773 7973 7465 6d2e  shboardz.system.
-00000f00: 4461 7368 626f 6172 644c 6179 6f75 7473  DashboardLayouts
-00000f10: 7244 0000 00da 0d77 696e 646f 775f 6c61  rD.....window_la
-00000f20: 796f 7574 2902 da0b 666f 726d 5f70 616e  yout)...form_pan
-00000f30: 656c 7372 0d00 0000 4672 2d00 0000 2935  elsr....Fr-...)5
-00000f40: 7223 0000 00da 0b43 484f 4943 454c 4953  r#.....CHOICELIS
-00000f50: 5453 da05 6974 656d 73da 0373 6574 da0b  TS..items..set..
-00000f60: 6163 746f 7273 5f6c 6973 74da 0b67 6574  actors_list..get
-00000f70: 5f61 6374 696f 6e73 da06 6163 7469 6f6e  _actions..action
-00000f80: da03 6164 64da 1173 6572 6961 6c69 7365  ..add..serialise
-00000f90: 5f6a 735f 636f 6465 7204 0000 00da 0453  _js_coder......S
-00000fa0: 4954 45da 0770 6c75 6769 6e73 da04 6469  ITE..plugins..di
-00000fb0: 6374 da0d 6765 745f 7369 7465 5f6d 656e  ct..get_site_men
-00000fc0: 7572 2900 0000 da06 7379 7374 656d 7257  ur).....systemrW
-00000fd0: 0000 00da 0574 6974 6c65 7241 0000 00da  .....titlerA....
-00000fe0: 0a75 726c 5f70 7265 6669 7872 5a00 0000  .url_prefixrZ...
-00000ff0: da0c 6973 5f69 6e73 7461 6c6c 6564 da06  ..is_installed..
-00001000: 7570 6461 7465 da04 6c69 7374 725b 0000  update..listr[..
-00001010: 00da 0670 6172 7365 72da 0a73 7567 6765  ...parser..sugge
-00001020: 7374 6572 73da 046b 6579 73da 0a63 6f64  sters..keys..cod
-00001030: 655f 6d74 696d 65da 026f 73da 0473 7461  e_mtime..os..sta
-00001040: 7472 0200 0000 da0b 5354 4154 4943 5f52  tr......STATIC_R
-00001050: 4f4f 54da 0873 745f 6d74 696d 65da 1146  OOT..st_mtime..F
-00001060: 696c 654e 6f74 466f 756e 6445 7272 6f72  ileNotFoundError
-00001070: da07 6861 7361 7474 7272 6000 0000 da0a  ..hasattrr`.....
-00001080: 7573 6572 5f6d 6f64 656c da05 7573 6572  user_model..user
-00001090: 7372 6200 0000 7263 0000 0072 6400 0000  srb...rc...rd...
-000010a0: da09 7573 655f 6c69 6e6f 6472 6700 0000  ..use_linodrg...
-000010b0: da0a 7061 6e65 6c32 6a73 6f6e da0f 5f66  ..panel2json.._f
-000010c0: 6f72 6d70 616e 656c 5f6e 616d 6572 3100  ormpanel_namer1.
-000010d0: 0000 7265 0000 00da 0c70 6172 616d 5f70  ..re.....param_p
-000010e0: 616e 656c 73da 1361 6374 696f 6e5f 7061  anels..action_pa
-000010f0: 7261 6d5f 7061 6e65 6c73 da0c 6f74 6865  ram_panels..othe
-00001100: 725f 7061 6e65 6c73 da05 7772 6974 6572  r_panels..writer
-00001110: 2600 0000 290c 7240 0000 00da 0166 da10  &...).r@.....f..
-00001120: 6368 6f69 6365 6c69 7374 735f 6461 7461  choicelists_data
-00001130: 7255 0000 00da 0372 7074 da02 6261 7271  rU.....rpt..barq
-00001140: 0000 00da 0464 6174 6172 6700 0000 da01  .....datarg.....
-00001150: 7072 3500 0000 da04 6974 656d 7237 0000  pr5.....itemr7..
-00001160: 0072 5100 0000 7238 0000 00da 0d77 7269  .rQ...r8.....wri
-00001170: 7465 5f6c 696e 6f5f 6a73 4a00 0000 7370  te_lino_jsJ...sp
-00001180: 0000 0006 0708 0306 fd06 050a 010c 020a  ................
-00001190: 010c 0102 8002 fe06 0408 0102 0110 010c  ................
-000011a0: 0206 0106 010a 0110 0106 f90c 0904 0210  ................
-000011b0: 0106 ff12 0602 0126 010c 0104 0102 ff0c  .......&........
-000011c0: 0310 010c 020e 010c 0110 010c 0218 0104  ................
-000011d0: 090a 0110 0114 0114 010e 0112 0104 800a  ................
-000011e0: 0112 010a 0114 010a 0114 010e 010e 0506  ................
-000011f0: 0204 017a 1652 656e 6465 7265 722e 7772  ...z.Renderer.wr
-00001200: 6974 655f 6c69 6e6f 5f6a 7363 0200 0000  ite_lino_jsc....
-00001210: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-00001220: 4300 0000 73c6 0000 0074 007c 0174 0183  C...s....t.|.t..
-00001230: 0273 074a 0082 0174 027c 016a 037c 01a0  .s.J...t.|.j.|..
-00001240: 04a1 007c 01a0 05a1 007c 016a 0664 018d  ...|.....|.j.d..
-00001250: 047d 0274 007c 0174 0783 0272 297c 016a  .}.t.|.t...r)|.j
-00001260: 086a 096a 037c 0264 023c 0074 0a7c 016a  .j.j.|.d.<.t.|.j
-00001270: 086a 0b83 017c 0264 033c 007c 016a 0c72  .j...|.d.<.|.j.r
-00001280: 317c 016a 0c7c 0264 043c 007c 016a 0d72  1|.j.|.d.<.|.j.r
-00001290: 397c 016a 0d7c 0264 053c 007c 016a 0e72  9|.j.|.d.<.|.j.r
-000012a0: 4064 067c 0264 073c 007c 016a 0f72 487c  @d.|.d.<.|.j.rH|
-000012b0: 016a 0f7c 0264 083c 007c 016a 1072 4f64  .j.|.d.<.|.j.rOd
-000012c0: 067c 0264 093c 007c 016a 1172 5664 067c  .|.d.<.|.j.rVd.|
-000012d0: 0264 0a3c 007c 00a0 127c 01a1 017d 037c  .d.<.|...|...}.|
-000012e0: 0372 617c 037c 0264 0b3c 007c 0253 0029  .ra|.|.d.<.|.S.)
-000012f0: 0c7a 3343 6f6e 7665 7274 7320 676c 6f62  .z3Converts glob
-00001300: 616c 206c 6973 7420 6f66 2061 6c6c 2061  al list of all a
-00001310: 6374 696f 6e73 2074 6f20 6a73 6f6e 2066  ctions to json f
-00001320: 6f72 6d61 742e 2904 da02 616e da05 6c61  ormat.)...an..la
-00001330: 6265 6cda 0d77 696e 646f 775f 6163 7469  bel..window_acti
-00001340: 6f6e da0b 6874 7470 5f6d 6574 686f 6472  on..http_methodr
-00001350: 9500 0000 da05 6163 746f 72da 0c70 7265  ......actor..pre
-00001360: 7072 6f63 6573 736f 72da 0b73 656c 6563  processor..selec
-00001370: 745f 726f 7773 54da 1073 7562 6d69 745f  t_rowsT..submit_
-00001380: 666f 726d 5f64 6174 61da 0b62 7574 746f  form_data..butto
-00001390: 6e5f 7465 7874 da14 7368 6f77 5f69 6e5f  n_text..show_in_
-000013a0: 7369 6465 5f74 6f6f 6c62 6172 da0e 6e65  side_toolbar..ne
-000013b0: 7665 725f 636f 6c6c 6170 7365 da04 6963  ver_collapse..ic
-000013c0: 6f6e 2913 da0a 6973 696e 7374 616e 6365  on)...isinstance
-000013d0: 7217 0000 0072 7200 0000 724e 0000 00da  r....rr...rN....
-000013e0: 0967 6574 5f6c 6162 656c da10 6973 5f77  .get_label..is_w
-000013f0: 696e 646f 775f 6163 7469 6f6e 7298 0000  indow_actionr...
-00001400: 0072 1200 0000 da0c 626f 756e 645f 6163  .r......bound_ac
-00001410: 7469 6f6e 726d 0000 0072 4600 0000 7299  tionrm...rF...r.
-00001420: 0000 0072 9a00 0000 729b 0000 0072 9c00  ...r....r....r..
-00001430: 0000 729d 0000 0072 9e00 0000 729f 0000  ..r....r....r...
-00001440: 00da 0f67 6574 5f61 6374 696f 6e5f 6963  ...get_action_ic
-00001450: 6f6e 2904 7240 0000 00da 0176 da06 7265  on).r@.....v..re
-00001460: 7375 6c74 72a0 0000 0072 3700 0000 7237  sultr....r7...r7
-00001470: 0000 0072 3800 0000 724f 0000 009f 0000  ...r8...rO......
-00001480: 0073 2400 0000 0e02 0604 0601 0601 0401  .s$.............
-00001490: 06fd 0a06 0e01 1001 1002 1002 0e01 1001  ................
-000014a0: 0e01 0e01 0a02 0c01 0402 7a14 5265 6e64  ..........z.Rend
-000014b0: 6572 6572 2e61 6374 696f 6e32 6a73 6f6e  erer.action2json
-000014c0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000014d0: 0004 0000 0043 0000 0073 2e00 0000 7400  .....C...s....t.
-000014e0: 7c01 7401 8302 7307 4a00 8201 7c01 a002  |.t...s.J...|...
-000014f0: a100 7d02 7403 7c00 a004 7c02 6a05 a101  ..}.t.|...|.j...
-00001500: 7c02 6a06 6a07 6401 8d02 5300 2902 4e29  |.j.j.d...S.).N)
-00001510: 02da 046d 6169 6eda 0b77 696e 646f 775f  ...main..window_
-00001520: 7369 7a65 2908 72a1 0000 0072 1d00 0000  size).r....r....
-00001530: da11 6765 745f 6c61 796f 7574 5f68 616e  ..get_layout_han
-00001540: 646c 6572 7200 0000 da09 656c 656d 326a  dlerr.....elem2j
-00001550: 736f 6e72 a800 0000 da06 6c61 796f 7574  sonr......layout
-00001560: 72a9 0000 0029 0372 4000 0000 7292 0000  r....).r@...r...
-00001570: 0072 a600 0000 7237 0000 0072 3700 0000  .r....r7...r7...
-00001580: 7238 0000 0072 8700 0000 bc00 0000 730a  r8...r........s.
-00001590: 0000 000e 0108 030c 0106 0106 ff7a 1352  .............z.R
-000015a0: 656e 6465 7265 722e 7061 6e65 6c32 6a73  enderer.panel2js
-000015b0: 6f6e 6302 0000 0000 0000 0000 0000 0004  onc.............
-000015c0: 0000 0005 0000 0003 0000 0073 da00 0000  ...........s....
-000015d0: 7400 7c01 7401 8302 7307 4a00 8201 7402  t.|.t...s.J...t.
-000015e0: 7c01 a003 a100 7c01 6a04 7c01 6a05 6a06  |.....|.j.|.j.j.
-000015f0: 6401 8d03 7d02 7407 7c01 6402 8302 7224  d...}.t.|.d...r$
-00001600: 8700 6601 6403 6404 8408 7c01 6a08 4400  ..f.d.d...|.j.D.
-00001610: 8301 7c02 6405 3c00 7c02 a009 740a 7c01  ..|.d.<.|...t.|.
-00001620: 6406 8302 a101 0100 7407 7c01 6407 8302  d.......t.|.d...
-00001630: 7255 7c02 a009 740a 7c01 6a0b 6408 8302  rU|...t.|.j.d...
-00001640: a101 0100 7407 7c01 6409 8302 7255 7c01  ....t.|.d...rU|.
-00001650: 6a0c 6400 7501 7255 7c01 6a0c a00d a100  j.d.u.rU|.j.....
-00001660: 4400 5d0b 5c02 7d03 7d01 8800 a00e 7c01  D.].\.}.}.....|.
-00001670: a101 7c02 7c03 3c00 7149 740f 7c01 6a05  ..|.|.<.qIt.|.j.
-00001680: 7410 8302 726b 7c02 6a09 7c01 a011 a100  t...rk|.j.|.....
-00001690: 640a 8d01 0100 7c02 6a09 7c01 6a12 6a13  d.....|.j.|.j.j.
-000016a0: 640b 8d01 0100 7c02 5300 290c 4e29 0372  d.....|.S.).N).r
-000016b0: 9600 0000 da08 736f 7274 6162 6c65 da0a  ......sortable..
-000016c0: 7265 6163 745f 6e61 6d65 da08 656c 656d  react_name..elem
-000016d0: 656e 7473 6301 0000 0000 0000 0000 0000  entsc...........
-000016e0: 0002 0000 0005 0000 0013 0000 0073 1e00  .............s..
-000016f0: 0000 6700 7c00 5d0b 7d01 7c01 a000 a100  ..g.|.].}.|.....
-00001700: 7202 8800 a001 7c01 a101 9102 7102 5300  r.....|.....q.S.
-00001710: 7237 0000 0029 02da 0a69 735f 7669 7369  r7...)...is_visi
-00001720: 626c 6572 ab00 0000 2902 7247 0000 00da  bler....).rG....
-00001730: 0165 7251 0000 0072 3700 0000 7238 0000  .erQ...r7...r8..
-00001740: 0072 4900 0000 cc00 0000 7302 0000 001e  .rI.......s.....
-00001750: 007a 2652 656e 6465 7265 722e 656c 656d  .z&Renderer.elem
-00001760: 326a 736f 6e2e 3c6c 6f63 616c 733e 2e3c  2json.<locals>.<
-00001770: 6c69 7374 636f 6d70 3e72 6900 0000 7a98  listcomp>ri...z.
-00001780: 6669 656c 6473 5f69 6e64 6578 2066 6965  fields_index fie
-00001790: 6c64 735f 696e 6465 785f 6869 6464 656e  lds_index_hidden
-000017a0: 2065 6469 7461 626c 6520 7665 7274 6963   editable vertic
-000017b0: 616c 2068 7061 6420 6973 5f66 6965 6c64  al hpad is_field
-000017c0: 7365 7420 6e61 6d65 2077 6964 7468 2070  set name width p
-000017d0: 7265 6665 7272 6564 5f77 6964 7468 2020  referred_width  
-000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001800: 6869 6464 656e 2076 616c 7565 2068 666c  hidden value hfl
-00001810: 6578 2076 666c 6578 7299 0000 007a 1561  ex vflexr....z.a
-00001820: 6374 6f72 5f69 6420 6469 7370 6c61 795f  ctor_id display_
-00001830: 6d6f 6465 da06 736c 6176 6573 2901 da0d  mode..slaves)...
-00001840: 6669 656c 645f 6f70 7469 6f6e 7329 01da  field_options)..
-00001850: 0968 656c 705f 7465 7874 2914 72a1 0000  .help_text).r...
-00001860: 0072 1e00 0000 7272 0000 0072 a200 0000  .r....rr...r....
-00001870: 72ad 0000 0072 4300 0000 da08 5f5f 6e61  r....rC.....__na
-00001880: 6d65 5f5f 7283 0000 0072 af00 0000 7278  me__r....r....rx
-00001890: 0000 0072 2800 0000 7299 0000 0072 b200  ...r(...r....r..
-000018a0: 0000 7269 0000 0072 ab00 0000 da0a 6973  ..ri...r......is
-000018b0: 7375 6263 6c61 7373 7221 0000 00da 1167  subclassr!.....g
-000018c0: 6574 5f66 6965 6c64 5f6f 7074 696f 6e73  et_field_options
-000018d0: da05 6669 656c 6472 b400 0000 2904 7240  ..fieldr....).r@
-000018e0: 0000 0072 a600 0000 72a7 0000 00da 016b  ...r....r......k
-000018f0: 7237 0000 0072 5100 0000 7238 0000 0072  r7...rQ...r8...r
-00001900: ab00 0000 c400 0000 7322 0000 000e 0108  ........s"......
-00001910: 0204 0106 0206 fd0a 0418 0110 020a 0412  ................
-00001920: 0214 0312 0110 010c 0310 0110 0104 027a  ...............z
-00001930: 1252 656e 6465 7265 722e 656c 656d 326a  .Renderer.elem2j
-00001940: 736f 6e63 0100 0000 0000 0000 0000 0000  sonc............
-00001950: 0100 0000 0100 0000 4300 0000 7304 0000  ........C...s...
-00001960: 0064 0153 0029 024e 7a1e 7769 6e64 6f77  .d.S.).Nz.window
-00001970: 2e41 7070 2e64 6173 6862 6f61 7264 2e72  .App.dashboard.r
-00001980: 656c 6f61 6428 293b 7237 0000 0072 5100  eload();r7...rQ.
-00001990: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
-000019a0: 00da 0972 656c 6f61 645f 6a73 e400 0000  ...reload_js....
-000019b0: 7302 0000 0004 017a 1252 656e 6465 7265  s......z.Rendere
-000019c0: 722e 7265 6c6f 6164 5f6a 7363 0200 0000  r.reload_jsc....
-000019d0: 0000 0000 0000 0000 0600 0000 0400 0000  ................
-000019e0: 4f00 0000 73dc 0000 007c 016a 006a 0164  O...s....|.j.j.d
-000019f0: 016b 0272 0f7c 006a 026a 037c 0269 007c  .k.r.|.j.j.|.i.|
-00001a00: 03a4 018e 0153 007c 01a0 04a1 007d 047c  .....S.|.....}.|
-00001a10: 03a0 057c 0464 0219 00a1 0101 0074 067c  ...|.d.......t.|
-00001a20: 037c 0183 0201 007c 016a 0764 0375 0172  .|.....|.j.d.u.r
-00001a30: 2c7c 03a0 0874 096a 0a7c 016a 07a1 0201  ,|...t.j.|.j....
-00001a40: 007c 016a 0b64 0375 0172 397c 03a0 0874  .|.j.d.u.r9|...t
-00001a50: 096a 0c7c 016a 0ba1 0201 007c 016a 0d64  .j.|.j.....|.j.d
-00001a60: 0375 0172 5c7c 016a 0d64 0419 007d 057c  .u.r\|.j.d...}.|
-00001a70: 05a0 0e64 05a1 0172 557c 0564 0664 0385  ...d...rU|.d.d..
-00001a80: 0219 007d 057c 03a0 0874 096a 0f64 07a1  ...}.|...t.j.d..
-00001a90: 0201 007c 03a0 0874 096a 107c 05a1 0201  ...|...t.j.|....
-00001aa0: 007c 006a 026a 037c 016a 006a 117c 016a  .|.j.j.|.j.j.|.j
-00001ab0: 006a 0167 027c 02a2 0152 0069 007c 03a4  .j.g.|...R.i.|..
-00001ac0: 018e 0153 0029 087a 2055 7365 6420 666f  ...S.).z Used fo
-00001ad0: 7220 7475 726e 2072 6571 7565 7374 7320  r turn requests 
-00001ae0: 696e 746f 2075 726c 73da 044d 6169 6eda  into urls..Main.
-00001af0: 0b62 6173 655f 7061 7261 6d73 4e72 0100  .base_paramsNr..
-00001b00: 0000 fa01 2d72 2d00 0000 da04 4445 5343  ....-r-.....DESC
-00001b10: 2912 7299 0000 0072 b500 0000 7241 0000  ).r....r....rA..
-00001b20: 00da 0f62 7569 6c64 5f70 6c61 696e 5f75  ...build_plain_u
-00001b30: 726c da0a 6765 745f 7374 6174 7573 7278  rl..get_statusrx
-00001b40: 0000 0072 0800 0000 da06 6f66 6673 6574  ...r......offset
-00001b50: da0a 7365 7464 6566 6175 6c74 720c 0000  ..setdefaultr...
-00001b60: 00da 0f55 524c 5f50 4152 414d 5f53 5441  ...URL_PARAM_STA
-00001b70: 5254 da05 6c69 6d69 74da 0f55 524c 5f50  RT..limit..URL_P
-00001b80: 4152 414d 5f4c 494d 4954 da08 6f72 6465  ARAM_LIMIT..orde
-00001b90: 725f 6279 da0a 7374 6172 7473 7769 7468  r_by..startswith
-00001ba0: da11 5552 4c5f 5041 5241 4d5f 534f 5254  ..URL_PARAM_SORT
-00001bb0: 4449 52da 0e55 524c 5f50 4152 414d 5f53  DIR..URL_PARAM_S
-00001bc0: 4f52 54da 0961 7070 5f6c 6162 656c 2906  ORT..app_label).
-00001bd0: 7240 0000 00da 0261 72da 0461 7267 73da  r@.....ar..args.
-00001be0: 026b 77da 0273 74da 0273 6372 3700 0000  .kw..st..scr7...
-00001bf0: 7237 0000 0072 3800 0000 da0f 6765 745f  r7...r8.....get_
-00001c00: 7265 7175 6573 745f 7572 6ce7 0000 0073  request_url....s
-00001c10: 2c00 0000 0c02 1201 0802 0e01 0a01 0a01  ,...............
-00001c20: 1001 0a01 1001 0a01 0a01 0a01 0c01 0e01  ................
-00001c30: 0e01 0603 0c01 02ff 0201 06ff 0201 06ff  ................
-00001c40: 7a18 5265 6e64 6572 6572 2e67 6574 5f72  z.Renderer.get_r
-00001c50: 6571 7565 7374 5f75 726c 4e63 0500 0000  equest_urlNc....
-00001c60: 0000 0000 0000 0000 0700 0000 0500 0000  ................
-00001c70: 4b00 0000 73ae 0000 007c 0470 057c 03a0  K...s....|.p.|..
-00001c80: 00a1 007d 0474 017c 0483 0164 016b 0272  ...}.t.|...d.k.r
-00001c90: 1164 02a0 027c 04a1 017d 047c 036a 036a  .d...|...}.|.j.j
-00001ca0: 0472 2c7c 036a 036a 0573 2c7c 00a0 067c  .r,|.j.j.s,|...|
-00001cb0: 027c 037c 01a1 037d 067c 006a 077c 027c  .|.|...}.|.j.|.|
-00001cc0: 037c 067c 0466 0469 007c 05a4 018e 0153  .|.|.f.i.|.....S
-00001cd0: 007c 036a 036a 0872 4b7c 02a0 09a1 007d  .|.j.j.rK|.....}
-00001ce0: 067c 0164 0075 0172 3f7c 066a 0a7c 016a  .|.d.u.r?|.j.|.j
-00001cf0: 0b64 038d 0101 007c 006a 077c 027c 037c  .d.....|.j.|.|.|
-00001d00: 067c 0466 0469 007c 05a4 018e 0153 007c  .|.f.i.|.....S.|
-00001d10: 006a 0c7c 017c 027c 037c 0466 0469 007c  .j.|.|.|.|.f.i.|
-00001d20: 05a4 018e 0153 0029 044e 722d 0000 0075  .....S.).Nr-...u
-00001d30: 0600 0000 c2a0 7b7d c2a0 2901 da09 7265  ......{}..)...re
-00001d40: 636f 7264 5f69 6429 0dda 1067 6574 5f62  cord_id)...get_b
-00001d50: 7574 746f 6e5f 6c61 6265 6cda 036c 656e  utton_label..len
-00001d60: da06 666f 726d 6174 726d 0000 00da 0a70  ..formatrm.....p
-00001d70: 6172 616d 6574 6572 73da 106e 6f5f 7061  arameters..no_pa
-00001d80: 7261 6d73 5f77 696e 646f 77da 1167 6574  rams_window..get
-00001d90: 5f61 6374 696f 6e5f 7374 6174 7573 da14  _action_status..
-00001da0: 7769 6e64 6f77 5f61 6374 696f 6e5f 6275  window_action_bu
-00001db0: 7474 6f6e da0e 6f70 656e 735f 615f 7769  tton..opens_a_wi
-00001dc0: 6e64 6f77 72c0 0000 0072 7800 0000 da02  ndowr....rx.....
-00001dd0: 706b da11 726f 775f 6163 7469 6f6e 5f62  pk..row_action_b
-00001de0: 7574 746f 6e29 0772 4000 0000 da03 6f62  utton).r@.....ob
-00001df0: 6a72 cb00 0000 7290 0000 0072 9600 0000  jr....r....r....
-00001e00: 72cd 0000 0072 ce00 0000 7237 0000 0072  r....r....r7...r
-00001e10: 3700 0000 7238 0000 00da 0d61 6374 696f  7...r8.....actio
-00001e20: 6e5f 6275 7474 6f6e ff00 0000 7320 0000  n_button....s ..
-00001e30: 000c 010c 010a 0110 020e 0104 0108 0104  ................
-00001e40: ff02 0106 ff08 0208 0108 010e 0118 0118  ................
-00001e50: 017a 1652 656e 6465 7265 722e 6163 7469  .z.Renderer.acti
-00001e60: 6f6e 5f62 7574 746f 6e63 0500 0000 0000  on_buttonc......
-00001e70: 0000 0000 0000 0700 0000 0400 0000 4b00  ..............K.
-00001e80: 0000 7340 0000 007c 0264 0175 0072 0d7c  ..s@...|.d.u.r.|
-00001e90: 036a 0064 0269 007c 04a4 018e 017d 066e  .j.d.i.|.....}.n
-00001ea0: 097c 026a 017c 0366 0169 007c 04a4 018e  .|.j.|.f.i.|....
-00001eb0: 017d 067c 006a 027c 067c 0166 0269 007c  .}.|.j.|.|.f.i.|
-00001ec0: 05a4 018e 0153 0029 0361 cf01 0000 4e6f  .....S.).a....No
-00001ed0: 7465 2074 6861 7420 6062 612e 6163 746f  te that `ba.acto
-00001ee0: 7260 206d 6179 2064 6966 6665 7220 6672  r` may differ fr
-00001ef0: 6f6d 2060 6172 2e61 6374 6f72 6020 7768  om `ar.actor` wh
-00001f00: 656e 2064 6566 696e 6564 206f 6e20 610a  en defined on a.
-00001f10: 2020 2020 2020 2020 6469 6666 6572 656e          differen
-00001f20: 7420 6163 746f 722e 2052 656d 656d 6265  t actor. Remembe
-00001f30: 7220 652e 672e 2074 6865 2022 4d75 7374  r e.g. the "Must
-00001f40: 2072 6561 6420 6549 4420 6361 7264 2220   read eID card" 
-00001f50: 6163 7469 6f6e 0a20 2020 2020 2020 2062  action.        b
-00001f60: 7574 746f 6e20 696e 2065 6964 5f69 6e66  utton in eid_inf
-00001f70: 6f20 6f66 206e 6577 636f 6d65 7273 2e4e  o of newcomers.N
-00001f80: 6577 436c 6965 6e74 7320 2832 3031 3430  ewClients (20140
-00001f90: 3432 3229 2e0a 0a20 2020 2020 2020 203a  422)...        :
-00001fa0: 6f62 6a3a 2020 5468 6520 6461 7461 6261  obj:  The databa
-00001fb0: 7365 206f 626a 6563 740a 2020 2020 2020  se object.      
-00001fc0: 2020 3a61 723a 2020 2054 6865 2061 6374    :ar:   The act
-00001fd0: 696f 6e20 7265 7175 6573 740a 2020 2020  ion request.    
-00001fe0: 2020 2020 3a62 613a 2020 5468 6520 626f      :ba:  The bo
-00001ff0: 756e 6420 6163 7469 6f6e 0a20 2020 2020  und action.     
-00002000: 2020 203a 7265 7175 6573 745f 6b77 6172     :request_kwar
-00002010: 6773 3a20 6b65 7977 6f72 6420 6172 6775  gs: keyword argu
-00002020: 6d65 6e74 7320 746f 2066 6f72 7761 7264  ments to forward
-00002030: 6564 2074 6f20 7468 6520 6368 696c 6420  ed to the child 
-00002040: 6163 7469 6f6e 2072 6571 7565 7374 0a0a  action request..
-00002050: 2020 2020 2020 2020 416e 7920 6b65 7977          Any keyw
-00002060: 6f72 6420 6f74 6865 7220 6172 6775 6d65  ord other argume
-00002070: 6e74 7320 6172 6520 666f 7277 6172 6465  nts are forwarde
-00002080: 6420 746f 203a 6d65 7468 3a60 6172 326a  d to :meth:`ar2j
-00002090: 7360 2e0a 0a20 2020 2020 2020 204e 7237  s`...        Nr7
-000020a0: 0000 0029 03da 0772 6571 7565 7374 da05  ...)...request..
-000020b0: 7370 6177 6eda 0561 7232 6a73 2907 7240  spawn..ar2js).r@
-000020c0: 0000 0072 dc00 0000 72cb 0000 0072 9000  ...r....r....r..
-000020d0: 0000 da0e 7265 7175 6573 745f 6b77 6172  ....request_kwar
-000020e0: 6773 da06 7374 6174 7573 da03 7361 7272  gs..status..sarr
-000020f0: 3700 0000 7237 0000 0072 3800 0000 da17  7...r7...r8.....
-00002100: 6163 7469 6f6e 5f63 616c 6c5f 6f6e 5f69  action_call_on_i
-00002110: 6e73 7461 6e63 6510 0100 0073 0800 0000  nstance....s....
-00002120: 080e 1201 1203 1401 7a20 5265 6e64 6572  ........z Render
-00002130: 6572 2e61 6374 696f 6e5f 6361 6c6c 5f6f  er.action_call_o
-00002140: 6e5f 696e 7374 616e 6365 6302 0000 0000  n_instancec.....
-00002150: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-00002160: 0000 0073 2c00 0000 7c01 6a00 7005 7c01  ...s,...|.j.p.|.
-00002170: 6a01 7d02 7402 a003 7c02 6401 a102 7d03  j.}.t...|.d...}.
-00002180: 7c03 6401 7500 7212 6401 5300 6402 7c03  |.d.u.r.d.S.d.|.
-00002190: 1600 5300 2903 7abf 0a20 2020 2020 2020  ..S.).z..       
-000021a0: 2055 7365 7320 616e 2069 6e74 6572 6e61   Uses an interna
-000021b0: 6c20 6d61 7070 696e 6720 666f 7220 6963  l mapping for ic
-000021c0: 6f6e 206e 616d 6573 2074 6f20 636f 6e76  on names to conv
-000021d0: 6572 7420 6578 6973 7469 6e67 2069 636f  ert existing ico
-000021e0: 6e73 2069 6e74 6f20 7265 6163 742d 7573  ns into react-us
-000021f0: 6162 6c65 2e0a 2020 2020 2020 2020 3a70  able..        :p
-00002200: 6172 616d 2061 6374 696f 6e3a 0a20 2020  aram action:.   
-00002210: 2020 2020 203a 7265 7475 726e 3a20 7374       :return: st
-00002220: 723a 2061 2069 636f 6e20 6e61 6d65 2066  r: a icon name f
-00002230: 6f72 2065 6974 6865 7220 7072 696d 652d  or either prime-
-00002240: 7265 6163 7420 6f72 2069 636f 6e38 0a20  react or icon8. 
-00002250: 2020 2020 2020 204e 7a05 7069 2025 7329         Nz.pi %s)
-00002260: 04da 0f72 6561 6374 5f69 636f 6e5f 6e61  ...react_icon_na
-00002270: 6d65 da09 6963 6f6e 5f6e 616d 6572 2e00  me..icon_namer..
-00002280: 0000 da03 6765 7429 0472 4000 0000 726d  ....get).r@...rm
-00002290: 0000 0072 a000 0000 da0a 7265 6163 745f  ...r......react_
-000022a0: 6963 6f6e 7237 0000 0072 3700 0000 7238  iconr7...r7...r8
-000022b0: 0000 0072 a500 0000 2501 0000 730a 0000  ...r....%...s...
-000022c0: 000c 070c 0108 0104 0108 027a 1852 656e  ...........z.Ren
-000022d0: 6465 7265 722e 6765 745f 6163 7469 6f6e  derer.get_action
-000022e0: 5f69 636f 6e63 0300 0000 0000 0000 0000  _iconc..........
-000022f0: 0000 0800 0000 0700 0000 4b00 0000 73a4  ..........K...s.
-00002300: 0000 007c 016a 007d 047c 016a 017d 0569  ...|.j.}.|.j.}.i
-00002310: 007d 067c 056a 02a0 03a1 0072 1c7c 03a0  .}.|.j.....r.|..
-00002320: 047c 00a0 057c 017c 057c 02a1 03a1 0101  .|...|.|.|......
-00002330: 007c 06a0 047c 03a1 0101 007c 06a0 047c  .|...|.....|...|
-00002340: 00a0 067c 017c 057c 02a1 03a1 0101 007c  ...|.|.|.......|
-00002350: 06a0 047c 03a1 0101 007c 047c 056a 026a  ...|.....|.|.j.j
-00002360: 077c 016a 087c 056a 096a 0a7c 0664 019c  .|.j.|.j.j.|.d..
-00002370: 057d 0774 0b7c 0264 0283 0272 437c 026a  .}.t.|.d...rC|.j
-00002380: 0c7c 0764 033c 006e 0974 0d7c 0274 0e83  .|.d.<.n.t.|.t..
-00002390: 0272 4c7c 027c 0764 033c 0064 0474 0f7c  .rL|.|.d.<.d.t.|
-000023a0: 0783 0116 0053 0029 057a 4349 6d70 6c65  .....S.).zCImple
-000023b0: 6d65 6e74 7320 3a6d 6574 683a 606c 696e  ments :meth:`lin
-000023c0: 6f2e 636f 7265 2e72 656e 6465 7265 722e  o.core.renderer.
-000023d0: 4874 6d6c 5265 6e64 6572 6572 2e61 7232  HtmlRenderer.ar2
-000023e0: 6a73 602e 0a0a 2020 2020 2020 2020 2905  js`...        ).
-000023f0: da02 7270 7295 0000 00da 066f 6e4d 6169  ..rpr......onMai
-00002400: 6eda 0761 6374 6f72 4964 72e2 0000 0072  n..actorIdr....r
-00002410: da00 0000 da02 7372 fa18 7769 6e64 6f77  ......sr..window
-00002420: 2e41 7070 2e72 756e 4163 7469 6f6e 2825  .App.runAction(%
-00002430: 7329 2910 da10 7265 7175 6573 7469 6e67  s))...requesting
-00002440: 5f70 616e 656c 72a4 0000 0072 6d00 0000  _panelr....rm...
-00002450: 72a3 0000 0072 7800 0000 72d7 0000 00da  r....rx...r.....
-00002460: 1167 6574 5f61 6374 696f 6e5f 7061 7261  .get_action_para
-00002470: 6d73 724e 0000 00da 1069 735f 6f6e 5f6d  msrN.....is_on_m
-00002480: 6169 6e5f 6163 746f 7272 9900 0000 da08  ain_actorr......
-00002490: 6163 746f 725f 6964 7283 0000 0072 da00  actor_idr....r..
-000024a0: 0000 72a1 0000 0072 7900 0000 7226 0000  ..r....ry...r&..
-000024b0: 0029 0872 4000 0000 72cb 0000 0072 dc00  .).r@...r....r..
-000024c0: 0000 72e2 0000 0072 e900 0000 7290 0000  ..r....r....r...
-000024d0: 00da 0670 6172 616d 73da 066a 735f 6f62  ...params..js_ob
-000024e0: 6a72 3700 0000 7237 0000 0072 3800 0000  jr7...r7...r8...
-000024f0: 72e0 0000 0033 0100 0073 2a00 0000 0604  r....3...s*.....
-00002500: 0601 0401 0a01 1404 0a01 1401 0a01 0203  ................
-00002510: 0601 0401 0601 0201 06fb 0a07 0c01 0a02  ................
-00002520: 0801 0202 0601 04ff 7a0e 5265 6e64 6572  ........z.Render
-00002530: 6572 2e61 7232 6a73 6302 0000 0000 0000  er.ar2jsc.......
-00002540: 0000 0000 0006 0000 0006 0000 0043 0000  .............C..
-00002550: 0073 bc01 0000 7c01 7400 6a01 6a02 7500  .s....|.t.j.j.u.
-00002560: 720a 7403 6401 8301 5300 7404 7c01 7405  r.t.d...S.t.|.t.
-00002570: 8302 7216 7406 6402 a007 7c01 a101 8301  ..r.t.d...|.....
-00002580: 8201 7404 7c01 7408 6a09 8302 7220 0900  ..t.|.t.j...r ..
-00002590: 7c01 6a0a 5300 7404 7c01 740b 6a0c 8302  |.j.S.t.|.t.j...
-000025a0: 7229 7c01 6a0d 5300 7404 7c01 7406 8302  r)|.j.S.t.|.t...
-000025b0: 7232 740e 7c01 8301 5300 7404 7c01 740f  r2t.|...S.t.|.t.
-000025c0: 8302 724a 7c01 6a10 6403 7500 723f 7c01  ..rJ|.j.d.u.r?|.
-000025d0: 6a11 5300 7412 7c01 6a13 7412 7c01 6a11  j.S.t.|.j.t.|.j.
-000025e0: 6404 8d01 6405 8d02 5300 7404 7c01 7414  d...d...S.t.|.t.
-000025f0: 8302 72cc 7c01 6a15 6403 7501 726d 7c00  ..r.|.j.d.u.rm|.
-00002600: a016 6403 7c01 6a15 6403 a103 7d02 7c02  ..d.|.j.d...}.|.
-00002610: 6403 7501 7362 4a00 8201 6406 7c02 1600  d.u.sbJ...d.|...
-00002620: 7d03 7c00 a017 7c01 7c02 6403 a103 5300  }.|...|.|.d...S.
-00002630: 7c01 6a18 6403 7501 7295 7c01 6a19 7285  |.j.d.u.r.|.j.r.
-00002640: 7c01 6a18 6a1a 640d 6900 7c01 6a19 a401  |.j.j.d.i.|.j...
-00002650: 8e01 7d04 7c00 a01b 7c04 a101 7d03 6e08  ..}.|...|...}.n.
-00002660: 7c00 a01c 6403 7c01 6a18 6900 a103 7d03  |...d.|.j.i...}.
-00002670: 7c00 a017 7c01 7c03 7c01 6a1d a103 5300  |...|.|.|.j...S.
-00002680: 7c01 6a1e 6403 7501 72a7 6406 7c01 6a1e  |.j.d.u.r.d.|.j.
-00002690: 1600 7d03 7c00 a017 7c01 7c03 7c01 6a1d  ..}.|...|.|.|.j.
-000026a0: a103 5300 7c01 6a1f 6403 7501 72b0 7c01  ..S.|.j.d.u.r.|.
-000026b0: 6a1f 7d05 6e03 7c01 6a13 5300 7c01 6a10  j.}.n.|.j.S.|.j.
-000026c0: 6a10 6403 7500 72c5 7412 6407 7c01 6a13  j.d.u.r.t.d.|.j.
-000026d0: 7403 6408 7c05 1600 8301 6409 8d03 5300  t.d.|.....d...S.
-000026e0: 7412 7c01 6a13 7c05 640a 8d02 5300 7404  t.|.j.|.d...S.t.
-000026f0: 7c01 7403 8302 72dc 7420 7c00 640b 640c  |.t...r.t |.d.d.
-00002700: 8303 72dc 740e 7c01 6a21 8301 5300 7c01  ..r.t.|.j!..S.|.
-00002710: 5300 290e 7a54 0a20 2020 2020 2020 2041  S.).zT.        A
-00002720: 6464 6974 696f 6e61 6c20 636f 6e76 6572  dditional conver
-00002730: 7469 6e67 206c 6f67 6963 2066 6f72 2073  ting logic for s
-00002740: 6572 6961 6c69 7a69 6e67 2050 7974 686f  erializing Pytho
-00002750: 6e20 7661 6c75 6573 2074 6f20 6a73 6f6e  n values to json
-00002760: 2e0a 2020 2020 2020 2020 da10 4c41 4e47  ..        ..LANG
-00002770: 5541 4745 5f43 484f 4943 4553 7a0b 3230  UAGE_CHOICESz.20
-00002780: 3231 3035 3137 207b 7d4e 2901 7269 0000  210517 {}N).ri..
-00002790: 0029 0272 4500 0000 7256 0000 007a 0225  .).rE...rV...z.%
-000027a0: 73da 0662 7574 746f 6e7a 2366 756e 6374  s..buttonz#funct
-000027b0: 696f 6e28 2920 7b20 4c69 6e6f 2e6c 6f61  ion() { Lino.loa
-000027c0: 645f 7572 6c28 2725 7327 293b 207d 2903  d_url('%s'); }).
-000027d0: da05 7874 7970 6572 4500 0000 da07 6861  ..xtyperE.....ha
-000027e0: 6e64 6c65 7229 0272 4500 0000 da04 6872  ndler).rE.....hr
-000027f0: 6566 726f 0000 0046 7237 0000 0029 2272  efro...Fr7...)"r
-00002800: 0400 0000 7270 0000 0072 f400 0000 7227  ....rp...r....r'
-00002810: 0000 0072 a100 0000 721c 0000 00da 0945  ...r....r......E
-00002820: 7863 6570 7469 6f6e 72d4 0000 0072 0d00  xceptionr....r..
-00002830: 0000 da06 4368 6f69 6365 7244 0000 0072  ....ChoicerD...r
-00002840: 0500 0000 da05 4d6f 6465 6c72 da00 0000  ......Modelr....
-00002850: 7246 0000 0072 0a00 0000 da06 7061 7265  rF...r......pare
-00002860: 6e74 7269 0000 0072 7200 0000 7296 0000  ntri...rr...r...
-00002870: 0072 0b00 0000 da08 696e 7374 616e 6365  .r......instance
-00002880: da10 696e 7374 616e 6365 5f68 616e 646c  ..instance_handl
-00002890: 6572 da0c 6861 6e64 6c65 725f 6974 656d  er..handler_item
-000028a0: 72a4 0000 0072 f200 0000 72de 0000 00da  r....r....r.....
-000028b0: 0f72 6571 7565 7374 5f68 616e 646c 6572  .request_handler
-000028c0: da0b 6163 7469 6f6e 5f63 616c 6c72 b400  ..action_callr..
-000028d0: 0000 da0a 6a61 7661 7363 7269 7074 72f8  ....javascriptr.
-000028e0: 0000 00da 0767 6574 6174 7472 da01 7329  .....getattr..s)
-000028f0: 0672 4000 0000 72a6 0000 00da 0168 da02  .r@...r......h..
-00002900: 6a73 72cb 0000 00da 0375 726c 7237 0000  jsr......urlr7..
-00002910: 0072 3700 0000 7238 0000 0072 3f00 0000  .r7...r8...r?...
-00002920: 5401 0000 7354 0000 000c 0408 010a 010e  T...sT..........
-00002930: 010c 0102 0106 030c 0106 010a 0108 010a  ................
-00002940: 010a 0106 0116 030a 020a 0110 010c 0108  ................
-00002950: 010e 010a 0106 0114 010c 0110 0210 010a  ................
-00002960: 020a 0110 010a 0108 0106 070c 0202 0206  ................
-00002970: 010a 0206 fd0e 0416 020a 0204 027a 1852  .............z.R
-00002980: 656e 6465 7265 722e 7079 326a 735f 636f  enderer.py2js_co
-00002990: 6e76 6572 7465 7263 0400 0000 0000 0000  nverterc........
-000029a0: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
-000029b0: 7350 0000 0074 007c 016a 017c 0264 018d  sP...t.|.j.|.d..
-000029c0: 027d 047c 016a 0272 1a7c 016a 026a 036a  .}.|.j.r.|.j.j.j
-000029d0: 0472 1a7c 046a 0564 027c 016a 026a 036a  .r.|.j.d.|.j.j.j
-000029e0: 0417 0064 038d 0101 0074 066a 076a 0872  ...d.....t.j.j.r
-000029f0: 267c 0372 267c 046a 057c 0364 048d 0101  &|.r&|.j.|.d....
-00002a00: 007c 0453 0029 05da 0029 0272 4500 0000  .|.S.)...).rE...
-00002a10: 72f7 0000 007a 0778 2d74 6261 722d 2901  r....z.x-tbar-).
-00002a20: da07 6963 6f6e 436c 7329 01da 0774 6f6f  ..iconCls)...too
-00002a30: 6c54 6970 2909 7272 0000 0072 9600 0000  lTip).rr...r....
-00002a40: 72a4 0000 0072 6d00 0000 72e6 0000 0072  r....rm...r....r
-00002a50: 7800 0000 7204 0000 0072 7000 0000 da0d  x...r....rp.....
-00002a60: 7573 655f 7175 6963 6b74 6970 7329 0572  use_quicktips).r
-00002a70: 4000 0000 da02 6d69 72f7 0000 0072 b400  @.....mir....r..
-00002a80: 0000 da01 6472 3700 0000 7237 0000 0072  ....dr7...r7...r
-00002a90: 3800 0000 72ff 0000 00a2 0100 0073 0c00  8...r........s..
-00002aa0: 0000 0e04 1001 1601 0c01 0c03 0401 7a15  ..............z.
-00002ab0: 5265 6e64 6572 6572 2e68 616e 646c 6572  Renderer.handler
-00002ac0: 5f69 7465 6d63 0200 0000 0000 0000 0000  _itemc..........
-00002ad0: 0000 0500 0000 0500 0000 4f00 0000 7320  ..........O...s 
-00002ae0: 0000 007c 016a 0064 0269 007c 03a4 018e  ...|.j.d.i.|....
-00002af0: 017d 047c 00a0 017c 017c 016a 027c 04a1  .}.|...|.|.j.|..
-00002b00: 0353 0029 037a 3620 4765 6e65 7261 7465  .S.).z6 Generate
-00002b10: 7320 6a73 2073 7472 696e 6720 666f 7220  s js string for 
-00002b20: 6163 7469 6f6e 2062 7574 746f 6e20 6361  action button ca
-00002b30: 6c6c 732e 0a20 2020 2020 2020 204e 7237  lls..        Nr7
-00002b40: 0000 0029 0372 c000 0000 7201 0100 0072  ...).r....r....r
-00002b50: a400 0000 2905 7240 0000 0072 cb00 0000  ....).r@...r....
-00002b60: 72cc 0000 0072 cd00 0000 72ce 0000 0072  r....r....r....r
-00002b70: 3700 0000 7237 0000 0072 3800 0000 7200  7...r7...r8...r.
-00002b80: 0100 00b0 0100 0073 0400 0000 1004 1001  .......s........
-00002b90: 7a18 5265 6e64 6572 6572 2e72 6571 7565  z.Renderer.reque
-00002ba0: 7374 5f68 616e 646c 6572 6304 0000 0000  st_handlerc.....
-00002bb0: 0000 0000 0000 0008 0000 0008 0000 0043  ...............C
-00002bc0: 0000 0073 9c00 0000 7c02 6a00 7d04 7c02  ...s....|.j.}.|.
-00002bd0: a001 a100 a002 6401 6402 a102 5c02 7d05  ......d.d...\.}.
-00002be0: 7d06 7c03 7311 6900 7d03 7c01 6400 7501  }.|.s.i.}.|.d.u.
-00002bf0: 7222 7403 7c01 6403 8302 7222 7c01 6a04  r"t.|.d...r"|.j.
-00002c00: 6408 6900 7c03 a401 8e01 7d03 7c01 722d  d.i.|.....}.|.r-
-00002c10: 7c01 6a05 722d 7c01 6a05 7c03 7406 6a07  |.j.r-|.j.|.t.j.
-00002c20: 3c00 7c06 6404 6b02 7239 7403 7c03 6405  <.|.d.k.r9t.|.d.
-00002c30: 8302 7239 7c03 6405 3d00 7c01 6400 7500  ..r9|.d.=.|.d.u.
-00002c40: 723f 6400 6e02 7c01 6a08 7d07 6406 7409  r?d.n.|.j.}.d.t.
-00002c50: 740a 7c06 7c05 7c03 7c07 6407 8d04 8301  t.|.|.|.|.d.....
-00002c60: 1600 5300 2909 4eda 012e 722d 0000 0072  ..S.).N...r-...r
-00002c70: c000 0000 da04 6772 6964 72d1 0000 0072  ......gridr....r
-00002c80: ed00 0000 2904 7295 0000 0072 eb00 0000  ....).r....r....
-00002c90: 72e2 0000 0072 e900 0000 7237 0000 0029  r....r....r7...)
-00002ca0: 0b72 6d00 0000 da09 6675 6c6c 5f6e 616d  .rm.....full_nam
-00002cb0: 65da 0672 7370 6c69 7472 8300 0000 72c0  e..rsplitr....r.
-00002cc0: 0000 00da 0a73 7562 7374 5f75 7365 7272  .....subst_userr
-00002cd0: 0c00 0000 da14 5552 4c5f 5041 5241 4d5f  ......URL_PARAM_
-00002ce0: 5355 4253 545f 5553 4552 72ee 0000 0072  SUBST_USERr....r
-00002cf0: 2600 0000 7272 0000 0029 0872 4000 0000  &...rr...).r@...
-00002d00: 72cb 0000 0072 a400 0000 72e2 0000 0072  r....r....r....r
-00002d10: 5000 0000 72eb 0000 0072 9500 0000 72e9  P...r....r....r.
-00002d20: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
-00002d30: 0000 7201 0100 00ba 0100 0073 2200 0000  ..r........s"...
-00002d40: 0602 1402 0402 0401 1202 1001 0a02 0c01  ................
-00002d50: 1211 0601 1202 0602 0201 0201 0201 0201  ................
-00002d60: 0afc 7a14 5265 6e64 6572 6572 2e61 6374  ..z.Renderer.act
-00002d70: 696f 6e5f 6361 6c6c 6302 0000 0000 0000  ion_callc.......
-00002d80: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00002d90: 0073 2e00 0000 7c01 7304 6400 5300 7400  .s....|.s.d.S.t.
-00002da0: 7c01 7401 8302 730d 7401 7c01 8301 7d01  |.t...s.t.|...}.
-00002db0: 7402 7c01 6401 6402 8d02 7d01 6403 7c01  t.|.d.d...}.d.|.
-00002dc0: 1700 5300 2904 4e46 2901 da05 7175 6f74  ..S.).NF)...quot
-00002dd0: 657a 0b6a 6176 6173 6372 6970 743a 2903  ez.javascript:).
-00002de0: 72a1 0000 0072 4600 0000 7203 0000 0029  r....rF...r....)
-00002df0: 0272 4000 0000 7206 0100 0072 3700 0000  .r@...r....r7...
-00002e00: 7237 0000 0072 3800 0000 da06 6a73 3275  r7...r8.....js2u
-00002e10: 726c e401 0000 730c 0000 0004 0104 010a  rl....s.........
-00002e20: 0208 010c 0108 017a 0f52 656e 6465 7265  .......z.Rendere
-00002e30: 722e 6a73 3275 726c 6306 0000 0000 0000  r.js2urlc.......
-00002e40: 0000 0000 0007 0000 0004 0000 0043 0000  .............C..
-00002e50: 0073 5600 0000 7400 6a01 6a02 7227 7400  .sV...t.j.j.r't.
-00002e60: 6a01 6a03 720f 6401 7c04 7c05 6602 1600  j.j.r.d.|.|.f...
-00002e70: 7d06 6e02 6402 7d06 7c02 7219 7404 6403  }.n.d.}.|.r.t.d.
-00002e80: 7c06 7c02 8303 7d06 7c06 7229 7c01 6a05  |.|...}.|.r)|.j.
-00002e90: 6404 7c03 7c06 6602 1600 6405 8d01 0100  d.|.|.f...d.....
-00002ea0: 6400 5300 6400 5300 6400 5300 2906 4e7a  d.S.d.S.d.S.).Nz
-00002eb0: 0828 2573 2e25 7329 2072 0801 0000 7a04  .(%s.%s) r....z.
-00002ec0: 7b7d 7b7d 7a07 2825 732c 2573 2929 01da  {}{}z.(%s,%s))..
-00002ed0: 0871 7569 636b 7469 7029 0672 0400 0000  .quicktip).r....
-00002ee0: 7270 0000 0072 0b01 0000 da19 7368 6f77  rp...r......show
-00002ef0: 5f69 6e74 6572 6e61 6c5f 6669 656c 645f  _internal_field_
-00002f00: 6e61 6d65 7372 0600 0000 7278 0000 0029  namesr....rx...)
-00002f10: 0772 4000 0000 72cd 0000 0072 b400 0000  .r@...r....r....
-00002f20: 7275 0000 00da 0a64 6174 6173 6f75 7263  ru.....datasourc
-00002f30: 65da 0966 6965 6c64 6e61 6d65 da03 7474  e..fieldname..tt
-00002f40: 7472 3700 0000 7237 0000 0072 3800 0000  tr7...r7...r8...
-00002f50: da0d 6164 645f 6865 6c70 5f74 6578 74ed  ..add_help_text.
-00002f60: 0100 0073 1800 0000 0801 0801 0e01 0402  ...s............
-00002f70: 0401 0c01 0401 0804 0201 0eff 04f5 0407  ................
-00002f80: 7a16 5265 6e64 6572 6572 2e61 6464 5f68  z.Renderer.add_h
-00002f90: 656c 705f 7465 7874 6302 0000 0000 0000  elp_textc.......
-00002fa0: 0000 0000 0005 0000 0003 0000 0043 0000  .............C..
-00002fb0: 0073 5600 0000 7400 8300 7d02 6401 7c01  .sV...t...}.d.|.
-00002fc0: 1700 6402 1700 7d03 7c00 6a01 a002 6403  ..d...}.|.j...d.
-00002fd0: a101 6404 1900 7d04 7c02 6405 7501 721c  ..d...}.|.d.u.r.
-00002fe0: 7c03 7c02 6a03 6402 1700 3700 7d03 7c03  |.|.j.d...7.}.|.
-00002ff0: 7404 a005 a100 6403 1700 7c04 1700 3700  t.....d...|...7.
-00003000: 7d03 6406 7c04 7c03 6603 5300 2907 7a2c  }.d.|.|.f.S.).z,
-00003010: 4c69 6b65 206c 696e 6f5f 6a73 5f70 6172  Like lino_js_par
-00003020: 7473 2c20 6275 7420 666f 7220 6163 746f  ts, but for acto
-00003030: 725f 6c65 7665 6c20 6461 7461 da05 4c69  r_level data..Li
-00003040: 6e6f 5fda 015f 720e 0100 0072 2f00 0000  no_.._r....r/...
-00003050: 4eda 0563 6163 6865 2906 7229 0000 00da  N..cache).r)....
-00003060: 116c 696e 6f5f 7765 625f 7465 6d70 6c61  .lino_web_templa
-00003070: 7465 7211 0100 0072 4400 0000 7207 0000  ter....rD...r...
-00003080: 00da 0c67 6574 5f6c 616e 6775 6167 6529  ...get_language)
-00003090: 0572 4000 0000 72eb 0000 00da 0975 7365  .r@...r......use
-000030a0: 725f 7479 7065 da08 6669 6c65 6e61 6d65  r_type..filename
-000030b0: da09 6669 6c65 5f74 7970 6572 3700 0000  ..file_typer7...
-000030c0: 7237 0000 0072 3800 0000 da15 6c69 6e6f  r7...r8.....lino
-000030d0: 5f6a 735f 7061 7274 735f 6368 756e 6b65  _js_parts_chunke
-000030e0: 64fc 0100 0073 0e00 0000 0602 0c01 1001  d....s..........
-000030f0: 0801 0e01 1401 0a01 7a1e 5265 6e64 6572  ........z.Render
-00003100: 6572 2e6c 696e 6f5f 6a73 5f70 6172 7473  er.lino_js_parts
-00003110: 5f63 6875 6e6b 6564 6302 0000 0000 0000  _chunkedc.......
-00003120: 0000 0000 0011 0000 0006 0000 0043 0000  .............C..
-00003130: 0073 de01 0000 6700 7d02 6700 7d03 7c01  .s....g.}.g.}.|.
-00003140: 4400 5de4 7d04 7c04 a000 a100 7d05 7c05  D.].}.|.....}.|.
-00003150: 7312 7c04 6a01 6a02 72cc 7403 6a04 7c04  s.|.j.j.r.t.j.|.
-00003160: 6a01 6a05 6901 7d06 7c05 7223 7c06 6a06  j.j.i.}.|.r#|.j.
-00003170: 7c05 6a07 6a08 6401 8d01 0100 7c04 6a01  |.j.j.d.....|.j.
-00003180: 6a02 72c7 6700 7d07 7409 8300 7d08 7c04  j.r.g.}.t...}.|.
-00003190: 6a0a a00b 7c04 6a01 740c 8300 a102 4400  j...|.j.t.....D.
-000031a0: 5d72 7d09 7409 7c09 6a01 6a05 6402 8d01  ]r}.t.|.j.j.d...
-000031b0: 7d0a 7c09 6a01 6a0d 7d0b 7c0b 7248 7c0b  }.|.j.j.}.|.rH|.
-000031c0: 7c0a 6403 3c00 7c09 6a01 6a0e 7d0c 7c0c  |.d.<.|.j.j.}.|.
-000031d0: 725e 740f 7c0c 8301 725a 7c0c 7c09 6a0a  r^t.|...rZ|.|.j.
-000031e0: 8301 7c0a 6404 3c00 6e04 7c0c 7c0a 6404  ..|.d.<.n.|.|.d.
-000031f0: 3c00 7c09 6a01 6a10 6405 7501 7284 7c09  <.|.j.j.d.u.r.|.
-00003200: 6a01 6a10 7d0d 7c0d 7c08 7600 7274 7c08  j.j.}.|.|.v.rt|.
-00003210: 7c0d 1900 a011 7c0a a101 0100 6e15 7409  |.....|.....n.t.
-00003220: 7c0d 6406 8d01 7d0e 7c0a 6701 7c08 7c0d  |.d...}.|.g.|.|.
-00003230: 3c00 7c07 a011 7c0e a101 0100 6e05 7c07  <.|...|.....n.|.
-00003240: a011 7c0a a101 0100 7c09 6a01 6a12 72a7  ..|.....|.j.j.r.
-00003250: 7413 7c09 6a01 6a12 8301 7d0f 7414 7c0f  t.|.j.j...}.t.|.
-00003260: 6407 8302 739e 7c09 6a01 6a05 7c0f 6407  d...s.|.j.j.|.d.
-00003270: 3c00 7c0f 7c03 7601 72a7 7c03 a011 7c0f  <.|.|.v.r.|...|.
-00003280: a101 0100 7135 7c08 72c3 7415 7c07 8301  ....q5|.r.t.|...
-00003290: 4400 5d14 5c02 7d10 7d0a 7c0a a016 6408  D.].\.}.}.|...d.
-000032a0: 6409 a102 72c2 7c08 7c0a 6408 1900 1900  d...r.|.|.d.....
-000032b0: 7c07 7c10 1900 640a 3c00 71ae 7c07 7c06  |.|...d.<.q.|.|.
-000032c0: 640b 3c00 7c02 a011 7c06 a101 0100 7c04  d.<.|...|.....|.
-000032d0: 6a01 6a12 72ea 7413 7c04 6a01 6a12 8301  j.j.r.t.|.j.j...
-000032e0: 7d0f 7414 7c0f 6407 8302 73e1 7c04 6a01  }.t.|.d...s.|.j.
-000032f0: 6a05 7c0f 6407 3c00 7c0f 7c03 7601 72ea  j.|.d.<.|.|.v.r.
-00003300: 7c03 a011 7c0f a101 0100 7106 7c02 7c03  |...|.....q.|.|.
-00003310: 6602 5300 290c 7a45 436f 6e76 6572 7473  f.S.).zEConverts
-00003320: 206f 6620 616c 6c20 7468 6520 626f 756e   of all the boun
-00003330: 6461 6374 696f 6e73 206f 6620 616e 2061  dactions of an a
-00003340: 6374 6f72 2074 6f20 6a73 6f6e 2066 6f72  ctor to json for
-00003350: 6d61 742e 0a20 2020 2020 2020 20a9 0172  mat..        ..r
-00003360: 6600 0000 2901 7295 0000 0072 b400 0000  f...).r....r....
-00003370: da0a 6a73 5f68 616e 646c 6572 4e29 01da  ..js_handlerN)..
-00003380: 0563 6f6d 626f 7290 0000 0072 2701 0000  .combor....r'...
-00003390: 4672 5600 0000 da0e 746f 6f6c 6261 7241  FrV.....toolbarA
-000033a0: 6374 696f 6e73 2917 da11 6765 745f 6c61  ctions)...get_la
-000033b0: 796f 7574 5f68 616e 6465 6c72 6d00 0000  yout_handelrm...
-000033c0: da0b 7769 6e64 6f77 5f74 7970 6572 0c00  ..window_typer..
-000033d0: 0000 da15 5552 4c5f 5041 5241 4d5f 4143  ....URL_PARAM_AC
-000033e0: 5449 4f4e 5f4e 414d 4572 4e00 0000 7278  TION_NAMErN...rx
-000033f0: 0000 0072 ac00 0000 7288 0000 0072 7200  ...r....r....rr.
-00003400: 0000 7299 0000 00da 1367 6574 5f74 6f6f  ..r......get_too
-00003410: 6c62 6172 5f61 6374 696f 6e73 7229 0000  lbar_actionsr)..
-00003420: 0072 b400 0000 7226 0100 0072 3000 0000  .r....r&...r0...
-00003430: da0b 636f 6d62 6f5f 6772 6f75 70da 0661  ..combo_group..a
-00003440: 7070 656e 64da 0668 6f74 6b65 79da 0476  ppend..hotkey..v
-00003450: 6172 7372 8300 0000 7231 0000 0072 e700  arsr....r1...r..
-00003460: 0000 2911 7240 0000 00da 0c61 6374 696f  ..).r@.....actio
-00003470: 6e73 5f6c 6973 7472 a700 0000 da07 686f  ns_listr......ho
-00003480: 746b 6579 7372 9000 0000 da02 6c68 da11  tkeysr......lh..
-00003490: 6163 7469 6f6e 5f64 6573 6372 6970 746f  action_descripto
-000034a0: 72da 0474 6261 73da 0963 6f6d 626f 5f6d  r..tbas..combo_m
-000034b0: 6170 7250 0000 00da 0374 6261 72b4 0000  aprP.....tbar...
-000034c0: 0072 2601 0000 722d 0100 0072 2701 0000  .r&...r-...r'...
-000034d0: 722f 0100 0072 3500 0000 7237 0000 0072  r/...r5...r7...r
-000034e0: 3700 0000 7238 0000 00da 0c61 6374 696f  7...r8.....actio
-000034f0: 6e73 326a 736f 6e06 0200 0073 6800 0000  ns2json....sh...
-00003500: 0404 0401 0802 0801 0c01 0e02 0401 1001  ................
-00003510: 0801 0401 0601 0602 0801 08ff 0e03 0801  ................
-00003520: 0c01 0801 0401 0801 1001 0802 0c02 0801  ................
-00003530: 0802 1001 0a02 0a01 0c01 0a02 0802 0c01  ................
-00003540: 0a01 0c01 0801 0a01 0280 0402 1001 0c01  ................
-00003550: 1401 0280 0802 0a02 0802 0c01 0a01 0c01  ................
-00003560: 0801 0a01 0280 0802 7a15 5265 6e64 6572  ........z.Render
-00003570: 6572 2e61 6374 696f 6e73 326a 736f 6e63  er.actions2jsonc
-00003580: 0200 0000 0000 0000 0000 0000 0500 0000  ................
-00003590: 0500 0000 4300 0000 7358 0000 0067 007d  ....C...sX...g.}
-000035a0: 0264 007d 037c 0144 005d 147d 047c 0464  .d.}.|.D.].}.|.d
-000035b0: 0119 0064 0075 0072 137c 0464 0219 007d  ...d.u.r.|.d...}
-000035c0: 0371 067c 02a0 0074 017c 0483 01a1 0101  .q.|...t.|......
-000035d0: 0071 0674 027c 0264 0364 0484 0064 058d  .q.t.|.d.d...d..
-000035e0: 027d 027c 02a0 0064 007c 0367 02a1 0101  .}.|...d.|.g....
-000035f0: 007c 0253 0029 064e 7201 0000 0072 2d00  .|.S.).Nr....r-.
-00003600: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00003610: 0000 0002 0000 0053 0000 0073 0800 0000  .......S...s....
-00003620: 7c00 6401 1900 5300 2902 4e72 0100 0000  |.d...S.).Nr....
-00003630: 7237 0000 0029 0172 3600 0000 7237 0000  r7...).r6...r7..
-00003640: 0072 3700 0000 7238 0000 00da 083c 6c61  .r7...r8.....<la
-00003650: 6d62 6461 3e52 0200 0073 0200 0000 0800  mbda>R...s......
-00003660: 7a2c 5265 6e64 6572 6572 2e64 6973 706c  z,Renderer.displ
-00003670: 6179 5f6d 6f64 6532 6a73 6f6e 2e3c 6c6f  ay_mode2json.<lo
-00003680: 6361 6c73 3e2e 3c6c 616d 6264 613e a901  cals>.<lambda>..
-00003690: 7234 0000 0029 0372 2e01 0000 7279 0000  r4...).r....ry..
-000036a0: 00da 0673 6f72 7465 6429 0572 4000 0000  ...sorted).r@...
-000036b0: da0c 6469 7370 6c61 795f 6d6f 6465 da03  ..display_mode..
-000036c0: 646d 73da 0364 6d64 7293 0000 0072 3700  dms..dmdr....r7.
-000036d0: 0000 7237 0000 0072 3800 0000 da11 6469  ..r7...r8.....di
-000036e0: 7370 6c61 795f 6d6f 6465 326a 736f 6e4a  splay_mode2jsonJ
-000036f0: 0200 0073 1200 0000 0401 0401 0801 0c01  ...s............
-00003700: 0a01 1002 1001 0e01 0401 7a1a 5265 6e64  ..........z.Rend
-00003710: 6572 6572 2e64 6973 706c 6179 5f6d 6f64  erer.display_mod
-00003720: 6532 6a73 6f6e 6302 0000 0000 0000 0000  e2jsonc.........
-00003730: 0000 0011 0000 0008 0000 0043 0000 0073  ...........C...s
-00003740: 2203 0000 7400 7c01 8301 7209 7401 7c01  "...t.|...r.t.|.
-00003750: 7402 8302 730b 4a00 8201 7c00 a003 7c01  t...s.J...|...|.
-00003760: 6a04 a101 5c02 7d02 7d03 7405 7c01 6a06  j...\.}.}.t.|.j.
-00003770: 7c02 7c01 a007 a100 7408 7c01 6a09 8301  |.|.....t.|.j...
-00003780: 7c01 a00a 740b 8300 a101 0c00 6401 8d05  |...t.......d...
-00003790: 7d04 740c 7c03 8301 7231 7c04 6a0d 7c03  }.t.|...r1|.j.|.
-000037a0: 6402 8d01 0100 7c01 a00e a100 7d05 7c05  d.....|.....}.|.
-000037b0: 6a0f 6400 7500 7243 7410 6a11 6a12 a013  j.d.u.rCt.j.j...
-000037c0: 6403 7c01 a102 0100 6e5d 7414 7c05 6404  d.|.....n]t.|.d.
-000037d0: 8302 7297 6700 7d06 6405 7d07 7c05 a015  ..r.g.}.d.}.|...
-000037e0: a100 7d08 7c08 4400 5d40 7d09 7c00 a016  ..}.|.D.]@}.|...
-000037f0: 7c09 a101 7d0a 7c0a 6a0d 7417 7c05 6a0f  |...}.|.j.t.|.j.
-00003800: 6a18 7c09 6a19 6a1a 6406 6407 8400 6408  j.|.j.j.d.d...d.
-00003810: 8d03 7c07 1700 6409 8d01 0100 741b 7c09  ..|...d.....t.|.
-00003820: 741c 8302 7284 741b 7c09 741d 8302 7384  t...r.t.|.t...s.
-00003830: 7c0a 6a0d 7c0a 640a 1900 640b 1700 640c  |.j.|.d...d...d.
-00003840: 8d01 0100 7c07 640b 3700 7d07 741b 7c09  ....|.d.7.}.t.|.
-00003850: 741e 8302 728d 7c07 640d 3700 7d07 7c06  t...r.|.d.7.}.|.
-00003860: a01f 7c0a a101 0100 7152 7c06 7c04 640e  ..|.....qR|.|.d.
-00003870: 3c00 7c04 a00d 7420 7c05 6a0f 640f 8302  <.|...t |.j.d...
-00003880: a101 0100 7c04 a00d 7420 7c01 6410 8302  ....|...t |.d...
-00003890: a101 0100 7414 7c01 6a21 6411 8302 72b4  ....t.|.j!d...r.
-000038a0: 7c04 6a0d 6412 6413 8d01 0100 7400 7c01  |.j.d.d.....t.|.
-000038b0: 6a21 8301 72c5 7401 7c01 6a21 7422 8302  j!..r.t.|.j!t"..
-000038c0: 72c5 7c04 6a0d 6412 6414 8d01 0100 7c01  r.|.j.d.d.....|.
-000038d0: 6a23 6400 7501 72d2 7c00 a024 7c01 6a23  j#d.u.r.|..$|.j#
-000038e0: a101 7c04 6415 3c00 7c01 6a25 6400 7501  ..|.d.<.|.j%d.u.
-000038f0: 72e7 7c01 6a25 a026 a100 7d0b 7c0b 6400  r.|.j%.&..}.|.d.
-00003900: 7501 72e7 7c04 6a0d 7c0b 6a27 6416 8d01  u.r.|.j.|.j'd...
-00003910: 0100 7c01 6a28 72f3 7c04 6a0d 7429 7c01  ..|.j(r.|.j.t)|.
-00003920: 6a28 8301 6417 8d01 0100 742a 7c01 6418  j(..d.....t*|.d.
-00003930: 6400 8303 7d0c 7c0c 6400 7501 9001 7205  d...}.|.d.u...r.
-00003940: 7c04 6a0d 7c0c 6a27 6419 8d01 0100 742a  |.j.|.j'd.....t*
-00003950: 7c01 641a 6400 8303 7d0d 7c0d 6400 7501  |.d.d...}.|.d.u.
-00003960: 9001 7217 7c04 6a0d 7c0d 6a27 641b 8d01  ..r.|.j.|.j'd...
-00003970: 0100 742a 7c01 6a21 641c 6900 8303 7d0e  ..t*|.j!d.i...}.
-00003980: 7c0e 9001 722e 7c04 6a0d 641d 641e 8400  |...r.|.j.d.d...
-00003990: 7c0e a02b a100 4400 8301 641f 8d01 0100  |..+..D...d.....
-000039a0: 7410 6a11 a02c 6420 a101 9001 7251 742a  t.j..,d ....rQt*
-000039b0: 7c01 6421 6400 8303 6400 7501 9001 7251  |.d!d...d.u...rQ
-000039c0: 7414 7c01 6a21 6422 8302 9001 7251 7c04  t.|.j!d"....rQ|.
-000039d0: 6a0d 742d 6a2e a02f 7c01 6a21 a101 6a30  j.t-j../|.j!..j0
-000039e0: 6423 8d01 0100 6424 4400 5d17 7d0f 742a  d#....d$D.].}.t*
-000039f0: 7c01 7c0f 6400 8303 7d10 7c10 6400 7501  |.|.d...}.|.d.u.
-00003a00: 9001 7269 7c04 a00d 7c0f 7c10 6a31 6a32  ..ri|...|.|.j1j2
-00003a10: 6901 a101 0100 9001 7153 7c01 6a33 6400  i.......qS|.j3d.
-00003a20: 7501 9001 728f 7c04 6a0d 7c01 6a33 6a27  u...r.|.j.|.j3j'
-00003a30: 6425 6426 8400 7c01 6a33 6a34 6a35 4400  d%d&..|.j3j4j5D.
-00003a40: 8301 6427 8d02 0100 7414 7c01 6428 8302  ..d'....t.|.d(..
-00003a50: 9001 728f 7c04 6a0d 7c01 6a36 6429 8d01  ..r.|.j.|.j6d)..
-00003a60: 0100 7c04 5300 292a 4e29 05da 0269 6472  ..|.S.)*N)...idr
-00003a70: 3101 0000 7296 0000 00da 0573 6c61 7665  1...r......slave
-00003a80: da08 6564 6974 6162 6c65 2901 7232 0100  ..editable).r2..
-00003a90: 007a 0f25 7320 6861 7320 6e6f 2073 746f  .z.%s has no sto
-00003aa0: 7265 da0b 6765 745f 636f 6c75 6d6e 7372  re..get_columnsr
-00003ab0: 0100 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00003ac0: 0001 0000 0001 0000 0053 0000 0073 0600  .........S...s..
-00003ad0: 0000 7c00 6a00 5300 723b 0000 00a9 0172  ..|.j.S.r;.....r
-00003ae0: 5300 0000 a901 728d 0000 0072 3700 0000  S.....r....r7...
-00003af0: 7237 0000 0072 3800 0000 7239 0100 006f  r7...r8...r9...o
-00003b00: 0200 0073 0200 0000 0600 7a25 5265 6e64  ...s......z%Rend
-00003b10: 6572 6572 2e61 6374 6f72 326a 736f 6e2e  erer.actor2json.
-00003b20: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00003b30: 3e72 3a01 0000 2901 da0c 6669 656c 6473  >r:...)...fields
-00003b40: 5f69 6e64 6578 7246 0100 0072 2d00 0000  _indexrF...r-...
-00003b50: 2901 da13 6669 656c 6473 5f69 6e64 6578  )...fields_index
-00003b60: 5f68 6964 6465 6ee9 0200 0000 da03 636f  _hidden.......co
-00003b70: 6cda 0870 6b5f 696e 6465 787a d070 7265  l..pk_indexz.pre
-00003b80: 7669 6577 5f6c 696d 6974 2075 7365 5f64  view_limit use_d
-00003b90: 6574 6169 6c5f 7061 7261 6d5f 7061 6e65  etail_param_pane
-00003ba0: 6c20 7573 655f 6465 7461 696c 5f70 6172  l use_detail_par
-00003bb0: 616d 735f 7661 6c75 6520 6869 6465 5f6e  ams_value hide_n
-00003bc0: 6176 6967 6174 6f72 2075 7365 5f64 6574  avigator use_det
-00003bd0: 6169 6c5f 7061 7261 6d73 5f76 616c 7565  ail_params_value
-00003be0: 2072 6561 6374 5f72 6573 706f 6e73 6976   react_responsiv
-00003bf0: 6520 6d61 785f 7265 6e64 6572 5f64 6570  e max_render_dep
-00003c00: 7468 2073 696d 706c 655f 736c 6176 6567  th simple_slaveg
-00003c10: 7269 645f 6865 6164 6572 2070 6167 696e  rid_header pagin
-00003c20: 6174 6f72 5f74 656d 706c 6174 6520 6869  ator_template hi
-00003c30: 6465 5f74 6f70 5f74 6f6f 6c62 6172 2068  de_top_toolbar h
-00003c40: 6964 655f 6966 5f65 6d70 7479 20da 0466  ide_if_empty ..f
-00003c50: 696c 6554 2901 da0d 636f 6e74 6169 6e5f  ileT)...contain_
-00003c60: 6d65 6469 6129 01da 0965 6469 745f 7361  media)...edit_sa
-00003c70: 6665 723c 0100 0072 2501 0000 2901 da0d  fer<...r%...)...
-00003c80: 6163 7469 7665 5f66 6965 6c64 73da 0b63  active_fields..c
-00003c90: 6172 645f 6c61 796f 7574 2901 724f 0100  ard_layout).rO..
-00003ca0: 00da 0b6c 6973 745f 6c61 796f 7574 2901  ...list_layout).
-00003cb0: 7250 0100 00da 0e5f 6368 6f6f 7365 7273  rP....._choosers
-00003cc0: 5f64 6963 7463 0100 0000 0000 0000 0000  _dictc..........
-00003cd0: 0000 0300 0000 0500 0000 5300 0000 7322  ..........S...s"
-00003ce0: 0000 0069 007c 005d 0d5c 027d 017d 027c  ...i.|.].\.}.}.|
-00003cf0: 0164 0064 0184 007c 026a 0044 0083 0193  .d.d...|.j.D....
-00003d00: 0271 0253 0029 0263 0100 0000 0000 0000  .q.S.).c........
-00003d10: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
-00003d20: f312 0000 0067 007c 005d 057d 017c 016a  .....g.|.].}.|.j
-00003d30: 0091 0271 0253 0072 3700 0000 7244 0100  ...q.S.r7...rD..
-00003d40: 0029 0272 4700 0000 da02 6366 7237 0000  .).rG.....cfr7..
-00003d50: 0072 3700 0000 7238 0000 0072 4900 0000  .r7...r8...rI...
-00003d60: a802 0000 f302 0000 0012 007a 3252 656e  ...........z2Ren
-00003d70: 6465 7265 722e 6163 746f 7232 6a73 6f6e  derer.actor2json
-00003d80: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00003d90: 6f6d 703e 2e3c 6c69 7374 636f 6d70 3e29  omp>.<listcomp>)
-00003da0: 01da 0e63 6f6e 7465 7874 5f66 6965 6c64  ...context_field
-00003db0: 7329 0372 4700 0000 da02 666e 7248 0000  s).rG.....fnrH..
-00003dc0: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
-00003dd0: 724d 0000 00a8 0200 0073 0600 0000 0600  rM.......s......
-00003de0: 0601 16ff 7a27 5265 6e64 6572 6572 2e61  ....z'Renderer.a
-00003df0: 6374 6f72 326a 736f 6e2e 3c6c 6f63 616c  ctor2json.<local
-00003e00: 733e 2e3c 6469 6374 636f 6d70 3e29 01da  s>.<dictcomp>)..
-00003e10: 0c63 686f 6f73 6572 5f64 6963 74da 0c63  .chooser_dict..c
-00003e20: 6f6e 7465 6e74 7479 7065 73da 056d 6f64  ontenttypes..mod
-00003e30: 656c da05 5f6d 6574 6129 01da 0c63 6f6e  el.._meta)...con
-00003e40: 7465 6e74 5f74 7970 6529 03da 0d64 6574  tent_type)...det
-00003e50: 6169 6c5f 6163 7469 6f6e da0d 696e 7365  ail_action..inse
-00003e60: 7274 5f61 6374 696f 6eda 0e64 6566 6175  rt_action..defau
-00003e70: 6c74 5f61 6374 696f 6e63 0100 0000 0000  lt_actionc......
-00003e80: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
-00003e90: 0000 7252 0100 0072 3700 0000 7244 0100  ..rR...r7...rD..
-00003ea0: 0029 0272 4700 0000 728d 0000 0072 3700  .).rG...r....r7.
-00003eb0: 0000 7237 0000 0072 3800 0000 7249 0000  ..r7...r8...rI..
-00003ec0: 00b8 0200 0072 5401 0000 7a27 5265 6e64  .....rT...z'Rend
-00003ed0: 6572 6572 2e61 6374 6f72 326a 736f 6e2e  erer.actor2json.
-00003ee0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00003ef0: 6d70 3e29 02da 0d70 6172 616d 735f 6c61  mp>)...params_la
-00003f00: 796f 7574 da0d 7061 7261 6d73 5f66 6965  yout..params_fie
-00003f10: 6c64 73da 1070 6172 616d 735f 7061 6e65  lds..params_pane
-00003f20: 6c5f 706f 7329 0172 6101 0000 2937 722c  l_pos).ra...)7r,
-00003f30: 0000 0072 b600 0000 721b 0000 0072 3801  ...r....r....r8.
-00003f40: 0000 da0d 5f61 6374 696f 6e73 5f6c 6973  ...._actions_lis
-00003f50: 7472 7200 0000 72f1 0000 00da 0f67 6574  trr...r......get
-00003f60: 5f61 6374 6f72 5f6c 6162 656c da04 626f  _actor_label..bo
-00003f70: 6f6c da06 6d61 7374 6572 da0c 6869 6465  ol..master..hide
-00003f80: 5f65 6469 7469 6e67 7229 0000 0072 d300  _editingr)...r..
-00003f90: 0000 7278 0000 00da 0a67 6574 5f68 616e  ..rx.....get_han
-00003fa0: 646c 65da 0573 746f 7265 7204 0000 0072  dle..storer....r
-00003fb0: 7000 0000 da06 6c6f 6767 6572 da07 7761  p.....logger..wa
-00003fc0: 726e 696e 6772 8300 0000 7243 0100 0072  rningr....rC...r
-00003fd0: ab00 0000 7239 0000 00da 0b6c 6973 745f  ....r9.....list_
-00003fe0: 6669 656c 6473 72b8 0000 0072 5300 0000  fieldsr....rS...
-00003ff0: 72a1 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-00004000: 2200 0000 722e 0100 0072 2800 0000 7259  "...r....r(...rY
-00004010: 0100 0072 2b00 0000 723c 0100 0072 3f01  ...r+...r<...r?.
-00004020: 0000 725c 0100 00da 1167 6574 5f77 696e  ..r\.....get_win
-00004030: 646f 775f 6c61 796f 7574 7288 0000 0072  dow_layoutr....r
-00004040: 4e01 0000 7279 0000 0072 0301 0000 7269  N...ry...r....ri
-00004050: 0000 0072 7700 0000 720e 0000 00da 076f  ...rw...r......o
-00004060: 626a 6563 7473 da0d 6765 745f 666f 725f  bjects..get_for_
-00004070: 6d6f 6465 6c72 da00 0000 726d 0000 0072  modelr....rm...r
-00004080: 4e00 0000 725f 0100 00da 0c70 6172 616d  N...r_.....param
-00004090: 735f 7374 6f72 65da 0c70 6172 616d 5f66  s_store..param_f
-000040a0: 6965 6c64 7372 6101 0000 2911 7240 0000  ieldsra...).r@..
-000040b0: 0072 a600 0000 da02 616c da02 686b 72a7  .r......al..hkr.
-000040c0: 0000 00da 0261 68da 0763 6f6c 756d 6e73  .....ah..columns
-000040d0: da09 696e 6465 785f 6d6f 64da 0963 6f6c  ..index_mod..col
-000040e0: 5f65 6c65 6d73 7249 0100 0072 0d01 0000  _elemsrI...r....
-000040f0: da02 776c 724f 0100 0072 5001 0000 7257  ..wlrO...rP...rW
-00004100: 0100 0072 b900 0000 7290 0000 0072 3700  ...r....r....r7.
-00004110: 0000 7237 0000 0072 3800 0000 da0a 6163  ..r7...r8.....ac
-00004120: 746f 7232 6a73 6f6e 5602 0000 7392 0000  tor2jsonV...s...
-00004130: 0016 0110 0106 0102 0106 0108 010c 0106  ................
-00004140: fc08 070c 0108 020a 0112 010a 0304 0104  ................
-00004150: 0108 0108 010a 0112 0106 0104 ff02 0108  ................
-00004160: ff14 0214 0308 010a 0108 010c 0108 0112  ................
-00004170: 0510 010c 0d0c 0116 020c 010a 0210 010a  ................
-00004180: 020a 0108 010e 0106 0212 010c 020a 010e  ................
-00004190: 010c 020a 010e 020e 0306 010a 0106 010a  ................
-000041a0: ff26 0302 0106 ff18 0308 010c 010a 0112  .&..............
-000041b0: 0104 800c 0204 0206 0112 0106 fe0c 040e  ................
-000041c0: 0104 017a 1352 656e 6465 7265 722e 6163  ...z.Renderer.ac
-000041d0: 746f 7232 6a73 6f6e 6302 0000 0000 0000  tor2jsonc.......
-000041e0: 0000 0000 0004 0000 0006 0000 0003 0000  ................
-000041f0: 0073 6400 0000 6401 8801 5f00 8801 6a01  .sd...d..._...j.
-00004200: 4400 5d22 8900 8800 6a02 6400 7501 720e  D.]"....j.d.u.r.
-00004210: 7106 7403 6a04 6a05 8801 a006 8800 6a07  q.t.j.j.......j.
-00004220: a101 8e00 7d02 8700 8701 6602 6402 6403  ....}.....f.d.d.
-00004230: 8408 7d03 7408 6a09 6a0a a00b 7c02 7c03  ..}.t.j.j...|.|.
-00004240: 7c01 a103 0100 7106 6404 8801 5f00 740c  |.....q.d..._.t.
-00004250: 8300 a00d 7c01 a101 5300 2905 4e54 6301  ....|...S.).NTc.
-00004260: 0000 0000 0000 0000 0000 0001 0000 0006  ................
-00004270: 0000 0013 0000 0073 1800 0000 7c00 a000  .......s....|...
-00004280: 7401 8801 a002 8800 a101 8301 a101 0100  t...............
-00004290: 6400 5300 723b 0000 0029 0372 8c00 0000  d.S.r;...).r....
-000042a0: 7226 0000 0072 7801 0000 7245 0100 00a9  r&...rx...rE....
-000042b0: 0272 9900 0000 7240 0000 0072 3700 0000  .r....r@...r7...
-000042c0: 7238 0000 0072 8c00 0000 c702 0000 7302  r8...r........s.
-000042d0: 0000 0018 017a 2652 656e 6465 7265 722e  .....z&Renderer.
-000042e0: 6275 696c 645f 6a73 5f63 6163 6865 2e3c  build_js_cache.<
-000042f0: 6c6f 6361 6c73 3e2e 7772 6974 6546 290e  locals>.writeF).
-00004300: 726f 0000 0072 6b00 0000 da0f 6765 745f  ro...rk.....get_
-00004310: 6861 6e64 6c65 5f6e 616d 6572 7e00 0000  handle_namer~...
-00004320: da04 7061 7468 da04 6a6f 696e 7224 0100  ..path..joinr$..
-00004330: 0072 f100 0000 7204 0000 0072 7000 0000  .r....r....rp...
-00004340: 7223 0000 00da 0f6d 616b 655f 6361 6368  r#.....make_cach
-00004350: 655f 6669 6c65 723c 0000 00da 0e62 7569  e_filer<.....bui
-00004360: 6c64 5f6a 735f 6361 6368 6529 0472 4000  ld_js_cache).r@.
-00004370: 0000 da05 666f 7263 6572 5601 0000 728c  ....forcerV...r.
-00004380: 0000 0072 4200 0000 7279 0100 0072 3800  ...rB...ry...r8.
-00004390: 0000 727e 0100 00be 0200 0073 1200 0000  ..r~.......s....
-000043a0: 0602 0a02 0a01 0201 1401 0e02 1403 0602  ................
-000043b0: 0c01 7a17 5265 6e64 6572 6572 2e62 7569  ..z.Renderer.bui
-000043c0: 6c64 5f6a 735f 6361 6368 6572 3b00 0000  ld_js_cacher;...
-000043d0: 2920 72b5 0000 00da 0a5f 5f6d 6f64 756c  ) r......__modul
-000043e0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000043f0: 5fda 075f 5f64 6f63 5f5f da0e 6973 5f69  _..__doc__..is_i
-00004400: 6e74 6572 6163 7469 7665 da08 6361 6e5f  nteractive..can_
-00004410: 6175 7468 721f 0100 0072 2301 0000 da18  authr....r#.....
-00004420: 7375 7070 6f72 745f 6461 7368 626f 6172  support_dashboar
-00004430: 645f 6c61 796f 7574 723d 0000 0072 9400  d_layoutr=...r..
-00004440: 0000 724f 0000 0072 8700 0000 72ab 0000  ..rO...r....r...
-00004450: 0072 ba00 0000 72d0 0000 0072 dd00 0000  .r....r....r....
-00004460: 72e4 0000 0072 a500 0000 72e0 0000 0072  r....r....r....r
-00004470: 3f00 0000 72ff 0000 0072 0001 0000 7201  ?...r....r....r.
-00004480: 0100 0072 1501 0000 721b 0100 0072 2401  ...r....r....r$.
-00004490: 0000 7238 0100 0072 3f01 0000 7278 0100  ..r8...r?...rx..
-000044a0: 0072 7e01 0000 da0d 5f5f 636c 6173 7363  .r~.....__classc
-000044b0: 656c 6c5f 5f72 3700 0000 7237 0000 0072  ell__r7...r7...r
-000044c0: 4200 0000 7238 0000 0072 3a00 0000 3b00  B...r8...r:...;.
-000044d0: 0000 733c 0000 0008 0004 0104 0304 0104  ..s<............
-000044e0: 0204 0104 010c 0208 0408 5508 1d08 0808  ..........U.....
-000044f0: 2008 030a 1802 120a ff08 1508 0e08 2108   .............!.
-00004500: 4e08 0e08 0a08 2a08 0908 0f08 0a08 4408  N.....*.......D.
-00004510: 0c14 6872 3a00 0000 723b 0000 0029 4872  ..hr:...r;...)Hr
-00004520: 7e00 0000 da07 7061 7468 6c69 6272 0200  ~.....pathlibr..
-00004530: 0000 da04 6874 6d6c 7203 0000 00da 0b64  ....htmlr......d
-00004540: 6a61 6e67 6f2e 636f 6e66 7204 0000 00da  jango.confr.....
-00004550: 0964 6a61 6e67 6f2e 6462 7205 0000 00da  .django.dbr.....
-00004560: 1164 6a61 6e67 6f2e 7574 696c 732e 7465  .django.utils.te
-00004570: 7874 7206 0000 00da 0c64 6a61 6e67 6f2e  xtr......django.
-00004580: 7574 696c 7372 0700 0000 da12 6c69 6e6f  utilsr......lino
-00004590: 2e63 6f72 652e 7265 6e64 6572 6572 7208  .core.rendererr.
-000045a0: 0000 0072 0900 0000 da0f 6c69 6e6f 2e63  ...r......lino.c
-000045b0: 6f72 652e 6d65 6e75 7372 0a00 0000 720b  ore.menusr....r.
-000045c0: 0000 00da 096c 696e 6f2e 636f 7265 720c  .....lino.corer.
-000045d0: 0000 0072 0d00 0000 da0e 6c69 6e6f 2e63  ...r......lino.c
-000045e0: 6f72 652e 6766 6b73 720e 0000 00da 1e6c  ore.gfksr......l
-000045f0: 696e 6f2e 6d6f 646c 6962 2e65 7874 6a73  ino.modlib.extjs
-00004600: 2e65 7874 5f72 656e 6465 7265 7272 0f00  .ext_rendererr..
-00004610: 0000 da11 6c69 6e6f 2e63 6f72 652e 6163  ....lino.core.ac
-00004620: 7469 6f6e 7372 1000 0000 7211 0000 0072  tionsr....r....r
-00004630: 1200 0000 7213 0000 0072 1400 0000 7215  ....r....r....r.
-00004640: 0000 0072 1600 0000 7217 0000 00da 156c  ...r....r......l
-00004650: 696e 6f2e 636f 7265 2e62 6f75 6e64 6163  ino.core.boundac
-00004660: 7469 6f6e 7218 0000 00da 156c 696e 6f2e  tionr......lino.
-00004670: 636f 7265 2e63 686f 6963 656c 6973 7473  core.choicelists
-00004680: 7219 0000 00da 1e6c 696e 6f2e 6d6f 646c  r......lino.modl
-00004690: 6962 2e73 7973 7465 6d2e 6368 6f69 6365  ib.system.choice
-000046a0: 6c69 7374 7372 1a00 0000 da10 6c69 6e6f  listsr......lino
-000046b0: 2e63 6f72 652e 6163 746f 7273 721b 0000  .core.actorsr...
-000046c0: 00da 116c 696e 6f2e 636f 7265 2e6c 6179  ...lino.core.lay
-000046d0: 6f75 7473 721c 0000 0072 1d00 0000 da0f  outsr....r......
-000046e0: 6c69 6e6f 2e63 6f72 652e 656c 656d 7372  lino.core.elemsr
-000046f0: 1e00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
-00004700: 0000 0072 2200 0000 7223 0000 00da 0a65  ...r"...r#.....e
-00004710: 7467 656e 2e68 746d 6c72 2400 0000 da0a  tgen.htmlr$.....
-00004720: 6c69 6e6f 2e75 7469 6c73 7225 0000 00da  lino.utilsr%....
-00004730: 106c 696e 6f2e 7574 696c 732e 6a73 6765  .lino.utils.jsge
-00004740: 6e72 2600 0000 7227 0000 0072 2800 0000  nr&...r'...r(...
-00004750: da17 6c69 6e6f 2e6d 6f64 6c69 622e 7573  ..lino.modlib.us
-00004760: 6572 732e 7574 696c 7372 2900 0000 722a  ers.utilsr)...r*
-00004770: 0000 00da 196c 696e 6f2e 6d6f 646c 6962  .....lino.modlib
-00004780: 2e73 7973 7465 6d2e 6d69 7869 6e73 722b  .system.mixinsr+
-00004790: 0000 00da 0769 6e73 7065 6374 722c 0000  .....inspectr,..
-000047a0: 00da 0569 636f 6e73 722e 0000 0072 3900  ...iconsr....r9.
-000047b0: 0000 723a 0000 0072 3700 0000 7237 0000  ..r:...r7...r7..
-000047c0: 0072 3700 0000 7238 0000 00da 083c 6d6f  .r7...r8.....<mo
-000047d0: 6475 6c65 3e01 0000 0073 3c00 0000 0804  dule>....s<.....
-000047e0: 0c01 0c01 0c01 0c01 0c01 0c01 1002 1002  ................
-000047f0: 0c01 0c01 0c01 0c01 2802 0c03 0c01 0c01  ........(.......
-00004800: 0c01 1001 1c01 0c02 0c02 0c02 1401 1002  ................
-00004810: 0c01 0c02 0c02 0a03 140d                 ..........
+00000930: 640a 8d01 0100 7a12 741d a01e 741f 7409  d.....z.t...t.t.
+00000940: 6a20 8301 640b 1b00 640c 1b00 a101 6a21  j ..d...d.....j!
+00000950: 7c07 7422 6a23 3c00 5700 6e09 0400 7424  |.t"j#<.W.n...t$
+00000960: 7988 0100 0100 0100 5900 6e01 7700 7425  y.......Y.n.w.t%
+00000970: 7409 6a0a 640d 8302 7297 7c07 6a16 7409  t.j.d...r.|.j.t.
+00000980: 6a0a 6a26 640e 8d01 0100 7409 6a0a 6a27  j.j&d.....t.j.j'
+00000990: 6405 6b02 72a4 7c07 6a16 6403 640f 8d01  d.k.r.|.j.d.d...
+000009a0: 0100 6e0e 7425 7c06 6a28 6410 8302 72b2  ..n.t%|.j(d...r.
+000009b0: 7c07 6a16 7c06 6a28 6a29 6411 8d01 0100  |.j.|.j(j)d.....
+000009c0: 7409 6a0a a015 6412 a101 72c4 7c07 6a16  t.j...d...r.|.j.
+000009d0: 7c06 6a2a 6a2b 6fc1 7409 6a0a 6a2c 6413  |.j*j+o.t.j.j,d.
+000009e0: 8d01 0100 6900 7d08 8800 6a2d 4400 5d2f  ....i.}...j-D.]/
+000009f0: 7d09 8800 a02e 7c09 a101 7c08 7c09 6a2f  }.....|...|.|.j/
+00000a00: 3c00 7425 7c09 6414 8302 72f8 6415 7c09  <.t%|.d...r.d.|.
+00000a10: 6a2f 7600 72f8 7430 7c02 6416 1900 8301  j/v.r.t0|.d.....
+00000a20: 4400 5d14 5c02 7d0a 7d0b 7c0b 6417 1900  D.].\.}.}.|.d...
+00000a30: 7c09 6a31 6b02 72f7 7c09 6a2f 7c02 6416  |.j1k.r.|.j/|.d.
+00000a40: 1900 7c0a 1900 6418 3c00 71e3 71c9 8800  ..|...d.<.q.q...
+00000a50: 6a32 4400 5d0a 7d09 8800 a02e 7c09 a101  j2D.].}.....|...
+00000a60: 7c08 7c09 6a2f 3c00 71fc 8800 6a33 4400  |.|.j/<.q...j3D.
+00000a70: 5d0b 7d09 8800 a02e 7c09 a101 7c08 7c09  ].}.....|...|.|.
+00000a80: 6a2f 3c00 9001 710a 8800 6a34 4400 5d0b  j/<...q...j4D.].
+00000a90: 7d09 8800 a02e 7c09 a101 7c08 7c09 6a2f  }.....|...|.|.j/
+00000aa0: 3c00 9001 7119 7c07 6a16 7c08 7c02 6419  <...q.|.j.|.|.d.
+00000ab0: 8d02 0100 7c01 a035 7436 7c07 8301 a101  ....|..5t6|.....
+00000ac0: 0100 641a 8800 5f08 641b 5300 291c 7a86  ..d..._.d.S.).z.
+00000ad0: 0a20 2020 2020 2020 2043 7265 6174 6573  .        Creates
+00000ae0: 2077 6861 7420 6973 206b 6e6f 776e 2061   what is known a
+00000af0: 7320 7769 6e64 6f77 2e41 7070 2e73 7461  s window.App.sta
+00000b00: 7465 2e73 6974 655f 6461 7461 2069 6e20  te.site_data in 
+00000b10: 5265 6163 7420 636f 6465 2e0a 0a20 2020  React code...   
+00000b20: 2020 2020 203a 7061 7261 6d20 663a 2046       :param f: F
+00000b30: 696c 6520 6f62 6a65 6374 0a20 2020 2020  ile object.     
+00000b40: 2020 203a 7265 7475 726e 3a20 310a 2020     :return: 1.  
+00000b50: 2020 2020 2020 6301 0000 0000 0000 0000        c.........
+00000b60: 0000 0003 0000 0006 0000 0053 0000 0073  ...........S...s
+00000b70: 2400 0000 6900 7c00 5d0e 5c02 7d01 7d02  $...i.|.].\.}.}.
+00000b80: 7c01 6400 6401 8400 7c02 a000 a100 4400  |.d.d...|.....D.
+00000b90: 8301 9302 7102 5300 2902 6301 0000 0000  ....q.S.).c.....
+00000ba0: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
+00000bb0: 0000 0073 2400 0000 6700 7c00 5d0e 7d01  ...s$...g.|.].}.
+00000bc0: 7c01 6400 1900 6a00 7401 7c01 6401 1900  |.d...j.t.|.d...
+00000bd0: 8301 6402 9c02 9102 7102 5300 2903 7201  ..d.....q.S.).r.
+00000be0: 0000 0072 2d00 0000 2902 da05 7661 6c75  ...r-...)...valu
+00000bf0: 65da 0474 6578 7429 0272 4400 0000 da03  e..text).rD.....
+00000c00: 7374 7229 02da 022e 30da 0163 7237 0000  str)....0..cr7..
+00000c10: 0072 3700 0000 7238 0000 00da 0a3c 6c69  .r7...r8.....<li
+00000c20: 7374 636f 6d70 3e53 0000 0073 0200 0000  stcomp>S...s....
+00000c30: 2400 7a35 5265 6e64 6572 6572 2e77 7269  $.z5Renderer.wri
+00000c40: 7465 5f6c 696e 6f5f 6a73 2e3c 6c6f 6361  te_lino_js.<loca
+00000c50: 6c73 3e2e 3c64 6963 7463 6f6d 703e 2e3c  ls>.<dictcomp>.<
+00000c60: 6c69 7374 636f 6d70 3e29 01da 0b67 6574  listcomp>)...get
+00000c70: 5f63 686f 6963 6573 2903 7247 0000 00da  _choices).rG....
+00000c80: 0249 44da 0263 6c72 3700 0000 7237 0000  .ID..clr7...r7..
+00000c90: 0072 3800 0000 da0a 3c64 6963 7463 6f6d  .r8.....<dictcom
+00000ca0: 703e 5100 0000 7308 0000 0006 0006 0312  p>Q...s.........
+00000cb0: ff06 fe7a 2a52 656e 6465 7265 722e 7772  ...z*Renderer.wr
+00000cc0: 6974 655f 6c69 6e6f 5f6a 732e 3c6c 6f63  ite_lino_js.<loc
+00000cd0: 616c 733e 2e3c 6469 6374 636f 6d70 3e54  als>.<dictcomp>T
+00000ce0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000cf0: 0006 0000 0013 0000 0073 1a00 0000 6900  .........s....i.
+00000d00: 7c00 5d09 7d01 7c01 6a00 8800 a001 7c01  |.].}.|.j.....|.
+00000d10: a101 9302 7102 5300 7237 0000 0029 02da  ....q.S.r7...)..
+00000d20: 0b61 6374 696f 6e5f 6e61 6d65 da0b 6163  .action_name..ac
+00000d30: 7469 6f6e 326a 736f 6e29 0272 4700 0000  tion2json).rG...
+00000d40: da01 61a9 0172 4000 0000 7237 0000 0072  ..a..r@...r7...r
+00000d50: 3800 0000 724d 0000 0060 0000 0073 0200  8...rM...`...s..
+00000d60: 0000 1a00 4e63 0100 0000 0000 0000 0000  ....Nc..........
+00000d70: 0000 0200 0000 0400 0000 5300 0000 7316  ..........S...s.
+00000d80: 0000 0069 007c 005d 077d 017c 016a 007c  ...i.|.].}.|.j.|
+00000d90: 016a 0193 0271 0253 0072 3700 0000 2902  .j...q.S.r7...).
+00000da0: da0b 646a 616e 676f 5f63 6f64 65da 046e  ..django_code..n
+00000db0: 616d 6529 0272 4700 0000 da04 6c61 6e67  ame).rG.....lang
+00000dc0: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
+00000dd0: 4d00 0000 6600 0000 7302 0000 0016 0029  M...f...s......)
+00000de0: 06da 0761 6374 696f 6e73 da04 6d65 6e75  ...actions..menu
+00000df0: da15 7573 655f 6461 7368 626f 6172 645f  ..use_dashboard_
+00000e00: 6c61 796f 7574 73da 0a73 6974 655f 7469  layouts..site_ti
+00000e10: 746c 65da 1065 6469 7469 6e67 5f66 726f  tle..editing_fro
+00000e20: 6e74 656e 64da 096c 616e 6775 6167 6573  ntend..languages
+00000e30: da04 6d65 6d6f 2901 da0a 7375 6767 6573  ..memo)...sugges
+00000e40: 746f 7273 2901 da0f 7265 7669 7369 6f6e  tors)...revision
+00000e50: 5f6e 756d 6265 72da 0572 6561 6374 7a07  _number..reactz.
+00000e60: 6d61 696e 2e6a 73da 0a74 6865 6d65 5f6e  main.js..theme_n
+00000e70: 616d 6529 0172 5f00 0000 2901 da0d 6e6f  ame).r_...)...no
+00000e80: 5f75 7365 725f 6d6f 6465 6cda 1961 6c6c  _user_model..all
+00000e90: 6f77 5f6f 6e6c 696e 655f 7265 6769 7374  ow_online_regist
+00000ea0: 7261 7469 6f6e 2901 7261 0000 00da 066e  ration).ra.....n
+00000eb0: 6f74 6966 7929 01da 0c75 7365 5f70 7573  otify)...use_pus
+00000ec0: 685f 6170 69da 0b63 686f 6963 655f 6e61  h_api..choice_na
+00000ed0: 6d65 7a10 7379 7374 656d 2e44 6173 6862  mez.system.Dashb
+00000ee0: 6f61 7264 7a17 7379 7374 656d 2e44 6173  oardz.system.Das
+00000ef0: 6862 6f61 7264 4c61 796f 7574 7372 4400  hboardLayoutsrD.
+00000f00: 0000 da0d 7769 6e64 6f77 5f6c 6179 6f75  ....window_layou
+00000f10: 7429 02da 0b66 6f72 6d5f 7061 6e65 6c73  t)...form_panels
+00000f20: 720d 0000 0046 722d 0000 0029 3772 2300  r....Fr-...)7r#.
+00000f30: 0000 da0b 4348 4f49 4345 4c49 5354 53da  ....CHOICELISTS.
+00000f40: 0569 7465 6d73 da03 7365 74da 0b61 6374  .items..set..act
+00000f50: 6f72 735f 6c69 7374 da0b 6765 745f 6163  ors_list..get_ac
+00000f60: 7469 6f6e 73da 0661 6374 696f 6eda 0361  tions..action..a
+00000f70: 6464 da11 7365 7269 616c 6973 655f 6a73  dd..serialise_js
+00000f80: 5f63 6f64 6572 0400 0000 da04 5349 5445  _coder......SITE
+00000f90: da07 706c 7567 696e 73da 0464 6963 74da  ..plugins..dict.
+00000fa0: 0d67 6574 5f73 6974 655f 6d65 6e75 7229  .get_site_menur)
+00000fb0: 0000 00da 0673 7973 7465 6d72 5700 0000  .....systemrW...
+00000fc0: da05 7469 746c 6572 4100 0000 da0a 7572  ..titlerA.....ur
+00000fd0: 6c5f 7072 6566 6978 725a 0000 00da 0c69  l_prefixrZ.....i
+00000fe0: 735f 696e 7374 616c 6c65 64da 0675 7064  s_installed..upd
+00000ff0: 6174 65da 046c 6973 7472 5b00 0000 da06  ate..listr[.....
+00001000: 7061 7273 6572 da0a 7375 6767 6573 7465  parser..suggeste
+00001010: 7273 da04 6b65 7973 da0a 636f 6465 5f6d  rs..keys..code_m
+00001020: 7469 6d65 da02 6f73 da04 7374 6174 7202  time..os..statr.
+00001030: 0000 00da 0b53 5441 5449 435f 524f 4f54  .....STATIC_ROOT
+00001040: da08 7374 5f6d 7469 6d65 720c 0000 00da  ..st_mtimer.....
+00001050: 1b55 524c 5f50 4152 414d 5f4d 4149 4e5f  .URL_PARAM_MAIN_
+00001060: 4a53 5f54 494d 4553 5441 4d50 da11 4669  JS_TIMESTAMP..Fi
+00001070: 6c65 4e6f 7446 6f75 6e64 4572 726f 72da  leNotFoundError.
+00001080: 0768 6173 6174 7472 725f 0000 00da 0a75  .hasattrr_.....u
+00001090: 7365 725f 6d6f 6465 6cda 0575 7365 7273  ser_model..users
+000010a0: 7261 0000 0072 6200 0000 7263 0000 00da  ra...rb...rc....
+000010b0: 0975 7365 5f6c 696e 6f64 7266 0000 00da  .use_linodrf....
+000010c0: 0a70 616e 656c 326a 736f 6eda 0f5f 666f  .panel2json.._fo
+000010d0: 726d 7061 6e65 6c5f 6e61 6d65 7231 0000  rmpanel_namer1..
+000010e0: 0072 6400 0000 da0c 7061 7261 6d5f 7061  .rd.....param_pa
+000010f0: 6e65 6c73 da13 6163 7469 6f6e 5f70 6172  nels..action_par
+00001100: 616d 5f70 616e 656c 73da 0c6f 7468 6572  am_panels..other
+00001110: 5f70 616e 656c 73da 0577 7269 7465 7226  _panels..writer&
+00001120: 0000 0029 0c72 4000 0000 da01 66da 1063  ...).r@.....f..c
+00001130: 686f 6963 656c 6973 7473 5f64 6174 6172  hoicelists_datar
+00001140: 5500 0000 da03 7270 74da 0262 6172 7000  U.....rpt..barp.
+00001150: 0000 da04 6461 7461 7266 0000 00da 0170  ....datarf.....p
+00001160: 7235 0000 00da 0469 7465 6d72 3700 0000  r5.....itemr7...
+00001170: 7251 0000 0072 3800 0000 da0d 7772 6974  rQ...r8.....writ
+00001180: 655f 6c69 6e6f 5f6a 734a 0000 0073 7800  e_lino_jsJ...sx.
+00001190: 0000 0607 0803 06fd 0605 0a01 0c02 0a01  ................
+000011a0: 0c01 0280 02fe 0604 0801 0201 1001 0c02  ................
+000011b0: 0601 0601 0a01 1001 06f9 0c09 0402 1001  ................
+000011c0: 06ff 1206 0201 0401 1001 02ff 0202 0cfe  ................
+000011d0: 0c03 0401 02ff 0c03 1001 0c02 0e01 0c01  ................
+000011e0: 1001 0c02 1801 0409 0a01 1001 1401 1401  ................
+000011f0: 0e01 1201 0480 0a01 1201 0a01 1401 0a01  ................
+00001200: 1401 0e01 0e05 0602 0401 7a16 5265 6e64  ..........z.Rend
+00001210: 6572 6572 2e77 7269 7465 5f6c 696e 6f5f  erer.write_lino_
+00001220: 6a73 6302 0000 0000 0000 0000 0000 0004  jsc.............
+00001230: 0000 0006 0000 0043 0000 0073 c600 0000  .......C...s....
+00001240: 7400 7c01 7401 8302 7307 4a00 8201 7402  t.|.t...s.J...t.
+00001250: 7c01 6a03 7c01 a004 a100 7c01 a005 a100  |.j.|.....|.....
+00001260: 7c01 6a06 6401 8d04 7d02 7400 7c01 7407  |.j.d...}.t.|.t.
+00001270: 8302 7229 7c01 6a08 6a09 6a03 7c02 6402  ..r)|.j.j.j.|.d.
+00001280: 3c00 740a 7c01 6a08 6a0b 8301 7c02 6403  <.t.|.j.j...|.d.
+00001290: 3c00 7c01 6a0c 7231 7c01 6a0c 7c02 6404  <.|.j.r1|.j.|.d.
+000012a0: 3c00 7c01 6a0d 7239 7c01 6a0d 7c02 6405  <.|.j.r9|.j.|.d.
+000012b0: 3c00 7c01 6a0e 7240 6406 7c02 6407 3c00  <.|.j.r@d.|.d.<.
+000012c0: 7c01 6a0f 7248 7c01 6a0f 7c02 6408 3c00  |.j.rH|.j.|.d.<.
+000012d0: 7c01 6a10 724f 6406 7c02 6409 3c00 7c01  |.j.rOd.|.d.<.|.
+000012e0: 6a11 7256 6406 7c02 640a 3c00 7c00 a012  j.rVd.|.d.<.|...
+000012f0: 7c01 a101 7d03 7c03 7261 7c03 7c02 640b  |...}.|.ra|.|.d.
+00001300: 3c00 7c02 5300 290c 7a33 436f 6e76 6572  <.|.S.).z3Conver
+00001310: 7473 2067 6c6f 6261 6c20 6c69 7374 206f  ts global list o
+00001320: 6620 616c 6c20 6163 7469 6f6e 7320 746f  f all actions to
+00001330: 206a 736f 6e20 666f 726d 6174 2e29 04da   json format.)..
+00001340: 0261 6eda 056c 6162 656c da0d 7769 6e64  .an..label..wind
+00001350: 6f77 5f61 6374 696f 6eda 0b68 7474 705f  ow_action..http_
+00001360: 6d65 7468 6f64 7295 0000 00da 0561 6374  methodr......act
+00001370: 6f72 da0c 7072 6570 726f 6365 7373 6f72  or..preprocessor
+00001380: da0b 7365 6c65 6374 5f72 6f77 7354 da10  ..select_rowsT..
+00001390: 7375 626d 6974 5f66 6f72 6d5f 6461 7461  submit_form_data
+000013a0: da0b 6275 7474 6f6e 5f74 6578 74da 1473  ..button_text..s
+000013b0: 686f 775f 696e 5f73 6964 655f 746f 6f6c  how_in_side_tool
+000013c0: 6261 72da 0e6e 6576 6572 5f63 6f6c 6c61  bar..never_colla
+000013d0: 7073 65da 0469 636f 6e29 13da 0a69 7369  pse..icon)...isi
+000013e0: 6e73 7461 6e63 6572 1700 0000 7271 0000  nstancer....rq..
+000013f0: 0072 4e00 0000 da09 6765 745f 6c61 6265  .rN.....get_labe
+00001400: 6cda 1069 735f 7769 6e64 6f77 5f61 6374  l..is_window_act
+00001410: 696f 6e72 9800 0000 7212 0000 00da 0c62  ionr....r......b
+00001420: 6f75 6e64 5f61 6374 696f 6e72 6c00 0000  ound_actionrl...
+00001430: 7246 0000 0072 9900 0000 729a 0000 0072  rF...r....r....r
+00001440: 9b00 0000 729c 0000 0072 9d00 0000 729e  ....r....r....r.
+00001450: 0000 0072 9f00 0000 da0f 6765 745f 6163  ...r......get_ac
+00001460: 7469 6f6e 5f69 636f 6e29 0472 4000 0000  tion_icon).r@...
+00001470: da01 76da 0672 6573 756c 7472 a000 0000  ..v..resultr....
+00001480: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
+00001490: 4f00 0000 a100 0000 7324 0000 000e 0206  O.......s$......
+000014a0: 0406 0106 0104 0106 fd0a 060e 0110 0110  ................
+000014b0: 0210 020e 0110 010e 010e 010a 020c 0104  ................
+000014c0: 027a 1452 656e 6465 7265 722e 6163 7469  .z.Renderer.acti
+000014d0: 6f6e 326a 736f 6e63 0200 0000 0000 0000  on2jsonc........
+000014e0: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+000014f0: 732e 0000 0074 007c 0174 0183 0273 074a  s....t.|.t...s.J
+00001500: 0082 017c 01a0 02a1 007d 0274 037c 00a0  ...|.....}.t.|..
+00001510: 047c 026a 05a1 017c 026a 066a 0764 018d  .|.j...|.j.j.d..
+00001520: 0253 0029 024e 2902 da04 6d61 696e da0b  .S.).N)...main..
+00001530: 7769 6e64 6f77 5f73 697a 6529 0872 a100  window_size).r..
+00001540: 0000 721d 0000 00da 1167 6574 5f6c 6179  ..r......get_lay
+00001550: 6f75 745f 6861 6e64 6c65 7271 0000 00da  out_handlerq....
+00001560: 0965 6c65 6d32 6a73 6f6e 72a8 0000 00da  .elem2jsonr.....
+00001570: 066c 6179 6f75 7472 a900 0000 2903 7240  .layoutr....).r@
+00001580: 0000 0072 9200 0000 72a6 0000 0072 3700  ...r....r....r7.
+00001590: 0000 7237 0000 0072 3800 0000 7287 0000  ..r7...r8...r...
+000015a0: 00be 0000 0073 0a00 0000 0e01 0803 0c01  .....s..........
+000015b0: 0601 06ff 7a13 5265 6e64 6572 6572 2e70  ....z.Renderer.p
+000015c0: 616e 656c 326a 736f 6e63 0200 0000 0000  anel2jsonc......
+000015d0: 0000 0000 0000 0400 0000 0500 0000 0300  ................
+000015e0: 0000 73da 0000 0074 007c 0174 0183 0273  ..s....t.|.t...s
+000015f0: 074a 0082 0174 027c 01a0 03a1 007c 016a  .J...t.|.....|.j
+00001600: 047c 016a 056a 0664 018d 037d 0274 077c  .|.j.j.d...}.t.|
+00001610: 0164 0283 0272 2487 0066 0164 0364 0484  .d...r$..f.d.d..
+00001620: 087c 016a 0844 0083 017c 0264 053c 007c  .|.j.D...|.d.<.|
+00001630: 02a0 0974 0a7c 0164 0683 02a1 0101 0074  ...t.|.d.......t
+00001640: 077c 0164 0783 0272 557c 02a0 0974 0a7c  .|.d...rU|...t.|
+00001650: 016a 0b64 0883 02a1 0101 0074 077c 0164  .j.d.......t.|.d
+00001660: 0983 0272 557c 016a 0c64 0075 0172 557c  ...rU|.j.d.u.rU|
+00001670: 016a 0ca0 0da1 0044 005d 0b5c 027d 037d  .j.....D.].\.}.}
+00001680: 0188 00a0 0e7c 01a1 017c 027c 033c 0071  .....|...|.|.<.q
+00001690: 4974 0f7c 016a 0574 1083 0272 6b7c 026a  It.|.j.t...rk|.j
+000016a0: 097c 01a0 11a1 0064 0a8d 0101 007c 026a  .|.....d.....|.j
+000016b0: 097c 016a 126a 1364 0b8d 0101 007c 0253  .|.j.j.d.....|.S
+000016c0: 0029 0c4e 2903 7296 0000 00da 0873 6f72  .).N).r......sor
+000016d0: 7461 626c 65da 0a72 6561 6374 5f6e 616d  table..react_nam
+000016e0: 65da 0865 6c65 6d65 6e74 7363 0100 0000  e..elementsc....
+000016f0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00001700: 1300 0000 731e 0000 0067 007c 005d 0b7d  ....s....g.|.].}
+00001710: 017c 01a0 00a1 0072 0288 00a0 017c 01a1  .|.....r.....|..
+00001720: 0191 0271 0253 0072 3700 0000 2902 da0a  ...q.S.r7...)...
+00001730: 6973 5f76 6973 6962 6c65 72ab 0000 0029  is_visibler....)
+00001740: 0272 4700 0000 da01 6572 5100 0000 7237  .rG.....erQ...r7
+00001750: 0000 0072 3800 0000 7249 0000 00ce 0000  ...r8...rI......
+00001760: 0073 0200 0000 1e00 7a26 5265 6e64 6572  .s......z&Render
+00001770: 6572 2e65 6c65 6d32 6a73 6f6e 2e3c 6c6f  er.elem2json.<lo
+00001780: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00001790: 7268 0000 007a 9866 6965 6c64 735f 696e  rh...z.fields_in
+000017a0: 6465 7820 6669 656c 6473 5f69 6e64 6578  dex fields_index
+000017b0: 5f68 6964 6465 6e20 6564 6974 6162 6c65  _hidden editable
+000017c0: 2076 6572 7469 6361 6c20 6870 6164 2069   vertical hpad i
+000017d0: 735f 6669 656c 6473 6574 206e 616d 6520  s_fieldset name 
+000017e0: 7769 6474 6820 7072 6566 6572 7265 645f  width preferred_
+000017f0: 7769 6474 6820 2020 2020 2020 2020 2020  width           
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 2020 2020 2020 2068 6964 6465 6e20 7661         hidden va
+00001820: 6c75 6520 6866 6c65 7820 7666 6c65 7872  lue hflex vflexr
+00001830: 9900 0000 7a15 6163 746f 725f 6964 2064  ....z.actor_id d
+00001840: 6973 706c 6179 5f6d 6f64 65da 0673 6c61  isplay_mode..sla
+00001850: 7665 7329 01da 0d66 6965 6c64 5f6f 7074  ves)...field_opt
+00001860: 696f 6e73 2901 da09 6865 6c70 5f74 6578  ions)...help_tex
+00001870: 7429 1472 a100 0000 721e 0000 0072 7100  t).r....r....rq.
+00001880: 0000 72a2 0000 0072 ad00 0000 7243 0000  ..r....r....rC..
+00001890: 00da 085f 5f6e 616d 655f 5f72 8300 0000  ...__name__r....
+000018a0: 72af 0000 0072 7700 0000 7228 0000 0072  r....rw...r(...r
+000018b0: 9900 0000 72b2 0000 0072 6800 0000 72ab  ....r....rh...r.
+000018c0: 0000 00da 0a69 7373 7562 636c 6173 7372  .....issubclassr
+000018d0: 2100 0000 da11 6765 745f 6669 656c 645f  !.....get_field_
+000018e0: 6f70 7469 6f6e 73da 0566 6965 6c64 72b4  options..fieldr.
+000018f0: 0000 0029 0472 4000 0000 72a6 0000 0072  ...).r@...r....r
+00001900: a700 0000 da01 6b72 3700 0000 7251 0000  ......kr7...rQ..
+00001910: 0072 3800 0000 72ab 0000 00c6 0000 0073  .r8...r........s
+00001920: 2200 0000 0e01 0802 0401 0602 06fd 0a04  "...............
+00001930: 1801 1002 0a04 1202 1403 1201 1001 0c03  ................
+00001940: 1001 1001 0402 7a12 5265 6e64 6572 6572  ......z.Renderer
+00001950: 2e65 6c65 6d32 6a73 6f6e 6301 0000 0000  .elem2jsonc.....
+00001960: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00001970: 0000 0073 0400 0000 6401 5300 2902 4e7a  ...s....d.S.).Nz
+00001980: 1e77 696e 646f 772e 4170 702e 6461 7368  .window.App.dash
+00001990: 626f 6172 642e 7265 6c6f 6164 2829 3b72  board.reload();r
+000019a0: 3700 0000 7251 0000 0072 3700 0000 7237  7...rQ...r7...r7
+000019b0: 0000 0072 3800 0000 da09 7265 6c6f 6164  ...r8.....reload
+000019c0: 5f6a 73e6 0000 0073 0200 0000 0401 7a12  _js....s......z.
+000019d0: 5265 6e64 6572 6572 2e72 656c 6f61 645f  Renderer.reload_
+000019e0: 6a73 6302 0000 0000 0000 0000 0000 0006  jsc.............
+000019f0: 0000 0004 0000 004f 0000 0073 dc00 0000  .......O...s....
+00001a00: 7c01 6a00 6a01 6401 6b02 720f 7c00 6a02  |.j.j.d.k.r.|.j.
+00001a10: 6a03 7c02 6900 7c03 a401 8e01 5300 7c01  j.|.i.|.....S.|.
+00001a20: a004 a100 7d04 7c03 a005 7c04 6402 1900  ....}.|...|.d...
+00001a30: a101 0100 7406 7c03 7c01 8302 0100 7c01  ....t.|.|.....|.
+00001a40: 6a07 6403 7501 722c 7c03 a008 7409 6a0a  j.d.u.r,|...t.j.
+00001a50: 7c01 6a07 a102 0100 7c01 6a0b 6403 7501  |.j.....|.j.d.u.
+00001a60: 7239 7c03 a008 7409 6a0c 7c01 6a0b a102  r9|...t.j.|.j...
+00001a70: 0100 7c01 6a0d 6403 7501 725c 7c01 6a0d  ..|.j.d.u.r\|.j.
+00001a80: 6404 1900 7d05 7c05 a00e 6405 a101 7255  d...}.|...d...rU
+00001a90: 7c05 6406 6403 8502 1900 7d05 7c03 a008  |.d.d.....}.|...
+00001aa0: 7409 6a0f 6407 a102 0100 7c03 a008 7409  t.j.d.....|...t.
+00001ab0: 6a10 7c05 a102 0100 7c00 6a02 6a03 7c01  j.|.....|.j.j.|.
+00001ac0: 6a00 6a11 7c01 6a00 6a01 6702 7c02 a201  j.j.|.j.j.g.|...
+00001ad0: 5200 6900 7c03 a401 8e01 5300 2908 7a20  R.i.|.....S.).z 
+00001ae0: 5573 6564 2066 6f72 2074 7572 6e20 7265  Used for turn re
+00001af0: 7175 6573 7473 2069 6e74 6f20 7572 6c73  quests into urls
+00001b00: da04 4d61 696e da0b 6261 7365 5f70 6172  ..Main..base_par
+00001b10: 616d 734e 7201 0000 00fa 012d 722d 0000  amsNr......-r-..
+00001b20: 00da 0444 4553 4329 1272 9900 0000 72b5  ...DESC).r....r.
+00001b30: 0000 0072 4100 0000 da0f 6275 696c 645f  ...rA.....build_
+00001b40: 706c 6169 6e5f 7572 6cda 0a67 6574 5f73  plain_url..get_s
+00001b50: 7461 7475 7372 7700 0000 7208 0000 00da  tatusrw...r.....
+00001b60: 066f 6666 7365 74da 0a73 6574 6465 6661  .offset..setdefa
+00001b70: 756c 7472 0c00 0000 da0f 5552 4c5f 5041  ultr......URL_PA
+00001b80: 5241 4d5f 5354 4152 54da 056c 696d 6974  RAM_START..limit
+00001b90: da0f 5552 4c5f 5041 5241 4d5f 4c49 4d49  ..URL_PARAM_LIMI
+00001ba0: 54da 086f 7264 6572 5f62 79da 0a73 7461  T..order_by..sta
+00001bb0: 7274 7377 6974 68da 1155 524c 5f50 4152  rtswith..URL_PAR
+00001bc0: 414d 5f53 4f52 5444 4952 da0e 5552 4c5f  AM_SORTDIR..URL_
+00001bd0: 5041 5241 4d5f 534f 5254 da09 6170 705f  PARAM_SORT..app_
+00001be0: 6c61 6265 6c29 0672 4000 0000 da02 6172  label).r@.....ar
+00001bf0: da04 6172 6773 da02 6b77 da02 7374 da02  ..args..kw..st..
+00001c00: 7363 7237 0000 0072 3700 0000 7238 0000  scr7...r7...r8..
+00001c10: 00da 0f67 6574 5f72 6571 7565 7374 5f75  ...get_request_u
+00001c20: 726c e900 0000 732c 0000 000c 0212 0108  rl....s,........
+00001c30: 020e 010a 010a 0110 010a 0110 010a 010a  ................
+00001c40: 010a 010c 010e 010e 0106 030c 0102 ff02  ................
+00001c50: 0106 ff02 0106 ff7a 1852 656e 6465 7265  .......z.Rendere
+00001c60: 722e 6765 745f 7265 7175 6573 745f 7572  r.get_request_ur
+00001c70: 6c4e 6305 0000 0000 0000 0000 0000 0007  lNc.............
+00001c80: 0000 0005 0000 004b 0000 0073 ae00 0000  .......K...s....
+00001c90: 7c04 7005 7c03 a000 a100 7d04 7401 7c04  |.p.|.....}.t.|.
+00001ca0: 8301 6401 6b02 7211 6402 a002 7c04 a101  ..d.k.r.d...|...
+00001cb0: 7d04 7c03 6a03 6a04 722c 7c03 6a03 6a05  }.|.j.j.r,|.j.j.
+00001cc0: 732c 7c00 a006 7c02 7c03 7c01 a103 7d06  s,|...|.|.|...}.
+00001cd0: 7c00 6a07 7c02 7c03 7c06 7c04 6604 6900  |.j.|.|.|.|.f.i.
+00001ce0: 7c05 a401 8e01 5300 7c03 6a03 6a08 724b  |.....S.|.j.j.rK
+00001cf0: 7c02 a009 a100 7d06 7c01 6400 7501 723f  |.....}.|.d.u.r?
+00001d00: 7c06 6a0a 7c01 6a0b 6403 8d01 0100 7c00  |.j.|.j.d.....|.
+00001d10: 6a07 7c02 7c03 7c06 7c04 6604 6900 7c05  j.|.|.|.|.f.i.|.
+00001d20: a401 8e01 5300 7c00 6a0c 7c01 7c02 7c03  ....S.|.j.|.|.|.
+00001d30: 7c04 6604 6900 7c05 a401 8e01 5300 2904  |.f.i.|.....S.).
+00001d40: 4e72 2d00 0000 7506 0000 00c2 a07b 7dc2  Nr-...u......{}.
+00001d50: a029 01da 0972 6563 6f72 645f 6964 290d  .)...record_id).
+00001d60: da10 6765 745f 6275 7474 6f6e 5f6c 6162  ..get_button_lab
+00001d70: 656c da03 6c65 6eda 0666 6f72 6d61 7472  el..len..formatr
+00001d80: 6c00 0000 da0a 7061 7261 6d65 7465 7273  l.....parameters
+00001d90: da10 6e6f 5f70 6172 616d 735f 7769 6e64  ..no_params_wind
+00001da0: 6f77 da11 6765 745f 6163 7469 6f6e 5f73  ow..get_action_s
+00001db0: 7461 7475 73da 1477 696e 646f 775f 6163  tatus..window_ac
+00001dc0: 7469 6f6e 5f62 7574 746f 6eda 0e6f 7065  tion_button..ope
+00001dd0: 6e73 5f61 5f77 696e 646f 7772 c000 0000  ns_a_windowr....
+00001de0: 7277 0000 00da 0270 6bda 1172 6f77 5f61  rw.....pk..row_a
+00001df0: 6374 696f 6e5f 6275 7474 6f6e 2907 7240  ction_button).r@
+00001e00: 0000 00da 036f 626a 72cb 0000 0072 9000  .....objr....r..
+00001e10: 0000 7296 0000 0072 cd00 0000 72ce 0000  ..r....r....r...
+00001e20: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
+00001e30: da0d 6163 7469 6f6e 5f62 7574 746f 6e01  ..action_button.
+00001e40: 0100 0073 2000 0000 0c01 0c01 0a01 1002  ...s ...........
+00001e50: 0e01 0401 0801 04ff 0201 06ff 0802 0801  ................
+00001e60: 0801 0e01 1801 1801 7a16 5265 6e64 6572  ........z.Render
+00001e70: 6572 2e61 6374 696f 6e5f 6275 7474 6f6e  er.action_button
+00001e80: 6305 0000 0000 0000 0000 0000 0007 0000  c...............
+00001e90: 0004 0000 004b 0000 0073 4000 0000 7c02  .....K...s@...|.
+00001ea0: 6401 7500 720d 7c03 6a00 6402 6900 7c04  d.u.r.|.j.d.i.|.
+00001eb0: a401 8e01 7d06 6e09 7c02 6a01 7c03 6601  ....}.n.|.j.|.f.
+00001ec0: 6900 7c04 a401 8e01 7d06 7c00 6a02 7c06  i.|.....}.|.j.|.
+00001ed0: 7c01 6602 6900 7c05 a401 8e01 5300 2903  |.f.i.|.....S.).
+00001ee0: 61cf 0100 004e 6f74 6520 7468 6174 2060  a....Note that `
+00001ef0: 6261 2e61 6374 6f72 6020 6d61 7920 6469  ba.actor` may di
+00001f00: 6666 6572 2066 726f 6d20 6061 722e 6163  ffer from `ar.ac
+00001f10: 746f 7260 2077 6865 6e20 6465 6669 6e65  tor` when define
+00001f20: 6420 6f6e 2061 0a20 2020 2020 2020 2064  d on a.        d
+00001f30: 6966 6665 7265 6e74 2061 6374 6f72 2e20  ifferent actor. 
+00001f40: 5265 6d65 6d62 6572 2065 2e67 2e20 7468  Remember e.g. th
+00001f50: 6520 224d 7573 7420 7265 6164 2065 4944  e "Must read eID
+00001f60: 2063 6172 6422 2061 6374 696f 6e0a 2020   card" action.  
+00001f70: 2020 2020 2020 6275 7474 6f6e 2069 6e20        button in 
+00001f80: 6569 645f 696e 666f 206f 6620 6e65 7763  eid_info of newc
+00001f90: 6f6d 6572 732e 4e65 7743 6c69 656e 7473  omers.NewClients
+00001fa0: 2028 3230 3134 3034 3232 292e 0a0a 2020   (20140422)...  
+00001fb0: 2020 2020 2020 3a6f 626a 3a20 2054 6865        :obj:  The
+00001fc0: 2064 6174 6162 6173 6520 6f62 6a65 6374   database object
+00001fd0: 0a20 2020 2020 2020 203a 6172 3a20 2020  .        :ar:   
+00001fe0: 5468 6520 6163 7469 6f6e 2072 6571 7565  The action reque
+00001ff0: 7374 0a20 2020 2020 2020 203a 6261 3a20  st.        :ba: 
+00002000: 2054 6865 2062 6f75 6e64 2061 6374 696f   The bound actio
+00002010: 6e0a 2020 2020 2020 2020 3a72 6571 7565  n.        :reque
+00002020: 7374 5f6b 7761 7267 733a 206b 6579 776f  st_kwargs: keywo
+00002030: 7264 2061 7267 756d 656e 7473 2074 6f20  rd arguments to 
+00002040: 666f 7277 6172 6465 6420 746f 2074 6865  forwarded to the
+00002050: 2063 6869 6c64 2061 6374 696f 6e20 7265   child action re
+00002060: 7175 6573 740a 0a20 2020 2020 2020 2041  quest..        A
+00002070: 6e79 206b 6579 776f 7264 206f 7468 6572  ny keyword other
+00002080: 2061 7267 756d 656e 7473 2061 7265 2066   arguments are f
+00002090: 6f72 7761 7264 6564 2074 6f20 3a6d 6574  orwarded to :met
+000020a0: 683a 6061 7232 6a73 602e 0a0a 2020 2020  h:`ar2js`...    
+000020b0: 2020 2020 4e72 3700 0000 2903 da07 7265      Nr7...)...re
+000020c0: 7175 6573 74da 0573 7061 776e da05 6172  quest..spawn..ar
+000020d0: 326a 7329 0772 4000 0000 72dc 0000 0072  2js).r@...r....r
+000020e0: cb00 0000 7290 0000 00da 0e72 6571 7565  ....r......reque
+000020f0: 7374 5f6b 7761 7267 73da 0673 7461 7475  st_kwargs..statu
+00002100: 73da 0373 6172 7237 0000 0072 3700 0000  s..sarr7...r7...
+00002110: 7238 0000 00da 1761 6374 696f 6e5f 6361  r8.....action_ca
+00002120: 6c6c 5f6f 6e5f 696e 7374 616e 6365 1201  ll_on_instance..
+00002130: 0000 7308 0000 0008 0e12 0112 0314 017a  ..s............z
+00002140: 2052 656e 6465 7265 722e 6163 7469 6f6e   Renderer.action
+00002150: 5f63 616c 6c5f 6f6e 5f69 6e73 7461 6e63  _call_on_instanc
+00002160: 6563 0200 0000 0000 0000 0000 0000 0400  ec..............
+00002170: 0000 0400 0000 4300 0000 732c 0000 007c  ......C...s,...|
+00002180: 016a 0070 057c 016a 017d 0274 02a0 037c  .j.p.|.j.}.t...|
+00002190: 0264 01a1 027d 037c 0364 0175 0072 1264  .d...}.|.d.u.r.d
+000021a0: 0153 0064 027c 0316 0053 0029 037a bf0a  .S.d.|...S.).z..
+000021b0: 2020 2020 2020 2020 5573 6573 2061 6e20          Uses an 
+000021c0: 696e 7465 726e 616c 206d 6170 7069 6e67  internal mapping
+000021d0: 2066 6f72 2069 636f 6e20 6e61 6d65 7320   for icon names 
+000021e0: 746f 2063 6f6e 7665 7274 2065 7869 7374  to convert exist
+000021f0: 696e 6720 6963 6f6e 7320 696e 746f 2072  ing icons into r
+00002200: 6561 6374 2d75 7361 626c 652e 0a20 2020  eact-usable..   
+00002210: 2020 2020 203a 7061 7261 6d20 6163 7469       :param acti
+00002220: 6f6e 3a0a 2020 2020 2020 2020 3a72 6574  on:.        :ret
+00002230: 7572 6e3a 2073 7472 3a20 6120 6963 6f6e  urn: str: a icon
+00002240: 206e 616d 6520 666f 7220 6569 7468 6572   name for either
+00002250: 2070 7269 6d65 2d72 6561 6374 206f 7220   prime-react or 
+00002260: 6963 6f6e 380a 2020 2020 2020 2020 4e7a  icon8.        Nz
+00002270: 0570 6920 2573 2904 da0f 7265 6163 745f  .pi %s)...react_
+00002280: 6963 6f6e 5f6e 616d 65da 0969 636f 6e5f  icon_name..icon_
+00002290: 6e61 6d65 722e 0000 00da 0367 6574 2904  namer......get).
+000022a0: 7240 0000 0072 6c00 0000 72a0 0000 00da  r@...rl...r.....
+000022b0: 0a72 6561 6374 5f69 636f 6e72 3700 0000  .react_iconr7...
+000022c0: 7237 0000 0072 3800 0000 72a5 0000 0027  r7...r8...r....'
+000022d0: 0100 0073 0a00 0000 0c07 0c01 0801 0401  ...s............
+000022e0: 0802 7a18 5265 6e64 6572 6572 2e67 6574  ..z.Renderer.get
+000022f0: 5f61 6374 696f 6e5f 6963 6f6e 6303 0000  _action_iconc...
+00002300: 0000 0000 0000 0000 0008 0000 0007 0000  ................
+00002310: 004b 0000 0073 a400 0000 7c01 6a00 7d04  .K...s....|.j.}.
+00002320: 7c01 6a01 7d05 6900 7d06 7c05 6a02 a003  |.j.}.i.}.|.j...
+00002330: a100 721c 7c03 a004 7c00 a005 7c01 7c05  ..r.|...|...|.|.
+00002340: 7c02 a103 a101 0100 7c06 a004 7c03 a101  |.......|...|...
+00002350: 0100 7c06 a004 7c00 a006 7c01 7c05 7c02  ..|...|...|.|.|.
+00002360: a103 a101 0100 7c06 a004 7c03 a101 0100  ......|...|.....
+00002370: 7c04 7c05 6a02 6a07 7c01 6a08 7c05 6a09  |.|.j.j.|.j.|.j.
+00002380: 6a0a 7c06 6401 9c05 7d07 740b 7c02 6402  j.|.d...}.t.|.d.
+00002390: 8302 7243 7c02 6a0c 7c07 6403 3c00 6e09  ..rC|.j.|.d.<.n.
+000023a0: 740d 7c02 740e 8302 724c 7c02 7c07 6403  t.|.t...rL|.|.d.
+000023b0: 3c00 6404 740f 7c07 8301 1600 5300 2905  <.d.t.|.....S.).
+000023c0: 7a43 496d 706c 656d 656e 7473 203a 6d65  zCImplements :me
+000023d0: 7468 3a60 6c69 6e6f 2e63 6f72 652e 7265  th:`lino.core.re
+000023e0: 6e64 6572 6572 2e48 746d 6c52 656e 6465  nderer.HtmlRende
+000023f0: 7265 722e 6172 326a 7360 2e0a 0a20 2020  rer.ar2js`...   
+00002400: 2020 2020 2029 05da 0272 7072 9500 0000       )...rpr....
+00002410: da06 6f6e 4d61 696e da07 6163 746f 7249  ..onMain..actorI
+00002420: 6472 e200 0000 72da 0000 00da 0273 72fa  dr....r......sr.
+00002430: 1877 696e 646f 772e 4170 702e 7275 6e41  .window.App.runA
+00002440: 6374 696f 6e28 2573 2929 10da 1072 6571  ction(%s))...req
+00002450: 7565 7374 696e 675f 7061 6e65 6c72 a400  uesting_panelr..
+00002460: 0000 726c 0000 0072 a300 0000 7277 0000  ..rl...r....rw..
+00002470: 0072 d700 0000 da11 6765 745f 6163 7469  .r......get_acti
+00002480: 6f6e 5f70 6172 616d 7372 4e00 0000 da10  on_paramsrN.....
+00002490: 6973 5f6f 6e5f 6d61 696e 5f61 6374 6f72  is_on_main_actor
+000024a0: 7299 0000 00da 0861 6374 6f72 5f69 6472  r......actor_idr
+000024b0: 8300 0000 72da 0000 0072 a100 0000 7278  ....r....r....rx
+000024c0: 0000 0072 2600 0000 2908 7240 0000 0072  ...r&...).r@...r
+000024d0: cb00 0000 72dc 0000 0072 e200 0000 72e9  ....r....r....r.
+000024e0: 0000 0072 9000 0000 da06 7061 7261 6d73  ...r......params
+000024f0: da06 6a73 5f6f 626a 7237 0000 0072 3700  ..js_objr7...r7.
+00002500: 0000 7238 0000 0072 e000 0000 3501 0000  ..r8...r....5...
+00002510: 732a 0000 0006 0406 0104 010a 0114 040a  s*..............
+00002520: 0114 010a 0102 0306 0104 0106 0102 0106  ................
+00002530: fb0a 070c 010a 0208 0102 0206 0104 ff7a  ...............z
+00002540: 0e52 656e 6465 7265 722e 6172 326a 7363  .Renderer.ar2jsc
+00002550: 0200 0000 0000 0000 0000 0000 0600 0000  ................
+00002560: 0600 0000 4300 0000 73bc 0100 007c 0174  ....C...s....|.t
+00002570: 006a 016a 0275 0072 0a74 0364 0183 0153  .j.j.u.r.t.d...S
+00002580: 0074 047c 0174 0583 0272 1674 0664 02a0  .t.|.t...r.t.d..
+00002590: 077c 01a1 0183 0182 0174 047c 0174 086a  .|.......t.|.t.j
+000025a0: 0983 0272 2009 007c 016a 0a53 0074 047c  ...r ..|.j.S.t.|
+000025b0: 0174 0b6a 0c83 0272 297c 016a 0d53 0074  .t.j...r)|.j.S.t
+000025c0: 047c 0174 0683 0272 3274 0e7c 0183 0153  .|.t...r2t.|...S
+000025d0: 0074 047c 0174 0f83 0272 4a7c 016a 1064  .t.|.t...rJ|.j.d
+000025e0: 0375 0072 3f7c 016a 1153 0074 127c 016a  .u.r?|.j.S.t.|.j
+000025f0: 1374 127c 016a 1164 048d 0164 058d 0253  .t.|.j.d...d...S
+00002600: 0074 047c 0174 1483 0272 cc7c 016a 1564  .t.|.t...r.|.j.d
+00002610: 0375 0172 6d7c 00a0 1664 037c 016a 1564  .u.rm|...d.|.j.d
+00002620: 03a1 037d 027c 0264 0375 0173 624a 0082  ...}.|.d.u.sbJ..
+00002630: 0164 067c 0216 007d 037c 00a0 177c 017c  .d.|...}.|...|.|
+00002640: 0264 03a1 0353 007c 016a 1864 0375 0172  .d...S.|.j.d.u.r
+00002650: 957c 016a 1972 857c 016a 186a 1a64 0d69  .|.j.r.|.j.j.d.i
+00002660: 007c 016a 19a4 018e 017d 047c 00a0 1b7c  .|.j.....}.|...|
+00002670: 04a1 017d 036e 087c 00a0 1c64 037c 016a  ...}.n.|...d.|.j
+00002680: 1869 00a1 037d 037c 00a0 177c 017c 037c  .i...}.|...|.|.|
+00002690: 016a 1da1 0353 007c 016a 1e64 0375 0172  .j...S.|.j.d.u.r
+000026a0: a764 067c 016a 1e16 007d 037c 00a0 177c  .d.|.j...}.|...|
+000026b0: 017c 037c 016a 1da1 0353 007c 016a 1f64  .|.|.j...S.|.j.d
+000026c0: 0375 0172 b07c 016a 1f7d 056e 037c 016a  .u.r.|.j.}.n.|.j
+000026d0: 1353 007c 016a 106a 1064 0375 0072 c574  .S.|.j.j.d.u.r.t
+000026e0: 1264 077c 016a 1374 0364 087c 0516 0083  .d.|.j.t.d.|....
+000026f0: 0164 098d 0353 0074 127c 016a 137c 0564  .d...S.t.|.j.|.d
+00002700: 0a8d 0253 0074 047c 0174 0383 0272 dc74  ...S.t.|.t...r.t
+00002710: 207c 0064 0b64 0c83 0372 dc74 0e7c 016a   |.d.d...r.t.|.j
+00002720: 2183 0153 007c 0153 0029 0e7a 540a 2020  !..S.|.S.).zT.  
+00002730: 2020 2020 2020 4164 6469 7469 6f6e 616c        Additional
+00002740: 2063 6f6e 7665 7274 696e 6720 6c6f 6769   converting logi
+00002750: 6320 666f 7220 7365 7269 616c 697a 696e  c for serializin
+00002760: 6720 5079 7468 6f6e 2076 616c 7565 7320  g Python values 
+00002770: 746f 206a 736f 6e2e 0a20 2020 2020 2020  to json..       
+00002780: 20da 104c 414e 4755 4147 455f 4348 4f49   ..LANGUAGE_CHOI
+00002790: 4345 537a 0b32 3032 3130 3531 3720 7b7d  CESz.20210517 {}
+000027a0: 4e29 0172 6800 0000 2902 7245 0000 0072  N).rh...).rE...r
+000027b0: 5600 0000 7a02 2573 da06 6275 7474 6f6e  V...z.%s..button
+000027c0: 7a23 6675 6e63 7469 6f6e 2829 207b 204c  z#function() { L
+000027d0: 696e 6f2e 6c6f 6164 5f75 726c 2827 2573  ino.load_url('%s
+000027e0: 2729 3b20 7d29 03da 0578 7479 7065 7245  '); })...xtyperE
+000027f0: 0000 00da 0768 616e 646c 6572 2902 7245  .....handler).rE
+00002800: 0000 00da 0468 7265 6672 6e00 0000 4672  .....hrefrn...Fr
+00002810: 3700 0000 2922 7204 0000 0072 6f00 0000  7...)"r....ro...
+00002820: 72f4 0000 0072 2700 0000 72a1 0000 0072  r....r'...r....r
+00002830: 1c00 0000 da09 4578 6365 7074 696f 6e72  ......Exceptionr
+00002840: d400 0000 720d 0000 00da 0643 686f 6963  ....r......Choic
+00002850: 6572 4400 0000 7205 0000 00da 054d 6f64  erD...r......Mod
+00002860: 656c 72da 0000 0072 4600 0000 720a 0000  elr....rF...r...
+00002870: 00da 0670 6172 656e 7472 6800 0000 7271  ...parentrh...rq
+00002880: 0000 0072 9600 0000 720b 0000 00da 0869  ...r....r......i
+00002890: 6e73 7461 6e63 65da 1069 6e73 7461 6e63  nstance..instanc
+000028a0: 655f 6861 6e64 6c65 72da 0c68 616e 646c  e_handler..handl
+000028b0: 6572 5f69 7465 6d72 a400 0000 72f2 0000  er_itemr....r...
+000028c0: 0072 de00 0000 da0f 7265 7175 6573 745f  .r......request_
+000028d0: 6861 6e64 6c65 72da 0b61 6374 696f 6e5f  handler..action_
+000028e0: 6361 6c6c 72b4 0000 00da 0a6a 6176 6173  callr......javas
+000028f0: 6372 6970 7472 f800 0000 da07 6765 7461  criptr......geta
+00002900: 7474 72da 0173 2906 7240 0000 0072 a600  ttr..s).r@...r..
+00002910: 0000 da01 68da 026a 7372 cb00 0000 da03  ....h..jsr......
+00002920: 7572 6c72 3700 0000 7237 0000 0072 3800  urlr7...r7...r8.
+00002930: 0000 723f 0000 0056 0100 0073 5400 0000  ..r?...V...sT...
+00002940: 0c04 0801 0a01 0e01 0c01 0201 0603 0c01  ................
+00002950: 0601 0a01 0801 0a01 0a01 0601 1603 0a02  ................
+00002960: 0a01 1001 0c01 0801 0e01 0a01 0601 1401  ................
+00002970: 0c01 1002 1001 0a02 0a01 1001 0a01 0801  ................
+00002980: 0607 0c02 0202 0601 0a02 06fd 0e04 1602  ................
+00002990: 0a02 0402 7a18 5265 6e64 6572 6572 2e70  ....z.Renderer.p
+000029a0: 7932 6a73 5f63 6f6e 7665 7274 6572 6304  y2js_converterc.
+000029b0: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+000029c0: 0000 0043 0000 0073 5000 0000 7400 7c01  ...C...sP...t.|.
+000029d0: 6a01 7c02 6401 8d02 7d04 7c01 6a02 721a  j.|.d...}.|.j.r.
+000029e0: 7c01 6a02 6a03 6a04 721a 7c04 6a05 6402  |.j.j.j.r.|.j.d.
+000029f0: 7c01 6a02 6a03 6a04 1700 6403 8d01 0100  |.j.j.j...d.....
+00002a00: 7406 6a07 6a08 7226 7c03 7226 7c04 6a05  t.j.j.r&|.r&|.j.
+00002a10: 7c03 6404 8d01 0100 7c04 5300 2905 da00  |.d.....|.S.)...
+00002a20: 2902 7245 0000 0072 f700 0000 7a07 782d  ).rE...r....z.x-
+00002a30: 7462 6172 2d29 01da 0769 636f 6e43 6c73  tbar-)...iconCls
+00002a40: 2901 da07 746f 6f6c 5469 7029 0972 7100  )...toolTip).rq.
+00002a50: 0000 7296 0000 0072 a400 0000 726c 0000  ..r....r....rl..
+00002a60: 0072 e600 0000 7277 0000 0072 0400 0000  .r....rw...r....
+00002a70: 726f 0000 00da 0d75 7365 5f71 7569 636b  ro.....use_quick
+00002a80: 7469 7073 2905 7240 0000 00da 026d 6972  tips).r@.....mir
+00002a90: f700 0000 72b4 0000 00da 0164 7237 0000  ....r......dr7..
+00002aa0: 0072 3700 0000 7238 0000 0072 ff00 0000  .r7...r8...r....
+00002ab0: a401 0000 730c 0000 000e 0410 0116 010c  ....s...........
+00002ac0: 010c 0304 017a 1552 656e 6465 7265 722e  .....z.Renderer.
+00002ad0: 6861 6e64 6c65 725f 6974 656d 6302 0000  handler_itemc...
+00002ae0: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+00002af0: 004f 0000 0073 2000 0000 7c01 6a00 6402  .O...s ...|.j.d.
+00002b00: 6900 7c03 a401 8e01 7d04 7c00 a001 7c01  i.|.....}.|...|.
+00002b10: 7c01 6a02 7c04 a103 5300 2903 7a36 2047  |.j.|...S.).z6 G
+00002b20: 656e 6572 6174 6573 206a 7320 7374 7269  enerates js stri
+00002b30: 6e67 2066 6f72 2061 6374 696f 6e20 6275  ng for action bu
+00002b40: 7474 6f6e 2063 616c 6c73 2e0a 2020 2020  tton calls..    
+00002b50: 2020 2020 4e72 3700 0000 2903 72c0 0000      Nr7...).r...
+00002b60: 0072 0101 0000 72a4 0000 0029 0572 4000  .r....r....).r@.
+00002b70: 0000 72cb 0000 0072 cc00 0000 72cd 0000  ..r....r....r...
+00002b80: 0072 ce00 0000 7237 0000 0072 3700 0000  .r....r7...r7...
+00002b90: 7238 0000 0072 0001 0000 b201 0000 7304  r8...r........s.
+00002ba0: 0000 0010 0410 017a 1852 656e 6465 7265  .......z.Rendere
+00002bb0: 722e 7265 7175 6573 745f 6861 6e64 6c65  r.request_handle
+00002bc0: 7263 0400 0000 0000 0000 0000 0000 0800  rc..............
+00002bd0: 0000 0800 0000 4300 0000 739c 0000 007c  ......C...s....|
+00002be0: 026a 007d 047c 02a0 01a1 00a0 0264 0164  .j.}.|.......d.d
+00002bf0: 02a1 025c 027d 057d 067c 0373 1169 007d  ...\.}.}.|.s.i.}
+00002c00: 037c 0164 0075 0172 2274 037c 0164 0383  .|.d.u.r"t.|.d..
+00002c10: 0272 227c 016a 0464 0869 007c 03a4 018e  .r"|.j.d.i.|....
+00002c20: 017d 037c 0172 2d7c 016a 0572 2d7c 016a  .}.|.r-|.j.r-|.j
+00002c30: 057c 0374 066a 073c 007c 0664 046b 0272  .|.t.j.<.|.d.k.r
+00002c40: 3974 037c 0364 0583 0272 397c 0364 053d  9t.|.d...r9|.d.=
+00002c50: 007c 0164 0075 0072 3f64 006e 027c 016a  .|.d.u.r?d.n.|.j
+00002c60: 087d 0764 0674 0974 0a7c 067c 057c 037c  .}.d.t.t.|.|.|.|
+00002c70: 0764 078d 0483 0116 0053 0029 094e da01  .d.......S.).N..
+00002c80: 2e72 2d00 0000 72c0 0000 00da 0467 7269  .r-...r......gri
+00002c90: 6472 d100 0000 72ed 0000 0029 0472 9500  dr....r....).r..
+00002ca0: 0000 72eb 0000 0072 e200 0000 72e9 0000  ..r....r....r...
+00002cb0: 0072 3700 0000 290b 726c 0000 00da 0966  .r7...).rl.....f
+00002cc0: 756c 6c5f 6e61 6d65 da06 7273 706c 6974  ull_name..rsplit
+00002cd0: 7283 0000 0072 c000 0000 da0a 7375 6273  r....r......subs
+00002ce0: 745f 7573 6572 720c 0000 00da 1455 524c  t_userr......URL
+00002cf0: 5f50 4152 414d 5f53 5542 5354 5f55 5345  _PARAM_SUBST_USE
+00002d00: 5272 ee00 0000 7226 0000 0072 7100 0000  Rr....r&...rq...
+00002d10: 2908 7240 0000 0072 cb00 0000 72a4 0000  ).r@...r....r...
+00002d20: 0072 e200 0000 7250 0000 0072 eb00 0000  .r....rP...r....
+00002d30: 7295 0000 0072 e900 0000 7237 0000 0072  r....r....r7...r
+00002d40: 3700 0000 7238 0000 0072 0101 0000 bc01  7...r8...r......
+00002d50: 0000 7322 0000 0006 0214 0204 0204 0112  ..s"............
+00002d60: 0210 010a 020c 0112 1106 0112 0206 0202  ................
+00002d70: 0102 0102 0102 010a fc7a 1452 656e 6465  .........z.Rende
+00002d80: 7265 722e 6163 7469 6f6e 5f63 616c 6c63  rer.action_callc
+00002d90: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00002da0: 0400 0000 4300 0000 732e 0000 007c 0173  ....C...s....|.s
+00002db0: 0464 0053 0074 007c 0174 0183 0273 0d74  .d.S.t.|.t...s.t
+00002dc0: 017c 0183 017d 0174 027c 0164 0164 028d  .|...}.t.|.d.d..
+00002dd0: 027d 0164 037c 0117 0053 0029 044e 4629  .}.d.|...S.).NF)
+00002de0: 01da 0571 756f 7465 7a0b 6a61 7661 7363  ...quotez.javasc
+00002df0: 7269 7074 3a29 0372 a100 0000 7246 0000  ript:).r....rF..
+00002e00: 0072 0300 0000 2902 7240 0000 0072 0601  .r....).r@...r..
+00002e10: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
+00002e20: 00da 066a 7332 7572 6ce6 0100 0073 0c00  ...js2url....s..
+00002e30: 0000 0401 0401 0a02 0801 0c01 0801 7a0f  ..............z.
+00002e40: 5265 6e64 6572 6572 2e6a 7332 7572 6c63  Renderer.js2urlc
+00002e50: 0600 0000 0000 0000 0000 0000 0700 0000  ................
+00002e60: 0400 0000 4300 0000 7356 0000 0074 006a  ....C...sV...t.j
+00002e70: 016a 0272 2774 006a 016a 0372 0f64 017c  .j.r't.j.j.r.d.|
+00002e80: 047c 0566 0216 007d 066e 0264 027d 067c  .|.f...}.n.d.}.|
+00002e90: 0272 1974 0464 037c 067c 0283 037d 067c  .r.t.d.|.|...}.|
+00002ea0: 0672 297c 016a 0564 047c 037c 0666 0216  .r)|.j.d.|.|.f..
+00002eb0: 0064 058d 0101 0064 0053 0064 0053 0064  .d.....d.S.d.S.d
+00002ec0: 0053 0029 064e 7a08 2825 732e 2573 2920  .S.).Nz.(%s.%s) 
+00002ed0: 7208 0100 007a 047b 7d7b 7d7a 0728 2573  r....z.{}{}z.(%s
+00002ee0: 2c25 7329 2901 da08 7175 6963 6b74 6970  ,%s))...quicktip
+00002ef0: 2906 7204 0000 0072 6f00 0000 720b 0100  ).r....ro...r...
+00002f00: 00da 1973 686f 775f 696e 7465 726e 616c  ...show_internal
+00002f10: 5f66 6965 6c64 5f6e 616d 6573 7206 0000  _field_namesr...
+00002f20: 0072 7700 0000 2907 7240 0000 0072 cd00  .rw...).r@...r..
+00002f30: 0000 72b4 0000 0072 7400 0000 da0a 6461  ..r....rt.....da
+00002f40: 7461 736f 7572 6365 da09 6669 656c 646e  tasource..fieldn
+00002f50: 616d 65da 0374 7474 7237 0000 0072 3700  ame..tttr7...r7.
+00002f60: 0000 7238 0000 00da 0d61 6464 5f68 656c  ..r8.....add_hel
+00002f70: 705f 7465 7874 ef01 0000 7318 0000 0008  p_text....s.....
+00002f80: 0108 010e 0104 0204 010c 0104 0108 0402  ................
+00002f90: 010e ff04 f504 077a 1652 656e 6465 7265  .......z.Rendere
+00002fa0: 722e 6164 645f 6865 6c70 5f74 6578 7463  r.add_help_textc
+00002fb0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00002fc0: 0300 0000 4300 0000 7356 0000 0074 0083  ....C...sV...t..
+00002fd0: 007d 0264 017c 0117 0064 0217 007d 037c  .}.d.|...d...}.|
+00002fe0: 006a 01a0 0264 03a1 0164 0419 007d 047c  .j...d...d...}.|
+00002ff0: 0264 0575 0172 1c7c 037c 026a 0364 0217  .d.u.r.|.|.j.d..
+00003000: 0037 007d 037c 0374 04a0 05a1 0064 0317  .7.}.|.t.....d..
+00003010: 007c 0417 0037 007d 0364 067c 047c 0366  .|...7.}.d.|.|.f
+00003020: 0353 0029 077a 2c4c 696b 6520 6c69 6e6f  .S.).z,Like lino
+00003030: 5f6a 735f 7061 7274 732c 2062 7574 2066  _js_parts, but f
+00003040: 6f72 2061 6374 6f72 5f6c 6576 656c 2064  or actor_level d
+00003050: 6174 61da 054c 696e 6f5f da01 5f72 0e01  ata..Lino_.._r..
+00003060: 0000 722f 0000 004e da05 6361 6368 6529  ..r/...N..cache)
+00003070: 0672 2900 0000 da11 6c69 6e6f 5f77 6562  .r).....lino_web
+00003080: 5f74 656d 706c 6174 6572 1101 0000 7244  _templater....rD
+00003090: 0000 0072 0700 0000 da0c 6765 745f 6c61  ...r......get_la
+000030a0: 6e67 7561 6765 2905 7240 0000 0072 eb00  nguage).r@...r..
+000030b0: 0000 da09 7573 6572 5f74 7970 65da 0866  ....user_type..f
+000030c0: 696c 656e 616d 65da 0966 696c 655f 7479  ilename..file_ty
+000030d0: 7065 7237 0000 0072 3700 0000 7238 0000  per7...r7...r8..
+000030e0: 00da 156c 696e 6f5f 6a73 5f70 6172 7473  ...lino_js_parts
+000030f0: 5f63 6875 6e6b 6564 fe01 0000 730e 0000  _chunked....s...
+00003100: 0006 020c 0110 0108 010e 0114 010a 017a  ...............z
+00003110: 1e52 656e 6465 7265 722e 6c69 6e6f 5f6a  .Renderer.lino_j
+00003120: 735f 7061 7274 735f 6368 756e 6b65 6463  s_parts_chunkedc
+00003130: 0200 0000 0000 0000 0000 0000 1100 0000  ................
+00003140: 0600 0000 4300 0000 73de 0100 0067 007d  ....C...s....g.}
+00003150: 0267 007d 037c 0144 005d e47d 047c 04a0  .g.}.|.D.].}.|..
+00003160: 00a1 007d 057c 0573 127c 046a 016a 0272  ...}.|.s.|.j.j.r
+00003170: cc74 036a 047c 046a 016a 0569 017d 067c  .t.j.|.j.j.i.}.|
+00003180: 0572 237c 066a 067c 056a 076a 0864 018d  .r#|.j.|.j.j.d..
+00003190: 0101 007c 046a 016a 0272 c767 007d 0774  ...|.j.j.r.g.}.t
+000031a0: 0983 007d 087c 046a 0aa0 0b7c 046a 0174  ...}.|.j...|.j.t
+000031b0: 0c83 00a1 0244 005d 727d 0974 097c 096a  .....D.]r}.t.|.j
+000031c0: 016a 0564 028d 017d 0a7c 096a 016a 0d7d  .j.d...}.|.j.j.}
+000031d0: 0b7c 0b72 487c 0b7c 0a64 033c 007c 096a  .|.rH|.|.d.<.|.j
+000031e0: 016a 0e7d 0c7c 0c72 5e74 0f7c 0c83 0172  .j.}.|.r^t.|...r
+000031f0: 5a7c 0c7c 096a 0a83 017c 0a64 043c 006e  Z|.|.j...|.d.<.n
+00003200: 047c 0c7c 0a64 043c 007c 096a 016a 1064  .|.|.d.<.|.j.j.d
+00003210: 0575 0172 847c 096a 016a 107d 0d7c 0d7c  .u.r.|.j.j.}.|.|
+00003220: 0876 0072 747c 087c 0d19 00a0 117c 0aa1  .v.rt|.|.....|..
+00003230: 0101 006e 1574 097c 0d64 068d 017d 0e7c  ...n.t.|.d...}.|
+00003240: 0a67 017c 087c 0d3c 007c 07a0 117c 0ea1  .g.|.|.<.|...|..
+00003250: 0101 006e 057c 07a0 117c 0aa1 0101 007c  ...n.|...|.....|
+00003260: 096a 016a 1272 a774 137c 096a 016a 1283  .j.j.r.t.|.j.j..
+00003270: 017d 0f74 147c 0f64 0783 0273 9e7c 096a  .}.t.|.d...s.|.j
+00003280: 016a 057c 0f64 073c 007c 0f7c 0376 0172  .j.|.d.<.|.|.v.r
+00003290: a77c 03a0 117c 0fa1 0101 0071 357c 0872  .|...|.....q5|.r
+000032a0: c374 157c 0783 0144 005d 145c 027d 107d  .t.|...D.].\.}.}
+000032b0: 0a7c 0aa0 1664 0864 09a1 0272 c27c 087c  .|...d.d...r.|.|
+000032c0: 0a64 0819 0019 007c 077c 1019 0064 0a3c  .d.....|.|...d.<
+000032d0: 0071 ae7c 077c 0664 0b3c 007c 02a0 117c  .q.|.|.d.<.|...|
+000032e0: 06a1 0101 007c 046a 016a 1272 ea74 137c  .....|.j.j.r.t.|
+000032f0: 046a 016a 1283 017d 0f74 147c 0f64 0783  .j.j...}.t.|.d..
+00003300: 0273 e17c 046a 016a 057c 0f64 073c 007c  .s.|.j.j.|.d.<.|
+00003310: 0f7c 0376 0172 ea7c 03a0 117c 0fa1 0101  .|.v.r.|...|....
+00003320: 0071 067c 027c 0366 0253 0029 0c7a 4543  .q.|.|.f.S.).zEC
+00003330: 6f6e 7665 7274 7320 6f66 2061 6c6c 2074  onverts of all t
+00003340: 6865 2062 6f75 6e64 6163 7469 6f6e 7320  he boundactions 
+00003350: 6f66 2061 6e20 6163 746f 7220 746f 206a  of an actor to j
+00003360: 736f 6e20 666f 726d 6174 2e0a 2020 2020  son format..    
+00003370: 2020 2020 a901 7265 0000 0029 0172 9500      ..re...).r..
+00003380: 0000 72b4 0000 00da 0a6a 735f 6861 6e64  ..r......js_hand
+00003390: 6c65 724e 2901 da05 636f 6d62 6f72 9000  lerN)...combor..
+000033a0: 0000 7227 0100 0046 7256 0000 00da 0e74  ..r'...FrV.....t
+000033b0: 6f6f 6c62 6172 4163 7469 6f6e 7329 17da  oolbarActions)..
+000033c0: 1167 6574 5f6c 6179 6f75 745f 6861 6e64  .get_layout_hand
+000033d0: 656c 726c 0000 00da 0b77 696e 646f 775f  elrl.....window_
+000033e0: 7479 7065 720c 0000 00da 1555 524c 5f50  typer......URL_P
+000033f0: 4152 414d 5f41 4354 494f 4e5f 4e41 4d45  ARAM_ACTION_NAME
+00003400: 724e 0000 0072 7700 0000 72ac 0000 0072  rN...rw...r....r
+00003410: 8800 0000 7271 0000 0072 9900 0000 da13  ....rq...r......
+00003420: 6765 745f 746f 6f6c 6261 725f 6163 7469  get_toolbar_acti
+00003430: 6f6e 7372 2900 0000 72b4 0000 0072 2601  onsr)...r....r&.
+00003440: 0000 7230 0000 00da 0b63 6f6d 626f 5f67  ..r0.....combo_g
+00003450: 726f 7570 da06 6170 7065 6e64 da06 686f  roup..append..ho
+00003460: 746b 6579 da04 7661 7273 7283 0000 0072  tkey..varsr....r
+00003470: 3100 0000 72e7 0000 0029 1172 4000 0000  1...r....).r@...
+00003480: da0c 6163 7469 6f6e 735f 6c69 7374 72a7  ..actions_listr.
+00003490: 0000 00da 0768 6f74 6b65 7973 7290 0000  .....hotkeysr...
+000034a0: 00da 026c 68da 1161 6374 696f 6e5f 6465  ...lh..action_de
+000034b0: 7363 7269 7074 6f72 da04 7462 6173 da09  scriptor..tbas..
+000034c0: 636f 6d62 6f5f 6d61 7072 5000 0000 da03  combo_maprP.....
+000034d0: 7462 6172 b400 0000 7226 0100 0072 2d01  tbar....r&...r-.
+000034e0: 0000 7227 0100 0072 2f01 0000 7235 0000  ..r'...r/...r5..
+000034f0: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
+00003500: da0c 6163 7469 6f6e 7332 6a73 6f6e 0802  ..actions2json..
+00003510: 0000 7368 0000 0004 0404 0108 0208 010c  ..sh............
+00003520: 010e 0204 0110 0108 0104 0106 0106 0208  ................
+00003530: 0108 ff0e 0308 010c 0108 0104 0108 0110  ................
+00003540: 0108 020c 0208 0108 0210 010a 020a 010c  ................
+00003550: 010a 0208 020c 010a 010c 0108 010a 0102  ................
+00003560: 8004 0210 010c 0114 0102 8008 020a 0208  ................
+00003570: 020c 010a 010c 0108 010a 0102 8008 027a  ...............z
+00003580: 1552 656e 6465 7265 722e 6163 7469 6f6e  .Renderer.action
+00003590: 7332 6a73 6f6e 6302 0000 0000 0000 0000  s2jsonc.........
+000035a0: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
+000035b0: 5800 0000 6700 7d02 6400 7d03 7c01 4400  X...g.}.d.}.|.D.
+000035c0: 5d14 7d04 7c04 6401 1900 6400 7500 7213  ].}.|.d...d.u.r.
+000035d0: 7c04 6402 1900 7d03 7106 7c02 a000 7401  |.d...}.q.|...t.
+000035e0: 7c04 8301 a101 0100 7106 7402 7c02 6403  |.......q.t.|.d.
+000035f0: 6404 8400 6405 8d02 7d02 7c02 a000 6400  d...d...}.|...d.
+00003600: 7c03 6702 a101 0100 7c02 5300 2906 4e72  |.g.....|.S.).Nr
+00003610: 0100 0000 722d 0000 0063 0100 0000 0000  ....r-...c......
+00003620: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
+00003630: 0000 7308 0000 007c 0064 0119 0053 0029  ..s....|.d...S.)
+00003640: 024e 7201 0000 0072 3700 0000 2901 7236  .Nr....r7...).r6
+00003650: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
+00003660: 0000 da08 3c6c 616d 6264 613e 5402 0000  ....<lambda>T...
+00003670: 7302 0000 0008 007a 2c52 656e 6465 7265  s......z,Rendere
+00003680: 722e 6469 7370 6c61 795f 6d6f 6465 326a  r.display_mode2j
+00003690: 736f 6e2e 3c6c 6f63 616c 733e 2e3c 6c61  son.<locals>.<la
+000036a0: 6d62 6461 3ea9 0172 3400 0000 2903 722e  mbda>..r4...).r.
+000036b0: 0100 0072 7800 0000 da06 736f 7274 6564  ...rx.....sorted
+000036c0: 2905 7240 0000 00da 0c64 6973 706c 6179  ).r@.....display
+000036d0: 5f6d 6f64 65da 0364 6d73 da03 646d 6472  _mode..dms..dmdr
+000036e0: 9300 0000 7237 0000 0072 3700 0000 7238  ....r7...r7...r8
+000036f0: 0000 00da 1164 6973 706c 6179 5f6d 6f64  .....display_mod
+00003700: 6532 6a73 6f6e 4c02 0000 7312 0000 0004  e2jsonL...s.....
+00003710: 0104 0108 010c 010a 0110 0210 010e 0104  ................
+00003720: 017a 1a52 656e 6465 7265 722e 6469 7370  .z.Renderer.disp
+00003730: 6c61 795f 6d6f 6465 326a 736f 6e63 0200  lay_mode2jsonc..
+00003740: 0000 0000 0000 0000 0000 1100 0000 0800  ................
+00003750: 0000 4300 0000 7322 0300 0074 007c 0183  ..C...s"...t.|..
+00003760: 0172 0974 017c 0174 0283 0273 0b4a 0082  .r.t.|.t...s.J..
+00003770: 017c 00a0 037c 016a 04a1 015c 027d 027d  .|...|.j...\.}.}
+00003780: 0374 057c 016a 067c 027c 01a0 07a1 0074  .t.|.j.|.|.....t
+00003790: 087c 016a 0983 017c 01a0 0a74 0b83 00a1  .|.j...|...t....
+000037a0: 010c 0064 018d 057d 0474 0c7c 0383 0172  ...d...}.t.|...r
+000037b0: 317c 046a 0d7c 0364 028d 0101 007c 01a0  1|.j.|.d.....|..
+000037c0: 0ea1 007d 057c 056a 0f64 0075 0072 4374  ...}.|.j.d.u.rCt
+000037d0: 106a 116a 12a0 1364 037c 01a1 0201 006e  .j.j...d.|.....n
+000037e0: 5d74 147c 0564 0483 0272 9767 007d 0664  ]t.|.d...r.g.}.d
+000037f0: 057d 077c 05a0 15a1 007d 087c 0844 005d  .}.|.....}.|.D.]
+00003800: 407d 097c 00a0 167c 09a1 017d 0a7c 0a6a  @}.|...|...}.|.j
+00003810: 0d74 177c 056a 0f6a 187c 096a 196a 1a64  .t.|.j.j.|.j.j.d
+00003820: 0664 0784 0064 088d 037c 0717 0064 098d  .d...d...|...d..
+00003830: 0101 0074 1b7c 0974 1c83 0272 8474 1b7c  ...t.|.t...r.t.|
+00003840: 0974 1d83 0273 847c 0a6a 0d7c 0a64 0a19  .t...s.|.j.|.d..
+00003850: 0064 0b17 0064 0c8d 0101 007c 0764 0b37  .d...d.....|.d.7
+00003860: 007d 0774 1b7c 0974 1e83 0272 8d7c 0764  .}.t.|.t...r.|.d
+00003870: 0d37 007d 077c 06a0 1f7c 0aa1 0101 0071  .7.}.|...|.....q
+00003880: 527c 067c 0464 0e3c 007c 04a0 0d74 207c  R|.|.d.<.|...t |
+00003890: 056a 0f64 0f83 02a1 0101 007c 04a0 0d74  .j.d.......|...t
+000038a0: 207c 0164 1083 02a1 0101 0074 147c 016a   |.d.......t.|.j
+000038b0: 2164 1183 0272 b47c 046a 0d64 1264 138d  !d...r.|.j.d.d..
+000038c0: 0101 0074 007c 016a 2183 0172 c574 017c  ...t.|.j!..r.t.|
+000038d0: 016a 2174 2283 0272 c57c 046a 0d64 1264  .j!t"..r.|.j.d.d
+000038e0: 148d 0101 007c 016a 2364 0075 0172 d27c  .....|.j#d.u.r.|
+000038f0: 00a0 247c 016a 23a1 017c 0464 153c 007c  ..$|.j#..|.d.<.|
+00003900: 016a 2564 0075 0172 e77c 016a 25a0 26a1  .j%d.u.r.|.j%.&.
+00003910: 007d 0b7c 0b64 0075 0172 e77c 046a 0d7c  .}.|.d.u.r.|.j.|
+00003920: 0b6a 2764 168d 0101 007c 016a 2872 f37c  .j'd.....|.j(r.|
+00003930: 046a 0d74 297c 016a 2883 0164 178d 0101  .j.t)|.j(..d....
+00003940: 0074 2a7c 0164 1864 0083 037d 0c7c 0c64  .t*|.d.d...}.|.d
+00003950: 0075 0190 0172 057c 046a 0d7c 0c6a 2764  .u...r.|.j.|.j'd
+00003960: 198d 0101 0074 2a7c 0164 1a64 0083 037d  .....t*|.d.d...}
+00003970: 0d7c 0d64 0075 0190 0172 177c 046a 0d7c  .|.d.u...r.|.j.|
+00003980: 0d6a 2764 1b8d 0101 0074 2a7c 016a 2164  .j'd.....t*|.j!d
+00003990: 1c69 0083 037d 0e7c 0e90 0172 2e7c 046a  .i...}.|...r.|.j
+000039a0: 0d64 1d64 1e84 007c 0ea0 2ba1 0044 0083  .d.d...|..+..D..
+000039b0: 0164 1f8d 0101 0074 106a 11a0 2c64 20a1  .d.....t.j..,d .
+000039c0: 0190 0172 5174 2a7c 0164 2164 0083 0364  ...rQt*|.d!d...d
+000039d0: 0075 0190 0172 5174 147c 016a 2164 2283  .u...rQt.|.j!d".
+000039e0: 0290 0172 517c 046a 0d74 2d6a 2ea0 2f7c  ...rQ|.j.t-j../|
+000039f0: 016a 21a1 016a 3064 238d 0101 0064 2444  .j!..j0d#....d$D
+00003a00: 005d 177d 0f74 2a7c 017c 0f64 0083 037d  .].}.t*|.|.d...}
+00003a10: 107c 1064 0075 0190 0172 697c 04a0 0d7c  .|.d.u...ri|...|
+00003a20: 0f7c 106a 316a 3269 01a1 0101 0090 0171  .|.j1j2i.......q
+00003a30: 537c 016a 3364 0075 0190 0172 8f7c 046a  S|.j3d.u...r.|.j
+00003a40: 0d7c 016a 336a 2764 2564 2684 007c 016a  .|.j3j'd%d&..|.j
+00003a50: 336a 346a 3544 0083 0164 278d 0201 0074  3j4j5D...d'....t
+00003a60: 147c 0164 2883 0290 0172 8f7c 046a 0d7c  .|.d(....r.|.j.|
+00003a70: 016a 3664 298d 0101 007c 0453 0029 2a4e  .j6d)....|.S.)*N
+00003a80: 2905 da02 6964 7231 0100 0072 9600 0000  )...idr1...r....
+00003a90: da05 736c 6176 65da 0865 6469 7461 626c  ..slave..editabl
+00003aa0: 6529 0172 3201 0000 7a0f 2573 2068 6173  e).r2...z.%s has
+00003ab0: 206e 6f20 7374 6f72 65da 0b67 6574 5f63   no store..get_c
+00003ac0: 6f6c 756d 6e73 7201 0000 0063 0100 0000  olumnsr....c....
+00003ad0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00003ae0: 5300 0000 7306 0000 007c 006a 0053 0072  S...s....|.j.S.r
+00003af0: 3b00 0000 a901 7253 0000 00a9 0172 8d00  ;.....rS.....r..
+00003b00: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
+00003b10: 0072 3901 0000 7102 0000 7302 0000 0006  .r9...q...s.....
+00003b20: 007a 2552 656e 6465 7265 722e 6163 746f  .z%Renderer.acto
+00003b30: 7232 6a73 6f6e 2e3c 6c6f 6361 6c73 3e2e  r2json.<locals>.
+00003b40: 3c6c 616d 6264 613e 723a 0100 0029 01da  <lambda>r:...)..
+00003b50: 0c66 6965 6c64 735f 696e 6465 7872 4601  .fields_indexrF.
+00003b60: 0000 722d 0000 0029 01da 1366 6965 6c64  ..r-...)...field
+00003b70: 735f 696e 6465 785f 6869 6464 656e e902  s_index_hidden..
+00003b80: 0000 00da 0363 6f6c da08 706b 5f69 6e64  .....col..pk_ind
+00003b90: 6578 7ad0 7072 6576 6965 775f 6c69 6d69  exz.preview_limi
+00003ba0: 7420 7573 655f 6465 7461 696c 5f70 6172  t use_detail_par
+00003bb0: 616d 5f70 616e 656c 2075 7365 5f64 6574  am_panel use_det
+00003bc0: 6169 6c5f 7061 7261 6d73 5f76 616c 7565  ail_params_value
+00003bd0: 2068 6964 655f 6e61 7669 6761 746f 7220   hide_navigator 
+00003be0: 7573 655f 6465 7461 696c 5f70 6172 616d  use_detail_param
+00003bf0: 735f 7661 6c75 6520 7265 6163 745f 7265  s_value react_re
+00003c00: 7370 6f6e 7369 7665 206d 6178 5f72 656e  sponsive max_ren
+00003c10: 6465 725f 6465 7074 6820 7369 6d70 6c65  der_depth simple
+00003c20: 5f73 6c61 7665 6772 6964 5f68 6561 6465  _slavegrid_heade
+00003c30: 7220 7061 6769 6e61 746f 725f 7465 6d70  r paginator_temp
+00003c40: 6c61 7465 2068 6964 655f 746f 705f 746f  late hide_top_to
+00003c50: 6f6c 6261 7220 6869 6465 5f69 665f 656d  olbar hide_if_em
+00003c60: 7074 7920 da04 6669 6c65 5429 01da 0d63  pty ..fileT)...c
+00003c70: 6f6e 7461 696e 5f6d 6564 6961 2901 da09  ontain_media)...
+00003c80: 6564 6974 5f73 6166 6572 3c01 0000 7225  edit_safer<...r%
+00003c90: 0100 0029 01da 0d61 6374 6976 655f 6669  ...)...active_fi
+00003ca0: 656c 6473 da0b 6361 7264 5f6c 6179 6f75  elds..card_layou
+00003cb0: 7429 0172 4f01 0000 da0b 6c69 7374 5f6c  t).rO.....list_l
+00003cc0: 6179 6f75 7429 0172 5001 0000 da0e 5f63  ayout).rP....._c
+00003cd0: 686f 6f73 6572 735f 6469 6374 6301 0000  hoosers_dictc...
+00003ce0: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00003cf0: 0053 0000 0073 2200 0000 6900 7c00 5d0d  .S...s"...i.|.].
+00003d00: 5c02 7d01 7d02 7c01 6400 6401 8400 7c02  \.}.}.|.d.d...|.
+00003d10: 6a00 4400 8301 9302 7102 5300 2902 6301  j.D.....q.S.).c.
+00003d20: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00003d30: 0000 0053 0000 00f3 1200 0000 6700 7c00  ...S........g.|.
+00003d40: 5d05 7d01 7c01 6a00 9102 7102 5300 7237  ].}.|.j...q.S.r7
+00003d50: 0000 0072 4401 0000 2902 7247 0000 00da  ...rD...).rG....
+00003d60: 0263 6672 3700 0000 7237 0000 0072 3800  .cfr7...r7...r8.
+00003d70: 0000 7249 0000 00aa 0200 00f3 0200 0000  ..rI............
+00003d80: 1200 7a32 5265 6e64 6572 6572 2e61 6374  ..z2Renderer.act
+00003d90: 6f72 326a 736f 6e2e 3c6c 6f63 616c 733e  or2json.<locals>
+00003da0: 2e3c 6469 6374 636f 6d70 3e2e 3c6c 6973  .<dictcomp>.<lis
+00003db0: 7463 6f6d 703e 2901 da0e 636f 6e74 6578  tcomp>)...contex
+00003dc0: 745f 6669 656c 6473 2903 7247 0000 00da  t_fields).rG....
+00003dd0: 0266 6e72 4800 0000 7237 0000 0072 3700  .fnrH...r7...r7.
+00003de0: 0000 7238 0000 0072 4d00 0000 aa02 0000  ..r8...rM.......
+00003df0: 7306 0000 0006 0006 0116 ff7a 2752 656e  s..........z'Ren
+00003e00: 6465 7265 722e 6163 746f 7232 6a73 6f6e  derer.actor2json
+00003e10: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00003e20: 6f6d 703e 2901 da0c 6368 6f6f 7365 725f  omp>)...chooser_
+00003e30: 6469 6374 da0c 636f 6e74 656e 7474 7970  dict..contenttyp
+00003e40: 6573 da05 6d6f 6465 6cda 055f 6d65 7461  es..model.._meta
+00003e50: 2901 da0c 636f 6e74 656e 745f 7479 7065  )...content_type
+00003e60: 2903 da0d 6465 7461 696c 5f61 6374 696f  )...detail_actio
+00003e70: 6eda 0d69 6e73 6572 745f 6163 7469 6f6e  n..insert_action
+00003e80: da0e 6465 6661 756c 745f 6163 7469 6f6e  ..default_action
+00003e90: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00003ea0: 0003 0000 0053 0000 0072 5201 0000 7237  .....S...rR...r7
+00003eb0: 0000 0072 4401 0000 2902 7247 0000 0072  ...rD...).rG...r
+00003ec0: 8d00 0000 7237 0000 0072 3700 0000 7238  ....r7...r7...r8
+00003ed0: 0000 0072 4900 0000 ba02 0000 7254 0100  ...rI.......rT..
+00003ee0: 007a 2752 656e 6465 7265 722e 6163 746f  .z'Renderer.acto
+00003ef0: 7232 6a73 6f6e 2e3c 6c6f 6361 6c73 3e2e  r2json.<locals>.
+00003f00: 3c6c 6973 7463 6f6d 703e 2902 da0d 7061  <listcomp>)...pa
+00003f10: 7261 6d73 5f6c 6179 6f75 74da 0d70 6172  rams_layout..par
+00003f20: 616d 735f 6669 656c 6473 da10 7061 7261  ams_fields..para
+00003f30: 6d73 5f70 616e 656c 5f70 6f73 2901 7261  ms_panel_pos).ra
+00003f40: 0100 0029 3772 2c00 0000 72b6 0000 0072  ...)7r,...r....r
+00003f50: 1b00 0000 7238 0100 00da 0d5f 6163 7469  ....r8....._acti
+00003f60: 6f6e 735f 6c69 7374 7271 0000 0072 f100  ons_listrq...r..
+00003f70: 0000 da0f 6765 745f 6163 746f 725f 6c61  ....get_actor_la
+00003f80: 6265 6cda 0462 6f6f 6cda 066d 6173 7465  bel..bool..maste
+00003f90: 72da 0c68 6964 655f 6564 6974 696e 6772  r..hide_editingr
+00003fa0: 2900 0000 72d3 0000 0072 7700 0000 da0a  )...r....rw.....
+00003fb0: 6765 745f 6861 6e64 6c65 da05 7374 6f72  get_handle..stor
+00003fc0: 6572 0400 0000 726f 0000 00da 066c 6f67  er....ro.....log
+00003fd0: 6765 72da 0777 6172 6e69 6e67 7283 0000  ger..warningr...
+00003fe0: 0072 4301 0000 72ab 0000 0072 3900 0000  .rC...r....r9...
+00003ff0: da0b 6c69 7374 5f66 6965 6c64 7372 b800  ..list_fieldsr..
+00004000: 0000 7253 0000 0072 a100 0000 721f 0000  ..rS...r....r...
+00004010: 0072 2000 0000 7222 0000 0072 2e01 0000  .r ...r"...r....
+00004020: 7228 0000 0072 5901 0000 722b 0000 0072  r(...rY...r+...r
+00004030: 3c01 0000 723f 0100 0072 5c01 0000 da11  <...r?...r\.....
+00004040: 6765 745f 7769 6e64 6f77 5f6c 6179 6f75  get_window_layou
+00004050: 7472 8800 0000 724e 0100 0072 7800 0000  tr....rN...rx...
+00004060: 7203 0100 0072 6800 0000 7276 0000 0072  r....rh...rv...r
+00004070: 0e00 0000 da07 6f62 6a65 6374 73da 0d67  ......objects..g
+00004080: 6574 5f66 6f72 5f6d 6f64 656c 72da 0000  et_for_modelr...
+00004090: 0072 6c00 0000 724e 0000 0072 5f01 0000  .rl...rN...r_...
+000040a0: da0c 7061 7261 6d73 5f73 746f 7265 da0c  ..params_store..
+000040b0: 7061 7261 6d5f 6669 656c 6473 7261 0100  param_fieldsra..
+000040c0: 0029 1172 4000 0000 72a6 0000 00da 0261  .).r@...r......a
+000040d0: 6cda 0268 6b72 a700 0000 da02 6168 da07  l..hkr......ah..
+000040e0: 636f 6c75 6d6e 73da 0969 6e64 6578 5f6d  columns..index_m
+000040f0: 6f64 da09 636f 6c5f 656c 656d 7372 4901  od..col_elemsrI.
+00004100: 0000 720d 0100 00da 0277 6c72 4f01 0000  ..r......wlrO...
+00004110: 7250 0100 0072 5701 0000 72b9 0000 0072  rP...rW...r....r
+00004120: 9000 0000 7237 0000 0072 3700 0000 7238  ....r7...r7...r8
+00004130: 0000 00da 0a61 6374 6f72 326a 736f 6e58  .....actor2jsonX
+00004140: 0200 0073 9200 0000 1601 1001 0601 0201  ...s............
+00004150: 0601 0801 0c01 06fc 0807 0c01 0802 0a01  ................
+00004160: 1201 0a03 0401 0401 0801 0801 0a01 1201  ................
+00004170: 0601 04ff 0201 08ff 1402 1403 0801 0a01  ................
+00004180: 0801 0c01 0801 1205 1001 0c0d 0c01 1602  ................
+00004190: 0c01 0a02 1001 0a02 0a01 0801 0e01 0602  ................
+000041a0: 1201 0c02 0a01 0e01 0c02 0a01 0e02 0e03  ................
+000041b0: 0601 0a01 0601 0aff 2603 0201 06ff 1803  ........&.......
+000041c0: 0801 0c01 0a01 1201 0480 0c02 0402 0601  ................
+000041d0: 1201 06fe 0c04 0e01 0401 7a13 5265 6e64  ..........z.Rend
+000041e0: 6572 6572 2e61 6374 6f72 326a 736f 6e63  erer.actor2jsonc
+000041f0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00004200: 0600 0000 0300 0000 7364 0000 0064 0188  ........sd...d..
+00004210: 015f 0088 016a 0144 005d 2289 0088 006a  ._...j.D.]"....j
+00004220: 0264 0075 0172 0e71 0674 036a 046a 0588  .d.u.r.q.t.j.j..
+00004230: 01a0 0688 006a 07a1 018e 007d 0287 0087  .....j.....}....
+00004240: 0166 0264 0264 0384 087d 0374 086a 096a  .f.d.d...}.t.j.j
+00004250: 0aa0 0b7c 027c 037c 01a1 0301 0071 0664  ...|.|.|.....q.d
+00004260: 0488 015f 0074 0c83 00a0 0d7c 01a1 0153  ..._.t.....|...S
+00004270: 0029 054e 5463 0100 0000 0000 0000 0000  .).NTc..........
+00004280: 0000 0100 0000 0600 0000 1300 0000 7318  ..............s.
+00004290: 0000 007c 00a0 0074 0188 01a0 0288 00a1  ...|...t........
+000042a0: 0183 01a1 0101 0064 0053 0072 3b00 0000  .......d.S.r;...
+000042b0: 2903 728c 0000 0072 2600 0000 7278 0100  ).r....r&...rx..
+000042c0: 0072 4501 0000 a902 7299 0000 0072 4000  .rE.....r....r@.
+000042d0: 0000 7237 0000 0072 3800 0000 728c 0000  ..r7...r8...r...
+000042e0: 00c9 0200 0073 0200 0000 1801 7a26 5265  .....s......z&Re
+000042f0: 6e64 6572 6572 2e62 7569 6c64 5f6a 735f  nderer.build_js_
+00004300: 6361 6368 652e 3c6c 6f63 616c 733e 2e77  cache.<locals>.w
+00004310: 7269 7465 4629 0e72 6e00 0000 726a 0000  riteF).rn...rj..
+00004320: 00da 0f67 6574 5f68 616e 646c 655f 6e61  ...get_handle_na
+00004330: 6d65 727d 0000 00da 0470 6174 68da 046a  mer}.....path..j
+00004340: 6f69 6e72 2401 0000 72f1 0000 0072 0400  oinr$...r....r..
+00004350: 0000 726f 0000 0072 2300 0000 da0f 6d61  ..ro...r#.....ma
+00004360: 6b65 5f63 6163 6865 5f66 696c 6572 3c00  ke_cache_filer<.
+00004370: 0000 da0e 6275 696c 645f 6a73 5f63 6163  ....build_js_cac
+00004380: 6865 2904 7240 0000 00da 0566 6f72 6365  he).r@.....force
+00004390: 7256 0100 0072 8c00 0000 7242 0000 0072  rV...r....rB...r
+000043a0: 7901 0000 7238 0000 0072 7e01 0000 c002  y...r8...r~.....
+000043b0: 0000 7312 0000 0006 020a 020a 0102 0114  ..s.............
+000043c0: 010e 0214 0306 020c 017a 1752 656e 6465  .........z.Rende
+000043d0: 7265 722e 6275 696c 645f 6a73 5f63 6163  rer.build_js_cac
+000043e0: 6865 723b 0000 0029 2072 b500 0000 da0a  her;...) r......
+000043f0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00004400: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00004410: 5fda 0e69 735f 696e 7465 7261 6374 6976  _..is_interactiv
+00004420: 65da 0863 616e 5f61 7574 6872 1f01 0000  e..can_authr....
+00004430: 7223 0100 00da 1873 7570 706f 7274 5f64  r#.....support_d
+00004440: 6173 6862 6f61 7264 5f6c 6179 6f75 7472  ashboard_layoutr
+00004450: 3d00 0000 7294 0000 0072 4f00 0000 7287  =...r....rO...r.
+00004460: 0000 0072 ab00 0000 72ba 0000 0072 d000  ...r....r....r..
+00004470: 0000 72dd 0000 0072 e400 0000 72a5 0000  ..r....r....r...
+00004480: 0072 e000 0000 723f 0000 0072 ff00 0000  .r....r?...r....
+00004490: 7200 0100 0072 0101 0000 7215 0100 0072  r....r....r....r
+000044a0: 1b01 0000 7224 0100 0072 3801 0000 723f  ....r$...r8...r?
+000044b0: 0100 0072 7801 0000 727e 0100 00da 0d5f  ...rx...r~....._
+000044c0: 5f63 6c61 7373 6365 6c6c 5f5f 7237 0000  _classcell__r7..
+000044d0: 0072 3700 0000 7242 0000 0072 3800 0000  .r7...rB...r8...
+000044e0: 723a 0000 003b 0000 0073 3c00 0000 0800  r:...;...s<.....
+000044f0: 0401 0403 0401 0402 0401 0401 0c02 0804  ................
+00004500: 0857 081d 0808 0820 0803 0a18 0212 0aff  .W..... ........
+00004510: 0815 080e 0821 084e 080e 080a 082a 0809  .....!.N.....*..
+00004520: 080f 080a 0844 080c 1468 723a 0000 0072  .....D...hr:...r
+00004530: 3b00 0000 2948 727d 0000 00da 0770 6174  ;...)Hr}.....pat
+00004540: 686c 6962 7202 0000 00da 0468 746d 6c72  hlibr......htmlr
+00004550: 0300 0000 da0b 646a 616e 676f 2e63 6f6e  ......django.con
+00004560: 6672 0400 0000 da09 646a 616e 676f 2e64  fr......django.d
+00004570: 6272 0500 0000 da11 646a 616e 676f 2e75  br......django.u
+00004580: 7469 6c73 2e74 6578 7472 0600 0000 da0c  tils.textr......
+00004590: 646a 616e 676f 2e75 7469 6c73 7207 0000  django.utilsr...
+000045a0: 00da 126c 696e 6f2e 636f 7265 2e72 656e  ...lino.core.ren
+000045b0: 6465 7265 7272 0800 0000 7209 0000 00da  dererr....r.....
+000045c0: 0f6c 696e 6f2e 636f 7265 2e6d 656e 7573  .lino.core.menus
+000045d0: 720a 0000 0072 0b00 0000 da09 6c69 6e6f  r....r......lino
+000045e0: 2e63 6f72 6572 0c00 0000 720d 0000 00da  .corer....r.....
+000045f0: 0e6c 696e 6f2e 636f 7265 2e67 666b 7372  .lino.core.gfksr
+00004600: 0e00 0000 da1e 6c69 6e6f 2e6d 6f64 6c69  ......lino.modli
+00004610: 622e 6578 746a 732e 6578 745f 7265 6e64  b.extjs.ext_rend
+00004620: 6572 6572 720f 0000 00da 116c 696e 6f2e  ererr......lino.
+00004630: 636f 7265 2e61 6374 696f 6e73 7210 0000  core.actionsr...
+00004640: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00004650: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00004660: 1700 0000 da15 6c69 6e6f 2e63 6f72 652e  ......lino.core.
+00004670: 626f 756e 6461 6374 696f 6e72 1800 0000  boundactionr....
+00004680: da15 6c69 6e6f 2e63 6f72 652e 6368 6f69  ..lino.core.choi
+00004690: 6365 6c69 7374 7372 1900 0000 da1e 6c69  celistsr......li
+000046a0: 6e6f 2e6d 6f64 6c69 622e 7379 7374 656d  no.modlib.system
+000046b0: 2e63 686f 6963 656c 6973 7473 721a 0000  .choicelistsr...
+000046c0: 00da 106c 696e 6f2e 636f 7265 2e61 6374  ...lino.core.act
+000046d0: 6f72 7372 1b00 0000 da11 6c69 6e6f 2e63  orsr......lino.c
+000046e0: 6f72 652e 6c61 796f 7574 7372 1c00 0000  ore.layoutsr....
+000046f0: 721d 0000 00da 0f6c 696e 6f2e 636f 7265  r......lino.core
+00004700: 2e65 6c65 6d73 721e 0000 0072 1f00 0000  .elemsr....r....
+00004710: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
+00004720: 2300 0000 da0a 6574 6765 6e2e 6874 6d6c  #.....etgen.html
+00004730: 7224 0000 00da 0a6c 696e 6f2e 7574 696c  r$.....lino.util
+00004740: 7372 2500 0000 da10 6c69 6e6f 2e75 7469  sr%.....lino.uti
+00004750: 6c73 2e6a 7367 656e 7226 0000 0072 2700  ls.jsgenr&...r'.
+00004760: 0000 7228 0000 00da 176c 696e 6f2e 6d6f  ..r(.....lino.mo
+00004770: 646c 6962 2e75 7365 7273 2e75 7469 6c73  dlib.users.utils
+00004780: 7229 0000 0072 2a00 0000 da19 6c69 6e6f  r)...r*.....lino
+00004790: 2e6d 6f64 6c69 622e 7379 7374 656d 2e6d  .modlib.system.m
+000047a0: 6978 696e 7372 2b00 0000 da07 696e 7370  ixinsr+.....insp
+000047b0: 6563 7472 2c00 0000 da05 6963 6f6e 7372  ectr,.....iconsr
+000047c0: 2e00 0000 7239 0000 0072 3a00 0000 7237  ....r9...r:...r7
+000047d0: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
+000047e0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000047f0: 733c 0000 0008 040c 010c 010c 010c 010c  s<..............
+00004800: 010c 0110 0210 020c 010c 010c 010c 0128  ...............(
+00004810: 020c 030c 010c 010c 0110 011c 010c 020c  ................
+00004820: 020c 0214 0110 020c 010c 020c 020a 0314  ................
+00004830: 0d                                       .
```

### Comparing `lino_react-23.7.1/lino_react/react/__pycache__/views.cpython-310.pyc` & `lino_react-23.7.2/lino_react/react/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/config/react/main.html` & `lino_react-23.7.2/lino_react/react/config/react/main.html`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/config/react/service-worker.js` & `lino_react-23.7.2/lino_react/react/config/react/service-worker.js`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/icons.py` & `lino_react-23.7.2/lino_react/react/icons.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/renderer.py` & `lino_react-23.7.2/lino_react/react/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,17 @@
                 suggestors=list(plugins.memo.parser.suggesters.keys()))
 
         # if settings.SITE.never_build_site_cache:
         #     data.update(revision_number=settings.SITE.kernel.lino_version)
         # else:
         data.update(revision_number=settings.SITE.kernel.code_mtime)
         try:
-            data.update(mjs_timestamp=os.stat(Path(settings.STATIC_ROOT) / 'react' / 'main.js').st_mtime)
+            data[constants.URL_PARAM_MAIN_JS_TIMESTAMP] = os.stat(
+                Path(settings.STATIC_ROOT) / 'react' / 'main.js'
+            ).st_mtime
         except FileNotFoundError:
             pass
 
         if hasattr(settings.SITE, 'theme_name'):
             data.update(theme_name=settings.SITE.theme_name)
 
         if settings.SITE.user_model == None:
```

### Comparing `lino_react-23.7.1/lino_react/react/static/media/color.6441e63a.png` & `lino_react-23.7.2/lino_react/react/static/media/color.6441e63a.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/media/color.c7a33805.png` & `lino_react-23.7.2/lino_react/react/static/media/color.c7a33805.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/media/line.567f5738.gif` & `lino_react-23.7.2/lino_react/react/static/media/line.567f5738.gif`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/media/primeicons.2d2afb27.eot` & `lino_react-23.7.2/lino_react/react/static/media/primeicons.2d2afb27.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/media/primeicons.3a0d4a58.ttf` & `lino_react-23.7.2/lino_react/react/static/media/primeicons.3a0d4a58.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/media/primeicons.66ee0deb.woff` & `lino_react-23.7.2/lino_react/react/static/media/primeicons.66ee0deb.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/media/primeicons.c55d94a2.svg` & `lino_react-23.7.2/lino_react/react/static/media/primeicons.c55d94a2.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/media/primeicons.df0140f8.ttf` & `lino_react-23.7.2/lino_react/react/static/media/primeicons.df0140f8.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/media/primeicons.dfbfef2d.eot` & `lino_react-23.7.2/lino_react/react/static/media/primeicons.dfbfef2d.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/media/primeicons.e5e0e944.svg` & `lino_react-23.7.2/lino_react/react/static/media/primeicons.e5e0e944.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/media/primeicons.e61f3495.woff` & `lino_react-23.7.2/lino_react/react/static/media/primeicons.e61f3495.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/static/react/main.js` & `lino_react-23.7.2/lino_react/react/static/react/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5472,15 +5472,15 @@
                                 page: h.page,
                                 query: h.query,
                                 sortFieldName: h.sortFieldName,
                                 sortOrder: h.sortOrder,
                                 topRow: h.page * this.data.rowsPerPage
                             });
                             var m = {};
-                            if (m[me.i5] = me.oi, m[me.qg] = h.page * this.data.rowsPerPage, m[me.EL] = this.data.rowsPerPage, m[me.Vk] = h.query, m[me.mQ] = this.rp || c()(this), m[me.Vp] = h.displayMode, m[me.$S] = me.zf, m[me.xX] = window.App.state.site_data.revision_number, m[me.fH] = window.App.data.selectedLanguage || window.App.state.user_settings.lang, m[me.jT] = window.App.state.site_data.mjsts, void 0 !== h.sortFieldName && (m.sort = h.sortFieldName), 0 !== h.sortOrder && (m.dir = 1 === h.sortOrder ? "ASC" : "DESC"), this.props.actorData.use_detail_params_value && this.props.parent_pv) m.pv = (0, x.ku)(this.props.parent_pv, this.props.actorData.params_fields);
+                            if (m[me.i5] = me.oi, m[me.qg] = h.page * this.data.rowsPerPage, m[me.EL] = this.data.rowsPerPage, m[me.Vk] = h.query, m[me.mQ] = this.rp || c()(this), m[me.Vp] = h.displayMode, m[me.$S] = me.zf, m[me.xX] = window.App.state.site_data.revision_number, m[me.fH] = window.App.data.selectedLanguage || window.App.state.user_settings.lang, m[me.jT] = window.App.state.site_data[me.jT], void 0 !== h.sortFieldName && (m.sort = h.sortFieldName), 0 !== h.sortOrder && (m.dir = 1 === h.sortOrder ? "ASC" : "DESC"), this.props.actorData.use_detail_params_value && this.props.parent_pv) m.pv = (0, x.ku)(this.props.parent_pv, this.props.actorData.params_fields);
                             else if (this.props.actorData.params_layout) {
                                 var b = g.parse(this.props.router.history.location.search);
                                 this.props.inDetail || void 0 !== a || 0 !== Object.keys(this.data.params_values).length ? 0 !== Object.keys(this.data.params_values).length && (m.pv = (0, x.ku)(a || this.data.params_values, this.props.actorData.params_fields)) : m.pv = b.pv
                             }
                             return void 0 !== this.props.mk && null !== this.props.mt && (m.mk = this.props.mk), void 0 !== this.props.mt && null !== this.props.mt && (m.mt = this.props.mt), window.App.add_su(m), m
                         }
                     }, {
@@ -5646,15 +5646,15 @@
                                 return !i.includes(e.fields_index)
                             })).forEach((function(e) {
                                 n.push(e.name), e.width ? o.push(e.width) : o.push(15)
                             })), n.forEach((function(e) {
                                 r.push(t.filter((function(t) {
                                     return t.name === e
                                 }))[0].hidden)
-                            })), e[me.Td] = n, e[me.SX] = r, e[me.EO] = o, e
+                            })), e[me.Td] = n, e[me.SX] = r, e[me.EO] = o, e[me.ks] = (0, x.ku)(this.data.params_values, this.props.actorData.params_fields), e
                         }
                     }, {
                         key: "render",
                         value: function() {
                             var e = this,
                                 t = "l-grid ";
                             if ("whitewall" === window.App.data.themeName && (t += "l-whitewall-body "), this.props.actorData.hide_if_empty && this.props.inDetail && 0 === this.data.rows.length) return null;
@@ -10984,19 +10984,20 @@
                     Jg: () => b,
                     Vk: () => g,
                     qg: () => v,
                     EL: () => y,
                     i5: () => w,
                     oi: () => _,
                     mQ: () => k,
-                    fH: () => x,
-                    EO: () => E,
-                    SX: () => O,
-                    Td: () => C,
-                    X8: () => S
+                    ks: () => x,
+                    fH: () => E,
+                    EO: () => O,
+                    SX: () => C,
+                    Td: () => S,
+                    X8: () => D
                 });
                 var o = "lv",
                     r = "mjsts",
                     i = "wt",
                     a = "d",
                     l = "p",
                     s = "dm",
@@ -11010,19 +11011,20 @@
                     b = "html",
                     g = "query",
                     v = "start",
                     y = "limit",
                     w = "fmt",
                     _ = "json",
                     k = "rp",
-                    x = "ul",
-                    E = "cw",
-                    O = "ch",
-                    C = "ci",
-                    S = ["submit_detail", "delete_selected"]
+                    x = "pv",
+                    E = "ul",
+                    O = "cw",
+                    C = "ch",
+                    S = "ci",
+                    D = ["submit_detail", "delete_selected"]
             },
             7002: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     C: () => K,
                     q: () => W
                 });
```

### Comparing `lino_react-23.7.1/lino_react/react/static/react/main.js.LICENSE.txt` & `lino_react-23.7.2/lino_react/react/static/react/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/react/views.py` & `lino_react-23.7.2/lino_react/react/views.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.1/lino_react/setup_info.py` & `lino_react-23.7.2/lino_react/setup_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 SETUP_INFO = dict(
     name='lino_react',
-    version='23.7.1',
+    version='23.7.2',
     install_requires=['lino'],
     tests_require=[],
     test_suite='tests',
     description="The React front end for Lino",
     license_files=['COPYING'],
     include_package_data=False,
     zip_safe=False,
```

### Comparing `lino_react-23.7.1/lino_react.egg-info/PKG-INFO` & `lino_react-23.7.2/lino_react.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-react
-Version: 23.7.1
+Version: 23.7.2
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier:   Programming Language :: Python
```

### Comparing `lino_react-23.7.1/lino_react.egg-info/SOURCES.txt` & `lino_react-23.7.2/lino_react.egg-info/SOURCES.txt`

 * *Files identical despite different names*

