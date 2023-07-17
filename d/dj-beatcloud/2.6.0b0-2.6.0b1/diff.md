# Comparing `tmp/dj_beatcloud-2.6.0b0.tar.gz` & `tmp/dj_beatcloud-2.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.6.0b0.tar", last modified: Sat Jul 15 20:44:14 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.6.0b1.tar", last modified: Mon Jul 17 23:19:11 2023, max compression
```

## Comparing `dj_beatcloud-2.6.0b0.tar` & `dj_beatcloud-2.6.0b1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.137101 dj_beatcloud-2.6.0b0/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b0/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b0/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2575 2023-07-15 20:44:14.137210 dj_beatcloud-2.6.0b0/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b0/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.130185 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2575 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1248 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-15 20:44:14.000000 dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.130675 dj_beatcloud-2.6.0b0/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2543 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1776 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.132313 dj_beatcloud-2.6.0b0/djtools/collections/
--rw-r--r--   0 alrichards   (502) staff       (20)     1434 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)    12878 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/collections.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2408 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2515 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    27150 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7584 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15833 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2405 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13832 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/collections/tracks.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.133861 dj_beatcloud-2.6.0b0/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/configs/collection_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     3758 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1301 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13868 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/configs/spotify_playlists.yaml
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.134013 dj_beatcloud-2.6.0b0/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.134604 dj_beatcloud-2.6.0b0/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/spotify/playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.135287 dj_beatcloud-2.6.0b0/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      825 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3435 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7959 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4888 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/djtools/sync/sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-15 20:44:14.136769 dj_beatcloud-2.6.0b0/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b0/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b0/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b0/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b0/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-15 20:43:27.000000 dj_beatcloud-2.6.0b0/djtools/version.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b0/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-15 20:44:14.137549 dj_beatcloud-2.6.0b0/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2371 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b0/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.668217 dj_beatcloud-2.6.0b1/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b1/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b1/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2575 2023-07-17 23:19:11.668380 dj_beatcloud-2.6.0b1/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b1/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.513790 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2575 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1248 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.525350 dj_beatcloud-2.6.0b1/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2543 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1776 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.617071 dj_beatcloud-2.6.0b1/djtools/collections/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1434 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    12878 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/collections.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2810 2023-07-17 22:44:15.000000 dj_beatcloud-2.6.0b1/djtools/collections/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2515 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    27150 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7584 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15833 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2405 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13832 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/tracks.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.649746 dj_beatcloud-2.6.0b1/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b1/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/configs/collection_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-17 22:43:41.000000 dj_beatcloud-2.6.0b1/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1301 2023-07-17 23:15:45.000000 dj_beatcloud-2.6.0b1/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    15653 2023-07-17 23:14:09.000000 dj_beatcloud-2.6.0b1/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b1/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b1/djtools/configs/spotify_playlists.yaml
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.650762 dj_beatcloud-2.6.0b1/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b1/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.657011 dj_beatcloud-2.6.0b1/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/spotify/playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.661345 dj_beatcloud-2.6.0b1/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      825 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3535 2023-07-17 22:33:04.000000 dj_beatcloud-2.6.0b1/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7959 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4888 2023-07-17 21:15:05.000000 dj_beatcloud-2.6.0b1/djtools/sync/sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.667129 dj_beatcloud-2.6.0b1/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b1/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b1/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-17 22:43:18.000000 dj_beatcloud-2.6.0b1/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b1/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b1/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-17 23:16:00.000000 dj_beatcloud-2.6.0b1/djtools/version.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b1/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-17 23:19:11.668902 dj_beatcloud-2.6.0b1/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2371 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/setup.py
```

### Comparing `dj_beatcloud-2.6.0b0/LICENSE` & `dj_beatcloud-2.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/PKG-INFO` & `dj_beatcloud-2.6.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.6.0b0
+Version: 2.6.0b1
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b0 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b1 Summary: DJ Tools is
 a library for managing a collection of music. Home-page: https://github.com/a-
 rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
 License: GNU GPLv3 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Other Audience Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
```

### Comparing `dj_beatcloud-2.6.0b0/README.md` & `dj_beatcloud-2.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.6.0b0
+Version: 2.6.0b1
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b0 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b1 Summary: DJ Tools is
 a library for managing a collection of music. Home-page: https://github.com/a-
 rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
 License: GNU GPLv3 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Other Audience Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
```

### Comparing `dj_beatcloud-2.6.0b0/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/__init__.py` & `dj_beatcloud-2.6.0b1/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/__main__.py` & `dj_beatcloud-2.6.0b1/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/collections/__init__.py` & `dj_beatcloud-2.6.0b1/djtools/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/collections/collections.py` & `dj_beatcloud-2.6.0b1/djtools/collections/collections.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/collections/config.py` & `dj_beatcloud-2.6.0b1/djtools/collections/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 """
 from __future__ import annotations
 import logging
 from pathlib import Path
 from typing import List, Optional, Union
 from typing_extensions import Literal
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, Extra, ValidationError
+import yaml
 
 from djtools.configs.config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
 
 
 class CollectionConfig(BaseConfig):
     """Configuration object for the collections package."""
 
+    COLLECTION_PATH: Path = None
     COLLECTION_PLAYLISTS: bool = False
     COLLECTION_PLAYLISTS_REMAINDER: Literal["folder", "playlist"] = "folder"
     COPY_PLAYLISTS:  List[str] = []
     COPY_PLAYLISTS_DESTINATION: Path = None
     PLATFORM: Literal["rekordbox"] = "rekordbox"
     SHUFFLE_PLAYLISTS:  List[str] = []
 
@@ -44,23 +46,31 @@
         ) and (not self.COLLECTION_PATH or not self.COLLECTION_PATH.exists()):
             raise RuntimeError(
                 "Using the collections package requires the config option "
                 "COLLECTION_PATH to be a valid collection path"
             )
 
         if self.COLLECTION_PLAYLISTS:
-            playlist_config = (
+            playlist_config_path = (
                 Path(__file__).parent.parent / "configs" /
                 "collection_playlists.yaml"
             )
-            if not playlist_config.exists():
-                raise RuntimeError(
-                    "collection_playlists.yaml must be a valid YAML to use the "
-                    "COLLECTION_PLAYLISTS feature"
-                )
+            err = (
+                "collection_playlists.yaml must be a valid YAML to use the "
+                "COLLECTION_PLAYLISTS feature"
+            )
+            if not playlist_config_path.exists():
+                raise RuntimeError(err)
+            try:
+                with open(
+                    playlist_config_path, mode="r", encoding="utf-8"
+                ) as _file:
+                    PlaylistConfig(**yaml.load(_file, Loader=yaml.FullLoader) or {})
+            except ValidationError as exc:
+                raise RuntimeError(err) from exc
 
 
 class PlaylistConfigContent(BaseModel, extra=Extra.forbid):
     "A class for type checking the content of the playlist config YAML."
     name: str
     playlists: List[Union[PlaylistConfigContent, str]]
```

### Comparing `dj_beatcloud-2.6.0b0/djtools/collections/copy_playlists.py` & `dj_beatcloud-2.6.0b1/djtools/collections/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/collections/helpers.py` & `dj_beatcloud-2.6.0b1/djtools/collections/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/collections/playlist_builder.py` & `dj_beatcloud-2.6.0b1/djtools/collections/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/collections/playlists.py` & `dj_beatcloud-2.6.0b1/djtools/collections/playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/collections/shuffle_playlists.py` & `dj_beatcloud-2.6.0b1/djtools/collections/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/collections/tracks.py` & `dj_beatcloud-2.6.0b1/djtools/collections/tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/configs/collection_playlists.yaml` & `dj_beatcloud-2.6.0b1/djtools/configs/collection_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/configs/config.yaml` & `dj_beatcloud-2.6.0b1/djtools/configs/config.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 collections:
+  COLLECTION_PATH: null
   COLLECTION_PLAYLISTS: false
   COLLECTION_PLAYLISTS_REMAINDER: folder
   COPY_PLAYLISTS: []
   COPY_PLAYLISTS_DESTINATION: null
   PLATFORM: rekordbox
   SHUFFLE_PLAYLISTS: []
 configs:
-  AWS_PROFILE: default
-  COLLECTION_PATH: null
   LOG_LEVEL: INFO
   VERBOSITY: 0
 spotify:
   REDDIT_CLIENT_ID: ''
   REDDIT_CLIENT_SECRET: ''
   REDDIT_USER_AGENT: ''
   SPOTIFY_CLIENT_ID: ''
@@ -24,14 +23,15 @@
   SPOTIFY_PLAYLIST_FUZZ_RATIO: 70
   SPOTIFY_PLAYLIST_POST_LIMIT: 100
   SPOTIFY_PLAYLIST_SUBREDDITS: []
   SPOTIFY_REDIRECT_URI: ''
   SPOTIFY_USERNAME: ''
 sync:
   ARTIST_FIRST: false
+  AWS_PROFILE: default
   AWS_USE_DATE_MODIFIED: false
   DISCORD_URL: ''
   DOWNLOAD_COLLECTION: false
   DOWNLOAD_EXCLUDE_DIRS: []
   DOWNLOAD_INCLUDE_DIRS: []
   DOWNLOAD_MUSIC: false
   DOWNLOAD_SPOTIFY_PLAYLIST: ''
```

### Comparing `dj_beatcloud-2.6.0b0/djtools/configs/helpers.py` & `dj_beatcloud-2.6.0b1/djtools/configs/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,300 +35,331 @@
 
     It also sets the log level and symlinks a user-provided directory to the
     library's configs folder via the --link-configs argument.
 
     Returns:
         argparse.NameSpace: Command-line arguments.
     """
-    parser = ArgumentParser()
-    parser.add_argument(
-        "--artist-first",
-        action="store_true",
-        help=(
-            "Indicate that Beatcloud tracks are in the format "
-            "`Artist - Track Title` instead of `Track Title - Artist`"
+    parser = ArgumentParser(
+        description=(
+            "djtools is a Python library with many features for streamlining "
+            "the processes around collecting, curating, and sharing a music "
+            "collection."
         ),
     )
     parser.add_argument(
-        "--aws-profile",
-        type=str,
-        help="AWS config profile",
-    )
-    parser.add_argument(
-        "--aws-use-date-modified",
-        action="store_true",
-        help=(
-            'Drop --size-only flag for "aws s3 sync" command; '
-            '"--aws-use-date-modified" will permit re-downloading/'
-            "re-uploading files if the date modified field changes"
-        ),
-    )
-    parser.add_argument(
-        "--check-tracks",
-        action="store_true",
-        help=(
-            "Trigger checking for track overlap between the Beatcloud and"
-            "CHECK_TRACKS_LOCAL_DIRS and / or CHECK_TRACKS_SPOTIFY_PLAYLISTS"
-        ),
+        "--link-configs",
+        type=convert_to_paths,
+        help="Location to symlink library configuration files to",
     )
     parser.add_argument(
-        "--check-tracks-fuzz-ratio",
-        type=int,
-        help=(
-            "Minimum similarity to indicate overlap between Beatcloud and "
-            "Spotify / local tracks"
-        ),
+        "--log-level",
+        choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
+        help="Logger level",
     )
     parser.add_argument(
-        "--check-tracks-local-dirs",
-        type=convert_to_paths,
-        nargs="+",
-        help="List of local directories to check against the Beatcloud",
+        "--verbosity",
+        "-v",
+        action="count",
+        default=0,
+        help="Logging verbosity",
     )
     parser.add_argument(
-        "--check-tracks-spotify-playlists",
-        type=str,
-        nargs="+",
-        help="List of Spotify playlist names to check against the Beatcloud",
+        "--version",
+        action="store_true",
+        help="Display package version",
     )
+    subparsers = parser.add_subparsers(title="subcommands")
+
+    ###########################################################################
+    # Sub-command for the collections package.
+    ###########################################################################
+    collections_parser = subparsers.add_parser("collections")
     parser.add_argument(
         "--collection-path",
         type=convert_to_paths,
         help='Path to a collection database',
     )
-    parser.add_argument(
+    collections_parser.add_argument(
         "--collection-playlists",
         action="store_true",
         help="Trigger building collection playlists",
     )
-    parser.add_argument(
+    collections_parser.add_argument(
         "--collection-playlists-remainder",
         type=str,
         choices=["folder", "playlist"],
         help=(
             'Place remainder tracks in either an "Other" folder of playlists '
             'or a single "Other" playlist'
         ),
     )
-    parser.add_argument(
+    collections_parser.add_argument(
         "--copy-playlists",
         type=str,
         nargs="+",
         help="List of playlists to copy audio files from",
     )
-    parser.add_argument(
+    collections_parser.add_argument(
         "--copy-playlists-destination",
         type=convert_to_paths,
         help="Location to copy playlists' audio files to",
     )
-    parser.add_argument(
-        "--discord-url",
-        type=str,
-        help="Discord webhook URL",
-    )
-    parser.add_argument(
-        "--download-collection",
-        action="store_true",
-        help=(
-            "Trigger downloading the collection of IMPORT_USER from the "
-            "Beatcloud"
-        ),
-    )
-    parser.add_argument(
-        "--download-exclude-dirs",
-        type=convert_to_paths,
-        nargs="+",
-        help="Paths to exclude when downloading from the Beatcloud",
-    )
-    parser.add_argument(
-        "--download-include-dirs",
-        type=convert_to_paths,
-        nargs="+",
-        help="Paths to include when downloading from the Beatcloud",
-    )
-    parser.add_argument(
-        "--download-music",
-        action="store_true",
-        help="Trigger downloading new tracks from the Beatcloud",
-    )
-    parser.add_argument(
-        "--download-spotify-playlist",
-        type=str,
-        help="Playlist name containing tracks to download from the Beatcloud",
-    )
-    parser.add_argument(
-        "--dryrun",
-        action="store_true",
-        help='Show result of "aws s3 sync" command without running it',
-    )
-    parser.add_argument(
-        "--import-user",
-        type=str,
-        help="USER whose COLLECTION_PATH you're downloading",
-    )
-    parser.add_argument(
-        "--link-configs",
-        type=convert_to_paths,
-        help="Location to symlink library configuration files to",
-    )
-    parser.add_argument(
-        "--log-level",
-        choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
-        help="Logger level",
-    )
-    parser.add_argument(
+    collections_parser.add_argument(
         "--platform",
         type=str,
         choices=["rekordbox"],
         help="DJ platform to use for the collections package",
     )
-    parser.add_argument(
+    collections_parser.add_argument(
+        "--shuffle-playlists",
+        type=str,
+        nargs="+",
+        help="List of playlist names to randomize tracks in",
+    )
+
+    ###########################################################################
+    # Sub-command for the spotify package.
+    ###########################################################################
+    spotify_parser = subparsers.add_parser("spotify")
+    spotify_parser.add_argument(
         "--reddit-client-id",
         type=str,
         help="Reddit API client ID",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--reddit-client-secret",
         type=str,
         help="Reddit API client secret",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--reddit-user-agent",
         type=str,
         help="Reddit API user agent",
     )
-    parser.add_argument(
-        "--shuffle-playlists",
-        type=str,
-        nargs="+",
-        help="List of playlist names to randomize tracks in",
-    )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-client-id",
         type=str,
         help="Spotify API client ID",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-client-secret",
         type=str,
         help="Spotify API client secret",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-playlist-default-limit",
         type=int,
         help="Default number of tracks for a Spotify playlist",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-playlist-default-period",
         type=str,
         help="Default Subreddit time filter for a Spotify playlist",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-playlist-default-type",
         type=str,
         help="Default Subreddit post filter for a Spotify playlist",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-playlist-from-upload",
         action="store_true",
         help=(
             "Trigger creating a Spotify playlist using the Discord webhook "
             "output of a music upload"
         ),
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-playlist-fuzz-ratio",
         type=int,
         help="Minimum similarity to add track to a playlist",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-playlist-post-limit",
         type=int,
         help="Maximum Subreddit posts to query for each playlist",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-playlist-subreddits",
         type=parse_yaml,
         help=(
             "List of Subreddits configs to generate playlists from; YAML "
             'strings with "name", "type", "period", and "limit" keys'
         ),
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-playlists",
         action="store_true",
         help="Trigger building Spotify playlists",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-redirect-uri",
         type=str,
         help="Spotify API redirect URI",
     )
-    parser.add_argument(
+    spotify_parser.add_argument(
         "--spotify-username",
         type=str,
         help="Spotify user to maintain playlists for",
     )
-    parser.add_argument(
+
+    ###########################################################################
+    # Sub-command for the sync package.
+    ###########################################################################
+    sync_parser = subparsers.add_parser("sync")
+    sync_parser.add_argument(
+        "--artist-first",
+        action="store_true",
+        help=(
+            "Indicate that Beatcloud tracks are in the format "
+            "`Artist - Track Title` instead of `Track Title - Artist`"
+        ),
+    )
+    sync_parser.add_argument(
+        "--aws-profile",
+        type=str,
+        help="AWS config profile",
+    )
+    sync_parser.add_argument(
+        "--aws-use-date-modified",
+        action="store_true",
+        help=(
+            'Drop --size-only flag for "aws s3 sync" command; '
+            '"--aws-use-date-modified" will permit re-downloading/'
+            "re-uploading files if the date modified field changes"
+        ),
+    )
+    sync_parser.add_argument(
+        "--discord-url",
+        type=str,
+        help="Discord webhook URL",
+    )
+    sync_parser.add_argument(
+        "--download-collection",
+        action="store_true",
+        help=(
+            "Trigger downloading the collection of IMPORT_USER from the "
+            "Beatcloud"
+        ),
+    )
+    sync_parser.add_argument(
+        "--download-exclude-dirs",
+        type=convert_to_paths,
+        nargs="+",
+        help="Paths to exclude when downloading from the Beatcloud",
+    )
+    sync_parser.add_argument(
+        "--download-include-dirs",
+        type=convert_to_paths,
+        nargs="+",
+        help="Paths to include when downloading from the Beatcloud",
+    )
+    sync_parser.add_argument(
+        "--download-music",
+        action="store_true",
+        help="Trigger downloading new tracks from the Beatcloud",
+    )
+    sync_parser.add_argument(
+        "--download-spotify-playlist",
+        type=str,
+        help="Playlist name containing tracks to download from the Beatcloud",
+    )
+    sync_parser.add_argument(
+        "--dryrun",
+        action="store_true",
+        help='Show result of "aws s3 sync" command without running it',
+    )
+    sync_parser.add_argument(
+        "--import-user",
+        type=str,
+        help="USER whose COLLECTION_PATH you're downloading",
+    )
+    sync_parser.add_argument(
         "--upload-collection",
         action="store_true",
         help=(
             "Trigger uploading the collection of IMPORT_USER from the "
             "Beatcloud"
         ),
     )
-    parser.add_argument(
+    sync_parser.add_argument(
         "--upload-exclude-dirs",
         type=convert_to_paths,
         nargs="+",
         help="List of paths to exclude when uploading to the Beatcloud",
     )
-    parser.add_argument(
+    sync_parser.add_argument(
         "--upload-include-dirs",
         type=convert_to_paths,
         nargs="+",
         help="List of paths to include when uploading to the Beatcloud",
     )
-    parser.add_argument(
+    sync_parser.add_argument(
         "--upload-music",
         action="store_true",
         help="Trigger uploading new tracks from the Beatcloud",
     )
-    parser.add_argument(
-        "--url-download",
-        type=str,
-        help="URL to download audio file(s) from",
-    )
-    parser.add_argument(
-        "--url-download-destination",
-        type=convert_to_paths,
-        help="Location to download audio file(s) to",
-    )
-    parser.add_argument(
+    sync_parser.add_argument(
         "--usb-path",
         type=convert_to_paths,
         help="Path to a drive with audio files",
     )
-    parser.add_argument(
+    sync_parser.add_argument(
         "--user",
         type=str,
         help="Username of the current user",
     )
-    parser.add_argument(
-        "--verbosity",
-        "-v",
-        action="count",
-        default=0,
-        help="Logging verbosity",
-    )
-    parser.add_argument(
-        "--version",
+
+    ###########################################################################
+    # Sub-command for the utils package.
+    ###########################################################################
+    utils_parser = subparsers.add_parser("utils")
+    utils_parser.add_argument(
+        "--check-tracks",
         action="store_true",
-        help="Display package version",
+        help=(
+            "Trigger checking for track overlap between the Beatcloud and"
+            "CHECK_TRACKS_LOCAL_DIRS and / or CHECK_TRACKS_SPOTIFY_PLAYLISTS"
+        ),
+    )
+    utils_parser.add_argument(
+        "--check-tracks-fuzz-ratio",
+        type=int,
+        help=(
+            "Minimum similarity to indicate overlap between Beatcloud and "
+            "Spotify / local tracks"
+        ),
+    )
+    utils_parser.add_argument(
+        "--check-tracks-local-dirs",
+        type=convert_to_paths,
+        nargs="+",
+        help="List of local directories to check against the Beatcloud",
+    )
+    utils_parser.add_argument(
+        "--check-tracks-spotify-playlists",
+        type=str,
+        nargs="+",
+        help="List of Spotify playlist names to check against the Beatcloud",
+    )
+    utils_parser.add_argument(
+        "--url-download",
+        type=str,
+        help="URL to download audio file(s) from",
+    )
+    utils_parser.add_argument(
+        "--url-download-destination",
+        type=convert_to_paths,
+        help="Location to download audio file(s) to",
     )
+
+    ###########################################################################
+    ###########################################################################
+
     args = parser.parse_args()
 
     if args.log_level:
         logger.setLevel(args.log_level)
 
     if args.version:
         print(__version__)
```

### Comparing `dj_beatcloud-2.6.0b0/djtools/spotify/__init__.py` & `dj_beatcloud-2.6.0b1/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/spotify/config.py` & `dj_beatcloud-2.6.0b1/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/spotify/helpers.py` & `dj_beatcloud-2.6.0b1/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.6.0b1/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/sync/__init__.py` & `dj_beatcloud-2.6.0b1/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/sync/config.py` & `dj_beatcloud-2.6.0b1/djtools/sync/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """This module contains the configuration object for the sync package.
 The attributes of this configuration object correspond with the "sync" key
 of config.yaml
 """
 import getpass
 import logging
+import os
 from pathlib import Path
 from typing import List, Optional, Union
 
 from pydantic import validator
 
 from djtools.configs.config import BaseConfig
 
@@ -15,14 +16,15 @@
 logger = logging.getLogger(__name__)
 
 
 class SyncConfig(BaseConfig):
     """Configuration object for the sync package."""
 
     ARTIST_FIRST: bool = False
+    AWS_PROFILE: str = "default"
     AWS_USE_DATE_MODIFIED: bool = False
     DISCORD_URL: str = ""
     DOWNLOAD_COLLECTION: bool = False
     DOWNLOAD_EXCLUDE_DIRS: List[Path] = []
     DOWNLOAD_INCLUDE_DIRS: List[Path] = []
     DOWNLOAD_MUSIC: bool = False
     DOWNLOAD_SPOTIFY_PLAYLIST: str = ""
@@ -67,14 +69,15 @@
                 self.UPLOAD_MUSIC,
             ]
         ):
             if not self.AWS_PROFILE:
                 msg = "Config must include AWS_PROFILE for sync operations"
                 logger.critical(msg)
                 raise RuntimeError(msg)
+            os.environ["AWS_PROFILE"] = self.AWS_PROFILE
 
         if (
             any([self.DOWNLOAD_MUSIC, self.UPLOAD_MUSIC]) and
             (not self.USB_PATH or not self.USB_PATH.exists())
         ):
             msg = (
                 "Config must include USB_PATH for both DOWNLOAD_MUSIC and "
```

### Comparing `dj_beatcloud-2.6.0b0/djtools/sync/helpers.py` & `dj_beatcloud-2.6.0b1/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/sync/sync_operations.py` & `dj_beatcloud-2.6.0b1/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/utils/__init__.py` & `dj_beatcloud-2.6.0b1/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/utils/check_tracks.py` & `dj_beatcloud-2.6.0b1/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/utils/helpers.py` & `dj_beatcloud-2.6.0b1/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/djtools/utils/url_download.py` & `dj_beatcloud-2.6.0b1/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b0/setup.py` & `dj_beatcloud-2.6.0b1/setup.py`

 * *Files identical despite different names*

