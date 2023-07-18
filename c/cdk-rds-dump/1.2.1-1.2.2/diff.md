# Comparing `tmp/cdk-rds-dump-1.2.1.tar.gz` & `tmp/cdk-rds-dump-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-rds-dump-1.2.1.tar", last modified: Tue Jul 18 13:11:56 2023, max compression
+gzip compressed data, was "cdk-rds-dump-1.2.2.tar", last modified: Tue Jul 18 14:11:39 2023, max compression
```

## Comparing `cdk-rds-dump-1.2.1.tar` & `cdk-rds-dump-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:11:56.514784 cdk-rds-dump-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 13:11:43.000000 cdk-rds-dump-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 13:11:43.000000 cdk-rds-dump-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 13:11:56.514784 cdk-rds-dump-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-18 13:11:43.000000 cdk-rds-dump-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 13:11:43.000000 cdk-rds-dump-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:11:56.514784 cdk-rds-dump-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-18 13:11:43.000000 cdk-rds-dump-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:11:56.510784 cdk-rds-dump-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:11:56.510784 cdk-rds-dump-1.2.1/src/cdk_rds_dump/
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-07-18 13:11:43.000000 cdk-rds-dump-1.2.1/src/cdk_rds_dump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:11:56.510784 cdk-rds-dump-1.2.1/src/cdk_rds_dump/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 13:11:43.000000 cdk-rds-dump-1.2.1/src/cdk_rds_dump/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2405664 2023-07-18 13:11:43.000000 cdk-rds-dump-1.2.1/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:11:43.000000 cdk-rds-dump-1.2.1/src/cdk_rds_dump/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:11:56.510784 cdk-rds-dump-1.2.1/src/cdk_rds_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 13:11:56.000000 cdk-rds-dump-1.2.1/src/cdk_rds_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 13:11:56.000000 cdk-rds-dump-1.2.1/src/cdk_rds_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:11:56.000000 cdk-rds-dump-1.2.1/src/cdk_rds_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 13:11:56.000000 cdk-rds-dump-1.2.1/src/cdk_rds_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 13:11:56.000000 cdk-rds-dump-1.2.1/src/cdk_rds_dump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:11:39.714419 cdk-rds-dump-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-18 14:11:39.714419 cdk-rds-dump-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:11:39.714419 cdk-rds-dump-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:11:39.710419 cdk-rds-dump-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:11:39.710419 cdk-rds-dump-1.2.2/src/cdk_rds_dump/
+-rw-r--r--   0 runner    (1001) docker     (123)    21573 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:11:39.710419 cdk-rds-dump-1.2.2/src/cdk_rds_dump/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2576253 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump/_jsii/cdk-rds-dump@1.2.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:11:18.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:11:39.710419 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-18 14:11:39.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 14:11:39.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:11:39.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 14:11:39.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 14:11:39.000000 cdk-rds-dump-1.2.2/src/cdk_rds_dump.egg-info/top_level.txt
```

### Comparing `cdk-rds-dump-1.2.1/LICENSE` & `cdk-rds-dump-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-1.2.1/setup.py` & `cdk-rds-dump-1.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-rds-dump",
-    "version": "1.2.1",
+    "version": "1.2.2",
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
-            "cdk-rds-dump@1.2.1.jsii.tgz"
+            "cdk-rds-dump@1.2.2.jsii.tgz"
         ],
         "cdk_rds_dump": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-rds-dump-1.2.1/src/cdk_rds_dump/__init__.py` & `cdk-rds-dump-1.2.2/src/cdk_rds_dump/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,63 @@
 '''
-# Under construction!!!!!!!
-
 # cdk-rds-dump
 
-CDK constructs that dump the contents of AWS RDS, generate SQL files, and save them to S3
+cdk-rds-dump is a Constructs library for AWS CDK that provides the functionality to dump the contents of Amazon RDS, generate it as an SQL file, and store it in Amazon S3.
+
+![Architecture](./image/architecture.png)
+
+[![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/badmintoncryer/cdk-rds-dump)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![npm version](https://badge.fury.io/js/cdk-rds-dump.svg)](https://badge.fury.io/js/cdk-rds-dump)
+[![Build Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/build.yml)
+[![Release Status](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml/badge.svg)](https://github.com/badmintoncryer/cdk-rds-dump/actions/workflows/release.yml)
+[![npm downloads](https://img.shields.io/npm/dm/cdk-rds-dump.svg?style=flat)](https://www.npmjs.com/package/cdk-rds-dump)
+
+## Usage
+
+Install from npm:
+
+```sh
+npm i cdk-rds-dump
+```
+
+Then write CDK code as below:
+
+```python
+import { RdsDump } from 'cdk-rds-dump';
+
+declare const rdsCluster: rds.DatabaseCluster;
+new RdsDump(this, 'MyRdsDump', {
+  dbEngine: "mysql",
+  rdsCluster: rdsCluster,
+  schedule: events.Schedule.cron({ minute: "0", hour: "0" }),
+  databaseName: 'myDatabase',
+  createSecretsManagerVPCEndpoint: false,
+});
+```
+
+## How does it work?
+
+This code creates a new RDS cluster and uses the RdsDump Construct to dump the data from that RDS cluster. The dumped data is generated as an SQL file and stored in Amazon S3.
+
+For detailed usage and details of the parameters, refer to the API documentation.
+
+## Why do we need this construct?
 
-# Welcome to your CDK TypeScript Construct Library project
+AWS RDS is a very useful managed RDB service and includes, by default, the ability to create snapshots.
+However, in some cases, such as for development reasons, it is easier to handle SQL files dumped from the DB.
+Therefore, cdk-rds-dump was created as a construct to easily create SQL files on a regular basis.
 
-You should explore the contents of this project. It demonstrates a CDK Construct Library that includes a construct (`CdkRdsDump`)
-which contains an Amazon SQS queue that is subscribed to an Amazon SNS topic.
+## Contribution
 
-The construct defines an interface (`CdkRdsDumpProps`) to configure the visibility timeout of the queue.
+Contributions to the project are welcome. Submit improvement proposals via pull requests or propose new features.
 
-## Useful commands
+## License
 
-* `npm run build`   compile typescript to js
-* `npm run watch`   watch for changes and compile
-* `npm run test`    perform the jest unit tests
+This project is licensed under the Apache-2.0 License.
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
```

