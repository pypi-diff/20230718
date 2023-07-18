# Comparing `tmp/ory-oathkeeper-client-0.40.5.tar.gz` & `tmp/ory-oathkeeper-client-0.40.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ory-oathkeeper-client-0.40.5.tar", last modified: Mon Jul 17 14:23:07 2023, max compression
+gzip compressed data, was "dist/ory-oathkeeper-client-0.40.6.tar", last modified: Tue Jul 18 10:31:59 2023, max compression
```

## Comparing `ory-oathkeeper-client-0.40.5.tar` & `ory-oathkeeper-client-0.40.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4424 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/
--rw-r--r--   0 root         (0) root         (0)      919 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/api/
--rw-r--r--   0 root         (0) root         (0)      221 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20793 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/api/api_api.py
--rw-r--r--   0 root         (0) root         (0)    11127 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/api/health_api.py
--rw-r--r--   0 root         (0) root         (0)     5887 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/api/version_api.py
--rw-r--r--   0 root         (0) root         (0)    39198 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/apis/
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16329 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5193 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/
--rw-r--r--   0 root         (0) root         (0)      355 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12695 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/generic_error.py
--rw-r--r--   0 root         (0) root         (0)    11733 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/health_not_ready_status.py
--rw-r--r--   0 root         (0) root         (0)    11607 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/health_status.py
--rw-r--r--   0 root         (0) root         (0)    17999 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/json_web_key.py
--rw-r--r--   0 root         (0) root         (0)    12300 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)    15131 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/rule.py
--rw-r--r--   0 root         (0) root         (0)    12500 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/rule_handler.py
--rw-r--r--   0 root         (0) root         (0)    13888 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/rule_match.py
--rw-r--r--   0 root         (0) root         (0)    12686 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/upstream.py
--rw-r--r--   0 root         (0) root         (0)    11603 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/version.py
--rw-r--r--   0 root         (0) root         (0)    82710 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/models/
--rw-r--r--   0 root         (0) root         (0)     1027 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14404 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1514 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/ory_oathkeeper_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1251 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 14:23:07.000000 ory-oathkeeper-client-0.40.5/test/
--rw-r--r--   0 root         (0) root         (0)     1254 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_api_api.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_generic_error.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_health_api.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_health_not_ready_status.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_health_status.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_json_web_key.py
--rw-r--r--   0 root         (0) root         (0)      985 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)     1109 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_rule.py
--rw-r--r--   0 root         (0) root         (0)      868 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_rule_handler.py
--rw-r--r--   0 root         (0) root         (0)      854 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_rule_match.py
--rw-r--r--   0 root         (0) root         (0)      846 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_upstream.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_version.py
--rw-r--r--   0 root         (0) root         (0)      834 2023-07-17 14:18:29.000000 ory-oathkeeper-client-0.40.5/test/test_version_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/
+-rw-r--r--   0 root         (0) root         (0)      919 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/api/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20793 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/api/api_api.py
+-rw-r--r--   0 root         (0) root         (0)    11127 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/api/health_api.py
+-rw-r--r--   0 root         (0) root         (0)     5887 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/api/version_api.py
+-rw-r--r--   0 root         (0) root         (0)    39198 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16329 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12695 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/generic_error.py
+-rw-r--r--   0 root         (0) root         (0)    11733 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/health_not_ready_status.py
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/health_status.py
+-rw-r--r--   0 root         (0) root         (0)    17999 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)    12300 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)    15131 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/rule.py
+-rw-r--r--   0 root         (0) root         (0)    12500 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/rule_handler.py
+-rw-r--r--   0 root         (0) root         (0)    13888 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/rule_match.py
+-rw-r--r--   0 root         (0) root         (0)    12686 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/upstream.py
+-rw-r--r--   0 root         (0) root         (0)    11603 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/version.py
+-rw-r--r--   0 root         (0) root         (0)    82710 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/models/
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14404 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/ory_oathkeeper_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:31:59.000000 ory-oathkeeper-client-0.40.6/test/
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_api_api.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_generic_error.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_health_api.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_health_not_ready_status.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_health_status.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)      985 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)      868 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_rule_handler.py
+-rw-r--r--   0 root         (0) root         (0)      854 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_rule_match.py
+-rw-r--r--   0 root         (0) root         (0)      846 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_upstream.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_version.py
+-rw-r--r--   0 root         (0) root         (0)      834 2023-07-18 10:27:29.000000 ory-oathkeeper-client-0.40.6/test/test_version_api.py
```

### Comparing `ory-oathkeeper-client-0.40.5/LICENSE` & `ory-oathkeeper-client-0.40.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ory-oathkeeper-client-0.40.5/README.md` & `ory-oathkeeper-client-0.40.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ory-oathkeeper-client
 ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: v0.40.5
-- Package version: v0.40.5
+- API version: v0.40.6
+- Package version: v0.40.6
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.ory.am](https://www.ory.am)
 
 ## Requirements.
 
 Python >=3.6
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/__init__.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "v0.40.5"
+__version__ = "v0.40.6"
 
 # import ApiClient
 from ory_oathkeeper_client.api_client import ApiClient
 
 # import Configuration
 from ory_oathkeeper_client.configuration import Configuration
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/api/api_api.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/api/api_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/api/health_api.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/api/health_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/api/version_api.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/api/version_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/api_client.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/v0.40.5/python'
+        self.user_agent = 'OpenAPI-Generator/v0.40.6/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/apis/__init__.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/configuration.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -376,16 +376,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: v0.40.5\n"\
-               "SDK Package Version: v0.40.5".\
+               "Version of the API: v0.40.6\n"\
+               "SDK Package Version: v0.40.6".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/exceptions.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/generic_error.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/generic_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/health_not_ready_status.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/health_not_ready_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/health_status.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/health_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/json_web_key.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/json_web_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/json_web_key_set.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/json_web_key_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/rule.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/rule_handler.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/rule_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/rule_match.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/rule_match.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/upstream.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/upstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model/version.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/model_utils.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/models/__init__.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client/rest.py` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `ory-oathkeeper-client-0.40.5/ory_oathkeeper_client.egg-info/SOURCES.txt` & `ory-oathkeeper-client-0.40.6/ory_oathkeeper_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ory-oathkeeper-client-0.40.5/setup.py` & `ory-oathkeeper-client-0.40.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ory-oathkeeper-client"
-VERSION = "v0.40.5"
+VERSION = "v0.40.6"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_api_api.py` & `ory-oathkeeper-client-0.40.6/test/test_api_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_generic_error.py` & `ory-oathkeeper-client-0.40.6/test/test_generic_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_health_api.py` & `ory-oathkeeper-client-0.40.6/test/test_health_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_health_not_ready_status.py` & `ory-oathkeeper-client-0.40.6/test/test_health_not_ready_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_health_status.py` & `ory-oathkeeper-client-0.40.6/test/test_health_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_json_web_key.py` & `ory-oathkeeper-client-0.40.6/test/test_json_web_key.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_json_web_key_set.py` & `ory-oathkeeper-client-0.40.6/test/test_json_web_key_set.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_rule.py` & `ory-oathkeeper-client-0.40.6/test/test_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_rule_handler.py` & `ory-oathkeeper-client-0.40.6/test/test_rule_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_rule_match.py` & `ory-oathkeeper-client-0.40.6/test/test_rule_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_upstream.py` & `ory-oathkeeper-client-0.40.6/test/test_upstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_version.py` & `ory-oathkeeper-client-0.40.6/test/test_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-oathkeeper-client-0.40.5/test/test_version_api.py` & `ory-oathkeeper-client-0.40.6/test/test_version_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ORY Oathkeeper
 
     ORY Oathkeeper is a reverse proxy that checks the HTTP Authorization for validity against a set of rules. This service uses Hydra to validate access tokens and policies.  # noqa: E501
 
-    The version of the OpenAPI document: v0.40.5
+    The version of the OpenAPI document: v0.40.6
     Contact: hi@ory.am
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

