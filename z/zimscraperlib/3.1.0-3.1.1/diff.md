# Comparing `tmp/zimscraperlib-3.1.0.tar.gz` & `tmp/zimscraperlib-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimscraperlib-3.1.0.tar", last modified: Fri May  5 10:18:17 2023, max compression
+gzip compressed data, was "zimscraperlib-3.1.1.tar", last modified: Tue Jul 18 18:19:26 2023, max compression
```

## Comparing `zimscraperlib-3.1.0.tar` & `zimscraperlib-3.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.286519 zimscraperlib-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-05 10:18:17.286519 zimscraperlib-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:18:17.286519 zimscraperlib-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.266518 zimscraperlib-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.274518 zimscraperlib-3.1.0/src/zimscraperlib/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/filesystem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/fix_ogvjs_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.278519 zimscraperlib-3.1.0/src/zimscraperlib/image/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/convertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/probing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/image/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.286519 zimscraperlib-3.1.0/src/zimscraperlib/video/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/video/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/video/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/video/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/video/probing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.286519 zimscraperlib-3.1.0/src/zimscraperlib/zim/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/_libkiwix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-05 10:18:01.000000 zimscraperlib-3.1.0/src/zimscraperlib/zim/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:18:17.278519 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 10:18:17.000000 zimscraperlib-3.1.0/src/zimscraperlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:19:26.016142 zimscraperlib-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-18 18:19:26.016142 zimscraperlib-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:19:26.016142 zimscraperlib-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:19:26.000141 zimscraperlib-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:19:26.008141 zimscraperlib-3.1.1/src/zimscraperlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/filesystem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/fix_ogvjs_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:19:26.012141 zimscraperlib-3.1.1/src/zimscraperlib/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/image/convertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/image/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/image/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/image/probing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/image/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/image/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:19:26.016142 zimscraperlib-3.1.1/src/zimscraperlib/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/video/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/video/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/video/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/video/probing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:19:26.016142 zimscraperlib-3.1.1/src/zimscraperlib/zim/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/zim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/zim/_libkiwix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/zim/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/zim/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/zim/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/zim/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/zim/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-18 18:19:14.000000 zimscraperlib-3.1.1/src/zimscraperlib/zim/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:19:26.012141 zimscraperlib-3.1.1/src/zimscraperlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-18 18:19:25.000000 zimscraperlib-3.1.1/src/zimscraperlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-18 18:19:26.000000 zimscraperlib-3.1.1/src/zimscraperlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:19:25.000000 zimscraperlib-3.1.1/src/zimscraperlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-18 18:19:25.000000 zimscraperlib-3.1.1/src/zimscraperlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:19:25.000000 zimscraperlib-3.1.1/src/zimscraperlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-18 18:19:25.000000 zimscraperlib-3.1.1/src/zimscraperlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 18:19:25.000000 zimscraperlib-3.1.1/src/zimscraperlib.egg-info/top_level.txt
```

### Comparing `zimscraperlib-3.1.0/CHANGELOG.md` & `zimscraperlib-3.1.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 ## Changelog
 
 All notable changes to this project are documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (as of version 1.5.0).
 
+## [3.1.1]
+
+### Changed
+
+- Fixed declared (hint) return type of `download.stream_file` #104
+- Fixed declared (hint) type of `content` param for `Creator.add_item_for` #107
+
 ## [3.1.0] - 2023-05-05
 
 ### Changed
 
 - Using pylibzim `3.1.0`
 - ZIM metadata check now allows multiple values (comma-separated) for `Language`
 - Using `yt_dlp` instead of `youtube_dl`
```

### Comparing `zimscraperlib-3.1.0/LICENSE` & `zimscraperlib-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/PKG-INFO` & `zimscraperlib-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimscraperlib
-Version: 3.1.0
+Version: 3.1.1
 Summary: Collection of python tools to re-use common code across scrapers
 Home-page: https://github.com/openzim/python_scraperlib
 Author: kiwix
 Author-email: reg@kiwix.org
 License: GPLv3+
 Keywords: kiwix zim offline
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zimscraperlib-3.1.0/README.md` & `zimscraperlib-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/setup.py` & `zimscraperlib-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/constants.py` & `zimscraperlib-3.1.1/src/zimscraperlib/constants.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/download.py` & `zimscraperlib-3.1.1/src/zimscraperlib/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # vim: ai ts=4 sts=4 et sw=4 nu
 
+from __future__ import annotations
+
 import io
 import pathlib
 import subprocess
 from concurrent.futures import Future, ThreadPoolExecutor
 from typing import Dict, Optional, Union
 
 import requests
@@ -170,15 +172,15 @@
     byte_stream: Optional[io.BytesIO] = None,
     block_size: Optional[int] = 1024,
     proxies: Optional[dict] = None,
     only_first_block: Optional[bool] = False,
     max_retries: Optional[int] = 5,
     headers: Optional[Dict[str, str]] = None,
     session: Optional[requests.Session] = None,
-) -> Union[int, requests.structures.CaseInsensitiveDict]:
+) -> tuple[int, requests.structures.CaseInsensitiveDict]:
     """Stream data from a URL to either a BytesIO object or a file
     Arguments -
         fpath - Path of the file where data is sent
         byte_stream - The BytesIO object where data is sent
         block_size - Size of each chunk of data read in one iteration
         proxies - A dict of proxies to be used
         https://requests.readthedocs.io/en/master/user/advanced/#proxies
```

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/filesystem.py` & `zimscraperlib-3.1.1/src/zimscraperlib/filesystem.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/fix_ogvjs_dist.py` & `zimscraperlib-3.1.1/src/zimscraperlib/fix_ogvjs_dist.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/html.py` & `zimscraperlib-3.1.1/src/zimscraperlib/html.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/i18n.py` & `zimscraperlib-3.1.1/src/zimscraperlib/i18n.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/image/convertion.py` & `zimscraperlib-3.1.1/src/zimscraperlib/image/convertion.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/image/optimization.py` & `zimscraperlib-3.1.1/src/zimscraperlib/image/optimization.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/image/presets.py` & `zimscraperlib-3.1.1/src/zimscraperlib/image/presets.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/image/probing.py` & `zimscraperlib-3.1.1/src/zimscraperlib/image/probing.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/image/transformation.py` & `zimscraperlib-3.1.1/src/zimscraperlib/image/transformation.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/inputs.py` & `zimscraperlib-3.1.1/src/zimscraperlib/inputs.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/logging.py` & `zimscraperlib-3.1.1/src/zimscraperlib/logging.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/types.py` & `zimscraperlib-3.1.1/src/zimscraperlib/types.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/uri.py` & `zimscraperlib-3.1.1/src/zimscraperlib/uri.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/video/config.py` & `zimscraperlib-3.1.1/src/zimscraperlib/video/config.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/video/encoding.py` & `zimscraperlib-3.1.1/src/zimscraperlib/video/encoding.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/video/presets.py` & `zimscraperlib-3.1.1/src/zimscraperlib/video/presets.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/video/probing.py` & `zimscraperlib-3.1.1/src/zimscraperlib/video/probing.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/zim/__init__.py` & `zimscraperlib-3.1.1/src/zimscraperlib/zim/__init__.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/zim/_libkiwix.py` & `zimscraperlib-3.1.1/src/zimscraperlib/zim/_libkiwix.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/zim/archive.py` & `zimscraperlib-3.1.1/src/zimscraperlib/zim/archive.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/zim/creator.py` & `zimscraperlib-3.1.1/src/zimscraperlib/zim/creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
         return self.config_metadata(**devel_default_metadata)
 
     def add_item_for(
         self,
         path: str,
         title: Optional[str] = None,
         fpath: Optional[pathlib.Path] = None,
-        content: Optional[bytes] = None,
+        content: Optional[Union[bytes, str]] = None,
         mimetype: Optional[str] = None,
         is_front: Optional[bool] = None,
         should_compress: Optional[bool] = None,
         delete_fpath: Optional[bool] = False,
         duplicate_ok: Optional[bool] = None,
         callback: Optional[Union[callable, Tuple[callable, Any]]] = None,
     ):
```

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/zim/filesystem.py` & `zimscraperlib-3.1.1/src/zimscraperlib/zim/filesystem.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/zim/items.py` & `zimscraperlib-3.1.1/src/zimscraperlib/zim/items.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/zim/metadata.py` & `zimscraperlib-3.1.1/src/zimscraperlib/zim/metadata.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib/zim/providers.py` & `zimscraperlib-3.1.1/src/zimscraperlib/zim/providers.py`

 * *Files identical despite different names*

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib.egg-info/PKG-INFO` & `zimscraperlib-3.1.1/src/zimscraperlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimscraperlib
-Version: 3.1.0
+Version: 3.1.1
 Summary: Collection of python tools to re-use common code across scrapers
 Home-page: https://github.com/openzim/python_scraperlib
 Author: kiwix
 Author-email: reg@kiwix.org
 License: GPLv3+
 Keywords: kiwix zim offline
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zimscraperlib-3.1.0/src/zimscraperlib.egg-info/SOURCES.txt` & `zimscraperlib-3.1.1/src/zimscraperlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

