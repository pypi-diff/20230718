# Comparing `tmp/ckanext-statistics-3.1.7.tar.gz` & `tmp/ckanext-statistics-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-statistics-3.1.7.tar", last modified: Mon Jul 17 08:24:52 2023, max compression
+gzip compressed data, was "ckanext-statistics-3.1.8.tar", last modified: Tue Jul 18 09:54:58 2023, max compression
```

## Comparing `ckanext-statistics-3.1.7.tar` & `ckanext-statistics-3.1.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.548147 ckanext-statistics-3.1.7/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.548147 ckanext-statistics-3.1.7/ckanext/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.548147 ckanext-statistics-3.1.7/ckanext/statistics/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/data/data-portal-backfill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.548147 ckanext-statistics-3.1.7/ckanext/statistics/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/lib/dataset_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/lib/download_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/lib/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/ckanext/statistics/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/logic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/logic/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/ckanext/statistics/model/
--rwxr-xr-x   0 runner    (1001) docker     (123)      139 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/model/gbif_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/ckanext/statistics/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:24:52.000000 ckanext-statistics-3.1.7/ckanext_statistics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.548147 ckanext-statistics-3.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:52.552147 ckanext-statistics-3.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-07-17 08:24:38.000000 ckanext-statistics-3.1.7/tests/test_download_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.837638 ckanext-statistics-3.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-18 09:54:58.833639 ckanext-statistics-3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.833639 ckanext-statistics-3.1.8/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.833639 ckanext-statistics-3.1.8/ckanext/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.833639 ckanext-statistics-3.1.8/ckanext/statistics/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/data/data-portal-backfill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.833639 ckanext-statistics-3.1.8/ckanext/statistics/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/lib/dataset_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/lib/download_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/lib/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.833639 ckanext-statistics-3.1.8/ckanext/statistics/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/logic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/logic/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.833639 ckanext-statistics-3.1.8/ckanext/statistics/model/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      139 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/model/gbif_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/ckanext/statistics/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.833639 ckanext-statistics-3.1.8/ckanext_statistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-18 09:54:58.000000 ckanext-statistics-3.1.8/ckanext_statistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-18 09:54:58.000000 ckanext-statistics-3.1.8/ckanext_statistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:54:58.000000 ckanext-statistics-3.1.8/ckanext_statistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 09:54:58.000000 ckanext-statistics-3.1.8/ckanext_statistics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:54:58.000000 ckanext-statistics-3.1.8/ckanext_statistics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 09:54:58.000000 ckanext-statistics-3.1.8/ckanext_statistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 09:54:58.000000 ckanext-statistics-3.1.8/ckanext_statistics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.829639 ckanext-statistics-3.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.833639 ckanext-statistics-3.1.8/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:54:58.837638 ckanext-statistics-3.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:54:58.833639 ckanext-statistics-3.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20014 2023-07-18 09:54:47.000000 ckanext-statistics-3.1.8/tests/test_download_statistics.py
```

### Comparing `ckanext-statistics-3.1.7/LICENSE` & `ckanext-statistics-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/PKG-INFO` & `ckanext-statistics-3.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-statistics
-Version: 3.1.7
+Version: 3.1.8
 Summary: A CKAN extension for accessing instance statistics.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-statistics
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-statistics/blob/main/CHANGELOG.md
 Keywords: CKAN,data,statistics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-statistics-3.1.7/README.md` & `ckanext-statistics-3.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/ckanext/statistics/cli.py` & `ckanext-statistics-3.1.8/ckanext/statistics/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/ckanext/statistics/data/data-portal-backfill.json` & `ckanext-statistics-3.1.8/ckanext/statistics/data/data-portal-backfill.json`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/ckanext/statistics/lib/dataset_statistics.py` & `ckanext-statistics-3.1.8/ckanext/statistics/lib/dataset_statistics.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/ckanext/statistics/lib/download_statistics.py` & `ckanext-statistics-3.1.8/ckanext/statistics/lib/download_statistics.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/ckanext/statistics/lib/statistics.py` & `ckanext-statistics-3.1.8/ckanext/statistics/lib/statistics.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/ckanext/statistics/logic/action.py` & `ckanext-statistics-3.1.8/ckanext/statistics/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/ckanext/statistics/logic/schema.py` & `ckanext-statistics-3.1.8/ckanext/statistics/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/ckanext/statistics/model/gbif_download.py` & `ckanext-statistics-3.1.8/ckanext/statistics/model/gbif_download.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/ckanext/statistics/plugin.py` & `ckanext-statistics-3.1.8/ckanext/statistics/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/ckanext_statistics.egg-info/PKG-INFO` & `ckanext-statistics-3.1.8/ckanext_statistics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-statistics
-Version: 3.1.7
+Version: 3.1.8
 Summary: A CKAN extension for accessing instance statistics.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-statistics
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-statistics/blob/main/CHANGELOG.md
 Keywords: CKAN,data,statistics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-statistics-3.1.7/ckanext_statistics.egg-info/SOURCES.txt` & `ckanext-statistics-3.1.8/ckanext_statistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/docs/_scripts/gen_api_pages.py` & `ckanext-statistics-3.1.8/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-statistics-3.1.7/pyproject.toml` & `ckanext-statistics-3.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-statistics"
-version = "3.1.7"
+version = "3.1.8"
 description = "A CKAN extension for accessing instance statistics."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -18,16 +18,16 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8"
 ]
 dependencies = [
     "importlib-resources",
     "requests",
     "tqdm>=4.55.1",
-    "ckanext-ckanpackager~=2.2.0",
-    "ckanext-versioned-datastore~=4.2.0",
+    "ckanext-ckanpackager~=3.0.0",
+    "ckanext-versioned-datastore~=5.0.0",
     "ckantools>=0.3.0"
 ]
 
 [project.optional-dependencies]
 test = [
     "mock",
     "pytest>=4.6.5",
@@ -57,15 +57,15 @@
 
 [tool.setuptools.package-data]
 "ckanext.statistics.theme" = ["*", "**/*"]
 "ckanext.statistics.data" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "3.1.7"
+version = "3.1.8"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-statistics-3.1.7/tests/test_download_statistics.py` & `ckanext-statistics-3.1.8/tests/test_download_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,14 +301,15 @@
     Simple fixture which resets the database and creates the tables we need from this
     extension plus the versioned datastore and ckanpackager extensions.
     """
     reset_db()
     tables = [
         stats.import_stats_table,
         slugs.datastore_slugs_table,
+        slugs.navigational_slugs_table,
         details.datastore_resource_details_table,
         downloads.datastore_downloads_core_files_table,
         downloads.datastore_downloads_derivative_files_table,
         downloads.datastore_downloads_requests_table,
         ckanpackager_stats_table,
         gbif_downloads_table,
     ]
```

