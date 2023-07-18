# Comparing `tmp/youtube-bz-0.3.3.tar.gz` & `tmp/youtube_bz-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube-bz-0.3.3.tar", last modified: Tue May 31 18:44:29 2022, max compression
+gzip compressed data, was "youtube_bz-0.3.4.tar", max compression
```

## Comparing `youtube-bz-0.3.3.tar` & `youtube_bz-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 18:44:29.495679 youtube-bz-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-05-31 18:44:15.000000 youtube-bz-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-05-31 18:44:29.495679 youtube-bz-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-05-31 18:44:15.000000 youtube-bz-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-31 18:44:29.495679 youtube-bz-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-05-31 18:44:15.000000 youtube-bz-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 18:44:29.491679 youtube-bz-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 18:44:15.000000 youtube-bz-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-05-31 18:44:15.000000 youtube-bz-0.3.3/tests/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 18:44:29.495679 youtube-bz-0.3.3/youtube_bz/
--rw-r--r--   0 runner    (1001) docker     (121)     4893 2022-05-31 18:44:15.000000 youtube-bz-0.3.3/youtube_bz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-31 18:44:15.000000 youtube-bz-0.3.3/youtube_bz/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 18:44:29.495679 youtube-bz-0.3.3/youtube_bz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-05-31 18:44:28.000000 youtube-bz-0.3.3/youtube_bz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-05-31 18:44:29.000000 youtube-bz-0.3.3/youtube_bz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 18:44:29.000000 youtube-bz-0.3.3/youtube_bz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-05-31 18:44:29.000000 youtube-bz-0.3.3/youtube_bz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-31 18:44:29.000000 youtube-bz-0.3.3/youtube_bz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-31 18:44:29.000000 youtube-bz-0.3.3/youtube_bz.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2023-07-18 20:30:09.327308 youtube_bz-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1879 2023-07-18 20:30:09.327308 youtube_bz-0.3.4/README.md
+-rw-r--r--   0        0        0      865 2023-07-18 20:30:09.371311 youtube_bz-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3041 2023-07-18 20:30:09.371311 youtube_bz-0.3.4/youtube_bz/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-18 20:30:09.371311 youtube_bz-0.3.4/youtube_bz/__main__.py
+-rw-r--r--   0        0        0      100 2023-07-18 20:30:09.371311 youtube_bz-0.3.4/youtube_bz/exceptions.py
+-rw-r--r--   0        0        0     1059 2023-07-18 20:30:09.371311 youtube_bz-0.3.4/youtube_bz/musicbrainz.py
+-rw-r--r--   0        0        0        0 2023-07-18 20:30:09.371311 youtube_bz-0.3.4/youtube_bz/utils/__init__.py
+-rw-r--r--   0        0        0     1983 2023-07-18 20:30:09.371311 youtube_bz-0.3.4/youtube_bz/utils/levenshtein_distance.py
+-rw-r--r--   0        0        0     1616 2023-07-18 20:30:09.371311 youtube_bz-0.3.4/youtube_bz/youtube.py
+-rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 youtube_bz-0.3.4/PKG-INFO
```

### Comparing `youtube-bz-0.3.3/LICENSE` & `youtube_bz-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube-bz-0.3.3/PKG-INFO` & `youtube_bz-0.3.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,12 @@
-Metadata-Version: 2.1
-Name: youtube-bz
-Version: 0.3.3
-Summary: YoutubeBrainz allow you to find and download Youtube Videos associated to an Album on MusicBrainz.
-Home-page: https://github.com/flowrey/youtube-bz
-Author: Flowrey
-Author-email: flowrey@laposte.net
-Project-URL: Bug Tracker, https://github.com/flowrey/youtube-bz/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # YouTubeBrainz
 
 YoutubeBrainz allows you to find and download Youtube videos associated to an album on MusicBrainz.
 
-[![PyPi version](https://img.shields.io/badge/pypi-0.3.2-blue)](https://pypi.org/project/youtube-bz/)
+[![PyPi version](https://img.shields.io/badge/pypi-0.3.4-blue)](https://pypi.org/project/youtube-bz/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![GPL 3.0](https://img.shields.io/badge/license-GPL_3.0-blue.svg)](LICENSE.md)
 [![Coverage Status](https://coveralls.io/repos/github/Flowrey/youtube-bz/badge.svg?branch=master)](https://coveralls.io/github/Flowrey/youtube-bz?branch=master)
 ![Coverage Status](https://github.com/flowrey/youtube-bz/actions/workflows/python-test.yml/badge.svg)
 
 
 ## Summary
```

### Comparing `youtube-bz-0.3.3/youtube_bz.egg-info/PKG-INFO` & `youtube_bz-0.3.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: youtube-bz
-Version: 0.3.3
+Version: 0.3.4
 Summary: YoutubeBrainz allow you to find and download Youtube Videos associated to an Album on MusicBrainz.
-Home-page: https://github.com/flowrey/youtube-bz
+License: GPL-3.0
 Author: Flowrey
 Author-email: flowrey@laposte.net
-Project-URL: Bug Tracker, https://github.com/flowrey/youtube-bz/issues
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # YouTubeBrainz
 
 YoutubeBrainz allows you to find and download Youtube videos associated to an album on MusicBrainz.
 
-[![PyPi version](https://img.shields.io/badge/pypi-0.3.2-blue)](https://pypi.org/project/youtube-bz/)
+[![PyPi version](https://img.shields.io/badge/pypi-0.3.4-blue)](https://pypi.org/project/youtube-bz/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![GPL 3.0](https://img.shields.io/badge/license-GPL_3.0-blue.svg)](LICENSE.md)
 [![Coverage Status](https://coveralls.io/repos/github/Flowrey/youtube-bz/badge.svg?branch=master)](https://coveralls.io/github/Flowrey/youtube-bz?branch=master)
 ![Coverage Status](https://github.com/flowrey/youtube-bz/actions/workflows/python-test.yml/badge.svg)
 
 
 ## Summary
@@ -74,7 +77,8 @@
 This project is licensed under the [GPL-3.0](LICENSE)
 GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for
 details
 
 ## Acknowledgments
 
   - This project's structure has been greatly inspired by youtube-dl
+
```

