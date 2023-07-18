# Comparing `tmp/molgenis_emx2_pyclient-8.206.1.tar.gz` & `tmp/molgenis_emx2_pyclient-8.207.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis_emx2_pyclient-8.206.1.tar", last modified: Mon Jul 17 10:10:57 2023, max compression
+gzip compressed data, was "molgenis_emx2_pyclient-8.207.0.tar", last modified: Tue Jul 18 05:20:03 2023, max compression
```

## Comparing `molgenis_emx2_pyclient-8.206.1.tar` & `molgenis_emx2_pyclient-8.207.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:10:57.790853 molgenis_emx2_pyclient-8.206.1/
--rw-r--r--   0 root         (0) root         (0)     7631 2023-07-17 10:01:02.000000 molgenis_emx2_pyclient-8.206.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-17 10:10:57.790853 molgenis_emx2_pyclient-8.206.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-17 10:01:02.000000 molgenis_emx2_pyclient-8.206.1/README.md
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-17 10:01:02.000000 molgenis_emx2_pyclient-8.206.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-17 10:01:02.000000 molgenis_emx2_pyclient-8.206.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 10:10:57.790853 molgenis_emx2_pyclient-8.206.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:10:57.790853 molgenis_emx2_pyclient-8.206.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:10:57.790853 molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient/
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-17 10:01:02.000000 molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-07-17 10:01:02.000000 molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:10:57.790853 molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1342 2023-07-17 10:10:57.000000 molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2023-07-17 10:10:57.000000 molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 10:10:57.000000 molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-17 10:10:57.000000 molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-17 10:10:57.000000 molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 10:06:55.000000 molgenis_emx2_pyclient-8.206.1/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:20:03.912136 molgenis_emx2_pyclient-8.207.0/
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-07-18 05:10:37.000000 molgenis_emx2_pyclient-8.207.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-18 05:20:03.912136 molgenis_emx2_pyclient-8.207.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-18 05:10:37.000000 molgenis_emx2_pyclient-8.207.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-18 05:10:37.000000 molgenis_emx2_pyclient-8.207.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-18 05:10:37.000000 molgenis_emx2_pyclient-8.207.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 05:20:03.912136 molgenis_emx2_pyclient-8.207.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:20:03.908136 molgenis_emx2_pyclient-8.207.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:20:03.912136 molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-18 05:10:37.000000 molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-07-18 05:10:37.000000 molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:20:03.912136 molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-07-18 05:20:03.000000 molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      386 2023-07-18 05:20:03.000000 molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 05:20:03.000000 molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-18 05:20:03.000000 molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-18 05:20:03.000000 molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-18 05:16:05.000000 molgenis_emx2_pyclient-8.207.0/version.txt
```

### Comparing `molgenis_emx2_pyclient-8.206.1/LICENSE` & `molgenis_emx2_pyclient-8.207.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.206.1/PKG-INFO` & `molgenis_emx2_pyclient-8.207.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: molgenis_emx2_pyclient
-Version: 8.206.1
-Summary: Python client for the Molgenis EMX2 API
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Installation
 
     pip install molgenis_emx2_pyclient
 
 # How to use
 Within your Python project import the class Client and use it to sign in
```

### Comparing `molgenis_emx2_pyclient-8.206.1/pyproject.toml` & `molgenis_emx2_pyclient-8.207.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient/client.py` & `molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient/client.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.206.1/src/molgenis_emx2_pyclient.egg-info/PKG-INFO` & `molgenis_emx2_pyclient-8.207.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-pyclient
-Version: 8.206.1
+Version: 8.207.0
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

