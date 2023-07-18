# Comparing `tmp/federated-content-connector-1.1.0.tar.gz` & `tmp/federated-content-connector-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "federated-content-connector-1.1.0.tar", last modified: Wed Jun 21 07:01:48 2023, max compression
+gzip compressed data, was "federated-content-connector-1.2.0.tar", last modified: Tue Jul 18 13:07:34 2023, max compression
```

## Comparing `federated-content-connector-1.1.0.tar` & `federated-content-connector-1.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.831844 federated-content-connector-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-21 07:01:48.831844 federated-content-connector-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.823843 federated-content-connector-1.1.0/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    10613 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/course_metadata_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/filters/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/management/commands/import_course_runs_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     3821 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/management/commands/refresh_course_runs_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/migrations/0002_coursedetailsimportstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.819843 federated-content-connector-1.1.0/federated_content_connector/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/federated_content_connector/templates/federated_content_connector/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/templates/federated_content_connector/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/federated_content_connector/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.823843 federated-content-connector-1.1.0/federated_content_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-21 07:01:48.000000 federated-content-connector-1.1.0/federated_content_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-21 07:01:48.831844 federated-content-connector-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 07:01:48.827844 federated-content-connector-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-21 07:01:41.000000 federated-content-connector-1.1.0/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6576 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.177981 federated-content-connector-1.2.0/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10362 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/course_metadata_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.177981 federated-content-connector-1.2.0/federated_content_connector/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/filters/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.177981 federated-content-connector-1.2.0/federated_content_connector/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/federated_content_connector/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/management/commands/import_course_runs_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3821 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/management/commands/refresh_course_runs_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/federated_content_connector/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/migrations/0002_coursedetailsimportstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/federated_content_connector/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.173981 federated-content-connector-1.2.0/federated_content_connector/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/federated_content_connector/templates/federated_content_connector/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/templates/federated_content_connector/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/federated_content_connector/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.177981 federated-content-connector-1.2.0/federated_content_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-18 13:07:34.000000 federated-content-connector-1.2.0/federated_content_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5383 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 13:07:34.181981 federated-content-connector-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-07-18 13:07:26.000000 federated-content-connector-1.2.0/tests/test_signals.py
```

### Comparing `federated-content-connector-1.1.0/CHANGELOG.rst` & `federated-content-connector-1.2.0/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.2.0 – 2023-07-18
+------------------
+* Refactor `import_course_runs_metadata` command to import all courseruns
+
 1.1.0 – 2023-06-21
 ------------------
 * Management command to refresh CourseDetails data
 
 1.0.3 – 2023-06-15
 ------------------
 * backfill all data
```

### Comparing `federated-content-connector-1.1.0/LICENSE.txt` & `federated-content-connector-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/PKG-INFO` & `federated-content-connector-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.1.0
+Version: 1.2.0
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.2.0 – 2023-07-18
+------------------
+* Refactor `import_course_runs_metadata` command to import all courseruns
+
 1.1.0 – 2023-06-21
 ------------------
 * Management command to refresh CourseDetails data
 
 1.0.3 – 2023-06-15
 ------------------
 * backfill all data
```

### Comparing `federated-content-connector-1.1.0/README.rst` & `federated-content-connector-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/federated_content_connector/apps.py` & `federated-content-connector-1.2.0/federated_content_connector/apps.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/federated_content_connector/course_metadata_importer.py` & `federated-content-connector-1.2.0/federated_content_connector/course_metadata_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Course metadata importer."""
 
-import datetime
 import logging
 from urllib.parse import quote_plus, urlencode, urljoin
 
-import pytz
 from common.djangoapps.course_modes.models import CourseMode
 from django.contrib.auth import get_user_model
-from django.db.models import Q
 from openedx.core.djangoapps.catalog.models import CatalogIntegration
 from openedx.core.djangoapps.catalog.utils import get_catalog_api_base_url, get_catalog_api_client
 from openedx.core.djangoapps.content.course_overviews.models import CourseOverview
 
+from federated_content_connector.constants import BOOTCAMP_2U, EXEC_ED_COURSE_TYPE
 from federated_content_connector.models import CourseDetails
 
-EXEC_ED_COURSE_TYPE = "executive-education-2u"
 BEST_MODE_ORDER = [
     CourseMode.VERIFIED,
     CourseMode.PROFESSIONAL,
     CourseMode.NO_ID_PROFESSIONAL_MODE,
     CourseMode.UNPAID_EXECUTIVE_EDUCATION,
     CourseMode.AUDIT,
 ]
@@ -102,27 +99,17 @@
             logger.info(f'[COURSE_METADATA_IMPORTER] Import completed. Courses: {courserun_keys}')
 
         logger.info('[COURSE_METADATA_IMPORTER] Course metadata import completed for all courses.')
 
     @classmethod
     def courserun_locators_to_import(cls):
         """
-        Construct list of active course locators for which we want to import data.
+        Construct list of all course locators for which we want to import data.
         """
-        now = datetime.datetime.now(pytz.UTC)
-        return list(CourseOverview.objects.filter(
-            Q(end__gt=now) &
-            (
-                Q(enrollment_end__gt=now) |
-                Q(enrollment_end__isnull=True)
-            )
-        ).values_list(
-            'id',
-            flat=True
-        ))
+        return list(CourseOverview.objects.all().values_list('id', flat=True))
 
     @classmethod
     def fetch_courses_details(cls, client, courserun_locators, api_base_url):
         """
         Fetch the course data from discovery using `/api/v1/courses` endpoint.
         """
         course_keys = [cls.construct_course_key(courserun_locator) for courserun_locator in courserun_locators]
@@ -191,15 +178,15 @@
             course_type = course_metadata.get('course_type') or ''
             product_source = course_metadata.get('product_source') or ''
             if product_source:
                 product_source = product_source.get('slug')
 
             enroll_by = start_date = end_date = None
 
-            if course_type == EXEC_ED_COURSE_TYPE:
+            if course_type in (EXEC_ED_COURSE_TYPE, BOOTCAMP_2U):
                 additional_metadata = course_metadata.get('additional_metadata')
                 if additional_metadata:
                     enroll_by = additional_metadata.get('registration_deadline')
                     start_date = additional_metadata.get('start_date')
                     end_date = additional_metadata.get('end_date')
             else:
                 course_run = cls.find_attr(course_metadata.get('course_runs'), 'key', courserun_key)
```

### Comparing `federated-content-connector-1.1.0/federated_content_connector/filters/pipeline.py` & `federated-content-connector-1.2.0/federated_content_connector/filters/pipeline.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/federated_content_connector/management/commands/refresh_course_runs_metadata.py` & `federated-content-connector-1.2.0/federated_content_connector/management/commands/refresh_course_runs_metadata.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/federated_content_connector/migrations/0001_initial.py` & `federated-content-connector-1.2.0/federated_content_connector/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/federated_content_connector/migrations/0002_coursedetailsimportstatus.py` & `federated-content-connector-1.2.0/federated_content_connector/migrations/0002_coursedetailsimportstatus.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/federated_content_connector/models.py` & `federated-content-connector-1.2.0/federated_content_connector/models.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/federated_content_connector/signals.py` & `federated-content-connector-1.2.0/federated_content_connector/signals.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/federated_content_connector/tasks.py` & `federated-content-connector-1.2.0/federated_content_connector/tasks.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/federated_content_connector/templates/federated_content_connector/base.html` & `federated-content-connector-1.2.0/federated_content_connector/templates/federated_content_connector/base.html`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/federated_content_connector.egg-info/PKG-INFO` & `federated-content-connector-1.2.0/federated_content_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-content-connector
-Version: 1.1.0
+Version: 1.2.0
 Summary: One-line description for README and other doc files.
 Home-page: https://github.com/openedx/federated-content-connector
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -227,14 +227,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.2.0 – 2023-07-18
+------------------
+* Refactor `import_course_runs_metadata` command to import all courseruns
+
 1.1.0 – 2023-06-21
 ------------------
 * Management command to refresh CourseDetails data
 
 1.0.3 – 2023-06-15
 ------------------
 * backfill all data
```

### Comparing `federated-content-connector-1.1.0/federated_content_connector.egg-info/SOURCES.txt` & `federated-content-connector-1.2.0/federated_content_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/requirements/constraints.txt` & `federated-content-connector-1.2.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/setup.py` & `federated-content-connector-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `federated-content-connector-1.1.0/tests/test_signals.py` & `federated-content-connector-1.2.0/tests/test_signals.py`

 * *Files identical despite different names*

