# Comparing `tmp/eb-create-environment-0.0.5.tar.gz` & `tmp/eb-create-environment-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eb-create-environment-0.0.5.tar", last modified: Thu Sep 15 18:07:33 2022, max compression
+gzip compressed data, was "eb-create-environment-0.1.0.tar", last modified: Mon Jul 17 22:24:53 2023, max compression
```

## Comparing `eb-create-environment-0.0.5.tar` & `eb-create-environment-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2022-09-15 18:07:33.037272 eb-create-environment-0.0.5/
--rw-r--r--   0 zags      (1000) zags      (1000)     1080 2021-03-12 16:36:03.000000 eb-create-environment-0.0.5/LICENSE
--rw-r--r--   0 zags      (1000) zags      (1000)     3836 2022-09-15 18:07:33.037272 eb-create-environment-0.0.5/PKG-INFO
--rw-r--r--   0 zags      (1000) zags      (1000)     3243 2022-09-15 18:07:21.000000 eb-create-environment-0.0.5/README.md
-drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2022-09-15 18:07:33.037272 eb-create-environment-0.0.5/eb_create_environment/
--rw-r--r--   0 zags      (1000) zags      (1000)        0 2021-03-12 16:36:03.000000 eb-create-environment-0.0.5/eb_create_environment/__init__.py
--rw-r--r--   0 zags      (1000) zags      (1000)     6606 2022-09-15 18:07:21.000000 eb-create-environment-0.0.5/eb_create_environment/database.py
--rw-r--r--   0 zags      (1000) zags      (1000)     1617 2022-07-18 18:38:09.000000 eb-create-environment-0.0.5/eb_create_environment/default_config.yml
--rw-r--r--   0 zags      (1000) zags      (1000)     8013 2022-07-18 18:35:42.000000 eb-create-environment-0.0.5/eb_create_environment/eb_setup.py
--rw-r--r--   0 zags      (1000) zags      (1000)     9687 2022-09-15 18:07:21.000000 eb-create-environment-0.0.5/eb_create_environment/script.py
--rw-r--r--   0 zags      (1000) zags      (1000)      566 2021-03-12 16:36:04.000000 eb-create-environment-0.0.5/eb_create_environment/utils.py
--rw-r--r--   0 zags      (1000) zags      (1000)     2718 2021-11-22 22:41:44.000000 eb-create-environment-0.0.5/eb_create_environment/vpc.py
-drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2022-09-15 18:07:33.037272 eb-create-environment-0.0.5/eb_create_environment.egg-info/
--rw-r--r--   0 zags      (1000) zags      (1000)     3836 2022-09-15 18:07:33.000000 eb-create-environment-0.0.5/eb_create_environment.egg-info/PKG-INFO
--rw-r--r--   0 zags      (1000) zags      (1000)      533 2022-09-15 18:07:33.000000 eb-create-environment-0.0.5/eb_create_environment.egg-info/SOURCES.txt
--rw-r--r--   0 zags      (1000) zags      (1000)        1 2022-09-15 18:07:33.000000 eb-create-environment-0.0.5/eb_create_environment.egg-info/dependency_links.txt
--rw-r--r--   0 zags      (1000) zags      (1000)       76 2022-09-15 18:07:33.000000 eb-create-environment-0.0.5/eb_create_environment.egg-info/entry_points.txt
--rw-r--r--   0 zags      (1000) zags      (1000)       38 2022-09-15 18:07:33.000000 eb-create-environment-0.0.5/eb_create_environment.egg-info/requires.txt
--rw-r--r--   0 zags      (1000) zags      (1000)       22 2022-09-15 18:07:33.000000 eb-create-environment-0.0.5/eb_create_environment.egg-info/top_level.txt
--rw-r--r--   0 zags      (1000) zags      (1000)       38 2022-09-15 18:07:33.037272 eb-create-environment-0.0.5/setup.cfg
--rw-r--r--   0 zags      (1000) zags      (1000)     1124 2022-09-15 18:07:21.000000 eb-create-environment-0.0.5/setup.py
+drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2023-07-17 22:24:53.887081 eb-create-environment-0.1.0/
+-rw-r--r--   0 zags      (1000) zags      (1000)     1080 2021-03-12 16:36:03.000000 eb-create-environment-0.1.0/LICENSE
+-rw-r--r--   0 zags      (1000) zags      (1000)     3836 2023-07-17 22:24:53.887081 eb-create-environment-0.1.0/PKG-INFO
+-rw-r--r--   0 zags      (1000) zags      (1000)     3243 2022-09-15 18:07:21.000000 eb-create-environment-0.1.0/README.md
+drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2023-07-17 22:24:53.887081 eb-create-environment-0.1.0/eb_create_environment/
+-rw-r--r--   0 zags      (1000) zags      (1000)        0 2021-03-12 16:36:03.000000 eb-create-environment-0.1.0/eb_create_environment/__init__.py
+-rw-r--r--   0 zags      (1000) zags      (1000)       22 2023-07-17 21:39:30.000000 eb-create-environment-0.1.0/eb_create_environment/_version.py
+-rw-r--r--   0 zags      (1000) zags      (1000)     7114 2023-07-17 21:30:59.000000 eb-create-environment-0.1.0/eb_create_environment/database.py
+-rw-r--r--   0 zags      (1000) zags      (1000)     1617 2023-07-17 21:33:31.000000 eb-create-environment-0.1.0/eb_create_environment/default_config.yml
+-rw-r--r--   0 zags      (1000) zags      (1000)     8013 2022-07-18 18:35:42.000000 eb-create-environment-0.1.0/eb_create_environment/eb_setup.py
+-rw-r--r--   0 zags      (1000) zags      (1000)     9882 2023-07-17 21:41:37.000000 eb-create-environment-0.1.0/eb_create_environment/script.py
+-rw-r--r--   0 zags      (1000) zags      (1000)      566 2021-03-12 16:36:04.000000 eb-create-environment-0.1.0/eb_create_environment/utils.py
+-rw-r--r--   0 zags      (1000) zags      (1000)     2718 2021-11-22 22:41:44.000000 eb-create-environment-0.1.0/eb_create_environment/vpc.py
+drwxr-xr-x   0 zags      (1000) zags      (1000)        0 2023-07-17 22:24:53.887081 eb-create-environment-0.1.0/eb_create_environment.egg-info/
+-rw-r--r--   0 zags      (1000) zags      (1000)     3836 2023-07-17 22:24:53.000000 eb-create-environment-0.1.0/eb_create_environment.egg-info/PKG-INFO
+-rw-r--r--   0 zags      (1000) zags      (1000)      567 2023-07-17 22:24:53.000000 eb-create-environment-0.1.0/eb_create_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 zags      (1000) zags      (1000)        1 2023-07-17 22:24:53.000000 eb-create-environment-0.1.0/eb_create_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 zags      (1000) zags      (1000)       76 2023-07-17 22:24:53.000000 eb-create-environment-0.1.0/eb_create_environment.egg-info/entry_points.txt
+-rw-r--r--   0 zags      (1000) zags      (1000)       38 2023-07-17 22:24:53.000000 eb-create-environment-0.1.0/eb_create_environment.egg-info/requires.txt
+-rw-r--r--   0 zags      (1000) zags      (1000)       22 2023-07-17 22:24:53.000000 eb-create-environment-0.1.0/eb_create_environment.egg-info/top_level.txt
+-rw-r--r--   0 zags      (1000) zags      (1000)       38 2023-07-17 22:24:53.887081 eb-create-environment-0.1.0/setup.cfg
+-rw-r--r--   0 zags      (1000) zags      (1000)     1183 2023-07-17 21:39:57.000000 eb-create-environment-0.1.0/setup.py
```

### Comparing `eb-create-environment-0.0.5/LICENSE` & `eb-create-environment-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eb-create-environment-0.0.5/PKG-INFO` & `eb-create-environment-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eb-create-environment
-Version: 0.0.5
+Version: 0.1.0
 Summary: Tool to create an Elastic Beanstalk environment and linked database using sensible defaults
 Home-page: https://github.com/zagaran/eb-environment-creation
 Author: Zagaran, Inc.
 Author-email: info@zagaran.com
 License: MIT
 Keywords: aws eb elastic beanstalk rds database create environment
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eb-create-environment-0.0.5/README.md` & `eb-create-environment-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `eb-create-environment-0.0.5/eb_create_environment/database.py` & `eb-create-environment-0.1.0/eb_create_environment/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 import boto3
+import fnmatch
 
 from botocore.exceptions import ParamValidationError
 from choicesenum import ChoicesEnum
 from eb_create_environment.utils import generate_secure_password
 from eb_create_environment.vpc import VPCAccessor
 
 
@@ -162,19 +163,28 @@
         config_engine_name = ENGINE_NAME_LOOKUP[self.engine]
         base_params = {
             param: self.config['RDS'][param] for param in BASE_PARAMS
         }
         engine_params = {
             param: self.config['RDS'][config_engine_name][param] for param in PARAMS_BY_ENGINE[self.engine]
         }
+        engine_version = engine_params.get("EngineVersion")
+        if "*" in engine_version:
+            engine_params["EngineVersion"] = self.get_engine_version(engine_version)
         return {
             **base_params,
             **engine_params,
         }
 
+    def get_engine_version(self, version_string):
+        ret = self.client.describe_db_engine_versions(Engine="postgres")
+        engine_versions = [i["EngineVersion"] for i in ret["DBEngineVersions"]]
+        engine_versions = fnmatch.filter(engine_versions, version_string)
+        return max(engine_versions)
+
     def get_db_url(self, user, host, port):
         postgres_db_name = self.config["RDS"]["Postgres"]["DBName"]
         if self.engine == Engine.postgres:
             return f"postgres://{user}:{self.password}@{host}:{port}/{postgres_db_name}?sslmode=require"
         else:
             return ""
```

### Comparing `eb-create-environment-0.0.5/eb_create_environment/default_config.yml` & `eb-create-environment-0.1.0/eb_create_environment/default_config.yml`

 * *Files 7% similar despite different names*

```diff
@@ -35,11 +35,11 @@
   CopyTagsToSnapshot: True
   MonitoringInterval: 0  # 60 but 0 disables this
   DeletionProtection: False
   MaxAllocatedStorage: 1000
   Postgres:
     DBName: "ebdb"
     Engine: "postgres"
-    EngineVersion: "13.4"
+    EngineVersion: "15.*"
     Port: 5432
-    DBParameterGroupName: "default.postgres13"
+    DBParameterGroupName: "default.postgres15"
     LicenseModel: "postgresql-license"
```

### Comparing `eb-create-environment-0.0.5/eb_create_environment/eb_setup.py` & `eb-create-environment-0.1.0/eb_create_environment/eb_setup.py`

 * *Files identical despite different names*

### Comparing `eb-create-environment-0.0.5/eb_create_environment/script.py` & `eb-create-environment-0.1.0/eb_create_environment/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import argparse
 import boto3
 import os
 import sys
 import yaml
 
+from eb_create_environment._version import __version__
 from eb_create_environment.database import DatabaseInitializer, Engine
 from eb_create_environment.eb_setup import EBInitializer
 from eb_create_environment.vpc import VPCAccessor
 
 
 DEFAULT_CONFIG_FILE_PATH = "default_config.yml"
 EB_GLOBAL_CONFIG_DIRECTORY = ".elasticbeanstalk"
 EB_GLOBAL_CONFIG_FILE_PATH = os.path.join(EB_GLOBAL_CONFIG_DIRECTORY, "config.yml")
 
 
 class SetupWrapper(object):
     def __init__(self):
         parser = argparse.ArgumentParser(description="Set up linked EB and RDS instances")
         parser.add_argument(
+            "--version",
+            action="version",
+            version=f"%(prog)s {__version__}"
+        )
+        parser.add_argument(
             "-c", "--config",
             default=None,
             help="Specify a custom config file",
         )
         parser.add_argument(
             "-a", "--application_name",
             default=None,
```

### Comparing `eb-create-environment-0.0.5/eb_create_environment/utils.py` & `eb-create-environment-0.1.0/eb_create_environment/utils.py`

 * *Files identical despite different names*

### Comparing `eb-create-environment-0.0.5/eb_create_environment/vpc.py` & `eb-create-environment-0.1.0/eb_create_environment/vpc.py`

 * *Files identical despite different names*

### Comparing `eb-create-environment-0.0.5/eb_create_environment.egg-info/PKG-INFO` & `eb-create-environment-0.1.0/eb_create_environment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eb-create-environment
-Version: 0.0.5
+Version: 0.1.0
 Summary: Tool to create an Elastic Beanstalk environment and linked database using sensible defaults
 Home-page: https://github.com/zagaran/eb-environment-creation
 Author: Zagaran, Inc.
 Author-email: info@zagaran.com
 License: MIT
 Keywords: aws eb elastic beanstalk rds database create environment
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eb-create-environment-0.0.5/eb_create_environment.egg-info/SOURCES.txt` & `eb-create-environment-0.1.0/eb_create_environment.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 eb_create_environment/__init__.py
+eb_create_environment/_version.py
 eb_create_environment/database.py
 eb_create_environment/default_config.yml
 eb_create_environment/eb_setup.py
 eb_create_environment/script.py
 eb_create_environment/utils.py
 eb_create_environment/vpc.py
 eb_create_environment.egg-info/PKG-INFO
```

### Comparing `eb-create-environment-0.0.5/setup.py` & `eb-create-environment-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import setuptools
 
+from eb_create_environment._version import __version__
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 setuptools.setup(
     author="Zagaran, Inc.",
     author_email="info@zagaran.com",
@@ -24,9 +25,9 @@
     long_description_content_type="text/markdown",
     name="eb-create-environment",
     packages=setuptools.find_packages(),
     package_data={'': ['default_config.yml']},
     include_package_data=True,
     python_requires='>=3.6',
     url="https://github.com/zagaran/eb-environment-creation",
-    version="0.0.5",
+    version=__version__,
 )
```

