# Comparing `tmp/cdk-rds-dump-1.2.2.tar.gz` & `tmp/cdk-rds-dump-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-rds-dump-1.2.2.tar", last modified: Tue Jul 18 14:11:39 2023, max compression
+gzip compressed data, was "cdk-rds-dump-1.2.3.tar", last modified: Tue Jul 18 14:20:15 2023, max compression
```

## Comparing `cdk-rds-dump-1.2.2.tar` & `cdk-rds-dump-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:11:39.714419 cdk-rds-dump-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-18 14:11:39.714419 cdk-rds-dump-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:11:39.714419 cdk-rds-dump-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:11:39.710419 cdk-rds-dump-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:11:39.710419 cdk-rds-dump-1.2.2/src/cdk_rds_dump/
--rw-r--r--   0 runner    (1001) docker     (123)    21573 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:11:39.710419 cdk-rds-dump-1.2.2/src/cdk_rds_dump/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2576253 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:11:39.710419 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-18 14:11:39.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 14:11:39.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:11:39.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 14:11:39.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 14:11:39.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:20:15.084325 cdk-rds-dump-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-18 14:20:15.084325 cdk-rds-dump-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:20:15.084325 cdk-rds-dump-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:20:15.080325 cdk-rds-dump-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:20:15.080325 cdk-rds-dump-1.2.3/src/cdk_rds_dump/
+-rw-r--r--   0 runner    (1001) docker     (123)    21676 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:20:15.080325 cdk-rds-dump-1.2.3/src/cdk_rds_dump/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2576417 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:20:03.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:20:15.080325 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-18 14:20:15.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 14:20:15.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:20:15.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 14:20:15.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 14:20:15.000000 cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/top_level.txt
```

### Comparing `cdk-rds-dump-1.2.2/LICENSE` & `cdk-rds-dump-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.2.2/PKG-INFO` & `cdk-rds-dump-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 1.2.2
+Version: 1.2.3
 Summary: CDK Construct Library by Typescript for RDS Dump
-Home-page: https://github.com/malaysia.cryer/cdk-rds-dump.git
+Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
-Project-URL: Source, https://github.com/malaysia.cryer/cdk-rds-dump.git
+Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,15 +24,15 @@
 
 # cdk-rds-dump
 
 cdk-rds-dump is a Constructs library for AWS CDK that provides the functionality to dump the contents of Amazon RDS, generate it as an SQL file, and store it in Amazon S3.
 
 ![Architecture](./image/architecture.png)
 
-[![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
+[![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm version](https://badge.fury.io/js/cdk-rds-dump.svg)](https://badge.fury.io/js/cdk-rds-dump)
 [![Build Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-rds-dump.svg?style=flat)](https://www.npmjs.com/package/cdk-rds-dump)
 
 ## Usage
```

### Comparing `cdk-rds-dump-1.2.2/README.md` & `cdk-rds-dump-1.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cdk-rds-dump
 
 cdk-rds-dump is a Constructs library for AWS CDK that provides the functionality to dump the contents of Amazon RDS, generate it as an SQL file, and store it in Amazon S3.
 
 ![Architecture](./image/architecture.png)
 
-[![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
+[![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm version](https://badge.fury.io/js/cdk-rds-dump.svg)](https://badge.fury.io/js/cdk-rds-dump)
 [![Build Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-rds-dump.svg?style=flat)](https://www.npmjs.com/package/cdk-rds-dump)
 
 ## Usage
```

### Comparing `cdk-rds-dump-1.2.2/setup.py` & `cdk-rds-dump-1.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-rds-dump",
-    "version": "1.2.2",
+    "version": "1.2.3",
     "description": "CDK Construct Library by Typescript for RDS Dump",
     "license": "Apache-2.0",
-    "url": "https://github.com/malaysia.cryer/cdk-rds-dump.git",
+    "url": "https://github.com/badmintoncryer/cdk-rds-dump.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
     },
     "project_urls": {
-        "Source": "https://github.com/malaysia.cryer/cdk-rds-dump.git"
+        "Source": "https://github.com/badmintoncryer/cdk-rds-dump.git"
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "cdk_rds_dump",
         "cdk_rds_dump._jsii"
     ],
     "package_data": {
         "cdk_rds_dump._jsii": [
-            "cdk-rds-dump@1.2.2.jsii.tgz"
+            "cdk-rds-dump@1.2.3.jsii.tgz"
         ],
         "cdk_rds_dump": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-rds-dump-1.2.2/src/cdk_rds_dump/__init__.py` & `cdk-rds-dump-1.2.3/src/cdk_rds_dump/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 # cdk-rds-dump
 
 cdk-rds-dump is a Constructs library for AWS CDK that provides the functionality to dump the contents of Amazon RDS, generate it as an SQL file, and store it in Amazon S3.
 
 ![Architecture](./image/architecture.png)
 
-[![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
+[![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm version](https://badge.fury.io/js/cdk-rds-dump.svg)](https://badge.fury.io/js/cdk-rds-dump)
 [![Build Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-rds-dump.svg?style=flat)](https://www.npmjs.com/package/cdk-rds-dump)
 
 ## Usage
```

### Comparing `cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/PKG-INFO` & `cdk-rds-dump-1.2.3/src/cdk_rds_dump.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 1.2.2
+Version: 1.2.3
 Summary: CDK Construct Library by Typescript for RDS Dump
-Home-page: https://github.com/malaysia.cryer/cdk-rds-dump.git
+Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
-Project-URL: Source, https://github.com/malaysia.cryer/cdk-rds-dump.git
+Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,15 +24,15 @@
 
 # cdk-rds-dump
 
 cdk-rds-dump is a Constructs library for AWS CDK that provides the functionality to dump the contents of Amazon RDS, generate it as an SQL file, and store it in Amazon S3.
 
 ![Architecture](./image/architecture.png)
 
-[![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
+[![Open in Visual Studio Code](https://img.shields.io/static/v1?logo=visualstudiocode&label=&message=Open%20in%20Visual%20Studio%20Code&labelColor=2c2c32&color=007acc&logoColor=007acc)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![npm version](https://badge.fury.io/js/cdk-rds-dump.svg)](https://badge.fury.io/js/cdk-rds-dump)
 [![Build Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml)
 [![Release Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml)
 [![npm downloads](https://img.shields.io/npm/dm/cdk-rds-dump.svg?style=flat)](https://www.npmjs.com/package/cdk-rds-dump)
 
 ## Usage
```

