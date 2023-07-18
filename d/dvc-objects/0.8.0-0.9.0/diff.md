# Comparing `tmp/dvc-objects-0.8.0.tar.gz` & `tmp/dvc-objects-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-objects-0.8.0.tar", last modified: Thu Oct 13 10:21:49 2022, max compression
+gzip compressed data, was "dvc-objects-0.9.0.tar", last modified: Mon Oct 17 15:43:10 2022, max compression
```

## Comparing `dvc-objects-0.8.0.tar` & `dvc-objects-0.9.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:49.513070 dvc-objects-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:49.509070 dvc-objects-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:49.509070 dvc-objects-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2048 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1380 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3066 2022-10-13 10:21:49.513070 dvc-objects-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-10-13 10:21:49.517070 dvc-objects-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:49.509070 dvc-objects-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:49.509070 dvc-objects-0.8.0/src/dvc_objects/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4797 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (121)    13871 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/db.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/executors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:49.513070 dvc-objects-0.8.0/src/dvc_objects/fs/
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11818 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/_local.py
--rw-r--r--   0 runner    (1001) docker     (121)    16028 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6604 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/local.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/path.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/scheme.py
--rw-r--r--   0 runner    (1001) docker     (121)     3356 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/system.py
--rw-r--r--   0 runner    (1001) docker     (121)     5918 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/fs/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/obj.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/src/dvc_objects/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:49.513070 dvc-objects-0.8.0/src/dvc_objects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3066 2022-10-13 10:21:49.000000 dvc-objects-0.8.0/src/dvc_objects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-10-13 10:21:49.000000 dvc-objects-0.8.0/src/dvc_objects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 10:21:49.000000 dvc-objects-0.8.0/src/dvc_objects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 10:21:49.000000 dvc-objects-0.8.0/src/dvc_objects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-10-13 10:21:49.000000 dvc-objects-0.8.0/src/dvc_objects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-13 10:21:49.000000 dvc-objects-0.8.0/src/dvc_objects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:49.513070 dvc-objects-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:49.513070 dvc-objects-0.8.0/tests/fs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/tests/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/tests/fs/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/tests/fs/test_localfs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/tests/fs/test_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/tests/fs/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7918 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/tests/test_odb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/tests/test_reflink.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-13 10:21:14.000000 dvc-objects-0.8.0/tests/test_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:43:10.324941 dvc-objects-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:43:10.320941 dvc-objects-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      737 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:43:10.320941 dvc-objects-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2048 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1380 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3066 2022-10-17 15:43:10.324941 dvc-objects-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-10-17 15:43:10.324941 dvc-objects-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:43:10.320941 dvc-objects-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:43:10.320941 dvc-objects-0.9.0/src/dvc_objects/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4797 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/_tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13871 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/executors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:43:10.324941 dvc-objects-0.9.0/src/dvc_objects/fs/
+-rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11818 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16028 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      596 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6604 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3356 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5918 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/fs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/obj.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/src/dvc_objects/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:43:10.324941 dvc-objects-0.9.0/src/dvc_objects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3066 2022-10-17 15:43:10.000000 dvc-objects-0.9.0/src/dvc_objects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-10-17 15:43:10.000000 dvc-objects-0.9.0/src/dvc_objects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 15:43:10.000000 dvc-objects-0.9.0/src/dvc_objects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 15:43:09.000000 dvc-objects-0.9.0/src/dvc_objects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-17 15:43:10.000000 dvc-objects-0.9.0/src/dvc_objects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-17 15:43:10.000000 dvc-objects-0.9.0/src/dvc_objects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:43:10.324941 dvc-objects-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:43:10.324941 dvc-objects-0.9.0/tests/fs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/tests/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/tests/fs/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3820 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/tests/fs/test_localfs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/tests/fs/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/tests/fs/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7918 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/tests/test_odb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/tests/test_reflink.py
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-17 15:42:47.000000 dvc-objects-0.9.0/tests/test_transfer.py
```

### Comparing `dvc-objects-0.8.0/.cruft.json` & `dvc-objects-0.9.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/.github/dependabot.yml` & `dvc-objects-0.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/.github/workflows/release.yml` & `dvc-objects-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/.github/workflows/tests.yml` & `dvc-objects-0.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/.gitignore` & `dvc-objects-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/.pre-commit-config.yaml` & `dvc-objects-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/CODE_OF_CONDUCT.rst` & `dvc-objects-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/CONTRIBUTING.rst` & `dvc-objects-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/LICENSE` & `dvc-objects-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/PKG-INFO` & `dvc-objects-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-objects
-Version: 0.8.0
+Version: 0.9.0
 Summary: dvc objects
 Home-page: https://github.com/iterative/dvc-objects
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-objects-0.8.0/README.rst` & `dvc-objects-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/noxfile.py` & `dvc-objects-0.9.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/pyproject.toml` & `dvc-objects-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/setup.cfg` & `dvc-objects-0.9.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 package_dir = 
 	=src
 packages = find:
 install_requires = 
 	tqdm>=4.63.1,<5
 	shortuuid>=0.5.0
 	funcy>=1.14
-	fsspec>=2021.10.1
+	fsspec>=2022.5.0
 	typing-extensions>=3.7.4
 
 [options.extras_require]
 tests = 
 	pytest==7.1.2
 	pytest-sugar==0.9.5
 	pytest-cov==3.0.0
```

### Comparing `dvc-objects-0.8.0/src/dvc_objects/_tqdm.py` & `dvc-objects-0.9.0/src/dvc_objects/_tqdm.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/db.py` & `dvc-objects-0.9.0/src/dvc_objects/db.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/executors.py` & `dvc-objects-0.9.0/src/dvc_objects/executors.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/__init__.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/_local.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/_local.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/base.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/base.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/callbacks.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/callbacks.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/errors.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/errors.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/generic.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/generic.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/local.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/local.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/memory.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/memory.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/path.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/path.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/system.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/system.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/fs/utils.py` & `dvc-objects-0.9.0/src/dvc_objects/fs/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/obj.py` & `dvc-objects-0.9.0/src/dvc_objects/obj.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects/transfer.py` & `dvc-objects-0.9.0/src/dvc_objects/transfer.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/src/dvc_objects.egg-info/PKG-INFO` & `dvc-objects-0.9.0/src/dvc_objects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-objects
-Version: 0.8.0
+Version: 0.9.0
 Summary: dvc objects
 Home-page: https://github.com/iterative/dvc-objects
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-objects-0.8.0/src/dvc_objects.egg-info/SOURCES.txt` & `dvc-objects-0.9.0/src/dvc_objects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/tests/fs/test_callbacks.py` & `dvc-objects-0.9.0/tests/fs/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/tests/fs/test_localfs.py` & `dvc-objects-0.9.0/tests/fs/test_localfs.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/tests/fs/test_system.py` & `dvc-objects-0.9.0/tests/fs/test_system.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/tests/fs/test_utils.py` & `dvc-objects-0.9.0/tests/fs/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/tests/test_odb.py` & `dvc-objects-0.9.0/tests/test_odb.py`

 * *Files identical despite different names*

### Comparing `dvc-objects-0.8.0/tests/test_reflink.py` & `dvc-objects-0.9.0/tests/test_reflink.py`

 * *Files identical despite different names*

