# Comparing `tmp/pmm_cfg_gen-0.2.5.tar.gz` & `tmp/pmm_cfg_gen-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmm_cfg_gen-0.2.5.tar", max compression
+gzip compressed data, was "pmm_cfg_gen-0.2.6.tar", max compression
```

## Comparing `pmm_cfg_gen-0.2.5.tar` & `pmm_cfg_gen-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0    35149 2023-04-01 09:59:32.119583 pmm_cfg_gen-0.2.5/LICENSE
--rw-r--r--   0        0        0     2502 2023-06-13 21:13:26.509716 pmm_cfg_gen-0.2.5/README.md
--rw-r--r--   0        0        0     1263 2023-06-28 13:11:14.647360 pmm_cfg_gen-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       29 2023-04-04 21:44:17.290489 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/.gitignore
--rw-r--r--   0        0        0     1691 2023-04-24 15:14:53.409283 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/__init__.py
--rw-r--r--   0        0        0     5242 2023-06-08 14:36:04.841456 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/config_default.yaml
--rw-r--r--   0        0        0     2705 2023-06-13 15:55:55.365775 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/logging.yaml
--rw-r--r--   0        0        0       27 2023-04-25 13:15:00.359814 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/library.json.j2
--rw-r--r--   0        0        0       24 2023-04-25 13:14:55.063789 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/movie.collection.json.j2
--rw-r--r--   0        0        0     3855 2023-06-13 12:28:08.719838 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/movie.collection.yaml.j2
--rw-r--r--   0        0        0       25 2023-04-21 20:29:02.908227 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/movie.metadata.json.j2
--rw-r--r--   0        0        0     3527 2023-06-28 12:16:51.792847 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/movie.metadata.yaml.j2
--rw-r--r--   0        0        0       24 2023-04-25 13:14:34.303691 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/show.collection.json.j2
--rw-r--r--   0        0        0     3854 2023-06-13 12:50:38.818656 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/show.collection.yaml.j2
--rw-r--r--   0        0        0       24 2023-04-21 20:28:17.955980 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/show.metadata.json.j2
--rw-r--r--   0        0        0     3859 2023-06-28 12:17:20.073017 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/show.metadata.yaml.j2
--rw-r--r--   0        0        0     1107 2023-05-11 19:57:56.303215 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/template.collection.yaml.j2
--rw-r--r--   0        0        0        0 2023-04-03 13:48:27.869541 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/__init__.py
--rw-r--r--   0        0        0     2592 2023-06-08 14:35:32.685306 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/cli_args.py
--rw-r--r--   0        0        0     1956 2023-05-10 00:07:32.747680 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/file_utils.py
--rw-r--r--   0        0        0     1778 2023-04-13 17:07:10.794833 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/logging_utils.py
--rw-r--r--   0        0        0    37611 2023-06-15 15:59:43.139022 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/plex.py
--rw-r--r--   0        0        0     2951 2023-06-12 16:23:04.350525 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/plex_cache.py
--rw-r--r--   0        0        0     2150 2023-06-12 16:23:51.874774 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/plex_stats.py
--rw-r--r--   0        0        0    17324 2023-06-15 19:42:50.434591 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/plex_utils.py
--rwxr-xr-x   0        0        0    14285 2023-06-13 12:50:09.094516 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/pmm_utils.py
--rw-r--r--   0        0        0    18201 2023-06-08 15:54:52.364845 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/settings_utils_v1.py
--rw-r--r--   0        0        0    10122 2023-06-13 02:22:42.005047 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/template_filters.py
--rw-r--r--   0        0        0     5057 2023-06-13 01:24:01.797107 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/template_manager.py
--rwxr-xr-x   0        0        0     4443 2023-05-11 12:21:27.849258 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/time_span.py
--rw-r--r--   0        0        0     2691 2023-04-10 21:13:51.972712 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/timer.py
--rw-r--r--   0        0        0     2579 2023-04-26 13:50:19.226275 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/tmdb_utils.py
--rw-r--r--   0        0        0     1361 2023-04-24 15:15:17.785439 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/trakt_utils.py
--rw-r--r--   0        0        0     1514 2023-04-10 21:13:52.064713 pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/tvdb_utils.py
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 pmm_cfg_gen-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-01 09:59:32.119583 pmm_cfg_gen-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2569 2023-07-18 20:20:41.735401 pmm_cfg_gen-0.2.6/README.md
+-rw-r--r--   0        0        0     1263 2023-07-18 19:57:49.326120 pmm_cfg_gen-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-04-04 21:44:17.290489 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/.gitignore
+-rw-r--r--   0        0        0     1691 2023-04-24 15:14:53.409283 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/__init__.py
+-rw-r--r--   0        0        0     5262 2023-07-18 17:55:20.086253 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/config_default.yaml
+-rw-r--r--   0        0        0     2705 2023-06-13 15:55:55.365775 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/logging.yaml
+-rw-r--r--   0        0        0       27 2023-04-25 13:15:00.359814 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/library.json.j2
+-rw-r--r--   0        0        0       24 2023-04-25 13:14:55.063789 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/movie.collection.json.j2
+-rw-r--r--   0        0        0     3855 2023-06-13 12:28:08.719838 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/movie.collection.yaml.j2
+-rw-r--r--   0        0        0       25 2023-04-21 20:29:02.908227 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/movie.metadata.json.j2
+-rw-r--r--   0        0        0     3527 2023-06-28 12:16:51.792847 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/movie.metadata.yaml.j2
+-rw-r--r--   0        0        0       24 2023-07-18 17:44:12.698009 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/music.collection.json.j2
+-rw-r--r--   0        0        0       25 2023-07-18 17:42:22.245419 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/music.metadata.json.j2
+-rw-r--r--   0        0        0       24 2023-04-25 13:14:34.303691 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/show.collection.json.j2
+-rw-r--r--   0        0        0     3854 2023-06-13 12:50:38.818656 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/show.collection.yaml.j2
+-rw-r--r--   0        0        0       24 2023-04-21 20:28:17.955980 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/show.metadata.json.j2
+-rw-r--r--   0        0        0     3859 2023-06-28 12:17:20.073017 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/show.metadata.yaml.j2
+-rw-r--r--   0        0        0     1107 2023-05-11 19:57:56.303215 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/template.collection.yaml.j2
+-rw-r--r--   0        0        0        0 2023-04-03 13:48:27.869541 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/__init__.py
+-rw-r--r--   0        0        0     2592 2023-06-08 14:35:32.685306 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/cli_args.py
+-rw-r--r--   0        0        0     1956 2023-05-10 00:07:32.747680 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/file_utils.py
+-rw-r--r--   0        0        0     1778 2023-04-13 17:07:10.794833 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/logging_utils.py
+-rw-r--r--   0        0        0    38052 2023-07-18 19:43:03.373472 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/plex.py
+-rw-r--r--   0        0        0     2951 2023-06-12 16:23:04.350525 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/plex_cache.py
+-rw-r--r--   0        0        0     2150 2023-06-12 16:23:51.874774 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/plex_stats.py
+-rw-r--r--   0        0        0    17494 2023-07-18 18:24:24.048737 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/plex_utils.py
+-rwxr-xr-x   0        0        0    14285 2023-06-13 12:50:09.094516 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/pmm_utils.py
+-rw-r--r--   0        0        0    18201 2023-06-08 15:54:52.364845 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/settings_utils_v1.py
+-rw-r--r--   0        0        0    10122 2023-06-13 02:22:42.005047 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/template_filters.py
+-rw-r--r--   0        0        0     5057 2023-06-13 01:24:01.797107 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/template_manager.py
+-rwxr-xr-x   0        0        0     4443 2023-05-11 12:21:27.849258 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/time_span.py
+-rw-r--r--   0        0        0     2691 2023-04-10 21:13:51.972712 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/timer.py
+-rw-r--r--   0        0        0     2579 2023-04-26 13:50:19.226275 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/tmdb_utils.py
+-rw-r--r--   0        0        0     1361 2023-04-24 15:15:17.785439 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/trakt_utils.py
+-rw-r--r--   0        0        0     1514 2023-04-10 21:13:52.064713 pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/tvdb_utils.py
+-rw-r--r--   0        0        0     3912 1970-01-01 00:00:00.000000 pmm_cfg_gen-0.2.6/PKG-INFO
```

### Comparing `pmm_cfg_gen-0.2.5/LICENSE` & `pmm_cfg_gen-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/README.md` & `pmm_cfg_gen-0.2.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Plex-Meta-Manager-Config-Generator
 
 [![PyPI version](https://badge.fury.io/py/pmm-cfg-gen.svg)](https://badge.fury.io/py/pmm-cfg-gen)
 
 A python application to automatically generate Plex Meta Manager configuration files based on your plex libraries.
 
+Library types supported:
+
+* Movie
+* TV
+* Music (json format only)
+
 ## Install
 
 ```shell
 pip install pmm-cfg-gen
 ```
 
 ## Running from command line
```

### Comparing `pmm_cfg_gen-0.2.5/pyproject.toml` & `pmm_cfg_gen-0.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pmm-cfg-gen"
-version = "0.2.5"
+version = "0.2.6"
 description = "A script to help automatically generate Plex Meta Manager configuration files for your libraries"
 license = "GPL-3.0-or-later"
 authors = ["Shawn Anderson <sanderson@eye-catcher.com>"]
 readme = "README.md"
 homepage = "https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator"
 repository = "https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator"
 keywords = [ "pmm", "plex-meta-manager", "plex" ]
```

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/__init__.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/config_default.yaml` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/config_default.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -20,54 +20,68 @@
 # theTvDatabase:
 #   apiKey:
 templates:
   library:
   - { type: "library.any", format: "yaml", file: "library.yaml.j2" }
   - { type: "library.any", format: "html", file: "library.html.j2" }
   - { type: "library.any", format: "json", file: "library.json.j2", subFolder: "json" }
+
   collection:
   - { type: "collection.movie", format: "yaml", file: "movie.collection.yaml.j2", defaultTemplate: "tplTMDBCollection" }
   - { type: "collection.movie", format: "html", file: "movie.collection.html.j2" }
   - { type: "collection.movie", format: "json", file: "movie.collection.json.j2", subFolder: "json" }
+
   - { type: "collection.show", format: "yaml", file: "show.collection.yaml.j2", defaultTemplate: "tplTMDBCollection"  }
   - { type: "collection.show", format: "html", file: "show.collection.html.j2" }
   - { type: "collection.show", format: "json", file: "show.collection.json.j2", subFolder: "json" }
-  - { type: "collection.music", format: "yaml", file: "music.collection.yaml.j2" }
-  - { type: "collection.music", format: "html", file: "music.collection.html.j2" }
-  - { type: "collection.music", format: "json", file: "music.collection.json.j2", subFolder: "json" }
+
+  - { type: "collection.artist", format: "yaml", file: "music.collection.yaml.j2" }
+  - { type: "collection.artist", format: "html", file: "music.collection.html.j2" }
+  - { type: "collection.atist", format: "json", file: "music.collection.json.j2", subFolder: "json" }
+
   - { type: "collection.report", format: "yaml", file: "report.collection.yaml.j2" }
   - { type: "collection.report", format: "html", file: "report.collection.html.j2" }
   - { type: "collection.report", format: "json", file: "report.collection.json.j2", subFolder: "json" }
+
   - { type: "collection.template", "format": "yaml", "file": "template.collection.yaml.j2" }
+
   metadata:
   - { type: "metadata.movie", format: "yaml", file: "movie.metadata.yaml.j2", defaultTemplate: "tplTMDBCollection"  }
   - { type: "metadata.movie", format: "html", file: "movie.metadata.html.j2" }
   - { type: "metadata.movie", format: "json", file: "movie.metadata.json.j2", subFolder: "json" }
+
   - { type: "metadata.show", format: "yaml", file: "show.metadata.yaml.j2", defaultTemplate: "tplTMDBCollection"  }
   - { type: "metadata.show", format: "html", file: "show.metadata.html.j2" }
   - { type: "metadata.show", format: "json", file: "show.metadata.json.j2", subFolder: "json" }
-  - { type: "metadata.music", format: "yaml", file: "music.metadata.yaml.j2" }
-  - { type: "metadata.music", format: "html", file: "music.metadata.html.j2" }
-  - { type: "metadata.music", format: "json", file: "music.metadata.json.j2", subFolder: "json" }
+
+  - { type: "metadata.artist", format: "yaml", file: "music.metadata.yaml.j2" }
+  - { type: "metadata.artist", format: "html", file: "music.metadata.html.j2" }
+  - { type: "metadata.artist", format: "json", file: "music.metadata.json.j2", subFolder: "json" }
+
   - { type: "metadata.report", format: "yaml", file: "report.metadata.yaml.j2" }
   - { type: "metadata.report", format: "html", file: "report.metadata.html.j2" }
   - { type: "metadata.report", format: "json", file: "report.metadata.json.j2", subFolder: "json" }
+
   overlay:
   - { type: "overlay.movie", format: "yaml", file: "movie.overlay.yaml.j2" }
   - { type: "overlay.movie", format: "html", file: "movie.overlay.html.j2" }
   - { type: "overlay.movie", format: "json", file: "movie.overlay.json.j2", subFolder: "json" }
+
   - { type: "overlay.show", format: "yaml", file: "show.overlay.yaml.j2" }
   - { type: "overlay.show", format: "html", file: "show.overlay.html.j2" }
   - { type: "overlay.show", format: "json", file: "show.overlay.json.j2", subFolder: "json" }
-  - { type: "overlay.music", format: "yaml", file: "music.overlay.yaml.j2" }
-  - { type: "overlay.music", format: "html", file: "music.overlay.html.j2" }
-  - { type: "overlay.music", format: "json", file: "music.overlay.json.j2", subFolder: "json" }
+
+  - { type: "overlay.artist", format: "yaml", file: "music.overlay.yaml.j2" }
+  - { type: "overlay.artist", format: "html", file: "music.overlay.html.j2" }
+  - { type: "overlay.artist", format: "json", file: "music.overlay.json.j2", subFolder: "json" }
+
   - { type: "overlay.report", format: "yaml", file: "report.overlay.yaml.j2" }
   - { type: "overlay.report", format: "html", file: "report.overlay.html.j2" }
   - { type: "overlay.report", format: "json", file: "report.overlay.json.j2", subFolder: "json" }
+
   # report:
   # - { type: "report.any", format: "yaml", file: "report.yaml.j2" }
   # - { type: "report.any", format: "json", file: "report.json.j2" }
   # - { type: "report.any", format: "html", file: "report.html.j2" }
 output:
   path: "./data"
   
@@ -81,20 +95,20 @@
     metadataReport: "{{library.title}} - Metadata Report"
     report: "{{library.title}} - Report"
     template: "template"
 generate:
   types:
   - library.any
   - collection.movie
-  # - collection.music
+  - collection.artist
   - collection.show
   - collection.report
   - collection.template
   - metadata.movie
-  # - metadata.music
+  - metadata.artist
   - metadata.show
   - metadata.report
   # - overlay.movie
   # - overlay.music
   # - overlay.show
   - report.any
   formats:
```

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/logging.yaml` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/logging.yaml`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/movie.collection.yaml.j2` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/movie.collection.yaml.j2`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/movie.metadata.yaml.j2` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/movie.metadata.yaml.j2`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/show.collection.yaml.j2` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/show.collection.yaml.j2`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/show.metadata.yaml.j2` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/show.metadata.yaml.j2`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/templates/template.collection.yaml.j2` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/templates/template.collection.yaml.j2`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/cli_args.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/cli_args.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/file_utils.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/logging_utils.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/plex.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/plex.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import requests
 
 import urllib3
 import urllib3.exceptions
 from plexapi.library import LibrarySection
 from plexapi.collection import Collection
 from plexapi.video import Video
+from plexapi.audio import Artist
 from plexapi.server import PlexServer
 
 from pmm_cfg_gen.utils.settings_utils_v1 import globalSettingsMgr, SettingsTemplateLibraryTypeEnum, SettingsTemplateFileFormatEnum, SettingsPlexLibrary
 from pmm_cfg_gen.utils.file_utils import formatLibraryItemPath
 from pmm_cfg_gen.utils.plex_stats import PlexStats
 from pmm_cfg_gen.utils.plex_utils import PlexItemHelper, PlexVideoHelper, PlexCollectionHelper
 from pmm_cfg_gen.utils.template_manager import TemplateManager
@@ -323,15 +324,15 @@
         itemName: str = ""
         if collection is not None:
             itemName=collection.title
             
             pmmItem = self.__plexMetaManagerCache[self.plexLibrarySettings.name].collectionItem_to_dict(collection.title)
             
             fileNameBase = PlexItemHelper.formatString(globalSettingsMgr.settings.output.fileNameFormat.collections, library=self.plexLibrary, collection=collection, item=None, pmm=pmmItem, cleanTitleStrings=True)
-        elif len(items) == 1 and isinstance(items[0], Video):
+        elif len(items) == 1 and (isinstance(items[0], Video) or isinstance(items[0], Artist)):
             itemName=items[0].title
             
             pmmItem = self.__plexMetaManagerCache[self.plexLibrarySettings.name].metadataItem_to_dict(items[0].title)
             
             fileNameBase = PlexItemHelper.formatString(globalSettingsMgr.settings.output.fileNameFormat.metadata, library=self.plexLibrary, collection=collection, item=items[0], pmm=pmmItem, cleanTitleStrings=True)
         else:
             self._logger.error("Invalid item attempted to be processed: {}".format(items))
@@ -389,32 +390,39 @@
                         ].items.processed,
                         self.__stats.countsLibraries[self.plexLibrarySettings.name].items.total,
                         item.type,
                         PlexItemHelper.formatItemTitle(item),
                     )
                 )
 
-                pmmItem = self.__plexMetaManagerCache[self.plexLibrarySettings.name].metadataItem_to_dict(item.title, item.year)
+                pmmItem = self.__plexMetaManagerCache[self.plexLibrarySettings.name].metadataItem_to_dict(item.title, item.year if isinstance(item, Video) else None)
 
                 self._addItemToProcessedCache(collection, item, pmmItem)
 
                 itemDict = { "metadata": item, "pmm": pmmItem }
-                
-                seasons = []
-                if "childCount" in item.__dict__:
-                    self._logger.debug("  Loading Seasons...")
-                    seasons = item.seasons()
 
-                    itemDict.update({"seasons": seasons})
+                if isinstance(item, Video):
+                    seasons = []
+                    if "childCount" in item.__dict__:
+                        self._logger.debug("  Loading Seasons...")
+                        seasons = item.seasons()
+
+                        itemDict.update({"seasons": seasons})
+                elif isinstance(item, Artist):
+                    albums = item.albums()
+                    itemDict.update({"albums": albums})
+
+                    tracks = item.tracks()
+                    itemDict.update({"tracks": tracks})
 
                 itemsWithExtras.append(itemDict)
 
         # Do we have anything we need to process
         if len(itemsWithExtras) > 0:
-            sorted(itemsWithExtras, key=lambda x: x["metadata"].year)
+            sorted(itemsWithExtras, key=lambda x: x["metadata"].year if "year" in x["metadata"].__dict__ else 0)
 
             for tplFile in tplFiles:
                 try:
                     if globalSettingsMgr.settings.generate.isFormatEnabled(tplFile.format) and globalSettingsMgr.settings.generate.isTypeEnabled(tplFile.type):
                         
                         if tplFile.subFolder is not None:
                             fileName = Path(self.pathLibrary, "metadata", tplFile.subFolder, "{}.{}".format(fileNameBase, tplFile.fileExtension))
```

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/plex_cache.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/plex_cache.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/plex_stats.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/plex_stats.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/plex_utils.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/plex_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 
 import jsonpickle.handlers
 from plexapi.base import PlexObject, PlexPartialObject
 from plexapi.library import LibrarySection
 from plexapi.collection import Collection
 from plexapi.video import Video, Movie, Show
+from plexapi.audio import Artist
 from plexapi.server import PlexServer
 import re
 
 from pmm_cfg_gen.utils.settings_utils_v1 import SettingsPlexLibrary, globalSettingsMgr
 
 ###################################################################################################
 
@@ -113,15 +114,15 @@
          @param s - The title to be cleaned. This should be a string that has no punctuation or other non - alphanumeric characters.
          
          @return A string that has all characters in the form of a - zA - Z0 - 9 and underscores
         """
         return title.replace("/", "-").replace("\\", "-").replace(":", "-").replace("*", "-").replace("?", "-").replace("\"", "-").replace("<", "-").replace(">", "-").replace("|", "-")
 
     @classmethod
-    def formatString(cls, formatString: str, library : LibrarySection | None = None, collection : Collection | None = None, item : Video | None = None, pmm : dict | None = None, librarySettings : SettingsPlexLibrary | None = None, cleanTitleStrings : bool = False) -> str:
+    def formatString(cls, formatString: str, library : LibrarySection | None = None, collection : Collection | None = None, item : Video | Artist | None = None, pmm : dict | None = None, librarySettings : SettingsPlexLibrary | None = None, cleanTitleStrings : bool = False) -> str:
         """
         The format string to format. This is a string with placeholders to be substituted.
         
         @param cls - The class that owns the LibrarySection. Defaults to None.
         @param library - The LibrarySection to format. Defaults to None.
         @param collection - The Collection to format. Defaults to None.
         @param item - The Videobutton to format. Defaults to None.
@@ -152,20 +153,23 @@
                 if lstLabels is not None and len(lstLabels) > 0:
                     logging.getLogger("pmm_cfg_gen").debug("formatString collection labels: {}".format(lstLabels))
                     result = result.replace("{{universe}}", lstLabels[0] if lstLabels[0] not in result else "")
 
         if item is not None:
             result = result.replace("{{item.title}}", cls.cleanString(item.title) if cleanTitleStrings else item.title)
             result = result.replace("{{item.titleSort}}", item.titleSort if item.titleSort else "")
-            result = result.replace("{{item.year}}", str(item.year) if item.year and str(item.year) not in item.title else "")
-            result = result.replace("{{item.type}}", item.type if item.type else "")
-            result = result.replace("{{item.titleSort}}", item.titleSort if item.titleSort else "")
-            result = result.replace("{{item.contentRating}}", item.contentRating if item.contentRating else "")
-            result = result.replace("{{item.editionTitle}}", item.editionTitle if isinstance(item, Movie) and item.editionTitle else "")
 
+            if isinstance(item, Video):
+                result = result.replace("{{item.year}}", str(item.year) if item.year and str(item.year) not in item.title else "")
+                result = result.replace("{{item.type}}", item.type if item.type else "")
+                result = result.replace("{{item.contentRating}}", item.contentRating if item.contentRating else "")
+                result = result.replace("{{item.editionTitle}}", item.editionTitle if isinstance(item, Movie) and item.editionTitle else "")
+            elif isinstance(item, Artist):
+                pass
+    
             if "{{universe}}" in result:
                 lstLabels = PlexItemHelper.getNamedCollectionLabels(item)
                 if lstLabels is not None and len(lstLabels) > 0:
                     logging.getLogger("pmm_cfg_gen").debug("formatString item labels: {}".format(lstLabels))
                     result = result.replace("{{universe}}", lstLabels[0] if lstLabels[0] not in result else "")
 
         if pmm is not None:
@@ -196,24 +200,27 @@
          @param item - The item to clean. Should be a L { PlexPartialObject }.
          
          @return The cleaned title of the item as a string. Will be empty if there is no title or it is not valid
         """
         return cls.cleanString(str(item.title))
 
     @classmethod
-    def formatItemTitle(cls, item : PlexPartialObject, includeYear : bool = True, includeEdition : bool = True ) -> str:
+    def formatItemTitle(cls, item : Collection | Video | Artist, includeYear : bool = True, includeEdition : bool = True ) -> str:
 
         strFormat = "{{item.title}}"
 
         if isinstance(item, Collection):
             return PlexItemHelper.formatString(strFormat, collection=item)
-        elif isinstance(item, Video):
-            if re.match(r"[\s\S]*\([\d]{4}\)$", item.title, flags=re.DOTALL) is None:
-                strFormat += " ({{item.year}})" if includeYear else ""
-            strFormat += " [{{item.editionTitle}}]" if includeEdition and isinstance(item, Movie) else ""
+        else:
+            if isinstance(item, Video):
+                if re.match(r"[\s\S]*\([\d]{4}\)$", item.title, flags=re.DOTALL) is None:
+                    strFormat += " ({{item.year}})" if includeYear else ""
+                strFormat += " [{{item.editionTitle}}]" if includeEdition and isinstance(item, Movie) else ""
+            elif isinstance(item, Artist): 
+                pass
 
             return PlexItemHelper.formatString(strFormat, item=item)
 
         return ""
 
     @classmethod
     def getItemLabels(cls, item: PlexPartialObject) -> list[str] | None:
```

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/pmm_utils.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/pmm_utils.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/settings_utils_v1.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/settings_utils_v1.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/template_filters.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/template_filters.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/template_manager.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/template_manager.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/time_span.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/time_span.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/timer.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/timer.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/tmdb_utils.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/tmdb_utils.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/trakt_utils.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/trakt_utils.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/src/pmm_cfg_gen/utils/tvdb_utils.py` & `pmm_cfg_gen-0.2.6/src/pmm_cfg_gen/utils/tvdb_utils.py`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.5/PKG-INFO` & `pmm_cfg_gen-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmm-cfg-gen
-Version: 0.2.5
+Version: 0.2.6
 Summary: A script to help automatically generate Plex Meta Manager configuration files for your libraries
 Home-page: https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator
 License: GPL-3.0-or-later
 Keywords: pmm,plex-meta-manager,plex
 Author: Shawn Anderson
 Author-email: sanderson@eye-catcher.com
 Requires-Python: >=3.10,<4.0
@@ -32,14 +32,20 @@
 
 # Plex-Meta-Manager-Config-Generator
 
 [![PyPI version](https://badge.fury.io/py/pmm-cfg-gen.svg)](https://badge.fury.io/py/pmm-cfg-gen)
 
 A python application to automatically generate Plex Meta Manager configuration files based on your plex libraries.
 
+Library types supported:
+
+* Movie
+* TV
+* Music (json format only)
+
 ## Install
 
 ```shell
 pip install pmm-cfg-gen
 ```
 
 ## Running from command line
```

