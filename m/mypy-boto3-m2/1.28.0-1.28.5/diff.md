# Comparing `tmp/mypy-boto3-m2-1.28.0.tar.gz` & `tmp/mypy-boto3-m2-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-m2-1.28.0.tar", last modified: Thu Jul  6 21:00:01 2023, max compression
+gzip compressed data, was "mypy-boto3-m2-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-m2-1.28.0.tar` & `mypy-boto3-m2-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.762359 mypy-boto3-m2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:16.000000 mypy-boto3-m2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-07-06 21:00:01.762359 mypy-boto3-m2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16992 2023-07-06 20:46:16.000000 mypy-boto3-m2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.754358 mypy-boto3-m2-1.28.0/mypy_boto3_m2/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-06 20:46:17.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-06 20:46:16.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:46:17.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27363 2023-07-06 20:46:19.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27315 2023-07-06 20:46:19.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-07-06 20:46:19.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-06 20:46:19.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-06 20:46:19.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-06 20:46:19.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:17.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42321 2023-07-06 20:46:20.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42253 2023-07-06 20:46:20.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:16.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.762359 mypy-boto3-m2-1.28.0/mypy_boto3_m2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-07-06 21:00:01.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 21:00:01.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:01.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:01.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:01.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 21:00:01.000000 mypy-boto3-m2-1.28.0/mypy_boto3_m2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:01.762359 mypy-boto3-m2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-06 20:46:16.000000 mypy-boto3-m2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/mypy_boto3_m2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27910 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42524 2023-07-18 19:32:27.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42470 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-18 19:32:24.000000 mypy-boto3-m2-1.28.5/setup.py
```

### Comparing `mypy-boto3-m2-1.28.0/LICENSE` & `mypy-boto3-m2-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.0/PKG-INFO` & `mypy-boto3-m2-1.28.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.28.0
-Summary: Type annotations for boto3.MainframeModernization 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.5
+Summary: Type annotations for boto3.MainframeModernization 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,19 +362,22 @@
 ### Typed dictionaries
 
 `mypy_boto3_m2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_m2.type_defs import (
+    AlternateKeyOutputTypeDef,
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
+    FileBatchJobIdentifierOutputTypeDef,
+    ScriptBatchJobIdentifierOutputTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
     CreateApplicationResponseTypeDef,
     CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
@@ -392,28 +395,32 @@
     PoAttributesTypeDef,
     PsAttributesTypeDef,
     DeleteApplicationFromEnvironmentRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeployedVersionSummaryTypeDef,
     DeploymentSummaryTypeDef,
+    EfsStorageConfigurationOutputTypeDef,
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
+    FsxStorageConfigurationOutputTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
     GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
+    HighAvailabilityConfigOutputTypeDef,
+    GetSignedBluinsightsUrlResponseTypeDef,
     ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
     ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
@@ -428,60 +435,63 @@
     ListEngineVersionsRequestRequestTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
     PaginatorConfigTypeDef,
+    PrimaryKeyOutputTypeDef,
     PrimaryKeyTypeDef,
     ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
     StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
+    BatchJobIdentifierOutputTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
+    StorageConfigurationOutputTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
     PendingMaintenanceTypeDef,
-    VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
+    VsamAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
-    DatasetOrgAttributesTypeDef,
     DatasetDetailOrgAttributesTypeDef,
+    DatasetOrgAttributesTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
-    DataSetTypeDef,
     GetDataSetDetailsResponseTypeDef,
+    DataSetTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AlternateKeyTypeDef:
+def get_structure() -> AlternateKeyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-m2-1.28.0/README.md` & `mypy-boto3-m2-1.28.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,19 +330,22 @@
 ### Typed dictionaries
 
 `mypy_boto3_m2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_m2.type_defs import (
+    AlternateKeyOutputTypeDef,
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
+    FileBatchJobIdentifierOutputTypeDef,
+    ScriptBatchJobIdentifierOutputTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
     CreateApplicationResponseTypeDef,
     CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
@@ -360,28 +363,32 @@
     PoAttributesTypeDef,
     PsAttributesTypeDef,
     DeleteApplicationFromEnvironmentRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeployedVersionSummaryTypeDef,
     DeploymentSummaryTypeDef,
+    EfsStorageConfigurationOutputTypeDef,
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
+    FsxStorageConfigurationOutputTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
     GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
+    HighAvailabilityConfigOutputTypeDef,
+    GetSignedBluinsightsUrlResponseTypeDef,
     ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
     ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
@@ -396,60 +403,63 @@
     ListEngineVersionsRequestRequestTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
     PaginatorConfigTypeDef,
+    PrimaryKeyOutputTypeDef,
     PrimaryKeyTypeDef,
     ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
     StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
+    BatchJobIdentifierOutputTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
+    StorageConfigurationOutputTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
     PendingMaintenanceTypeDef,
-    VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
+    VsamAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
-    DatasetOrgAttributesTypeDef,
     DatasetDetailOrgAttributesTypeDef,
+    DatasetOrgAttributesTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
-    DataSetTypeDef,
     GetDataSetDetailsResponseTypeDef,
+    DataSetTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AlternateKeyTypeDef:
+def get_structure() -> AlternateKeyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/__init__.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/__init__.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/__main__.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MainframeModernization 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MainframeModernization 1.28.5\nVersion:         1.28.5\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/client.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     GetApplicationResponseTypeDef,
     GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     GetDataSetDetailsResponseTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     GetDeploymentResponseTypeDef,
     GetEnvironmentResponseTypeDef,
+    GetSignedBluinsightsUrlResponseTypeDef,
     HighAvailabilityConfigTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     ListDataSetsResponseTypeDef,
@@ -310,14 +311,22 @@
         """
         Describes a specific runtime environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#get_environment)
         """
 
+    def get_signed_bluinsights_url(self) -> GetSignedBluinsightsUrlResponseTypeDef:
+        """
+        Gets a single sign-on URL that can be used to connect to AWS Blu Insights.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_signed_bluinsights_url)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#get_signed_bluinsights_url)
+        """
+
     def list_application_versions(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListApplicationVersionsResponseTypeDef:
         """
         Returns a list of the application versions for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_application_versions)
```

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/client.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     GetApplicationResponseTypeDef,
     GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     GetDataSetDetailsResponseTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     GetDeploymentResponseTypeDef,
     GetEnvironmentResponseTypeDef,
+    GetSignedBluinsightsUrlResponseTypeDef,
     HighAvailabilityConfigTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     ListDataSetsResponseTypeDef,
@@ -287,14 +288,21 @@
     def get_environment(self, *, environmentId: str) -> GetEnvironmentResponseTypeDef:
         """
         Describes a specific runtime environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#get_environment)
         """
+    def get_signed_bluinsights_url(self) -> GetSignedBluinsightsUrlResponseTypeDef:
+        """
+        Gets a single sign-on URL that can be used to connect to AWS Blu Insights.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_signed_bluinsights_url)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/client/#get_signed_bluinsights_url)
+        """
     def list_application_versions(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListApplicationVersionsResponseTypeDef:
         """
         Returns a list of the application versions for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_application_versions)
```

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/literals.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/literals.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/paginator.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/paginator.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/type_defs.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for m2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_m2.type_defs import AlternateKeyTypeDef
+    from mypy_boto3_m2.type_defs import AlternateKeyOutputTypeDef
 
-    data: AlternateKeyTypeDef = {...}
+    data: AlternateKeyOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -30,19 +30,22 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AlternateKeyOutputTypeDef",
     "AlternateKeyTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
+    "FileBatchJobIdentifierOutputTypeDef",
+    "ScriptBatchJobIdentifierOutputTypeDef",
     "FileBatchJobIdentifierTypeDef",
     "ScriptBatchJobIdentifierTypeDef",
     "CancelBatchJobExecutionRequestRequestTypeDef",
     "DefinitionTypeDef",
     "CreateApplicationResponseTypeDef",
     "CreateDataSetImportTaskResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
@@ -60,28 +63,32 @@
     "PoAttributesTypeDef",
     "PsAttributesTypeDef",
     "DeleteApplicationFromEnvironmentRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeployedVersionSummaryTypeDef",
     "DeploymentSummaryTypeDef",
+    "EfsStorageConfigurationOutputTypeDef",
     "EfsStorageConfigurationTypeDef",
     "EngineVersionsSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
+    "FsxStorageConfigurationOutputTypeDef",
     "FsxStorageConfigurationTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "LogGroupSummaryTypeDef",
     "GetApplicationVersionRequestRequestTypeDef",
     "GetApplicationVersionResponseTypeDef",
     "GetBatchJobExecutionRequestRequestTypeDef",
     "GetDataSetDetailsRequestRequestTypeDef",
     "GetDataSetImportTaskRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetDeploymentResponseTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
+    "HighAvailabilityConfigOutputTypeDef",
+    "GetSignedBluinsightsUrlResponseTypeDef",
     "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
     "ListBatchJobDefinitionsRequestRequestTypeDef",
     "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
@@ -96,58 +103,71 @@
     "ListEngineVersionsRequestRequestTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "MaintenanceScheduleTypeDef",
     "PaginatorConfigTypeDef",
+    "PrimaryKeyOutputTypeDef",
     "PrimaryKeyTypeDef",
     "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "StartBatchJobResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "BatchJobDefinitionTypeDef",
+    "BatchJobIdentifierOutputTypeDef",
     "BatchJobIdentifierTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "DataSetImportTaskTypeDef",
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
     "ListEngineVersionsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
+    "StorageConfigurationOutputTypeDef",
     "StorageConfigurationTypeDef",
     "GetApplicationResponseTypeDef",
     "PendingMaintenanceTypeDef",
-    "VsamAttributesTypeDef",
     "VsamDetailAttributesTypeDef",
+    "VsamAttributesTypeDef",
     "ListBatchJobDefinitionsResponseTypeDef",
     "BatchJobExecutionSummaryTypeDef",
     "GetBatchJobExecutionResponseTypeDef",
     "StartBatchJobRequestRequestTypeDef",
     "ListDataSetImportHistoryResponseTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "GetEnvironmentResponseTypeDef",
-    "DatasetOrgAttributesTypeDef",
     "DatasetDetailOrgAttributesTypeDef",
+    "DatasetOrgAttributesTypeDef",
     "ListBatchJobExecutionsResponseTypeDef",
-    "DataSetTypeDef",
     "GetDataSetDetailsResponseTypeDef",
+    "DataSetTypeDef",
     "DataSetImportItemTypeDef",
     "DataSetImportConfigTypeDef",
     "CreateDataSetImportTaskRequestRequestTypeDef",
 )
 
+AlternateKeyOutputTypeDef = TypedDict(
+    "AlternateKeyOutputTypeDef",
+    {
+        "allowDuplicates": bool,
+        "length": int,
+        "name": str,
+        "offset": int,
+    },
+)
+
 _RequiredAlternateKeyTypeDef = TypedDict(
     "_RequiredAlternateKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -161,92 +181,68 @@
 )
 
 
 class AlternateKeyTypeDef(_RequiredAlternateKeyTypeDef, _OptionalAlternateKeyTypeDef):
     pass
 
 
-_RequiredApplicationSummaryTypeDef = TypedDict(
-    "_RequiredApplicationSummaryTypeDef",
+ApplicationSummaryTypeDef = TypedDict(
+    "ApplicationSummaryTypeDef",
     {
         "applicationArn": str,
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
-        "engineType": EngineTypeType,
-        "name": str,
-        "status": ApplicationLifecycleType,
-    },
-)
-_OptionalApplicationSummaryTypeDef = TypedDict(
-    "_OptionalApplicationSummaryTypeDef",
-    {
         "deploymentStatus": ApplicationDeploymentLifecycleType,
         "description": str,
+        "engineType": EngineTypeType,
         "environmentId": str,
         "lastStartTime": datetime,
+        "name": str,
         "roleArn": str,
+        "status": ApplicationLifecycleType,
         "versionStatus": ApplicationVersionLifecycleType,
     },
-    total=False,
 )
 
-
-class ApplicationSummaryTypeDef(
-    _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
-):
-    pass
-
-
-_RequiredApplicationVersionSummaryTypeDef = TypedDict(
-    "_RequiredApplicationVersionSummaryTypeDef",
+ApplicationVersionSummaryTypeDef = TypedDict(
+    "ApplicationVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "creationTime": datetime,
         "status": ApplicationVersionLifecycleType,
+        "statusReason": str,
     },
 )
-_OptionalApplicationVersionSummaryTypeDef = TypedDict(
-    "_OptionalApplicationVersionSummaryTypeDef",
+
+FileBatchJobDefinitionTypeDef = TypedDict(
+    "FileBatchJobDefinitionTypeDef",
     {
-        "statusReason": str,
+        "fileName": str,
+        "folderPath": str,
     },
-    total=False,
 )
 
-
-class ApplicationVersionSummaryTypeDef(
-    _RequiredApplicationVersionSummaryTypeDef, _OptionalApplicationVersionSummaryTypeDef
-):
-    pass
-
-
-_RequiredFileBatchJobDefinitionTypeDef = TypedDict(
-    "_RequiredFileBatchJobDefinitionTypeDef",
+ScriptBatchJobDefinitionTypeDef = TypedDict(
+    "ScriptBatchJobDefinitionTypeDef",
     {
-        "fileName": str,
+        "scriptName": str,
     },
 )
-_OptionalFileBatchJobDefinitionTypeDef = TypedDict(
-    "_OptionalFileBatchJobDefinitionTypeDef",
+
+FileBatchJobIdentifierOutputTypeDef = TypedDict(
+    "FileBatchJobIdentifierOutputTypeDef",
     {
+        "fileName": str,
         "folderPath": str,
     },
-    total=False,
 )
 
-
-class FileBatchJobDefinitionTypeDef(
-    _RequiredFileBatchJobDefinitionTypeDef, _OptionalFileBatchJobDefinitionTypeDef
-):
-    pass
-
-
-ScriptBatchJobDefinitionTypeDef = TypedDict(
-    "ScriptBatchJobDefinitionTypeDef",
+ScriptBatchJobIdentifierOutputTypeDef = TypedDict(
+    "ScriptBatchJobIdentifierOutputTypeDef",
     {
         "scriptName": str,
     },
 )
 
 _RequiredFileBatchJobIdentifierTypeDef = TypedDict(
     "_RequiredFileBatchJobIdentifierTypeDef",
@@ -372,52 +368,40 @@
         "inProgress": int,
         "pending": int,
         "succeeded": int,
         "total": int,
     },
 )
 
-_RequiredDataSetSummaryTypeDef = TypedDict(
-    "_RequiredDataSetSummaryTypeDef",
-    {
-        "dataSetName": str,
-    },
-)
-_OptionalDataSetSummaryTypeDef = TypedDict(
-    "_OptionalDataSetSummaryTypeDef",
+DataSetSummaryTypeDef = TypedDict(
+    "DataSetSummaryTypeDef",
     {
         "creationTime": datetime,
+        "dataSetName": str,
         "dataSetOrg": str,
         "format": str,
         "lastReferencedTime": datetime,
         "lastUpdatedTime": datetime,
     },
-    total=False,
 )
 
-
-class DataSetSummaryTypeDef(_RequiredDataSetSummaryTypeDef, _OptionalDataSetSummaryTypeDef):
-    pass
-
-
 RecordLengthTypeDef = TypedDict(
     "RecordLengthTypeDef",
     {
         "max": int,
         "min": int,
     },
 )
 
 GdgDetailAttributesTypeDef = TypedDict(
     "GdgDetailAttributesTypeDef",
     {
         "limit": int,
         "rollDisposition": str,
     },
-    total=False,
 )
 
 PoDetailAttributesTypeDef = TypedDict(
     "PoDetailAttributesTypeDef",
     {
         "encoding": str,
         "format": str,
@@ -498,62 +482,44 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-_RequiredDeployedVersionSummaryTypeDef = TypedDict(
-    "_RequiredDeployedVersionSummaryTypeDef",
+DeployedVersionSummaryTypeDef = TypedDict(
+    "DeployedVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "status": DeploymentLifecycleType,
-    },
-)
-_OptionalDeployedVersionSummaryTypeDef = TypedDict(
-    "_OptionalDeployedVersionSummaryTypeDef",
-    {
         "statusReason": str,
     },
-    total=False,
 )
 
-
-class DeployedVersionSummaryTypeDef(
-    _RequiredDeployedVersionSummaryTypeDef, _OptionalDeployedVersionSummaryTypeDef
-):
-    pass
-
-
-_RequiredDeploymentSummaryTypeDef = TypedDict(
-    "_RequiredDeploymentSummaryTypeDef",
+DeploymentSummaryTypeDef = TypedDict(
+    "DeploymentSummaryTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
         "deploymentId": str,
         "environmentId": str,
         "status": DeploymentLifecycleType,
+        "statusReason": str,
     },
 )
-_OptionalDeploymentSummaryTypeDef = TypedDict(
-    "_OptionalDeploymentSummaryTypeDef",
+
+EfsStorageConfigurationOutputTypeDef = TypedDict(
+    "EfsStorageConfigurationOutputTypeDef",
     {
-        "statusReason": str,
+        "fileSystemId": str,
+        "mountPoint": str,
     },
-    total=False,
 )
 
-
-class DeploymentSummaryTypeDef(
-    _RequiredDeploymentSummaryTypeDef, _OptionalDeploymentSummaryTypeDef
-):
-    pass
-
-
 EfsStorageConfigurationTypeDef = TypedDict(
     "EfsStorageConfigurationTypeDef",
     {
         "fileSystemId": str,
         "mountPoint": str,
     },
 )
@@ -576,14 +542,22 @@
         "environmentId": str,
         "instanceType": str,
         "name": str,
         "status": EnvironmentLifecycleType,
     },
 )
 
+FsxStorageConfigurationOutputTypeDef = TypedDict(
+    "FsxStorageConfigurationOutputTypeDef",
+    {
+        "fileSystemId": str,
+        "mountPoint": str,
+    },
+)
+
 FsxStorageConfigurationTypeDef = TypedDict(
     "FsxStorageConfigurationTypeDef",
     {
         "fileSystemId": str,
         "mountPoint": str,
     },
 )
@@ -674,14 +648,29 @@
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
+HighAvailabilityConfigOutputTypeDef = TypedDict(
+    "HighAvailabilityConfigOutputTypeDef",
+    {
+        "desiredCapacity": int,
+    },
+)
+
+GetSignedBluinsightsUrlResponseTypeDef = TypedDict(
+    "GetSignedBluinsightsUrlResponseTypeDef",
+    {
+        "signedBiUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
@@ -1038,27 +1027,35 @@
 
 MaintenanceScheduleTypeDef = TypedDict(
     "MaintenanceScheduleTypeDef",
     {
         "endTime": datetime,
         "startTime": datetime,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PrimaryKeyOutputTypeDef = TypedDict(
+    "PrimaryKeyOutputTypeDef",
+    {
+        "length": int,
+        "name": str,
+        "offset": int,
+    },
+)
+
 _RequiredPrimaryKeyTypeDef = TypedDict(
     "_RequiredPrimaryKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -1199,15 +1196,22 @@
 
 BatchJobDefinitionTypeDef = TypedDict(
     "BatchJobDefinitionTypeDef",
     {
         "fileBatchJobDefinition": FileBatchJobDefinitionTypeDef,
         "scriptBatchJobDefinition": ScriptBatchJobDefinitionTypeDef,
     },
-    total=False,
+)
+
+BatchJobIdentifierOutputTypeDef = TypedDict(
+    "BatchJobIdentifierOutputTypeDef",
+    {
+        "fileBatchJobIdentifier": FileBatchJobIdentifierOutputTypeDef,
+        "scriptBatchJobIdentifier": ScriptBatchJobIdentifierOutputTypeDef,
+    },
 )
 
 BatchJobIdentifierTypeDef = TypedDict(
     "BatchJobIdentifierTypeDef",
     {
         "fileBatchJobIdentifier": FileBatchJobIdentifierTypeDef,
         "scriptBatchJobIdentifier": ScriptBatchJobIdentifierTypeDef,
@@ -1316,14 +1320,22 @@
     {
         "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StorageConfigurationOutputTypeDef = TypedDict(
+    "StorageConfigurationOutputTypeDef",
+    {
+        "efs": EfsStorageConfigurationOutputTypeDef,
+        "fsx": FsxStorageConfigurationOutputTypeDef,
+    },
+)
+
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "efs": EfsStorageConfigurationTypeDef,
         "fsx": FsxStorageConfigurationTypeDef,
     },
     total=False,
@@ -1358,15 +1370,26 @@
 
 PendingMaintenanceTypeDef = TypedDict(
     "PendingMaintenanceTypeDef",
     {
         "engineVersion": str,
         "schedule": MaintenanceScheduleTypeDef,
     },
-    total=False,
+)
+
+VsamDetailAttributesTypeDef = TypedDict(
+    "VsamDetailAttributesTypeDef",
+    {
+        "alternateKeys": List[AlternateKeyOutputTypeDef],
+        "cacheAtStartup": bool,
+        "compressed": bool,
+        "encoding": str,
+        "primaryKey": PrimaryKeyOutputTypeDef,
+        "recordFormat": str,
+    },
 )
 
 _RequiredVsamAttributesTypeDef = TypedDict(
     "_RequiredVsamAttributesTypeDef",
     {
         "format": str,
     },
@@ -1383,70 +1406,44 @@
 )
 
 
 class VsamAttributesTypeDef(_RequiredVsamAttributesTypeDef, _OptionalVsamAttributesTypeDef):
     pass
 
 
-VsamDetailAttributesTypeDef = TypedDict(
-    "VsamDetailAttributesTypeDef",
-    {
-        "alternateKeys": List[AlternateKeyTypeDef],
-        "cacheAtStartup": bool,
-        "compressed": bool,
-        "encoding": str,
-        "primaryKey": PrimaryKeyTypeDef,
-        "recordFormat": str,
-    },
-    total=False,
-)
-
 ListBatchJobDefinitionsResponseTypeDef = TypedDict(
     "ListBatchJobDefinitionsResponseTypeDef",
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_RequiredBatchJobExecutionSummaryTypeDef",
+BatchJobExecutionSummaryTypeDef = TypedDict(
+    "BatchJobExecutionSummaryTypeDef",
     {
         "applicationId": str,
-        "executionId": str,
-        "startTime": datetime,
-        "status": BatchJobExecutionStatusType,
-    },
-)
-_OptionalBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_OptionalBatchJobExecutionSummaryTypeDef",
-    {
-        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
+        "executionId": str,
         "jobId": str,
         "jobName": str,
         "jobType": BatchJobTypeType,
         "returnCode": str,
+        "startTime": datetime,
+        "status": BatchJobExecutionStatusType,
     },
-    total=False,
 )
 
-
-class BatchJobExecutionSummaryTypeDef(
-    _RequiredBatchJobExecutionSummaryTypeDef, _OptionalBatchJobExecutionSummaryTypeDef
-):
-    pass
-
-
 GetBatchJobExecutionResponseTypeDef = TypedDict(
     "GetBatchJobExecutionResponseTypeDef",
     {
         "applicationId": str,
-        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
         "executionId": str,
         "jobId": str,
         "jobName": str,
         "jobType": BatchJobTypeType,
         "jobUser": str,
         "returnCode": str,
@@ -1527,64 +1524,78 @@
         "actualCapacity": int,
         "creationTime": datetime,
         "description": str,
         "engineType": EngineTypeType,
         "engineVersion": str,
         "environmentArn": str,
         "environmentId": str,
-        "highAvailabilityConfig": HighAvailabilityConfigTypeDef,
+        "highAvailabilityConfig": HighAvailabilityConfigOutputTypeDef,
         "instanceType": str,
         "kmsKeyId": str,
         "loadBalancerArn": str,
         "name": str,
         "pendingMaintenance": PendingMaintenanceTypeDef,
         "preferredMaintenanceWindow": str,
         "publiclyAccessible": bool,
         "securityGroupIds": List[str],
         "status": EnvironmentLifecycleType,
         "statusReason": str,
-        "storageConfigurations": List[StorageConfigurationTypeDef],
+        "storageConfigurations": List[StorageConfigurationOutputTypeDef],
         "subnetIds": List[str],
         "tags": Dict[str, str],
         "vpcId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatasetOrgAttributesTypeDef = TypedDict(
-    "DatasetOrgAttributesTypeDef",
-    {
-        "gdg": GdgAttributesTypeDef,
-        "po": PoAttributesTypeDef,
-        "ps": PsAttributesTypeDef,
-        "vsam": VsamAttributesTypeDef,
-    },
-    total=False,
-)
-
 DatasetDetailOrgAttributesTypeDef = TypedDict(
     "DatasetDetailOrgAttributesTypeDef",
     {
         "gdg": GdgDetailAttributesTypeDef,
         "po": PoDetailAttributesTypeDef,
         "ps": PsDetailAttributesTypeDef,
         "vsam": VsamDetailAttributesTypeDef,
     },
+)
+
+DatasetOrgAttributesTypeDef = TypedDict(
+    "DatasetOrgAttributesTypeDef",
+    {
+        "gdg": GdgAttributesTypeDef,
+        "po": PoAttributesTypeDef,
+        "ps": PsAttributesTypeDef,
+        "vsam": VsamAttributesTypeDef,
+    },
     total=False,
 )
 
 ListBatchJobExecutionsResponseTypeDef = TypedDict(
     "ListBatchJobExecutionsResponseTypeDef",
     {
         "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GetDataSetDetailsResponseTypeDef = TypedDict(
+    "GetDataSetDetailsResponseTypeDef",
+    {
+        "blocksize": int,
+        "creationTime": datetime,
+        "dataSetName": str,
+        "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
+        "lastReferencedTime": datetime,
+        "lastUpdatedTime": datetime,
+        "location": str,
+        "recordLength": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDataSetTypeDef = TypedDict(
     "_RequiredDataSetTypeDef",
     {
         "datasetName": str,
         "datasetOrg": DatasetOrgAttributesTypeDef,
         "recordLength": RecordLengthTypeDef,
     },
@@ -1599,29 +1610,14 @@
 )
 
 
 class DataSetTypeDef(_RequiredDataSetTypeDef, _OptionalDataSetTypeDef):
     pass
 
 
-GetDataSetDetailsResponseTypeDef = TypedDict(
-    "GetDataSetDetailsResponseTypeDef",
-    {
-        "blocksize": int,
-        "creationTime": datetime,
-        "dataSetName": str,
-        "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
-        "lastReferencedTime": datetime,
-        "lastUpdatedTime": datetime,
-        "location": str,
-        "recordLength": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataSetImportItemTypeDef = TypedDict(
     "DataSetImportItemTypeDef",
     {
         "dataSet": DataSetTypeDef,
         "externalLocation": ExternalLocationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2/type_defs.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for m2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_m2.type_defs import AlternateKeyTypeDef
+    from mypy_boto3_m2.type_defs import AlternateKeyOutputTypeDef
 
-    data: AlternateKeyTypeDef = {...}
+    data: AlternateKeyOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -29,19 +29,22 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AlternateKeyOutputTypeDef",
     "AlternateKeyTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
+    "FileBatchJobIdentifierOutputTypeDef",
+    "ScriptBatchJobIdentifierOutputTypeDef",
     "FileBatchJobIdentifierTypeDef",
     "ScriptBatchJobIdentifierTypeDef",
     "CancelBatchJobExecutionRequestRequestTypeDef",
     "DefinitionTypeDef",
     "CreateApplicationResponseTypeDef",
     "CreateDataSetImportTaskResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
@@ -59,28 +62,32 @@
     "PoAttributesTypeDef",
     "PsAttributesTypeDef",
     "DeleteApplicationFromEnvironmentRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeployedVersionSummaryTypeDef",
     "DeploymentSummaryTypeDef",
+    "EfsStorageConfigurationOutputTypeDef",
     "EfsStorageConfigurationTypeDef",
     "EngineVersionsSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
+    "FsxStorageConfigurationOutputTypeDef",
     "FsxStorageConfigurationTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "LogGroupSummaryTypeDef",
     "GetApplicationVersionRequestRequestTypeDef",
     "GetApplicationVersionResponseTypeDef",
     "GetBatchJobExecutionRequestRequestTypeDef",
     "GetDataSetDetailsRequestRequestTypeDef",
     "GetDataSetImportTaskRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetDeploymentResponseTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
+    "HighAvailabilityConfigOutputTypeDef",
+    "GetSignedBluinsightsUrlResponseTypeDef",
     "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
     "ListBatchJobDefinitionsRequestRequestTypeDef",
     "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
@@ -95,58 +102,71 @@
     "ListEngineVersionsRequestRequestTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "MaintenanceScheduleTypeDef",
     "PaginatorConfigTypeDef",
+    "PrimaryKeyOutputTypeDef",
     "PrimaryKeyTypeDef",
     "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "StartBatchJobResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "BatchJobDefinitionTypeDef",
+    "BatchJobIdentifierOutputTypeDef",
     "BatchJobIdentifierTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "DataSetImportTaskTypeDef",
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
     "ListEngineVersionsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
+    "StorageConfigurationOutputTypeDef",
     "StorageConfigurationTypeDef",
     "GetApplicationResponseTypeDef",
     "PendingMaintenanceTypeDef",
-    "VsamAttributesTypeDef",
     "VsamDetailAttributesTypeDef",
+    "VsamAttributesTypeDef",
     "ListBatchJobDefinitionsResponseTypeDef",
     "BatchJobExecutionSummaryTypeDef",
     "GetBatchJobExecutionResponseTypeDef",
     "StartBatchJobRequestRequestTypeDef",
     "ListDataSetImportHistoryResponseTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "GetEnvironmentResponseTypeDef",
-    "DatasetOrgAttributesTypeDef",
     "DatasetDetailOrgAttributesTypeDef",
+    "DatasetOrgAttributesTypeDef",
     "ListBatchJobExecutionsResponseTypeDef",
-    "DataSetTypeDef",
     "GetDataSetDetailsResponseTypeDef",
+    "DataSetTypeDef",
     "DataSetImportItemTypeDef",
     "DataSetImportConfigTypeDef",
     "CreateDataSetImportTaskRequestRequestTypeDef",
 )
 
+AlternateKeyOutputTypeDef = TypedDict(
+    "AlternateKeyOutputTypeDef",
+    {
+        "allowDuplicates": bool,
+        "length": int,
+        "name": str,
+        "offset": int,
+    },
+)
+
 _RequiredAlternateKeyTypeDef = TypedDict(
     "_RequiredAlternateKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -158,86 +178,68 @@
     },
     total=False,
 )
 
 class AlternateKeyTypeDef(_RequiredAlternateKeyTypeDef, _OptionalAlternateKeyTypeDef):
     pass
 
-_RequiredApplicationSummaryTypeDef = TypedDict(
-    "_RequiredApplicationSummaryTypeDef",
+ApplicationSummaryTypeDef = TypedDict(
+    "ApplicationSummaryTypeDef",
     {
         "applicationArn": str,
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
-        "engineType": EngineTypeType,
-        "name": str,
-        "status": ApplicationLifecycleType,
-    },
-)
-_OptionalApplicationSummaryTypeDef = TypedDict(
-    "_OptionalApplicationSummaryTypeDef",
-    {
         "deploymentStatus": ApplicationDeploymentLifecycleType,
         "description": str,
+        "engineType": EngineTypeType,
         "environmentId": str,
         "lastStartTime": datetime,
+        "name": str,
         "roleArn": str,
+        "status": ApplicationLifecycleType,
         "versionStatus": ApplicationVersionLifecycleType,
     },
-    total=False,
 )
 
-class ApplicationSummaryTypeDef(
-    _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
-):
-    pass
-
-_RequiredApplicationVersionSummaryTypeDef = TypedDict(
-    "_RequiredApplicationVersionSummaryTypeDef",
+ApplicationVersionSummaryTypeDef = TypedDict(
+    "ApplicationVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "creationTime": datetime,
         "status": ApplicationVersionLifecycleType,
+        "statusReason": str,
     },
 )
-_OptionalApplicationVersionSummaryTypeDef = TypedDict(
-    "_OptionalApplicationVersionSummaryTypeDef",
+
+FileBatchJobDefinitionTypeDef = TypedDict(
+    "FileBatchJobDefinitionTypeDef",
     {
-        "statusReason": str,
+        "fileName": str,
+        "folderPath": str,
     },
-    total=False,
 )
 
-class ApplicationVersionSummaryTypeDef(
-    _RequiredApplicationVersionSummaryTypeDef, _OptionalApplicationVersionSummaryTypeDef
-):
-    pass
-
-_RequiredFileBatchJobDefinitionTypeDef = TypedDict(
-    "_RequiredFileBatchJobDefinitionTypeDef",
+ScriptBatchJobDefinitionTypeDef = TypedDict(
+    "ScriptBatchJobDefinitionTypeDef",
     {
-        "fileName": str,
+        "scriptName": str,
     },
 )
-_OptionalFileBatchJobDefinitionTypeDef = TypedDict(
-    "_OptionalFileBatchJobDefinitionTypeDef",
+
+FileBatchJobIdentifierOutputTypeDef = TypedDict(
+    "FileBatchJobIdentifierOutputTypeDef",
     {
+        "fileName": str,
         "folderPath": str,
     },
-    total=False,
 )
 
-class FileBatchJobDefinitionTypeDef(
-    _RequiredFileBatchJobDefinitionTypeDef, _OptionalFileBatchJobDefinitionTypeDef
-):
-    pass
-
-ScriptBatchJobDefinitionTypeDef = TypedDict(
-    "ScriptBatchJobDefinitionTypeDef",
+ScriptBatchJobIdentifierOutputTypeDef = TypedDict(
+    "ScriptBatchJobIdentifierOutputTypeDef",
     {
         "scriptName": str,
     },
 )
 
 _RequiredFileBatchJobIdentifierTypeDef = TypedDict(
     "_RequiredFileBatchJobIdentifierTypeDef",
@@ -359,50 +361,40 @@
         "inProgress": int,
         "pending": int,
         "succeeded": int,
         "total": int,
     },
 )
 
-_RequiredDataSetSummaryTypeDef = TypedDict(
-    "_RequiredDataSetSummaryTypeDef",
-    {
-        "dataSetName": str,
-    },
-)
-_OptionalDataSetSummaryTypeDef = TypedDict(
-    "_OptionalDataSetSummaryTypeDef",
+DataSetSummaryTypeDef = TypedDict(
+    "DataSetSummaryTypeDef",
     {
         "creationTime": datetime,
+        "dataSetName": str,
         "dataSetOrg": str,
         "format": str,
         "lastReferencedTime": datetime,
         "lastUpdatedTime": datetime,
     },
-    total=False,
 )
 
-class DataSetSummaryTypeDef(_RequiredDataSetSummaryTypeDef, _OptionalDataSetSummaryTypeDef):
-    pass
-
 RecordLengthTypeDef = TypedDict(
     "RecordLengthTypeDef",
     {
         "max": int,
         "min": int,
     },
 )
 
 GdgDetailAttributesTypeDef = TypedDict(
     "GdgDetailAttributesTypeDef",
     {
         "limit": int,
         "rollDisposition": str,
     },
-    total=False,
 )
 
 PoDetailAttributesTypeDef = TypedDict(
     "PoDetailAttributesTypeDef",
     {
         "encoding": str,
         "format": str,
@@ -479,58 +471,44 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-_RequiredDeployedVersionSummaryTypeDef = TypedDict(
-    "_RequiredDeployedVersionSummaryTypeDef",
+DeployedVersionSummaryTypeDef = TypedDict(
+    "DeployedVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "status": DeploymentLifecycleType,
-    },
-)
-_OptionalDeployedVersionSummaryTypeDef = TypedDict(
-    "_OptionalDeployedVersionSummaryTypeDef",
-    {
         "statusReason": str,
     },
-    total=False,
 )
 
-class DeployedVersionSummaryTypeDef(
-    _RequiredDeployedVersionSummaryTypeDef, _OptionalDeployedVersionSummaryTypeDef
-):
-    pass
-
-_RequiredDeploymentSummaryTypeDef = TypedDict(
-    "_RequiredDeploymentSummaryTypeDef",
+DeploymentSummaryTypeDef = TypedDict(
+    "DeploymentSummaryTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
         "deploymentId": str,
         "environmentId": str,
         "status": DeploymentLifecycleType,
+        "statusReason": str,
     },
 )
-_OptionalDeploymentSummaryTypeDef = TypedDict(
-    "_OptionalDeploymentSummaryTypeDef",
+
+EfsStorageConfigurationOutputTypeDef = TypedDict(
+    "EfsStorageConfigurationOutputTypeDef",
     {
-        "statusReason": str,
+        "fileSystemId": str,
+        "mountPoint": str,
     },
-    total=False,
 )
 
-class DeploymentSummaryTypeDef(
-    _RequiredDeploymentSummaryTypeDef, _OptionalDeploymentSummaryTypeDef
-):
-    pass
-
 EfsStorageConfigurationTypeDef = TypedDict(
     "EfsStorageConfigurationTypeDef",
     {
         "fileSystemId": str,
         "mountPoint": str,
     },
 )
@@ -553,14 +531,22 @@
         "environmentId": str,
         "instanceType": str,
         "name": str,
         "status": EnvironmentLifecycleType,
     },
 )
 
+FsxStorageConfigurationOutputTypeDef = TypedDict(
+    "FsxStorageConfigurationOutputTypeDef",
+    {
+        "fileSystemId": str,
+        "mountPoint": str,
+    },
+)
+
 FsxStorageConfigurationTypeDef = TypedDict(
     "FsxStorageConfigurationTypeDef",
     {
         "fileSystemId": str,
         "mountPoint": str,
     },
 )
@@ -651,14 +637,29 @@
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
+HighAvailabilityConfigOutputTypeDef = TypedDict(
+    "HighAvailabilityConfigOutputTypeDef",
+    {
+        "desiredCapacity": int,
+    },
+)
+
+GetSignedBluinsightsUrlResponseTypeDef = TypedDict(
+    "GetSignedBluinsightsUrlResponseTypeDef",
+    {
+        "signedBiUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
@@ -991,27 +992,35 @@
 
 MaintenanceScheduleTypeDef = TypedDict(
     "MaintenanceScheduleTypeDef",
     {
         "endTime": datetime,
         "startTime": datetime,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PrimaryKeyOutputTypeDef = TypedDict(
+    "PrimaryKeyOutputTypeDef",
+    {
+        "length": int,
+        "name": str,
+        "offset": int,
+    },
+)
+
 _RequiredPrimaryKeyTypeDef = TypedDict(
     "_RequiredPrimaryKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -1146,15 +1155,22 @@
 
 BatchJobDefinitionTypeDef = TypedDict(
     "BatchJobDefinitionTypeDef",
     {
         "fileBatchJobDefinition": FileBatchJobDefinitionTypeDef,
         "scriptBatchJobDefinition": ScriptBatchJobDefinitionTypeDef,
     },
-    total=False,
+)
+
+BatchJobIdentifierOutputTypeDef = TypedDict(
+    "BatchJobIdentifierOutputTypeDef",
+    {
+        "fileBatchJobIdentifier": FileBatchJobIdentifierOutputTypeDef,
+        "scriptBatchJobIdentifier": ScriptBatchJobIdentifierOutputTypeDef,
+    },
 )
 
 BatchJobIdentifierTypeDef = TypedDict(
     "BatchJobIdentifierTypeDef",
     {
         "fileBatchJobIdentifier": FileBatchJobIdentifierTypeDef,
         "scriptBatchJobIdentifier": ScriptBatchJobIdentifierTypeDef,
@@ -1259,14 +1275,22 @@
     {
         "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StorageConfigurationOutputTypeDef = TypedDict(
+    "StorageConfigurationOutputTypeDef",
+    {
+        "efs": EfsStorageConfigurationOutputTypeDef,
+        "fsx": FsxStorageConfigurationOutputTypeDef,
+    },
+)
+
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "efs": EfsStorageConfigurationTypeDef,
         "fsx": FsxStorageConfigurationTypeDef,
     },
     total=False,
@@ -1301,15 +1325,26 @@
 
 PendingMaintenanceTypeDef = TypedDict(
     "PendingMaintenanceTypeDef",
     {
         "engineVersion": str,
         "schedule": MaintenanceScheduleTypeDef,
     },
-    total=False,
+)
+
+VsamDetailAttributesTypeDef = TypedDict(
+    "VsamDetailAttributesTypeDef",
+    {
+        "alternateKeys": List[AlternateKeyOutputTypeDef],
+        "cacheAtStartup": bool,
+        "compressed": bool,
+        "encoding": str,
+        "primaryKey": PrimaryKeyOutputTypeDef,
+        "recordFormat": str,
+    },
 )
 
 _RequiredVsamAttributesTypeDef = TypedDict(
     "_RequiredVsamAttributesTypeDef",
     {
         "format": str,
     },
@@ -1324,68 +1359,44 @@
     },
     total=False,
 )
 
 class VsamAttributesTypeDef(_RequiredVsamAttributesTypeDef, _OptionalVsamAttributesTypeDef):
     pass
 
-VsamDetailAttributesTypeDef = TypedDict(
-    "VsamDetailAttributesTypeDef",
-    {
-        "alternateKeys": List[AlternateKeyTypeDef],
-        "cacheAtStartup": bool,
-        "compressed": bool,
-        "encoding": str,
-        "primaryKey": PrimaryKeyTypeDef,
-        "recordFormat": str,
-    },
-    total=False,
-)
-
 ListBatchJobDefinitionsResponseTypeDef = TypedDict(
     "ListBatchJobDefinitionsResponseTypeDef",
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_RequiredBatchJobExecutionSummaryTypeDef",
+BatchJobExecutionSummaryTypeDef = TypedDict(
+    "BatchJobExecutionSummaryTypeDef",
     {
         "applicationId": str,
-        "executionId": str,
-        "startTime": datetime,
-        "status": BatchJobExecutionStatusType,
-    },
-)
-_OptionalBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_OptionalBatchJobExecutionSummaryTypeDef",
-    {
-        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
+        "executionId": str,
         "jobId": str,
         "jobName": str,
         "jobType": BatchJobTypeType,
         "returnCode": str,
+        "startTime": datetime,
+        "status": BatchJobExecutionStatusType,
     },
-    total=False,
 )
 
-class BatchJobExecutionSummaryTypeDef(
-    _RequiredBatchJobExecutionSummaryTypeDef, _OptionalBatchJobExecutionSummaryTypeDef
-):
-    pass
-
 GetBatchJobExecutionResponseTypeDef = TypedDict(
     "GetBatchJobExecutionResponseTypeDef",
     {
         "applicationId": str,
-        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
         "executionId": str,
         "jobId": str,
         "jobName": str,
         "jobType": BatchJobTypeType,
         "jobUser": str,
         "returnCode": str,
@@ -1462,64 +1473,78 @@
         "actualCapacity": int,
         "creationTime": datetime,
         "description": str,
         "engineType": EngineTypeType,
         "engineVersion": str,
         "environmentArn": str,
         "environmentId": str,
-        "highAvailabilityConfig": HighAvailabilityConfigTypeDef,
+        "highAvailabilityConfig": HighAvailabilityConfigOutputTypeDef,
         "instanceType": str,
         "kmsKeyId": str,
         "loadBalancerArn": str,
         "name": str,
         "pendingMaintenance": PendingMaintenanceTypeDef,
         "preferredMaintenanceWindow": str,
         "publiclyAccessible": bool,
         "securityGroupIds": List[str],
         "status": EnvironmentLifecycleType,
         "statusReason": str,
-        "storageConfigurations": List[StorageConfigurationTypeDef],
+        "storageConfigurations": List[StorageConfigurationOutputTypeDef],
         "subnetIds": List[str],
         "tags": Dict[str, str],
         "vpcId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatasetOrgAttributesTypeDef = TypedDict(
-    "DatasetOrgAttributesTypeDef",
-    {
-        "gdg": GdgAttributesTypeDef,
-        "po": PoAttributesTypeDef,
-        "ps": PsAttributesTypeDef,
-        "vsam": VsamAttributesTypeDef,
-    },
-    total=False,
-)
-
 DatasetDetailOrgAttributesTypeDef = TypedDict(
     "DatasetDetailOrgAttributesTypeDef",
     {
         "gdg": GdgDetailAttributesTypeDef,
         "po": PoDetailAttributesTypeDef,
         "ps": PsDetailAttributesTypeDef,
         "vsam": VsamDetailAttributesTypeDef,
     },
+)
+
+DatasetOrgAttributesTypeDef = TypedDict(
+    "DatasetOrgAttributesTypeDef",
+    {
+        "gdg": GdgAttributesTypeDef,
+        "po": PoAttributesTypeDef,
+        "ps": PsAttributesTypeDef,
+        "vsam": VsamAttributesTypeDef,
+    },
     total=False,
 )
 
 ListBatchJobExecutionsResponseTypeDef = TypedDict(
     "ListBatchJobExecutionsResponseTypeDef",
     {
         "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GetDataSetDetailsResponseTypeDef = TypedDict(
+    "GetDataSetDetailsResponseTypeDef",
+    {
+        "blocksize": int,
+        "creationTime": datetime,
+        "dataSetName": str,
+        "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
+        "lastReferencedTime": datetime,
+        "lastUpdatedTime": datetime,
+        "location": str,
+        "recordLength": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDataSetTypeDef = TypedDict(
     "_RequiredDataSetTypeDef",
     {
         "datasetName": str,
         "datasetOrg": DatasetOrgAttributesTypeDef,
         "recordLength": RecordLengthTypeDef,
     },
@@ -1532,29 +1557,14 @@
     },
     total=False,
 )
 
 class DataSetTypeDef(_RequiredDataSetTypeDef, _OptionalDataSetTypeDef):
     pass
 
-GetDataSetDetailsResponseTypeDef = TypedDict(
-    "GetDataSetDetailsResponseTypeDef",
-    {
-        "blocksize": int,
-        "creationTime": datetime,
-        "dataSetName": str,
-        "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
-        "lastReferencedTime": datetime,
-        "lastUpdatedTime": datetime,
-        "location": str,
-        "recordLength": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataSetImportItemTypeDef = TypedDict(
     "DataSetImportItemTypeDef",
     {
         "dataSet": DataSetTypeDef,
         "externalLocation": ExternalLocationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2.egg-info/PKG-INFO` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.28.0
-Summary: Type annotations for boto3.MainframeModernization 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.5
+Summary: Type annotations for boto3.MainframeModernization 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,19 +362,22 @@
 ### Typed dictionaries
 
 `mypy_boto3_m2.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_m2.type_defs import (
+    AlternateKeyOutputTypeDef,
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
+    FileBatchJobIdentifierOutputTypeDef,
+    ScriptBatchJobIdentifierOutputTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
     CreateApplicationResponseTypeDef,
     CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
@@ -392,28 +395,32 @@
     PoAttributesTypeDef,
     PsAttributesTypeDef,
     DeleteApplicationFromEnvironmentRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeployedVersionSummaryTypeDef,
     DeploymentSummaryTypeDef,
+    EfsStorageConfigurationOutputTypeDef,
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
+    FsxStorageConfigurationOutputTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
     GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
+    HighAvailabilityConfigOutputTypeDef,
+    GetSignedBluinsightsUrlResponseTypeDef,
     ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
     ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
@@ -428,60 +435,63 @@
     ListEngineVersionsRequestRequestTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
     PaginatorConfigTypeDef,
+    PrimaryKeyOutputTypeDef,
     PrimaryKeyTypeDef,
     ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
     StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
+    BatchJobIdentifierOutputTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
+    StorageConfigurationOutputTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
     PendingMaintenanceTypeDef,
-    VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
+    VsamAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
-    DatasetOrgAttributesTypeDef,
     DatasetDetailOrgAttributesTypeDef,
+    DatasetOrgAttributesTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
-    DataSetTypeDef,
     GetDataSetDetailsResponseTypeDef,
+    DataSetTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AlternateKeyTypeDef:
+def get_structure() -> AlternateKeyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-m2-1.28.0/mypy_boto3_m2.egg-info/SOURCES.txt` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.0/setup.py` & `mypy-boto3-m2-1.28.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-m2",
-    version="1.28.0",
+    version="1.28.5",
     packages=["mypy_boto3_m2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MainframeModernization 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MainframeModernization 1.28.5 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

