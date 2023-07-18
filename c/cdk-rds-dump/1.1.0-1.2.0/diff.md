# Comparing `tmp/cdk-rds-dump-1.1.0.tar.gz` & `tmp/cdk-rds-dump-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-rds-dump-1.1.0.tar", last modified: Tue Jul 18 10:09:25 2023, max compression
+gzip compressed data, was "cdk-rds-dump-1.2.0.tar", last modified: Tue Jul 18 12:52:26 2023, max compression
```

## Comparing `cdk-rds-dump-1.1.0.tar` & `cdk-rds-dump-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:09:25.112844 cdk-rds-dump-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 10:09:11.000000 cdk-rds-dump-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 10:09:11.000000 cdk-rds-dump-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 10:09:25.108844 cdk-rds-dump-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-18 10:09:11.000000 cdk-rds-dump-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 10:09:11.000000 cdk-rds-dump-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:09:25.112844 cdk-rds-dump-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-18 10:09:11.000000 cdk-rds-dump-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:09:25.104844 cdk-rds-dump-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:09:25.108844 cdk-rds-dump-1.1.0/src/cdk_rds_dump/
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-07-18 10:09:11.000000 cdk-rds-dump-1.1.0/src/cdk_rds_dump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:09:25.108844 cdk-rds-dump-1.1.0/src/cdk_rds_dump/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 10:09:11.000000 cdk-rds-dump-1.1.0/src/cdk_rds_dump/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1860486 2023-07-18 10:09:11.000000 cdk-rds-dump-1.1.0/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:09:11.000000 cdk-rds-dump-1.1.0/src/cdk_rds_dump/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:09:25.108844 cdk-rds-dump-1.1.0/src/cdk_rds_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 10:09:25.000000 cdk-rds-dump-1.1.0/src/cdk_rds_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 10:09:25.000000 cdk-rds-dump-1.1.0/src/cdk_rds_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:09:25.000000 cdk-rds-dump-1.1.0/src/cdk_rds_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 10:09:25.000000 cdk-rds-dump-1.1.0/src/cdk_rds_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 10:09:25.000000 cdk-rds-dump-1.1.0/src/cdk_rds_dump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:52:26.036585 cdk-rds-dump-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 12:52:13.000000 cdk-rds-dump-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 12:52:13.000000 cdk-rds-dump-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 12:52:26.036585 cdk-rds-dump-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-18 12:52:13.000000 cdk-rds-dump-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 12:52:13.000000 cdk-rds-dump-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 12:52:26.036585 cdk-rds-dump-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-18 12:52:13.000000 cdk-rds-dump-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:52:26.032585 cdk-rds-dump-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:52:26.032585 cdk-rds-dump-1.2.0/src/cdk_rds_dump/
+-rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-07-18 12:52:13.000000 cdk-rds-dump-1.2.0/src/cdk_rds_dump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:52:26.032585 cdk-rds-dump-1.2.0/src/cdk_rds_dump/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 12:52:13.000000 cdk-rds-dump-1.2.0/src/cdk_rds_dump/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2405653 2023-07-18 12:52:13.000000 cdk-rds-dump-1.2.0/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:52:13.000000 cdk-rds-dump-1.2.0/src/cdk_rds_dump/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:52:26.032585 cdk-rds-dump-1.2.0/src/cdk_rds_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 12:52:26.000000 cdk-rds-dump-1.2.0/src/cdk_rds_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 12:52:26.000000 cdk-rds-dump-1.2.0/src/cdk_rds_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:52:26.000000 cdk-rds-dump-1.2.0/src/cdk_rds_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 12:52:26.000000 cdk-rds-dump-1.2.0/src/cdk_rds_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 12:52:26.000000 cdk-rds-dump-1.2.0/src/cdk_rds_dump.egg-info/top_level.txt
```

### Comparing `cdk-rds-dump-1.1.0/LICENSE` & `cdk-rds-dump-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.1.0/PKG-INFO` & `cdk-rds-dump-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 1.1.0
+Version: 1.2.0
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/malaysia.cryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/malaysia.cryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-rds-dump-1.1.0/README.md` & `cdk-rds-dump-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.1.0/setup.py` & `cdk-rds-dump-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-rds-dump",
-    "version": "1.1.0",
+    "version": "1.2.0",
     "description": "CDK Construct Library by Typescript for RDS Dump",
     "license": "Apache-2.0",
     "url": "https://github.com/malaysia.cryer/cdk-rds-dump.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_rds_dump",
         "cdk_rds_dump._jsii"
     ],
     "package_data": {
         "cdk_rds_dump._jsii": [
-            "cdk-rds-dump@1.1.0.jsii.tgz"
+            "cdk-rds-dump@1.2.0.jsii.tgz"
         ],
         "cdk_rds_dump": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-rds-dump-1.1.0/src/cdk_rds_dump.egg-info/PKG-INFO` & `cdk-rds-dump-1.2.0/src/cdk_rds_dump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 1.1.0
+Version: 1.2.0
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/malaysia.cryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/malaysia.cryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

