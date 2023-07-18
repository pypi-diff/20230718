# Comparing `tmp/spatiafi-1.1.8.tar.gz` & `tmp/spatiafi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatiafi-1.1.8.tar", last modified: Thu Jun 22 00:35:58 2023, max compression
+gzip compressed data, was "spatiafi-1.2.0.tar", last modified: Tue Jul 18 18:49:36 2023, max compression
```

## Comparing `spatiafi-1.1.8.tar` & `spatiafi-1.2.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3978 2023-06-12 18:08:33.000000 spatiafi-1.1.8/.dockerignore
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3996 2023-06-12 18:08:33.000000 spatiafi-1.1.8/.gitignore
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1464 2023-06-12 18:08:33.000000 spatiafi-1.1.8/.pre-commit-config.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      136 2023-06-17 16:21:46.000000 spatiafi-1.1.8/.requirements.sha256
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1148 2023-06-12 18:08:33.000000 spatiafi-1.1.8/Dockerfile
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)    11357 2023-06-12 18:08:33.000000 spatiafi-1.1.8/LICENSE
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-22 00:35:58.156515 spatiafi-1.1.8/PKG-INFO
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3683 2023-06-17 16:27:30.000000 spatiafi-1.1.8/README.md
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      845 2023-06-12 18:08:33.000000 spatiafi-1.1.8/pyproject.toml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4698 2023-06-17 16:21:46.000000 spatiafi-1.1.8/requirements-dev.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      912 2023-06-17 16:20:25.000000 spatiafi-1.1.8/requirements.txt
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/scripts/
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     1517 2023-06-12 18:08:33.000000 spatiafi-1.1.8/scripts/bootstrap_dev.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      486 2023-06-12 18:08:33.000000 spatiafi-1.1.8/scripts/build_docker.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     2074 2023-06-12 18:08:33.000000 spatiafi-1.1.8/scripts/gen_requirements.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      228 2023-06-12 18:08:33.000000 spatiafi-1.1.8/scripts/install_package.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      322 2023-06-12 18:08:33.000000 spatiafi-1.1.8/scripts/test.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      135 2023-06-21 17:00:42.000000 spatiafi-1.1.8/scripts/upload_pypi.sh
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      935 2023-06-22 00:35:58.156515 spatiafi-1.1.8/setup.cfg
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       92 2023-06-12 18:08:33.000000 spatiafi-1.1.8/setup.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.152515 spatiafi-1.1.8/src/
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/src/spatiafi/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      506 2023-06-17 16:27:44.000000 spatiafi-1.1.8/src/spatiafi/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:12:50.000000 spatiafi-1.1.8/src/spatiafi/__main__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      160 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi/_version.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2370 2023-06-12 18:12:08.000000 spatiafi-1.1.8/src/spatiafi/auth.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/src/spatiafi/gdal_auth/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       79 2023-06-18 01:03:50.000000 spatiafi-1.1.8/src/spatiafi/gdal_auth/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:27:45.000000 spatiafi-1.1.8/src/spatiafi/gdal_auth/__main__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3743 2023-06-17 16:27:45.000000 spatiafi-1.1.8/src/spatiafi/gdal_auth/cli.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     5981 2023-06-22 00:35:11.000000 spatiafi-1.1.8/src/spatiafi/gdal_auth/gdal_auth.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2054 2023-06-17 16:27:45.000000 spatiafi-1.1.8/src/spatiafi/session.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/src/spatiafi.egg-info/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/PKG-INFO
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      987 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/SOURCES.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        1 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/dependency_links.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       53 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/entry_points.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      235 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/requires.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        9 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/top_level.txt
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/tests/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-12 18:08:33.000000 spatiafi-1.1.8/tests/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       34 2023-06-12 18:08:33.000000 spatiafi-1.1.8/tests/test_dummy.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/workflows/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1674 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/README.md
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1131 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/delpoy-sensor.sh
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      440 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/kustomization.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      300 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/py-spfi-api-build-wf.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1785 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/repo-sensor.yaml
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      831 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/submit-wf.sh
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-07-18 18:49:36.939102 spatiafi-1.2.0/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3978 2023-06-12 18:08:33.000000 spatiafi-1.2.0/.dockerignore
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3996 2023-06-12 18:08:33.000000 spatiafi-1.2.0/.gitignore
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1464 2023-06-12 18:08:33.000000 spatiafi-1.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      136 2023-07-18 18:10:45.000000 spatiafi-1.2.0/.requirements.sha256
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1148 2023-06-12 18:08:33.000000 spatiafi-1.2.0/Dockerfile
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)    11357 2023-06-12 18:08:33.000000 spatiafi-1.2.0/LICENSE
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-07-18 18:49:36.939102 spatiafi-1.2.0/PKG-INFO
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3683 2023-07-18 18:10:45.000000 spatiafi-1.2.0/README.md
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      845 2023-07-18 18:48:52.000000 spatiafi-1.2.0/pyproject.toml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4698 2023-07-18 18:10:45.000000 spatiafi-1.2.0/requirements-dev.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      912 2023-07-18 18:10:45.000000 spatiafi-1.2.0/requirements.txt
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-07-18 18:49:36.939102 spatiafi-1.2.0/scripts/
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     1517 2023-06-12 18:08:33.000000 spatiafi-1.2.0/scripts/bootstrap_dev.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      486 2023-06-12 18:08:33.000000 spatiafi-1.2.0/scripts/build_docker.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     2074 2023-07-18 18:13:43.000000 spatiafi-1.2.0/scripts/gen_requirements.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      228 2023-06-12 18:08:33.000000 spatiafi-1.2.0/scripts/install_package.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      322 2023-06-12 18:08:33.000000 spatiafi-1.2.0/scripts/test.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      135 2023-07-18 18:10:45.000000 spatiafi-1.2.0/scripts/upload_pypi.sh
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      935 2023-07-18 18:49:36.939102 spatiafi-1.2.0/setup.cfg
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       92 2023-06-12 18:08:33.000000 spatiafi-1.2.0/setup.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-07-18 18:49:36.935102 spatiafi-1.2.0/src/
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-07-18 18:49:36.939102 spatiafi-1.2.0/src/spatiafi/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      506 2023-07-18 18:10:45.000000 spatiafi-1.2.0/src/spatiafi/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-07-18 18:10:45.000000 spatiafi-1.2.0/src/spatiafi/__main__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      160 2023-07-18 18:49:36.000000 spatiafi-1.2.0/src/spatiafi/_version.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2370 2023-06-12 18:12:08.000000 spatiafi-1.2.0/src/spatiafi/auth.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-07-18 18:49:36.939102 spatiafi-1.2.0/src/spatiafi/gdal_auth/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       79 2023-07-18 18:10:45.000000 spatiafi-1.2.0/src/spatiafi/gdal_auth/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-07-18 18:10:45.000000 spatiafi-1.2.0/src/spatiafi/gdal_auth/__main__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3743 2023-07-18 18:10:45.000000 spatiafi-1.2.0/src/spatiafi/gdal_auth/cli.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     5981 2023-07-18 18:10:45.000000 spatiafi-1.2.0/src/spatiafi/gdal_auth/gdal_auth.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2054 2023-07-18 18:10:45.000000 spatiafi-1.2.0/src/spatiafi/session.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-07-18 18:49:36.939102 spatiafi-1.2.0/src/spatiafi.egg-info/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-07-18 18:49:36.000000 spatiafi-1.2.0/src/spatiafi.egg-info/PKG-INFO
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      987 2023-07-18 18:49:36.000000 spatiafi-1.2.0/src/spatiafi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        1 2023-07-18 18:49:36.000000 spatiafi-1.2.0/src/spatiafi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       53 2023-07-18 18:49:36.000000 spatiafi-1.2.0/src/spatiafi.egg-info/entry_points.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      235 2023-07-18 18:49:36.000000 spatiafi-1.2.0/src/spatiafi.egg-info/requires.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        9 2023-07-18 18:49:36.000000 spatiafi-1.2.0/src/spatiafi.egg-info/top_level.txt
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-07-18 18:49:36.939102 spatiafi-1.2.0/tests/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-12 18:08:33.000000 spatiafi-1.2.0/tests/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       34 2023-06-12 18:08:33.000000 spatiafi-1.2.0/tests/test_dummy.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-07-18 18:49:36.939102 spatiafi-1.2.0/workflows/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1674 2023-06-12 18:08:33.000000 spatiafi-1.2.0/workflows/README.md
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1131 2023-06-12 18:08:33.000000 spatiafi-1.2.0/workflows/delpoy-sensor.sh
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      440 2023-06-22 02:13:14.000000 spatiafi-1.2.0/workflows/kustomization.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      300 2023-06-12 18:08:33.000000 spatiafi-1.2.0/workflows/py-spfi-api-build-wf.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1785 2023-06-12 18:08:33.000000 spatiafi-1.2.0/workflows/repo-sensor.yaml
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      831 2023-06-12 18:08:33.000000 spatiafi-1.2.0/workflows/submit-wf.sh
```

### Comparing `spatiafi-1.1.8/.dockerignore` & `spatiafi-1.2.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/.gitignore` & `spatiafi-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/.pre-commit-config.yaml` & `spatiafi-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/Dockerfile` & `spatiafi-1.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/LICENSE` & `spatiafi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/PKG-INFO` & `spatiafi-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatiafi
-Version: 1.1.8
+Version: 1.2.0
 Summary: Python library for interacting with the SpatiaFi API
 Home-page: https://github.com/climateengine/py-spfi-api
 Author: Climate Engine Team
 Author-email: admin@climateengine.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spatiafi-1.1.8/README.md` & `spatiafi-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/pyproject.toml` & `spatiafi-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/requirements-dev.txt` & `spatiafi-1.2.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/requirements.txt` & `spatiafi-1.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/scripts/bootstrap_dev.sh` & `spatiafi-1.2.0/scripts/bootstrap_dev.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/scripts/gen_requirements.sh` & `spatiafi-1.2.0/scripts/gen_requirements.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/setup.cfg` & `spatiafi-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/src/spatiafi/auth.py` & `spatiafi-1.2.0/src/spatiafi/auth.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/src/spatiafi/gdal_auth/cli.py` & `spatiafi-1.2.0/src/spatiafi/gdal_auth/cli.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/src/spatiafi/gdal_auth/gdal_auth.py` & `spatiafi-1.2.0/src/spatiafi/gdal_auth/gdal_auth.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/src/spatiafi/session.py` & `spatiafi-1.2.0/src/spatiafi/session.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/src/spatiafi.egg-info/PKG-INFO` & `spatiafi-1.2.0/src/spatiafi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatiafi
-Version: 1.1.8
+Version: 1.2.0
 Summary: Python library for interacting with the SpatiaFi API
 Home-page: https://github.com/climateengine/py-spfi-api
 Author: Climate Engine Team
 Author-email: admin@climateengine.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spatiafi-1.1.8/src/spatiafi.egg-info/SOURCES.txt` & `spatiafi-1.2.0/src/spatiafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/workflows/README.md` & `spatiafi-1.2.0/workflows/README.md`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/workflows/delpoy-sensor.sh` & `spatiafi-1.2.0/workflows/delpoy-sensor.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/workflows/repo-sensor.yaml` & `spatiafi-1.2.0/workflows/repo-sensor.yaml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.8/workflows/submit-wf.sh` & `spatiafi-1.2.0/workflows/submit-wf.sh`

 * *Files identical despite different names*

