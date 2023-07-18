# Comparing `tmp/transitle-0.0.1.tar.gz` & `tmp/transitle-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transitle-0.0.1.tar", last modified: Tue Jul 18 09:28:53 2023, max compression
+gzip compressed data, was "transitle-1.0.0.tar", last modified: Tue Jul 18 12:28:20 2023, max compression
```

## Comparing `transitle-0.0.1.tar` & `transitle-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2023-07-18 09:28:53.785618 transitle-0.0.1/
--rw-r--r--   0 mesutgunes   (501) staff       (20)    35149 2023-07-17 14:35:41.000000 transitle-0.0.1/LICENSE
--rw-r--r--   0 mesutgunes   (501) staff       (20)      373 2023-07-18 09:28:53.785333 transitle-0.0.1/PKG-INFO
--rw-r--r--   0 mesutgunes   (501) staff       (20)     2371 2023-07-18 09:24:28.000000 transitle-0.0.1/README.md
--rw-r--r--   0 mesutgunes   (501) staff       (20)       38 2023-07-18 09:28:53.785679 transitle-0.0.1/setup.cfg
--rw-r--r--   0 mesutgunes   (501) staff       (20)      671 2023-07-18 09:14:40.000000 transitle-0.0.1/setup.py
-drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2023-07-18 09:28:53.772058 transitle-0.0.1/transitle/
--rw-r--r--   0 mesutgunes   (501) staff       (20)       60 2023-07-17 10:16:33.000000 transitle-0.0.1/transitle/__init__.py
--rw-r--r--   0 mesutgunes   (501) staff       (20)     1289 2023-07-17 10:25:19.000000 transitle-0.0.1/transitle/__main__.py
--rw-r--r--   0 mesutgunes   (501) staff       (20)     1130 2023-07-18 09:15:31.000000 transitle-0.0.1/transitle/translator.py
--rw-r--r--   0 mesutgunes   (501) staff       (20)     5938 2023-07-17 10:46:14.000000 transitle-0.0.1/transitle/ts.py
-drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2023-07-18 09:28:53.784866 transitle-0.0.1/transitle.egg-info/
--rw-r--r--   0 mesutgunes   (501) staff       (20)      373 2023-07-18 09:28:53.000000 transitle-0.0.1/transitle.egg-info/PKG-INFO
--rw-r--r--   0 mesutgunes   (501) staff       (20)      310 2023-07-18 09:28:53.000000 transitle-0.0.1/transitle.egg-info/SOURCES.txt
--rw-r--r--   0 mesutgunes   (501) staff       (20)        1 2023-07-18 09:28:53.000000 transitle-0.0.1/transitle.egg-info/dependency_links.txt
--rw-r--r--   0 mesutgunes   (501) staff       (20)       47 2023-07-18 09:28:53.000000 transitle-0.0.1/transitle.egg-info/entry_points.txt
--rw-r--r--   0 mesutgunes   (501) staff       (20)       12 2023-07-18 09:28:53.000000 transitle-0.0.1/transitle.egg-info/requires.txt
--rw-r--r--   0 mesutgunes   (501) staff       (20)       10 2023-07-18 09:28:53.000000 transitle-0.0.1/transitle.egg-info/top_level.txt
+drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2023-07-18 12:28:20.864143 transitle-1.0.0/
+-rw-r--r--   0 mesutgunes   (501) staff       (20)    35149 2023-07-17 14:35:41.000000 transitle-1.0.0/LICENSE
+-rw-r--r--   0 mesutgunes   (501) staff       (20)      527 2023-07-18 12:28:20.863785 transitle-1.0.0/PKG-INFO
+-rw-r--r--   0 mesutgunes   (501) staff       (20)      346 2023-07-18 12:26:59.000000 transitle-1.0.0/README.rst
+-rw-r--r--   0 mesutgunes   (501) staff       (20)       38 2023-07-18 12:28:20.864229 transitle-1.0.0/setup.cfg
+-rw-r--r--   0 mesutgunes   (501) staff       (20)     1262 2023-07-18 12:28:13.000000 transitle-1.0.0/setup.py
+drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2023-07-18 12:28:20.854307 transitle-1.0.0/transitle/
+-rw-r--r--   0 mesutgunes   (501) staff       (20)       60 2023-07-17 10:16:33.000000 transitle-1.0.0/transitle/__init__.py
+-rw-r--r--   0 mesutgunes   (501) staff       (20)     1289 2023-07-17 10:25:19.000000 transitle-1.0.0/transitle/__main__.py
+-rw-r--r--   0 mesutgunes   (501) staff       (20)     1130 2023-07-18 09:15:31.000000 transitle-1.0.0/transitle/translator.py
+-rw-r--r--   0 mesutgunes   (501) staff       (20)     5938 2023-07-17 10:46:14.000000 transitle-1.0.0/transitle/ts.py
+drwxr-xr-x   0 mesutgunes   (501) staff       (20)        0 2023-07-18 12:28:20.863305 transitle-1.0.0/transitle.egg-info/
+-rw-r--r--   0 mesutgunes   (501) staff       (20)      527 2023-07-18 12:28:20.000000 transitle-1.0.0/transitle.egg-info/PKG-INFO
+-rw-r--r--   0 mesutgunes   (501) staff       (20)      311 2023-07-18 12:28:20.000000 transitle-1.0.0/transitle.egg-info/SOURCES.txt
+-rw-r--r--   0 mesutgunes   (501) staff       (20)        1 2023-07-18 12:28:20.000000 transitle-1.0.0/transitle.egg-info/dependency_links.txt
+-rw-r--r--   0 mesutgunes   (501) staff       (20)       47 2023-07-18 12:28:20.000000 transitle-1.0.0/transitle.egg-info/entry_points.txt
+-rw-r--r--   0 mesutgunes   (501) staff       (20)       12 2023-07-18 12:28:20.000000 transitle-1.0.0/transitle.egg-info/requires.txt
+-rw-r--r--   0 mesutgunes   (501) staff       (20)       10 2023-07-18 12:28:20.000000 transitle-1.0.0/transitle.egg-info/top_level.txt
```

### Comparing `transitle-0.0.1/LICENSE` & `transitle-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transitle-0.0.1/transitle/__main__.py` & `transitle-1.0.0/transitle/__main__.py`

 * *Files identical despite different names*

### Comparing `transitle-0.0.1/transitle/translator.py` & `transitle-1.0.0/transitle/translator.py`

 * *Files identical despite different names*

### Comparing `transitle-0.0.1/transitle/ts.py` & `transitle-1.0.0/transitle/ts.py`

 * *Files identical despite different names*

