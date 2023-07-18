# Comparing `tmp/gfx_perp_python_sdk-0.0.3.tar.gz` & `tmp/gfx_perp_python_sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfx_perp_python_sdk-0.0.3.tar", last modified: Mon Jul 17 16:35:18 2023, max compression
+gzip compressed data, was "gfx_perp_python_sdk-0.0.4.tar", last modified: Tue Jul 18 06:19:57 2023, max compression
```

## Comparing `gfx_perp_python_sdk-0.0.3.tar` & `gfx_perp_python_sdk-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:35:18.404509 gfx_perp_python_sdk-0.0.3/
--rw-r--r--   0 shashank   (501) staff       (20)     1064 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.3/LICENSE
--rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-17 16:35:18.404385 gfx_perp_python_sdk-0.0.3/PKG-INFO
--rw-r--r--   0 shashank   (501) staff       (20)       21 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.3/README.md
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:35:18.402668 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/
--rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-17 16:35:18.000000 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 shashank   (501) staff       (20)      325 2023-07-17 16:35:18.000000 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 shashank   (501) staff       (20)        1 2023-07-17 16:35:18.000000 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 shashank   (501) staff       (20)        7 2023-07-17 16:35:18.000000 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/requires.txt
--rw-r--r--   0 shashank   (501) staff       (20)       11 2023-07-17 16:35:18.000000 gfx_perp_python_sdk-0.0.3/gfx_perp_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-17 16:35:18.404085 gfx_perp_python_sdk-0.0.3/my_project/
--rw-r--r--   0 shashank   (501) staff       (20)        0 2023-07-16 08:25:37.000000 gfx_perp_python_sdk-0.0.3/my_project/__init__.py
--rw-r--r--   0 shashank   (501) staff       (20)       93 2023-07-17 12:08:31.000000 gfx_perp_python_sdk-0.0.3/my_project/perp.py
--rw-r--r--   0 shashank   (501) staff       (20)      412 2023-07-14 13:02:36.000000 gfx_perp_python_sdk-0.0.3/my_project/product.py
--rw-r--r--   0 shashank   (501) staff       (20)      549 2023-07-14 13:01:36.000000 gfx_perp_python_sdk-0.0.3/my_project/trader.py
--rw-r--r--   0 shashank   (501) staff       (20)       38 2023-07-17 16:35:18.404545 gfx_perp_python_sdk-0.0.3/setup.cfg
--rw-r--r--   0 shashank   (501) staff       (20)      383 2023-07-17 16:33:38.000000 gfx_perp_python_sdk-0.0.3/setup.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-18 06:19:57.889276 gfx_perp_python_sdk-0.0.4/
+-rw-r--r--   0 shashank   (501) staff       (20)     1064 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.4/LICENSE
+-rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-18 06:19:57.889119 gfx_perp_python_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0 shashank   (501) staff       (20)       21 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.4/README.md
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-18 06:19:57.888083 gfx_perp_python_sdk-0.0.4/gfx-perp-python-sdk/
+-rw-r--r--   0 shashank   (501) staff       (20)        0 2023-07-16 08:25:37.000000 gfx_perp_python_sdk-0.0.4/gfx-perp-python-sdk/__init__.py
+-rw-r--r--   0 shashank   (501) staff       (20)       93 2023-07-17 12:08:31.000000 gfx_perp_python_sdk-0.0.4/gfx-perp-python-sdk/perp.py
+-rw-r--r--   0 shashank   (501) staff       (20)      412 2023-07-14 13:02:36.000000 gfx_perp_python_sdk-0.0.4/gfx-perp-python-sdk/product.py
+-rw-r--r--   0 shashank   (501) staff       (20)      549 2023-07-14 13:01:36.000000 gfx_perp_python_sdk-0.0.4/gfx-perp-python-sdk/trader.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-18 06:19:57.888906 gfx_perp_python_sdk-0.0.4/gfx_perp_python_sdk.egg-info/
+-rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-18 06:19:57.000000 gfx_perp_python_sdk-0.0.4/gfx_perp_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 shashank   (501) staff       (20)      361 2023-07-18 06:19:57.000000 gfx_perp_python_sdk-0.0.4/gfx_perp_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shashank   (501) staff       (20)        1 2023-07-18 06:19:57.000000 gfx_perp_python_sdk-0.0.4/gfx_perp_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shashank   (501) staff       (20)        7 2023-07-18 06:19:57.000000 gfx_perp_python_sdk-0.0.4/gfx_perp_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 shashank   (501) staff       (20)       31 2023-07-18 06:19:57.000000 gfx_perp_python_sdk-0.0.4/gfx_perp_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 shashank   (501) staff       (20)       38 2023-07-18 06:19:57.889310 gfx_perp_python_sdk-0.0.4/setup.cfg
+-rw-r--r--   0 shashank   (501) staff       (20)      383 2023-07-18 06:17:20.000000 gfx_perp_python_sdk-0.0.4/setup.py
```

### Comparing `gfx_perp_python_sdk-0.0.3/LICENSE` & `gfx_perp_python_sdk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gfx_perp_python_sdk-0.0.3/my_project/trader.py` & `gfx_perp_python_sdk-0.0.4/gfx-perp-python-sdk/trader.py`

 * *Files identical despite different names*

