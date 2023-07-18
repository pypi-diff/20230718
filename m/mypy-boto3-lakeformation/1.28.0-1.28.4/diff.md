# Comparing `tmp/mypy-boto3-lakeformation-1.28.0.tar.gz` & `tmp/mypy-boto3-lakeformation-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lakeformation-1.28.0.tar", last modified: Thu Jul  6 20:59:57 2023, max compression
+gzip compressed data, was "mypy-boto3-lakeformation-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-lakeformation-1.28.0.tar` & `mypy-boto3-lakeformation-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.550350 mypy-boto3-lakeformation-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-07-06 20:59:57.538350 mypy-boto3-lakeformation-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.538350 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37090 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37031 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-06 20:45:04.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48249 2023-07-06 20:45:07.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48164 2023-07-06 20:45:06.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.538350 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-07-06 20:59:57.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 20:59:57.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:57.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:57.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:57.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 20:59:57.000000 mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:57.550350 mypy-boto3-lakeformation-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-06 20:45:03.000000 mypy-boto3-lakeformation-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19383 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37043 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53022 2023-07-18 01:01:31.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52937 2023-07-18 01:01:31.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19383 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-18 01:01:29.000000 mypy-boto3-lakeformation-1.28.4/setup.py
```

### Comparing `mypy-boto3-lakeformation-1.28.0/LICENSE` & `mypy-boto3-lakeformation-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.0/PKG-INFO` & `mypy-boto3-lakeformation-1.28.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.28.0
-Summary: Type annotations for boto3.LakeFormation 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.4
+Summary: Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,28 +352,34 @@
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
+    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
+    LFTagPairOutputTypeDef,
+    ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
+    RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
@@ -384,105 +390,116 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
-    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
-    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
     GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
+    LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
+    LFTagOutputTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     TableObjectTypeDef,
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartQueryPlanningResponseTypeDef,
+    TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
-    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    GetLFTagResponseTypeDef,
+    GetQueryStateResponseTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    StartQueryPlanningResponseTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
-    ColumnLFTagTypeDef,
-    ListLFTagsResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
-    LFTagErrorTypeDef,
+    PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    ColumnLFTagTypeDef,
+    LFTagErrorTypeDef,
+    ListLFTagsResponseTypeDef,
+    TableWithColumnsResourceOutputTypeDef,
     TableWithColumnsResourceTypeDef,
+    DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
     DeleteObjectsOnCancelRequestRequestTypeDef,
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
+    LFTagPolicyResourceOutputTypeDef,
     LFTagPolicyResourceTypeDef,
     SearchDatabasesByLFTagsRequestRequestTypeDef,
     SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
     StartQueryPlanningRequestRequestTypeDef,
+    DataLakeSettingsOutputTypeDef,
+    DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    DataLakeSettingsTypeDef,
-    CreateDataCellsFilterRequestRequestTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
+    CreateDataCellsFilterRequestRequestTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     GetTableObjectsResponseTypeDef,
-    SearchTablesByLFTagsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
+    SearchTablesByLFTagsResponseTypeDef,
+    BatchPermissionsRequestEntryOutputTypeDef,
+    PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
-    PrincipalResourcePermissionsTypeDef,
     RemoveLFTagsFromResourceRequestRequestTypeDef,
     RevokePermissionsRequestRequestTypeDef,
-    BatchGrantPermissionsRequestRequestTypeDef,
     BatchPermissionsFailureEntryTypeDef,
-    BatchRevokePermissionsRequestRequestTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     ListPermissionsResponseTypeDef,
+    BatchGrantPermissionsRequestRequestTypeDef,
+    BatchRevokePermissionsRequestRequestTypeDef,
     BatchGrantPermissionsResponseTypeDef,
     BatchRevokePermissionsResponseTypeDef,
 )
 
 
 def get_structure() -> LFTagPairTypeDef:
     return {...}
```

### Comparing `mypy-boto3-lakeformation-1.28.0/README.md` & `mypy-boto3-lakeformation-1.28.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,28 +320,34 @@
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
+    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
+    LFTagPairOutputTypeDef,
+    ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
+    RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
@@ -352,105 +358,116 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
-    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
-    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
     GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
+    LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
+    LFTagOutputTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     TableObjectTypeDef,
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartQueryPlanningResponseTypeDef,
+    TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
-    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    GetLFTagResponseTypeDef,
+    GetQueryStateResponseTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    StartQueryPlanningResponseTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
-    ColumnLFTagTypeDef,
-    ListLFTagsResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
-    LFTagErrorTypeDef,
+    PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    ColumnLFTagTypeDef,
+    LFTagErrorTypeDef,
+    ListLFTagsResponseTypeDef,
+    TableWithColumnsResourceOutputTypeDef,
     TableWithColumnsResourceTypeDef,
+    DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
     DeleteObjectsOnCancelRequestRequestTypeDef,
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
+    LFTagPolicyResourceOutputTypeDef,
     LFTagPolicyResourceTypeDef,
     SearchDatabasesByLFTagsRequestRequestTypeDef,
     SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
     StartQueryPlanningRequestRequestTypeDef,
+    DataLakeSettingsOutputTypeDef,
+    DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    DataLakeSettingsTypeDef,
-    CreateDataCellsFilterRequestRequestTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
+    CreateDataCellsFilterRequestRequestTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     GetTableObjectsResponseTypeDef,
-    SearchTablesByLFTagsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
+    SearchTablesByLFTagsResponseTypeDef,
+    BatchPermissionsRequestEntryOutputTypeDef,
+    PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
-    PrincipalResourcePermissionsTypeDef,
     RemoveLFTagsFromResourceRequestRequestTypeDef,
     RevokePermissionsRequestRequestTypeDef,
-    BatchGrantPermissionsRequestRequestTypeDef,
     BatchPermissionsFailureEntryTypeDef,
-    BatchRevokePermissionsRequestRequestTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     ListPermissionsResponseTypeDef,
+    BatchGrantPermissionsRequestRequestTypeDef,
+    BatchRevokePermissionsRequestRequestTypeDef,
     BatchGrantPermissionsResponseTypeDef,
     BatchRevokePermissionsResponseTypeDef,
 )
 
 
 def get_structure() -> LFTagPairTypeDef:
     return {...}
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/__init__.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/__init__.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/__main__.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LakeFormation 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.LakeFormation 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/client.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,35 +404,35 @@
         """
 
     def get_temporary_glue_partition_credentials(
         self,
         *,
         TableArn: str,
         Partition: PartitionValueListTypeDef,
-        SupportedPermissionTypes: Sequence[PermissionTypeType],
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
     ) -> GetTemporaryGluePartitionCredentialsResponseTypeDef:
         """
         This API is identical to `GetTemporaryTableCredentials` except that this is used
         when the target Data Catalog resource is of type Partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_partition_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_temporary_glue_partition_credentials)
         """
 
     def get_temporary_glue_table_credentials(
         self,
         *,
         TableArn: str,
-        SupportedPermissionTypes: Sequence[PermissionTypeType],
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
     ) -> GetTemporaryGlueTableCredentialsResponseTypeDef:
         """
         Allows a caller in a secure environment to assume a role with permission to
         access Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_table_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_temporary_glue_table_credentials)
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/client.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -373,34 +373,34 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_table_objects)
         """
     def get_temporary_glue_partition_credentials(
         self,
         *,
         TableArn: str,
         Partition: PartitionValueListTypeDef,
-        SupportedPermissionTypes: Sequence[PermissionTypeType],
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
     ) -> GetTemporaryGluePartitionCredentialsResponseTypeDef:
         """
         This API is identical to `GetTemporaryTableCredentials` except that this is used
         when the target Data Catalog resource is of type Partition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_partition_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_temporary_glue_partition_credentials)
         """
     def get_temporary_glue_table_credentials(
         self,
         *,
         TableArn: str,
-        SupportedPermissionTypes: Sequence[PermissionTypeType],
         Permissions: Sequence[PermissionType] = ...,
         DurationSeconds: int = ...,
-        AuditContext: AuditContextTypeDef = ...
+        AuditContext: AuditContextTypeDef = ...,
+        SupportedPermissionTypes: Sequence[PermissionTypeType] = ...
     ) -> GetTemporaryGlueTableCredentialsResponseTypeDef:
         """
         Allows a caller in a secure environment to assume a role with permission to
         access Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_temporary_glue_table_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_temporary_glue_table_credentials)
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/literals.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,24 +64,27 @@
 ListLFTagsPaginatorName = Literal["list_lf_tags"]
 OptimizerTypeType = Literal["ALL", "COMPACTION", "GARBAGE_COLLECTION"]
 PermissionType = Literal[
     "ALL",
     "ALTER",
     "ASSOCIATE",
     "CREATE_DATABASE",
+    "CREATE_LF_TAG",
     "CREATE_TABLE",
-    "CREATE_TAG",
     "DATA_LOCATION_ACCESS",
     "DELETE",
     "DESCRIBE",
     "DROP",
+    "GRANT_WITH_LF_TAG_EXPRESSION",
     "INSERT",
     "SELECT",
 ]
-PermissionTypeType = Literal["CELL_FILTER_PERMISSION", "COLUMN_PERMISSION"]
+PermissionTypeType = Literal[
+    "CELL_FILTER_PERMISSION", "COLUMN_PERMISSION", "NESTED_CELL_PERMISSION", "NESTED_PERMISSION"
+]
 QueryStateStringType = Literal["ERROR", "EXPIRED", "FINISHED", "PENDING", "WORKUNITS_AVAILABLE"]
 ResourceShareTypeType = Literal["ALL", "FOREIGN"]
 ResourceTypeType = Literal["DATABASE", "TABLE"]
 SearchDatabasesByLFTagsPaginatorName = Literal["search_databases_by_lf_tags"]
 SearchTablesByLFTagsPaginatorName = Literal["search_tables_by_lf_tags"]
 TransactionStatusFilterType = Literal["ABORTED", "ACTIVE", "ALL", "COMMITTED", "COMPLETED"]
 TransactionStatusType = Literal["ABORTED", "ACTIVE", "COMMITTED", "COMMIT_IN_PROGRESS"]
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/literals.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -62,24 +62,27 @@
 ListLFTagsPaginatorName = Literal["list_lf_tags"]
 OptimizerTypeType = Literal["ALL", "COMPACTION", "GARBAGE_COLLECTION"]
 PermissionType = Literal[
     "ALL",
     "ALTER",
     "ASSOCIATE",
     "CREATE_DATABASE",
+    "CREATE_LF_TAG",
     "CREATE_TABLE",
-    "CREATE_TAG",
     "DATA_LOCATION_ACCESS",
     "DELETE",
     "DESCRIBE",
     "DROP",
+    "GRANT_WITH_LF_TAG_EXPRESSION",
     "INSERT",
     "SELECT",
 ]
-PermissionTypeType = Literal["CELL_FILTER_PERMISSION", "COLUMN_PERMISSION"]
+PermissionTypeType = Literal[
+    "CELL_FILTER_PERMISSION", "COLUMN_PERMISSION", "NESTED_CELL_PERMISSION", "NESTED_PERMISSION"
+]
 QueryStateStringType = Literal["ERROR", "EXPIRED", "FINISHED", "PENDING", "WORKUNITS_AVAILABLE"]
 ResourceShareTypeType = Literal["ALL", "FOREIGN"]
 ResourceTypeType = Literal["DATABASE", "TABLE"]
 SearchDatabasesByLFTagsPaginatorName = Literal["search_databases_by_lf_tags"]
 SearchTablesByLFTagsPaginatorName = Literal["search_tables_by_lf_tags"]
 TransactionStatusFilterType = Literal["ABORTED", "ACTIVE", "ALL", "COMMITTED", "COMPLETED"]
 TransactionStatusType = Literal["ABORTED", "ACTIVE", "COMMITTED", "COMMIT_IN_PROGRESS"]
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/paginator.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,103 +47,96 @@
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
     "SearchTablesByLFTagsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetWorkUnitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
     """
 
     def paginate(
-        self, *, QueryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetWorkUnitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
         """
 
-
 class ListDataCellsFilterPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
-
 class ListLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
         """
 
-
 class SearchDatabasesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
-
 class SearchTablesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/paginator.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,96 +47,103 @@
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
     "SearchTablesByLFTagsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetWorkUnitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
     """
 
     def paginate(
-        self, *, QueryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetWorkUnitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
         """
 
+
 class ListDataCellsFilterPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
+
 class ListLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
         """
 
+
 class SearchDatabasesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
+
 class SearchTablesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
         Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/type_defs.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,28 +36,34 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "LFTagPairTypeDef",
+    "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
+    "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
+    "LFTagPairOutputTypeDef",
+    "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
-    "CommitTransactionResponseTypeDef",
     "CreateLFTagRequestRequestTypeDef",
+    "RowFilterOutputTypeDef",
+    "DataCellsFilterResourceOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
+    "DataLocationResourceOutputTypeDef",
     "DataLocationResourceTypeDef",
+    "DatabaseResourceOutputTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
     "VirtualObjectTypeDef",
     "DeregisterResourceRequestRequestTypeDef",
     "DescribeResourceRequestRequestTypeDef",
@@ -68,105 +74,116 @@
     "ExecutionStatisticsTypeDef",
     "ExtendTransactionRequestRequestTypeDef",
     "FilterConditionTypeDef",
     "GetDataCellsFilterRequestRequestTypeDef",
     "GetDataLakeSettingsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathRequestRequestTypeDef",
     "GetLFTagRequestRequestTypeDef",
-    "GetLFTagResponseTypeDef",
     "GetQueryStateRequestRequestTypeDef",
-    "GetQueryStateResponseTypeDef",
     "GetQueryStatisticsRequestRequestTypeDef",
     "PlanningStatisticsTypeDef",
     "GetTableObjectsRequestRequestTypeDef",
     "PartitionValueListTypeDef",
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
-    "GetWorkUnitResultsResponseTypeDef",
-    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
+    "LFTagKeyResourceOutputTypeDef",
     "LFTagKeyResourceTypeDef",
+    "LFTagOutputTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "TableObjectTypeDef",
     "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartQueryPlanningResponseTypeDef",
+    "TableResourceOutputTypeDef",
     "StartTransactionRequestRequestTypeDef",
-    "StartTransactionResponseTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
+    "CommitTransactionResponseTypeDef",
+    "GetLFTagResponseTypeDef",
+    "GetQueryStateResponseTypeDef",
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    "GetWorkUnitResultsResponseTypeDef",
+    "StartQueryPlanningResponseTypeDef",
+    "StartTransactionResponseTypeDef",
     "UpdateTableStorageOptimizerResponseTypeDef",
-    "ColumnLFTagTypeDef",
-    "ListLFTagsResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
-    "LFTagErrorTypeDef",
+    "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
+    "ColumnLFTagTypeDef",
+    "LFTagErrorTypeDef",
+    "ListLFTagsResponseTypeDef",
+    "TableWithColumnsResourceOutputTypeDef",
     "TableWithColumnsResourceTypeDef",
+    "DataCellsFilterOutputTypeDef",
     "DataCellsFilterTypeDef",
     "TaggedDatabaseTypeDef",
     "WriteOperationTypeDef",
     "DeleteObjectsOnCancelRequestRequestTypeDef",
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
     "ListTransactionsResponseTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "GetQueryStatisticsResponseTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
+    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
+    "LFTagPolicyResourceOutputTypeDef",
     "LFTagPolicyResourceTypeDef",
     "SearchDatabasesByLFTagsRequestRequestTypeDef",
     "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     "SearchTablesByLFTagsRequestRequestTypeDef",
     "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     "ListDataCellsFilterRequestRequestTypeDef",
     "ListTableStorageOptimizersResponseTypeDef",
     "PartitionObjectsTypeDef",
     "StartQueryPlanningRequestRequestTypeDef",
+    "DataLakeSettingsOutputTypeDef",
+    "DataLakeSettingsTypeDef",
     "GetResourceLFTagsResponseTypeDef",
     "TaggedTableTypeDef",
     "AddLFTagsToResourceResponseTypeDef",
     "RemoveLFTagsFromResourceResponseTypeDef",
-    "DataLakeSettingsTypeDef",
-    "CreateDataCellsFilterRequestRequestTypeDef",
     "GetDataCellsFilterResponseTypeDef",
     "ListDataCellsFilterResponseTypeDef",
+    "CreateDataCellsFilterRequestRequestTypeDef",
     "UpdateDataCellsFilterRequestRequestTypeDef",
     "SearchDatabasesByLFTagsResponseTypeDef",
     "UpdateTableObjectsRequestRequestTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "GetTableObjectsResponseTypeDef",
-    "SearchTablesByLFTagsResponseTypeDef",
     "GetDataLakeSettingsResponseTypeDef",
     "PutDataLakeSettingsRequestRequestTypeDef",
+    "SearchTablesByLFTagsResponseTypeDef",
+    "BatchPermissionsRequestEntryOutputTypeDef",
+    "PrincipalResourcePermissionsTypeDef",
     "AddLFTagsToResourceRequestRequestTypeDef",
     "BatchPermissionsRequestEntryTypeDef",
     "GetResourceLFTagsRequestRequestTypeDef",
     "GrantPermissionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
-    "PrincipalResourcePermissionsTypeDef",
     "RemoveLFTagsFromResourceRequestRequestTypeDef",
     "RevokePermissionsRequestRequestTypeDef",
-    "BatchGrantPermissionsRequestRequestTypeDef",
     "BatchPermissionsFailureEntryTypeDef",
-    "BatchRevokePermissionsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathResponseTypeDef",
     "ListPermissionsResponseTypeDef",
+    "BatchGrantPermissionsRequestRequestTypeDef",
+    "BatchRevokePermissionsRequestRequestTypeDef",
     "BatchGrantPermissionsResponseTypeDef",
     "BatchRevokePermissionsResponseTypeDef",
 )
 
 _RequiredLFTagPairTypeDef = TypedDict(
     "_RequiredLFTagPairTypeDef",
     {
@@ -183,14 +200,25 @@
 )
 
 
 class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
     pass
 
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredAddObjectInputTypeDef = TypedDict(
     "_RequiredAddObjectInputTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
@@ -228,40 +256,35 @@
 class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
 
-AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
     },
     total=False,
 )
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+DataLakePrincipalOutputTypeDef = TypedDict(
+    "DataLakePrincipalOutputTypeDef",
+    {
+        "DataLakePrincipalIdentifier": str,
+    },
 )
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
@@ -271,14 +294,30 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
+LFTagPairOutputTypeDef = TypedDict(
+    "LFTagPairOutputTypeDef",
+    {
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
+ColumnWildcardOutputTypeDef = TypedDict(
+    "ColumnWildcardOutputTypeDef",
+    {
+        "ExcludedColumnNames": List[str],
+    },
+)
+
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
     total=False,
 )
@@ -286,22 +325,14 @@
 CommitTransactionRequestRequestTypeDef = TypedDict(
     "CommitTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-CommitTransactionResponseTypeDef = TypedDict(
-    "CommitTransactionResponseTypeDef",
-    {
-        "TransactionStatus": TransactionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -316,14 +347,32 @@
 
 class CreateLFTagRequestRequestTypeDef(
     _RequiredCreateLFTagRequestRequestTypeDef, _OptionalCreateLFTagRequestRequestTypeDef
 ):
     pass
 
 
+RowFilterOutputTypeDef = TypedDict(
+    "RowFilterOutputTypeDef",
+    {
+        "FilterExpression": str,
+        "AllRowsWildcard": Dict[str, Any],
+    },
+)
+
+DataCellsFilterResourceOutputTypeDef = TypedDict(
+    "DataCellsFilterResourceOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+    },
+)
+
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -336,14 +385,22 @@
     {
         "FilterExpression": str,
         "AllRowsWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
+DataLocationResourceOutputTypeDef = TypedDict(
+    "DataLocationResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredDataLocationResourceTypeDef = TypedDict(
     "_RequiredDataLocationResourceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalDataLocationResourceTypeDef = TypedDict(
@@ -357,14 +414,22 @@
 
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
 
+DatabaseResourceOutputTypeDef = TypedDict(
+    "DatabaseResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "Name": str,
+    },
+)
+
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
@@ -471,15 +536,14 @@
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
         "WithFederation": bool,
     },
-    total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -489,33 +553,30 @@
     "TransactionDescriptionTypeDef",
     {
         "TransactionId": str,
         "TransactionStatus": TransactionStatusType,
         "TransactionStartTime": datetime,
         "TransactionEndTime": datetime,
     },
-    total=False,
 )
 
 DetailsMapTypeDef = TypedDict(
     "DetailsMapTypeDef",
     {
         "ResourceShare": List[str],
     },
-    total=False,
 )
 
 ExecutionStatisticsTypeDef = TypedDict(
     "ExecutionStatisticsTypeDef",
     {
         "AverageExecutionTimeMillis": int,
         "DataScannedBytes": int,
         "WorkUnitsExecutedCount": int,
     },
-    total=False,
 )
 
 ExtendTransactionRequestRequestTypeDef = TypedDict(
     "ExtendTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -591,40 +652,21 @@
 
 class GetLFTagRequestRequestTypeDef(
     _RequiredGetLFTagRequestRequestTypeDef, _OptionalGetLFTagRequestRequestTypeDef
 ):
     pass
 
 
-GetLFTagResponseTypeDef = TypedDict(
-    "GetLFTagResponseTypeDef",
-    {
-        "CatalogId": str,
-        "TagKey": str,
-        "TagValues": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStateRequestRequestTypeDef = TypedDict(
     "GetQueryStateRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-GetQueryStateResponseTypeDef = TypedDict(
-    "GetQueryStateResponseTypeDef",
-    {
-        "Error": str,
-        "State": QueryStateStringType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStatisticsRequestRequestTypeDef = TypedDict(
     "GetQueryStatisticsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
@@ -632,15 +674,14 @@
     "PlanningStatisticsTypeDef",
     {
         "EstimatedDataToScanBytes": int,
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
-    total=False,
 )
 
 _RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
@@ -669,75 +710,33 @@
 PartitionValueListTypeDef = TypedDict(
     "PartitionValueListTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
-GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkUnitResultsRequestRequestTypeDef = TypedDict(
     "GetWorkUnitResultsRequestRequestTypeDef",
     {
         "QueryId": str,
         "WorkUnitId": int,
         "WorkUnitToken": str,
     },
 )
 
-GetWorkUnitResultsResponseTypeDef = TypedDict(
-    "GetWorkUnitResultsResponseTypeDef",
-    {
-        "ResultStream": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    {
-        "QueryId": str,
-    },
-)
-_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
-    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetWorkUnitsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkUnitsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalGetWorkUnitsRequestRequestTypeDef = TypedDict(
@@ -761,14 +760,23 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
+LFTagKeyResourceOutputTypeDef = TypedDict(
+    "LFTagKeyResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -781,14 +789,22 @@
 )
 
 
 class LFTagKeyResourceTypeDef(_RequiredLFTagKeyResourceTypeDef, _OptionalLFTagKeyResourceTypeDef):
     pass
 
 
+LFTagOutputTypeDef = TypedDict(
+    "LFTagOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -810,24 +826,14 @@
 )
 
 
 class TableResourceTypeDef(_RequiredTableResourceTypeDef, _OptionalTableResourceTypeDef):
     pass
 
 
-ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "ResourceShareType": ResourceShareTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLFTagsRequestRequestTypeDef = TypedDict(
     "ListLFTagsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "MaxResults": int,
         "NextToken": str,
@@ -866,46 +872,34 @@
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
         "LastRunDetails": str,
     },
-    total=False,
 )
 
 ListTransactionsRequestRequestTypeDef = TypedDict(
     "ListTransactionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "StatusFilter": TransactionStatusFilterType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
-    total=False,
 )
 
 _RequiredQueryPlanningContextTypeDef = TypedDict(
     "_RequiredQueryPlanningContextTypeDef",
     {
         "DatabaseName": str,
     },
@@ -947,49 +941,32 @@
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-StartQueryPlanningResponseTypeDef = TypedDict(
-    "StartQueryPlanningResponseTypeDef",
+TableResourceOutputTypeDef = TypedDict(
+    "TableResourceOutputTypeDef",
     {
-        "QueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CatalogId": str,
+        "DatabaseName": str,
+        "Name": str,
+        "TableWildcard": Dict[str, Any],
     },
 )
 
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
 
-StartTransactionResponseTypeDef = TypedDict(
-    "StartTransactionResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
     },
 )
 _OptionalUpdateLFTagRequestRequestTypeDef = TypedDict(
@@ -1051,83 +1028,184 @@
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
-    "UpdateTableStorageOptimizerResponseTypeDef",
+AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     {
-        "Result": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ColumnLFTagTypeDef = TypedDict(
-    "ColumnLFTagTypeDef",
+CommitTransactionResponseTypeDef = TypedDict(
+    "CommitTransactionResponseTypeDef",
     {
-        "Name": str,
-        "LFTags": List[LFTagPairTypeDef],
+        "TransactionStatus": TransactionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListLFTagsResponseTypeDef = TypedDict(
-    "ListLFTagsResponseTypeDef",
+GetLFTagResponseTypeDef = TypedDict(
+    "GetLFTagResponseTypeDef",
     {
-        "LFTags": List[LFTagPairTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueryStateResponseTypeDef = TypedDict(
+    "GetQueryStateResponseTypeDef",
+    {
+        "Error": str,
+        "State": QueryStateStringType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkUnitResultsResponseTypeDef = TypedDict(
+    "GetWorkUnitResultsResponseTypeDef",
+    {
+        "ResultStream": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryPlanningResponseTypeDef = TypedDict(
+    "StartQueryPlanningResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartTransactionResponseTypeDef = TypedDict(
+    "StartTransactionResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
+    "UpdateTableStorageOptimizerResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
-        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
 )
 _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "Permissions": Sequence[PermissionType],
         "DurationSeconds": int,
         "AuditContext": AuditContextTypeDef,
+        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
     total=False,
 )
 
 
 class GetTemporaryGlueTableCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
 ):
     pass
 
 
-LFTagErrorTypeDef = TypedDict(
-    "LFTagErrorTypeDef",
+PrincipalPermissionsOutputTypeDef = TypedDict(
+    "PrincipalPermissionsOutputTypeDef",
     {
-        "LFTag": LFTagPairTypeDef,
-        "Error": ErrorDetailTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
+        "Permissions": List[PermissionType],
     },
-    total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
-        "Permissions": List[PermissionType],
+        "Permissions": Sequence[PermissionType],
     },
     total=False,
 )
 
+ColumnLFTagTypeDef = TypedDict(
+    "ColumnLFTagTypeDef",
+    {
+        "Name": str,
+        "LFTags": List[LFTagPairOutputTypeDef],
+    },
+)
+
+LFTagErrorTypeDef = TypedDict(
+    "LFTagErrorTypeDef",
+    {
+        "LFTag": LFTagPairOutputTypeDef,
+        "Error": ErrorDetailTypeDef,
+    },
+)
+
+ListLFTagsResponseTypeDef = TypedDict(
+    "ListLFTagsResponseTypeDef",
+    {
+        "LFTags": List[LFTagPairOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableWithColumnsResourceOutputTypeDef = TypedDict(
+    "TableWithColumnsResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "DatabaseName": str,
+        "Name": str,
+        "ColumnNames": List[str],
+        "ColumnWildcard": ColumnWildcardOutputTypeDef,
+    },
+)
+
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1144,14 +1222,28 @@
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
 
+DataCellsFilterOutputTypeDef = TypedDict(
+    "DataCellsFilterOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+        "RowFilter": RowFilterOutputTypeDef,
+        "ColumnNames": List[str],
+        "ColumnWildcard": ColumnWildcardOutputTypeDef,
+        "VersionId": str,
+    },
+)
+
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1172,18 +1264,17 @@
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
-        "Database": DatabaseResourceTypeDef,
-        "LFTags": List[LFTagPairTypeDef],
+        "Database": DatabaseResourceOutputTypeDef,
+        "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
         "AddObject": AddObjectInputTypeDef,
         "DeleteObject": DeleteObjectInputTypeDef,
@@ -1216,41 +1307,41 @@
     pass
 
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceInfo": ResourceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "ResourceInfoList": List[ResourceInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTransactionResponseTypeDef = TypedDict(
     "DescribeTransactionResponseTypeDef",
     {
         "TransactionDescription": TransactionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTransactionsResponseTypeDef = TypedDict(
     "ListTransactionsResponseTypeDef",
     {
         "Transactions": List[TransactionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesRequestRequestTypeDef = TypedDict(
     "ListResourcesRequestRequestTypeDef",
     {
         "FilterConditionList": Sequence[FilterConditionTypeDef],
@@ -1262,51 +1353,92 @@
 
 GetQueryStatisticsResponseTypeDef = TypedDict(
     "GetQueryStatisticsResponseTypeDef",
     {
         "ExecutionStatistics": ExecutionStatisticsTypeDef,
         "PlanningStatistics": PlanningStatisticsTypeDef,
         "QuerySubmissionTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
         "Partition": PartitionValueListTypeDef,
-        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
 )
 _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "Permissions": Sequence[PermissionType],
         "DurationSeconds": int,
         "AuditContext": AuditContextTypeDef,
+        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
     total=False,
 )
 
 
 class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    {
+        "QueryId": str,
+    },
+)
+_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
+    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+):
+    pass
+
+
+ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceShareType": ResourceShareTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetWorkUnitsResponseTypeDef = TypedDict(
     "GetWorkUnitsResponseTypeDef",
     {
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LFTagPolicyResourceOutputTypeDef = TypedDict(
+    "LFTagPolicyResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceType": ResourceTypeType,
+        "Expression": List[LFTagOutputTypeDef],
     },
 )
 
 _RequiredLFTagPolicyResourceTypeDef = TypedDict(
     "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
@@ -1358,15 +1490,15 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
     _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
@@ -1405,15 +1537,15 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
     _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
@@ -1422,15 +1554,15 @@
     pass
 
 
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDataCellsFilterRequestRequestTypeDef = TypedDict(
     "ListDataCellsFilterRequestRequestTypeDef",
     {
@@ -1442,108 +1574,124 @@
 )
 
 ListTableStorageOptimizersResponseTypeDef = TypedDict(
     "ListTableStorageOptimizersResponseTypeDef",
     {
         "StorageOptimizerList": List[StorageOptimizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
-    total=False,
 )
 
 StartQueryPlanningRequestRequestTypeDef = TypedDict(
     "StartQueryPlanningRequestRequestTypeDef",
     {
         "QueryPlanningContext": QueryPlanningContextTypeDef,
         "QueryString": str,
     },
 )
 
+DataLakeSettingsOutputTypeDef = TypedDict(
+    "DataLakeSettingsOutputTypeDef",
+    {
+        "DataLakeAdmins": List[DataLakePrincipalOutputTypeDef],
+        "ReadOnlyAdmins": List[DataLakePrincipalOutputTypeDef],
+        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "Parameters": Dict[str, str],
+        "TrustedResourceOwners": List[str],
+        "AllowExternalDataFiltering": bool,
+        "AllowFullTableExternalDataAccess": bool,
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalOutputTypeDef],
+        "AuthorizedSessionTagValueList": List[str],
+    },
+)
+
+DataLakeSettingsTypeDef = TypedDict(
+    "DataLakeSettingsTypeDef",
+    {
+        "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
+        "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
+        "CreateDatabaseDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "Parameters": Mapping[str, str],
+        "TrustedResourceOwners": Sequence[str],
+        "AllowExternalDataFiltering": bool,
+        "AllowFullTableExternalDataAccess": bool,
+        "ExternalDataFilteringAllowList": Sequence[DataLakePrincipalTypeDef],
+        "AuthorizedSessionTagValueList": Sequence[str],
+    },
+    total=False,
+)
+
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
-        "LFTagOnDatabase": List[LFTagPairTypeDef],
-        "LFTagsOnTable": List[LFTagPairTypeDef],
+        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
+        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedTableTypeDef = TypedDict(
     "TaggedTableTypeDef",
     {
-        "Table": TableResourceTypeDef,
-        "LFTagOnDatabase": List[LFTagPairTypeDef],
-        "LFTagsOnTable": List[LFTagPairTypeDef],
+        "Table": TableResourceOutputTypeDef,
+        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
+        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
-    total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveLFTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DataLakeSettingsTypeDef = TypedDict(
-    "DataLakeSettingsTypeDef",
-    {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsTypeDef],
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
-        "Parameters": Dict[str, str],
-        "TrustedResourceOwners": List[str],
-        "AllowExternalDataFiltering": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": List[str],
-    },
-    total=False,
-)
-
-CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
-    "CreateDataCellsFilterRequestRequestTypeDef",
-    {
-        "TableData": DataCellsFilterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilter": DataCellsFilterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataCellsFilter": DataCellsFilterOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataCellsFilterResponseTypeDef = TypedDict(
     "ListDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilters": List[DataCellsFilterTypeDef],
+        "DataCellsFilters": List[DataCellsFilterOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
+    "CreateDataCellsFilterRequestRequestTypeDef",
+    {
+        "TableData": DataCellsFilterTypeDef,
     },
 )
 
 UpdateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "UpdateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
@@ -1551,15 +1699,15 @@
 )
 
 SearchDatabasesByLFTagsResponseTypeDef = TypedDict(
     "SearchDatabasesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "DatabaseList": List[TaggedDatabaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -1580,14 +1728,28 @@
 class UpdateTableObjectsRequestRequestTypeDef(
     _RequiredUpdateTableObjectsRequestRequestTypeDef,
     _OptionalUpdateTableObjectsRequestRequestTypeDef,
 ):
     pass
 
 
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
+    {
+        "Catalog": Dict[str, Any],
+        "Database": DatabaseResourceOutputTypeDef,
+        "Table": TableResourceOutputTypeDef,
+        "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
+        "DataLocation": DataLocationResourceOutputTypeDef,
+        "DataCellsFilter": DataCellsFilterResourceOutputTypeDef,
+        "LFTag": LFTagKeyResourceOutputTypeDef,
+        "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
+    },
+)
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
         "Table": TableResourceTypeDef,
         "TableWithColumns": TableWithColumnsResourceTypeDef,
@@ -1600,32 +1762,23 @@
 )
 
 GetTableObjectsResponseTypeDef = TypedDict(
     "GetTableObjectsResponseTypeDef",
     {
         "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SearchTablesByLFTagsResponseTypeDef = TypedDict(
-    "SearchTablesByLFTagsResponseTypeDef",
-    {
-        "NextToken": str,
-        "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
-        "DataLakeSettings": DataLakeSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataLakeSettings": DataLakeSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
@@ -1643,14 +1796,45 @@
 class PutDataLakeSettingsRequestRequestTypeDef(
     _RequiredPutDataLakeSettingsRequestRequestTypeDef,
     _OptionalPutDataLakeSettingsRequestRequestTypeDef,
 ):
     pass
 
 
+SearchTablesByLFTagsResponseTypeDef = TypedDict(
+    "SearchTablesByLFTagsResponseTypeDef",
+    {
+        "NextToken": str,
+        "TableList": List[TaggedTableTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "BatchPermissionsRequestEntryOutputTypeDef",
+    {
+        "Id": str,
+        "Principal": DataLakePrincipalOutputTypeDef,
+        "Resource": ResourceOutputTypeDef,
+        "Permissions": List[PermissionType],
+        "PermissionsWithGrantOption": List[PermissionType],
+    },
+)
+
+PrincipalResourcePermissionsTypeDef = TypedDict(
+    "PrincipalResourcePermissionsTypeDef",
+    {
+        "Principal": DataLakePrincipalOutputTypeDef,
+        "Resource": ResourceOutputTypeDef,
+        "Permissions": List[PermissionType],
+        "PermissionsWithGrantOption": List[PermissionType],
+        "AdditionalDetails": DetailsMapTypeDef,
+    },
+)
+
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
         "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
@@ -1750,26 +1934,14 @@
         "NextToken": str,
         "MaxResults": int,
         "IncludeRelated": str,
     },
     total=False,
 )
 
-PrincipalResourcePermissionsTypeDef = TypedDict(
-    "PrincipalResourcePermissionsTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Resource": ResourceTypeDef,
-        "Permissions": List[PermissionType],
-        "PermissionsWithGrantOption": List[PermissionType],
-        "AdditionalDetails": DetailsMapTypeDef,
-    },
-    total=False,
-)
-
 _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
         "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
@@ -1809,14 +1981,40 @@
 
 class RevokePermissionsRequestRequestTypeDef(
     _RequiredRevokePermissionsRequestRequestTypeDef, _OptionalRevokePermissionsRequestRequestTypeDef
 ):
     pass
 
 
+BatchPermissionsFailureEntryTypeDef = TypedDict(
+    "BatchPermissionsFailureEntryTypeDef",
+    {
+        "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
+        "Error": ErrorDetailTypeDef,
+    },
+)
+
+GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
+    "GetEffectivePermissionsForPathResponseTypeDef",
+    {
+        "Permissions": List[PrincipalResourcePermissionsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPermissionsResponseTypeDef = TypedDict(
+    "ListPermissionsResponseTypeDef",
+    {
+        "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
     {
         "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
@@ -1831,23 +2029,14 @@
 class BatchGrantPermissionsRequestRequestTypeDef(
     _RequiredBatchGrantPermissionsRequestRequestTypeDef,
     _OptionalBatchGrantPermissionsRequestRequestTypeDef,
 ):
     pass
 
 
-BatchPermissionsFailureEntryTypeDef = TypedDict(
-    "BatchPermissionsFailureEntryTypeDef",
-    {
-        "RequestEntry": BatchPermissionsRequestEntryTypeDef,
-        "Error": ErrorDetailTypeDef,
-    },
-    total=False,
-)
-
 _RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
     {
         "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
@@ -1862,40 +2051,22 @@
 class BatchRevokePermissionsRequestRequestTypeDef(
     _RequiredBatchRevokePermissionsRequestRequestTypeDef,
     _OptionalBatchRevokePermissionsRequestRequestTypeDef,
 ):
     pass
 
 
-GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
-    "GetEffectivePermissionsForPathResponseTypeDef",
-    {
-        "Permissions": List[PrincipalResourcePermissionsTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPermissionsResponseTypeDef = TypedDict(
-    "ListPermissionsResponseTypeDef",
-    {
-        "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchGrantPermissionsResponseTypeDef = TypedDict(
     "BatchGrantPermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchRevokePermissionsResponseTypeDef = TypedDict(
     "BatchRevokePermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation/type_defs.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -35,28 +35,34 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "LFTagPairTypeDef",
+    "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
+    "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
+    "LFTagPairOutputTypeDef",
+    "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
-    "CommitTransactionResponseTypeDef",
     "CreateLFTagRequestRequestTypeDef",
+    "RowFilterOutputTypeDef",
+    "DataCellsFilterResourceOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
+    "DataLocationResourceOutputTypeDef",
     "DataLocationResourceTypeDef",
+    "DatabaseResourceOutputTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
     "VirtualObjectTypeDef",
     "DeregisterResourceRequestRequestTypeDef",
     "DescribeResourceRequestRequestTypeDef",
@@ -67,105 +73,116 @@
     "ExecutionStatisticsTypeDef",
     "ExtendTransactionRequestRequestTypeDef",
     "FilterConditionTypeDef",
     "GetDataCellsFilterRequestRequestTypeDef",
     "GetDataLakeSettingsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathRequestRequestTypeDef",
     "GetLFTagRequestRequestTypeDef",
-    "GetLFTagResponseTypeDef",
     "GetQueryStateRequestRequestTypeDef",
-    "GetQueryStateResponseTypeDef",
     "GetQueryStatisticsRequestRequestTypeDef",
     "PlanningStatisticsTypeDef",
     "GetTableObjectsRequestRequestTypeDef",
     "PartitionValueListTypeDef",
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
-    "GetWorkUnitResultsResponseTypeDef",
-    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
+    "LFTagKeyResourceOutputTypeDef",
     "LFTagKeyResourceTypeDef",
+    "LFTagOutputTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "TableObjectTypeDef",
     "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartQueryPlanningResponseTypeDef",
+    "TableResourceOutputTypeDef",
     "StartTransactionRequestRequestTypeDef",
-    "StartTransactionResponseTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
+    "CommitTransactionResponseTypeDef",
+    "GetLFTagResponseTypeDef",
+    "GetQueryStateResponseTypeDef",
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    "GetWorkUnitResultsResponseTypeDef",
+    "StartQueryPlanningResponseTypeDef",
+    "StartTransactionResponseTypeDef",
     "UpdateTableStorageOptimizerResponseTypeDef",
-    "ColumnLFTagTypeDef",
-    "ListLFTagsResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
-    "LFTagErrorTypeDef",
+    "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
+    "ColumnLFTagTypeDef",
+    "LFTagErrorTypeDef",
+    "ListLFTagsResponseTypeDef",
+    "TableWithColumnsResourceOutputTypeDef",
     "TableWithColumnsResourceTypeDef",
+    "DataCellsFilterOutputTypeDef",
     "DataCellsFilterTypeDef",
     "TaggedDatabaseTypeDef",
     "WriteOperationTypeDef",
     "DeleteObjectsOnCancelRequestRequestTypeDef",
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
     "ListTransactionsResponseTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "GetQueryStatisticsResponseTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
+    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
+    "LFTagPolicyResourceOutputTypeDef",
     "LFTagPolicyResourceTypeDef",
     "SearchDatabasesByLFTagsRequestRequestTypeDef",
     "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     "SearchTablesByLFTagsRequestRequestTypeDef",
     "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     "ListDataCellsFilterRequestRequestTypeDef",
     "ListTableStorageOptimizersResponseTypeDef",
     "PartitionObjectsTypeDef",
     "StartQueryPlanningRequestRequestTypeDef",
+    "DataLakeSettingsOutputTypeDef",
+    "DataLakeSettingsTypeDef",
     "GetResourceLFTagsResponseTypeDef",
     "TaggedTableTypeDef",
     "AddLFTagsToResourceResponseTypeDef",
     "RemoveLFTagsFromResourceResponseTypeDef",
-    "DataLakeSettingsTypeDef",
-    "CreateDataCellsFilterRequestRequestTypeDef",
     "GetDataCellsFilterResponseTypeDef",
     "ListDataCellsFilterResponseTypeDef",
+    "CreateDataCellsFilterRequestRequestTypeDef",
     "UpdateDataCellsFilterRequestRequestTypeDef",
     "SearchDatabasesByLFTagsResponseTypeDef",
     "UpdateTableObjectsRequestRequestTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "GetTableObjectsResponseTypeDef",
-    "SearchTablesByLFTagsResponseTypeDef",
     "GetDataLakeSettingsResponseTypeDef",
     "PutDataLakeSettingsRequestRequestTypeDef",
+    "SearchTablesByLFTagsResponseTypeDef",
+    "BatchPermissionsRequestEntryOutputTypeDef",
+    "PrincipalResourcePermissionsTypeDef",
     "AddLFTagsToResourceRequestRequestTypeDef",
     "BatchPermissionsRequestEntryTypeDef",
     "GetResourceLFTagsRequestRequestTypeDef",
     "GrantPermissionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
-    "PrincipalResourcePermissionsTypeDef",
     "RemoveLFTagsFromResourceRequestRequestTypeDef",
     "RevokePermissionsRequestRequestTypeDef",
-    "BatchGrantPermissionsRequestRequestTypeDef",
     "BatchPermissionsFailureEntryTypeDef",
-    "BatchRevokePermissionsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathResponseTypeDef",
     "ListPermissionsResponseTypeDef",
+    "BatchGrantPermissionsRequestRequestTypeDef",
+    "BatchRevokePermissionsRequestRequestTypeDef",
     "BatchGrantPermissionsResponseTypeDef",
     "BatchRevokePermissionsResponseTypeDef",
 )
 
 _RequiredLFTagPairTypeDef = TypedDict(
     "_RequiredLFTagPairTypeDef",
     {
@@ -180,14 +197,25 @@
     },
     total=False,
 )
 
 class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
     pass
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredAddObjectInputTypeDef = TypedDict(
     "_RequiredAddObjectInputTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
@@ -221,40 +249,35 @@
 
 class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
-AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
     },
     total=False,
 )
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+DataLakePrincipalOutputTypeDef = TypedDict(
+    "DataLakePrincipalOutputTypeDef",
+    {
+        "DataLakePrincipalIdentifier": str,
+    },
 )
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
@@ -264,14 +287,30 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
+LFTagPairOutputTypeDef = TypedDict(
+    "LFTagPairOutputTypeDef",
+    {
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
+ColumnWildcardOutputTypeDef = TypedDict(
+    "ColumnWildcardOutputTypeDef",
+    {
+        "ExcludedColumnNames": List[str],
+    },
+)
+
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
     total=False,
 )
@@ -279,22 +318,14 @@
 CommitTransactionRequestRequestTypeDef = TypedDict(
     "CommitTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-CommitTransactionResponseTypeDef = TypedDict(
-    "CommitTransactionResponseTypeDef",
-    {
-        "TransactionStatus": TransactionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -307,14 +338,32 @@
 )
 
 class CreateLFTagRequestRequestTypeDef(
     _RequiredCreateLFTagRequestRequestTypeDef, _OptionalCreateLFTagRequestRequestTypeDef
 ):
     pass
 
+RowFilterOutputTypeDef = TypedDict(
+    "RowFilterOutputTypeDef",
+    {
+        "FilterExpression": str,
+        "AllRowsWildcard": Dict[str, Any],
+    },
+)
+
+DataCellsFilterResourceOutputTypeDef = TypedDict(
+    "DataCellsFilterResourceOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+    },
+)
+
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -327,14 +376,22 @@
     {
         "FilterExpression": str,
         "AllRowsWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
+DataLocationResourceOutputTypeDef = TypedDict(
+    "DataLocationResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredDataLocationResourceTypeDef = TypedDict(
     "_RequiredDataLocationResourceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalDataLocationResourceTypeDef = TypedDict(
@@ -346,14 +403,22 @@
 )
 
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
+DatabaseResourceOutputTypeDef = TypedDict(
+    "DatabaseResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "Name": str,
+    },
+)
+
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
@@ -452,15 +517,14 @@
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
         "WithFederation": bool,
     },
-    total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -470,33 +534,30 @@
     "TransactionDescriptionTypeDef",
     {
         "TransactionId": str,
         "TransactionStatus": TransactionStatusType,
         "TransactionStartTime": datetime,
         "TransactionEndTime": datetime,
     },
-    total=False,
 )
 
 DetailsMapTypeDef = TypedDict(
     "DetailsMapTypeDef",
     {
         "ResourceShare": List[str],
     },
-    total=False,
 )
 
 ExecutionStatisticsTypeDef = TypedDict(
     "ExecutionStatisticsTypeDef",
     {
         "AverageExecutionTimeMillis": int,
         "DataScannedBytes": int,
         "WorkUnitsExecutedCount": int,
     },
-    total=False,
 )
 
 ExtendTransactionRequestRequestTypeDef = TypedDict(
     "ExtendTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -568,40 +629,21 @@
 )
 
 class GetLFTagRequestRequestTypeDef(
     _RequiredGetLFTagRequestRequestTypeDef, _OptionalGetLFTagRequestRequestTypeDef
 ):
     pass
 
-GetLFTagResponseTypeDef = TypedDict(
-    "GetLFTagResponseTypeDef",
-    {
-        "CatalogId": str,
-        "TagKey": str,
-        "TagValues": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStateRequestRequestTypeDef = TypedDict(
     "GetQueryStateRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-GetQueryStateResponseTypeDef = TypedDict(
-    "GetQueryStateResponseTypeDef",
-    {
-        "Error": str,
-        "State": QueryStateStringType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStatisticsRequestRequestTypeDef = TypedDict(
     "GetQueryStatisticsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
@@ -609,15 +651,14 @@
     "PlanningStatisticsTypeDef",
     {
         "EstimatedDataToScanBytes": int,
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
-    total=False,
 )
 
 _RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
@@ -644,73 +685,33 @@
 PartitionValueListTypeDef = TypedDict(
     "PartitionValueListTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
-GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkUnitResultsRequestRequestTypeDef = TypedDict(
     "GetWorkUnitResultsRequestRequestTypeDef",
     {
         "QueryId": str,
         "WorkUnitId": int,
         "WorkUnitToken": str,
     },
 )
 
-GetWorkUnitResultsResponseTypeDef = TypedDict(
-    "GetWorkUnitResultsResponseTypeDef",
-    {
-        "ResultStream": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    {
-        "QueryId": str,
-    },
-)
-_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
-    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetWorkUnitsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkUnitsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalGetWorkUnitsRequestRequestTypeDef = TypedDict(
@@ -732,14 +733,23 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
+LFTagKeyResourceOutputTypeDef = TypedDict(
+    "LFTagKeyResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -750,14 +760,22 @@
     },
     total=False,
 )
 
 class LFTagKeyResourceTypeDef(_RequiredLFTagKeyResourceTypeDef, _OptionalLFTagKeyResourceTypeDef):
     pass
 
+LFTagOutputTypeDef = TypedDict(
+    "LFTagOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -777,24 +795,14 @@
     },
     total=False,
 )
 
 class TableResourceTypeDef(_RequiredTableResourceTypeDef, _OptionalTableResourceTypeDef):
     pass
 
-ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "ResourceShareType": ResourceShareTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLFTagsRequestRequestTypeDef = TypedDict(
     "ListLFTagsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "MaxResults": int,
         "NextToken": str,
@@ -831,46 +839,34 @@
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
         "LastRunDetails": str,
     },
-    total=False,
 )
 
 ListTransactionsRequestRequestTypeDef = TypedDict(
     "ListTransactionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "StatusFilter": TransactionStatusFilterType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
-    total=False,
 )
 
 _RequiredQueryPlanningContextTypeDef = TypedDict(
     "_RequiredQueryPlanningContextTypeDef",
     {
         "DatabaseName": str,
     },
@@ -908,49 +904,32 @@
 )
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-StartQueryPlanningResponseTypeDef = TypedDict(
-    "StartQueryPlanningResponseTypeDef",
+TableResourceOutputTypeDef = TypedDict(
+    "TableResourceOutputTypeDef",
     {
-        "QueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CatalogId": str,
+        "DatabaseName": str,
+        "Name": str,
+        "TableWildcard": Dict[str, Any],
     },
 )
 
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
 
-StartTransactionResponseTypeDef = TypedDict(
-    "StartTransactionResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
     },
 )
 _OptionalUpdateLFTagRequestRequestTypeDef = TypedDict(
@@ -1006,81 +985,182 @@
 
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
-UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
-    "UpdateTableStorageOptimizerResponseTypeDef",
+AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     {
-        "Result": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ColumnLFTagTypeDef = TypedDict(
-    "ColumnLFTagTypeDef",
+CommitTransactionResponseTypeDef = TypedDict(
+    "CommitTransactionResponseTypeDef",
     {
-        "Name": str,
-        "LFTags": List[LFTagPairTypeDef],
+        "TransactionStatus": TransactionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListLFTagsResponseTypeDef = TypedDict(
-    "ListLFTagsResponseTypeDef",
+GetLFTagResponseTypeDef = TypedDict(
+    "GetLFTagResponseTypeDef",
     {
-        "LFTags": List[LFTagPairTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueryStateResponseTypeDef = TypedDict(
+    "GetQueryStateResponseTypeDef",
+    {
+        "Error": str,
+        "State": QueryStateStringType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkUnitResultsResponseTypeDef = TypedDict(
+    "GetWorkUnitResultsResponseTypeDef",
+    {
+        "ResultStream": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryPlanningResponseTypeDef = TypedDict(
+    "StartQueryPlanningResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartTransactionResponseTypeDef = TypedDict(
+    "StartTransactionResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
+    "UpdateTableStorageOptimizerResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
-        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
 )
 _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "Permissions": Sequence[PermissionType],
         "DurationSeconds": int,
         "AuditContext": AuditContextTypeDef,
+        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
     total=False,
 )
 
 class GetTemporaryGlueTableCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
 ):
     pass
 
-LFTagErrorTypeDef = TypedDict(
-    "LFTagErrorTypeDef",
+PrincipalPermissionsOutputTypeDef = TypedDict(
+    "PrincipalPermissionsOutputTypeDef",
     {
-        "LFTag": LFTagPairTypeDef,
-        "Error": ErrorDetailTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
+        "Permissions": List[PermissionType],
     },
-    total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
-        "Permissions": List[PermissionType],
+        "Permissions": Sequence[PermissionType],
     },
     total=False,
 )
 
+ColumnLFTagTypeDef = TypedDict(
+    "ColumnLFTagTypeDef",
+    {
+        "Name": str,
+        "LFTags": List[LFTagPairOutputTypeDef],
+    },
+)
+
+LFTagErrorTypeDef = TypedDict(
+    "LFTagErrorTypeDef",
+    {
+        "LFTag": LFTagPairOutputTypeDef,
+        "Error": ErrorDetailTypeDef,
+    },
+)
+
+ListLFTagsResponseTypeDef = TypedDict(
+    "ListLFTagsResponseTypeDef",
+    {
+        "LFTags": List[LFTagPairOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableWithColumnsResourceOutputTypeDef = TypedDict(
+    "TableWithColumnsResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "DatabaseName": str,
+        "Name": str,
+        "ColumnNames": List[str],
+        "ColumnWildcard": ColumnWildcardOutputTypeDef,
+    },
+)
+
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1095,14 +1175,28 @@
 )
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
+DataCellsFilterOutputTypeDef = TypedDict(
+    "DataCellsFilterOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+        "RowFilter": RowFilterOutputTypeDef,
+        "ColumnNames": List[str],
+        "ColumnWildcard": ColumnWildcardOutputTypeDef,
+        "VersionId": str,
+    },
+)
+
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1121,18 +1215,17 @@
 
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
-        "Database": DatabaseResourceTypeDef,
-        "LFTags": List[LFTagPairTypeDef],
+        "Database": DatabaseResourceOutputTypeDef,
+        "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
         "AddObject": AddObjectInputTypeDef,
         "DeleteObject": DeleteObjectInputTypeDef,
@@ -1163,41 +1256,41 @@
 ):
     pass
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceInfo": ResourceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "ResourceInfoList": List[ResourceInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTransactionResponseTypeDef = TypedDict(
     "DescribeTransactionResponseTypeDef",
     {
         "TransactionDescription": TransactionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTransactionsResponseTypeDef = TypedDict(
     "ListTransactionsResponseTypeDef",
     {
         "Transactions": List[TransactionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesRequestRequestTypeDef = TypedDict(
     "ListResourcesRequestRequestTypeDef",
     {
         "FilterConditionList": Sequence[FilterConditionTypeDef],
@@ -1209,49 +1302,88 @@
 
 GetQueryStatisticsResponseTypeDef = TypedDict(
     "GetQueryStatisticsResponseTypeDef",
     {
         "ExecutionStatistics": ExecutionStatisticsTypeDef,
         "PlanningStatistics": PlanningStatisticsTypeDef,
         "QuerySubmissionTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
         "Partition": PartitionValueListTypeDef,
-        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
 )
 _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "Permissions": Sequence[PermissionType],
         "DurationSeconds": int,
         "AuditContext": AuditContextTypeDef,
+        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
     total=False,
 )
 
 class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    {
+        "QueryId": str,
+    },
+)
+_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
+    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+):
+    pass
+
+ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceShareType": ResourceShareTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetWorkUnitsResponseTypeDef = TypedDict(
     "GetWorkUnitsResponseTypeDef",
     {
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LFTagPolicyResourceOutputTypeDef = TypedDict(
+    "LFTagPolicyResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceType": ResourceTypeType,
+        "Expression": List[LFTagOutputTypeDef],
     },
 )
 
 _RequiredLFTagPolicyResourceTypeDef = TypedDict(
     "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
@@ -1299,15 +1431,15 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
     _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
@@ -1342,30 +1474,30 @@
         "Expression": Sequence[LFTagTypeDef],
     },
 )
 _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
     "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
     _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
 ):
     pass
 
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDataCellsFilterRequestRequestTypeDef = TypedDict(
     "ListDataCellsFilterRequestRequestTypeDef",
     {
@@ -1377,108 +1509,124 @@
 )
 
 ListTableStorageOptimizersResponseTypeDef = TypedDict(
     "ListTableStorageOptimizersResponseTypeDef",
     {
         "StorageOptimizerList": List[StorageOptimizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
-    total=False,
 )
 
 StartQueryPlanningRequestRequestTypeDef = TypedDict(
     "StartQueryPlanningRequestRequestTypeDef",
     {
         "QueryPlanningContext": QueryPlanningContextTypeDef,
         "QueryString": str,
     },
 )
 
+DataLakeSettingsOutputTypeDef = TypedDict(
+    "DataLakeSettingsOutputTypeDef",
+    {
+        "DataLakeAdmins": List[DataLakePrincipalOutputTypeDef],
+        "ReadOnlyAdmins": List[DataLakePrincipalOutputTypeDef],
+        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "Parameters": Dict[str, str],
+        "TrustedResourceOwners": List[str],
+        "AllowExternalDataFiltering": bool,
+        "AllowFullTableExternalDataAccess": bool,
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalOutputTypeDef],
+        "AuthorizedSessionTagValueList": List[str],
+    },
+)
+
+DataLakeSettingsTypeDef = TypedDict(
+    "DataLakeSettingsTypeDef",
+    {
+        "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
+        "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
+        "CreateDatabaseDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "Parameters": Mapping[str, str],
+        "TrustedResourceOwners": Sequence[str],
+        "AllowExternalDataFiltering": bool,
+        "AllowFullTableExternalDataAccess": bool,
+        "ExternalDataFilteringAllowList": Sequence[DataLakePrincipalTypeDef],
+        "AuthorizedSessionTagValueList": Sequence[str],
+    },
+    total=False,
+)
+
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
-        "LFTagOnDatabase": List[LFTagPairTypeDef],
-        "LFTagsOnTable": List[LFTagPairTypeDef],
+        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
+        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedTableTypeDef = TypedDict(
     "TaggedTableTypeDef",
     {
-        "Table": TableResourceTypeDef,
-        "LFTagOnDatabase": List[LFTagPairTypeDef],
-        "LFTagsOnTable": List[LFTagPairTypeDef],
+        "Table": TableResourceOutputTypeDef,
+        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
+        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
-    total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveLFTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DataLakeSettingsTypeDef = TypedDict(
-    "DataLakeSettingsTypeDef",
-    {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsTypeDef],
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
-        "Parameters": Dict[str, str],
-        "TrustedResourceOwners": List[str],
-        "AllowExternalDataFiltering": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": List[str],
-    },
-    total=False,
-)
-
-CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
-    "CreateDataCellsFilterRequestRequestTypeDef",
-    {
-        "TableData": DataCellsFilterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilter": DataCellsFilterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataCellsFilter": DataCellsFilterOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataCellsFilterResponseTypeDef = TypedDict(
     "ListDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilters": List[DataCellsFilterTypeDef],
+        "DataCellsFilters": List[DataCellsFilterOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
+    "CreateDataCellsFilterRequestRequestTypeDef",
+    {
+        "TableData": DataCellsFilterTypeDef,
     },
 )
 
 UpdateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "UpdateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
@@ -1486,15 +1634,15 @@
 )
 
 SearchDatabasesByLFTagsResponseTypeDef = TypedDict(
     "SearchDatabasesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "DatabaseList": List[TaggedDatabaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -1513,14 +1661,28 @@
 
 class UpdateTableObjectsRequestRequestTypeDef(
     _RequiredUpdateTableObjectsRequestRequestTypeDef,
     _OptionalUpdateTableObjectsRequestRequestTypeDef,
 ):
     pass
 
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
+    {
+        "Catalog": Dict[str, Any],
+        "Database": DatabaseResourceOutputTypeDef,
+        "Table": TableResourceOutputTypeDef,
+        "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
+        "DataLocation": DataLocationResourceOutputTypeDef,
+        "DataCellsFilter": DataCellsFilterResourceOutputTypeDef,
+        "LFTag": LFTagKeyResourceOutputTypeDef,
+        "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
+    },
+)
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
         "Table": TableResourceTypeDef,
         "TableWithColumns": TableWithColumnsResourceTypeDef,
@@ -1533,32 +1695,23 @@
 )
 
 GetTableObjectsResponseTypeDef = TypedDict(
     "GetTableObjectsResponseTypeDef",
     {
         "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SearchTablesByLFTagsResponseTypeDef = TypedDict(
-    "SearchTablesByLFTagsResponseTypeDef",
-    {
-        "NextToken": str,
-        "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
-        "DataLakeSettings": DataLakeSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataLakeSettings": DataLakeSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
@@ -1574,14 +1727,45 @@
 
 class PutDataLakeSettingsRequestRequestTypeDef(
     _RequiredPutDataLakeSettingsRequestRequestTypeDef,
     _OptionalPutDataLakeSettingsRequestRequestTypeDef,
 ):
     pass
 
+SearchTablesByLFTagsResponseTypeDef = TypedDict(
+    "SearchTablesByLFTagsResponseTypeDef",
+    {
+        "NextToken": str,
+        "TableList": List[TaggedTableTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "BatchPermissionsRequestEntryOutputTypeDef",
+    {
+        "Id": str,
+        "Principal": DataLakePrincipalOutputTypeDef,
+        "Resource": ResourceOutputTypeDef,
+        "Permissions": List[PermissionType],
+        "PermissionsWithGrantOption": List[PermissionType],
+    },
+)
+
+PrincipalResourcePermissionsTypeDef = TypedDict(
+    "PrincipalResourcePermissionsTypeDef",
+    {
+        "Principal": DataLakePrincipalOutputTypeDef,
+        "Resource": ResourceOutputTypeDef,
+        "Permissions": List[PermissionType],
+        "PermissionsWithGrantOption": List[PermissionType],
+        "AdditionalDetails": DetailsMapTypeDef,
+    },
+)
+
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
         "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
@@ -1673,26 +1857,14 @@
         "NextToken": str,
         "MaxResults": int,
         "IncludeRelated": str,
     },
     total=False,
 )
 
-PrincipalResourcePermissionsTypeDef = TypedDict(
-    "PrincipalResourcePermissionsTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Resource": ResourceTypeDef,
-        "Permissions": List[PermissionType],
-        "PermissionsWithGrantOption": List[PermissionType],
-        "AdditionalDetails": DetailsMapTypeDef,
-    },
-    total=False,
-)
-
 _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
         "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
@@ -1728,14 +1900,40 @@
 )
 
 class RevokePermissionsRequestRequestTypeDef(
     _RequiredRevokePermissionsRequestRequestTypeDef, _OptionalRevokePermissionsRequestRequestTypeDef
 ):
     pass
 
+BatchPermissionsFailureEntryTypeDef = TypedDict(
+    "BatchPermissionsFailureEntryTypeDef",
+    {
+        "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
+        "Error": ErrorDetailTypeDef,
+    },
+)
+
+GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
+    "GetEffectivePermissionsForPathResponseTypeDef",
+    {
+        "Permissions": List[PrincipalResourcePermissionsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPermissionsResponseTypeDef = TypedDict(
+    "ListPermissionsResponseTypeDef",
+    {
+        "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
     {
         "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
@@ -1748,23 +1946,14 @@
 
 class BatchGrantPermissionsRequestRequestTypeDef(
     _RequiredBatchGrantPermissionsRequestRequestTypeDef,
     _OptionalBatchGrantPermissionsRequestRequestTypeDef,
 ):
     pass
 
-BatchPermissionsFailureEntryTypeDef = TypedDict(
-    "BatchPermissionsFailureEntryTypeDef",
-    {
-        "RequestEntry": BatchPermissionsRequestEntryTypeDef,
-        "Error": ErrorDetailTypeDef,
-    },
-    total=False,
-)
-
 _RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
     {
         "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
@@ -1777,40 +1966,22 @@
 
 class BatchRevokePermissionsRequestRequestTypeDef(
     _RequiredBatchRevokePermissionsRequestRequestTypeDef,
     _OptionalBatchRevokePermissionsRequestRequestTypeDef,
 ):
     pass
 
-GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
-    "GetEffectivePermissionsForPathResponseTypeDef",
-    {
-        "Permissions": List[PrincipalResourcePermissionsTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPermissionsResponseTypeDef = TypedDict(
-    "ListPermissionsResponseTypeDef",
-    {
-        "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchGrantPermissionsResponseTypeDef = TypedDict(
     "BatchGrantPermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchRevokePermissionsResponseTypeDef = TypedDict(
     "BatchRevokePermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation.egg-info/PKG-INFO` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.28.0
-Summary: Type annotations for boto3.LakeFormation 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.4
+Summary: Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,28 +352,34 @@
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
+    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
+    LFTagPairOutputTypeDef,
+    ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
+    RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
@@ -384,105 +390,116 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
-    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
-    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
     GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
+    LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
+    LFTagOutputTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     TableObjectTypeDef,
     QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartQueryPlanningResponseTypeDef,
+    TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
-    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    GetLFTagResponseTypeDef,
+    GetQueryStateResponseTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    StartQueryPlanningResponseTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
-    ColumnLFTagTypeDef,
-    ListLFTagsResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
-    LFTagErrorTypeDef,
+    PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    ColumnLFTagTypeDef,
+    LFTagErrorTypeDef,
+    ListLFTagsResponseTypeDef,
+    TableWithColumnsResourceOutputTypeDef,
     TableWithColumnsResourceTypeDef,
+    DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
     DeleteObjectsOnCancelRequestRequestTypeDef,
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
+    LFTagPolicyResourceOutputTypeDef,
     LFTagPolicyResourceTypeDef,
     SearchDatabasesByLFTagsRequestRequestTypeDef,
     SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
     SearchTablesByLFTagsRequestRequestTypeDef,
     SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
     StartQueryPlanningRequestRequestTypeDef,
+    DataLakeSettingsOutputTypeDef,
+    DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    DataLakeSettingsTypeDef,
-    CreateDataCellsFilterRequestRequestTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
+    CreateDataCellsFilterRequestRequestTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
     GetTableObjectsResponseTypeDef,
-    SearchTablesByLFTagsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
+    SearchTablesByLFTagsResponseTypeDef,
+    BatchPermissionsRequestEntryOutputTypeDef,
+    PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
-    PrincipalResourcePermissionsTypeDef,
     RemoveLFTagsFromResourceRequestRequestTypeDef,
     RevokePermissionsRequestRequestTypeDef,
-    BatchGrantPermissionsRequestRequestTypeDef,
     BatchPermissionsFailureEntryTypeDef,
-    BatchRevokePermissionsRequestRequestTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     ListPermissionsResponseTypeDef,
+    BatchGrantPermissionsRequestRequestTypeDef,
+    BatchRevokePermissionsRequestRequestTypeDef,
     BatchGrantPermissionsResponseTypeDef,
     BatchRevokePermissionsResponseTypeDef,
 )
 
 
 def get_structure() -> LFTagPairTypeDef:
     return {...}
```

### Comparing `mypy-boto3-lakeformation-1.28.0/mypy_boto3_lakeformation.egg-info/SOURCES.txt` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.0/setup.py` & `mypy-boto3-lakeformation-1.28.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lakeformation",
-    version="1.28.0",
+    version="1.28.4",
     packages=["mypy_boto3_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LakeFormation 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

