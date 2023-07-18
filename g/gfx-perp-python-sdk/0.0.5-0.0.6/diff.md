# Comparing `tmp/gfx_perp_python_sdk-0.0.5.tar.gz` & `tmp/gfx_perp_python_sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfx_perp_python_sdk-0.0.5.tar", last modified: Tue Jul 18 06:55:08 2023, max compression
+gzip compressed data, was "gfx_perp_python_sdk-0.0.6.tar", last modified: Tue Jul 18 07:08:20 2023, max compression
```

## Comparing `gfx_perp_python_sdk-0.0.5.tar` & `gfx_perp_python_sdk-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-18 06:55:08.582981 gfx_perp_python_sdk-0.0.5/
--rw-r--r--   0 shashank   (501) staff       (20)     1064 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.5/LICENSE
--rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-18 06:55:08.582834 gfx_perp_python_sdk-0.0.5/PKG-INFO
--rw-r--r--   0 shashank   (501) staff       (20)       21 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.5/README.md
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-18 06:55:08.581904 gfx_perp_python_sdk-0.0.5/gfx-perp-python-sdk/
--rw-r--r--   0 shashank   (501) staff       (20)        0 2023-07-16 08:25:37.000000 gfx_perp_python_sdk-0.0.5/gfx-perp-python-sdk/__init__.py
--rw-r--r--   0 shashank   (501) staff       (20)       93 2023-07-17 12:08:31.000000 gfx_perp_python_sdk-0.0.5/gfx-perp-python-sdk/perp.py
--rw-r--r--   0 shashank   (501) staff       (20)      412 2023-07-14 13:02:36.000000 gfx_perp_python_sdk-0.0.5/gfx-perp-python-sdk/product.py
--rw-r--r--   0 shashank   (501) staff       (20)      549 2023-07-14 13:01:36.000000 gfx_perp_python_sdk-0.0.5/gfx-perp-python-sdk/trader.py
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-18 06:55:08.582658 gfx_perp_python_sdk-0.0.5/gfx_perp_python_sdk.egg-info/
--rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-18 06:55:08.000000 gfx_perp_python_sdk-0.0.5/gfx_perp_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 shashank   (501) staff       (20)      361 2023-07-18 06:55:08.000000 gfx_perp_python_sdk-0.0.5/gfx_perp_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 shashank   (501) staff       (20)        1 2023-07-18 06:55:08.000000 gfx_perp_python_sdk-0.0.5/gfx_perp_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 shashank   (501) staff       (20)        7 2023-07-18 06:55:08.000000 gfx_perp_python_sdk-0.0.5/gfx_perp_python_sdk.egg-info/requires.txt
--rw-r--r--   0 shashank   (501) staff       (20)       20 2023-07-18 06:55:08.000000 gfx_perp_python_sdk-0.0.5/gfx_perp_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 shashank   (501) staff       (20)       38 2023-07-18 06:55:08.583035 gfx_perp_python_sdk-0.0.5/setup.cfg
--rw-r--r--   0 shashank   (501) staff       (20)      352 2023-07-18 06:54:20.000000 gfx_perp_python_sdk-0.0.5/setup.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-18 07:08:20.375545 gfx_perp_python_sdk-0.0.6/
+-rw-r--r--   0 shashank   (501) staff       (20)     1064 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.6/LICENSE
+-rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-18 07:08:20.375373 gfx_perp_python_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0 shashank   (501) staff       (20)       21 2023-07-16 07:52:04.000000 gfx_perp_python_sdk-0.0.6/README.md
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-18 07:08:20.374160 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk/
+-rw-r--r--   0 shashank   (501) staff       (20)        0 2023-07-16 08:25:37.000000 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk/__init__.py
+-rw-r--r--   0 shashank   (501) staff       (20)       93 2023-07-17 12:08:31.000000 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk/perp.py
+-rw-r--r--   0 shashank   (501) staff       (20)      412 2023-07-14 13:02:36.000000 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk/product.py
+-rw-r--r--   0 shashank   (501) staff       (20)      549 2023-07-14 13:01:36.000000 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk/trader.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-07-18 07:08:20.375155 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk.egg-info/
+-rw-r--r--   0 shashank   (501) staff       (20)      228 2023-07-18 07:08:20.000000 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 shashank   (501) staff       (20)      361 2023-07-18 07:08:20.000000 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shashank   (501) staff       (20)        1 2023-07-18 07:08:20.000000 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shashank   (501) staff       (20)        7 2023-07-18 07:08:20.000000 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 shashank   (501) staff       (20)       20 2023-07-18 07:08:20.000000 gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 shashank   (501) staff       (20)       38 2023-07-18 07:08:20.375596 gfx_perp_python_sdk-0.0.6/setup.cfg
+-rw-r--r--   0 shashank   (501) staff       (20)      360 2023-07-18 07:07:16.000000 gfx_perp_python_sdk-0.0.6/setup.py
```

### Comparing `gfx_perp_python_sdk-0.0.5/LICENSE` & `gfx_perp_python_sdk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gfx_perp_python_sdk-0.0.5/gfx-perp-python-sdk/trader.py` & `gfx_perp_python_sdk-0.0.6/gfx_perp_python_sdk/trader.py`

 * *Files identical despite different names*

