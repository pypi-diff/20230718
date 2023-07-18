# Comparing `tmp/bibtutils-1.2.0.tar.gz` & `tmp/bibtutils-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibtutils-1.2.0.tar", last modified: Thu Jul  6 18:21:08 2023, max compression
+gzip compressed data, was "bibtutils-1.2.1.tar", last modified: Tue Jul 18 15:49:59 2023, max compression
```

## Comparing `bibtutils-1.2.0.tar` & `bibtutils-1.2.1.tar`

### file list

```diff
@@ -1,36 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.774853 bibtutils-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-06 18:20:59.000000 bibtutils-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:20:59.000000 bibtutils-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-06 18:21:08.774853 bibtutils-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 18:20:59.000000 bibtutils-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.766852 bibtutils-1.2.0/bibtutils/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.770853 bibtutils-1.2.0/bibtutils/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24430 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.770853 bibtutils-1.2.0/bibtutils/slack/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/slack/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/slack/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.766852 bibtutils-1.2.0/bibtutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 18:20:59.000000 bibtutils-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-06 18:21:08.774853 bibtutils-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:20:59.000000 bibtutils-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.770853 bibtutils-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/test_gcp_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/test_gcp_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/test_gcp_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/test_gcp_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:49:59.728368 bibtutils-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-18 15:49:50.000000 bibtutils-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:49:50.000000 bibtutils-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-18 15:49:59.728368 bibtutils-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-18 15:49:50.000000 bibtutils-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:49:59.724367 bibtutils-1.2.1/bibtutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:49:59.724367 bibtutils-1.2.1/bibtutils/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24430 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/gcp/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/gcp/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/gcp/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:49:59.724367 bibtutils-1.2.1/bibtutils/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/slack/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/slack/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 15:49:50.000000 bibtutils-1.2.1/bibtutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:49:59.724367 bibtutils-1.2.1/bibtutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-18 15:49:59.000000 bibtutils-1.2.1/bibtutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-18 15:49:59.000000 bibtutils-1.2.1/bibtutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:49:59.000000 bibtutils-1.2.1/bibtutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-18 15:49:59.000000 bibtutils-1.2.1/bibtutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:49:59.000000 bibtutils-1.2.1/bibtutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:49:59.000000 bibtutils-1.2.1/bibtutils.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-18 15:49:50.000000 bibtutils-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-18 15:49:59.728368 bibtutils-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:49:50.000000 bibtutils-1.2.1/setup.py
```

### Comparing `bibtutils-1.2.0/LICENSE` & `bibtutils-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bibtutils-1.2.0/PKG-INFO` & `bibtutils-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibtutils
-Version: 1.2.0
+Version: 1.2.1
 Summary: Functionality often used by BITS Blue Team.
 Home-page: https://github.com/broadinstitute/bibtutils
 Author: Matthew OBrien
 Author-email: mobrien@broadinstitute.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bibtutils-1.2.0/README.md` & `bibtutils-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bibtutils-1.2.0/bibtutils/gcp/bigquery.py` & `bibtutils-1.2.1/bibtutils/gcp/bigquery.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.2.0/bibtutils/gcp/iam.py` & `bibtutils-1.2.1/bibtutils/gcp/iam.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.2.0/bibtutils/gcp/pubsub.py` & `bibtutils-1.2.1/bibtutils/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.2.0/bibtutils/gcp/secrets.py` & `bibtutils-1.2.1/bibtutils/gcp/secrets.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.2.0/bibtutils/gcp/storage.py` & `bibtutils-1.2.1/bibtutils/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.2.0/bibtutils/slack/error.py` & `bibtutils-1.2.1/bibtutils/slack/error.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.2.0/bibtutils/slack/message.py` & `bibtutils-1.2.1/bibtutils/slack/message.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.2.0/bibtutils.egg-info/PKG-INFO` & `bibtutils-1.2.1/bibtutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibtutils
-Version: 1.2.0
+Version: 1.2.1
 Summary: Functionality often used by BITS Blue Team.
 Home-page: https://github.com/broadinstitute/bibtutils
 Author: Matthew OBrien
 Author-email: mobrien@broadinstitute.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bibtutils-1.2.0/setup.cfg` & `bibtutils-1.2.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bibtutils
-version = 1.2.0
+version = 1.2.1
 author = Matthew OBrien
 author_email = mobrien@broadinstitute.org
 description = Functionality often used by BITS Blue Team.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/broadinstitute/bibtutils
 license = MIT
```

