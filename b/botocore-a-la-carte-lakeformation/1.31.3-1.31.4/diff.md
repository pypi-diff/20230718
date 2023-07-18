# Comparing `tmp/botocore-a-la-carte-lakeformation-1.31.3.tar.gz` & `tmp/botocore-a-la-carte-lakeformation-1.31.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-lakeformation-1.31.3.tar", last modified: Fri Jul 14 01:46:21 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-lakeformation-1.31.4.tar", last modified: Tue Jul 18 01:55:20 2023, max compression
```

## Comparing `botocore-a-la-carte-lakeformation-1.31.3.tar` & `botocore-a-la-carte-lakeformation-1.31.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:21.898781 botocore-a-la-carte-lakeformation-1.31.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 01:46:21.000000 botocore-a-la-carte-lakeformation-1.31.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-14 01:46:21.898781 botocore-a-la-carte-lakeformation-1.31.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:21.898781 botocore-a-la-carte-lakeformation-1.31.3/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:21.898781 botocore-a-la-carte-lakeformation-1.31.3/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:21.898781 botocore-a-la-carte-lakeformation-1.31.3/botocore/data/lakeformation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:21.898781 botocore-a-la-carte-lakeformation-1.31.3/botocore/data/lakeformation/2017-03-31/
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-14 01:45:45.000000 botocore-a-la-carte-lakeformation-1.31.3/botocore/data/lakeformation/2017-03-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:45.000000 botocore-a-la-carte-lakeformation-1.31.3/botocore/data/lakeformation/2017-03-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 01:45:45.000000 botocore-a-la-carte-lakeformation-1.31.3/botocore/data/lakeformation/2017-03-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 01:45:45.000000 botocore-a-la-carte-lakeformation-1.31.3/botocore/data/lakeformation/2017-03-31/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)   145923 2023-07-14 01:45:45.000000 botocore-a-la-carte-lakeformation-1.31.3/botocore/data/lakeformation/2017-03-31/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:21.898781 botocore-a-la-carte-lakeformation-1.31.3/botocore_a_la_carte_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-14 01:46:21.000000 botocore-a-la-carte-lakeformation-1.31.3/botocore_a_la_carte_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-14 01:46:21.000000 botocore-a-la-carte-lakeformation-1.31.3/botocore_a_la_carte_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:46:21.000000 botocore-a-la-carte-lakeformation-1.31.3/botocore_a_la_carte_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:46:21.000000 botocore-a-la-carte-lakeformation-1.31.3/botocore_a_la_carte_lakeformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:46:21.902781 botocore-a-la-carte-lakeformation-1.31.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-14 01:46:21.000000 botocore-a-la-carte-lakeformation-1.31.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:20.284265 botocore-a-la-carte-lakeformation-1.31.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 01:55:20.000000 botocore-a-la-carte-lakeformation-1.31.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-18 01:55:20.284265 botocore-a-la-carte-lakeformation-1.31.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:20.284265 botocore-a-la-carte-lakeformation-1.31.4/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:20.284265 botocore-a-la-carte-lakeformation-1.31.4/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:20.284265 botocore-a-la-carte-lakeformation-1.31.4/botocore/data/lakeformation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:20.284265 botocore-a-la-carte-lakeformation-1.31.4/botocore/data/lakeformation/2017-03-31/
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-18 01:54:50.000000 botocore-a-la-carte-lakeformation-1.31.4/botocore/data/lakeformation/2017-03-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-lakeformation-1.31.4/botocore/data/lakeformation/2017-03-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-18 01:54:50.000000 botocore-a-la-carte-lakeformation-1.31.4/botocore/data/lakeformation/2017-03-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-18 01:54:50.000000 botocore-a-la-carte-lakeformation-1.31.4/botocore/data/lakeformation/2017-03-31/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)   146692 2023-07-18 01:54:50.000000 botocore-a-la-carte-lakeformation-1.31.4/botocore/data/lakeformation/2017-03-31/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:20.284265 botocore-a-la-carte-lakeformation-1.31.4/botocore_a_la_carte_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-18 01:55:20.000000 botocore-a-la-carte-lakeformation-1.31.4/botocore_a_la_carte_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-18 01:55:20.000000 botocore-a-la-carte-lakeformation-1.31.4/botocore_a_la_carte_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:55:20.000000 botocore-a-la-carte-lakeformation-1.31.4/botocore_a_la_carte_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 01:55:20.000000 botocore-a-la-carte-lakeformation-1.31.4/botocore_a_la_carte_lakeformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:55:20.284265 botocore-a-la-carte-lakeformation-1.31.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 01:55:20.000000 botocore-a-la-carte-lakeformation-1.31.4/setup.py
```

### Comparing `botocore-a-la-carte-lakeformation-1.31.3/LICENSE.txt` & `botocore-a-la-carte-lakeformation-1.31.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lakeformation-1.31.3/PKG-INFO` & `botocore-a-la-carte-lakeformation-1.31.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-lakeformation
-Version: 1.31.3
+Version: 1.31.4
 Summary: lakeformation data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-lakeformation-1.31.3/botocore/data/lakeformation/2017-03-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-lakeformation-1.31.4/botocore/data/lakeformation/2017-03-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lakeformation-1.31.3/botocore/data/lakeformation/2017-03-31/paginators-1.json` & `botocore-a-la-carte-lakeformation-1.31.4/botocore/data/lakeformation/2017-03-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lakeformation-1.31.3/botocore/data/lakeformation/2017-03-31/service-2.json` & `botocore-a-la-carte-lakeformation-1.31.4/botocore/data/lakeformation/2017-03-31/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998441448455473%*

 * *Differences: {"'operations'": "{'ListPermissions': {'documentation': '<p>Returns a list of the principal "*

 * *                 'permissions on the resource, filtered by the permissions of the caller. For '*

 * *                 'example, if you are granted an ALTER permission, you are able to see only the '*

 * *                 'principal permissions for ALTER.</p> <p>This operation returns only those '*

 * *                 'permissions that have been explicitly granted.</p> <p>For information about '*

 * *                 'permissions, see […]*

```diff
@@ -958,15 +958,15 @@
             },
             "name": "ListLFTags",
             "output": {
                 "shape": "ListLFTagsResponse"
             }
         },
         "ListPermissions": {
-            "documentation": "<p>Returns a list of the principal permissions on the resource, filtered by the permissions of the caller. For example, if you are granted an ALTER permission, you are able to see only the principal permissions for ALTER.</p> <p>This operation returns only those permissions that have been explicitly granted.</p> <p>For information about permissions, see <a href=\"https://docs-aws.amazon.com/lake-formation/latest/dg/security-data-access.html\">Security and Access Control to Metadata and Data</a>.</p>",
+            "documentation": "<p>Returns a list of the principal permissions on the resource, filtered by the permissions of the caller. For example, if you are granted an ALTER permission, you are able to see only the principal permissions for ALTER.</p> <p>This operation returns only those permissions that have been explicitly granted.</p> <p>For information about permissions, see <a href=\"https://docs.aws.amazon.com/lake-formation/latest/dg/security-data-access.html\">Security and Access Control to Metadata and Data</a>.</p>",
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "OperationTimeoutException"
                 },
@@ -1902,15 +1902,15 @@
             "min": 900,
             "type": "integer"
         },
         "DataCellsFilter": {
             "documentation": "<p>A structure that describes certain columns on certain rows.</p>",
             "members": {
                 "ColumnNames": {
-                    "documentation": "<p>A list of column names.</p>",
+                    "documentation": "<p>A list of column names and/or nested column attributes. When specifying nested attributes, use a qualified dot (.) delimited format such as \"address\".\"zip\". Nested attributes within this list may not exceed a depth of 5.</p>",
                     "shape": "ColumnNames"
                 },
                 "ColumnWildcard": {
                     "documentation": "<p>A wildcard with exclusions.</p> <p>You must specify either a <code>ColumnNames</code> list or the <code>ColumnWildCard</code>. </p>",
                     "shape": "ColumnWildcard"
                 },
                 "DatabaseName": {
@@ -2010,15 +2010,19 @@
             ],
             "type": "string"
         },
         "DataLakeSettings": {
             "documentation": "<p>A structure representing a list of Lake Formation principals designated as data lake administrators and lists of principal permission entries for default create database and default create table permissions.</p>",
             "members": {
                 "AllowExternalDataFiltering": {
-                    "documentation": "<p>Whether to allow Amazon EMR clusters to access data managed by Lake Formation. </p> <p>If true, you allow Amazon EMR clusters to access data in Amazon S3 locations that are registered with Lake Formation.</p> <p>If false or null, no Amazon EMR clusters will be able to access data in Amazon S3 locations that are registered with Lake Formation.</p> <p>For more information, see <a href=\"https://docs-aws.amazon.com/lake-formation/latest/dg/getting-started-setup.html#emr-switch\">(Optional) Allow Data Filtering on Amazon EMR</a>.</p>",
+                    "documentation": "<p>Whether to allow Amazon EMR clusters to access data managed by Lake Formation. </p> <p>If true, you allow Amazon EMR clusters to access data in Amazon S3 locations that are registered with Lake Formation.</p> <p>If false or null, no Amazon EMR clusters will be able to access data in Amazon S3 locations that are registered with Lake Formation.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/lake-formation/latest/dg/initial-LF-setup.html#external-data-filter\">(Optional) Allow external data filtering</a>.</p>",
+                    "shape": "NullableBoolean"
+                },
+                "AllowFullTableExternalDataAccess": {
+                    "documentation": "<p>Whether to allow a third-party query engine to get data access credentials without session tags when a caller has full data access permissions.</p>",
                     "shape": "NullableBoolean"
                 },
                 "AuthorizedSessionTagValueList": {
                     "documentation": "<p>Lake Formation relies on a privileged process secured by Amazon EMR or the third party integrator to tag the user's role while assuming it. Lake Formation will publish the acceptable key-value pair, for example key = \"LakeFormationTrustedCaller\" and value = \"TRUE\" and the third party integrator must properly tag the temporary security credentials that will be used to call Lake Formation's administrative APIs.</p>",
                     "shape": "AuthorizedSessionTagValueList"
                 },
                 "CreateDatabaseDefaultPermissions": {
@@ -2037,14 +2041,18 @@
                     "documentation": "<p>A list of the account IDs of Amazon Web Services accounts with Amazon EMR clusters that are to perform data filtering.&gt;</p>",
                     "shape": "DataLakePrincipalList"
                 },
                 "Parameters": {
                     "documentation": "<p>A key-value map that provides an additional configuration on your data lake. CrossAccountVersion is the key you can configure in the Parameters field. Accepted values for the CrossAccountVersion key are 1, 2, and 3.</p>",
                     "shape": "ParametersMap"
                 },
+                "ReadOnlyAdmins": {
+                    "documentation": "<p>A list of Lake Formation principals with only view access to the resources, without the ability to make changes. Supported principals are IAM users or IAM roles.</p>",
+                    "shape": "DataLakePrincipalList"
+                },
                 "TrustedResourceOwners": {
                     "documentation": "<p>A list of the resource-owning account IDs that the caller's account can use to share their user access details (user ARNs). The user ARNs can be logged in the resource owner's CloudTrail log.</p> <p>You may want to specify this property when you are in a high-trust boundary, such as the same team or company. </p>",
                     "shape": "TrustedResourceOwners"
                 }
             },
             "type": "structure"
         },
@@ -2698,16 +2706,15 @@
                 "TableArn": {
                     "documentation": "<p>The ARN of the partitions' table.</p>",
                     "shape": "ResourceArnString"
                 }
             },
             "required": [
                 "TableArn",
-                "Partition",
-                "SupportedPermissionTypes"
+                "Partition"
             ],
             "type": "structure"
         },
         "GetTemporaryGluePartitionCredentialsResponse": {
             "members": {
                 "AccessKeyId": {
                     "documentation": "<p>The access key ID for the temporary credentials.</p>",
@@ -2748,16 +2755,15 @@
                 },
                 "TableArn": {
                     "documentation": "<p>The ARN identifying a table in the Data Catalog for the temporary credentials request.</p>",
                     "shape": "ResourceArnString"
                 }
             },
             "required": [
-                "TableArn",
-                "SupportedPermissionTypes"
+                "TableArn"
             ],
             "type": "structure"
         },
         "GetTemporaryGlueTableCredentialsResponse": {
             "members": {
                 "AccessKeyId": {
                     "documentation": "<p>The access key ID for the temporary credentials.</p>",
@@ -3428,29 +3434,32 @@
                 "DROP",
                 "DELETE",
                 "INSERT",
                 "DESCRIBE",
                 "CREATE_DATABASE",
                 "CREATE_TABLE",
                 "DATA_LOCATION_ACCESS",
-                "CREATE_TAG",
-                "ASSOCIATE"
+                "CREATE_LF_TAG",
+                "ASSOCIATE",
+                "GRANT_WITH_LF_TAG_EXPRESSION"
             ],
             "type": "string"
         },
         "PermissionList": {
             "member": {
                 "shape": "Permission"
             },
             "type": "list"
         },
         "PermissionType": {
             "enum": [
                 "COLUMN_PERMISSION",
-                "CELL_FILTER_PERMISSION"
+                "CELL_FILTER_PERMISSION",
+                "NESTED_PERMISSION",
+                "NESTED_CELL_PERMISSION"
             ],
             "type": "string"
         },
         "PermissionTypeList": {
             "max": 255,
             "member": {
                 "shape": "PermissionType"
```

### Comparing `botocore-a-la-carte-lakeformation-1.31.3/botocore_a_la_carte_lakeformation.egg-info/PKG-INFO` & `botocore-a-la-carte-lakeformation-1.31.4/botocore_a_la_carte_lakeformation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-lakeformation
-Version: 1.31.3
+Version: 1.31.4
 Summary: lakeformation data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-lakeformation-1.31.3/botocore_a_la_carte_lakeformation.egg-info/SOURCES.txt` & `botocore-a-la-carte-lakeformation-1.31.4/botocore_a_la_carte_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lakeformation-1.31.3/setup.py` & `botocore-a-la-carte-lakeformation-1.31.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-lakeformation',
-    version="1.31.3",
+    version="1.31.4",
     description='lakeformation data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/lakeformation/*/*.json'],
```

