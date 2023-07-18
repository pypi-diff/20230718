# Comparing `tmp/mypy-boto3-glue-1.28.1.tar.gz` & `tmp/mypy-boto3-glue-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glue-1.28.1.tar", last modified: Fri Jul  7 19:32:38 2023, max compression
+gzip compressed data, was "mypy-boto3-glue-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-glue-1.28.1.tar` & `mypy-boto3-glue-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.903385 mypy-boto3-glue-1.28.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 19:32:06.000000 mypy-boto3-glue-1.28.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42132 2023-07-07 19:32:38.903385 mypy-boto3-glue-1.28.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40659 2023-07-07 19:32:06.000000 mypy-boto3-glue-1.28.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.903385 mypy-boto3-glue-1.28.1/mypy_boto3_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-07 19:32:06.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-07 19:32:06.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-07 19:32:06.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   137259 2023-07-07 19:32:08.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   137031 2023-07-07 19:32:07.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20839 2023-07-07 19:32:08.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20837 2023-07-07 19:32:08.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-07-07 19:32:08.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-07-07 19:32:08.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:06.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   254038 2023-07-07 19:32:15.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   253661 2023-07-07 19:32:12.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 19:32:06.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:32:38.903385 mypy-boto3-glue-1.28.1/mypy_boto3_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42132 2023-07-07 19:32:38.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 19:32:38.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:32:38.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 19:32:38.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 19:32:38.000000 mypy-boto3-glue-1.28.1/mypy_boto3_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:32:38.903385 mypy-boto3-glue-1.28.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-07 19:32:06.000000 mypy-boto3-glue-1.28.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-glue-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47930 2023-07-18 01:01:41.973310 mypy-boto3-glue-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    46457 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-glue-1.28.4/mypy_boto3_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137259 2023-07-18 01:01:19.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137031 2023-07-18 01:01:18.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20892 2023-07-18 01:01:19.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20890 2023-07-18 01:01:19.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-07-18 01:01:19.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-07-18 01:01:19.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   302062 2023-07-18 01:01:27.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   301703 2023-07-18 01:01:23.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47930 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 01:01:41.000000 mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.973310 mypy-boto3-glue-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-18 01:01:17.000000 mypy-boto3-glue-1.28.4/setup.py
```

### Comparing `mypy-boto3-glue-1.28.1/LICENSE` & `mypy-boto3-glue-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.1/PKG-INFO` & `mypy-boto3-glue-1.28.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-glue
-Version: 1.28.1
-Summary: Type annotations for boto3.Glue 1.28.1 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 glue type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-glue"></a>
 
 # mypy-boto3-glue
 
 [![PyPI - mypy-boto3-glue](https://img.shields.io/pypi/v/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
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
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
 
@@ -472,62 +440,101 @@
 ### Typed dictionaries
 
 `mypy_boto3_glue.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glue.type_defs import (
+    NotificationPropertyOutputTypeDef,
     NotificationPropertyTypeDef,
+    AggregateOperationOutputTypeDef,
     AggregateOperationTypeDef,
+    AmazonRedshiftAdvancedOptionOutputTypeDef,
     AmazonRedshiftAdvancedOptionTypeDef,
+    OptionOutputTypeDef,
     OptionTypeDef,
+    ApplyMappingOutputTypeDef,
     ApplyMappingTypeDef,
     AuditContextTypeDef,
-    PartitionValueListTypeDef,
+    PartitionValueListOutputTypeDef,
+    BasicCatalogTargetOutputTypeDef,
     BasicCatalogTargetTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteConnectionRequestRequestTypeDef,
     ErrorDetailTypeDef,
+    PartitionValueListTypeDef,
     BatchDeleteTableRequestRequestTypeDef,
     BatchDeleteTableVersionRequestRequestTypeDef,
     BatchGetBlueprintsRequestRequestTypeDef,
     BatchGetCrawlersRequestRequestTypeDef,
     BatchGetCustomEntityTypesRequestRequestTypeDef,
     CustomEntityTypeTypeDef,
     BatchGetDataQualityResultRequestRequestTypeDef,
     BatchGetDevEndpointsRequestRequestTypeDef,
     DevEndpointTypeDef,
     BatchGetJobsRequestRequestTypeDef,
     BatchGetTriggersRequestRequestTypeDef,
     BatchGetWorkflowsRequestRequestTypeDef,
     BatchStopJobRunRequestRequestTypeDef,
     BatchStopJobRunSuccessfulSubmissionTypeDef,
+    BinaryColumnStatisticsDataOutputTypeDef,
     BinaryColumnStatisticsDataTypeDef,
     BlueprintDetailsTypeDef,
     BlueprintRunTypeDef,
     LastActiveDefinitionTypeDef,
+    BooleanColumnStatisticsDataOutputTypeDef,
     BooleanColumnStatisticsDataTypeDef,
     CancelDataQualityRuleRecommendationRunRequestRequestTypeDef,
     CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CancelMLTaskRunRequestRequestTypeDef,
     CancelStatementRequestRequestTypeDef,
     CatalogEntryTypeDef,
     CatalogImportStatusTypeDef,
+    KafkaStreamingSourceOptionsOutputTypeDef,
+    StreamingDataPreviewOptionsOutputTypeDef,
     KafkaStreamingSourceOptionsTypeDef,
     StreamingDataPreviewOptionsTypeDef,
+    KinesisStreamingSourceOptionsOutputTypeDef,
     KinesisStreamingSourceOptionsTypeDef,
+    CatalogSchemaChangePolicyOutputTypeDef,
     CatalogSchemaChangePolicyTypeDef,
+    CatalogSourceOutputTypeDef,
     CatalogSourceTypeDef,
+    CatalogTargetOutputTypeDef,
     CatalogTargetTypeDef,
     CheckSchemaVersionValidityInputRequestTypeDef,
     CsvClassifierTypeDef,
     GrokClassifierTypeDef,
     JsonClassifierTypeDef,
     XMLClassifierTypeDef,
+    CloudWatchEncryptionOutputTypeDef,
     CloudWatchEncryptionTypeDef,
+    DirectJDBCSourceOutputTypeDef,
+    DropDuplicatesOutputTypeDef,
+    DropFieldsOutputTypeDef,
+    DynamoDBCatalogSourceOutputTypeDef,
+    FillMissingValuesOutputTypeDef,
+    MergeOutputTypeDef,
+    MicrosoftSQLServerCatalogSourceOutputTypeDef,
+    MicrosoftSQLServerCatalogTargetOutputTypeDef,
+    MySQLCatalogSourceOutputTypeDef,
+    MySQLCatalogTargetOutputTypeDef,
+    OracleSQLCatalogSourceOutputTypeDef,
+    OracleSQLCatalogTargetOutputTypeDef,
+    PIIDetectionOutputTypeDef,
+    PostgreSQLCatalogSourceOutputTypeDef,
+    PostgreSQLCatalogTargetOutputTypeDef,
+    RedshiftSourceOutputTypeDef,
+    RelationalCatalogSourceOutputTypeDef,
+    RenameFieldOutputTypeDef,
+    SelectFieldsOutputTypeDef,
+    SelectFromCollectionOutputTypeDef,
+    SpigotOutputTypeDef,
+    SplitFieldsOutputTypeDef,
+    UnionOutputTypeDef,
     DirectJDBCSourceTypeDef,
     DropDuplicatesTypeDef,
     DropFieldsTypeDef,
     DynamoDBCatalogSourceTypeDef,
     FillMissingValuesTypeDef,
     MergeTypeDef,
     MicrosoftSQLServerCatalogSourceTypeDef,
@@ -543,71 +550,103 @@
     RelationalCatalogSourceTypeDef,
     RenameFieldTypeDef,
     SelectFieldsTypeDef,
     SelectFromCollectionTypeDef,
     SpigotTypeDef,
     SplitFieldsTypeDef,
     UnionTypeDef,
+    CodeGenEdgeOutputTypeDef,
     CodeGenEdgeTypeDef,
+    CodeGenNodeArgOutputTypeDef,
     CodeGenNodeArgTypeDef,
     ColumnImportanceTypeDef,
+    ColumnOutputTypeDef,
     ColumnRowFilterTypeDef,
+    DateColumnStatisticsDataOutputTypeDef,
+    DoubleColumnStatisticsDataOutputTypeDef,
+    LongColumnStatisticsDataOutputTypeDef,
+    StringColumnStatisticsDataOutputTypeDef,
     DateColumnStatisticsDataTypeDef,
     DoubleColumnStatisticsDataTypeDef,
     LongColumnStatisticsDataTypeDef,
     StringColumnStatisticsDataTypeDef,
     ColumnTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     ConfusionMatrixTypeDef,
     PhysicalConnectionRequirementsTypeDef,
+    ConnectionPasswordEncryptionOutputTypeDef,
     ConnectionPasswordEncryptionTypeDef,
+    PhysicalConnectionRequirementsOutputTypeDef,
+    ConnectionsListOutputTypeDef,
     ConnectionsListTypeDef,
     CrawlTypeDef,
     CrawlerHistoryTypeDef,
     CrawlerMetricsTypeDef,
+    DeltaTargetOutputTypeDef,
+    DynamoDBTargetOutputTypeDef,
+    IcebergTargetOutputTypeDef,
+    JdbcTargetOutputTypeDef,
+    MongoDBTargetOutputTypeDef,
+    S3TargetOutputTypeDef,
     DeltaTargetTypeDef,
     DynamoDBTargetTypeDef,
     IcebergTargetTypeDef,
     JdbcTargetTypeDef,
     MongoDBTargetTypeDef,
     S3TargetTypeDef,
-    LakeFormationConfigurationTypeDef,
+    LakeFormationConfigurationOutputTypeDef,
     LastCrawlInfoTypeDef,
-    LineageConfigurationTypeDef,
-    RecrawlPolicyTypeDef,
+    LineageConfigurationOutputTypeDef,
+    RecrawlPolicyOutputTypeDef,
     ScheduleTypeDef,
-    SchemaChangePolicyTypeDef,
+    SchemaChangePolicyOutputTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintRequestRequestTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateXMLClassifierRequestTypeDef,
+    LakeFormationConfigurationTypeDef,
+    LineageConfigurationTypeDef,
+    RecrawlPolicyTypeDef,
+    SchemaChangePolicyTypeDef,
     CreateCustomEntityTypeRequestRequestTypeDef,
     DataQualityTargetTableTypeDef,
     CreateDevEndpointRequestRequestTypeDef,
     ExecutionPropertyTypeDef,
     JobCommandTypeDef,
     SourceControlDetailsTypeDef,
     GlueTableTypeDef,
     PartitionIndexTypeDef,
     CreateRegistryInputRequestTypeDef,
     RegistryIdTypeDef,
     SessionCommandTypeDef,
     EventBatchingConditionTypeDef,
     CreateWorkflowRequestRequestTypeDef,
+    DQResultsPublishingOptionsOutputTypeDef,
     DQResultsPublishingOptionsTypeDef,
+    DQStopJobOnFailureOptionsOutputTypeDef,
     DQStopJobOnFailureOptionsTypeDef,
+    EncryptionAtRestOutputTypeDef,
     EncryptionAtRestTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
+    DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef,
     DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
     DataQualityRuleResultTypeDef,
+    DataQualityTargetTableOutputTypeDef,
+    GlueTableOutputTypeDef,
+    DatabaseIdentifierOutputTypeDef,
     DatabaseIdentifierTypeDef,
     FederatedDatabaseTypeDef,
+    FederatedDatabaseOutputTypeDef,
+    DatatypeOutputTypeDef,
     DatatypeTypeDef,
+    DecimalNumberOutputTypeDef,
     DecimalNumberTypeDef,
     DeleteBlueprintRequestRequestTypeDef,
     DeleteClassifierRequestRequestTypeDef,
     DeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     DeleteColumnStatisticsForTableRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteCrawlerRequestRequestTypeDef,
@@ -625,24 +664,33 @@
     DeleteSessionRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DeleteTableVersionRequestRequestTypeDef,
     DeleteTriggerRequestRequestTypeDef,
     DeleteUserDefinedFunctionRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DevEndpointCustomLibrariesTypeDef,
+    DirectSchemaChangePolicyOutputTypeDef,
     DirectSchemaChangePolicyTypeDef,
+    NullCheckBoxListOutputTypeDef,
     NullCheckBoxListTypeDef,
+    TransformConfigParameterOutputTypeDef,
     TransformConfigParameterTypeDef,
     EdgeTypeDef,
+    JobBookmarksEncryptionOutputTypeDef,
+    S3EncryptionOutputTypeDef,
     JobBookmarksEncryptionTypeDef,
     S3EncryptionTypeDef,
     ErrorDetailsTypeDef,
+    EventBatchingConditionOutputTypeDef,
+    ExecutionPropertyOutputTypeDef,
     ExportLabelsTaskRunPropertiesTypeDef,
     FederatedTableTypeDef,
+    FilterValueOutputTypeDef,
     FilterValueTypeDef,
+    FindMatchesParametersOutputTypeDef,
     FindMatchesParametersTypeDef,
     FindMatchesTaskRunPropertiesTypeDef,
     GetBlueprintRequestRequestTypeDef,
     GetBlueprintRunRequestRequestTypeDef,
     GetBlueprintRunsRequestRequestTypeDef,
     GetCatalogImportStatusRequestRequestTypeDef,
     GetClassifierRequestRequestTypeDef,
@@ -672,20 +720,21 @@
     GetJobRunRequestRequestTypeDef,
     GetJobRunsRequestRequestTypeDef,
     GetJobsRequestRequestTypeDef,
     GetMLTaskRunRequestRequestTypeDef,
     TaskRunFilterCriteriaTypeDef,
     TaskRunSortCriteriaTypeDef,
     GetMLTransformRequestRequestTypeDef,
-    SchemaColumnTypeDef,
+    SchemaColumnOutputTypeDef,
     TransformSortCriteriaTypeDef,
-    MappingEntryTypeDef,
+    MappingEntryOutputTypeDef,
     GetPartitionIndexesRequestRequestTypeDef,
     GetPartitionRequestRequestTypeDef,
     SegmentTypeDef,
+    MappingEntryTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GluePolicyTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     SchemaVersionNumberTypeDef,
     GetSecurityConfigurationRequestRequestTypeDef,
     GetSecurityConfigurationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
@@ -699,21 +748,27 @@
     GetTriggersRequestRequestTypeDef,
     GetUserDefinedFunctionRequestRequestTypeDef,
     GetUserDefinedFunctionsRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowRunPropertiesRequestRequestTypeDef,
     GetWorkflowRunRequestRequestTypeDef,
     GetWorkflowRunsRequestRequestTypeDef,
+    GlueStudioSchemaColumnOutputTypeDef,
     GlueStudioSchemaColumnTypeDef,
+    S3SourceAdditionalOptionsOutputTypeDef,
     S3SourceAdditionalOptionsTypeDef,
     IcebergInputTypeDef,
     ImportCatalogToGlueRequestRequestTypeDef,
     ImportLabelsTaskRunPropertiesTypeDef,
+    JDBCConnectorOptionsOutputTypeDef,
     JDBCConnectorOptionsTypeDef,
+    JobCommandOutputTypeDef,
     PredecessorTypeDef,
+    SourceControlDetailsOutputTypeDef,
+    JoinColumnOutputTypeDef,
     JoinColumnTypeDef,
     KeySchemaElementTypeDef,
     LabelingSetGenerationTaskRunPropertiesTypeDef,
     ListBlueprintsRequestRequestTypeDef,
     ListCrawlersRequestRequestTypeDef,
     ListCustomEntityTypesRequestRequestTypeDef,
     ListDevEndpointsRequestRequestTypeDef,
@@ -722,31 +777,43 @@
     RegistryListItemTypeDef,
     SchemaVersionListItemTypeDef,
     SchemaListItemTypeDef,
     ListSessionsRequestRequestTypeDef,
     ListStatementsRequestRequestTypeDef,
     ListTriggersRequestRequestTypeDef,
     ListWorkflowsRequestRequestTypeDef,
+    MLUserDataEncryptionOutputTypeDef,
     MLUserDataEncryptionTypeDef,
+    MappingOutputTypeDef,
     MappingTypeDef,
     OtherMetadataValueListItemTypeDef,
     MetadataKeyValuePairTypeDef,
+    OrderOutputTypeDef,
     OrderTypeDef,
     PropertyPredicateTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutWorkflowRunPropertiesRequestRequestTypeDef,
+    UpsertRedshiftTargetOptionsOutputTypeDef,
     UpsertRedshiftTargetOptionsTypeDef,
     ResetJobBookmarkRequestRequestTypeDef,
+    ResourceUriOutputTypeDef,
     ResourceUriTypeDef,
     ResumeWorkflowRunRequestRequestTypeDef,
     RunStatementRequestRequestTypeDef,
+    S3DirectSourceAdditionalOptionsOutputTypeDef,
     S3DirectSourceAdditionalOptionsTypeDef,
+    SchemaColumnTypeDef,
+    SchemaIdOutputTypeDef,
     SortCriterionTypeDef,
+    SerDeInfoOutputTypeDef,
     SerDeInfoTypeDef,
+    SessionCommandOutputTypeDef,
+    SkewedInfoOutputTypeDef,
     SkewedInfoTypeDef,
+    SqlAliasOutputTypeDef,
     SqlAliasTypeDef,
     StartBlueprintRunRequestRequestTypeDef,
     StartCrawlerRequestRequestTypeDef,
     StartCrawlerScheduleRequestRequestTypeDef,
     StartExportLabelsTaskRunRequestRequestTypeDef,
     StartImportLabelsTaskRunRequestRequestTypeDef,
     StartMLEvaluationTaskRunRequestRequestTypeDef,
@@ -756,37 +823,39 @@
     StartingEventBatchConditionTypeDef,
     StatementOutputDataTypeDef,
     StopCrawlerRequestRequestTypeDef,
     StopCrawlerScheduleRequestRequestTypeDef,
     StopSessionRequestRequestTypeDef,
     StopTriggerRequestRequestTypeDef,
     StopWorkflowRunRequestRequestTypeDef,
+    TableIdentifierOutputTypeDef,
     TableIdentifierTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBlueprintRequestRequestTypeDef,
     UpdateCsvClassifierRequestTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateXMLClassifierRequestTypeDef,
     UpdateCrawlerScheduleRequestRequestTypeDef,
     UpdateDataQualityRulesetRequestRequestTypeDef,
     UpdateJobFromSourceControlRequestRequestTypeDef,
     UpdateSourceControlFromJobRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     WorkflowRunStatisticsTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     StartJobRunRequestRequestTypeDef,
+    AggregateOutputTypeDef,
     AggregateTypeDef,
+    AmazonRedshiftNodeDataOutputTypeDef,
     AmazonRedshiftNodeDataTypeDef,
     GetUnfilteredPartitionMetadataRequestRequestTypeDef,
     GetUnfilteredTableMetadataRequestRequestTypeDef,
     BackfillErrorTypeDef,
-    BatchDeletePartitionRequestRequestTypeDef,
-    BatchGetPartitionRequestRequestTypeDef,
     CancelMLTaskRunResponseTypeDef,
     CheckSchemaVersionValidityResponseTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
     CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateJobResponseTypeDef,
@@ -853,78 +922,104 @@
     BatchDeleteConnectionResponseTypeDef,
     BatchStopJobRunErrorTypeDef,
     BatchUpdatePartitionFailureEntryTypeDef,
     ColumnErrorTypeDef,
     PartitionErrorTypeDef,
     TableErrorTypeDef,
     TableVersionErrorTypeDef,
+    BatchDeletePartitionRequestRequestTypeDef,
+    BatchGetPartitionRequestRequestTypeDef,
     BatchGetCustomEntityTypesResponseTypeDef,
     ListCustomEntityTypesResponseTypeDef,
     BatchGetDevEndpointsResponseTypeDef,
     GetDevEndpointResponseTypeDef,
     GetDevEndpointsResponseTypeDef,
     GetBlueprintRunResponseTypeDef,
     GetBlueprintRunsResponseTypeDef,
     BlueprintTypeDef,
     GetCatalogImportStatusResponseTypeDef,
+    CatalogKafkaSourceOutputTypeDef,
+    DirectKafkaSourceOutputTypeDef,
     CatalogKafkaSourceTypeDef,
     DirectKafkaSourceTypeDef,
+    CatalogKinesisSourceOutputTypeDef,
+    DirectKinesisSourceOutputTypeDef,
     CatalogKinesisSourceTypeDef,
     DirectKinesisSourceTypeDef,
+    GovernedCatalogTargetOutputTypeDef,
+    S3CatalogTargetOutputTypeDef,
+    S3DeltaCatalogTargetOutputTypeDef,
+    S3HudiCatalogTargetOutputTypeDef,
     GovernedCatalogTargetTypeDef,
     S3CatalogTargetTypeDef,
     S3DeltaCatalogTargetTypeDef,
     S3HudiCatalogTargetTypeDef,
     ClassifierTypeDef,
+    CodeGenNodeOutputTypeDef,
     CodeGenNodeTypeDef,
     LocationTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     FindMatchesMetricsTypeDef,
     ConnectionInputTypeDef,
     ConnectionTypeDef,
     CrawlerNodeDetailsTypeDef,
     ListCrawlsResponseTypeDef,
     GetCrawlerMetricsResponseTypeDef,
+    CrawlerTargetsOutputTypeDef,
     CrawlerTargetsTypeDef,
     ListCrawlsRequestRequestTypeDef,
     CreateClassifierRequestRequestTypeDef,
     CreateDataQualityRulesetRequestRequestTypeDef,
     DataQualityRulesetFilterCriteriaTypeDef,
-    DataQualityRulesetListDetailsTypeDef,
-    GetDataQualityRulesetResponseTypeDef,
     DataSourceTypeDef,
     CreatePartitionIndexRequestRequestTypeDef,
     CreateSchemaInputRequestTypeDef,
     DeleteRegistryInputRequestTypeDef,
     GetRegistryInputRequestTypeDef,
     ListSchemasInputRequestTypeDef,
     UpdateRegistryInputRequestTypeDef,
     CreateSessionRequestRequestTypeDef,
-    SessionTypeDef,
+    EvaluateDataQualityMultiFrameOutputTypeDef,
+    EvaluateDataQualityOutputTypeDef,
     EvaluateDataQualityMultiFrameTypeDef,
     EvaluateDataQualityTypeDef,
+    DataCatalogEncryptionSettingsOutputTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
+    PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    DataQualityRulesetListDetailsTypeDef,
+    GetDataQualityRulesetResponseTypeDef,
+    DataSourceOutputTypeDef,
+    NullValueFieldOutputTypeDef,
     NullValueFieldTypeDef,
+    DecimalColumnStatisticsDataOutputTypeDef,
     DecimalColumnStatisticsDataTypeDef,
     DeleteSchemaInputRequestTypeDef,
     DeleteSchemaVersionsInputRequestTypeDef,
     GetSchemaByDefinitionInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     ListSchemaVersionsInputRequestTypeDef,
     RegisterSchemaVersionInputRequestTypeDef,
     SchemaReferenceTypeDef,
     UpdateDevEndpointRequestRequestTypeDef,
+    S3DeltaDirectTargetOutputTypeDef,
+    S3DirectTargetOutputTypeDef,
+    S3GlueParquetTargetOutputTypeDef,
+    S3HudiDirectTargetOutputTypeDef,
     S3DeltaDirectTargetTypeDef,
     S3DirectTargetTypeDef,
     S3GlueParquetTargetTypeDef,
     S3HudiDirectTargetTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     SchemaVersionErrorItemTypeDef,
+    FilterExpressionOutputTypeDef,
     FilterExpressionTypeDef,
+    TransformParametersOutputTypeDef,
     TransformParametersTypeDef,
     GetClassifiersRequestGetClassifiersPaginateTypeDef,
     GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
     GetCrawlersRequestGetCrawlersPaginateTypeDef,
     GetDatabasesRequestGetDatabasesPaginateTypeDef,
     GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef,
     GetJobRunsRequestGetJobRunsPaginateTypeDef,
@@ -940,103 +1035,128 @@
     ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     ListSchemasInputListSchemasPaginateTypeDef,
     GetConnectionsRequestGetConnectionsPaginateTypeDef,
     GetConnectionsRequestRequestTypeDef,
     GetJobBookmarkResponseTypeDef,
     ResetJobBookmarkResponseTypeDef,
     GetMLTaskRunsRequestRequestTypeDef,
-    TransformFilterCriteriaTypeDef,
     GetMappingResponseTypeDef,
     GetPartitionsRequestGetPartitionsPaginateTypeDef,
     GetPartitionsRequestRequestTypeDef,
     GetUnfilteredPartitionsMetadataRequestRequestTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetSchemaVersionInputRequestTypeDef,
     GetSchemaVersionsDiffInputRequestTypeDef,
     UpdateSchemaInputRequestTypeDef,
+    GlueSchemaOutputTypeDef,
     GlueSchemaTypeDef,
+    GovernedCatalogSourceOutputTypeDef,
+    S3CatalogSourceOutputTypeDef,
     GovernedCatalogSourceTypeDef,
     S3CatalogSourceTypeDef,
     OpenTableFormatInputTypeDef,
     JobRunTypeDef,
+    JoinOutputTypeDef,
     JoinTypeDef,
     TaskRunPropertiesTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
+    TransformEncryptionOutputTypeDef,
     TransformEncryptionTypeDef,
     MetadataInfoTypeDef,
     PutSchemaVersionMetadataInputRequestTypeDef,
     QuerySchemaVersionMetadataInputRequestTypeDef,
     RemoveSchemaVersionMetadataInputRequestTypeDef,
+    RedshiftTargetOutputTypeDef,
     RedshiftTargetTypeDef,
-    UserDefinedFunctionInputTypeDef,
     UserDefinedFunctionTypeDef,
+    UserDefinedFunctionInputTypeDef,
+    TransformFilterCriteriaTypeDef,
+    SchemaReferenceOutputTypeDef,
     SearchTablesRequestRequestTypeDef,
+    SessionTypeDef,
     StatementOutputTypeDef,
     UpdateClassifierRequestRequestTypeDef,
+    AmazonRedshiftSourceOutputTypeDef,
+    AmazonRedshiftTargetOutputTypeDef,
     AmazonRedshiftSourceTypeDef,
     AmazonRedshiftTargetTypeDef,
     PartitionIndexDescriptorTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionResponseTypeDef,
     BatchCreatePartitionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
     BatchGetBlueprintsResponseTypeDef,
     GetBlueprintResponseTypeDef,
     GetClassifierResponseTypeDef,
     GetClassifiersResponseTypeDef,
-    CreateScriptRequestRequestTypeDef,
     GetDataflowGraphResponseTypeDef,
+    CreateScriptRequestRequestTypeDef,
     GetMappingRequestRequestTypeDef,
     GetPlanRequestRequestTypeDef,
-    CreateTriggerRequestRequestTypeDef,
     TriggerTypeDef,
+    CreateTriggerRequestRequestTypeDef,
     TriggerUpdateTypeDef,
     EvaluationMetricsTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     GetConnectionResponseTypeDef,
     GetConnectionsResponseTypeDef,
     CrawlerTypeDef,
     CreateCrawlerRequestRequestTypeDef,
     UpdateCrawlerRequestRequestTypeDef,
     ListDataQualityRulesetsRequestRequestTypeDef,
-    ListDataQualityRulesetsResponseTypeDef,
-    DataQualityResultDescriptionTypeDef,
     DataQualityResultFilterCriteriaTypeDef,
-    DataQualityResultTypeDef,
-    DataQualityRuleRecommendationRunDescriptionTypeDef,
     DataQualityRuleRecommendationRunFilterTypeDef,
-    DataQualityRulesetEvaluationRunDescriptionTypeDef,
     DataQualityRulesetEvaluationRunFilterTypeDef,
-    GetDataQualityResultResponseTypeDef,
-    GetDataQualityRuleRecommendationRunResponseTypeDef,
-    GetDataQualityRulesetEvaluationRunResponseTypeDef,
     StartDataQualityRuleRecommendationRunRequestRequestTypeDef,
     StartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-    CreateSessionResponseTypeDef,
-    GetSessionResponseTypeDef,
-    ListSessionsResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     PutDataCatalogEncryptionSettingsRequestRequestTypeDef,
-    DatabaseInputTypeDef,
     DatabaseTypeDef,
+    DatabaseInputTypeDef,
+    ListDataQualityRulesetsResponseTypeDef,
+    DataQualityResultDescriptionTypeDef,
+    DataQualityResultTypeDef,
+    DataQualityRuleRecommendationRunDescriptionTypeDef,
+    DataQualityRulesetEvaluationRunDescriptionTypeDef,
+    GetDataQualityResultResponseTypeDef,
+    GetDataQualityRuleRecommendationRunResponseTypeDef,
+    GetDataQualityRulesetEvaluationRunResponseTypeDef,
+    DropNullFieldsOutputTypeDef,
     DropNullFieldsTypeDef,
+    ColumnStatisticsDataOutputTypeDef,
     ColumnStatisticsDataTypeDef,
     StorageDescriptorTypeDef,
-    CreateSecurityConfigurationRequestRequestTypeDef,
     SecurityConfigurationTypeDef,
+    CreateSecurityConfigurationRequestRequestTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
     UpdateMLTransformRequestRequestTypeDef,
-    GetMLTransformsRequestRequestTypeDef,
-    ListMLTransformsRequestRequestTypeDef,
+    AthenaConnectorSourceOutputTypeDef,
+    CatalogDeltaSourceOutputTypeDef,
+    CatalogHudiSourceOutputTypeDef,
+    CustomCodeOutputTypeDef,
+    DynamicTransformOutputTypeDef,
+    JDBCConnectorSourceOutputTypeDef,
+    JDBCConnectorTargetOutputTypeDef,
+    S3CatalogDeltaSourceOutputTypeDef,
+    S3CatalogHudiSourceOutputTypeDef,
+    S3CsvSourceOutputTypeDef,
+    S3DeltaSourceOutputTypeDef,
+    S3HudiSourceOutputTypeDef,
+    S3JsonSourceOutputTypeDef,
+    S3ParquetSourceOutputTypeDef,
+    SparkConnectorSourceOutputTypeDef,
+    SparkConnectorTargetOutputTypeDef,
+    SparkSQLOutputTypeDef,
     AthenaConnectorSourceTypeDef,
     CatalogDeltaSourceTypeDef,
     CatalogHudiSourceTypeDef,
     CustomCodeTypeDef,
     DynamicTransformTypeDef,
     JDBCConnectorSourceTypeDef,
     JDBCConnectorTargetTypeDef,
@@ -1053,100 +1173,108 @@
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
     JobNodeDetailsTypeDef,
     GetMLTaskRunResponseTypeDef,
     TaskRunTypeDef,
     CreateMLTransformRequestRequestTypeDef,
     QuerySchemaVersionMetadataResponseTypeDef,
-    CreateUserDefinedFunctionRequestRequestTypeDef,
-    UpdateUserDefinedFunctionRequestRequestTypeDef,
     GetUserDefinedFunctionResponseTypeDef,
     GetUserDefinedFunctionsResponseTypeDef,
+    CreateUserDefinedFunctionRequestRequestTypeDef,
+    UpdateUserDefinedFunctionRequestRequestTypeDef,
+    GetMLTransformsRequestRequestTypeDef,
+    ListMLTransformsRequestRequestTypeDef,
+    StorageDescriptorOutputTypeDef,
+    CreateSessionResponseTypeDef,
+    GetSessionResponseTypeDef,
+    ListSessionsResponseTypeDef,
     StatementTypeDef,
     GetPartitionIndexesResponseTypeDef,
     BatchGetTriggersResponseTypeDef,
     GetTriggerResponseTypeDef,
     GetTriggersResponseTypeDef,
     TriggerNodeDetailsTypeDef,
     UpdateTriggerResponseTypeDef,
     UpdateTriggerRequestRequestTypeDef,
     GetMLTransformResponseTypeDef,
     MLTransformTypeDef,
     BatchGetCrawlersResponseTypeDef,
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
-    ListDataQualityResultsResponseTypeDef,
     ListDataQualityResultsRequestRequestTypeDef,
-    BatchGetDataQualityResultResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsResponseTypeDef,
     ListDataQualityRuleRecommendationRunsRequestRequestTypeDef,
-    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
     ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef,
-    CreateDatabaseRequestRequestTypeDef,
-    UpdateDatabaseRequestRequestTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
+    CreateDatabaseRequestRequestTypeDef,
+    UpdateDatabaseRequestRequestTypeDef,
+    ListDataQualityResultsResponseTypeDef,
+    BatchGetDataQualityResultResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsResponseTypeDef,
+    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
+    ColumnStatisticsOutputTypeDef,
     ColumnStatisticsTypeDef,
     PartitionInputTypeDef,
-    PartitionTypeDef,
     TableInputTypeDef,
-    TableTypeDef,
     GetSecurityConfigurationResponseTypeDef,
     GetSecurityConfigurationsResponseTypeDef,
+    CodeGenConfigurationNodeOutputTypeDef,
     CodeGenConfigurationNodeTypeDef,
     GetMLTaskRunsResponseTypeDef,
+    PartitionTypeDef,
+    TableTypeDef,
     GetStatementResponseTypeDef,
     ListStatementsResponseTypeDef,
     NodeTypeDef,
     GetMLTransformsResponseTypeDef,
     ColumnStatisticsErrorTypeDef,
     GetColumnStatisticsForPartitionResponseTypeDef,
     GetColumnStatisticsForTableResponseTypeDef,
     UpdateColumnStatisticsForPartitionRequestRequestTypeDef,
     UpdateColumnStatisticsForTableRequestRequestTypeDef,
     BatchCreatePartitionRequestRequestTypeDef,
     BatchUpdatePartitionRequestEntryTypeDef,
     CreatePartitionRequestRequestTypeDef,
     UpdatePartitionRequestRequestTypeDef,
+    CreateTableRequestRequestTypeDef,
+    UpdateTableRequestRequestTypeDef,
+    JobTypeDef,
+    CreateJobRequestRequestTypeDef,
+    JobUpdateTypeDef,
     BatchGetPartitionResponseTypeDef,
     GetPartitionResponseTypeDef,
     GetPartitionsResponseTypeDef,
     GetUnfilteredPartitionMetadataResponseTypeDef,
     UnfilteredPartitionTypeDef,
-    CreateTableRequestRequestTypeDef,
-    UpdateTableRequestRequestTypeDef,
     GetTableResponseTypeDef,
     GetTablesResponseTypeDef,
     GetUnfilteredTableMetadataResponseTypeDef,
     SearchTablesResponseTypeDef,
     TableVersionTypeDef,
-    CreateJobRequestRequestTypeDef,
-    JobTypeDef,
-    JobUpdateTypeDef,
     WorkflowGraphTypeDef,
     UpdateColumnStatisticsForPartitionResponseTypeDef,
     UpdateColumnStatisticsForTableResponseTypeDef,
     BatchUpdatePartitionRequestRequestTypeDef,
-    GetUnfilteredPartitionsMetadataResponseTypeDef,
-    GetTableVersionResponseTypeDef,
-    GetTableVersionsResponseTypeDef,
     BatchGetJobsResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobsResponseTypeDef,
     UpdateJobRequestRequestTypeDef,
+    GetUnfilteredPartitionsMetadataResponseTypeDef,
+    GetTableVersionResponseTypeDef,
+    GetTableVersionsResponseTypeDef,
     WorkflowRunTypeDef,
     GetWorkflowRunResponseTypeDef,
     GetWorkflowRunsResponseTypeDef,
     WorkflowTypeDef,
     BatchGetWorkflowsResponseTypeDef,
     GetWorkflowResponseTypeDef,
 )
 
 
-def get_structure() -> NotificationPropertyTypeDef:
+def get_structure() -> NotificationPropertyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-glue-1.28.1/README.md` & `mypy-boto3-glue-1.28.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-glue
+Version: 1.28.4
+Summary: Type annotations for boto3.Glue 1.28.4 service generated with mypy-boto3-builder 7.15.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 glue type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-glue"></a>
 
 # mypy-boto3-glue
 
 [![PyPI - mypy-boto3-glue](https://img.shields.io/pypi/v/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
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
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
 
@@ -440,62 +472,101 @@
 ### Typed dictionaries
 
 `mypy_boto3_glue.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glue.type_defs import (
+    NotificationPropertyOutputTypeDef,
     NotificationPropertyTypeDef,
+    AggregateOperationOutputTypeDef,
     AggregateOperationTypeDef,
+    AmazonRedshiftAdvancedOptionOutputTypeDef,
     AmazonRedshiftAdvancedOptionTypeDef,
+    OptionOutputTypeDef,
     OptionTypeDef,
+    ApplyMappingOutputTypeDef,
     ApplyMappingTypeDef,
     AuditContextTypeDef,
-    PartitionValueListTypeDef,
+    PartitionValueListOutputTypeDef,
+    BasicCatalogTargetOutputTypeDef,
     BasicCatalogTargetTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteConnectionRequestRequestTypeDef,
     ErrorDetailTypeDef,
+    PartitionValueListTypeDef,
     BatchDeleteTableRequestRequestTypeDef,
     BatchDeleteTableVersionRequestRequestTypeDef,
     BatchGetBlueprintsRequestRequestTypeDef,
     BatchGetCrawlersRequestRequestTypeDef,
     BatchGetCustomEntityTypesRequestRequestTypeDef,
     CustomEntityTypeTypeDef,
     BatchGetDataQualityResultRequestRequestTypeDef,
     BatchGetDevEndpointsRequestRequestTypeDef,
     DevEndpointTypeDef,
     BatchGetJobsRequestRequestTypeDef,
     BatchGetTriggersRequestRequestTypeDef,
     BatchGetWorkflowsRequestRequestTypeDef,
     BatchStopJobRunRequestRequestTypeDef,
     BatchStopJobRunSuccessfulSubmissionTypeDef,
+    BinaryColumnStatisticsDataOutputTypeDef,
     BinaryColumnStatisticsDataTypeDef,
     BlueprintDetailsTypeDef,
     BlueprintRunTypeDef,
     LastActiveDefinitionTypeDef,
+    BooleanColumnStatisticsDataOutputTypeDef,
     BooleanColumnStatisticsDataTypeDef,
     CancelDataQualityRuleRecommendationRunRequestRequestTypeDef,
     CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CancelMLTaskRunRequestRequestTypeDef,
     CancelStatementRequestRequestTypeDef,
     CatalogEntryTypeDef,
     CatalogImportStatusTypeDef,
+    KafkaStreamingSourceOptionsOutputTypeDef,
+    StreamingDataPreviewOptionsOutputTypeDef,
     KafkaStreamingSourceOptionsTypeDef,
     StreamingDataPreviewOptionsTypeDef,
+    KinesisStreamingSourceOptionsOutputTypeDef,
     KinesisStreamingSourceOptionsTypeDef,
+    CatalogSchemaChangePolicyOutputTypeDef,
     CatalogSchemaChangePolicyTypeDef,
+    CatalogSourceOutputTypeDef,
     CatalogSourceTypeDef,
+    CatalogTargetOutputTypeDef,
     CatalogTargetTypeDef,
     CheckSchemaVersionValidityInputRequestTypeDef,
     CsvClassifierTypeDef,
     GrokClassifierTypeDef,
     JsonClassifierTypeDef,
     XMLClassifierTypeDef,
+    CloudWatchEncryptionOutputTypeDef,
     CloudWatchEncryptionTypeDef,
+    DirectJDBCSourceOutputTypeDef,
+    DropDuplicatesOutputTypeDef,
+    DropFieldsOutputTypeDef,
+    DynamoDBCatalogSourceOutputTypeDef,
+    FillMissingValuesOutputTypeDef,
+    MergeOutputTypeDef,
+    MicrosoftSQLServerCatalogSourceOutputTypeDef,
+    MicrosoftSQLServerCatalogTargetOutputTypeDef,
+    MySQLCatalogSourceOutputTypeDef,
+    MySQLCatalogTargetOutputTypeDef,
+    OracleSQLCatalogSourceOutputTypeDef,
+    OracleSQLCatalogTargetOutputTypeDef,
+    PIIDetectionOutputTypeDef,
+    PostgreSQLCatalogSourceOutputTypeDef,
+    PostgreSQLCatalogTargetOutputTypeDef,
+    RedshiftSourceOutputTypeDef,
+    RelationalCatalogSourceOutputTypeDef,
+    RenameFieldOutputTypeDef,
+    SelectFieldsOutputTypeDef,
+    SelectFromCollectionOutputTypeDef,
+    SpigotOutputTypeDef,
+    SplitFieldsOutputTypeDef,
+    UnionOutputTypeDef,
     DirectJDBCSourceTypeDef,
     DropDuplicatesTypeDef,
     DropFieldsTypeDef,
     DynamoDBCatalogSourceTypeDef,
     FillMissingValuesTypeDef,
     MergeTypeDef,
     MicrosoftSQLServerCatalogSourceTypeDef,
@@ -511,71 +582,103 @@
     RelationalCatalogSourceTypeDef,
     RenameFieldTypeDef,
     SelectFieldsTypeDef,
     SelectFromCollectionTypeDef,
     SpigotTypeDef,
     SplitFieldsTypeDef,
     UnionTypeDef,
+    CodeGenEdgeOutputTypeDef,
     CodeGenEdgeTypeDef,
+    CodeGenNodeArgOutputTypeDef,
     CodeGenNodeArgTypeDef,
     ColumnImportanceTypeDef,
+    ColumnOutputTypeDef,
     ColumnRowFilterTypeDef,
+    DateColumnStatisticsDataOutputTypeDef,
+    DoubleColumnStatisticsDataOutputTypeDef,
+    LongColumnStatisticsDataOutputTypeDef,
+    StringColumnStatisticsDataOutputTypeDef,
     DateColumnStatisticsDataTypeDef,
     DoubleColumnStatisticsDataTypeDef,
     LongColumnStatisticsDataTypeDef,
     StringColumnStatisticsDataTypeDef,
     ColumnTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     ConfusionMatrixTypeDef,
     PhysicalConnectionRequirementsTypeDef,
+    ConnectionPasswordEncryptionOutputTypeDef,
     ConnectionPasswordEncryptionTypeDef,
+    PhysicalConnectionRequirementsOutputTypeDef,
+    ConnectionsListOutputTypeDef,
     ConnectionsListTypeDef,
     CrawlTypeDef,
     CrawlerHistoryTypeDef,
     CrawlerMetricsTypeDef,
+    DeltaTargetOutputTypeDef,
+    DynamoDBTargetOutputTypeDef,
+    IcebergTargetOutputTypeDef,
+    JdbcTargetOutputTypeDef,
+    MongoDBTargetOutputTypeDef,
+    S3TargetOutputTypeDef,
     DeltaTargetTypeDef,
     DynamoDBTargetTypeDef,
     IcebergTargetTypeDef,
     JdbcTargetTypeDef,
     MongoDBTargetTypeDef,
     S3TargetTypeDef,
-    LakeFormationConfigurationTypeDef,
+    LakeFormationConfigurationOutputTypeDef,
     LastCrawlInfoTypeDef,
-    LineageConfigurationTypeDef,
-    RecrawlPolicyTypeDef,
+    LineageConfigurationOutputTypeDef,
+    RecrawlPolicyOutputTypeDef,
     ScheduleTypeDef,
-    SchemaChangePolicyTypeDef,
+    SchemaChangePolicyOutputTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintRequestRequestTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateXMLClassifierRequestTypeDef,
+    LakeFormationConfigurationTypeDef,
+    LineageConfigurationTypeDef,
+    RecrawlPolicyTypeDef,
+    SchemaChangePolicyTypeDef,
     CreateCustomEntityTypeRequestRequestTypeDef,
     DataQualityTargetTableTypeDef,
     CreateDevEndpointRequestRequestTypeDef,
     ExecutionPropertyTypeDef,
     JobCommandTypeDef,
     SourceControlDetailsTypeDef,
     GlueTableTypeDef,
     PartitionIndexTypeDef,
     CreateRegistryInputRequestTypeDef,
     RegistryIdTypeDef,
     SessionCommandTypeDef,
     EventBatchingConditionTypeDef,
     CreateWorkflowRequestRequestTypeDef,
+    DQResultsPublishingOptionsOutputTypeDef,
     DQResultsPublishingOptionsTypeDef,
+    DQStopJobOnFailureOptionsOutputTypeDef,
     DQStopJobOnFailureOptionsTypeDef,
+    EncryptionAtRestOutputTypeDef,
     EncryptionAtRestTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
+    DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef,
     DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
     DataQualityRuleResultTypeDef,
+    DataQualityTargetTableOutputTypeDef,
+    GlueTableOutputTypeDef,
+    DatabaseIdentifierOutputTypeDef,
     DatabaseIdentifierTypeDef,
     FederatedDatabaseTypeDef,
+    FederatedDatabaseOutputTypeDef,
+    DatatypeOutputTypeDef,
     DatatypeTypeDef,
+    DecimalNumberOutputTypeDef,
     DecimalNumberTypeDef,
     DeleteBlueprintRequestRequestTypeDef,
     DeleteClassifierRequestRequestTypeDef,
     DeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     DeleteColumnStatisticsForTableRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteCrawlerRequestRequestTypeDef,
@@ -593,24 +696,33 @@
     DeleteSessionRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DeleteTableVersionRequestRequestTypeDef,
     DeleteTriggerRequestRequestTypeDef,
     DeleteUserDefinedFunctionRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DevEndpointCustomLibrariesTypeDef,
+    DirectSchemaChangePolicyOutputTypeDef,
     DirectSchemaChangePolicyTypeDef,
+    NullCheckBoxListOutputTypeDef,
     NullCheckBoxListTypeDef,
+    TransformConfigParameterOutputTypeDef,
     TransformConfigParameterTypeDef,
     EdgeTypeDef,
+    JobBookmarksEncryptionOutputTypeDef,
+    S3EncryptionOutputTypeDef,
     JobBookmarksEncryptionTypeDef,
     S3EncryptionTypeDef,
     ErrorDetailsTypeDef,
+    EventBatchingConditionOutputTypeDef,
+    ExecutionPropertyOutputTypeDef,
     ExportLabelsTaskRunPropertiesTypeDef,
     FederatedTableTypeDef,
+    FilterValueOutputTypeDef,
     FilterValueTypeDef,
+    FindMatchesParametersOutputTypeDef,
     FindMatchesParametersTypeDef,
     FindMatchesTaskRunPropertiesTypeDef,
     GetBlueprintRequestRequestTypeDef,
     GetBlueprintRunRequestRequestTypeDef,
     GetBlueprintRunsRequestRequestTypeDef,
     GetCatalogImportStatusRequestRequestTypeDef,
     GetClassifierRequestRequestTypeDef,
@@ -640,20 +752,21 @@
     GetJobRunRequestRequestTypeDef,
     GetJobRunsRequestRequestTypeDef,
     GetJobsRequestRequestTypeDef,
     GetMLTaskRunRequestRequestTypeDef,
     TaskRunFilterCriteriaTypeDef,
     TaskRunSortCriteriaTypeDef,
     GetMLTransformRequestRequestTypeDef,
-    SchemaColumnTypeDef,
+    SchemaColumnOutputTypeDef,
     TransformSortCriteriaTypeDef,
-    MappingEntryTypeDef,
+    MappingEntryOutputTypeDef,
     GetPartitionIndexesRequestRequestTypeDef,
     GetPartitionRequestRequestTypeDef,
     SegmentTypeDef,
+    MappingEntryTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GluePolicyTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     SchemaVersionNumberTypeDef,
     GetSecurityConfigurationRequestRequestTypeDef,
     GetSecurityConfigurationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
@@ -667,21 +780,27 @@
     GetTriggersRequestRequestTypeDef,
     GetUserDefinedFunctionRequestRequestTypeDef,
     GetUserDefinedFunctionsRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowRunPropertiesRequestRequestTypeDef,
     GetWorkflowRunRequestRequestTypeDef,
     GetWorkflowRunsRequestRequestTypeDef,
+    GlueStudioSchemaColumnOutputTypeDef,
     GlueStudioSchemaColumnTypeDef,
+    S3SourceAdditionalOptionsOutputTypeDef,
     S3SourceAdditionalOptionsTypeDef,
     IcebergInputTypeDef,
     ImportCatalogToGlueRequestRequestTypeDef,
     ImportLabelsTaskRunPropertiesTypeDef,
+    JDBCConnectorOptionsOutputTypeDef,
     JDBCConnectorOptionsTypeDef,
+    JobCommandOutputTypeDef,
     PredecessorTypeDef,
+    SourceControlDetailsOutputTypeDef,
+    JoinColumnOutputTypeDef,
     JoinColumnTypeDef,
     KeySchemaElementTypeDef,
     LabelingSetGenerationTaskRunPropertiesTypeDef,
     ListBlueprintsRequestRequestTypeDef,
     ListCrawlersRequestRequestTypeDef,
     ListCustomEntityTypesRequestRequestTypeDef,
     ListDevEndpointsRequestRequestTypeDef,
@@ -690,31 +809,43 @@
     RegistryListItemTypeDef,
     SchemaVersionListItemTypeDef,
     SchemaListItemTypeDef,
     ListSessionsRequestRequestTypeDef,
     ListStatementsRequestRequestTypeDef,
     ListTriggersRequestRequestTypeDef,
     ListWorkflowsRequestRequestTypeDef,
+    MLUserDataEncryptionOutputTypeDef,
     MLUserDataEncryptionTypeDef,
+    MappingOutputTypeDef,
     MappingTypeDef,
     OtherMetadataValueListItemTypeDef,
     MetadataKeyValuePairTypeDef,
+    OrderOutputTypeDef,
     OrderTypeDef,
     PropertyPredicateTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutWorkflowRunPropertiesRequestRequestTypeDef,
+    UpsertRedshiftTargetOptionsOutputTypeDef,
     UpsertRedshiftTargetOptionsTypeDef,
     ResetJobBookmarkRequestRequestTypeDef,
+    ResourceUriOutputTypeDef,
     ResourceUriTypeDef,
     ResumeWorkflowRunRequestRequestTypeDef,
     RunStatementRequestRequestTypeDef,
+    S3DirectSourceAdditionalOptionsOutputTypeDef,
     S3DirectSourceAdditionalOptionsTypeDef,
+    SchemaColumnTypeDef,
+    SchemaIdOutputTypeDef,
     SortCriterionTypeDef,
+    SerDeInfoOutputTypeDef,
     SerDeInfoTypeDef,
+    SessionCommandOutputTypeDef,
+    SkewedInfoOutputTypeDef,
     SkewedInfoTypeDef,
+    SqlAliasOutputTypeDef,
     SqlAliasTypeDef,
     StartBlueprintRunRequestRequestTypeDef,
     StartCrawlerRequestRequestTypeDef,
     StartCrawlerScheduleRequestRequestTypeDef,
     StartExportLabelsTaskRunRequestRequestTypeDef,
     StartImportLabelsTaskRunRequestRequestTypeDef,
     StartMLEvaluationTaskRunRequestRequestTypeDef,
@@ -724,37 +855,39 @@
     StartingEventBatchConditionTypeDef,
     StatementOutputDataTypeDef,
     StopCrawlerRequestRequestTypeDef,
     StopCrawlerScheduleRequestRequestTypeDef,
     StopSessionRequestRequestTypeDef,
     StopTriggerRequestRequestTypeDef,
     StopWorkflowRunRequestRequestTypeDef,
+    TableIdentifierOutputTypeDef,
     TableIdentifierTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBlueprintRequestRequestTypeDef,
     UpdateCsvClassifierRequestTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateXMLClassifierRequestTypeDef,
     UpdateCrawlerScheduleRequestRequestTypeDef,
     UpdateDataQualityRulesetRequestRequestTypeDef,
     UpdateJobFromSourceControlRequestRequestTypeDef,
     UpdateSourceControlFromJobRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     WorkflowRunStatisticsTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     StartJobRunRequestRequestTypeDef,
+    AggregateOutputTypeDef,
     AggregateTypeDef,
+    AmazonRedshiftNodeDataOutputTypeDef,
     AmazonRedshiftNodeDataTypeDef,
     GetUnfilteredPartitionMetadataRequestRequestTypeDef,
     GetUnfilteredTableMetadataRequestRequestTypeDef,
     BackfillErrorTypeDef,
-    BatchDeletePartitionRequestRequestTypeDef,
-    BatchGetPartitionRequestRequestTypeDef,
     CancelMLTaskRunResponseTypeDef,
     CheckSchemaVersionValidityResponseTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
     CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateJobResponseTypeDef,
@@ -821,78 +954,104 @@
     BatchDeleteConnectionResponseTypeDef,
     BatchStopJobRunErrorTypeDef,
     BatchUpdatePartitionFailureEntryTypeDef,
     ColumnErrorTypeDef,
     PartitionErrorTypeDef,
     TableErrorTypeDef,
     TableVersionErrorTypeDef,
+    BatchDeletePartitionRequestRequestTypeDef,
+    BatchGetPartitionRequestRequestTypeDef,
     BatchGetCustomEntityTypesResponseTypeDef,
     ListCustomEntityTypesResponseTypeDef,
     BatchGetDevEndpointsResponseTypeDef,
     GetDevEndpointResponseTypeDef,
     GetDevEndpointsResponseTypeDef,
     GetBlueprintRunResponseTypeDef,
     GetBlueprintRunsResponseTypeDef,
     BlueprintTypeDef,
     GetCatalogImportStatusResponseTypeDef,
+    CatalogKafkaSourceOutputTypeDef,
+    DirectKafkaSourceOutputTypeDef,
     CatalogKafkaSourceTypeDef,
     DirectKafkaSourceTypeDef,
+    CatalogKinesisSourceOutputTypeDef,
+    DirectKinesisSourceOutputTypeDef,
     CatalogKinesisSourceTypeDef,
     DirectKinesisSourceTypeDef,
+    GovernedCatalogTargetOutputTypeDef,
+    S3CatalogTargetOutputTypeDef,
+    S3DeltaCatalogTargetOutputTypeDef,
+    S3HudiCatalogTargetOutputTypeDef,
     GovernedCatalogTargetTypeDef,
     S3CatalogTargetTypeDef,
     S3DeltaCatalogTargetTypeDef,
     S3HudiCatalogTargetTypeDef,
     ClassifierTypeDef,
+    CodeGenNodeOutputTypeDef,
     CodeGenNodeTypeDef,
     LocationTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     FindMatchesMetricsTypeDef,
     ConnectionInputTypeDef,
     ConnectionTypeDef,
     CrawlerNodeDetailsTypeDef,
     ListCrawlsResponseTypeDef,
     GetCrawlerMetricsResponseTypeDef,
+    CrawlerTargetsOutputTypeDef,
     CrawlerTargetsTypeDef,
     ListCrawlsRequestRequestTypeDef,
     CreateClassifierRequestRequestTypeDef,
     CreateDataQualityRulesetRequestRequestTypeDef,
     DataQualityRulesetFilterCriteriaTypeDef,
-    DataQualityRulesetListDetailsTypeDef,
-    GetDataQualityRulesetResponseTypeDef,
     DataSourceTypeDef,
     CreatePartitionIndexRequestRequestTypeDef,
     CreateSchemaInputRequestTypeDef,
     DeleteRegistryInputRequestTypeDef,
     GetRegistryInputRequestTypeDef,
     ListSchemasInputRequestTypeDef,
     UpdateRegistryInputRequestTypeDef,
     CreateSessionRequestRequestTypeDef,
-    SessionTypeDef,
+    EvaluateDataQualityMultiFrameOutputTypeDef,
+    EvaluateDataQualityOutputTypeDef,
     EvaluateDataQualityMultiFrameTypeDef,
     EvaluateDataQualityTypeDef,
+    DataCatalogEncryptionSettingsOutputTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
+    PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    DataQualityRulesetListDetailsTypeDef,
+    GetDataQualityRulesetResponseTypeDef,
+    DataSourceOutputTypeDef,
+    NullValueFieldOutputTypeDef,
     NullValueFieldTypeDef,
+    DecimalColumnStatisticsDataOutputTypeDef,
     DecimalColumnStatisticsDataTypeDef,
     DeleteSchemaInputRequestTypeDef,
     DeleteSchemaVersionsInputRequestTypeDef,
     GetSchemaByDefinitionInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     ListSchemaVersionsInputRequestTypeDef,
     RegisterSchemaVersionInputRequestTypeDef,
     SchemaReferenceTypeDef,
     UpdateDevEndpointRequestRequestTypeDef,
+    S3DeltaDirectTargetOutputTypeDef,
+    S3DirectTargetOutputTypeDef,
+    S3GlueParquetTargetOutputTypeDef,
+    S3HudiDirectTargetOutputTypeDef,
     S3DeltaDirectTargetTypeDef,
     S3DirectTargetTypeDef,
     S3GlueParquetTargetTypeDef,
     S3HudiDirectTargetTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     SchemaVersionErrorItemTypeDef,
+    FilterExpressionOutputTypeDef,
     FilterExpressionTypeDef,
+    TransformParametersOutputTypeDef,
     TransformParametersTypeDef,
     GetClassifiersRequestGetClassifiersPaginateTypeDef,
     GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
     GetCrawlersRequestGetCrawlersPaginateTypeDef,
     GetDatabasesRequestGetDatabasesPaginateTypeDef,
     GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef,
     GetJobRunsRequestGetJobRunsPaginateTypeDef,
@@ -908,103 +1067,128 @@
     ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     ListSchemasInputListSchemasPaginateTypeDef,
     GetConnectionsRequestGetConnectionsPaginateTypeDef,
     GetConnectionsRequestRequestTypeDef,
     GetJobBookmarkResponseTypeDef,
     ResetJobBookmarkResponseTypeDef,
     GetMLTaskRunsRequestRequestTypeDef,
-    TransformFilterCriteriaTypeDef,
     GetMappingResponseTypeDef,
     GetPartitionsRequestGetPartitionsPaginateTypeDef,
     GetPartitionsRequestRequestTypeDef,
     GetUnfilteredPartitionsMetadataRequestRequestTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetSchemaVersionInputRequestTypeDef,
     GetSchemaVersionsDiffInputRequestTypeDef,
     UpdateSchemaInputRequestTypeDef,
+    GlueSchemaOutputTypeDef,
     GlueSchemaTypeDef,
+    GovernedCatalogSourceOutputTypeDef,
+    S3CatalogSourceOutputTypeDef,
     GovernedCatalogSourceTypeDef,
     S3CatalogSourceTypeDef,
     OpenTableFormatInputTypeDef,
     JobRunTypeDef,
+    JoinOutputTypeDef,
     JoinTypeDef,
     TaskRunPropertiesTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
+    TransformEncryptionOutputTypeDef,
     TransformEncryptionTypeDef,
     MetadataInfoTypeDef,
     PutSchemaVersionMetadataInputRequestTypeDef,
     QuerySchemaVersionMetadataInputRequestTypeDef,
     RemoveSchemaVersionMetadataInputRequestTypeDef,
+    RedshiftTargetOutputTypeDef,
     RedshiftTargetTypeDef,
-    UserDefinedFunctionInputTypeDef,
     UserDefinedFunctionTypeDef,
+    UserDefinedFunctionInputTypeDef,
+    TransformFilterCriteriaTypeDef,
+    SchemaReferenceOutputTypeDef,
     SearchTablesRequestRequestTypeDef,
+    SessionTypeDef,
     StatementOutputTypeDef,
     UpdateClassifierRequestRequestTypeDef,
+    AmazonRedshiftSourceOutputTypeDef,
+    AmazonRedshiftTargetOutputTypeDef,
     AmazonRedshiftSourceTypeDef,
     AmazonRedshiftTargetTypeDef,
     PartitionIndexDescriptorTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionResponseTypeDef,
     BatchCreatePartitionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
     BatchGetBlueprintsResponseTypeDef,
     GetBlueprintResponseTypeDef,
     GetClassifierResponseTypeDef,
     GetClassifiersResponseTypeDef,
-    CreateScriptRequestRequestTypeDef,
     GetDataflowGraphResponseTypeDef,
+    CreateScriptRequestRequestTypeDef,
     GetMappingRequestRequestTypeDef,
     GetPlanRequestRequestTypeDef,
-    CreateTriggerRequestRequestTypeDef,
     TriggerTypeDef,
+    CreateTriggerRequestRequestTypeDef,
     TriggerUpdateTypeDef,
     EvaluationMetricsTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     GetConnectionResponseTypeDef,
     GetConnectionsResponseTypeDef,
     CrawlerTypeDef,
     CreateCrawlerRequestRequestTypeDef,
     UpdateCrawlerRequestRequestTypeDef,
     ListDataQualityRulesetsRequestRequestTypeDef,
-    ListDataQualityRulesetsResponseTypeDef,
-    DataQualityResultDescriptionTypeDef,
     DataQualityResultFilterCriteriaTypeDef,
-    DataQualityResultTypeDef,
-    DataQualityRuleRecommendationRunDescriptionTypeDef,
     DataQualityRuleRecommendationRunFilterTypeDef,
-    DataQualityRulesetEvaluationRunDescriptionTypeDef,
     DataQualityRulesetEvaluationRunFilterTypeDef,
-    GetDataQualityResultResponseTypeDef,
-    GetDataQualityRuleRecommendationRunResponseTypeDef,
-    GetDataQualityRulesetEvaluationRunResponseTypeDef,
     StartDataQualityRuleRecommendationRunRequestRequestTypeDef,
     StartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-    CreateSessionResponseTypeDef,
-    GetSessionResponseTypeDef,
-    ListSessionsResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     PutDataCatalogEncryptionSettingsRequestRequestTypeDef,
-    DatabaseInputTypeDef,
     DatabaseTypeDef,
+    DatabaseInputTypeDef,
+    ListDataQualityRulesetsResponseTypeDef,
+    DataQualityResultDescriptionTypeDef,
+    DataQualityResultTypeDef,
+    DataQualityRuleRecommendationRunDescriptionTypeDef,
+    DataQualityRulesetEvaluationRunDescriptionTypeDef,
+    GetDataQualityResultResponseTypeDef,
+    GetDataQualityRuleRecommendationRunResponseTypeDef,
+    GetDataQualityRulesetEvaluationRunResponseTypeDef,
+    DropNullFieldsOutputTypeDef,
     DropNullFieldsTypeDef,
+    ColumnStatisticsDataOutputTypeDef,
     ColumnStatisticsDataTypeDef,
     StorageDescriptorTypeDef,
-    CreateSecurityConfigurationRequestRequestTypeDef,
     SecurityConfigurationTypeDef,
+    CreateSecurityConfigurationRequestRequestTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
     UpdateMLTransformRequestRequestTypeDef,
-    GetMLTransformsRequestRequestTypeDef,
-    ListMLTransformsRequestRequestTypeDef,
+    AthenaConnectorSourceOutputTypeDef,
+    CatalogDeltaSourceOutputTypeDef,
+    CatalogHudiSourceOutputTypeDef,
+    CustomCodeOutputTypeDef,
+    DynamicTransformOutputTypeDef,
+    JDBCConnectorSourceOutputTypeDef,
+    JDBCConnectorTargetOutputTypeDef,
+    S3CatalogDeltaSourceOutputTypeDef,
+    S3CatalogHudiSourceOutputTypeDef,
+    S3CsvSourceOutputTypeDef,
+    S3DeltaSourceOutputTypeDef,
+    S3HudiSourceOutputTypeDef,
+    S3JsonSourceOutputTypeDef,
+    S3ParquetSourceOutputTypeDef,
+    SparkConnectorSourceOutputTypeDef,
+    SparkConnectorTargetOutputTypeDef,
+    SparkSQLOutputTypeDef,
     AthenaConnectorSourceTypeDef,
     CatalogDeltaSourceTypeDef,
     CatalogHudiSourceTypeDef,
     CustomCodeTypeDef,
     DynamicTransformTypeDef,
     JDBCConnectorSourceTypeDef,
     JDBCConnectorTargetTypeDef,
@@ -1021,100 +1205,108 @@
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
     JobNodeDetailsTypeDef,
     GetMLTaskRunResponseTypeDef,
     TaskRunTypeDef,
     CreateMLTransformRequestRequestTypeDef,
     QuerySchemaVersionMetadataResponseTypeDef,
-    CreateUserDefinedFunctionRequestRequestTypeDef,
-    UpdateUserDefinedFunctionRequestRequestTypeDef,
     GetUserDefinedFunctionResponseTypeDef,
     GetUserDefinedFunctionsResponseTypeDef,
+    CreateUserDefinedFunctionRequestRequestTypeDef,
+    UpdateUserDefinedFunctionRequestRequestTypeDef,
+    GetMLTransformsRequestRequestTypeDef,
+    ListMLTransformsRequestRequestTypeDef,
+    StorageDescriptorOutputTypeDef,
+    CreateSessionResponseTypeDef,
+    GetSessionResponseTypeDef,
+    ListSessionsResponseTypeDef,
     StatementTypeDef,
     GetPartitionIndexesResponseTypeDef,
     BatchGetTriggersResponseTypeDef,
     GetTriggerResponseTypeDef,
     GetTriggersResponseTypeDef,
     TriggerNodeDetailsTypeDef,
     UpdateTriggerResponseTypeDef,
     UpdateTriggerRequestRequestTypeDef,
     GetMLTransformResponseTypeDef,
     MLTransformTypeDef,
     BatchGetCrawlersResponseTypeDef,
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
-    ListDataQualityResultsResponseTypeDef,
     ListDataQualityResultsRequestRequestTypeDef,
-    BatchGetDataQualityResultResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsResponseTypeDef,
     ListDataQualityRuleRecommendationRunsRequestRequestTypeDef,
-    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
     ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef,
-    CreateDatabaseRequestRequestTypeDef,
-    UpdateDatabaseRequestRequestTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
+    CreateDatabaseRequestRequestTypeDef,
+    UpdateDatabaseRequestRequestTypeDef,
+    ListDataQualityResultsResponseTypeDef,
+    BatchGetDataQualityResultResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsResponseTypeDef,
+    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
+    ColumnStatisticsOutputTypeDef,
     ColumnStatisticsTypeDef,
     PartitionInputTypeDef,
-    PartitionTypeDef,
     TableInputTypeDef,
-    TableTypeDef,
     GetSecurityConfigurationResponseTypeDef,
     GetSecurityConfigurationsResponseTypeDef,
+    CodeGenConfigurationNodeOutputTypeDef,
     CodeGenConfigurationNodeTypeDef,
     GetMLTaskRunsResponseTypeDef,
+    PartitionTypeDef,
+    TableTypeDef,
     GetStatementResponseTypeDef,
     ListStatementsResponseTypeDef,
     NodeTypeDef,
     GetMLTransformsResponseTypeDef,
     ColumnStatisticsErrorTypeDef,
     GetColumnStatisticsForPartitionResponseTypeDef,
     GetColumnStatisticsForTableResponseTypeDef,
     UpdateColumnStatisticsForPartitionRequestRequestTypeDef,
     UpdateColumnStatisticsForTableRequestRequestTypeDef,
     BatchCreatePartitionRequestRequestTypeDef,
     BatchUpdatePartitionRequestEntryTypeDef,
     CreatePartitionRequestRequestTypeDef,
     UpdatePartitionRequestRequestTypeDef,
+    CreateTableRequestRequestTypeDef,
+    UpdateTableRequestRequestTypeDef,
+    JobTypeDef,
+    CreateJobRequestRequestTypeDef,
+    JobUpdateTypeDef,
     BatchGetPartitionResponseTypeDef,
     GetPartitionResponseTypeDef,
     GetPartitionsResponseTypeDef,
     GetUnfilteredPartitionMetadataResponseTypeDef,
     UnfilteredPartitionTypeDef,
-    CreateTableRequestRequestTypeDef,
-    UpdateTableRequestRequestTypeDef,
     GetTableResponseTypeDef,
     GetTablesResponseTypeDef,
     GetUnfilteredTableMetadataResponseTypeDef,
     SearchTablesResponseTypeDef,
     TableVersionTypeDef,
-    CreateJobRequestRequestTypeDef,
-    JobTypeDef,
-    JobUpdateTypeDef,
     WorkflowGraphTypeDef,
     UpdateColumnStatisticsForPartitionResponseTypeDef,
     UpdateColumnStatisticsForTableResponseTypeDef,
     BatchUpdatePartitionRequestRequestTypeDef,
-    GetUnfilteredPartitionsMetadataResponseTypeDef,
-    GetTableVersionResponseTypeDef,
-    GetTableVersionsResponseTypeDef,
     BatchGetJobsResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobsResponseTypeDef,
     UpdateJobRequestRequestTypeDef,
+    GetUnfilteredPartitionsMetadataResponseTypeDef,
+    GetTableVersionResponseTypeDef,
+    GetTableVersionsResponseTypeDef,
     WorkflowRunTypeDef,
     GetWorkflowRunResponseTypeDef,
     GetWorkflowRunsResponseTypeDef,
     WorkflowTypeDef,
     BatchGetWorkflowsResponseTypeDef,
     GetWorkflowResponseTypeDef,
 )
 
 
-def get_structure() -> NotificationPropertyTypeDef:
+def get_structure() -> NotificationPropertyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/__init__.py` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/__init__.pyi` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/__main__.py` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glue 1.28.1\nVersion:         1.28.1\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Glue 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.1")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/client.py` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/client.pyi` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/literals.py` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AdditionalOptionKeysType",
     "AggFunctionType",
     "BackfillErrorCodeType",
     "BlueprintRunStateType",
     "BlueprintStatusType",
     "CatalogEncryptionModeType",
@@ -128,15 +127,14 @@
     "GlueServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdditionalOptionKeysType = Literal["performanceTuning.caching"]
 AggFunctionType = Literal[
     "avg",
     "count",
     "countDistinct",
     "first",
     "kurtosis",
@@ -320,15 +318,17 @@
     "CREATE_TABLE",
     "DATA_LOCATION_ACCESS",
     "DELETE",
     "DROP",
     "INSERT",
     "SELECT",
 ]
-PermissionTypeType = Literal["CELL_FILTER_PERMISSION", "COLUMN_PERMISSION"]
+PermissionTypeType = Literal[
+    "CELL_FILTER_PERMISSION", "COLUMN_PERMISSION", "NESTED_CELL_PERMISSION", "NESTED_PERMISSION"
+]
 PiiTypeType = Literal["ColumnAudit", "ColumnMasking", "RowAudit", "RowMasking"]
 PrincipalTypeType = Literal["GROUP", "ROLE", "USER"]
 QuoteCharType = Literal["disabled", "quillemet", "quote", "single_quote"]
 RecrawlBehaviorType = Literal["CRAWL_EVENT_MODE", "CRAWL_EVERYTHING", "CRAWL_NEW_FOLDERS_ONLY"]
 RegistryStatusType = Literal["AVAILABLE", "DELETING"]
 ResourceShareTypeType = Literal["ALL", "FEDERATED", "FOREIGN"]
 ResourceTypeType = Literal["ARCHIVE", "FILE", "JAR"]
```

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/literals.pyi` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AdditionalOptionKeysType",
     "AggFunctionType",
     "BackfillErrorCodeType",
     "BlueprintRunStateType",
     "BlueprintStatusType",
     "CatalogEncryptionModeType",
@@ -127,14 +128,15 @@
     "GlueServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AdditionalOptionKeysType = Literal["performanceTuning.caching"]
 AggFunctionType = Literal[
     "avg",
     "count",
     "countDistinct",
     "first",
     "kurtosis",
@@ -318,15 +320,17 @@
     "CREATE_TABLE",
     "DATA_LOCATION_ACCESS",
     "DELETE",
     "DROP",
     "INSERT",
     "SELECT",
 ]
-PermissionTypeType = Literal["CELL_FILTER_PERMISSION", "COLUMN_PERMISSION"]
+PermissionTypeType = Literal[
+    "CELL_FILTER_PERMISSION", "COLUMN_PERMISSION", "NESTED_CELL_PERMISSION", "NESTED_PERMISSION"
+]
 PiiTypeType = Literal["ColumnAudit", "ColumnMasking", "RowAudit", "RowMasking"]
 PrincipalTypeType = Literal["GROUP", "ROLE", "USER"]
 QuoteCharType = Literal["disabled", "quillemet", "quote", "single_quote"]
 RecrawlBehaviorType = Literal["CRAWL_EVENT_MODE", "CRAWL_EVERYTHING", "CRAWL_NEW_FOLDERS_ONLY"]
 RegistryStatusType = Literal["AVAILABLE", "DELETING"]
 ResourceShareTypeType = Literal["ALL", "FEDERATED", "FOREIGN"]
 ResourceTypeType = Literal["ARCHIVE", "FILE", "JAR"]
```

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/paginator.py` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/paginator.pyi` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/type_defs.py` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 Type annotations for glue service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_glue.type_defs import NotificationPropertyTypeDef
+    from mypy_boto3_glue.type_defs import NotificationPropertyOutputTypeDef
 
-    data: NotificationPropertyTypeDef = {...}
+    data: NotificationPropertyOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
+
+from botocore.response import StreamingBody
 
 from .literals import (
     AggFunctionType,
     BackfillErrorCodeType,
     BlueprintRunStateType,
     BlueprintStatusType,
     CatalogEncryptionModeType,
@@ -104,64 +106,102 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "NotificationPropertyOutputTypeDef",
     "NotificationPropertyTypeDef",
+    "AggregateOperationOutputTypeDef",
     "AggregateOperationTypeDef",
+    "AmazonRedshiftAdvancedOptionOutputTypeDef",
     "AmazonRedshiftAdvancedOptionTypeDef",
+    "OptionOutputTypeDef",
     "OptionTypeDef",
+    "ApplyMappingOutputTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
-    "PartitionValueListTypeDef",
+    "PartitionValueListOutputTypeDef",
+    "BasicCatalogTargetOutputTypeDef",
     "BasicCatalogTargetTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteConnectionRequestRequestTypeDef",
     "ErrorDetailTypeDef",
+    "PartitionValueListTypeDef",
     "BatchDeleteTableRequestRequestTypeDef",
     "BatchDeleteTableVersionRequestRequestTypeDef",
     "BatchGetBlueprintsRequestRequestTypeDef",
     "BatchGetCrawlersRequestRequestTypeDef",
     "BatchGetCustomEntityTypesRequestRequestTypeDef",
     "CustomEntityTypeTypeDef",
     "BatchGetDataQualityResultRequestRequestTypeDef",
     "BatchGetDevEndpointsRequestRequestTypeDef",
     "DevEndpointTypeDef",
     "BatchGetJobsRequestRequestTypeDef",
     "BatchGetTriggersRequestRequestTypeDef",
     "BatchGetWorkflowsRequestRequestTypeDef",
     "BatchStopJobRunRequestRequestTypeDef",
     "BatchStopJobRunSuccessfulSubmissionTypeDef",
+    "BinaryColumnStatisticsDataOutputTypeDef",
     "BinaryColumnStatisticsDataTypeDef",
     "BlueprintDetailsTypeDef",
     "BlueprintRunTypeDef",
     "LastActiveDefinitionTypeDef",
+    "BooleanColumnStatisticsDataOutputTypeDef",
     "BooleanColumnStatisticsDataTypeDef",
     "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
     "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CancelMLTaskRunRequestRequestTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "CatalogEntryTypeDef",
     "CatalogImportStatusTypeDef",
+    "KafkaStreamingSourceOptionsOutputTypeDef",
+    "StreamingDataPreviewOptionsOutputTypeDef",
     "KafkaStreamingSourceOptionsTypeDef",
     "StreamingDataPreviewOptionsTypeDef",
+    "KinesisStreamingSourceOptionsOutputTypeDef",
     "KinesisStreamingSourceOptionsTypeDef",
+    "CatalogSchemaChangePolicyOutputTypeDef",
     "CatalogSchemaChangePolicyTypeDef",
+    "CatalogSourceOutputTypeDef",
     "CatalogSourceTypeDef",
+    "CatalogTargetOutputTypeDef",
     "CatalogTargetTypeDef",
     "CheckSchemaVersionValidityInputRequestTypeDef",
     "CsvClassifierTypeDef",
     "GrokClassifierTypeDef",
     "JsonClassifierTypeDef",
     "XMLClassifierTypeDef",
+    "CloudWatchEncryptionOutputTypeDef",
     "CloudWatchEncryptionTypeDef",
+    "DirectJDBCSourceOutputTypeDef",
+    "DropDuplicatesOutputTypeDef",
+    "DropFieldsOutputTypeDef",
+    "DynamoDBCatalogSourceOutputTypeDef",
+    "FillMissingValuesOutputTypeDef",
+    "MergeOutputTypeDef",
+    "MicrosoftSQLServerCatalogSourceOutputTypeDef",
+    "MicrosoftSQLServerCatalogTargetOutputTypeDef",
+    "MySQLCatalogSourceOutputTypeDef",
+    "MySQLCatalogTargetOutputTypeDef",
+    "OracleSQLCatalogSourceOutputTypeDef",
+    "OracleSQLCatalogTargetOutputTypeDef",
+    "PIIDetectionOutputTypeDef",
+    "PostgreSQLCatalogSourceOutputTypeDef",
+    "PostgreSQLCatalogTargetOutputTypeDef",
+    "RedshiftSourceOutputTypeDef",
+    "RelationalCatalogSourceOutputTypeDef",
+    "RenameFieldOutputTypeDef",
+    "SelectFieldsOutputTypeDef",
+    "SelectFromCollectionOutputTypeDef",
+    "SpigotOutputTypeDef",
+    "SplitFieldsOutputTypeDef",
+    "UnionOutputTypeDef",
     "DirectJDBCSourceTypeDef",
     "DropDuplicatesTypeDef",
     "DropFieldsTypeDef",
     "DynamoDBCatalogSourceTypeDef",
     "FillMissingValuesTypeDef",
     "MergeTypeDef",
     "MicrosoftSQLServerCatalogSourceTypeDef",
@@ -177,71 +217,103 @@
     "RelationalCatalogSourceTypeDef",
     "RenameFieldTypeDef",
     "SelectFieldsTypeDef",
     "SelectFromCollectionTypeDef",
     "SpigotTypeDef",
     "SplitFieldsTypeDef",
     "UnionTypeDef",
+    "CodeGenEdgeOutputTypeDef",
     "CodeGenEdgeTypeDef",
+    "CodeGenNodeArgOutputTypeDef",
     "CodeGenNodeArgTypeDef",
     "ColumnImportanceTypeDef",
+    "ColumnOutputTypeDef",
     "ColumnRowFilterTypeDef",
+    "DateColumnStatisticsDataOutputTypeDef",
+    "DoubleColumnStatisticsDataOutputTypeDef",
+    "LongColumnStatisticsDataOutputTypeDef",
+    "StringColumnStatisticsDataOutputTypeDef",
     "DateColumnStatisticsDataTypeDef",
     "DoubleColumnStatisticsDataTypeDef",
     "LongColumnStatisticsDataTypeDef",
     "StringColumnStatisticsDataTypeDef",
     "ColumnTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "ConfusionMatrixTypeDef",
     "PhysicalConnectionRequirementsTypeDef",
+    "ConnectionPasswordEncryptionOutputTypeDef",
     "ConnectionPasswordEncryptionTypeDef",
+    "PhysicalConnectionRequirementsOutputTypeDef",
+    "ConnectionsListOutputTypeDef",
     "ConnectionsListTypeDef",
     "CrawlTypeDef",
     "CrawlerHistoryTypeDef",
     "CrawlerMetricsTypeDef",
+    "DeltaTargetOutputTypeDef",
+    "DynamoDBTargetOutputTypeDef",
+    "IcebergTargetOutputTypeDef",
+    "JdbcTargetOutputTypeDef",
+    "MongoDBTargetOutputTypeDef",
+    "S3TargetOutputTypeDef",
     "DeltaTargetTypeDef",
     "DynamoDBTargetTypeDef",
     "IcebergTargetTypeDef",
     "JdbcTargetTypeDef",
     "MongoDBTargetTypeDef",
     "S3TargetTypeDef",
-    "LakeFormationConfigurationTypeDef",
+    "LakeFormationConfigurationOutputTypeDef",
     "LastCrawlInfoTypeDef",
-    "LineageConfigurationTypeDef",
-    "RecrawlPolicyTypeDef",
+    "LineageConfigurationOutputTypeDef",
+    "RecrawlPolicyOutputTypeDef",
     "ScheduleTypeDef",
-    "SchemaChangePolicyTypeDef",
+    "SchemaChangePolicyOutputTypeDef",
     "CrawlsFilterTypeDef",
     "CreateBlueprintRequestRequestTypeDef",
     "CreateCsvClassifierRequestTypeDef",
     "CreateGrokClassifierRequestTypeDef",
     "CreateJsonClassifierRequestTypeDef",
     "CreateXMLClassifierRequestTypeDef",
+    "LakeFormationConfigurationTypeDef",
+    "LineageConfigurationTypeDef",
+    "RecrawlPolicyTypeDef",
+    "SchemaChangePolicyTypeDef",
     "CreateCustomEntityTypeRequestRequestTypeDef",
     "DataQualityTargetTableTypeDef",
     "CreateDevEndpointRequestRequestTypeDef",
     "ExecutionPropertyTypeDef",
     "JobCommandTypeDef",
     "SourceControlDetailsTypeDef",
     "GlueTableTypeDef",
     "PartitionIndexTypeDef",
     "CreateRegistryInputRequestTypeDef",
     "RegistryIdTypeDef",
     "SessionCommandTypeDef",
     "EventBatchingConditionTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
+    "DQResultsPublishingOptionsOutputTypeDef",
     "DQResultsPublishingOptionsTypeDef",
+    "DQStopJobOnFailureOptionsOutputTypeDef",
     "DQStopJobOnFailureOptionsTypeDef",
+    "EncryptionAtRestOutputTypeDef",
     "EncryptionAtRestTypeDef",
+    "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
+    "DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef",
     "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
     "DataQualityRuleResultTypeDef",
+    "DataQualityTargetTableOutputTypeDef",
+    "GlueTableOutputTypeDef",
+    "DatabaseIdentifierOutputTypeDef",
     "DatabaseIdentifierTypeDef",
     "FederatedDatabaseTypeDef",
+    "FederatedDatabaseOutputTypeDef",
+    "DatatypeOutputTypeDef",
     "DatatypeTypeDef",
+    "DecimalNumberOutputTypeDef",
     "DecimalNumberTypeDef",
     "DeleteBlueprintRequestRequestTypeDef",
     "DeleteClassifierRequestRequestTypeDef",
     "DeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     "DeleteColumnStatisticsForTableRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteCrawlerRequestRequestTypeDef",
@@ -259,24 +331,33 @@
     "DeleteSessionRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DeleteTableVersionRequestRequestTypeDef",
     "DeleteTriggerRequestRequestTypeDef",
     "DeleteUserDefinedFunctionRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DevEndpointCustomLibrariesTypeDef",
+    "DirectSchemaChangePolicyOutputTypeDef",
     "DirectSchemaChangePolicyTypeDef",
+    "NullCheckBoxListOutputTypeDef",
     "NullCheckBoxListTypeDef",
+    "TransformConfigParameterOutputTypeDef",
     "TransformConfigParameterTypeDef",
     "EdgeTypeDef",
+    "JobBookmarksEncryptionOutputTypeDef",
+    "S3EncryptionOutputTypeDef",
     "JobBookmarksEncryptionTypeDef",
     "S3EncryptionTypeDef",
     "ErrorDetailsTypeDef",
+    "EventBatchingConditionOutputTypeDef",
+    "ExecutionPropertyOutputTypeDef",
     "ExportLabelsTaskRunPropertiesTypeDef",
     "FederatedTableTypeDef",
+    "FilterValueOutputTypeDef",
     "FilterValueTypeDef",
+    "FindMatchesParametersOutputTypeDef",
     "FindMatchesParametersTypeDef",
     "FindMatchesTaskRunPropertiesTypeDef",
     "GetBlueprintRequestRequestTypeDef",
     "GetBlueprintRunRequestRequestTypeDef",
     "GetBlueprintRunsRequestRequestTypeDef",
     "GetCatalogImportStatusRequestRequestTypeDef",
     "GetClassifierRequestRequestTypeDef",
@@ -306,20 +387,21 @@
     "GetJobRunRequestRequestTypeDef",
     "GetJobRunsRequestRequestTypeDef",
     "GetJobsRequestRequestTypeDef",
     "GetMLTaskRunRequestRequestTypeDef",
     "TaskRunFilterCriteriaTypeDef",
     "TaskRunSortCriteriaTypeDef",
     "GetMLTransformRequestRequestTypeDef",
-    "SchemaColumnTypeDef",
+    "SchemaColumnOutputTypeDef",
     "TransformSortCriteriaTypeDef",
-    "MappingEntryTypeDef",
+    "MappingEntryOutputTypeDef",
     "GetPartitionIndexesRequestRequestTypeDef",
     "GetPartitionRequestRequestTypeDef",
     "SegmentTypeDef",
+    "MappingEntryTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GluePolicyTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "SchemaVersionNumberTypeDef",
     "GetSecurityConfigurationRequestRequestTypeDef",
     "GetSecurityConfigurationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
@@ -333,21 +415,27 @@
     "GetTriggersRequestRequestTypeDef",
     "GetUserDefinedFunctionRequestRequestTypeDef",
     "GetUserDefinedFunctionsRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     "GetWorkflowRunRequestRequestTypeDef",
     "GetWorkflowRunsRequestRequestTypeDef",
+    "GlueStudioSchemaColumnOutputTypeDef",
     "GlueStudioSchemaColumnTypeDef",
+    "S3SourceAdditionalOptionsOutputTypeDef",
     "S3SourceAdditionalOptionsTypeDef",
     "IcebergInputTypeDef",
     "ImportCatalogToGlueRequestRequestTypeDef",
     "ImportLabelsTaskRunPropertiesTypeDef",
+    "JDBCConnectorOptionsOutputTypeDef",
     "JDBCConnectorOptionsTypeDef",
+    "JobCommandOutputTypeDef",
     "PredecessorTypeDef",
+    "SourceControlDetailsOutputTypeDef",
+    "JoinColumnOutputTypeDef",
     "JoinColumnTypeDef",
     "KeySchemaElementTypeDef",
     "LabelingSetGenerationTaskRunPropertiesTypeDef",
     "ListBlueprintsRequestRequestTypeDef",
     "ListCrawlersRequestRequestTypeDef",
     "ListCustomEntityTypesRequestRequestTypeDef",
     "ListDevEndpointsRequestRequestTypeDef",
@@ -356,31 +444,43 @@
     "RegistryListItemTypeDef",
     "SchemaVersionListItemTypeDef",
     "SchemaListItemTypeDef",
     "ListSessionsRequestRequestTypeDef",
     "ListStatementsRequestRequestTypeDef",
     "ListTriggersRequestRequestTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
+    "MLUserDataEncryptionOutputTypeDef",
     "MLUserDataEncryptionTypeDef",
+    "MappingOutputTypeDef",
     "MappingTypeDef",
     "OtherMetadataValueListItemTypeDef",
     "MetadataKeyValuePairTypeDef",
+    "OrderOutputTypeDef",
     "OrderTypeDef",
     "PropertyPredicateTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
+    "UpsertRedshiftTargetOptionsOutputTypeDef",
     "UpsertRedshiftTargetOptionsTypeDef",
     "ResetJobBookmarkRequestRequestTypeDef",
+    "ResourceUriOutputTypeDef",
     "ResourceUriTypeDef",
     "ResumeWorkflowRunRequestRequestTypeDef",
     "RunStatementRequestRequestTypeDef",
+    "S3DirectSourceAdditionalOptionsOutputTypeDef",
     "S3DirectSourceAdditionalOptionsTypeDef",
+    "SchemaColumnTypeDef",
+    "SchemaIdOutputTypeDef",
     "SortCriterionTypeDef",
+    "SerDeInfoOutputTypeDef",
     "SerDeInfoTypeDef",
+    "SessionCommandOutputTypeDef",
+    "SkewedInfoOutputTypeDef",
     "SkewedInfoTypeDef",
+    "SqlAliasOutputTypeDef",
     "SqlAliasTypeDef",
     "StartBlueprintRunRequestRequestTypeDef",
     "StartCrawlerRequestRequestTypeDef",
     "StartCrawlerScheduleRequestRequestTypeDef",
     "StartExportLabelsTaskRunRequestRequestTypeDef",
     "StartImportLabelsTaskRunRequestRequestTypeDef",
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
@@ -390,37 +490,39 @@
     "StartingEventBatchConditionTypeDef",
     "StatementOutputDataTypeDef",
     "StopCrawlerRequestRequestTypeDef",
     "StopCrawlerScheduleRequestRequestTypeDef",
     "StopSessionRequestRequestTypeDef",
     "StopTriggerRequestRequestTypeDef",
     "StopWorkflowRunRequestRequestTypeDef",
+    "TableIdentifierOutputTypeDef",
     "TableIdentifierTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBlueprintRequestRequestTypeDef",
     "UpdateCsvClassifierRequestTypeDef",
     "UpdateGrokClassifierRequestTypeDef",
     "UpdateJsonClassifierRequestTypeDef",
     "UpdateXMLClassifierRequestTypeDef",
     "UpdateCrawlerScheduleRequestRequestTypeDef",
     "UpdateDataQualityRulesetRequestRequestTypeDef",
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "WorkflowRunStatisticsTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
+    "AggregateOutputTypeDef",
     "AggregateTypeDef",
+    "AmazonRedshiftNodeDataOutputTypeDef",
     "AmazonRedshiftNodeDataTypeDef",
     "GetUnfilteredPartitionMetadataRequestRequestTypeDef",
     "GetUnfilteredTableMetadataRequestRequestTypeDef",
     "BackfillErrorTypeDef",
-    "BatchDeletePartitionRequestRequestTypeDef",
-    "BatchGetPartitionRequestRequestTypeDef",
     "CancelMLTaskRunResponseTypeDef",
     "CheckSchemaVersionValidityResponseTypeDef",
     "CreateBlueprintResponseTypeDef",
     "CreateCustomEntityTypeResponseTypeDef",
     "CreateDataQualityRulesetResponseTypeDef",
     "CreateDevEndpointResponseTypeDef",
     "CreateJobResponseTypeDef",
@@ -487,78 +589,104 @@
     "BatchDeleteConnectionResponseTypeDef",
     "BatchStopJobRunErrorTypeDef",
     "BatchUpdatePartitionFailureEntryTypeDef",
     "ColumnErrorTypeDef",
     "PartitionErrorTypeDef",
     "TableErrorTypeDef",
     "TableVersionErrorTypeDef",
+    "BatchDeletePartitionRequestRequestTypeDef",
+    "BatchGetPartitionRequestRequestTypeDef",
     "BatchGetCustomEntityTypesResponseTypeDef",
     "ListCustomEntityTypesResponseTypeDef",
     "BatchGetDevEndpointsResponseTypeDef",
     "GetDevEndpointResponseTypeDef",
     "GetDevEndpointsResponseTypeDef",
     "GetBlueprintRunResponseTypeDef",
     "GetBlueprintRunsResponseTypeDef",
     "BlueprintTypeDef",
     "GetCatalogImportStatusResponseTypeDef",
+    "CatalogKafkaSourceOutputTypeDef",
+    "DirectKafkaSourceOutputTypeDef",
     "CatalogKafkaSourceTypeDef",
     "DirectKafkaSourceTypeDef",
+    "CatalogKinesisSourceOutputTypeDef",
+    "DirectKinesisSourceOutputTypeDef",
     "CatalogKinesisSourceTypeDef",
     "DirectKinesisSourceTypeDef",
+    "GovernedCatalogTargetOutputTypeDef",
+    "S3CatalogTargetOutputTypeDef",
+    "S3DeltaCatalogTargetOutputTypeDef",
+    "S3HudiCatalogTargetOutputTypeDef",
     "GovernedCatalogTargetTypeDef",
     "S3CatalogTargetTypeDef",
     "S3DeltaCatalogTargetTypeDef",
     "S3HudiCatalogTargetTypeDef",
     "ClassifierTypeDef",
+    "CodeGenNodeOutputTypeDef",
     "CodeGenNodeTypeDef",
     "LocationTypeDef",
+    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "FindMatchesMetricsTypeDef",
     "ConnectionInputTypeDef",
     "ConnectionTypeDef",
     "CrawlerNodeDetailsTypeDef",
     "ListCrawlsResponseTypeDef",
     "GetCrawlerMetricsResponseTypeDef",
+    "CrawlerTargetsOutputTypeDef",
     "CrawlerTargetsTypeDef",
     "ListCrawlsRequestRequestTypeDef",
     "CreateClassifierRequestRequestTypeDef",
     "CreateDataQualityRulesetRequestRequestTypeDef",
     "DataQualityRulesetFilterCriteriaTypeDef",
-    "DataQualityRulesetListDetailsTypeDef",
-    "GetDataQualityRulesetResponseTypeDef",
     "DataSourceTypeDef",
     "CreatePartitionIndexRequestRequestTypeDef",
     "CreateSchemaInputRequestTypeDef",
     "DeleteRegistryInputRequestTypeDef",
     "GetRegistryInputRequestTypeDef",
     "ListSchemasInputRequestTypeDef",
     "UpdateRegistryInputRequestTypeDef",
     "CreateSessionRequestRequestTypeDef",
-    "SessionTypeDef",
+    "EvaluateDataQualityMultiFrameOutputTypeDef",
+    "EvaluateDataQualityOutputTypeDef",
     "EvaluateDataQualityMultiFrameTypeDef",
     "EvaluateDataQualityTypeDef",
+    "DataCatalogEncryptionSettingsOutputTypeDef",
     "DataCatalogEncryptionSettingsTypeDef",
+    "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
+    "DataQualityRulesetListDetailsTypeDef",
+    "GetDataQualityRulesetResponseTypeDef",
+    "DataSourceOutputTypeDef",
+    "NullValueFieldOutputTypeDef",
     "NullValueFieldTypeDef",
+    "DecimalColumnStatisticsDataOutputTypeDef",
     "DecimalColumnStatisticsDataTypeDef",
     "DeleteSchemaInputRequestTypeDef",
     "DeleteSchemaVersionsInputRequestTypeDef",
     "GetSchemaByDefinitionInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "ListSchemaVersionsInputRequestTypeDef",
     "RegisterSchemaVersionInputRequestTypeDef",
     "SchemaReferenceTypeDef",
     "UpdateDevEndpointRequestRequestTypeDef",
+    "S3DeltaDirectTargetOutputTypeDef",
+    "S3DirectTargetOutputTypeDef",
+    "S3GlueParquetTargetOutputTypeDef",
+    "S3HudiDirectTargetOutputTypeDef",
     "S3DeltaDirectTargetTypeDef",
     "S3DirectTargetTypeDef",
     "S3GlueParquetTargetTypeDef",
     "S3HudiDirectTargetTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "SchemaVersionErrorItemTypeDef",
+    "FilterExpressionOutputTypeDef",
     "FilterExpressionTypeDef",
+    "TransformParametersOutputTypeDef",
     "TransformParametersTypeDef",
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
     "GetCrawlersRequestGetCrawlersPaginateTypeDef",
     "GetDatabasesRequestGetDatabasesPaginateTypeDef",
     "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
     "GetJobRunsRequestGetJobRunsPaginateTypeDef",
@@ -574,103 +702,128 @@
     "ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
     "ListSchemasInputListSchemasPaginateTypeDef",
     "GetConnectionsRequestGetConnectionsPaginateTypeDef",
     "GetConnectionsRequestRequestTypeDef",
     "GetJobBookmarkResponseTypeDef",
     "ResetJobBookmarkResponseTypeDef",
     "GetMLTaskRunsRequestRequestTypeDef",
-    "TransformFilterCriteriaTypeDef",
     "GetMappingResponseTypeDef",
     "GetPartitionsRequestGetPartitionsPaginateTypeDef",
     "GetPartitionsRequestRequestTypeDef",
     "GetUnfilteredPartitionsMetadataRequestRequestTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetSchemaVersionInputRequestTypeDef",
     "GetSchemaVersionsDiffInputRequestTypeDef",
     "UpdateSchemaInputRequestTypeDef",
+    "GlueSchemaOutputTypeDef",
     "GlueSchemaTypeDef",
+    "GovernedCatalogSourceOutputTypeDef",
+    "S3CatalogSourceOutputTypeDef",
     "GovernedCatalogSourceTypeDef",
     "S3CatalogSourceTypeDef",
     "OpenTableFormatInputTypeDef",
     "JobRunTypeDef",
+    "JoinOutputTypeDef",
     "JoinTypeDef",
     "TaskRunPropertiesTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
+    "TransformEncryptionOutputTypeDef",
     "TransformEncryptionTypeDef",
     "MetadataInfoTypeDef",
     "PutSchemaVersionMetadataInputRequestTypeDef",
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     "RemoveSchemaVersionMetadataInputRequestTypeDef",
+    "RedshiftTargetOutputTypeDef",
     "RedshiftTargetTypeDef",
-    "UserDefinedFunctionInputTypeDef",
     "UserDefinedFunctionTypeDef",
+    "UserDefinedFunctionInputTypeDef",
+    "TransformFilterCriteriaTypeDef",
+    "SchemaReferenceOutputTypeDef",
     "SearchTablesRequestRequestTypeDef",
+    "SessionTypeDef",
     "StatementOutputTypeDef",
     "UpdateClassifierRequestRequestTypeDef",
+    "AmazonRedshiftSourceOutputTypeDef",
+    "AmazonRedshiftTargetOutputTypeDef",
     "AmazonRedshiftSourceTypeDef",
     "AmazonRedshiftTargetTypeDef",
     "PartitionIndexDescriptorTypeDef",
     "BatchStopJobRunResponseTypeDef",
     "BatchUpdatePartitionResponseTypeDef",
     "BatchCreatePartitionResponseTypeDef",
     "BatchDeletePartitionResponseTypeDef",
     "BatchDeleteTableResponseTypeDef",
     "BatchDeleteTableVersionResponseTypeDef",
     "BatchGetBlueprintsResponseTypeDef",
     "GetBlueprintResponseTypeDef",
     "GetClassifierResponseTypeDef",
     "GetClassifiersResponseTypeDef",
-    "CreateScriptRequestRequestTypeDef",
     "GetDataflowGraphResponseTypeDef",
+    "CreateScriptRequestRequestTypeDef",
     "GetMappingRequestRequestTypeDef",
     "GetPlanRequestRequestTypeDef",
-    "CreateTriggerRequestRequestTypeDef",
     "TriggerTypeDef",
+    "CreateTriggerRequestRequestTypeDef",
     "TriggerUpdateTypeDef",
     "EvaluationMetricsTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "GetConnectionResponseTypeDef",
     "GetConnectionsResponseTypeDef",
     "CrawlerTypeDef",
     "CreateCrawlerRequestRequestTypeDef",
     "UpdateCrawlerRequestRequestTypeDef",
     "ListDataQualityRulesetsRequestRequestTypeDef",
-    "ListDataQualityRulesetsResponseTypeDef",
-    "DataQualityResultDescriptionTypeDef",
     "DataQualityResultFilterCriteriaTypeDef",
-    "DataQualityResultTypeDef",
-    "DataQualityRuleRecommendationRunDescriptionTypeDef",
     "DataQualityRuleRecommendationRunFilterTypeDef",
-    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
     "DataQualityRulesetEvaluationRunFilterTypeDef",
-    "GetDataQualityResultResponseTypeDef",
-    "GetDataQualityRuleRecommendationRunResponseTypeDef",
-    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
     "StartDataQualityRuleRecommendationRunRequestRequestTypeDef",
     "StartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    "CreateSessionResponseTypeDef",
-    "GetSessionResponseTypeDef",
-    "ListSessionsResponseTypeDef",
     "GetDataCatalogEncryptionSettingsResponseTypeDef",
     "PutDataCatalogEncryptionSettingsRequestRequestTypeDef",
-    "DatabaseInputTypeDef",
     "DatabaseTypeDef",
+    "DatabaseInputTypeDef",
+    "ListDataQualityRulesetsResponseTypeDef",
+    "DataQualityResultDescriptionTypeDef",
+    "DataQualityResultTypeDef",
+    "DataQualityRuleRecommendationRunDescriptionTypeDef",
+    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
+    "GetDataQualityResultResponseTypeDef",
+    "GetDataQualityRuleRecommendationRunResponseTypeDef",
+    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
+    "DropNullFieldsOutputTypeDef",
     "DropNullFieldsTypeDef",
+    "ColumnStatisticsDataOutputTypeDef",
     "ColumnStatisticsDataTypeDef",
     "StorageDescriptorTypeDef",
-    "CreateSecurityConfigurationRequestRequestTypeDef",
     "SecurityConfigurationTypeDef",
+    "CreateSecurityConfigurationRequestRequestTypeDef",
     "DeleteSchemaVersionsResponseTypeDef",
+    "FilterOutputTypeDef",
     "FilterTypeDef",
     "UpdateMLTransformRequestRequestTypeDef",
-    "GetMLTransformsRequestRequestTypeDef",
-    "ListMLTransformsRequestRequestTypeDef",
+    "AthenaConnectorSourceOutputTypeDef",
+    "CatalogDeltaSourceOutputTypeDef",
+    "CatalogHudiSourceOutputTypeDef",
+    "CustomCodeOutputTypeDef",
+    "DynamicTransformOutputTypeDef",
+    "JDBCConnectorSourceOutputTypeDef",
+    "JDBCConnectorTargetOutputTypeDef",
+    "S3CatalogDeltaSourceOutputTypeDef",
+    "S3CatalogHudiSourceOutputTypeDef",
+    "S3CsvSourceOutputTypeDef",
+    "S3DeltaSourceOutputTypeDef",
+    "S3HudiSourceOutputTypeDef",
+    "S3JsonSourceOutputTypeDef",
+    "S3ParquetSourceOutputTypeDef",
+    "SparkConnectorSourceOutputTypeDef",
+    "SparkConnectorTargetOutputTypeDef",
+    "SparkSQLOutputTypeDef",
     "AthenaConnectorSourceTypeDef",
     "CatalogDeltaSourceTypeDef",
     "CatalogHudiSourceTypeDef",
     "CustomCodeTypeDef",
     "DynamicTransformTypeDef",
     "JDBCConnectorSourceTypeDef",
     "JDBCConnectorTargetTypeDef",
@@ -687,164 +840,223 @@
     "GetJobRunResponseTypeDef",
     "GetJobRunsResponseTypeDef",
     "JobNodeDetailsTypeDef",
     "GetMLTaskRunResponseTypeDef",
     "TaskRunTypeDef",
     "CreateMLTransformRequestRequestTypeDef",
     "QuerySchemaVersionMetadataResponseTypeDef",
-    "CreateUserDefinedFunctionRequestRequestTypeDef",
-    "UpdateUserDefinedFunctionRequestRequestTypeDef",
     "GetUserDefinedFunctionResponseTypeDef",
     "GetUserDefinedFunctionsResponseTypeDef",
+    "CreateUserDefinedFunctionRequestRequestTypeDef",
+    "UpdateUserDefinedFunctionRequestRequestTypeDef",
+    "GetMLTransformsRequestRequestTypeDef",
+    "ListMLTransformsRequestRequestTypeDef",
+    "StorageDescriptorOutputTypeDef",
+    "CreateSessionResponseTypeDef",
+    "GetSessionResponseTypeDef",
+    "ListSessionsResponseTypeDef",
     "StatementTypeDef",
     "GetPartitionIndexesResponseTypeDef",
     "BatchGetTriggersResponseTypeDef",
     "GetTriggerResponseTypeDef",
     "GetTriggersResponseTypeDef",
     "TriggerNodeDetailsTypeDef",
     "UpdateTriggerResponseTypeDef",
     "UpdateTriggerRequestRequestTypeDef",
     "GetMLTransformResponseTypeDef",
     "MLTransformTypeDef",
     "BatchGetCrawlersResponseTypeDef",
     "GetCrawlerResponseTypeDef",
     "GetCrawlersResponseTypeDef",
-    "ListDataQualityResultsResponseTypeDef",
     "ListDataQualityResultsRequestRequestTypeDef",
-    "BatchGetDataQualityResultResponseTypeDef",
-    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
     "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
     "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
-    "CreateDatabaseRequestRequestTypeDef",
-    "UpdateDatabaseRequestRequestTypeDef",
     "GetDatabaseResponseTypeDef",
     "GetDatabasesResponseTypeDef",
+    "CreateDatabaseRequestRequestTypeDef",
+    "UpdateDatabaseRequestRequestTypeDef",
+    "ListDataQualityResultsResponseTypeDef",
+    "BatchGetDataQualityResultResponseTypeDef",
+    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+    "ColumnStatisticsOutputTypeDef",
     "ColumnStatisticsTypeDef",
     "PartitionInputTypeDef",
-    "PartitionTypeDef",
     "TableInputTypeDef",
-    "TableTypeDef",
     "GetSecurityConfigurationResponseTypeDef",
     "GetSecurityConfigurationsResponseTypeDef",
+    "CodeGenConfigurationNodeOutputTypeDef",
     "CodeGenConfigurationNodeTypeDef",
     "GetMLTaskRunsResponseTypeDef",
+    "PartitionTypeDef",
+    "TableTypeDef",
     "GetStatementResponseTypeDef",
     "ListStatementsResponseTypeDef",
     "NodeTypeDef",
     "GetMLTransformsResponseTypeDef",
     "ColumnStatisticsErrorTypeDef",
     "GetColumnStatisticsForPartitionResponseTypeDef",
     "GetColumnStatisticsForTableResponseTypeDef",
     "UpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     "UpdateColumnStatisticsForTableRequestRequestTypeDef",
     "BatchCreatePartitionRequestRequestTypeDef",
     "BatchUpdatePartitionRequestEntryTypeDef",
     "CreatePartitionRequestRequestTypeDef",
     "UpdatePartitionRequestRequestTypeDef",
+    "CreateTableRequestRequestTypeDef",
+    "UpdateTableRequestRequestTypeDef",
+    "JobTypeDef",
+    "CreateJobRequestRequestTypeDef",
+    "JobUpdateTypeDef",
     "BatchGetPartitionResponseTypeDef",
     "GetPartitionResponseTypeDef",
     "GetPartitionsResponseTypeDef",
     "GetUnfilteredPartitionMetadataResponseTypeDef",
     "UnfilteredPartitionTypeDef",
-    "CreateTableRequestRequestTypeDef",
-    "UpdateTableRequestRequestTypeDef",
     "GetTableResponseTypeDef",
     "GetTablesResponseTypeDef",
     "GetUnfilteredTableMetadataResponseTypeDef",
     "SearchTablesResponseTypeDef",
     "TableVersionTypeDef",
-    "CreateJobRequestRequestTypeDef",
-    "JobTypeDef",
-    "JobUpdateTypeDef",
     "WorkflowGraphTypeDef",
     "UpdateColumnStatisticsForPartitionResponseTypeDef",
     "UpdateColumnStatisticsForTableResponseTypeDef",
     "BatchUpdatePartitionRequestRequestTypeDef",
-    "GetUnfilteredPartitionsMetadataResponseTypeDef",
-    "GetTableVersionResponseTypeDef",
-    "GetTableVersionsResponseTypeDef",
     "BatchGetJobsResponseTypeDef",
     "GetJobResponseTypeDef",
     "GetJobsResponseTypeDef",
     "UpdateJobRequestRequestTypeDef",
+    "GetUnfilteredPartitionsMetadataResponseTypeDef",
+    "GetTableVersionResponseTypeDef",
+    "GetTableVersionsResponseTypeDef",
     "WorkflowRunTypeDef",
     "GetWorkflowRunResponseTypeDef",
     "GetWorkflowRunsResponseTypeDef",
     "WorkflowTypeDef",
     "BatchGetWorkflowsResponseTypeDef",
     "GetWorkflowResponseTypeDef",
 )
 
+NotificationPropertyOutputTypeDef = TypedDict(
+    "NotificationPropertyOutputTypeDef",
+    {
+        "NotifyDelayAfter": int,
+    },
+)
+
 NotificationPropertyTypeDef = TypedDict(
     "NotificationPropertyTypeDef",
     {
         "NotifyDelayAfter": int,
     },
     total=False,
 )
 
+AggregateOperationOutputTypeDef = TypedDict(
+    "AggregateOperationOutputTypeDef",
+    {
+        "Column": List[str],
+        "AggFunc": AggFunctionType,
+    },
+)
+
 AggregateOperationTypeDef = TypedDict(
     "AggregateOperationTypeDef",
     {
-        "Column": List[str],
+        "Column": Sequence[str],
         "AggFunc": AggFunctionType,
     },
 )
 
+AmazonRedshiftAdvancedOptionOutputTypeDef = TypedDict(
+    "AmazonRedshiftAdvancedOptionOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 AmazonRedshiftAdvancedOptionTypeDef = TypedDict(
     "AmazonRedshiftAdvancedOptionTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+OptionOutputTypeDef = TypedDict(
+    "OptionOutputTypeDef",
+    {
+        "Value": str,
+        "Label": str,
+        "Description": str,
+    },
+)
+
 OptionTypeDef = TypedDict(
     "OptionTypeDef",
     {
         "Value": str,
         "Label": str,
         "Description": str,
     },
     total=False,
 )
 
+ApplyMappingOutputTypeDef = TypedDict(
+    "ApplyMappingOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Mapping": List["MappingOutputTypeDef"],
+    },
+)
+
 ApplyMappingTypeDef = TypedDict(
     "ApplyMappingTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "Mapping": List["MappingTypeDef"],
+        "Inputs": Sequence[str],
+        "Mapping": Sequence["MappingTypeDef"],
     },
 )
 
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
         "RequestedColumns": Sequence[str],
         "AllColumnsRequested": bool,
     },
     total=False,
 )
 
-PartitionValueListTypeDef = TypedDict(
-    "PartitionValueListTypeDef",
+PartitionValueListOutputTypeDef = TypedDict(
+    "PartitionValueListOutputTypeDef",
     {
-        "Values": Sequence[str],
+        "Values": List[str],
+    },
+)
+
+BasicCatalogTargetOutputTypeDef = TypedDict(
+    "BasicCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
     },
 )
 
 BasicCatalogTargetTypeDef = TypedDict(
     "BasicCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
@@ -867,29 +1079,33 @@
     "_OptionalBatchDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteConnectionRequestRequestTypeDef(
     _RequiredBatchDeleteConnectionRequestRequestTypeDef,
     _OptionalBatchDeleteConnectionRequestRequestTypeDef,
 ):
     pass
 
-
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+PartitionValueListTypeDef = TypedDict(
+    "PartitionValueListTypeDef",
+    {
+        "Values": Sequence[str],
+    },
 )
 
 _RequiredBatchDeleteTableRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TablesToDelete": Sequence[str],
@@ -900,21 +1116,19 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteTableRequestRequestTypeDef(
     _RequiredBatchDeleteTableRequestRequestTypeDef, _OptionalBatchDeleteTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredBatchDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionIds": Sequence[str],
     },
@@ -923,22 +1137,20 @@
     "_OptionalBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteTableVersionRequestRequestTypeDef(
     _RequiredBatchDeleteTableVersionRequestRequestTypeDef,
     _OptionalBatchDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetBlueprintsRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 _OptionalBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
@@ -946,56 +1158,43 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
-
 class BatchGetBlueprintsRequestRequestTypeDef(
     _RequiredBatchGetBlueprintsRequestRequestTypeDef,
     _OptionalBatchGetBlueprintsRequestRequestTypeDef,
 ):
     pass
 
-
 BatchGetCrawlersRequestRequestTypeDef = TypedDict(
     "BatchGetCrawlersRequestRequestTypeDef",
     {
         "CrawlerNames": Sequence[str],
     },
 )
 
 BatchGetCustomEntityTypesRequestRequestTypeDef = TypedDict(
     "BatchGetCustomEntityTypesRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 
-_RequiredCustomEntityTypeTypeDef = TypedDict(
-    "_RequiredCustomEntityTypeTypeDef",
+CustomEntityTypeTypeDef = TypedDict(
+    "CustomEntityTypeTypeDef",
     {
         "Name": str,
         "RegexString": str,
-    },
-)
-_OptionalCustomEntityTypeTypeDef = TypedDict(
-    "_OptionalCustomEntityTypeTypeDef",
-    {
         "ContextWords": List[str],
     },
-    total=False,
 )
 
-
-class CustomEntityTypeTypeDef(_RequiredCustomEntityTypeTypeDef, _OptionalCustomEntityTypeTypeDef):
-    pass
-
-
 BatchGetDataQualityResultRequestRequestTypeDef = TypedDict(
     "BatchGetDataQualityResultRequestRequestTypeDef",
     {
         "ResultIds": Sequence[str],
     },
 )
 
@@ -1031,15 +1230,14 @@
         "CreatedTimestamp": datetime,
         "LastModifiedTimestamp": datetime,
         "PublicKey": str,
         "PublicKeys": List[str],
         "SecurityConfiguration": str,
         "Arguments": Dict[str, str],
     },
-    total=False,
 )
 
 BatchGetJobsRequestRequestTypeDef = TypedDict(
     "BatchGetJobsRequestRequestTypeDef",
     {
         "JobNames": Sequence[str],
     },
@@ -1062,36 +1260,42 @@
     "_OptionalBatchGetWorkflowsRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
-
 class BatchGetWorkflowsRequestRequestTypeDef(
     _RequiredBatchGetWorkflowsRequestRequestTypeDef, _OptionalBatchGetWorkflowsRequestRequestTypeDef
 ):
     pass
 
-
 BatchStopJobRunRequestRequestTypeDef = TypedDict(
     "BatchStopJobRunRequestRequestTypeDef",
     {
         "JobName": str,
         "JobRunIds": Sequence[str],
     },
 )
 
 BatchStopJobRunSuccessfulSubmissionTypeDef = TypedDict(
     "BatchStopJobRunSuccessfulSubmissionTypeDef",
     {
         "JobName": str,
         "JobRunId": str,
     },
-    total=False,
+)
+
+BinaryColumnStatisticsDataOutputTypeDef = TypedDict(
+    "BinaryColumnStatisticsDataOutputTypeDef",
+    {
+        "MaximumLength": int,
+        "AverageLength": float,
+        "NumberOfNulls": int,
+    },
 )
 
 BinaryColumnStatisticsDataTypeDef = TypedDict(
     "BinaryColumnStatisticsDataTypeDef",
     {
         "MaximumLength": int,
         "AverageLength": float,
@@ -1101,15 +1305,14 @@
 
 BlueprintDetailsTypeDef = TypedDict(
     "BlueprintDetailsTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
     },
-    total=False,
 )
 
 BlueprintRunTypeDef = TypedDict(
     "BlueprintRunTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
@@ -1118,27 +1321,34 @@
         "StartedOn": datetime,
         "CompletedOn": datetime,
         "ErrorMessage": str,
         "RollbackErrorMessage": str,
         "Parameters": str,
         "RoleArn": str,
     },
-    total=False,
 )
 
 LastActiveDefinitionTypeDef = TypedDict(
     "LastActiveDefinitionTypeDef",
     {
         "Description": str,
         "LastModifiedOn": datetime,
         "ParameterSpec": str,
         "BlueprintLocation": str,
         "BlueprintServiceLocation": str,
     },
-    total=False,
+)
+
+BooleanColumnStatisticsDataOutputTypeDef = TypedDict(
+    "BooleanColumnStatisticsDataOutputTypeDef",
+    {
+        "NumberOfTrues": int,
+        "NumberOfFalses": int,
+        "NumberOfNulls": int,
+    },
 )
 
 BooleanColumnStatisticsDataTypeDef = TypedDict(
     "BooleanColumnStatisticsDataTypeDef",
     {
         "NumberOfTrues": int,
         "NumberOfFalses": int,
@@ -1179,21 +1389,19 @@
     "_OptionalCancelStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class CancelStatementRequestRequestTypeDef(
     _RequiredCancelStatementRequestRequestTypeDef, _OptionalCancelStatementRequestRequestTypeDef
 ):
     pass
 
-
 CatalogEntryTypeDef = TypedDict(
     "CatalogEntryTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1201,15 +1409,47 @@
 CatalogImportStatusTypeDef = TypedDict(
     "CatalogImportStatusTypeDef",
     {
         "ImportCompleted": bool,
         "ImportTime": datetime,
         "ImportedBy": str,
     },
-    total=False,
+)
+
+KafkaStreamingSourceOptionsOutputTypeDef = TypedDict(
+    "KafkaStreamingSourceOptionsOutputTypeDef",
+    {
+        "BootstrapServers": str,
+        "SecurityProtocol": str,
+        "ConnectionName": str,
+        "TopicName": str,
+        "Assign": str,
+        "SubscribePattern": str,
+        "Classification": str,
+        "Delimiter": str,
+        "StartingOffsets": str,
+        "EndingOffsets": str,
+        "PollTimeoutMs": int,
+        "NumRetries": int,
+        "RetryIntervalMs": int,
+        "MaxOffsetsPerTrigger": int,
+        "MinPartitions": int,
+        "IncludeHeaders": bool,
+        "AddRecordTimestamp": str,
+        "EmitConsumerLagMetrics": str,
+        "StartingTimestamp": datetime,
+    },
+)
+
+StreamingDataPreviewOptionsOutputTypeDef = TypedDict(
+    "StreamingDataPreviewOptionsOutputTypeDef",
+    {
+        "PollingTime": int,
+        "RecordPollingLimit": int,
+    },
 )
 
 KafkaStreamingSourceOptionsTypeDef = TypedDict(
     "KafkaStreamingSourceOptionsTypeDef",
     {
         "BootstrapServers": str,
         "SecurityProtocol": str,
@@ -1225,28 +1465,55 @@
         "NumRetries": int,
         "RetryIntervalMs": int,
         "MaxOffsetsPerTrigger": int,
         "MinPartitions": int,
         "IncludeHeaders": bool,
         "AddRecordTimestamp": str,
         "EmitConsumerLagMetrics": str,
-        "StartingTimestamp": datetime,
+        "StartingTimestamp": Union[datetime, str],
     },
     total=False,
 )
 
 StreamingDataPreviewOptionsTypeDef = TypedDict(
     "StreamingDataPreviewOptionsTypeDef",
     {
         "PollingTime": int,
         "RecordPollingLimit": int,
     },
     total=False,
 )
 
+KinesisStreamingSourceOptionsOutputTypeDef = TypedDict(
+    "KinesisStreamingSourceOptionsOutputTypeDef",
+    {
+        "EndpointUrl": str,
+        "StreamName": str,
+        "Classification": str,
+        "Delimiter": str,
+        "StartingPosition": StartingPositionType,
+        "MaxFetchTimeInMs": int,
+        "MaxFetchRecordsPerShard": int,
+        "MaxRecordPerRead": int,
+        "AddIdleTimeBetweenReads": bool,
+        "IdleTimeBetweenReadsInMs": int,
+        "DescribeShardInterval": int,
+        "NumRetries": int,
+        "RetryIntervalMs": int,
+        "MaxRetryIntervalMs": int,
+        "AvoidEmptyBatches": bool,
+        "StreamArn": str,
+        "RoleArn": str,
+        "RoleSessionName": str,
+        "AddRecordTimestamp": str,
+        "EmitConsumerLagMetrics": str,
+        "StartingTimestamp": datetime,
+    },
+)
+
 KinesisStreamingSourceOptionsTypeDef = TypedDict(
     "KinesisStreamingSourceOptionsTypeDef",
     {
         "EndpointUrl": str,
         "StreamName": str,
         "Classification": str,
         "Delimiter": str,
@@ -1262,172 +1529,388 @@
         "MaxRetryIntervalMs": int,
         "AvoidEmptyBatches": bool,
         "StreamArn": str,
         "RoleArn": str,
         "RoleSessionName": str,
         "AddRecordTimestamp": str,
         "EmitConsumerLagMetrics": str,
-        "StartingTimestamp": datetime,
+        "StartingTimestamp": Union[datetime, str],
     },
     total=False,
 )
 
+CatalogSchemaChangePolicyOutputTypeDef = TypedDict(
+    "CatalogSchemaChangePolicyOutputTypeDef",
+    {
+        "EnableUpdateCatalog": bool,
+        "UpdateBehavior": UpdateCatalogBehaviorType,
+    },
+)
+
 CatalogSchemaChangePolicyTypeDef = TypedDict(
     "CatalogSchemaChangePolicyTypeDef",
     {
         "EnableUpdateCatalog": bool,
         "UpdateBehavior": UpdateCatalogBehaviorType,
     },
     total=False,
 )
 
+CatalogSourceOutputTypeDef = TypedDict(
+    "CatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+
 CatalogSourceTypeDef = TypedDict(
     "CatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
+CatalogTargetOutputTypeDef = TypedDict(
+    "CatalogTargetOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "Tables": List[str],
+        "ConnectionName": str,
+        "EventQueueArn": str,
+        "DlqEventQueueArn": str,
+    },
+)
+
 _RequiredCatalogTargetTypeDef = TypedDict(
     "_RequiredCatalogTargetTypeDef",
     {
         "DatabaseName": str,
-        "Tables": List[str],
+        "Tables": Sequence[str],
     },
 )
 _OptionalCatalogTargetTypeDef = TypedDict(
     "_OptionalCatalogTargetTypeDef",
     {
         "ConnectionName": str,
         "EventQueueArn": str,
         "DlqEventQueueArn": str,
     },
     total=False,
 )
 
-
 class CatalogTargetTypeDef(_RequiredCatalogTargetTypeDef, _OptionalCatalogTargetTypeDef):
     pass
 
-
 CheckSchemaVersionValidityInputRequestTypeDef = TypedDict(
     "CheckSchemaVersionValidityInputRequestTypeDef",
     {
         "DataFormat": DataFormatType,
         "SchemaDefinition": str,
     },
 )
 
-_RequiredCsvClassifierTypeDef = TypedDict(
-    "_RequiredCsvClassifierTypeDef",
+CsvClassifierTypeDef = TypedDict(
+    "CsvClassifierTypeDef",
     {
         "Name": str,
-    },
-)
-_OptionalCsvClassifierTypeDef = TypedDict(
-    "_OptionalCsvClassifierTypeDef",
-    {
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "Version": int,
         "Delimiter": str,
         "QuoteSymbol": str,
         "ContainsHeader": CsvHeaderOptionType,
         "Header": List[str],
         "DisableValueTrimming": bool,
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": List[str],
     },
-    total=False,
 )
 
-
-class CsvClassifierTypeDef(_RequiredCsvClassifierTypeDef, _OptionalCsvClassifierTypeDef):
-    pass
-
-
-_RequiredGrokClassifierTypeDef = TypedDict(
-    "_RequiredGrokClassifierTypeDef",
+GrokClassifierTypeDef = TypedDict(
+    "GrokClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
+        "CreationTime": datetime,
+        "LastUpdated": datetime,
+        "Version": int,
         "GrokPattern": str,
+        "CustomPatterns": str,
     },
 )
-_OptionalGrokClassifierTypeDef = TypedDict(
-    "_OptionalGrokClassifierTypeDef",
+
+JsonClassifierTypeDef = TypedDict(
+    "JsonClassifierTypeDef",
     {
+        "Name": str,
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "Version": int,
-        "CustomPatterns": str,
+        "JsonPath": str,
+    },
+)
+
+XMLClassifierTypeDef = TypedDict(
+    "XMLClassifierTypeDef",
+    {
+        "Name": str,
+        "Classification": str,
+        "CreationTime": datetime,
+        "LastUpdated": datetime,
+        "Version": int,
+        "RowTag": str,
+    },
+)
+
+CloudWatchEncryptionOutputTypeDef = TypedDict(
+    "CloudWatchEncryptionOutputTypeDef",
+    {
+        "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
+        "KmsKeyArn": str,
+    },
+)
+
+CloudWatchEncryptionTypeDef = TypedDict(
+    "CloudWatchEncryptionTypeDef",
+    {
+        "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
+        "KmsKeyArn": str,
     },
     total=False,
 )
 
+DirectJDBCSourceOutputTypeDef = TypedDict(
+    "DirectJDBCSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "ConnectionName": str,
+        "ConnectionType": JDBCConnectionTypeType,
+        "RedshiftTmpDir": str,
+    },
+)
+
+DropDuplicatesOutputTypeDef = TypedDict(
+    "DropDuplicatesOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Columns": List[List[str]],
+    },
+)
 
-class GrokClassifierTypeDef(_RequiredGrokClassifierTypeDef, _OptionalGrokClassifierTypeDef):
-    pass
+DropFieldsOutputTypeDef = TypedDict(
+    "DropFieldsOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Paths": List[List[str]],
+    },
+)
 
+DynamoDBCatalogSourceOutputTypeDef = TypedDict(
+    "DynamoDBCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
 
-_RequiredJsonClassifierTypeDef = TypedDict(
-    "_RequiredJsonClassifierTypeDef",
+FillMissingValuesOutputTypeDef = TypedDict(
+    "FillMissingValuesOutputTypeDef",
     {
         "Name": str,
-        "JsonPath": str,
+        "Inputs": List[str],
+        "ImputedPath": str,
+        "FilledPath": str,
     },
 )
-_OptionalJsonClassifierTypeDef = TypedDict(
-    "_OptionalJsonClassifierTypeDef",
+
+MergeOutputTypeDef = TypedDict(
+    "MergeOutputTypeDef",
     {
-        "CreationTime": datetime,
-        "LastUpdated": datetime,
-        "Version": int,
+        "Name": str,
+        "Inputs": List[str],
+        "Source": str,
+        "PrimaryKeys": List[List[str]],
     },
-    total=False,
 )
 
+MicrosoftSQLServerCatalogSourceOutputTypeDef = TypedDict(
+    "MicrosoftSQLServerCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
 
-class JsonClassifierTypeDef(_RequiredJsonClassifierTypeDef, _OptionalJsonClassifierTypeDef):
-    pass
+MicrosoftSQLServerCatalogTargetOutputTypeDef = TypedDict(
+    "MicrosoftSQLServerCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
+    },
+)
 
+MySQLCatalogSourceOutputTypeDef = TypedDict(
+    "MySQLCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
 
-_RequiredXMLClassifierTypeDef = TypedDict(
-    "_RequiredXMLClassifierTypeDef",
+MySQLCatalogTargetOutputTypeDef = TypedDict(
+    "MySQLCatalogTargetOutputTypeDef",
     {
         "Name": str,
-        "Classification": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
     },
 )
-_OptionalXMLClassifierTypeDef = TypedDict(
-    "_OptionalXMLClassifierTypeDef",
+
+OracleSQLCatalogSourceOutputTypeDef = TypedDict(
+    "OracleSQLCatalogSourceOutputTypeDef",
     {
-        "CreationTime": datetime,
-        "LastUpdated": datetime,
-        "Version": int,
-        "RowTag": str,
+        "Name": str,
+        "Database": str,
+        "Table": str,
     },
-    total=False,
 )
 
+OracleSQLCatalogTargetOutputTypeDef = TypedDict(
+    "OracleSQLCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
+    },
+)
 
-class XMLClassifierTypeDef(_RequiredXMLClassifierTypeDef, _OptionalXMLClassifierTypeDef):
-    pass
+PIIDetectionOutputTypeDef = TypedDict(
+    "PIIDetectionOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PiiType": PiiTypeType,
+        "EntityTypesToDetect": List[str],
+        "OutputColumnName": str,
+        "SampleFraction": float,
+        "ThresholdFraction": float,
+        "MaskValue": str,
+    },
+)
 
+PostgreSQLCatalogSourceOutputTypeDef = TypedDict(
+    "PostgreSQLCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
 
-CloudWatchEncryptionTypeDef = TypedDict(
-    "CloudWatchEncryptionTypeDef",
+PostgreSQLCatalogTargetOutputTypeDef = TypedDict(
+    "PostgreSQLCatalogTargetOutputTypeDef",
     {
-        "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
-        "KmsKeyArn": str,
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
+    },
+)
+
+RedshiftSourceOutputTypeDef = TypedDict(
+    "RedshiftSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "RedshiftTmpDir": str,
+        "TmpDirIAMRole": str,
+    },
+)
+
+RelationalCatalogSourceOutputTypeDef = TypedDict(
+    "RelationalCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+
+RenameFieldOutputTypeDef = TypedDict(
+    "RenameFieldOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "SourcePath": List[str],
+        "TargetPath": List[str],
+    },
+)
+
+SelectFieldsOutputTypeDef = TypedDict(
+    "SelectFieldsOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Paths": List[List[str]],
+    },
+)
+
+SelectFromCollectionOutputTypeDef = TypedDict(
+    "SelectFromCollectionOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Index": int,
+    },
+)
+
+SpigotOutputTypeDef = TypedDict(
+    "SpigotOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Path": str,
+        "Topk": int,
+        "Prob": float,
+    },
+)
+
+SplitFieldsOutputTypeDef = TypedDict(
+    "SplitFieldsOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Paths": List[List[str]],
+    },
+)
+
+UnionOutputTypeDef = TypedDict(
+    "UnionOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "UnionType": UnionTypeType,
     },
-    total=False,
 )
 
 _RequiredDirectJDBCSourceTypeDef = TypedDict(
     "_RequiredDirectJDBCSourceTypeDef",
     {
         "Name": str,
         "Database": str,
@@ -1440,45 +1923,41 @@
     "_OptionalDirectJDBCSourceTypeDef",
     {
         "RedshiftTmpDir": str,
     },
     total=False,
 )
 
-
 class DirectJDBCSourceTypeDef(_RequiredDirectJDBCSourceTypeDef, _OptionalDirectJDBCSourceTypeDef):
     pass
 
-
 _RequiredDropDuplicatesTypeDef = TypedDict(
     "_RequiredDropDuplicatesTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
     },
 )
 _OptionalDropDuplicatesTypeDef = TypedDict(
     "_OptionalDropDuplicatesTypeDef",
     {
-        "Columns": List[List[str]],
+        "Columns": Sequence[Sequence[str]],
     },
     total=False,
 )
 
-
 class DropDuplicatesTypeDef(_RequiredDropDuplicatesTypeDef, _OptionalDropDuplicatesTypeDef):
     pass
 
-
 DropFieldsTypeDef = TypedDict(
     "DropFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "Paths": List[List[str]],
+        "Inputs": Sequence[str],
+        "Paths": Sequence[Sequence[str]],
     },
 )
 
 DynamoDBCatalogSourceTypeDef = TypedDict(
     "DynamoDBCatalogSourceTypeDef",
     {
         "Name": str,
@@ -1487,40 +1966,38 @@
     },
 )
 
 _RequiredFillMissingValuesTypeDef = TypedDict(
     "_RequiredFillMissingValuesTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "ImputedPath": str,
     },
 )
 _OptionalFillMissingValuesTypeDef = TypedDict(
     "_OptionalFillMissingValuesTypeDef",
     {
         "FilledPath": str,
     },
     total=False,
 )
 
-
 class FillMissingValuesTypeDef(
     _RequiredFillMissingValuesTypeDef, _OptionalFillMissingValuesTypeDef
 ):
     pass
 
-
 MergeTypeDef = TypedDict(
     "MergeTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Source": str,
-        "PrimaryKeys": List[List[str]],
+        "PrimaryKeys": Sequence[Sequence[str]],
     },
 )
 
 MicrosoftSQLServerCatalogSourceTypeDef = TypedDict(
     "MicrosoftSQLServerCatalogSourceTypeDef",
     {
         "Name": str,
@@ -1529,15 +2006,15 @@
     },
 )
 
 MicrosoftSQLServerCatalogTargetTypeDef = TypedDict(
     "MicrosoftSQLServerCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 
 MySQLCatalogSourceTypeDef = TypedDict(
     "MySQLCatalogSourceTypeDef",
@@ -1548,15 +2025,15 @@
     },
 )
 
 MySQLCatalogTargetTypeDef = TypedDict(
     "MySQLCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 
 OracleSQLCatalogSourceTypeDef = TypedDict(
     "OracleSQLCatalogSourceTypeDef",
@@ -1567,59 +2044,57 @@
     },
 )
 
 OracleSQLCatalogTargetTypeDef = TypedDict(
     "OracleSQLCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 
 _RequiredPIIDetectionTypeDef = TypedDict(
     "_RequiredPIIDetectionTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "PiiType": PiiTypeType,
-        "EntityTypesToDetect": List[str],
+        "EntityTypesToDetect": Sequence[str],
     },
 )
 _OptionalPIIDetectionTypeDef = TypedDict(
     "_OptionalPIIDetectionTypeDef",
     {
         "OutputColumnName": str,
         "SampleFraction": float,
         "ThresholdFraction": float,
         "MaskValue": str,
     },
     total=False,
 )
 
-
 class PIIDetectionTypeDef(_RequiredPIIDetectionTypeDef, _OptionalPIIDetectionTypeDef):
     pass
 
-
 PostgreSQLCatalogSourceTypeDef = TypedDict(
     "PostgreSQLCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
 PostgreSQLCatalogTargetTypeDef = TypedDict(
     "PostgreSQLCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 
 _RequiredRedshiftSourceTypeDef = TypedDict(
     "_RequiredRedshiftSourceTypeDef",
@@ -1634,96 +2109,101 @@
     {
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
     },
     total=False,
 )
 
-
 class RedshiftSourceTypeDef(_RequiredRedshiftSourceTypeDef, _OptionalRedshiftSourceTypeDef):
     pass
 
-
 RelationalCatalogSourceTypeDef = TypedDict(
     "RelationalCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
 RenameFieldTypeDef = TypedDict(
     "RenameFieldTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "SourcePath": List[str],
-        "TargetPath": List[str],
+        "Inputs": Sequence[str],
+        "SourcePath": Sequence[str],
+        "TargetPath": Sequence[str],
     },
 )
 
 SelectFieldsTypeDef = TypedDict(
     "SelectFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "Paths": List[List[str]],
+        "Inputs": Sequence[str],
+        "Paths": Sequence[Sequence[str]],
     },
 )
 
 SelectFromCollectionTypeDef = TypedDict(
     "SelectFromCollectionTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Index": int,
     },
 )
 
 _RequiredSpigotTypeDef = TypedDict(
     "_RequiredSpigotTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Path": str,
     },
 )
 _OptionalSpigotTypeDef = TypedDict(
     "_OptionalSpigotTypeDef",
     {
         "Topk": int,
         "Prob": float,
     },
     total=False,
 )
 
-
 class SpigotTypeDef(_RequiredSpigotTypeDef, _OptionalSpigotTypeDef):
     pass
 
-
 SplitFieldsTypeDef = TypedDict(
     "SplitFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "Paths": List[List[str]],
+        "Inputs": Sequence[str],
+        "Paths": Sequence[Sequence[str]],
     },
 )
 
 UnionTypeDef = TypedDict(
     "UnionTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "UnionType": UnionTypeType,
     },
 )
 
+CodeGenEdgeOutputTypeDef = TypedDict(
+    "CodeGenEdgeOutputTypeDef",
+    {
+        "Source": str,
+        "Target": str,
+        "TargetParameter": str,
+    },
+)
+
 _RequiredCodeGenEdgeTypeDef = TypedDict(
     "_RequiredCodeGenEdgeTypeDef",
     {
         "Source": str,
         "Target": str,
     },
 )
@@ -1731,18 +2211,25 @@
     "_OptionalCodeGenEdgeTypeDef",
     {
         "TargetParameter": str,
     },
     total=False,
 )
 
-
 class CodeGenEdgeTypeDef(_RequiredCodeGenEdgeTypeDef, _OptionalCodeGenEdgeTypeDef):
     pass
 
+CodeGenNodeArgOutputTypeDef = TypedDict(
+    "CodeGenNodeArgOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+        "Param": bool,
+    },
+)
 
 _RequiredCodeGenNodeArgTypeDef = TypedDict(
     "_RequiredCodeGenNodeArgTypeDef",
     {
         "Name": str,
         "Value": str,
     },
@@ -1751,60 +2238,104 @@
     "_OptionalCodeGenNodeArgTypeDef",
     {
         "Param": bool,
     },
     total=False,
 )
 
-
 class CodeGenNodeArgTypeDef(_RequiredCodeGenNodeArgTypeDef, _OptionalCodeGenNodeArgTypeDef):
     pass
 
-
 ColumnImportanceTypeDef = TypedDict(
     "ColumnImportanceTypeDef",
     {
         "ColumnName": str,
         "Importance": float,
     },
-    total=False,
+)
+
+ColumnOutputTypeDef = TypedDict(
+    "ColumnOutputTypeDef",
+    {
+        "Name": str,
+        "Type": str,
+        "Comment": str,
+        "Parameters": Dict[str, str],
+    },
 )
 
 ColumnRowFilterTypeDef = TypedDict(
     "ColumnRowFilterTypeDef",
     {
         "ColumnName": str,
         "RowFilterExpression": str,
     },
-    total=False,
+)
+
+DateColumnStatisticsDataOutputTypeDef = TypedDict(
+    "DateColumnStatisticsDataOutputTypeDef",
+    {
+        "MinimumValue": datetime,
+        "MaximumValue": datetime,
+        "NumberOfNulls": int,
+        "NumberOfDistinctValues": int,
+    },
+)
+
+DoubleColumnStatisticsDataOutputTypeDef = TypedDict(
+    "DoubleColumnStatisticsDataOutputTypeDef",
+    {
+        "MinimumValue": float,
+        "MaximumValue": float,
+        "NumberOfNulls": int,
+        "NumberOfDistinctValues": int,
+    },
+)
+
+LongColumnStatisticsDataOutputTypeDef = TypedDict(
+    "LongColumnStatisticsDataOutputTypeDef",
+    {
+        "MinimumValue": int,
+        "MaximumValue": int,
+        "NumberOfNulls": int,
+        "NumberOfDistinctValues": int,
+    },
+)
+
+StringColumnStatisticsDataOutputTypeDef = TypedDict(
+    "StringColumnStatisticsDataOutputTypeDef",
+    {
+        "MaximumLength": int,
+        "AverageLength": float,
+        "NumberOfNulls": int,
+        "NumberOfDistinctValues": int,
+    },
 )
 
 _RequiredDateColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDateColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
 _OptionalDateColumnStatisticsDataTypeDef = TypedDict(
     "_OptionalDateColumnStatisticsDataTypeDef",
     {
-        "MinimumValue": datetime,
-        "MaximumValue": datetime,
+        "MinimumValue": Union[datetime, str],
+        "MaximumValue": Union[datetime, str],
     },
     total=False,
 )
 
-
 class DateColumnStatisticsDataTypeDef(
     _RequiredDateColumnStatisticsDataTypeDef, _OptionalDateColumnStatisticsDataTypeDef
 ):
     pass
 
-
 _RequiredDoubleColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDoubleColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1813,21 +2344,19 @@
     {
         "MinimumValue": float,
         "MaximumValue": float,
     },
     total=False,
 )
 
-
 class DoubleColumnStatisticsDataTypeDef(
     _RequiredDoubleColumnStatisticsDataTypeDef, _OptionalDoubleColumnStatisticsDataTypeDef
 ):
     pass
 
-
 _RequiredLongColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredLongColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1836,21 +2365,19 @@
     {
         "MinimumValue": int,
         "MaximumValue": int,
     },
     total=False,
 )
 
-
 class LongColumnStatisticsDataTypeDef(
     _RequiredLongColumnStatisticsDataTypeDef, _OptionalLongColumnStatisticsDataTypeDef
 ):
     pass
 
-
 StringColumnStatisticsDataTypeDef = TypedDict(
     "StringColumnStatisticsDataTypeDef",
     {
         "MaximumLength": int,
         "AverageLength": float,
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
@@ -1869,18 +2396,27 @@
         "Type": str,
         "Comment": str,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ColumnTypeDef(_RequiredColumnTypeDef, _OptionalColumnTypeDef):
     pass
 
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "LogicalOperator": Literal["EQUALS"],
+        "JobName": str,
+        "State": JobRunStateType,
+        "CrawlerName": str,
+        "CrawlState": CrawlStateType,
+    },
+)
 
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "LogicalOperator": Literal["EQUALS"],
         "JobName": str,
         "State": JobRunStateType,
@@ -1894,67 +2430,87 @@
     "ConfusionMatrixTypeDef",
     {
         "NumTruePositives": int,
         "NumFalsePositives": int,
         "NumTrueNegatives": int,
         "NumFalseNegatives": int,
     },
-    total=False,
 )
 
 PhysicalConnectionRequirementsTypeDef = TypedDict(
     "PhysicalConnectionRequirementsTypeDef",
     {
         "SubnetId": str,
         "SecurityGroupIdList": Sequence[str],
         "AvailabilityZone": str,
     },
     total=False,
 )
 
+ConnectionPasswordEncryptionOutputTypeDef = TypedDict(
+    "ConnectionPasswordEncryptionOutputTypeDef",
+    {
+        "ReturnConnectionPasswordEncrypted": bool,
+        "AwsKmsKeyId": str,
+    },
+)
+
 _RequiredConnectionPasswordEncryptionTypeDef = TypedDict(
     "_RequiredConnectionPasswordEncryptionTypeDef",
     {
         "ReturnConnectionPasswordEncrypted": bool,
     },
 )
 _OptionalConnectionPasswordEncryptionTypeDef = TypedDict(
     "_OptionalConnectionPasswordEncryptionTypeDef",
     {
         "AwsKmsKeyId": str,
     },
     total=False,
 )
 
-
 class ConnectionPasswordEncryptionTypeDef(
     _RequiredConnectionPasswordEncryptionTypeDef, _OptionalConnectionPasswordEncryptionTypeDef
 ):
     pass
 
+PhysicalConnectionRequirementsOutputTypeDef = TypedDict(
+    "PhysicalConnectionRequirementsOutputTypeDef",
+    {
+        "SubnetId": str,
+        "SecurityGroupIdList": List[str],
+        "AvailabilityZone": str,
+    },
+)
+
+ConnectionsListOutputTypeDef = TypedDict(
+    "ConnectionsListOutputTypeDef",
+    {
+        "Connections": List[str],
+    },
+)
 
 ConnectionsListTypeDef = TypedDict(
     "ConnectionsListTypeDef",
     {
-        "Connections": List[str],
+        "Connections": Sequence[str],
     },
     total=False,
 )
 
 CrawlTypeDef = TypedDict(
     "CrawlTypeDef",
     {
         "State": CrawlStateType,
         "StartedOn": datetime,
         "CompletedOn": datetime,
         "ErrorMessage": str,
         "LogGroup": str,
         "LogStream": str,
     },
-    total=False,
 )
 
 CrawlerHistoryTypeDef = TypedDict(
     "CrawlerHistoryTypeDef",
     {
         "CrawlId": str,
         "State": CrawlerHistoryStateType,
@@ -1963,36 +2519,94 @@
         "Summary": str,
         "ErrorMessage": str,
         "LogGroup": str,
         "LogStream": str,
         "MessagePrefix": str,
         "DPUHour": float,
     },
-    total=False,
 )
 
 CrawlerMetricsTypeDef = TypedDict(
     "CrawlerMetricsTypeDef",
     {
         "CrawlerName": str,
         "TimeLeftSeconds": float,
         "StillEstimating": bool,
         "LastRuntimeSeconds": float,
         "MedianRuntimeSeconds": float,
         "TablesCreated": int,
         "TablesUpdated": int,
         "TablesDeleted": int,
     },
-    total=False,
+)
+
+DeltaTargetOutputTypeDef = TypedDict(
+    "DeltaTargetOutputTypeDef",
+    {
+        "DeltaTables": List[str],
+        "ConnectionName": str,
+        "WriteManifest": bool,
+        "CreateNativeDeltaTable": bool,
+    },
+)
+
+DynamoDBTargetOutputTypeDef = TypedDict(
+    "DynamoDBTargetOutputTypeDef",
+    {
+        "Path": str,
+        "scanAll": bool,
+        "scanRate": float,
+    },
+)
+
+IcebergTargetOutputTypeDef = TypedDict(
+    "IcebergTargetOutputTypeDef",
+    {
+        "Paths": List[str],
+        "ConnectionName": str,
+        "Exclusions": List[str],
+        "MaximumTraversalDepth": int,
+    },
+)
+
+JdbcTargetOutputTypeDef = TypedDict(
+    "JdbcTargetOutputTypeDef",
+    {
+        "ConnectionName": str,
+        "Path": str,
+        "Exclusions": List[str],
+        "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
+    },
+)
+
+MongoDBTargetOutputTypeDef = TypedDict(
+    "MongoDBTargetOutputTypeDef",
+    {
+        "ConnectionName": str,
+        "Path": str,
+        "ScanAll": bool,
+    },
+)
+
+S3TargetOutputTypeDef = TypedDict(
+    "S3TargetOutputTypeDef",
+    {
+        "Path": str,
+        "Exclusions": List[str],
+        "ConnectionName": str,
+        "SampleSize": int,
+        "EventQueueArn": str,
+        "DlqEventQueueArn": str,
+    },
 )
 
 DeltaTargetTypeDef = TypedDict(
     "DeltaTargetTypeDef",
     {
-        "DeltaTables": List[str],
+        "DeltaTables": Sequence[str],
         "ConnectionName": str,
         "WriteManifest": bool,
         "CreateNativeDeltaTable": bool,
     },
     total=False,
 )
 
@@ -2005,29 +2619,29 @@
     },
     total=False,
 )
 
 IcebergTargetTypeDef = TypedDict(
     "IcebergTargetTypeDef",
     {
-        "Paths": List[str],
+        "Paths": Sequence[str],
         "ConnectionName": str,
-        "Exclusions": List[str],
+        "Exclusions": Sequence[str],
         "MaximumTraversalDepth": int,
     },
     total=False,
 )
 
 JdbcTargetTypeDef = TypedDict(
     "JdbcTargetTypeDef",
     {
         "ConnectionName": str,
         "Path": str,
-        "Exclusions": List[str],
-        "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
+        "Exclusions": Sequence[str],
+        "EnableAdditionalMetadata": Sequence[JdbcMetadataEntryType],
     },
     total=False,
 )
 
 MongoDBTargetTypeDef = TypedDict(
     "MongoDBTargetTypeDef",
     {
@@ -2038,77 +2652,71 @@
     total=False,
 )
 
 S3TargetTypeDef = TypedDict(
     "S3TargetTypeDef",
     {
         "Path": str,
-        "Exclusions": List[str],
+        "Exclusions": Sequence[str],
         "ConnectionName": str,
         "SampleSize": int,
         "EventQueueArn": str,
         "DlqEventQueueArn": str,
     },
     total=False,
 )
 
-LakeFormationConfigurationTypeDef = TypedDict(
-    "LakeFormationConfigurationTypeDef",
+LakeFormationConfigurationOutputTypeDef = TypedDict(
+    "LakeFormationConfigurationOutputTypeDef",
     {
         "UseLakeFormationCredentials": bool,
         "AccountId": str,
     },
-    total=False,
 )
 
 LastCrawlInfoTypeDef = TypedDict(
     "LastCrawlInfoTypeDef",
     {
         "Status": LastCrawlStatusType,
         "ErrorMessage": str,
         "LogGroup": str,
         "LogStream": str,
         "MessagePrefix": str,
         "StartTime": datetime,
     },
-    total=False,
 )
 
-LineageConfigurationTypeDef = TypedDict(
-    "LineageConfigurationTypeDef",
+LineageConfigurationOutputTypeDef = TypedDict(
+    "LineageConfigurationOutputTypeDef",
     {
         "CrawlerLineageSettings": CrawlerLineageSettingsType,
     },
-    total=False,
 )
 
-RecrawlPolicyTypeDef = TypedDict(
-    "RecrawlPolicyTypeDef",
+RecrawlPolicyOutputTypeDef = TypedDict(
+    "RecrawlPolicyOutputTypeDef",
     {
         "RecrawlBehavior": RecrawlBehaviorType,
     },
-    total=False,
 )
 
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "ScheduleExpression": str,
         "State": ScheduleStateType,
     },
-    total=False,
 )
 
-SchemaChangePolicyTypeDef = TypedDict(
-    "SchemaChangePolicyTypeDef",
+SchemaChangePolicyOutputTypeDef = TypedDict(
+    "SchemaChangePolicyOutputTypeDef",
     {
         "UpdateBehavior": UpdateBehaviorType,
         "DeleteBehavior": DeleteBehaviorType,
     },
-    total=False,
 )
 
 CrawlsFilterTypeDef = TypedDict(
     "CrawlsFilterTypeDef",
     {
         "FieldName": FieldNameType,
         "FilterOperator": FilterOperatorType,
@@ -2129,21 +2737,19 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateBlueprintRequestRequestTypeDef(
     _RequiredCreateBlueprintRequestRequestTypeDef, _OptionalCreateBlueprintRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateCsvClassifierRequestTypeDef = TypedDict(
@@ -2157,21 +2763,19 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateCsvClassifierRequestTypeDef(
     _RequiredCreateCsvClassifierRequestTypeDef, _OptionalCreateCsvClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateGrokClassifierRequestTypeDef",
     {
         "Classification": str,
         "Name": str,
         "GrokPattern": str,
     },
@@ -2180,21 +2784,19 @@
     "_OptionalCreateGrokClassifierRequestTypeDef",
     {
         "CustomPatterns": str,
     },
     total=False,
 )
 
-
 class CreateGrokClassifierRequestTypeDef(
     _RequiredCreateGrokClassifierRequestTypeDef, _OptionalCreateGrokClassifierRequestTypeDef
 ):
     pass
 
-
 CreateJsonClassifierRequestTypeDef = TypedDict(
     "CreateJsonClassifierRequestTypeDef",
     {
         "Name": str,
         "JsonPath": str,
     },
 )
@@ -2210,20 +2812,52 @@
     "_OptionalCreateXMLClassifierRequestTypeDef",
     {
         "RowTag": str,
     },
     total=False,
 )
 
-
 class CreateXMLClassifierRequestTypeDef(
     _RequiredCreateXMLClassifierRequestTypeDef, _OptionalCreateXMLClassifierRequestTypeDef
 ):
     pass
 
+LakeFormationConfigurationTypeDef = TypedDict(
+    "LakeFormationConfigurationTypeDef",
+    {
+        "UseLakeFormationCredentials": bool,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+LineageConfigurationTypeDef = TypedDict(
+    "LineageConfigurationTypeDef",
+    {
+        "CrawlerLineageSettings": CrawlerLineageSettingsType,
+    },
+    total=False,
+)
+
+RecrawlPolicyTypeDef = TypedDict(
+    "RecrawlPolicyTypeDef",
+    {
+        "RecrawlBehavior": RecrawlBehaviorType,
+    },
+    total=False,
+)
+
+SchemaChangePolicyTypeDef = TypedDict(
+    "SchemaChangePolicyTypeDef",
+    {
+        "UpdateBehavior": UpdateBehaviorType,
+        "DeleteBehavior": DeleteBehaviorType,
+    },
+    total=False,
+)
 
 _RequiredCreateCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
         "RegexString": str,
     },
@@ -2233,22 +2867,20 @@
     {
         "ContextWords": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateCustomEntityTypeRequestRequestTypeDef(
     _RequiredCreateCustomEntityTypeRequestRequestTypeDef,
     _OptionalCreateCustomEntityTypeRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDataQualityTargetTableTypeDef = TypedDict(
     "_RequiredDataQualityTargetTableTypeDef",
     {
         "TableName": str,
         "DatabaseName": str,
     },
 )
@@ -2256,21 +2888,19 @@
     "_OptionalDataQualityTargetTableTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DataQualityTargetTableTypeDef(
     _RequiredDataQualityTargetTableTypeDef, _OptionalDataQualityTargetTableTypeDef
 ):
     pass
 
-
 _RequiredCreateDevEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
         "RoleArn": str,
     },
 )
@@ -2290,21 +2920,19 @@
         "SecurityConfiguration": str,
         "Tags": Mapping[str, str],
         "Arguments": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDevEndpointRequestRequestTypeDef(
     _RequiredCreateDevEndpointRequestRequestTypeDef, _OptionalCreateDevEndpointRequestRequestTypeDef
 ):
     pass
 
-
 ExecutionPropertyTypeDef = TypedDict(
     "ExecutionPropertyTypeDef",
     {
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
@@ -2343,24 +2971,22 @@
     },
 )
 _OptionalGlueTableTypeDef = TypedDict(
     "_OptionalGlueTableTypeDef",
     {
         "CatalogId": str,
         "ConnectionName": str,
-        "AdditionalOptions": Dict[str, str],
+        "AdditionalOptions": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
     pass
 
-
 PartitionIndexTypeDef = TypedDict(
     "PartitionIndexTypeDef",
     {
         "Keys": Sequence[str],
         "IndexName": str,
     },
 )
@@ -2376,21 +3002,19 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateRegistryInputRequestTypeDef(
     _RequiredCreateRegistryInputRequestTypeDef, _OptionalCreateRegistryInputRequestTypeDef
 ):
     pass
 
-
 RegistryIdTypeDef = TypedDict(
     "RegistryIdTypeDef",
     {
         "RegistryName": str,
         "RegistryArn": str,
     },
     total=False,
@@ -2415,21 +3039,19 @@
     "_OptionalEventBatchingConditionTypeDef",
     {
         "BatchWindow": int,
     },
     total=False,
 )
 
-
 class EventBatchingConditionTypeDef(
     _RequiredEventBatchingConditionTypeDef, _OptionalEventBatchingConditionTypeDef
 ):
     pass
 
-
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2439,67 +3061,103 @@
         "DefaultRunProperties": Mapping[str, str],
         "Tags": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
-
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
+DQResultsPublishingOptionsOutputTypeDef = TypedDict(
+    "DQResultsPublishingOptionsOutputTypeDef",
+    {
+        "EvaluationContext": str,
+        "ResultsS3Prefix": str,
+        "CloudWatchMetricsEnabled": bool,
+        "ResultsPublishingEnabled": bool,
+    },
+)
 
 DQResultsPublishingOptionsTypeDef = TypedDict(
     "DQResultsPublishingOptionsTypeDef",
     {
         "EvaluationContext": str,
         "ResultsS3Prefix": str,
         "CloudWatchMetricsEnabled": bool,
         "ResultsPublishingEnabled": bool,
     },
     total=False,
 )
 
+DQStopJobOnFailureOptionsOutputTypeDef = TypedDict(
+    "DQStopJobOnFailureOptionsOutputTypeDef",
+    {
+        "StopJobOnFailureTiming": DQStopJobOnFailureTimingType,
+    },
+)
+
 DQStopJobOnFailureOptionsTypeDef = TypedDict(
     "DQStopJobOnFailureOptionsTypeDef",
     {
         "StopJobOnFailureTiming": DQStopJobOnFailureTimingType,
     },
     total=False,
 )
 
+EncryptionAtRestOutputTypeDef = TypedDict(
+    "EncryptionAtRestOutputTypeDef",
+    {
+        "CatalogEncryptionMode": CatalogEncryptionModeType,
+        "SseAwsKmsKeyId": str,
+    },
+)
+
 _RequiredEncryptionAtRestTypeDef = TypedDict(
     "_RequiredEncryptionAtRestTypeDef",
     {
         "CatalogEncryptionMode": CatalogEncryptionModeType,
     },
 )
 _OptionalEncryptionAtRestTypeDef = TypedDict(
     "_OptionalEncryptionAtRestTypeDef",
     {
         "SseAwsKmsKeyId": str,
     },
     total=False,
 )
 
-
 class EncryptionAtRestTypeDef(_RequiredEncryptionAtRestTypeDef, _OptionalEncryptionAtRestTypeDef):
     pass
 
+DataLakePrincipalOutputTypeDef = TypedDict(
+    "DataLakePrincipalOutputTypeDef",
+    {
+        "DataLakePrincipalIdentifier": str,
+    },
+)
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
     total=False,
 )
 
+DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef = TypedDict(
+    "DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef",
+    {
+        "CloudWatchMetricsEnabled": bool,
+        "ResultsS3Prefix": str,
+    },
+)
+
 DataQualityEvaluationRunAdditionalRunOptionsTypeDef = TypedDict(
     "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
     {
         "CloudWatchMetricsEnabled": bool,
         "ResultsS3Prefix": str,
     },
     total=False,
@@ -2510,15 +3168,43 @@
     {
         "Name": str,
         "Description": str,
         "EvaluationMessage": str,
         "Result": DataQualityRuleResultStatusType,
         "EvaluatedMetrics": Dict[str, float],
     },
-    total=False,
+)
+
+DataQualityTargetTableOutputTypeDef = TypedDict(
+    "DataQualityTargetTableOutputTypeDef",
+    {
+        "TableName": str,
+        "DatabaseName": str,
+        "CatalogId": str,
+    },
+)
+
+GlueTableOutputTypeDef = TypedDict(
+    "GlueTableOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "CatalogId": str,
+        "ConnectionName": str,
+        "AdditionalOptions": Dict[str, str],
+    },
+)
+
+DatabaseIdentifierOutputTypeDef = TypedDict(
+    "DatabaseIdentifierOutputTypeDef",
+    {
+        "CatalogId": str,
+        "DatabaseName": str,
+        "Region": str,
+    },
 )
 
 DatabaseIdentifierTypeDef = TypedDict(
     "DatabaseIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
@@ -2532,26 +3218,50 @@
     {
         "Identifier": str,
         "ConnectionName": str,
     },
     total=False,
 )
 
+FederatedDatabaseOutputTypeDef = TypedDict(
+    "FederatedDatabaseOutputTypeDef",
+    {
+        "Identifier": str,
+        "ConnectionName": str,
+    },
+)
+
+DatatypeOutputTypeDef = TypedDict(
+    "DatatypeOutputTypeDef",
+    {
+        "Id": str,
+        "Label": str,
+    },
+)
+
 DatatypeTypeDef = TypedDict(
     "DatatypeTypeDef",
     {
         "Id": str,
         "Label": str,
     },
 )
 
+DecimalNumberOutputTypeDef = TypedDict(
+    "DecimalNumberOutputTypeDef",
+    {
+        "UnscaledValue": bytes,
+        "Scale": int,
+    },
+)
+
 DecimalNumberTypeDef = TypedDict(
     "DecimalNumberTypeDef",
     {
-        "UnscaledValue": bytes,
+        "UnscaledValue": Union[str, bytes, IO[Any], StreamingBody],
         "Scale": int,
     },
 )
 
 DeleteBlueprintRequestRequestTypeDef = TypedDict(
     "DeleteBlueprintRequestRequestTypeDef",
     {
@@ -2579,22 +3289,20 @@
     "_OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnName": str,
     },
@@ -2603,43 +3311,39 @@
     "_OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionName": str,
     },
 )
 _OptionalDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteConnectionRequestRequestTypeDef(
     _RequiredDeleteConnectionRequestRequestTypeDef, _OptionalDeleteConnectionRequestRequestTypeDef
 ):
     pass
 
-
 DeleteCrawlerRequestRequestTypeDef = TypedDict(
     "DeleteCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2667,21 +3371,19 @@
     "_OptionalDeleteDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteDatabaseRequestRequestTypeDef(
     _RequiredDeleteDatabaseRequestRequestTypeDef, _OptionalDeleteDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 DeleteDevEndpointRequestRequestTypeDef = TypedDict(
     "DeleteDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 
@@ -2711,22 +3413,20 @@
     "_OptionalDeletePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeletePartitionIndexRequestRequestTypeDef(
     _RequiredDeletePartitionIndexRequestRequestTypeDef,
     _OptionalDeletePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeletePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -2735,21 +3435,19 @@
     "_OptionalDeletePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeletePartitionRequestRequestTypeDef(
     _RequiredDeletePartitionRequestRequestTypeDef, _OptionalDeletePartitionRequestRequestTypeDef
 ):
     pass
 
-
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyHashCondition": str,
         "ResourceArn": str,
     },
     total=False,
@@ -2782,21 +3480,19 @@
     "_OptionalDeleteSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class DeleteSessionRequestRequestTypeDef(
     _RequiredDeleteSessionRequestRequestTypeDef, _OptionalDeleteSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -2805,21 +3501,19 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
-
 class DeleteTableRequestRequestTypeDef(
     _RequiredDeleteTableRequestRequestTypeDef, _OptionalDeleteTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionId": str,
     },
@@ -2828,22 +3522,20 @@
     "_OptionalDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteTableVersionRequestRequestTypeDef(
     _RequiredDeleteTableVersionRequestRequestTypeDef,
     _OptionalDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteTriggerRequestRequestTypeDef = TypedDict(
     "DeleteTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2858,22 +3550,20 @@
     "_OptionalDeleteUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteUserDefinedFunctionRequestRequestTypeDef(
     _RequiredDeleteUserDefinedFunctionRequestRequestTypeDef,
     _OptionalDeleteUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2882,68 +3572,113 @@
     {
         "ExtraPythonLibsS3Path": str,
         "ExtraJarsS3Path": str,
     },
     total=False,
 )
 
+DirectSchemaChangePolicyOutputTypeDef = TypedDict(
+    "DirectSchemaChangePolicyOutputTypeDef",
+    {
+        "EnableUpdateCatalog": bool,
+        "UpdateBehavior": UpdateCatalogBehaviorType,
+        "Table": str,
+        "Database": str,
+    },
+)
+
 DirectSchemaChangePolicyTypeDef = TypedDict(
     "DirectSchemaChangePolicyTypeDef",
     {
         "EnableUpdateCatalog": bool,
         "UpdateBehavior": UpdateCatalogBehaviorType,
         "Table": str,
         "Database": str,
     },
     total=False,
 )
 
+NullCheckBoxListOutputTypeDef = TypedDict(
+    "NullCheckBoxListOutputTypeDef",
+    {
+        "IsEmpty": bool,
+        "IsNullString": bool,
+        "IsNegOne": bool,
+    },
+)
+
 NullCheckBoxListTypeDef = TypedDict(
     "NullCheckBoxListTypeDef",
     {
         "IsEmpty": bool,
         "IsNullString": bool,
         "IsNegOne": bool,
     },
     total=False,
 )
 
+TransformConfigParameterOutputTypeDef = TypedDict(
+    "TransformConfigParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Type": ParamTypeType,
+        "ValidationRule": str,
+        "ValidationMessage": str,
+        "Value": List[str],
+        "ListType": ParamTypeType,
+        "IsOptional": bool,
+    },
+)
+
 _RequiredTransformConfigParameterTypeDef = TypedDict(
     "_RequiredTransformConfigParameterTypeDef",
     {
         "Name": str,
         "Type": ParamTypeType,
     },
 )
 _OptionalTransformConfigParameterTypeDef = TypedDict(
     "_OptionalTransformConfigParameterTypeDef",
     {
         "ValidationRule": str,
         "ValidationMessage": str,
-        "Value": List[str],
+        "Value": Sequence[str],
         "ListType": ParamTypeType,
         "IsOptional": bool,
     },
     total=False,
 )
 
-
 class TransformConfigParameterTypeDef(
     _RequiredTransformConfigParameterTypeDef, _OptionalTransformConfigParameterTypeDef
 ):
     pass
 
-
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "SourceId": str,
         "DestinationId": str,
     },
-    total=False,
+)
+
+JobBookmarksEncryptionOutputTypeDef = TypedDict(
+    "JobBookmarksEncryptionOutputTypeDef",
+    {
+        "JobBookmarksEncryptionMode": JobBookmarksEncryptionModeType,
+        "KmsKeyArn": str,
+    },
+)
+
+S3EncryptionOutputTypeDef = TypedDict(
+    "S3EncryptionOutputTypeDef",
+    {
+        "S3EncryptionMode": S3EncryptionModeType,
+        "KmsKeyArn": str,
+    },
 )
 
 JobBookmarksEncryptionTypeDef = TypedDict(
     "JobBookmarksEncryptionTypeDef",
     {
         "JobBookmarksEncryptionMode": JobBookmarksEncryptionModeType,
         "KmsKeyArn": str,
@@ -2962,40 +3697,70 @@
 
 ErrorDetailsTypeDef = TypedDict(
     "ErrorDetailsTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+EventBatchingConditionOutputTypeDef = TypedDict(
+    "EventBatchingConditionOutputTypeDef",
+    {
+        "BatchSize": int,
+        "BatchWindow": int,
+    },
+)
+
+ExecutionPropertyOutputTypeDef = TypedDict(
+    "ExecutionPropertyOutputTypeDef",
+    {
+        "MaxConcurrentRuns": int,
+    },
 )
 
 ExportLabelsTaskRunPropertiesTypeDef = TypedDict(
     "ExportLabelsTaskRunPropertiesTypeDef",
     {
         "OutputS3Path": str,
     },
-    total=False,
 )
 
 FederatedTableTypeDef = TypedDict(
     "FederatedTableTypeDef",
     {
         "Identifier": str,
         "DatabaseIdentifier": str,
         "ConnectionName": str,
     },
-    total=False,
+)
+
+FilterValueOutputTypeDef = TypedDict(
+    "FilterValueOutputTypeDef",
+    {
+        "Type": FilterValueTypeType,
+        "Value": List[str],
+    },
 )
 
 FilterValueTypeDef = TypedDict(
     "FilterValueTypeDef",
     {
         "Type": FilterValueTypeType,
-        "Value": List[str],
+        "Value": Sequence[str],
+    },
+)
+
+FindMatchesParametersOutputTypeDef = TypedDict(
+    "FindMatchesParametersOutputTypeDef",
+    {
+        "PrimaryKeyColumnName": str,
+        "PrecisionRecallTradeoff": float,
+        "AccuracyCostTradeoff": float,
+        "EnforceProvidedLabels": bool,
     },
 )
 
 FindMatchesParametersTypeDef = TypedDict(
     "FindMatchesParametersTypeDef",
     {
         "PrimaryKeyColumnName": str,
@@ -3009,15 +3774,14 @@
 FindMatchesTaskRunPropertiesTypeDef = TypedDict(
     "FindMatchesTaskRunPropertiesTypeDef",
     {
         "JobId": str,
         "JobName": str,
         "JobRunId": str,
     },
-    total=False,
 )
 
 _RequiredGetBlueprintRequestRequestTypeDef = TypedDict(
     "_RequiredGetBlueprintRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -3027,21 +3791,19 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
-
 class GetBlueprintRequestRequestTypeDef(
     _RequiredGetBlueprintRequestRequestTypeDef, _OptionalGetBlueprintRequestRequestTypeDef
 ):
     pass
 
-
 GetBlueprintRunRequestRequestTypeDef = TypedDict(
     "GetBlueprintRunRequestRequestTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
     },
 )
@@ -3057,21 +3819,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetBlueprintRunsRequestRequestTypeDef(
     _RequiredGetBlueprintRunsRequestRequestTypeDef, _OptionalGetBlueprintRunsRequestRequestTypeDef
 ):
     pass
 
-
 GetCatalogImportStatusRequestRequestTypeDef = TypedDict(
     "GetCatalogImportStatusRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
@@ -3115,22 +3875,20 @@
     "_OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnNames": Sequence[str],
     },
@@ -3139,22 +3897,20 @@
     "_OptionalGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetConnectionRequestRequestTypeDef = TypedDict(
@@ -3162,21 +3918,19 @@
     {
         "CatalogId": str,
         "HidePassword": bool,
     },
     total=False,
 )
 
-
 class GetConnectionRequestRequestTypeDef(
     _RequiredGetConnectionRequestRequestTypeDef, _OptionalGetConnectionRequestRequestTypeDef
 ):
     pass
 
-
 GetConnectionsFilterTypeDef = TypedDict(
     "GetConnectionsFilterTypeDef",
     {
         "MatchCriteria": Sequence[str],
         "ConnectionType": ConnectionTypeType,
     },
     total=False,
@@ -3261,21 +4015,19 @@
     "_OptionalGetDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetDatabaseRequestRequestTypeDef(
     _RequiredGetDatabaseRequestRequestTypeDef, _OptionalGetDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 GetDatabasesRequestRequestTypeDef = TypedDict(
     "GetDatabasesRequestRequestTypeDef",
     {
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
         "ResourceShareType": ResourceShareTypeType,
@@ -3317,33 +4069,30 @@
     "_OptionalGetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
-
 class GetJobBookmarkRequestRequestTypeDef(
     _RequiredGetJobBookmarkRequestRequestTypeDef, _OptionalGetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
-
 JobBookmarkEntryTypeDef = TypedDict(
     "JobBookmarkEntryTypeDef",
     {
         "JobName": str,
         "Version": int,
         "Run": int,
         "Attempt": int,
         "PreviousRunId": str,
         "RunId": str,
         "JobBookmark": str,
     },
-    total=False,
 )
 
 GetJobRequestRequestTypeDef = TypedDict(
     "GetJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
@@ -3360,21 +4109,19 @@
     "_OptionalGetJobRunRequestRequestTypeDef",
     {
         "PredecessorsIncluded": bool,
     },
     total=False,
 )
 
-
 class GetJobRunRequestRequestTypeDef(
     _RequiredGetJobRunRequestRequestTypeDef, _OptionalGetJobRunRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJobRunsRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 _OptionalGetJobRunsRequestRequestTypeDef = TypedDict(
@@ -3382,21 +4129,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetJobRunsRequestRequestTypeDef(
     _RequiredGetJobRunsRequestRequestTypeDef, _OptionalGetJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 GetJobsRequestRequestTypeDef = TypedDict(
     "GetJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3432,42 +4177,40 @@
 GetMLTransformRequestRequestTypeDef = TypedDict(
     "GetMLTransformRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
-SchemaColumnTypeDef = TypedDict(
-    "SchemaColumnTypeDef",
+SchemaColumnOutputTypeDef = TypedDict(
+    "SchemaColumnOutputTypeDef",
     {
         "Name": str,
         "DataType": str,
     },
-    total=False,
 )
 
 TransformSortCriteriaTypeDef = TypedDict(
     "TransformSortCriteriaTypeDef",
     {
         "Column": TransformSortColumnTypeType,
         "SortDirection": SortDirectionTypeType,
     },
 )
 
-MappingEntryTypeDef = TypedDict(
-    "MappingEntryTypeDef",
+MappingEntryOutputTypeDef = TypedDict(
+    "MappingEntryOutputTypeDef",
     {
         "SourceTable": str,
         "SourcePath": str,
         "SourceType": str,
         "TargetTable": str,
         "TargetPath": str,
         "TargetType": str,
     },
-    total=False,
 )
 
 _RequiredGetPartitionIndexesRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionIndexesRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
@@ -3478,22 +4221,20 @@
     {
         "CatalogId": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetPartitionIndexesRequestRequestTypeDef(
     _RequiredGetPartitionIndexesRequestRequestTypeDef,
     _OptionalGetPartitionIndexesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -3502,29 +4243,40 @@
     "_OptionalGetPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetPartitionRequestRequestTypeDef(
     _RequiredGetPartitionRequestRequestTypeDef, _OptionalGetPartitionRequestRequestTypeDef
 ):
     pass
 
-
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentNumber": int,
         "TotalSegments": int,
     },
 )
 
+MappingEntryTypeDef = TypedDict(
+    "MappingEntryTypeDef",
+    {
+        "SourceTable": str,
+        "SourcePath": str,
+        "SourceType": str,
+        "TargetTable": str,
+        "TargetPath": str,
+        "TargetType": str,
+    },
+    total=False,
+)
+
 GetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "GetResourcePoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3534,15 +4286,14 @@
     "GluePolicyTypeDef",
     {
         "PolicyInJson": str,
         "PolicyHash": str,
         "CreateTime": datetime,
         "UpdateTime": datetime,
     },
-    total=False,
 )
 
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
@@ -3584,21 +4335,19 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetStatementRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementRequestRequestTypeDef",
     {
         "SessionId": str,
         "Id": int,
     },
 )
@@ -3606,21 +4355,19 @@
     "_OptionalGetStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class GetStatementRequestRequestTypeDef(
     _RequiredGetStatementRequestRequestTypeDef, _OptionalGetStatementRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTableRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -3630,21 +4377,19 @@
         "CatalogId": str,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetTableRequestRequestTypeDef(
     _RequiredGetTableRequestRequestTypeDef, _OptionalGetTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3653,21 +4398,19 @@
     {
         "CatalogId": str,
         "VersionId": str,
     },
     total=False,
 )
 
-
 class GetTableVersionRequestRequestTypeDef(
     _RequiredGetTableVersionRequestRequestTypeDef, _OptionalGetTableVersionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTableVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3677,21 +4420,19 @@
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetTableVersionsRequestRequestTypeDef(
     _RequiredGetTableVersionsRequestRequestTypeDef, _OptionalGetTableVersionsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTablesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTablesRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestRequestTypeDef = TypedDict(
@@ -3703,21 +4444,19 @@
         "MaxResults": int,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetTablesRequestRequestTypeDef(
     _RequiredGetTablesRequestRequestTypeDef, _OptionalGetTablesRequestRequestTypeDef
 ):
     pass
 
-
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -3749,22 +4488,20 @@
     "_OptionalGetUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetUserDefinedFunctionRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUserDefinedFunctionsRequestRequestTypeDef",
     {
         "Pattern": str,
     },
 )
 _OptionalGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
@@ -3774,43 +4511,39 @@
         "DatabaseName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetUserDefinedFunctionsRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionsRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalGetWorkflowRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
-
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
-
 GetWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -3826,21 +4559,19 @@
     "_OptionalGetWorkflowRunRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
-
 class GetWorkflowRunRequestRequestTypeDef(
     _RequiredGetWorkflowRunRequestRequestTypeDef, _OptionalGetWorkflowRunRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetWorkflowRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRunsRequestRequestTypeDef = TypedDict(
@@ -3849,20 +4580,26 @@
         "IncludeGraph": bool,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetWorkflowRunsRequestRequestTypeDef(
     _RequiredGetWorkflowRunsRequestRequestTypeDef, _OptionalGetWorkflowRunsRequestRequestTypeDef
 ):
     pass
 
+GlueStudioSchemaColumnOutputTypeDef = TypedDict(
+    "GlueStudioSchemaColumnOutputTypeDef",
+    {
+        "Name": str,
+        "Type": str,
+    },
+)
 
 _RequiredGlueStudioSchemaColumnTypeDef = TypedDict(
     "_RequiredGlueStudioSchemaColumnTypeDef",
     {
         "Name": str,
     },
 )
@@ -3870,20 +4607,26 @@
     "_OptionalGlueStudioSchemaColumnTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-
 class GlueStudioSchemaColumnTypeDef(
     _RequiredGlueStudioSchemaColumnTypeDef, _OptionalGlueStudioSchemaColumnTypeDef
 ):
     pass
 
+S3SourceAdditionalOptionsOutputTypeDef = TypedDict(
+    "S3SourceAdditionalOptionsOutputTypeDef",
+    {
+        "BoundedSize": int,
+        "BoundedFiles": int,
+    },
+)
 
 S3SourceAdditionalOptionsTypeDef = TypedDict(
     "S3SourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
     },
@@ -3900,65 +4643,107 @@
     "_OptionalIcebergInputTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class IcebergInputTypeDef(_RequiredIcebergInputTypeDef, _OptionalIcebergInputTypeDef):
     pass
 
-
 ImportCatalogToGlueRequestRequestTypeDef = TypedDict(
     "ImportCatalogToGlueRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
 ImportLabelsTaskRunPropertiesTypeDef = TypedDict(
     "ImportLabelsTaskRunPropertiesTypeDef",
     {
         "InputS3Path": str,
         "Replace": bool,
     },
-    total=False,
 )
 
-JDBCConnectorOptionsTypeDef = TypedDict(
-    "JDBCConnectorOptionsTypeDef",
+JDBCConnectorOptionsOutputTypeDef = TypedDict(
+    "JDBCConnectorOptionsOutputTypeDef",
     {
         "FilterPredicate": str,
         "PartitionColumn": str,
         "LowerBound": int,
         "UpperBound": int,
         "NumPartitions": int,
         "JobBookmarkKeys": List[str],
         "JobBookmarkKeysSortOrder": str,
         "DataTypeMapping": Dict[JDBCDataTypeType, GlueRecordTypeType],
     },
+)
+
+JDBCConnectorOptionsTypeDef = TypedDict(
+    "JDBCConnectorOptionsTypeDef",
+    {
+        "FilterPredicate": str,
+        "PartitionColumn": str,
+        "LowerBound": int,
+        "UpperBound": int,
+        "NumPartitions": int,
+        "JobBookmarkKeys": Sequence[str],
+        "JobBookmarkKeysSortOrder": str,
+        "DataTypeMapping": Mapping[JDBCDataTypeType, GlueRecordTypeType],
+    },
     total=False,
 )
 
+JobCommandOutputTypeDef = TypedDict(
+    "JobCommandOutputTypeDef",
+    {
+        "Name": str,
+        "ScriptLocation": str,
+        "PythonVersion": str,
+        "Runtime": str,
+    },
+)
+
 PredecessorTypeDef = TypedDict(
     "PredecessorTypeDef",
     {
         "JobName": str,
         "RunId": str,
     },
-    total=False,
+)
+
+SourceControlDetailsOutputTypeDef = TypedDict(
+    "SourceControlDetailsOutputTypeDef",
+    {
+        "Provider": SourceControlProviderType,
+        "Repository": str,
+        "Owner": str,
+        "Branch": str,
+        "Folder": str,
+        "LastCommitId": str,
+        "AuthStrategy": SourceControlAuthStrategyType,
+        "AuthToken": str,
+    },
+)
+
+JoinColumnOutputTypeDef = TypedDict(
+    "JoinColumnOutputTypeDef",
+    {
+        "From": str,
+        "Keys": List[List[str]],
+    },
 )
 
 JoinColumnTypeDef = TypedDict(
     "JoinColumnTypeDef",
     {
         "From": str,
-        "Keys": List[List[str]],
+        "Keys": Sequence[Sequence[str]],
     },
 )
 
 KeySchemaElementTypeDef = TypedDict(
     "KeySchemaElementTypeDef",
     {
         "Name": str,
@@ -3967,15 +4752,14 @@
 )
 
 LabelingSetGenerationTaskRunPropertiesTypeDef = TypedDict(
     "LabelingSetGenerationTaskRunPropertiesTypeDef",
     {
         "OutputS3Path": str,
     },
-    total=False,
 )
 
 ListBlueprintsRequestRequestTypeDef = TypedDict(
     "ListBlueprintsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -4039,41 +4823,38 @@
         "RegistryName": str,
         "RegistryArn": str,
         "Description": str,
         "Status": RegistryStatusType,
         "CreatedTime": str,
         "UpdatedTime": str,
     },
-    total=False,
 )
 
 SchemaVersionListItemTypeDef = TypedDict(
     "SchemaVersionListItemTypeDef",
     {
         "SchemaArn": str,
         "SchemaVersionId": str,
         "VersionNumber": int,
         "Status": SchemaVersionStatusType,
         "CreatedTime": str,
     },
-    total=False,
 )
 
 SchemaListItemTypeDef = TypedDict(
     "SchemaListItemTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
         "SchemaArn": str,
         "Description": str,
         "SchemaStatus": SchemaStatusType,
         "CreatedTime": str,
         "UpdatedTime": str,
     },
-    total=False,
 )
 
 ListSessionsRequestRequestTypeDef = TypedDict(
     "ListSessionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -4094,21 +4875,19 @@
     {
         "RequestOrigin": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStatementsRequestRequestTypeDef(
     _RequiredListStatementsRequestRequestTypeDef, _OptionalListStatementsRequestRequestTypeDef
 ):
     pass
 
-
 ListTriggersRequestRequestTypeDef = TypedDict(
     "ListTriggersRequestRequestTypeDef",
     {
         "NextToken": str,
         "DependentJobName": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
@@ -4121,66 +4900,91 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+MLUserDataEncryptionOutputTypeDef = TypedDict(
+    "MLUserDataEncryptionOutputTypeDef",
+    {
+        "MlUserDataEncryptionMode": MLUserDataEncryptionModeStringType,
+        "KmsKeyId": str,
+    },
+)
+
 _RequiredMLUserDataEncryptionTypeDef = TypedDict(
     "_RequiredMLUserDataEncryptionTypeDef",
     {
         "MlUserDataEncryptionMode": MLUserDataEncryptionModeStringType,
     },
 )
 _OptionalMLUserDataEncryptionTypeDef = TypedDict(
     "_OptionalMLUserDataEncryptionTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class MLUserDataEncryptionTypeDef(
     _RequiredMLUserDataEncryptionTypeDef, _OptionalMLUserDataEncryptionTypeDef
 ):
     pass
 
+MappingOutputTypeDef = TypedDict(
+    "MappingOutputTypeDef",
+    {
+        "ToKey": str,
+        "FromPath": List[str],
+        "FromType": str,
+        "ToType": str,
+        "Dropped": bool,
+        "Children": List[Dict[str, Any]],
+    },
+)
 
 MappingTypeDef = TypedDict(
     "MappingTypeDef",
     {
         "ToKey": str,
-        "FromPath": List[str],
+        "FromPath": Sequence[str],
         "FromType": str,
         "ToType": str,
         "Dropped": bool,
-        "Children": List[Dict[str, Any]],
+        "Children": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
 OtherMetadataValueListItemTypeDef = TypedDict(
     "OtherMetadataValueListItemTypeDef",
     {
         "MetadataValue": str,
         "CreatedTime": str,
     },
-    total=False,
 )
 
 MetadataKeyValuePairTypeDef = TypedDict(
     "MetadataKeyValuePairTypeDef",
     {
         "MetadataKey": str,
         "MetadataValue": str,
     },
     total=False,
 )
 
+OrderOutputTypeDef = TypedDict(
+    "OrderOutputTypeDef",
+    {
+        "Column": str,
+        "SortOrder": int,
+    },
+)
+
 OrderTypeDef = TypedDict(
     "OrderTypeDef",
     {
         "Column": str,
         "SortOrder": int,
     },
 )
@@ -4208,36 +5012,43 @@
         "PolicyHashCondition": str,
         "PolicyExistsCondition": ExistConditionType,
         "EnableHybrid": EnableHybridValuesType,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
 PutWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
         "RunProperties": Mapping[str, str],
     },
 )
 
+UpsertRedshiftTargetOptionsOutputTypeDef = TypedDict(
+    "UpsertRedshiftTargetOptionsOutputTypeDef",
+    {
+        "TableLocation": str,
+        "ConnectionName": str,
+        "UpsertKeys": List[str],
+    },
+)
+
 UpsertRedshiftTargetOptionsTypeDef = TypedDict(
     "UpsertRedshiftTargetOptionsTypeDef",
     {
         "TableLocation": str,
         "ConnectionName": str,
-        "UpsertKeys": List[str],
+        "UpsertKeys": Sequence[str],
     },
     total=False,
 )
 
 _RequiredResetJobBookmarkRequestRequestTypeDef = TypedDict(
     "_RequiredResetJobBookmarkRequestRequestTypeDef",
     {
@@ -4248,20 +5059,26 @@
     "_OptionalResetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
-
 class ResetJobBookmarkRequestRequestTypeDef(
     _RequiredResetJobBookmarkRequestRequestTypeDef, _OptionalResetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
+ResourceUriOutputTypeDef = TypedDict(
+    "ResourceUriOutputTypeDef",
+    {
+        "ResourceType": ResourceTypeType,
+        "Uri": str,
+    },
+)
 
 ResourceUriTypeDef = TypedDict(
     "ResourceUriTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Uri": str,
     },
@@ -4288,61 +5105,121 @@
     "_OptionalRunStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class RunStatementRequestRequestTypeDef(
     _RequiredRunStatementRequestRequestTypeDef, _OptionalRunStatementRequestRequestTypeDef
 ):
     pass
 
+S3DirectSourceAdditionalOptionsOutputTypeDef = TypedDict(
+    "S3DirectSourceAdditionalOptionsOutputTypeDef",
+    {
+        "BoundedSize": int,
+        "BoundedFiles": int,
+        "EnableSamplePath": bool,
+        "SamplePath": str,
+    },
+)
 
 S3DirectSourceAdditionalOptionsTypeDef = TypedDict(
     "S3DirectSourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
         "EnableSamplePath": bool,
         "SamplePath": str,
     },
     total=False,
 )
 
+SchemaColumnTypeDef = TypedDict(
+    "SchemaColumnTypeDef",
+    {
+        "Name": str,
+        "DataType": str,
+    },
+    total=False,
+)
+
+SchemaIdOutputTypeDef = TypedDict(
+    "SchemaIdOutputTypeDef",
+    {
+        "SchemaArn": str,
+        "SchemaName": str,
+        "RegistryName": str,
+    },
+)
+
 SortCriterionTypeDef = TypedDict(
     "SortCriterionTypeDef",
     {
         "FieldName": str,
         "Sort": SortType,
     },
     total=False,
 )
 
+SerDeInfoOutputTypeDef = TypedDict(
+    "SerDeInfoOutputTypeDef",
+    {
+        "Name": str,
+        "SerializationLibrary": str,
+        "Parameters": Dict[str, str],
+    },
+)
+
 SerDeInfoTypeDef = TypedDict(
     "SerDeInfoTypeDef",
     {
         "Name": str,
         "SerializationLibrary": str,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+SessionCommandOutputTypeDef = TypedDict(
+    "SessionCommandOutputTypeDef",
+    {
+        "Name": str,
+        "PythonVersion": str,
+    },
+)
+
+SkewedInfoOutputTypeDef = TypedDict(
+    "SkewedInfoOutputTypeDef",
+    {
+        "SkewedColumnNames": List[str],
+        "SkewedColumnValues": List[str],
+        "SkewedColumnValueLocationMaps": Dict[str, str],
+    },
+)
+
 SkewedInfoTypeDef = TypedDict(
     "SkewedInfoTypeDef",
     {
         "SkewedColumnNames": Sequence[str],
         "SkewedColumnValues": Sequence[str],
         "SkewedColumnValueLocationMaps": Mapping[str, str],
     },
     total=False,
 )
 
+SqlAliasOutputTypeDef = TypedDict(
+    "SqlAliasOutputTypeDef",
+    {
+        "From": str,
+        "Alias": str,
+    },
+)
+
 SqlAliasTypeDef = TypedDict(
     "SqlAliasTypeDef",
     {
         "From": str,
         "Alias": str,
     },
 )
@@ -4358,21 +5235,19 @@
     "_OptionalStartBlueprintRunRequestRequestTypeDef",
     {
         "Parameters": str,
     },
     total=False,
 )
 
-
 class StartBlueprintRunRequestRequestTypeDef(
     _RequiredStartBlueprintRunRequestRequestTypeDef, _OptionalStartBlueprintRunRequestRequestTypeDef
 ):
     pass
 
-
 StartCrawlerRequestRequestTypeDef = TypedDict(
     "StartCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4402,22 +5277,20 @@
     "_OptionalStartImportLabelsTaskRunRequestRequestTypeDef",
     {
         "ReplaceAllLabels": bool,
     },
     total=False,
 )
 
-
 class StartImportLabelsTaskRunRequestRequestTypeDef(
     _RequiredStartImportLabelsTaskRunRequestRequestTypeDef,
     _OptionalStartImportLabelsTaskRunRequestRequestTypeDef,
 ):
     pass
 
-
 StartMLEvaluationTaskRunRequestRequestTypeDef = TypedDict(
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
@@ -4446,36 +5319,32 @@
     "_OptionalStartWorkflowRunRequestRequestTypeDef",
     {
         "RunProperties": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartWorkflowRunRequestRequestTypeDef(
     _RequiredStartWorkflowRunRequestRequestTypeDef, _OptionalStartWorkflowRunRequestRequestTypeDef
 ):
     pass
 
-
 StartingEventBatchConditionTypeDef = TypedDict(
     "StartingEventBatchConditionTypeDef",
     {
         "BatchSize": int,
         "BatchWindow": int,
     },
-    total=False,
 )
 
 StatementOutputDataTypeDef = TypedDict(
     "StatementOutputDataTypeDef",
     {
         "TextPlain": str,
     },
-    total=False,
 )
 
 StopCrawlerRequestRequestTypeDef = TypedDict(
     "StopCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -4498,21 +5367,19 @@
     "_OptionalStopSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class StopSessionRequestRequestTypeDef(
     _RequiredStopSessionRequestRequestTypeDef, _OptionalStopSessionRequestRequestTypeDef
 ):
     pass
 
-
 StopTriggerRequestRequestTypeDef = TypedDict(
     "StopTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4520,14 +5387,24 @@
     "StopWorkflowRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
 
+TableIdentifierOutputTypeDef = TypedDict(
+    "TableIdentifierOutputTypeDef",
+    {
+        "CatalogId": str,
+        "DatabaseName": str,
+        "Name": str,
+        "Region": str,
+    },
+)
+
 TableIdentifierTypeDef = TypedDict(
     "TableIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
         "Region": str,
@@ -4562,21 +5439,19 @@
     "_OptionalUpdateBlueprintRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateBlueprintRequestRequestTypeDef(
     _RequiredUpdateBlueprintRequestRequestTypeDef, _OptionalUpdateBlueprintRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCsvClassifierRequestTypeDef = TypedDict(
@@ -4590,21 +5465,19 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateCsvClassifierRequestTypeDef(
     _RequiredUpdateCsvClassifierRequestTypeDef, _OptionalUpdateCsvClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateGrokClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateGrokClassifierRequestTypeDef = TypedDict(
@@ -4613,42 +5486,38 @@
         "Classification": str,
         "GrokPattern": str,
         "CustomPatterns": str,
     },
     total=False,
 )
 
-
 class UpdateGrokClassifierRequestTypeDef(
     _RequiredUpdateGrokClassifierRequestTypeDef, _OptionalUpdateGrokClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateJsonClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_OptionalUpdateJsonClassifierRequestTypeDef",
     {
         "JsonPath": str,
     },
     total=False,
 )
 
-
 class UpdateJsonClassifierRequestTypeDef(
     _RequiredUpdateJsonClassifierRequestTypeDef, _OptionalUpdateJsonClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateXMLClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateXMLClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateXMLClassifierRequestTypeDef = TypedDict(
@@ -4656,43 +5525,39 @@
     {
         "Classification": str,
         "RowTag": str,
     },
     total=False,
 )
 
-
 class UpdateXMLClassifierRequestTypeDef(
     _RequiredUpdateXMLClassifierRequestTypeDef, _OptionalUpdateXMLClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "CrawlerName": str,
     },
 )
 _OptionalUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "Schedule": str,
     },
     total=False,
 )
 
-
 class UpdateCrawlerScheduleRequestRequestTypeDef(
     _RequiredUpdateCrawlerScheduleRequestRequestTypeDef,
     _OptionalUpdateCrawlerScheduleRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataQualityRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
@@ -4700,22 +5565,20 @@
     {
         "Description": str,
         "Ruleset": str,
     },
     total=False,
 )
 
-
 class UpdateDataQualityRulesetRequestRequestTypeDef(
     _RequiredUpdateDataQualityRulesetRequestRequestTypeDef,
     _OptionalUpdateDataQualityRulesetRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateJobFromSourceControlRequestRequestTypeDef = TypedDict(
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     {
         "JobName": str,
         "Provider": SourceControlProviderType,
         "RepositoryName": str,
         "RepositoryOwner": str,
@@ -4756,41 +5619,50 @@
         "Description": str,
         "DefaultRunProperties": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
-
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
-
 WorkflowRunStatisticsTypeDef = TypedDict(
     "WorkflowRunStatisticsTypeDef",
     {
         "TotalActions": int,
         "TimeoutActions": int,
         "FailedActions": int,
         "StoppedActions": int,
         "SucceededActions": int,
         "RunningActions": int,
         "ErroredActions": int,
         "WaitingActions": int,
     },
-    total=False,
+)
+
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "JobName": str,
+        "Arguments": Dict[str, str],
+        "Timeout": int,
+        "SecurityConfiguration": str,
+        "NotificationProperty": NotificationPropertyOutputTypeDef,
+        "CrawlerName": str,
+    },
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "JobName": str,
-        "Arguments": Dict[str, str],
+        "Arguments": Mapping[str, str],
         "Timeout": int,
         "SecurityConfiguration": str,
         "NotificationProperty": NotificationPropertyTypeDef,
         "CrawlerName": str,
     },
     total=False,
 )
@@ -4814,28 +5686,68 @@
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "ExecutionClass": ExecutionClassType,
     },
     total=False,
 )
 
-
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
+AggregateOutputTypeDef = TypedDict(
+    "AggregateOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Groups": List[List[str]],
+        "Aggs": List[AggregateOperationOutputTypeDef],
+    },
+)
 
 AggregateTypeDef = TypedDict(
     "AggregateTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "Groups": List[List[str]],
-        "Aggs": List[AggregateOperationTypeDef],
+        "Inputs": Sequence[str],
+        "Groups": Sequence[Sequence[str]],
+        "Aggs": Sequence[AggregateOperationTypeDef],
+    },
+)
+
+AmazonRedshiftNodeDataOutputTypeDef = TypedDict(
+    "AmazonRedshiftNodeDataOutputTypeDef",
+    {
+        "AccessType": str,
+        "SourceType": str,
+        "Connection": OptionOutputTypeDef,
+        "Schema": OptionOutputTypeDef,
+        "Table": OptionOutputTypeDef,
+        "CatalogDatabase": OptionOutputTypeDef,
+        "CatalogTable": OptionOutputTypeDef,
+        "CatalogRedshiftSchema": str,
+        "CatalogRedshiftTable": str,
+        "TempDir": str,
+        "IamRole": OptionOutputTypeDef,
+        "AdvancedOptions": List[AmazonRedshiftAdvancedOptionOutputTypeDef],
+        "SampleQuery": str,
+        "PreAction": str,
+        "PostAction": str,
+        "Action": str,
+        "TablePrefix": str,
+        "Upsert": bool,
+        "MergeAction": str,
+        "MergeWhenMatched": str,
+        "MergeWhenNotMatched": str,
+        "MergeClause": str,
+        "CrawlerConnection": str,
+        "TableSchema": List[OptionOutputTypeDef],
+        "StagingTable": str,
+        "SelectedColumns": List[OptionOutputTypeDef],
     },
 )
 
 AmazonRedshiftNodeDataTypeDef = TypedDict(
     "AmazonRedshiftNodeDataTypeDef",
     {
         "AccessType": str,
@@ -4845,29 +5757,29 @@
         "Table": OptionTypeDef,
         "CatalogDatabase": OptionTypeDef,
         "CatalogTable": OptionTypeDef,
         "CatalogRedshiftSchema": str,
         "CatalogRedshiftTable": str,
         "TempDir": str,
         "IamRole": OptionTypeDef,
-        "AdvancedOptions": List[AmazonRedshiftAdvancedOptionTypeDef],
+        "AdvancedOptions": Sequence[AmazonRedshiftAdvancedOptionTypeDef],
         "SampleQuery": str,
         "PreAction": str,
         "PostAction": str,
         "Action": str,
         "TablePrefix": str,
         "Upsert": bool,
         "MergeAction": str,
         "MergeWhenMatched": str,
         "MergeWhenNotMatched": str,
         "MergeClause": str,
         "CrawlerConnection": str,
-        "TableSchema": List[OptionTypeDef],
+        "TableSchema": Sequence[OptionTypeDef],
         "StagingTable": str,
-        "SelectedColumns": List[OptionTypeDef],
+        "SelectedColumns": Sequence[OptionTypeDef],
     },
     total=False,
 )
 
 _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
@@ -4882,22 +5794,20 @@
     "_OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
-
 class GetUnfilteredPartitionMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -4907,78 +5817,28 @@
     "_OptionalGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
-
 class GetUnfilteredTableMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredTableMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 BackfillErrorTypeDef = TypedDict(
     "BackfillErrorTypeDef",
     {
         "Code": BackfillErrorCodeType,
-        "Partitions": List[PartitionValueListTypeDef],
+        "Partitions": List[PartitionValueListOutputTypeDef],
     },
-    total=False,
 )
 
-_RequiredBatchDeletePartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchDeletePartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "PartitionsToDelete": Sequence[PartitionValueListTypeDef],
-    },
-)
-_OptionalBatchDeletePartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchDeletePartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class BatchDeletePartitionRequestRequestTypeDef(
-    _RequiredBatchDeletePartitionRequestRequestTypeDef,
-    _OptionalBatchDeletePartitionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetPartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "PartitionsToGet": Sequence[PartitionValueListTypeDef],
-    },
-)
-_OptionalBatchGetPartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetPartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class BatchGetPartitionRequestRequestTypeDef(
-    _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
-):
-    pass
-
-
 CancelMLTaskRunResponseTypeDef = TypedDict(
     "CancelMLTaskRunResponseTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
         "Status": TaskStatusTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5628,63 +6488,100 @@
 BatchStopJobRunErrorTypeDef = TypedDict(
     "BatchStopJobRunErrorTypeDef",
     {
         "JobName": str,
         "JobRunId": str,
         "ErrorDetail": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 BatchUpdatePartitionFailureEntryTypeDef = TypedDict(
     "BatchUpdatePartitionFailureEntryTypeDef",
     {
         "PartitionValueList": List[str],
         "ErrorDetail": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 ColumnErrorTypeDef = TypedDict(
     "ColumnErrorTypeDef",
     {
         "ColumnName": str,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 PartitionErrorTypeDef = TypedDict(
     "PartitionErrorTypeDef",
     {
         "PartitionValues": List[str],
         "ErrorDetail": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 TableErrorTypeDef = TypedDict(
     "TableErrorTypeDef",
     {
         "TableName": str,
         "ErrorDetail": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 TableVersionErrorTypeDef = TypedDict(
     "TableVersionErrorTypeDef",
     {
         "TableName": str,
         "VersionId": str,
         "ErrorDetail": ErrorDetailTypeDef,
     },
+)
+
+_RequiredBatchDeletePartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchDeletePartitionRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "PartitionsToDelete": Sequence[PartitionValueListTypeDef],
+    },
+)
+_OptionalBatchDeletePartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchDeletePartitionRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class BatchDeletePartitionRequestRequestTypeDef(
+    _RequiredBatchDeletePartitionRequestRequestTypeDef,
+    _OptionalBatchDeletePartitionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetPartitionRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "PartitionsToGet": Sequence[PartitionValueListTypeDef],
+    },
+)
+_OptionalBatchGetPartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetPartitionRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
     total=False,
 )
 
+class BatchGetPartitionRequestRequestTypeDef(
+    _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
+):
+    pass
+
 BatchGetCustomEntityTypesResponseTypeDef = TypedDict(
     "BatchGetCustomEntityTypesResponseTypeDef",
     {
         "CustomEntityTypes": List[CustomEntityTypeTypeDef],
         "CustomEntityTypesNotFound": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5752,25 +6649,48 @@
         "ParameterSpec": str,
         "BlueprintLocation": str,
         "BlueprintServiceLocation": str,
         "Status": BlueprintStatusType,
         "ErrorMessage": str,
         "LastActiveDefinition": LastActiveDefinitionTypeDef,
     },
-    total=False,
 )
 
 GetCatalogImportStatusResponseTypeDef = TypedDict(
     "GetCatalogImportStatusResponseTypeDef",
     {
         "ImportStatus": CatalogImportStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CatalogKafkaSourceOutputTypeDef = TypedDict(
+    "CatalogKafkaSourceOutputTypeDef",
+    {
+        "Name": str,
+        "WindowSize": int,
+        "DetectSchema": bool,
+        "Table": str,
+        "Database": str,
+        "StreamingOptions": KafkaStreamingSourceOptionsOutputTypeDef,
+        "DataPreviewOptions": StreamingDataPreviewOptionsOutputTypeDef,
+    },
+)
+
+DirectKafkaSourceOutputTypeDef = TypedDict(
+    "DirectKafkaSourceOutputTypeDef",
+    {
+        "Name": str,
+        "StreamingOptions": KafkaStreamingSourceOptionsOutputTypeDef,
+        "WindowSize": int,
+        "DetectSchema": bool,
+        "DataPreviewOptions": StreamingDataPreviewOptionsOutputTypeDef,
+    },
+)
+
 _RequiredCatalogKafkaSourceTypeDef = TypedDict(
     "_RequiredCatalogKafkaSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
@@ -5782,21 +6702,19 @@
         "DetectSchema": bool,
         "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class CatalogKafkaSourceTypeDef(
     _RequiredCatalogKafkaSourceTypeDef, _OptionalCatalogKafkaSourceTypeDef
 ):
     pass
 
-
 _RequiredDirectKafkaSourceTypeDef = TypedDict(
     "_RequiredDirectKafkaSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKafkaSourceTypeDef = TypedDict(
@@ -5806,20 +6724,42 @@
         "WindowSize": int,
         "DetectSchema": bool,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class DirectKafkaSourceTypeDef(
     _RequiredDirectKafkaSourceTypeDef, _OptionalDirectKafkaSourceTypeDef
 ):
     pass
 
+CatalogKinesisSourceOutputTypeDef = TypedDict(
+    "CatalogKinesisSourceOutputTypeDef",
+    {
+        "Name": str,
+        "WindowSize": int,
+        "DetectSchema": bool,
+        "Table": str,
+        "Database": str,
+        "StreamingOptions": KinesisStreamingSourceOptionsOutputTypeDef,
+        "DataPreviewOptions": StreamingDataPreviewOptionsOutputTypeDef,
+    },
+)
+
+DirectKinesisSourceOutputTypeDef = TypedDict(
+    "DirectKinesisSourceOutputTypeDef",
+    {
+        "Name": str,
+        "WindowSize": int,
+        "DetectSchema": bool,
+        "StreamingOptions": KinesisStreamingSourceOptionsOutputTypeDef,
+        "DataPreviewOptions": StreamingDataPreviewOptionsOutputTypeDef,
+    },
+)
 
 _RequiredCatalogKinesisSourceTypeDef = TypedDict(
     "_RequiredCatalogKinesisSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
@@ -5832,21 +6772,19 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class CatalogKinesisSourceTypeDef(
     _RequiredCatalogKinesisSourceTypeDef, _OptionalCatalogKinesisSourceTypeDef
 ):
     pass
 
-
 _RequiredDirectKinesisSourceTypeDef = TypedDict(
     "_RequiredDirectKinesisSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKinesisSourceTypeDef = TypedDict(
@@ -5856,130 +6794,179 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class DirectKinesisSourceTypeDef(
     _RequiredDirectKinesisSourceTypeDef, _OptionalDirectKinesisSourceTypeDef
 ):
     pass
 
+GovernedCatalogTargetOutputTypeDef = TypedDict(
+    "GovernedCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Table": str,
+        "Database": str,
+        "SchemaChangePolicy": CatalogSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3CatalogTargetOutputTypeDef = TypedDict(
+    "S3CatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Table": str,
+        "Database": str,
+        "SchemaChangePolicy": CatalogSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3DeltaCatalogTargetOutputTypeDef = TypedDict(
+    "S3DeltaCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Table": str,
+        "Database": str,
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": CatalogSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3HudiCatalogTargetOutputTypeDef = TypedDict(
+    "S3HudiCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Table": str,
+        "Database": str,
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": CatalogSchemaChangePolicyOutputTypeDef,
+    },
+)
 
 _RequiredGovernedCatalogTargetTypeDef = TypedDict(
     "_RequiredGovernedCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalGovernedCatalogTargetTypeDef = TypedDict(
     "_OptionalGovernedCatalogTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class GovernedCatalogTargetTypeDef(
     _RequiredGovernedCatalogTargetTypeDef, _OptionalGovernedCatalogTargetTypeDef
 ):
     pass
 
-
 _RequiredS3CatalogTargetTypeDef = TypedDict(
     "_RequiredS3CatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalS3CatalogTargetTypeDef = TypedDict(
     "_OptionalS3CatalogTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
     pass
 
-
 _RequiredS3DeltaCatalogTargetTypeDef = TypedDict(
     "_RequiredS3DeltaCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalS3DeltaCatalogTargetTypeDef = TypedDict(
     "_OptionalS3DeltaCatalogTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
+        "PartitionKeys": Sequence[Sequence[str]],
+        "AdditionalOptions": Mapping[str, str],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3DeltaCatalogTargetTypeDef(
     _RequiredS3DeltaCatalogTargetTypeDef, _OptionalS3DeltaCatalogTargetTypeDef
 ):
     pass
 
-
 _RequiredS3HudiCatalogTargetTypeDef = TypedDict(
     "_RequiredS3HudiCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Table": str,
         "Database": str,
-        "AdditionalOptions": Dict[str, str],
+        "AdditionalOptions": Mapping[str, str],
     },
 )
 _OptionalS3HudiCatalogTargetTypeDef = TypedDict(
     "_OptionalS3HudiCatalogTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3HudiCatalogTargetTypeDef(
     _RequiredS3HudiCatalogTargetTypeDef, _OptionalS3HudiCatalogTargetTypeDef
 ):
     pass
 
-
 ClassifierTypeDef = TypedDict(
     "ClassifierTypeDef",
     {
         "GrokClassifier": GrokClassifierTypeDef,
         "XMLClassifier": XMLClassifierTypeDef,
         "JsonClassifier": JsonClassifierTypeDef,
         "CsvClassifier": CsvClassifierTypeDef,
     },
-    total=False,
+)
+
+CodeGenNodeOutputTypeDef = TypedDict(
+    "CodeGenNodeOutputTypeDef",
+    {
+        "Id": str,
+        "NodeType": str,
+        "Args": List[CodeGenNodeArgOutputTypeDef],
+        "LineNumber": int,
+    },
 )
 
 _RequiredCodeGenNodeTypeDef = TypedDict(
     "_RequiredCodeGenNodeTypeDef",
     {
         "Id": str,
         "NodeType": str,
@@ -5990,49 +6977,54 @@
     "_OptionalCodeGenNodeTypeDef",
     {
         "LineNumber": int,
     },
     total=False,
 )
 
-
 class CodeGenNodeTypeDef(_RequiredCodeGenNodeTypeDef, _OptionalCodeGenNodeTypeDef):
     pass
 
-
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "Jdbc": Sequence[CodeGenNodeArgTypeDef],
         "S3": Sequence[CodeGenNodeArgTypeDef],
         "DynamoDB": Sequence[CodeGenNodeArgTypeDef],
     },
     total=False,
 )
 
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
+    {
+        "Logical": LogicalType,
+        "Conditions": List[ConditionOutputTypeDef],
+    },
+)
+
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Logical": LogicalType,
-        "Conditions": List[ConditionTypeDef],
+        "Conditions": Sequence[ConditionTypeDef],
     },
     total=False,
 )
 
 FindMatchesMetricsTypeDef = TypedDict(
     "FindMatchesMetricsTypeDef",
     {
         "AreaUnderPRCurve": float,
         "Precision": float,
         "Recall": float,
         "F1": float,
         "ConfusionMatrix": ConfusionMatrixTypeDef,
         "ColumnImportances": List[ColumnImportanceTypeDef],
     },
-    total=False,
 )
 
 _RequiredConnectionInputTypeDef = TypedDict(
     "_RequiredConnectionInputTypeDef",
     {
         "Name": str,
         "ConnectionType": ConnectionTypeType,
@@ -6045,41 +7037,37 @@
         "Description": str,
         "MatchCriteria": Sequence[str],
         "PhysicalConnectionRequirements": PhysicalConnectionRequirementsTypeDef,
     },
     total=False,
 )
 
-
 class ConnectionInputTypeDef(_RequiredConnectionInputTypeDef, _OptionalConnectionInputTypeDef):
     pass
 
-
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "Name": str,
         "Description": str,
         "ConnectionType": ConnectionTypeType,
         "MatchCriteria": List[str],
         "ConnectionProperties": Dict[ConnectionPropertyKeyType, str],
-        "PhysicalConnectionRequirements": PhysicalConnectionRequirementsTypeDef,
+        "PhysicalConnectionRequirements": PhysicalConnectionRequirementsOutputTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "LastUpdatedBy": str,
     },
-    total=False,
 )
 
 CrawlerNodeDetailsTypeDef = TypedDict(
     "CrawlerNodeDetailsTypeDef",
     {
         "Crawls": List[CrawlTypeDef],
     },
-    total=False,
 )
 
 ListCrawlsResponseTypeDef = TypedDict(
     "ListCrawlsResponseTypeDef",
     {
         "Crawls": List[CrawlerHistoryTypeDef],
         "NextToken": str,
@@ -6092,24 +7080,37 @@
     {
         "CrawlerMetricsList": List[CrawlerMetricsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CrawlerTargetsOutputTypeDef = TypedDict(
+    "CrawlerTargetsOutputTypeDef",
+    {
+        "S3Targets": List[S3TargetOutputTypeDef],
+        "JdbcTargets": List[JdbcTargetOutputTypeDef],
+        "MongoDBTargets": List[MongoDBTargetOutputTypeDef],
+        "DynamoDBTargets": List[DynamoDBTargetOutputTypeDef],
+        "CatalogTargets": List[CatalogTargetOutputTypeDef],
+        "DeltaTargets": List[DeltaTargetOutputTypeDef],
+        "IcebergTargets": List[IcebergTargetOutputTypeDef],
+    },
+)
+
 CrawlerTargetsTypeDef = TypedDict(
     "CrawlerTargetsTypeDef",
     {
-        "S3Targets": List[S3TargetTypeDef],
-        "JdbcTargets": List[JdbcTargetTypeDef],
-        "MongoDBTargets": List[MongoDBTargetTypeDef],
-        "DynamoDBTargets": List[DynamoDBTargetTypeDef],
-        "CatalogTargets": List[CatalogTargetTypeDef],
-        "DeltaTargets": List[DeltaTargetTypeDef],
-        "IcebergTargets": List[IcebergTargetTypeDef],
+        "S3Targets": Sequence[S3TargetTypeDef],
+        "JdbcTargets": Sequence[JdbcTargetTypeDef],
+        "MongoDBTargets": Sequence[MongoDBTargetTypeDef],
+        "DynamoDBTargets": Sequence[DynamoDBTargetTypeDef],
+        "CatalogTargets": Sequence[CatalogTargetTypeDef],
+        "DeltaTargets": Sequence[DeltaTargetTypeDef],
+        "IcebergTargets": Sequence[IcebergTargetTypeDef],
     },
     total=False,
 )
 
 _RequiredListCrawlsRequestRequestTypeDef = TypedDict(
     "_RequiredListCrawlsRequestRequestTypeDef",
     {
@@ -6122,21 +7123,19 @@
         "MaxResults": int,
         "Filters": Sequence[CrawlsFilterTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListCrawlsRequestRequestTypeDef(
     _RequiredListCrawlsRequestRequestTypeDef, _OptionalListCrawlsRequestRequestTypeDef
 ):
     pass
 
-
 CreateClassifierRequestRequestTypeDef = TypedDict(
     "CreateClassifierRequestRequestTypeDef",
     {
         "GrokClassifier": CreateGrokClassifierRequestTypeDef,
         "XMLClassifier": CreateXMLClassifierRequestTypeDef,
         "JsonClassifier": CreateJsonClassifierRequestTypeDef,
         "CsvClassifier": CreateCsvClassifierRequestTypeDef,
@@ -6158,64 +7157,34 @@
         "Tags": Mapping[str, str],
         "TargetTable": DataQualityTargetTableTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateDataQualityRulesetRequestRequestTypeDef(
     _RequiredCreateDataQualityRulesetRequestRequestTypeDef,
     _OptionalCreateDataQualityRulesetRequestRequestTypeDef,
 ):
     pass
 
-
 DataQualityRulesetFilterCriteriaTypeDef = TypedDict(
     "DataQualityRulesetFilterCriteriaTypeDef",
     {
         "Name": str,
         "Description": str,
         "CreatedBefore": Union[datetime, str],
         "CreatedAfter": Union[datetime, str],
         "LastModifiedBefore": Union[datetime, str],
         "LastModifiedAfter": Union[datetime, str],
         "TargetTable": DataQualityTargetTableTypeDef,
     },
     total=False,
 )
 
-DataQualityRulesetListDetailsTypeDef = TypedDict(
-    "DataQualityRulesetListDetailsTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "CreatedOn": datetime,
-        "LastModifiedOn": datetime,
-        "TargetTable": DataQualityTargetTableTypeDef,
-        "RecommendationRunId": str,
-        "RuleCount": int,
-    },
-    total=False,
-)
-
-GetDataQualityRulesetResponseTypeDef = TypedDict(
-    "GetDataQualityRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Ruleset": str,
-        "TargetTable": DataQualityTargetTableTypeDef,
-        "CreatedOn": datetime,
-        "LastModifiedOn": datetime,
-        "RecommendationRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "GlueTable": GlueTableTypeDef,
     },
 )
 
@@ -6231,22 +7200,20 @@
     "_OptionalCreatePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class CreatePartitionIndexRequestRequestTypeDef(
     _RequiredCreatePartitionIndexRequestRequestTypeDef,
     _OptionalCreatePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSchemaInputRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaInputRequestTypeDef",
     {
         "SchemaName": str,
         "DataFormat": DataFormatType,
     },
 )
@@ -6258,21 +7225,19 @@
         "Description": str,
         "Tags": Mapping[str, str],
         "SchemaDefinition": str,
     },
     total=False,
 )
 
-
 class CreateSchemaInputRequestTypeDef(
     _RequiredCreateSchemaInputRequestTypeDef, _OptionalCreateSchemaInputRequestTypeDef
 ):
     pass
 
-
 DeleteRegistryInputRequestTypeDef = TypedDict(
     "DeleteRegistryInputRequestTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
     },
 )
 
@@ -6324,118 +7289,185 @@
         "GlueVersion": str,
         "Tags": Mapping[str, str],
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class CreateSessionRequestRequestTypeDef(
     _RequiredCreateSessionRequestRequestTypeDef, _OptionalCreateSessionRequestRequestTypeDef
 ):
     pass
 
+EvaluateDataQualityMultiFrameOutputTypeDef = TypedDict(
+    "EvaluateDataQualityMultiFrameOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "AdditionalDataSources": Dict[str, str],
+        "Ruleset": str,
+        "PublishingOptions": DQResultsPublishingOptionsOutputTypeDef,
+        "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
+        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsOutputTypeDef,
+    },
+)
 
-SessionTypeDef = TypedDict(
-    "SessionTypeDef",
+EvaluateDataQualityOutputTypeDef = TypedDict(
+    "EvaluateDataQualityOutputTypeDef",
     {
-        "Id": str,
-        "CreatedOn": datetime,
-        "Status": SessionStatusType,
-        "ErrorMessage": str,
-        "Description": str,
-        "Role": str,
-        "Command": SessionCommandTypeDef,
-        "DefaultArguments": Dict[str, str],
-        "Connections": ConnectionsListTypeDef,
-        "Progress": float,
-        "MaxCapacity": float,
-        "SecurityConfiguration": str,
-        "GlueVersion": str,
+        "Name": str,
+        "Inputs": List[str],
+        "Ruleset": str,
+        "Output": DQTransformOutputType,
+        "PublishingOptions": DQResultsPublishingOptionsOutputTypeDef,
+        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredEvaluateDataQualityMultiFrameTypeDef = TypedDict(
     "_RequiredEvaluateDataQualityMultiFrameTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Ruleset": str,
     },
 )
 _OptionalEvaluateDataQualityMultiFrameTypeDef = TypedDict(
     "_OptionalEvaluateDataQualityMultiFrameTypeDef",
     {
-        "AdditionalDataSources": Dict[str, str],
+        "AdditionalDataSources": Mapping[str, str],
         "PublishingOptions": DQResultsPublishingOptionsTypeDef,
-        "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
+        "AdditionalOptions": Mapping[Literal["performanceTuning.caching"], str],
         "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
     },
     total=False,
 )
 
-
 class EvaluateDataQualityMultiFrameTypeDef(
     _RequiredEvaluateDataQualityMultiFrameTypeDef, _OptionalEvaluateDataQualityMultiFrameTypeDef
 ):
     pass
 
-
 _RequiredEvaluateDataQualityTypeDef = TypedDict(
     "_RequiredEvaluateDataQualityTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Ruleset": str,
     },
 )
 _OptionalEvaluateDataQualityTypeDef = TypedDict(
     "_OptionalEvaluateDataQualityTypeDef",
     {
         "Output": DQTransformOutputType,
         "PublishingOptions": DQResultsPublishingOptionsTypeDef,
         "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
     },
     total=False,
 )
 
-
 class EvaluateDataQualityTypeDef(
     _RequiredEvaluateDataQualityTypeDef, _OptionalEvaluateDataQualityTypeDef
 ):
     pass
 
+DataCatalogEncryptionSettingsOutputTypeDef = TypedDict(
+    "DataCatalogEncryptionSettingsOutputTypeDef",
+    {
+        "EncryptionAtRest": EncryptionAtRestOutputTypeDef,
+        "ConnectionPasswordEncryption": ConnectionPasswordEncryptionOutputTypeDef,
+    },
+)
 
 DataCatalogEncryptionSettingsTypeDef = TypedDict(
     "DataCatalogEncryptionSettingsTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "ConnectionPasswordEncryption": ConnectionPasswordEncryptionTypeDef,
     },
     total=False,
 )
 
+PrincipalPermissionsOutputTypeDef = TypedDict(
+    "PrincipalPermissionsOutputTypeDef",
+    {
+        "Principal": DataLakePrincipalOutputTypeDef,
+        "Permissions": List[PermissionType],
+    },
+)
+
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Permissions": Sequence[PermissionType],
     },
     total=False,
 )
 
+DataQualityRulesetListDetailsTypeDef = TypedDict(
+    "DataQualityRulesetListDetailsTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "CreatedOn": datetime,
+        "LastModifiedOn": datetime,
+        "TargetTable": DataQualityTargetTableOutputTypeDef,
+        "RecommendationRunId": str,
+        "RuleCount": int,
+    },
+)
+
+GetDataQualityRulesetResponseTypeDef = TypedDict(
+    "GetDataQualityRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Ruleset": str,
+        "TargetTable": DataQualityTargetTableOutputTypeDef,
+        "CreatedOn": datetime,
+        "LastModifiedOn": datetime,
+        "RecommendationRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
+    {
+        "GlueTable": GlueTableOutputTypeDef,
+    },
+)
+
+NullValueFieldOutputTypeDef = TypedDict(
+    "NullValueFieldOutputTypeDef",
+    {
+        "Value": str,
+        "Datatype": DatatypeOutputTypeDef,
+    },
+)
+
 NullValueFieldTypeDef = TypedDict(
     "NullValueFieldTypeDef",
     {
         "Value": str,
         "Datatype": DatatypeTypeDef,
     },
 )
 
+DecimalColumnStatisticsDataOutputTypeDef = TypedDict(
+    "DecimalColumnStatisticsDataOutputTypeDef",
+    {
+        "MinimumValue": DecimalNumberOutputTypeDef,
+        "MaximumValue": DecimalNumberOutputTypeDef,
+        "NumberOfNulls": int,
+        "NumberOfDistinctValues": int,
+    },
+)
+
 _RequiredDecimalColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDecimalColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -6444,21 +7476,19 @@
     {
         "MinimumValue": DecimalNumberTypeDef,
         "MaximumValue": DecimalNumberTypeDef,
     },
     total=False,
 )
 
-
 class DecimalColumnStatisticsDataTypeDef(
     _RequiredDecimalColumnStatisticsDataTypeDef, _OptionalDecimalColumnStatisticsDataTypeDef
 ):
     pass
 
-
 DeleteSchemaInputRequestTypeDef = TypedDict(
     "DeleteSchemaInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
     },
 )
 
@@ -6496,21 +7526,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListSchemaVersionsInputRequestTypeDef(
     _RequiredListSchemaVersionsInputRequestTypeDef, _OptionalListSchemaVersionsInputRequestTypeDef
 ):
     pass
 
-
 RegisterSchemaVersionInputRequestTypeDef = TypedDict(
     "RegisterSchemaVersionInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaDefinition": str,
     },
 )
@@ -6541,123 +7569,175 @@
         "UpdateEtlLibraries": bool,
         "DeleteArguments": Sequence[str],
         "AddArguments": Mapping[str, str],
     },
     total=False,
 )
 
-
 class UpdateDevEndpointRequestRequestTypeDef(
     _RequiredUpdateDevEndpointRequestRequestTypeDef, _OptionalUpdateDevEndpointRequestRequestTypeDef
 ):
     pass
 
+S3DeltaDirectTargetOutputTypeDef = TypedDict(
+    "S3DeltaDirectTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Path": str,
+        "Compression": DeltaTargetCompressionTypeType,
+        "Format": TargetFormatType,
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": DirectSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3DirectTargetOutputTypeDef = TypedDict(
+    "S3DirectTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Path": str,
+        "Compression": str,
+        "Format": TargetFormatType,
+        "SchemaChangePolicy": DirectSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3GlueParquetTargetOutputTypeDef = TypedDict(
+    "S3GlueParquetTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Path": str,
+        "Compression": ParquetCompressionTypeType,
+        "SchemaChangePolicy": DirectSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3HudiDirectTargetOutputTypeDef = TypedDict(
+    "S3HudiDirectTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Path": str,
+        "Compression": HudiTargetCompressionTypeType,
+        "PartitionKeys": List[List[str]],
+        "Format": TargetFormatType,
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": DirectSchemaChangePolicyOutputTypeDef,
+    },
+)
 
 _RequiredS3DeltaDirectTargetTypeDef = TypedDict(
     "_RequiredS3DeltaDirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Path": str,
         "Compression": DeltaTargetCompressionTypeType,
         "Format": TargetFormatType,
     },
 )
 _OptionalS3DeltaDirectTargetTypeDef = TypedDict(
     "_OptionalS3DeltaDirectTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
+        "PartitionKeys": Sequence[Sequence[str]],
+        "AdditionalOptions": Mapping[str, str],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3DeltaDirectTargetTypeDef(
     _RequiredS3DeltaDirectTargetTypeDef, _OptionalS3DeltaDirectTargetTypeDef
 ):
     pass
 
-
 _RequiredS3DirectTargetTypeDef = TypedDict(
     "_RequiredS3DirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Path": str,
         "Format": TargetFormatType,
     },
 )
 _OptionalS3DirectTargetTypeDef = TypedDict(
     "_OptionalS3DirectTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "Compression": str,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3DirectTargetTypeDef(_RequiredS3DirectTargetTypeDef, _OptionalS3DirectTargetTypeDef):
     pass
 
-
 _RequiredS3GlueParquetTargetTypeDef = TypedDict(
     "_RequiredS3GlueParquetTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Path": str,
     },
 )
 _OptionalS3GlueParquetTargetTypeDef = TypedDict(
     "_OptionalS3GlueParquetTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "Compression": ParquetCompressionTypeType,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3GlueParquetTargetTypeDef(
     _RequiredS3GlueParquetTargetTypeDef, _OptionalS3GlueParquetTargetTypeDef
 ):
     pass
 
-
 _RequiredS3HudiDirectTargetTypeDef = TypedDict(
     "_RequiredS3HudiDirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Path": str,
         "Compression": HudiTargetCompressionTypeType,
         "Format": TargetFormatType,
-        "AdditionalOptions": Dict[str, str],
+        "AdditionalOptions": Mapping[str, str],
     },
 )
 _OptionalS3HudiDirectTargetTypeDef = TypedDict(
     "_OptionalS3HudiDirectTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3HudiDirectTargetTypeDef(
     _RequiredS3HudiDirectTargetTypeDef, _OptionalS3HudiDirectTargetTypeDef
 ):
     pass
 
+EncryptionConfigurationOutputTypeDef = TypedDict(
+    "EncryptionConfigurationOutputTypeDef",
+    {
+        "S3Encryption": List[S3EncryptionOutputTypeDef],
+        "CloudWatchEncryption": CloudWatchEncryptionOutputTypeDef,
+        "JobBookmarksEncryption": JobBookmarksEncryptionOutputTypeDef,
+    },
+)
 
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "S3Encryption": Sequence[S3EncryptionTypeDef],
         "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
         "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
@@ -6667,36 +7747,50 @@
 
 SchemaVersionErrorItemTypeDef = TypedDict(
     "SchemaVersionErrorItemTypeDef",
     {
         "VersionNumber": int,
         "ErrorDetails": ErrorDetailsTypeDef,
     },
-    total=False,
+)
+
+FilterExpressionOutputTypeDef = TypedDict(
+    "FilterExpressionOutputTypeDef",
+    {
+        "Operation": FilterOperationType,
+        "Negated": bool,
+        "Values": List[FilterValueOutputTypeDef],
+    },
 )
 
 _RequiredFilterExpressionTypeDef = TypedDict(
     "_RequiredFilterExpressionTypeDef",
     {
         "Operation": FilterOperationType,
-        "Values": List[FilterValueTypeDef],
+        "Values": Sequence[FilterValueTypeDef],
     },
 )
 _OptionalFilterExpressionTypeDef = TypedDict(
     "_OptionalFilterExpressionTypeDef",
     {
         "Negated": bool,
     },
     total=False,
 )
 
-
 class FilterExpressionTypeDef(_RequiredFilterExpressionTypeDef, _OptionalFilterExpressionTypeDef):
     pass
 
+TransformParametersOutputTypeDef = TypedDict(
+    "TransformParametersOutputTypeDef",
+    {
+        "TransformType": Literal["FIND_MATCHES"],
+        "FindMatchesParameters": FindMatchesParametersOutputTypeDef,
+    },
+)
 
 _RequiredTransformParametersTypeDef = TypedDict(
     "_RequiredTransformParametersTypeDef",
     {
         "TransformType": Literal["FIND_MATCHES"],
     },
 )
@@ -6704,21 +7798,19 @@
     "_OptionalTransformParametersTypeDef",
     {
         "FindMatchesParameters": FindMatchesParametersTypeDef,
     },
     total=False,
 )
 
-
 class TransformParametersTypeDef(
     _RequiredTransformParametersTypeDef, _OptionalTransformParametersTypeDef
 ):
     pass
 
-
 GetClassifiersRequestGetClassifiersPaginateTypeDef = TypedDict(
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6768,22 +7860,20 @@
     "_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetJobRunsRequestGetJobRunsPaginateTypeDef(
     _RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef,
     _OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef,
 ):
     pass
 
-
 GetJobsRequestGetJobsPaginateTypeDef = TypedDict(
     "GetJobsRequestGetJobsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6800,22 +7890,20 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(
     _RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
     _OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
 ):
     pass
 
-
 GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6840,22 +7928,20 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(
     _RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
     _OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
     "_RequiredGetTablesRequestGetTablesPaginateTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
@@ -6866,22 +7952,20 @@
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetTablesRequestGetTablesPaginateTypeDef(
     _RequiredGetTablesRequestGetTablesPaginateTypeDef,
     _OptionalGetTablesRequestGetTablesPaginateTypeDef,
 ):
     pass
 
-
 GetTriggersRequestGetTriggersPaginateTypeDef = TypedDict(
     "GetTriggersRequestGetTriggersPaginateTypeDef",
     {
         "DependentJobName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6899,22 +7983,20 @@
         "CatalogId": str,
         "DatabaseName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(
     _RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
     _OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
 ):
     pass
 
-
 ListRegistriesInputListRegistriesPaginateTypeDef = TypedDict(
     "ListRegistriesInputListRegistriesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6929,22 +8011,20 @@
     "_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(
     _RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     _OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListSchemasInputListSchemasPaginateTypeDef = TypedDict(
     "ListSchemasInputListSchemasPaginateTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -7002,41 +8082,23 @@
         "MaxResults": int,
         "Filter": TaskRunFilterCriteriaTypeDef,
         "Sort": TaskRunSortCriteriaTypeDef,
     },
     total=False,
 )
 
-
 class GetMLTaskRunsRequestRequestTypeDef(
     _RequiredGetMLTaskRunsRequestRequestTypeDef, _OptionalGetMLTaskRunsRequestRequestTypeDef
 ):
     pass
 
-
-TransformFilterCriteriaTypeDef = TypedDict(
-    "TransformFilterCriteriaTypeDef",
-    {
-        "Name": str,
-        "TransformType": Literal["FIND_MATCHES"],
-        "Status": TransformStatusTypeType,
-        "GlueVersion": str,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
-        "LastModifiedBefore": Union[datetime, str],
-        "LastModifiedAfter": Union[datetime, str],
-        "Schema": Sequence[SchemaColumnTypeDef],
-    },
-    total=False,
-)
-
 GetMappingResponseTypeDef = TypedDict(
     "GetMappingResponseTypeDef",
     {
-        "Mapping": List[MappingEntryTypeDef],
+        "Mapping": List[MappingEntryOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef = TypedDict(
     "_RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef",
     {
@@ -7054,22 +8116,20 @@
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetPartitionsRequestGetPartitionsPaginateTypeDef(
     _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef,
     _OptionalGetPartitionsRequestGetPartitionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetPartitionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -7084,21 +8144,19 @@
         "ExcludeColumnSchema": bool,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetPartitionsRequestRequestTypeDef(
     _RequiredGetPartitionsRequestRequestTypeDef, _OptionalGetPartitionsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -7112,22 +8170,20 @@
         "NextToken": str,
         "Segment": SegmentTypeDef,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetUnfilteredPartitionsMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "GetResourcePoliciesResponseList": List[GluePolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7165,29 +8221,56 @@
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "Compatibility": CompatibilityType,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateSchemaInputRequestTypeDef(
     _RequiredUpdateSchemaInputRequestTypeDef, _OptionalUpdateSchemaInputRequestTypeDef
 ):
     pass
 
+GlueSchemaOutputTypeDef = TypedDict(
+    "GlueSchemaOutputTypeDef",
+    {
+        "Columns": List[GlueStudioSchemaColumnOutputTypeDef],
+    },
+)
 
 GlueSchemaTypeDef = TypedDict(
     "GlueSchemaTypeDef",
     {
-        "Columns": List[GlueStudioSchemaColumnTypeDef],
+        "Columns": Sequence[GlueStudioSchemaColumnTypeDef],
     },
     total=False,
 )
 
+GovernedCatalogSourceOutputTypeDef = TypedDict(
+    "GovernedCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "PartitionPredicate": str,
+        "AdditionalOptions": S3SourceAdditionalOptionsOutputTypeDef,
+    },
+)
+
+S3CatalogSourceOutputTypeDef = TypedDict(
+    "S3CatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "PartitionPredicate": str,
+        "AdditionalOptions": S3SourceAdditionalOptionsOutputTypeDef,
+    },
+)
+
 _RequiredGovernedCatalogSourceTypeDef = TypedDict(
     "_RequiredGovernedCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -7197,21 +8280,19 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
-
 class GovernedCatalogSourceTypeDef(
     _RequiredGovernedCatalogSourceTypeDef, _OptionalGovernedCatalogSourceTypeDef
 ):
     pass
 
-
 _RequiredS3CatalogSourceTypeDef = TypedDict(
     "_RequiredS3CatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -7221,19 +8302,17 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
-
 class S3CatalogSourceTypeDef(_RequiredS3CatalogSourceTypeDef, _OptionalS3CatalogSourceTypeDef):
     pass
 
-
 OpenTableFormatInputTypeDef = TypedDict(
     "OpenTableFormatInputTypeDef",
     {
         "IcebergInput": IcebergInputTypeDef,
     },
     total=False,
 )
@@ -7257,42 +8336,50 @@
         "ExecutionTime": int,
         "Timeout": int,
         "MaxCapacity": float,
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "SecurityConfiguration": str,
         "LogGroupName": str,
-        "NotificationProperty": NotificationPropertyTypeDef,
+        "NotificationProperty": NotificationPropertyOutputTypeDef,
         "GlueVersion": str,
         "DPUSeconds": float,
         "ExecutionClass": ExecutionClassType,
     },
-    total=False,
+)
+
+JoinOutputTypeDef = TypedDict(
+    "JoinOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "JoinType": JoinTypeType,
+        "Columns": List[JoinColumnOutputTypeDef],
+    },
 )
 
 JoinTypeDef = TypedDict(
     "JoinTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "JoinType": JoinTypeType,
-        "Columns": List[JoinColumnTypeDef],
+        "Columns": Sequence[JoinColumnTypeDef],
     },
 )
 
 TaskRunPropertiesTypeDef = TypedDict(
     "TaskRunPropertiesTypeDef",
     {
         "TaskType": TaskTypeType,
         "ImportLabelsTaskRunProperties": ImportLabelsTaskRunPropertiesTypeDef,
         "ExportLabelsTaskRunProperties": ExportLabelsTaskRunPropertiesTypeDef,
         "LabelingSetGenerationTaskRunProperties": LabelingSetGenerationTaskRunPropertiesTypeDef,
         "FindMatchesTaskRunProperties": FindMatchesTaskRunPropertiesTypeDef,
     },
-    total=False,
 )
 
 ListRegistriesResponseTypeDef = TypedDict(
     "ListRegistriesResponseTypeDef",
     {
         "Registries": List[RegistryListItemTypeDef],
         "NextToken": str,
@@ -7314,14 +8401,22 @@
     {
         "Schemas": List[SchemaListItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TransformEncryptionOutputTypeDef = TypedDict(
+    "TransformEncryptionOutputTypeDef",
+    {
+        "MlUserDataEncryption": MLUserDataEncryptionOutputTypeDef,
+        "TaskRunSecurityConfigurationName": str,
+    },
+)
+
 TransformEncryptionTypeDef = TypedDict(
     "TransformEncryptionTypeDef",
     {
         "MlUserDataEncryption": MLUserDataEncryptionTypeDef,
         "TaskRunSecurityConfigurationName": str,
     },
     total=False,
@@ -7330,15 +8425,14 @@
 MetadataInfoTypeDef = TypedDict(
     "MetadataInfoTypeDef",
     {
         "MetadataValue": str,
         "CreatedTime": str,
         "OtherMetadataValueList": List[OtherMetadataValueListItemTypeDef],
     },
-    total=False,
 )
 
 _RequiredPutSchemaVersionMetadataInputRequestTypeDef = TypedDict(
     "_RequiredPutSchemaVersionMetadataInputRequestTypeDef",
     {
         "MetadataKeyValue": MetadataKeyValuePairTypeDef,
     },
@@ -7349,22 +8443,20 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
-
 class PutSchemaVersionMetadataInputRequestTypeDef(
     _RequiredPutSchemaVersionMetadataInputRequestTypeDef,
     _OptionalPutSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
-
 QuerySchemaVersionMetadataInputRequestTypeDef = TypedDict(
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
         "MetadataList": Sequence[MetadataKeyValuePairTypeDef],
@@ -7386,153 +8478,208 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
-
 class RemoveSchemaVersionMetadataInputRequestTypeDef(
     _RequiredRemoveSchemaVersionMetadataInputRequestTypeDef,
     _OptionalRemoveSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
+RedshiftTargetOutputTypeDef = TypedDict(
+    "RedshiftTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
+        "RedshiftTmpDir": str,
+        "TmpDirIAMRole": str,
+        "UpsertRedshiftOptions": UpsertRedshiftTargetOptionsOutputTypeDef,
+    },
+)
 
 _RequiredRedshiftTargetTypeDef = TypedDict(
     "_RequiredRedshiftTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 _OptionalRedshiftTargetTypeDef = TypedDict(
     "_OptionalRedshiftTargetTypeDef",
     {
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
         "UpsertRedshiftOptions": UpsertRedshiftTargetOptionsTypeDef,
     },
     total=False,
 )
 
-
 class RedshiftTargetTypeDef(_RequiredRedshiftTargetTypeDef, _OptionalRedshiftTargetTypeDef):
     pass
 
+UserDefinedFunctionTypeDef = TypedDict(
+    "UserDefinedFunctionTypeDef",
+    {
+        "FunctionName": str,
+        "DatabaseName": str,
+        "ClassName": str,
+        "OwnerName": str,
+        "OwnerType": PrincipalTypeType,
+        "CreateTime": datetime,
+        "ResourceUris": List[ResourceUriOutputTypeDef],
+        "CatalogId": str,
+    },
+)
 
 UserDefinedFunctionInputTypeDef = TypedDict(
     "UserDefinedFunctionInputTypeDef",
     {
         "FunctionName": str,
         "ClassName": str,
         "OwnerName": str,
         "OwnerType": PrincipalTypeType,
         "ResourceUris": Sequence[ResourceUriTypeDef],
     },
     total=False,
 )
 
-UserDefinedFunctionTypeDef = TypedDict(
-    "UserDefinedFunctionTypeDef",
+TransformFilterCriteriaTypeDef = TypedDict(
+    "TransformFilterCriteriaTypeDef",
     {
-        "FunctionName": str,
-        "DatabaseName": str,
-        "ClassName": str,
-        "OwnerName": str,
-        "OwnerType": PrincipalTypeType,
-        "CreateTime": datetime,
-        "ResourceUris": List[ResourceUriTypeDef],
-        "CatalogId": str,
+        "Name": str,
+        "TransformType": Literal["FIND_MATCHES"],
+        "Status": TransformStatusTypeType,
+        "GlueVersion": str,
+        "CreatedBefore": Union[datetime, str],
+        "CreatedAfter": Union[datetime, str],
+        "LastModifiedBefore": Union[datetime, str],
+        "LastModifiedAfter": Union[datetime, str],
+        "Schema": Sequence[SchemaColumnTypeDef],
     },
     total=False,
 )
 
+SchemaReferenceOutputTypeDef = TypedDict(
+    "SchemaReferenceOutputTypeDef",
+    {
+        "SchemaId": SchemaIdOutputTypeDef,
+        "SchemaVersionId": str,
+        "SchemaVersionNumber": int,
+    },
+)
+
 SearchTablesRequestRequestTypeDef = TypedDict(
     "SearchTablesRequestRequestTypeDef",
     {
         "CatalogId": str,
         "NextToken": str,
         "Filters": Sequence[PropertyPredicateTypeDef],
         "SearchText": str,
         "SortCriteria": Sequence[SortCriterionTypeDef],
         "MaxResults": int,
         "ResourceShareType": ResourceShareTypeType,
     },
     total=False,
 )
 
+SessionTypeDef = TypedDict(
+    "SessionTypeDef",
+    {
+        "Id": str,
+        "CreatedOn": datetime,
+        "Status": SessionStatusType,
+        "ErrorMessage": str,
+        "Description": str,
+        "Role": str,
+        "Command": SessionCommandOutputTypeDef,
+        "DefaultArguments": Dict[str, str],
+        "Connections": ConnectionsListOutputTypeDef,
+        "Progress": float,
+        "MaxCapacity": float,
+        "SecurityConfiguration": str,
+        "GlueVersion": str,
+    },
+)
+
 StatementOutputTypeDef = TypedDict(
     "StatementOutputTypeDef",
     {
         "Data": StatementOutputDataTypeDef,
         "ExecutionCount": int,
         "Status": StatementStateType,
         "ErrorName": str,
         "ErrorValue": str,
         "Traceback": List[str],
     },
-    total=False,
 )
 
 UpdateClassifierRequestRequestTypeDef = TypedDict(
     "UpdateClassifierRequestRequestTypeDef",
     {
         "GrokClassifier": UpdateGrokClassifierRequestTypeDef,
         "XMLClassifier": UpdateXMLClassifierRequestTypeDef,
         "JsonClassifier": UpdateJsonClassifierRequestTypeDef,
         "CsvClassifier": UpdateCsvClassifierRequestTypeDef,
     },
     total=False,
 )
 
+AmazonRedshiftSourceOutputTypeDef = TypedDict(
+    "AmazonRedshiftSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Data": AmazonRedshiftNodeDataOutputTypeDef,
+    },
+)
+
+AmazonRedshiftTargetOutputTypeDef = TypedDict(
+    "AmazonRedshiftTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Data": AmazonRedshiftNodeDataOutputTypeDef,
+        "Inputs": List[str],
+    },
+)
+
 AmazonRedshiftSourceTypeDef = TypedDict(
     "AmazonRedshiftSourceTypeDef",
     {
         "Name": str,
         "Data": AmazonRedshiftNodeDataTypeDef,
     },
     total=False,
 )
 
 AmazonRedshiftTargetTypeDef = TypedDict(
     "AmazonRedshiftTargetTypeDef",
     {
         "Name": str,
         "Data": AmazonRedshiftNodeDataTypeDef,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
     },
     total=False,
 )
 
-_RequiredPartitionIndexDescriptorTypeDef = TypedDict(
-    "_RequiredPartitionIndexDescriptorTypeDef",
+PartitionIndexDescriptorTypeDef = TypedDict(
+    "PartitionIndexDescriptorTypeDef",
     {
         "IndexName": str,
         "Keys": List[KeySchemaElementTypeDef],
         "IndexStatus": PartitionIndexStatusType,
-    },
-)
-_OptionalPartitionIndexDescriptorTypeDef = TypedDict(
-    "_OptionalPartitionIndexDescriptorTypeDef",
-    {
         "BackfillErrors": List[BackfillErrorTypeDef],
     },
-    total=False,
 )
 
-
-class PartitionIndexDescriptorTypeDef(
-    _RequiredPartitionIndexDescriptorTypeDef, _OptionalPartitionIndexDescriptorTypeDef
-):
-    pass
-
-
 BatchStopJobRunResponseTypeDef = TypedDict(
     "BatchStopJobRunResponseTypeDef",
     {
         "SuccessfulSubmissions": List[BatchStopJobRunSuccessfulSubmissionTypeDef],
         "Errors": List[BatchStopJobRunErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7608,33 +8755,33 @@
     {
         "Classifiers": List[ClassifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetDataflowGraphResponseTypeDef = TypedDict(
+    "GetDataflowGraphResponseTypeDef",
+    {
+        "DagNodes": List[CodeGenNodeOutputTypeDef],
+        "DagEdges": List[CodeGenEdgeOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateScriptRequestRequestTypeDef = TypedDict(
     "CreateScriptRequestRequestTypeDef",
     {
         "DagNodes": Sequence[CodeGenNodeTypeDef],
         "DagEdges": Sequence[CodeGenEdgeTypeDef],
         "Language": LanguageType,
     },
     total=False,
 )
 
-GetDataflowGraphResponseTypeDef = TypedDict(
-    "GetDataflowGraphResponseTypeDef",
-    {
-        "DagNodes": List[CodeGenNodeTypeDef],
-        "DagEdges": List[CodeGenEdgeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredGetMappingRequestRequestTypeDef = TypedDict(
     "_RequiredGetMappingRequestRequestTypeDef",
     {
         "Source": CatalogEntryTypeDef,
     },
 )
 _OptionalGetMappingRequestRequestTypeDef = TypedDict(
@@ -7642,21 +8789,19 @@
     {
         "Sinks": Sequence[CatalogEntryTypeDef],
         "Location": LocationTypeDef,
     },
     total=False,
 )
 
-
 class GetMappingRequestRequestTypeDef(
     _RequiredGetMappingRequestRequestTypeDef, _OptionalGetMappingRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPlanRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlanRequestRequestTypeDef",
     {
         "Mapping": Sequence[MappingEntryTypeDef],
         "Source": CatalogEntryTypeDef,
     },
 )
@@ -7667,20 +8812,34 @@
         "Location": LocationTypeDef,
         "Language": LanguageType,
         "AdditionalPlanOptionsMap": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetPlanRequestRequestTypeDef(
     _RequiredGetPlanRequestRequestTypeDef, _OptionalGetPlanRequestRequestTypeDef
 ):
     pass
 
+TriggerTypeDef = TypedDict(
+    "TriggerTypeDef",
+    {
+        "Name": str,
+        "WorkflowName": str,
+        "Id": str,
+        "Type": TriggerTypeType,
+        "State": TriggerStateType,
+        "Description": str,
+        "Schedule": str,
+        "Actions": List[ActionOutputTypeDef],
+        "Predicate": PredicateOutputTypeDef,
+        "EventBatchingCondition": EventBatchingConditionOutputTypeDef,
+    },
+)
 
 _RequiredCreateTriggerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTriggerRequestRequestTypeDef",
     {
         "Name": str,
         "Type": TriggerTypeType,
         "Actions": Sequence[ActionTypeDef],
@@ -7696,72 +8855,40 @@
         "StartOnCreation": bool,
         "Tags": Mapping[str, str],
         "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
-
 class CreateTriggerRequestRequestTypeDef(
     _RequiredCreateTriggerRequestRequestTypeDef, _OptionalCreateTriggerRequestRequestTypeDef
 ):
     pass
 
-
-TriggerTypeDef = TypedDict(
-    "TriggerTypeDef",
-    {
-        "Name": str,
-        "WorkflowName": str,
-        "Id": str,
-        "Type": TriggerTypeType,
-        "State": TriggerStateType,
-        "Description": str,
-        "Schedule": str,
-        "Actions": List[ActionTypeDef],
-        "Predicate": PredicateTypeDef,
-        "EventBatchingCondition": EventBatchingConditionTypeDef,
-    },
-    total=False,
-)
-
 TriggerUpdateTypeDef = TypedDict(
     "TriggerUpdateTypeDef",
     {
         "Name": str,
         "Description": str,
         "Schedule": str,
         "Actions": Sequence[ActionTypeDef],
         "Predicate": PredicateTypeDef,
         "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
-_RequiredEvaluationMetricsTypeDef = TypedDict(
-    "_RequiredEvaluationMetricsTypeDef",
+EvaluationMetricsTypeDef = TypedDict(
+    "EvaluationMetricsTypeDef",
     {
         "TransformType": Literal["FIND_MATCHES"],
-    },
-)
-_OptionalEvaluationMetricsTypeDef = TypedDict(
-    "_OptionalEvaluationMetricsTypeDef",
-    {
         "FindMatchesMetrics": FindMatchesMetricsTypeDef,
     },
-    total=False,
 )
 
-
-class EvaluationMetricsTypeDef(
-    _RequiredEvaluationMetricsTypeDef, _OptionalEvaluationMetricsTypeDef
-):
-    pass
-
-
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
 _OptionalCreateConnectionRequestRequestTypeDef = TypedDict(
@@ -7769,21 +8896,19 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectionRequestRequestTypeDef",
     {
         "Name": str,
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
@@ -7791,21 +8916,19 @@
     "_OptionalUpdateConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateConnectionRequestRequestTypeDef(
     _RequiredUpdateConnectionRequestRequestTypeDef, _OptionalUpdateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7820,34 +8943,33 @@
 )
 
 CrawlerTypeDef = TypedDict(
     "CrawlerTypeDef",
     {
         "Name": str,
         "Role": str,
-        "Targets": CrawlerTargetsTypeDef,
+        "Targets": CrawlerTargetsOutputTypeDef,
         "DatabaseName": str,
         "Description": str,
         "Classifiers": List[str],
-        "RecrawlPolicy": RecrawlPolicyTypeDef,
-        "SchemaChangePolicy": SchemaChangePolicyTypeDef,
-        "LineageConfiguration": LineageConfigurationTypeDef,
+        "RecrawlPolicy": RecrawlPolicyOutputTypeDef,
+        "SchemaChangePolicy": SchemaChangePolicyOutputTypeDef,
+        "LineageConfiguration": LineageConfigurationOutputTypeDef,
         "State": CrawlerStateType,
         "TablePrefix": str,
         "Schedule": ScheduleTypeDef,
         "CrawlElapsedTime": int,
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "LastCrawl": LastCrawlInfoTypeDef,
         "Version": int,
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
-        "LakeFormationConfiguration": LakeFormationConfigurationTypeDef,
+        "LakeFormationConfiguration": LakeFormationConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateCrawlerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCrawlerRequestRequestTypeDef",
     {
         "Name": str,
         "Role": str,
@@ -7869,21 +8991,19 @@
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateCrawlerRequestRequestTypeDef(
     _RequiredCreateCrawlerRequestRequestTypeDef, _OptionalCreateCrawlerRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateCrawlerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCrawlerRequestRequestTypeDef = TypedDict(
@@ -7902,94 +9022,42 @@
         "LakeFormationConfiguration": LakeFormationConfigurationTypeDef,
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
     },
     total=False,
 )
 
-
 class UpdateCrawlerRequestRequestTypeDef(
     _RequiredUpdateCrawlerRequestRequestTypeDef, _OptionalUpdateCrawlerRequestRequestTypeDef
 ):
     pass
 
-
 ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
     "ListDataQualityRulesetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filter": DataQualityRulesetFilterCriteriaTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-ListDataQualityRulesetsResponseTypeDef = TypedDict(
-    "ListDataQualityRulesetsResponseTypeDef",
-    {
-        "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DataQualityResultDescriptionTypeDef = TypedDict(
-    "DataQualityResultDescriptionTypeDef",
-    {
-        "ResultId": str,
-        "DataSource": DataSourceTypeDef,
-        "JobName": str,
-        "JobRunId": str,
-        "StartedOn": datetime,
-    },
-    total=False,
-)
-
 DataQualityResultFilterCriteriaTypeDef = TypedDict(
     "DataQualityResultFilterCriteriaTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "JobName": str,
         "JobRunId": str,
         "StartedAfter": Union[datetime, str],
         "StartedBefore": Union[datetime, str],
     },
     total=False,
 )
 
-DataQualityResultTypeDef = TypedDict(
-    "DataQualityResultTypeDef",
-    {
-        "ResultId": str,
-        "Score": float,
-        "DataSource": DataSourceTypeDef,
-        "RulesetName": str,
-        "EvaluationContext": str,
-        "StartedOn": datetime,
-        "CompletedOn": datetime,
-        "JobName": str,
-        "JobRunId": str,
-        "RulesetEvaluationRunId": str,
-        "RuleResults": List[DataQualityRuleResultTypeDef],
-    },
-    total=False,
-)
-
-DataQualityRuleRecommendationRunDescriptionTypeDef = TypedDict(
-    "DataQualityRuleRecommendationRunDescriptionTypeDef",
-    {
-        "RunId": str,
-        "Status": TaskStatusTypeType,
-        "StartedOn": datetime,
-        "DataSource": DataSourceTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
     "_RequiredDataQualityRuleRecommendationRunFilterTypeDef",
     {
         "DataSource": DataSourceTypeDef,
     },
 )
 _OptionalDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
@@ -7997,33 +9065,20 @@
     {
         "StartedBefore": Union[datetime, str],
         "StartedAfter": Union[datetime, str],
     },
     total=False,
 )
 
-
 class DataQualityRuleRecommendationRunFilterTypeDef(
     _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
     _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
 ):
     pass
 
-
-DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
-    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
-    {
-        "RunId": str,
-        "Status": TaskStatusTypeType,
-        "StartedOn": datetime,
-        "DataSource": DataSourceTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
     "_RequiredDataQualityRulesetEvaluationRunFilterTypeDef",
     {
         "DataSource": DataSourceTypeDef,
     },
 )
 _OptionalDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
@@ -8031,82 +9086,20 @@
     {
         "StartedBefore": Union[datetime, str],
         "StartedAfter": Union[datetime, str],
     },
     total=False,
 )
 
-
 class DataQualityRulesetEvaluationRunFilterTypeDef(
     _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
     _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
 ):
     pass
 
-
-GetDataQualityResultResponseTypeDef = TypedDict(
-    "GetDataQualityResultResponseTypeDef",
-    {
-        "ResultId": str,
-        "Score": float,
-        "DataSource": DataSourceTypeDef,
-        "RulesetName": str,
-        "EvaluationContext": str,
-        "StartedOn": datetime,
-        "CompletedOn": datetime,
-        "JobName": str,
-        "JobRunId": str,
-        "RulesetEvaluationRunId": str,
-        "RuleResults": List[DataQualityRuleResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
-    "GetDataQualityRuleRecommendationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "Status": TaskStatusTypeType,
-        "ErrorString": str,
-        "StartedOn": datetime,
-        "LastModifiedOn": datetime,
-        "CompletedOn": datetime,
-        "ExecutionTime": int,
-        "RecommendedRuleset": str,
-        "CreatedRulesetName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
-    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-        "Status": TaskStatusTypeType,
-        "ErrorString": str,
-        "StartedOn": datetime,
-        "LastModifiedOn": datetime,
-        "CompletedOn": datetime,
-        "ExecutionTime": int,
-        "RulesetNames": List[str],
-        "ResultIds": List[str],
-        "AdditionalDataSources": Dict[str, DataSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Role": str,
     },
 )
@@ -8117,22 +9110,20 @@
         "Timeout": int,
         "CreatedRulesetName": str,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
     _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
     _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Role": str,
         "RulesetNames": Sequence[str],
     },
@@ -8145,52 +9136,24 @@
         "ClientToken": str,
         "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
         "AdditionalDataSources": Mapping[str, DataSourceTypeDef],
     },
     total=False,
 )
 
-
 class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
     _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
 ):
     pass
 
-
-CreateSessionResponseTypeDef = TypedDict(
-    "CreateSessionResponseTypeDef",
-    {
-        "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListSessionsResponseTypeDef = TypedDict(
-    "ListSessionsResponseTypeDef",
-    {
-        "Ids": List[str],
-        "Sessions": List[SessionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetDataCatalogEncryptionSettingsResponseTypeDef = TypedDict(
     "GetDataCatalogEncryptionSettingsResponseTypeDef",
     {
-        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
+        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
@@ -8201,21 +9164,34 @@
     "_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(
     _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     _OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
 ):
     pass
 
+DatabaseTypeDef = TypedDict(
+    "DatabaseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "LocationUri": str,
+        "Parameters": Dict[str, str],
+        "CreateTime": datetime,
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "TargetDatabase": DatabaseIdentifierOutputTypeDef,
+        "CatalogId": str,
+        "FederatedDatabase": FederatedDatabaseOutputTypeDef,
+    },
+)
 
 _RequiredDatabaseInputTypeDef = TypedDict(
     "_RequiredDatabaseInputTypeDef",
     {
         "Name": str,
     },
 )
@@ -8228,65 +9204,176 @@
         "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
         "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
-
 class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
     pass
 
+ListDataQualityRulesetsResponseTypeDef = TypedDict(
+    "ListDataQualityRulesetsResponseTypeDef",
+    {
+        "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDatabaseTypeDef = TypedDict(
-    "_RequiredDatabaseTypeDef",
+DataQualityResultDescriptionTypeDef = TypedDict(
+    "DataQualityResultDescriptionTypeDef",
     {
-        "Name": str,
+        "ResultId": str,
+        "DataSource": DataSourceOutputTypeDef,
+        "JobName": str,
+        "JobRunId": str,
+        "StartedOn": datetime,
     },
 )
-_OptionalDatabaseTypeDef = TypedDict(
-    "_OptionalDatabaseTypeDef",
+
+DataQualityResultTypeDef = TypedDict(
+    "DataQualityResultTypeDef",
     {
-        "Description": str,
-        "LocationUri": str,
-        "Parameters": Dict[str, str],
-        "CreateTime": datetime,
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
-        "TargetDatabase": DatabaseIdentifierTypeDef,
-        "CatalogId": str,
-        "FederatedDatabase": FederatedDatabaseTypeDef,
+        "ResultId": str,
+        "Score": float,
+        "DataSource": DataSourceOutputTypeDef,
+        "RulesetName": str,
+        "EvaluationContext": str,
+        "StartedOn": datetime,
+        "CompletedOn": datetime,
+        "JobName": str,
+        "JobRunId": str,
+        "RulesetEvaluationRunId": str,
+        "RuleResults": List[DataQualityRuleResultTypeDef],
     },
-    total=False,
 )
 
+DataQualityRuleRecommendationRunDescriptionTypeDef = TypedDict(
+    "DataQualityRuleRecommendationRunDescriptionTypeDef",
+    {
+        "RunId": str,
+        "Status": TaskStatusTypeType,
+        "StartedOn": datetime,
+        "DataSource": DataSourceOutputTypeDef,
+    },
+)
 
-class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
-    pass
+DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
+    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
+    {
+        "RunId": str,
+        "Status": TaskStatusTypeType,
+        "StartedOn": datetime,
+        "DataSource": DataSourceOutputTypeDef,
+    },
+)
 
+GetDataQualityResultResponseTypeDef = TypedDict(
+    "GetDataQualityResultResponseTypeDef",
+    {
+        "ResultId": str,
+        "Score": float,
+        "DataSource": DataSourceOutputTypeDef,
+        "RulesetName": str,
+        "EvaluationContext": str,
+        "StartedOn": datetime,
+        "CompletedOn": datetime,
+        "JobName": str,
+        "JobRunId": str,
+        "RulesetEvaluationRunId": str,
+        "RuleResults": List[DataQualityRuleResultTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
+    "GetDataQualityRuleRecommendationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "DataSource": DataSourceOutputTypeDef,
+        "Role": str,
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "Status": TaskStatusTypeType,
+        "ErrorString": str,
+        "StartedOn": datetime,
+        "LastModifiedOn": datetime,
+        "CompletedOn": datetime,
+        "ExecutionTime": int,
+        "RecommendedRuleset": str,
+        "CreatedRulesetName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
+    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "DataSource": DataSourceOutputTypeDef,
+        "Role": str,
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef,
+        "Status": TaskStatusTypeType,
+        "ErrorString": str,
+        "StartedOn": datetime,
+        "LastModifiedOn": datetime,
+        "CompletedOn": datetime,
+        "ExecutionTime": int,
+        "RulesetNames": List[str],
+        "ResultIds": List[str],
+        "AdditionalDataSources": Dict[str, DataSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DropNullFieldsOutputTypeDef = TypedDict(
+    "DropNullFieldsOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "NullCheckBoxList": NullCheckBoxListOutputTypeDef,
+        "NullTextList": List[NullValueFieldOutputTypeDef],
+    },
+)
 
 _RequiredDropNullFieldsTypeDef = TypedDict(
     "_RequiredDropNullFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
     },
 )
 _OptionalDropNullFieldsTypeDef = TypedDict(
     "_OptionalDropNullFieldsTypeDef",
     {
         "NullCheckBoxList": NullCheckBoxListTypeDef,
-        "NullTextList": List[NullValueFieldTypeDef],
+        "NullTextList": Sequence[NullValueFieldTypeDef],
     },
     total=False,
 )
 
-
 class DropNullFieldsTypeDef(_RequiredDropNullFieldsTypeDef, _OptionalDropNullFieldsTypeDef):
     pass
 
+ColumnStatisticsDataOutputTypeDef = TypedDict(
+    "ColumnStatisticsDataOutputTypeDef",
+    {
+        "Type": ColumnStatisticsTypeType,
+        "BooleanColumnStatisticsData": BooleanColumnStatisticsDataOutputTypeDef,
+        "DateColumnStatisticsData": DateColumnStatisticsDataOutputTypeDef,
+        "DecimalColumnStatisticsData": DecimalColumnStatisticsDataOutputTypeDef,
+        "DoubleColumnStatisticsData": DoubleColumnStatisticsDataOutputTypeDef,
+        "LongColumnStatisticsData": LongColumnStatisticsDataOutputTypeDef,
+        "StringColumnStatisticsData": StringColumnStatisticsDataOutputTypeDef,
+        "BinaryColumnStatisticsData": BinaryColumnStatisticsDataOutputTypeDef,
+    },
+)
 
 _RequiredColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredColumnStatisticsDataTypeDef",
     {
         "Type": ColumnStatisticsTypeType,
     },
 )
@@ -8300,21 +9387,19 @@
         "LongColumnStatisticsData": LongColumnStatisticsDataTypeDef,
         "StringColumnStatisticsData": StringColumnStatisticsDataTypeDef,
         "BinaryColumnStatisticsData": BinaryColumnStatisticsDataTypeDef,
     },
     total=False,
 )
 
-
 class ColumnStatisticsDataTypeDef(
     _RequiredColumnStatisticsDataTypeDef, _OptionalColumnStatisticsDataTypeDef
 ):
     pass
 
-
 StorageDescriptorTypeDef = TypedDict(
     "StorageDescriptorTypeDef",
     {
         "Columns": Sequence[ColumnTypeDef],
         "Location": str,
         "AdditionalLocations": Sequence[str],
         "InputFormat": str,
@@ -8328,47 +9413,56 @@
         "SkewedInfo": SkewedInfoTypeDef,
         "StoredAsSubDirectories": bool,
         "SchemaReference": SchemaReferenceTypeDef,
     },
     total=False,
 )
 
-CreateSecurityConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateSecurityConfigurationRequestRequestTypeDef",
+SecurityConfigurationTypeDef = TypedDict(
+    "SecurityConfigurationTypeDef",
     {
         "Name": str,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "CreatedTimeStamp": datetime,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
     },
 )
 
-SecurityConfigurationTypeDef = TypedDict(
-    "SecurityConfigurationTypeDef",
+CreateSecurityConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateSecurityConfigurationRequestRequestTypeDef",
     {
         "Name": str,
-        "CreatedTimeStamp": datetime,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
-    total=False,
 )
 
 DeleteSchemaVersionsResponseTypeDef = TypedDict(
     "DeleteSchemaVersionsResponseTypeDef",
     {
         "SchemaVersionErrors": List[SchemaVersionErrorItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "LogicalOperator": FilterLogicalOperatorType,
+        "Filters": List[FilterExpressionOutputTypeDef],
+    },
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "LogicalOperator": FilterLogicalOperatorType,
-        "Filters": List[FilterExpressionTypeDef],
+        "Filters": Sequence[FilterExpressionTypeDef],
     },
 )
 
 _RequiredUpdateMLTransformRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMLTransformRequestRequestTypeDef",
     {
         "TransformId": str,
@@ -8387,42 +9481,246 @@
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
     },
     total=False,
 )
 
-
 class UpdateMLTransformRequestRequestTypeDef(
     _RequiredUpdateMLTransformRequestRequestTypeDef, _OptionalUpdateMLTransformRequestRequestTypeDef
 ):
     pass
 
+AthenaConnectorSourceOutputTypeDef = TypedDict(
+    "AthenaConnectorSourceOutputTypeDef",
+    {
+        "Name": str,
+        "ConnectionName": str,
+        "ConnectorName": str,
+        "ConnectionType": str,
+        "ConnectionTable": str,
+        "SchemaName": str,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
 
-GetMLTransformsRequestRequestTypeDef = TypedDict(
-    "GetMLTransformsRequestRequestTypeDef",
+CatalogDeltaSourceOutputTypeDef = TypedDict(
+    "CatalogDeltaSourceOutputTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filter": TransformFilterCriteriaTypeDef,
-        "Sort": TransformSortCriteriaTypeDef,
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
     },
-    total=False,
 )
 
-ListMLTransformsRequestRequestTypeDef = TypedDict(
-    "ListMLTransformsRequestRequestTypeDef",
+CatalogHudiSourceOutputTypeDef = TypedDict(
+    "CatalogHudiSourceOutputTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filter": TransformFilterCriteriaTypeDef,
-        "Sort": TransformSortCriteriaTypeDef,
-        "Tags": Mapping[str, str],
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+CustomCodeOutputTypeDef = TypedDict(
+    "CustomCodeOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Code": str,
+        "ClassName": str,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+DynamicTransformOutputTypeDef = TypedDict(
+    "DynamicTransformOutputTypeDef",
+    {
+        "Name": str,
+        "TransformName": str,
+        "Inputs": List[str],
+        "Parameters": List[TransformConfigParameterOutputTypeDef],
+        "FunctionName": str,
+        "Path": str,
+        "Version": str,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+JDBCConnectorSourceOutputTypeDef = TypedDict(
+    "JDBCConnectorSourceOutputTypeDef",
+    {
+        "Name": str,
+        "ConnectionName": str,
+        "ConnectorName": str,
+        "ConnectionType": str,
+        "AdditionalOptions": JDBCConnectorOptionsOutputTypeDef,
+        "ConnectionTable": str,
+        "Query": str,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+JDBCConnectorTargetOutputTypeDef = TypedDict(
+    "JDBCConnectorTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "ConnectionName": str,
+        "ConnectionTable": str,
+        "ConnectorName": str,
+        "ConnectionType": str,
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3CatalogDeltaSourceOutputTypeDef = TypedDict(
+    "S3CatalogDeltaSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3CatalogHudiSourceOutputTypeDef = TypedDict(
+    "S3CatalogHudiSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3CsvSourceOutputTypeDef = TypedDict(
+    "S3CsvSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+        "CompressionType": CompressionTypeType,
+        "Exclusions": List[str],
+        "GroupSize": str,
+        "GroupFiles": str,
+        "Recurse": bool,
+        "MaxBand": int,
+        "MaxFilesInBand": int,
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsOutputTypeDef,
+        "Separator": SeparatorType,
+        "Escaper": str,
+        "QuoteChar": QuoteCharType,
+        "Multiline": bool,
+        "WithHeader": bool,
+        "WriteHeader": bool,
+        "SkipFirst": bool,
+        "OptimizePerformance": bool,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3DeltaSourceOutputTypeDef = TypedDict(
+    "S3DeltaSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+        "AdditionalDeltaOptions": Dict[str, str],
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsOutputTypeDef,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3HudiSourceOutputTypeDef = TypedDict(
+    "S3HudiSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+        "AdditionalHudiOptions": Dict[str, str],
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsOutputTypeDef,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3JsonSourceOutputTypeDef = TypedDict(
+    "S3JsonSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+        "CompressionType": CompressionTypeType,
+        "Exclusions": List[str],
+        "GroupSize": str,
+        "GroupFiles": str,
+        "Recurse": bool,
+        "MaxBand": int,
+        "MaxFilesInBand": int,
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsOutputTypeDef,
+        "JsonPath": str,
+        "Multiline": bool,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3ParquetSourceOutputTypeDef = TypedDict(
+    "S3ParquetSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+        "CompressionType": ParquetCompressionTypeType,
+        "Exclusions": List[str],
+        "GroupSize": str,
+        "GroupFiles": str,
+        "Recurse": bool,
+        "MaxBand": int,
+        "MaxFilesInBand": int,
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsOutputTypeDef,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+SparkConnectorSourceOutputTypeDef = TypedDict(
+    "SparkConnectorSourceOutputTypeDef",
+    {
+        "Name": str,
+        "ConnectionName": str,
+        "ConnectorName": str,
+        "ConnectionType": str,
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+SparkConnectorTargetOutputTypeDef = TypedDict(
+    "SparkConnectorTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "ConnectionName": str,
+        "ConnectorName": str,
+        "ConnectionType": str,
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+SparkSQLOutputTypeDef = TypedDict(
+    "SparkSQLOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "SqlQuery": str,
+        "SqlAliases": List[SqlAliasOutputTypeDef],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredAthenaConnectorSourceTypeDef = TypedDict(
     "_RequiredAthenaConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
@@ -8431,121 +9729,111 @@
         "SchemaName": str,
     },
 )
 _OptionalAthenaConnectorSourceTypeDef = TypedDict(
     "_OptionalAthenaConnectorSourceTypeDef",
     {
         "ConnectionTable": str,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class AthenaConnectorSourceTypeDef(
     _RequiredAthenaConnectorSourceTypeDef, _OptionalAthenaConnectorSourceTypeDef
 ):
     pass
 
-
 _RequiredCatalogDeltaSourceTypeDef = TypedDict(
     "_RequiredCatalogDeltaSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 _OptionalCatalogDeltaSourceTypeDef = TypedDict(
     "_OptionalCatalogDeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalDeltaOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class CatalogDeltaSourceTypeDef(
     _RequiredCatalogDeltaSourceTypeDef, _OptionalCatalogDeltaSourceTypeDef
 ):
     pass
 
-
 _RequiredCatalogHudiSourceTypeDef = TypedDict(
     "_RequiredCatalogHudiSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 _OptionalCatalogHudiSourceTypeDef = TypedDict(
     "_OptionalCatalogHudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalHudiOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class CatalogHudiSourceTypeDef(
     _RequiredCatalogHudiSourceTypeDef, _OptionalCatalogHudiSourceTypeDef
 ):
     pass
 
-
 _RequiredCustomCodeTypeDef = TypedDict(
     "_RequiredCustomCodeTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Code": str,
         "ClassName": str,
     },
 )
 _OptionalCustomCodeTypeDef = TypedDict(
     "_OptionalCustomCodeTypeDef",
     {
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class CustomCodeTypeDef(_RequiredCustomCodeTypeDef, _OptionalCustomCodeTypeDef):
     pass
 
-
 _RequiredDynamicTransformTypeDef = TypedDict(
     "_RequiredDynamicTransformTypeDef",
     {
         "Name": str,
         "TransformName": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "FunctionName": str,
         "Path": str,
     },
 )
 _OptionalDynamicTransformTypeDef = TypedDict(
     "_OptionalDynamicTransformTypeDef",
     {
-        "Parameters": List[TransformConfigParameterTypeDef],
+        "Parameters": Sequence[TransformConfigParameterTypeDef],
         "Version": str,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class DynamicTransformTypeDef(_RequiredDynamicTransformTypeDef, _OptionalDynamicTransformTypeDef):
     pass
 
-
 _RequiredJDBCConnectorSourceTypeDef = TypedDict(
     "_RequiredJDBCConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -8553,312 +9841,288 @@
 )
 _OptionalJDBCConnectorSourceTypeDef = TypedDict(
     "_OptionalJDBCConnectorSourceTypeDef",
     {
         "AdditionalOptions": JDBCConnectorOptionsTypeDef,
         "ConnectionTable": str,
         "Query": str,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class JDBCConnectorSourceTypeDef(
     _RequiredJDBCConnectorSourceTypeDef, _OptionalJDBCConnectorSourceTypeDef
 ):
     pass
 
-
 _RequiredJDBCConnectorTargetTypeDef = TypedDict(
     "_RequiredJDBCConnectorTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "ConnectionName": str,
         "ConnectionTable": str,
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalJDBCConnectorTargetTypeDef = TypedDict(
     "_OptionalJDBCConnectorTargetTypeDef",
     {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class JDBCConnectorTargetTypeDef(
     _RequiredJDBCConnectorTargetTypeDef, _OptionalJDBCConnectorTargetTypeDef
 ):
     pass
 
-
 _RequiredS3CatalogDeltaSourceTypeDef = TypedDict(
     "_RequiredS3CatalogDeltaSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 _OptionalS3CatalogDeltaSourceTypeDef = TypedDict(
     "_OptionalS3CatalogDeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalDeltaOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3CatalogDeltaSourceTypeDef(
     _RequiredS3CatalogDeltaSourceTypeDef, _OptionalS3CatalogDeltaSourceTypeDef
 ):
     pass
 
-
 _RequiredS3CatalogHudiSourceTypeDef = TypedDict(
     "_RequiredS3CatalogHudiSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 _OptionalS3CatalogHudiSourceTypeDef = TypedDict(
     "_OptionalS3CatalogHudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalHudiOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3CatalogHudiSourceTypeDef(
     _RequiredS3CatalogHudiSourceTypeDef, _OptionalS3CatalogHudiSourceTypeDef
 ):
     pass
 
-
 _RequiredS3CsvSourceTypeDef = TypedDict(
     "_RequiredS3CsvSourceTypeDef",
     {
         "Name": str,
-        "Paths": List[str],
+        "Paths": Sequence[str],
         "Separator": SeparatorType,
         "QuoteChar": QuoteCharType,
     },
 )
 _OptionalS3CsvSourceTypeDef = TypedDict(
     "_OptionalS3CsvSourceTypeDef",
     {
         "CompressionType": CompressionTypeType,
-        "Exclusions": List[str],
+        "Exclusions": Sequence[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "Escaper": str,
         "Multiline": bool,
         "WithHeader": bool,
         "WriteHeader": bool,
         "SkipFirst": bool,
         "OptimizePerformance": bool,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
     pass
 
-
 _RequiredS3DeltaSourceTypeDef = TypedDict(
     "_RequiredS3DeltaSourceTypeDef",
     {
         "Name": str,
-        "Paths": List[str],
+        "Paths": Sequence[str],
     },
 )
 _OptionalS3DeltaSourceTypeDef = TypedDict(
     "_OptionalS3DeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Dict[str, str],
+        "AdditionalDeltaOptions": Mapping[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3DeltaSourceTypeDef(_RequiredS3DeltaSourceTypeDef, _OptionalS3DeltaSourceTypeDef):
     pass
 
-
 _RequiredS3HudiSourceTypeDef = TypedDict(
     "_RequiredS3HudiSourceTypeDef",
     {
         "Name": str,
-        "Paths": List[str],
+        "Paths": Sequence[str],
     },
 )
 _OptionalS3HudiSourceTypeDef = TypedDict(
     "_OptionalS3HudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Dict[str, str],
+        "AdditionalHudiOptions": Mapping[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3HudiSourceTypeDef(_RequiredS3HudiSourceTypeDef, _OptionalS3HudiSourceTypeDef):
     pass
 
-
 _RequiredS3JsonSourceTypeDef = TypedDict(
     "_RequiredS3JsonSourceTypeDef",
     {
         "Name": str,
-        "Paths": List[str],
+        "Paths": Sequence[str],
     },
 )
 _OptionalS3JsonSourceTypeDef = TypedDict(
     "_OptionalS3JsonSourceTypeDef",
     {
         "CompressionType": CompressionTypeType,
-        "Exclusions": List[str],
+        "Exclusions": Sequence[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "JsonPath": str,
         "Multiline": bool,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3JsonSourceTypeDef(_RequiredS3JsonSourceTypeDef, _OptionalS3JsonSourceTypeDef):
     pass
 
-
 _RequiredS3ParquetSourceTypeDef = TypedDict(
     "_RequiredS3ParquetSourceTypeDef",
     {
         "Name": str,
-        "Paths": List[str],
+        "Paths": Sequence[str],
     },
 )
 _OptionalS3ParquetSourceTypeDef = TypedDict(
     "_OptionalS3ParquetSourceTypeDef",
     {
         "CompressionType": ParquetCompressionTypeType,
-        "Exclusions": List[str],
+        "Exclusions": Sequence[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3ParquetSourceTypeDef(_RequiredS3ParquetSourceTypeDef, _OptionalS3ParquetSourceTypeDef):
     pass
 
-
 _RequiredSparkConnectorSourceTypeDef = TypedDict(
     "_RequiredSparkConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalSparkConnectorSourceTypeDef = TypedDict(
     "_OptionalSparkConnectorSourceTypeDef",
     {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class SparkConnectorSourceTypeDef(
     _RequiredSparkConnectorSourceTypeDef, _OptionalSparkConnectorSourceTypeDef
 ):
     pass
 
-
 _RequiredSparkConnectorTargetTypeDef = TypedDict(
     "_RequiredSparkConnectorTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalSparkConnectorTargetTypeDef = TypedDict(
     "_OptionalSparkConnectorTargetTypeDef",
     {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class SparkConnectorTargetTypeDef(
     _RequiredSparkConnectorTargetTypeDef, _OptionalSparkConnectorTargetTypeDef
 ):
     pass
 
-
 _RequiredSparkSQLTypeDef = TypedDict(
     "_RequiredSparkSQLTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "SqlQuery": str,
-        "SqlAliases": List[SqlAliasTypeDef],
+        "SqlAliases": Sequence[SqlAliasTypeDef],
     },
 )
 _OptionalSparkSQLTypeDef = TypedDict(
     "_OptionalSparkSQLTypeDef",
     {
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class SparkSQLTypeDef(_RequiredSparkSQLTypeDef, _OptionalSparkSQLTypeDef):
     pass
 
-
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "JobRun": JobRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8873,15 +10137,14 @@
 )
 
 JobNodeDetailsTypeDef = TypedDict(
     "JobNodeDetailsTypeDef",
     {
         "JobRuns": List[JobRunTypeDef],
     },
-    total=False,
 )
 
 GetMLTaskRunResponseTypeDef = TypedDict(
     "GetMLTaskRunResponseTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
@@ -8907,15 +10170,14 @@
         "Properties": TaskRunPropertiesTypeDef,
         "ErrorString": str,
         "StartedOn": datetime,
         "LastModifiedOn": datetime,
         "CompletedOn": datetime,
         "ExecutionTime": int,
     },
-    total=False,
 )
 
 _RequiredCreateMLTransformRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMLTransformRequestRequestTypeDef",
     {
         "Name": str,
         "InputRecordTables": Sequence[GlueTableTypeDef],
@@ -8935,31 +10197,46 @@
         "MaxRetries": int,
         "Tags": Mapping[str, str],
         "TransformEncryption": TransformEncryptionTypeDef,
     },
     total=False,
 )
 
-
 class CreateMLTransformRequestRequestTypeDef(
     _RequiredCreateMLTransformRequestRequestTypeDef, _OptionalCreateMLTransformRequestRequestTypeDef
 ):
     pass
 
-
 QuerySchemaVersionMetadataResponseTypeDef = TypedDict(
     "QuerySchemaVersionMetadataResponseTypeDef",
     {
         "MetadataInfoMap": Dict[str, MetadataInfoTypeDef],
         "SchemaVersionId": str,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetUserDefinedFunctionResponseTypeDef = TypedDict(
+    "GetUserDefinedFunctionResponseTypeDef",
+    {
+        "UserDefinedFunction": UserDefinedFunctionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUserDefinedFunctionsResponseTypeDef = TypedDict(
+    "GetUserDefinedFunctionsResponseTypeDef",
+    {
+        "UserDefinedFunctions": List[UserDefinedFunctionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionInput": UserDefinedFunctionInputTypeDef,
     },
 )
@@ -8967,22 +10244,20 @@
     "_OptionalCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class CreateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredCreateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalCreateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionName": str,
         "FunctionInput": UserDefinedFunctionInputTypeDef,
     },
@@ -8991,34 +10266,84 @@
     "_OptionalUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalUpdateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+GetMLTransformsRequestRequestTypeDef = TypedDict(
+    "GetMLTransformsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "Filter": TransformFilterCriteriaTypeDef,
+        "Sort": TransformSortCriteriaTypeDef,
+    },
+    total=False,
+)
 
-GetUserDefinedFunctionResponseTypeDef = TypedDict(
-    "GetUserDefinedFunctionResponseTypeDef",
+ListMLTransformsRequestRequestTypeDef = TypedDict(
+    "ListMLTransformsRequestRequestTypeDef",
     {
-        "UserDefinedFunction": UserDefinedFunctionTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "Filter": TransformFilterCriteriaTypeDef,
+        "Sort": TransformSortCriteriaTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+StorageDescriptorOutputTypeDef = TypedDict(
+    "StorageDescriptorOutputTypeDef",
+    {
+        "Columns": List[ColumnOutputTypeDef],
+        "Location": str,
+        "AdditionalLocations": List[str],
+        "InputFormat": str,
+        "OutputFormat": str,
+        "Compressed": bool,
+        "NumberOfBuckets": int,
+        "SerdeInfo": SerDeInfoOutputTypeDef,
+        "BucketColumns": List[str],
+        "SortColumns": List[OrderOutputTypeDef],
+        "Parameters": Dict[str, str],
+        "SkewedInfo": SkewedInfoOutputTypeDef,
+        "StoredAsSubDirectories": bool,
+        "SchemaReference": SchemaReferenceOutputTypeDef,
+    },
+)
+
+CreateSessionResponseTypeDef = TypedDict(
+    "CreateSessionResponseTypeDef",
+    {
+        "Session": SessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetUserDefinedFunctionsResponseTypeDef = TypedDict(
-    "GetUserDefinedFunctionsResponseTypeDef",
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
     {
-        "UserDefinedFunctions": List[UserDefinedFunctionTypeDef],
+        "Session": SessionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSessionsResponseTypeDef = TypedDict(
+    "ListSessionsResponseTypeDef",
+    {
+        "Ids": List[str],
+        "Sessions": List[SessionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StatementTypeDef = TypedDict(
     "StatementTypeDef",
@@ -9027,15 +10352,14 @@
         "Code": str,
         "State": StatementStateType,
         "Output": StatementOutputTypeDef,
         "Progress": float,
         "StartedOn": int,
         "CompletedOn": int,
     },
-    total=False,
 )
 
 GetPartitionIndexesResponseTypeDef = TypedDict(
     "GetPartitionIndexesResponseTypeDef",
     {
         "PartitionIndexDescriptorList": List[PartitionIndexDescriptorTypeDef],
         "NextToken": str,
@@ -9070,15 +10394,14 @@
 )
 
 TriggerNodeDetailsTypeDef = TypedDict(
     "TriggerNodeDetailsTypeDef",
     {
         "Trigger": TriggerTypeDef,
     },
-    total=False,
 )
 
 UpdateTriggerResponseTypeDef = TypedDict(
     "UpdateTriggerResponseTypeDef",
     {
         "Trigger": TriggerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -9098,55 +10421,54 @@
     {
         "TransformId": str,
         "Name": str,
         "Description": str,
         "Status": TransformStatusTypeType,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
-        "InputRecordTables": List[GlueTableTypeDef],
-        "Parameters": TransformParametersTypeDef,
+        "InputRecordTables": List[GlueTableOutputTypeDef],
+        "Parameters": TransformParametersOutputTypeDef,
         "EvaluationMetrics": EvaluationMetricsTypeDef,
         "LabelCount": int,
-        "Schema": List[SchemaColumnTypeDef],
+        "Schema": List[SchemaColumnOutputTypeDef],
         "Role": str,
         "GlueVersion": str,
         "MaxCapacity": float,
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
-        "TransformEncryption": TransformEncryptionTypeDef,
+        "TransformEncryption": TransformEncryptionOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MLTransformTypeDef = TypedDict(
     "MLTransformTypeDef",
     {
         "TransformId": str,
         "Name": str,
         "Description": str,
         "Status": TransformStatusTypeType,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
-        "InputRecordTables": List[GlueTableTypeDef],
-        "Parameters": TransformParametersTypeDef,
+        "InputRecordTables": List[GlueTableOutputTypeDef],
+        "Parameters": TransformParametersOutputTypeDef,
         "EvaluationMetrics": EvaluationMetricsTypeDef,
         "LabelCount": int,
-        "Schema": List[SchemaColumnTypeDef],
+        "Schema": List[SchemaColumnOutputTypeDef],
         "Role": str,
         "GlueVersion": str,
         "MaxCapacity": float,
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
-        "TransformEncryption": TransformEncryptionTypeDef,
+        "TransformEncryption": TransformEncryptionOutputTypeDef,
     },
-    total=False,
 )
 
 BatchGetCrawlersResponseTypeDef = TypedDict(
     "BatchGetCrawlersResponseTypeDef",
     {
         "Crawlers": List[CrawlerTypeDef],
         "CrawlersNotFound": List[str],
@@ -9167,78 +10489,59 @@
     {
         "Crawlers": List[CrawlerTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDataQualityResultsResponseTypeDef = TypedDict(
-    "ListDataQualityResultsResponseTypeDef",
-    {
-        "Results": List[DataQualityResultDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListDataQualityResultsRequestRequestTypeDef = TypedDict(
     "ListDataQualityResultsRequestRequestTypeDef",
     {
         "Filter": DataQualityResultFilterCriteriaTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-BatchGetDataQualityResultResponseTypeDef = TypedDict(
-    "BatchGetDataQualityResultResponseTypeDef",
-    {
-        "Results": List[DataQualityResultTypeDef],
-        "ResultsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityRuleRecommendationRunsResponseTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
     {
-        "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
+        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxResults": int,
     },
+    total=False,
 )
 
-ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
     {
-        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
+        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+GetDatabaseResponseTypeDef = TypedDict(
+    "GetDatabaseResponseTypeDef",
     {
-        "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
-        "NextToken": str,
+        "Database": DatabaseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
+GetDatabasesResponseTypeDef = TypedDict(
+    "GetDatabasesResponseTypeDef",
     {
-        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
+        "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
-        "MaxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseInput": DatabaseInputTypeDef,
     },
@@ -9248,21 +10551,19 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatabaseRequestRequestTypeDef",
     {
         "Name": str,
         "DatabaseInput": DatabaseInputTypeDef,
     },
 )
@@ -9270,44 +10571,71 @@
     "_OptionalUpdateDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateDatabaseRequestRequestTypeDef(
     _RequiredUpdateDatabaseRequestRequestTypeDef, _OptionalUpdateDatabaseRequestRequestTypeDef
 ):
     pass
 
+ListDataQualityResultsResponseTypeDef = TypedDict(
+    "ListDataQualityResultsResponseTypeDef",
+    {
+        "Results": List[DataQualityResultDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-GetDatabaseResponseTypeDef = TypedDict(
-    "GetDatabaseResponseTypeDef",
+BatchGetDataQualityResultResponseTypeDef = TypedDict(
+    "BatchGetDataQualityResultResponseTypeDef",
     {
-        "Database": DatabaseTypeDef,
+        "Results": List[DataQualityResultTypeDef],
+        "ResultsNotFound": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDatabasesResponseTypeDef = TypedDict(
-    "GetDatabasesResponseTypeDef",
+ListDataQualityRuleRecommendationRunsResponseTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
     {
-        "DatabaseList": List[DatabaseTypeDef],
+        "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+    {
+        "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ColumnStatisticsOutputTypeDef = TypedDict(
+    "ColumnStatisticsOutputTypeDef",
+    {
+        "ColumnName": str,
+        "ColumnType": str,
+        "AnalyzedTime": datetime,
+        "StatisticsData": ColumnStatisticsDataOutputTypeDef,
+    },
+)
+
 ColumnStatisticsTypeDef = TypedDict(
     "ColumnStatisticsTypeDef",
     {
         "ColumnName": str,
         "ColumnType": str,
-        "AnalyzedTime": datetime,
+        "AnalyzedTime": Union[datetime, str],
         "StatisticsData": ColumnStatisticsDataTypeDef,
     },
 )
 
 PartitionInputTypeDef = TypedDict(
     "PartitionInputTypeDef",
     {
@@ -9316,30 +10644,14 @@
         "StorageDescriptor": StorageDescriptorTypeDef,
         "Parameters": Mapping[str, str],
         "LastAnalyzedTime": Union[datetime, str],
     },
     total=False,
 )
 
-PartitionTypeDef = TypedDict(
-    "PartitionTypeDef",
-    {
-        "Values": List[str],
-        "DatabaseName": str,
-        "TableName": str,
-        "CreationTime": datetime,
-        "LastAccessTime": datetime,
-        "StorageDescriptor": StorageDescriptorTypeDef,
-        "Parameters": Dict[str, str],
-        "LastAnalyzedTime": datetime,
-        "CatalogId": str,
-    },
-    total=False,
-)
-
 _RequiredTableInputTypeDef = TypedDict(
     "_RequiredTableInputTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalTableInputTypeDef = TypedDict(
@@ -9357,57 +10669,17 @@
         "TableType": str,
         "Parameters": Mapping[str, str],
         "TargetTable": TableIdentifierTypeDef,
     },
     total=False,
 )
 
-
 class TableInputTypeDef(_RequiredTableInputTypeDef, _OptionalTableInputTypeDef):
     pass
 
-
-_RequiredTableTypeDef = TypedDict(
-    "_RequiredTableTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalTableTypeDef = TypedDict(
-    "_OptionalTableTypeDef",
-    {
-        "DatabaseName": str,
-        "Description": str,
-        "Owner": str,
-        "CreateTime": datetime,
-        "UpdateTime": datetime,
-        "LastAccessTime": datetime,
-        "LastAnalyzedTime": datetime,
-        "Retention": int,
-        "StorageDescriptor": StorageDescriptorTypeDef,
-        "PartitionKeys": List[ColumnTypeDef],
-        "ViewOriginalText": str,
-        "ViewExpandedText": str,
-        "TableType": str,
-        "Parameters": Dict[str, str],
-        "CreatedBy": str,
-        "IsRegisteredWithLakeFormation": bool,
-        "TargetTable": TableIdentifierTypeDef,
-        "CatalogId": str,
-        "VersionId": str,
-        "FederatedTable": FederatedTableTypeDef,
-    },
-    total=False,
-)
-
-
-class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
-    pass
-
-
 GetSecurityConfigurationResponseTypeDef = TypedDict(
     "GetSecurityConfigurationResponseTypeDef",
     {
         "SecurityConfiguration": SecurityConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9417,14 +10689,86 @@
     {
         "SecurityConfigurations": List[SecurityConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CodeGenConfigurationNodeOutputTypeDef = TypedDict(
+    "CodeGenConfigurationNodeOutputTypeDef",
+    {
+        "AthenaConnectorSource": AthenaConnectorSourceOutputTypeDef,
+        "JDBCConnectorSource": JDBCConnectorSourceOutputTypeDef,
+        "SparkConnectorSource": SparkConnectorSourceOutputTypeDef,
+        "CatalogSource": CatalogSourceOutputTypeDef,
+        "RedshiftSource": RedshiftSourceOutputTypeDef,
+        "S3CatalogSource": S3CatalogSourceOutputTypeDef,
+        "S3CsvSource": S3CsvSourceOutputTypeDef,
+        "S3JsonSource": S3JsonSourceOutputTypeDef,
+        "S3ParquetSource": S3ParquetSourceOutputTypeDef,
+        "RelationalCatalogSource": RelationalCatalogSourceOutputTypeDef,
+        "DynamoDBCatalogSource": DynamoDBCatalogSourceOutputTypeDef,
+        "JDBCConnectorTarget": JDBCConnectorTargetOutputTypeDef,
+        "SparkConnectorTarget": SparkConnectorTargetOutputTypeDef,
+        "CatalogTarget": BasicCatalogTargetOutputTypeDef,
+        "RedshiftTarget": RedshiftTargetOutputTypeDef,
+        "S3CatalogTarget": S3CatalogTargetOutputTypeDef,
+        "S3GlueParquetTarget": S3GlueParquetTargetOutputTypeDef,
+        "S3DirectTarget": S3DirectTargetOutputTypeDef,
+        "ApplyMapping": ApplyMappingOutputTypeDef,
+        "SelectFields": SelectFieldsOutputTypeDef,
+        "DropFields": DropFieldsOutputTypeDef,
+        "RenameField": RenameFieldOutputTypeDef,
+        "Spigot": SpigotOutputTypeDef,
+        "Join": JoinOutputTypeDef,
+        "SplitFields": SplitFieldsOutputTypeDef,
+        "SelectFromCollection": SelectFromCollectionOutputTypeDef,
+        "FillMissingValues": FillMissingValuesOutputTypeDef,
+        "Filter": FilterOutputTypeDef,
+        "CustomCode": CustomCodeOutputTypeDef,
+        "SparkSQL": SparkSQLOutputTypeDef,
+        "DirectKinesisSource": DirectKinesisSourceOutputTypeDef,
+        "DirectKafkaSource": DirectKafkaSourceOutputTypeDef,
+        "CatalogKinesisSource": CatalogKinesisSourceOutputTypeDef,
+        "CatalogKafkaSource": CatalogKafkaSourceOutputTypeDef,
+        "DropNullFields": DropNullFieldsOutputTypeDef,
+        "Merge": MergeOutputTypeDef,
+        "Union": UnionOutputTypeDef,
+        "PIIDetection": PIIDetectionOutputTypeDef,
+        "Aggregate": AggregateOutputTypeDef,
+        "DropDuplicates": DropDuplicatesOutputTypeDef,
+        "GovernedCatalogTarget": GovernedCatalogTargetOutputTypeDef,
+        "GovernedCatalogSource": GovernedCatalogSourceOutputTypeDef,
+        "MicrosoftSQLServerCatalogSource": MicrosoftSQLServerCatalogSourceOutputTypeDef,
+        "MySQLCatalogSource": MySQLCatalogSourceOutputTypeDef,
+        "OracleSQLCatalogSource": OracleSQLCatalogSourceOutputTypeDef,
+        "PostgreSQLCatalogSource": PostgreSQLCatalogSourceOutputTypeDef,
+        "MicrosoftSQLServerCatalogTarget": MicrosoftSQLServerCatalogTargetOutputTypeDef,
+        "MySQLCatalogTarget": MySQLCatalogTargetOutputTypeDef,
+        "OracleSQLCatalogTarget": OracleSQLCatalogTargetOutputTypeDef,
+        "PostgreSQLCatalogTarget": PostgreSQLCatalogTargetOutputTypeDef,
+        "DynamicTransform": DynamicTransformOutputTypeDef,
+        "EvaluateDataQuality": EvaluateDataQualityOutputTypeDef,
+        "S3CatalogHudiSource": S3CatalogHudiSourceOutputTypeDef,
+        "CatalogHudiSource": CatalogHudiSourceOutputTypeDef,
+        "S3HudiSource": S3HudiSourceOutputTypeDef,
+        "S3HudiCatalogTarget": S3HudiCatalogTargetOutputTypeDef,
+        "S3HudiDirectTarget": S3HudiDirectTargetOutputTypeDef,
+        "DirectJDBCSource": DirectJDBCSourceOutputTypeDef,
+        "S3CatalogDeltaSource": S3CatalogDeltaSourceOutputTypeDef,
+        "CatalogDeltaSource": CatalogDeltaSourceOutputTypeDef,
+        "S3DeltaSource": S3DeltaSourceOutputTypeDef,
+        "S3DeltaCatalogTarget": S3DeltaCatalogTargetOutputTypeDef,
+        "S3DeltaDirectTarget": S3DeltaDirectTargetOutputTypeDef,
+        "AmazonRedshiftSource": AmazonRedshiftSourceOutputTypeDef,
+        "AmazonRedshiftTarget": AmazonRedshiftTargetOutputTypeDef,
+        "EvaluateDataQualityMultiFrame": EvaluateDataQualityMultiFrameOutputTypeDef,
+    },
+)
+
 CodeGenConfigurationNodeTypeDef = TypedDict(
     "CodeGenConfigurationNodeTypeDef",
     {
         "AthenaConnectorSource": AthenaConnectorSourceTypeDef,
         "JDBCConnectorSource": JDBCConnectorSourceTypeDef,
         "SparkConnectorSource": SparkConnectorSourceTypeDef,
         "CatalogSource": CatalogSourceTypeDef,
@@ -9499,14 +10843,56 @@
     {
         "TaskRuns": List[TaskRunTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PartitionTypeDef = TypedDict(
+    "PartitionTypeDef",
+    {
+        "Values": List[str],
+        "DatabaseName": str,
+        "TableName": str,
+        "CreationTime": datetime,
+        "LastAccessTime": datetime,
+        "StorageDescriptor": StorageDescriptorOutputTypeDef,
+        "Parameters": Dict[str, str],
+        "LastAnalyzedTime": datetime,
+        "CatalogId": str,
+    },
+)
+
+TableTypeDef = TypedDict(
+    "TableTypeDef",
+    {
+        "Name": str,
+        "DatabaseName": str,
+        "Description": str,
+        "Owner": str,
+        "CreateTime": datetime,
+        "UpdateTime": datetime,
+        "LastAccessTime": datetime,
+        "LastAnalyzedTime": datetime,
+        "Retention": int,
+        "StorageDescriptor": StorageDescriptorOutputTypeDef,
+        "PartitionKeys": List[ColumnOutputTypeDef],
+        "ViewOriginalText": str,
+        "ViewExpandedText": str,
+        "TableType": str,
+        "Parameters": Dict[str, str],
+        "CreatedBy": str,
+        "IsRegisteredWithLakeFormation": bool,
+        "TargetTable": TableIdentifierOutputTypeDef,
+        "CatalogId": str,
+        "VersionId": str,
+        "FederatedTable": FederatedTableTypeDef,
+    },
+)
+
 GetStatementResponseTypeDef = TypedDict(
     "GetStatementResponseTypeDef",
     {
         "Statement": StatementTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9526,48 +10912,46 @@
         "Type": NodeTypeType,
         "Name": str,
         "UniqueId": str,
         "TriggerDetails": TriggerNodeDetailsTypeDef,
         "JobDetails": JobNodeDetailsTypeDef,
         "CrawlerDetails": CrawlerNodeDetailsTypeDef,
     },
-    total=False,
 )
 
 GetMLTransformsResponseTypeDef = TypedDict(
     "GetMLTransformsResponseTypeDef",
     {
         "Transforms": List[MLTransformTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ColumnStatisticsErrorTypeDef = TypedDict(
     "ColumnStatisticsErrorTypeDef",
     {
-        "ColumnStatistics": ColumnStatisticsTypeDef,
+        "ColumnStatistics": ColumnStatisticsOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 GetColumnStatisticsForPartitionResponseTypeDef = TypedDict(
     "GetColumnStatisticsForPartitionResponseTypeDef",
     {
-        "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
+        "ColumnStatisticsList": List[ColumnStatisticsOutputTypeDef],
         "Errors": List[ColumnErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetColumnStatisticsForTableResponseTypeDef = TypedDict(
     "GetColumnStatisticsForTableResponseTypeDef",
     {
-        "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
+        "ColumnStatisticsList": List[ColumnStatisticsOutputTypeDef],
         "Errors": List[ColumnErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
@@ -9582,22 +10966,20 @@
     "_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnStatisticsList": Sequence[ColumnStatisticsTypeDef],
     },
@@ -9606,22 +10988,20 @@
     "_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchCreatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionInputList": Sequence[PartitionInputTypeDef],
     },
@@ -9630,22 +11010,20 @@
     "_OptionalBatchCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchCreatePartitionRequestRequestTypeDef(
     _RequiredBatchCreatePartitionRequestRequestTypeDef,
     _OptionalBatchCreatePartitionRequestRequestTypeDef,
 ):
     pass
 
-
 BatchUpdatePartitionRequestEntryTypeDef = TypedDict(
     "BatchUpdatePartitionRequestEntryTypeDef",
     {
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
     },
 )
@@ -9662,21 +11040,19 @@
     "_OptionalCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class CreatePartitionRequestRequestTypeDef(
     _RequiredCreatePartitionRequestRequestTypeDef, _OptionalCreatePartitionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
@@ -9686,67 +11062,19 @@
     "_OptionalUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdatePartitionRequestRequestTypeDef(
     _RequiredUpdatePartitionRequestRequestTypeDef, _OptionalUpdatePartitionRequestRequestTypeDef
 ):
     pass
 
-
-BatchGetPartitionResponseTypeDef = TypedDict(
-    "BatchGetPartitionResponseTypeDef",
-    {
-        "Partitions": List[PartitionTypeDef],
-        "UnprocessedKeys": List[PartitionValueListTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPartitionResponseTypeDef = TypedDict(
-    "GetPartitionResponseTypeDef",
-    {
-        "Partition": PartitionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPartitionsResponseTypeDef = TypedDict(
-    "GetPartitionsResponseTypeDef",
-    {
-        "Partitions": List[PartitionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUnfilteredPartitionMetadataResponseTypeDef = TypedDict(
-    "GetUnfilteredPartitionMetadataResponseTypeDef",
-    {
-        "Partition": PartitionTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UnfilteredPartitionTypeDef = TypedDict(
-    "UnfilteredPartitionTypeDef",
-    {
-        "Partition": PartitionTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-    },
-    total=False,
-)
-
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableInput": TableInputTypeDef,
     },
 )
@@ -9757,21 +11085,19 @@
         "PartitionIndexes": Sequence[PartitionIndexTypeDef],
         "TransactionId": str,
         "OpenTableFormatInput": OpenTableFormatInputTypeDef,
     },
     total=False,
 )
 
-
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableInput": TableInputTypeDef,
     },
 )
@@ -9782,65 +11108,46 @@
         "SkipArchive": bool,
         "TransactionId": str,
         "VersionId": str,
     },
     total=False,
 )
 
-
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
-
-GetTableResponseTypeDef = TypedDict(
-    "GetTableResponseTypeDef",
-    {
-        "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTablesResponseTypeDef = TypedDict(
-    "GetTablesResponseTypeDef",
-    {
-        "TableList": List[TableTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUnfilteredTableMetadataResponseTypeDef = TypedDict(
-    "GetUnfilteredTableMetadataResponseTypeDef",
-    {
-        "Table": TableTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-        "CellFilters": List[ColumnRowFilterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchTablesResponseTypeDef = TypedDict(
-    "SearchTablesResponseTypeDef",
-    {
-        "NextToken": str,
-        "TableList": List[TableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TableVersionTypeDef = TypedDict(
-    "TableVersionTypeDef",
+JobTypeDef = TypedDict(
+    "JobTypeDef",
     {
-        "Table": TableTypeDef,
-        "VersionId": str,
+        "Name": str,
+        "Description": str,
+        "LogUri": str,
+        "Role": str,
+        "CreatedOn": datetime,
+        "LastModifiedOn": datetime,
+        "ExecutionProperty": ExecutionPropertyOutputTypeDef,
+        "Command": JobCommandOutputTypeDef,
+        "DefaultArguments": Dict[str, str],
+        "NonOverridableArguments": Dict[str, str],
+        "Connections": ConnectionsListOutputTypeDef,
+        "MaxRetries": int,
+        "AllocatedCapacity": int,
+        "Timeout": int,
+        "MaxCapacity": float,
+        "WorkerType": WorkerTypeType,
+        "NumberOfWorkers": int,
+        "SecurityConfiguration": str,
+        "NotificationProperty": NotificationPropertyOutputTypeDef,
+        "GlueVersion": str,
+        "CodeGenConfigurationNodes": Dict[str, CodeGenConfigurationNodeOutputTypeDef],
+        "ExecutionClass": ExecutionClassType,
+        "SourceControlDetails": SourceControlDetailsOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "Name": str,
         "Role": str,
@@ -9869,51 +11176,19 @@
         "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
-
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-
-JobTypeDef = TypedDict(
-    "JobTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "LogUri": str,
-        "Role": str,
-        "CreatedOn": datetime,
-        "LastModifiedOn": datetime,
-        "ExecutionProperty": ExecutionPropertyTypeDef,
-        "Command": JobCommandTypeDef,
-        "DefaultArguments": Dict[str, str],
-        "NonOverridableArguments": Dict[str, str],
-        "Connections": ConnectionsListTypeDef,
-        "MaxRetries": int,
-        "AllocatedCapacity": int,
-        "Timeout": int,
-        "MaxCapacity": float,
-        "WorkerType": WorkerTypeType,
-        "NumberOfWorkers": int,
-        "SecurityConfiguration": str,
-        "NotificationProperty": NotificationPropertyTypeDef,
-        "GlueVersion": str,
-        "CodeGenConfigurationNodes": Dict[str, CodeGenConfigurationNodeTypeDef],
-        "ExecutionClass": ExecutionClassType,
-        "SourceControlDetails": SourceControlDetailsTypeDef,
-    },
-    total=False,
-)
-
 JobUpdateTypeDef = TypedDict(
     "JobUpdateTypeDef",
     {
         "Description": str,
         "LogUri": str,
         "Role": str,
         "ExecutionProperty": ExecutionPropertyTypeDef,
@@ -9933,21 +11208,110 @@
         "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
+BatchGetPartitionResponseTypeDef = TypedDict(
+    "BatchGetPartitionResponseTypeDef",
+    {
+        "Partitions": List[PartitionTypeDef],
+        "UnprocessedKeys": List[PartitionValueListOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPartitionResponseTypeDef = TypedDict(
+    "GetPartitionResponseTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPartitionsResponseTypeDef = TypedDict(
+    "GetPartitionsResponseTypeDef",
+    {
+        "Partitions": List[PartitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUnfilteredPartitionMetadataResponseTypeDef = TypedDict(
+    "GetUnfilteredPartitionMetadataResponseTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnfilteredPartitionTypeDef = TypedDict(
+    "UnfilteredPartitionTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+    },
+)
+
+GetTableResponseTypeDef = TypedDict(
+    "GetTableResponseTypeDef",
+    {
+        "Table": TableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTablesResponseTypeDef = TypedDict(
+    "GetTablesResponseTypeDef",
+    {
+        "TableList": List[TableTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUnfilteredTableMetadataResponseTypeDef = TypedDict(
+    "GetUnfilteredTableMetadataResponseTypeDef",
+    {
+        "Table": TableTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+        "CellFilters": List[ColumnRowFilterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchTablesResponseTypeDef = TypedDict(
+    "SearchTablesResponseTypeDef",
+    {
+        "NextToken": str,
+        "TableList": List[TableTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableVersionTypeDef = TypedDict(
+    "TableVersionTypeDef",
+    {
+        "Table": TableTypeDef,
+        "VersionId": str,
+    },
+)
+
 WorkflowGraphTypeDef = TypedDict(
     "WorkflowGraphTypeDef",
     {
         "Nodes": List[NodeTypeDef],
         "Edges": List[EdgeTypeDef],
     },
-    total=False,
 )
 
 UpdateColumnStatisticsForPartitionResponseTypeDef = TypedDict(
     "UpdateColumnStatisticsForPartitionResponseTypeDef",
     {
         "Errors": List[ColumnStatisticsErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -9974,48 +11338,20 @@
     "_OptionalBatchUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchUpdatePartitionRequestRequestTypeDef(
     _RequiredBatchUpdatePartitionRequestRequestTypeDef,
     _OptionalBatchUpdatePartitionRequestRequestTypeDef,
 ):
     pass
 
-
-GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
-    "GetUnfilteredPartitionsMetadataResponseTypeDef",
-    {
-        "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTableVersionResponseTypeDef = TypedDict(
-    "GetTableVersionResponseTypeDef",
-    {
-        "TableVersion": TableVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTableVersionsResponseTypeDef = TypedDict(
-    "GetTableVersionsResponseTypeDef",
-    {
-        "TableVersions": List[TableVersionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetJobsResponseTypeDef = TypedDict(
     "BatchGetJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "JobsNotFound": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -10042,14 +11378,40 @@
     "UpdateJobRequestRequestTypeDef",
     {
         "JobName": str,
         "JobUpdate": JobUpdateTypeDef,
     },
 )
 
+GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
+    "GetUnfilteredPartitionsMetadataResponseTypeDef",
+    {
+        "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTableVersionResponseTypeDef = TypedDict(
+    "GetTableVersionResponseTypeDef",
+    {
+        "TableVersion": TableVersionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTableVersionsResponseTypeDef = TypedDict(
+    "GetTableVersionsResponseTypeDef",
+    {
+        "TableVersions": List[TableVersionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 WorkflowRunTypeDef = TypedDict(
     "WorkflowRunTypeDef",
     {
         "Name": str,
         "WorkflowRunId": str,
         "PreviousRunId": str,
         "WorkflowRunProperties": Dict[str, str],
@@ -10057,15 +11419,14 @@
         "CompletedOn": datetime,
         "Status": WorkflowRunStatusType,
         "ErrorMessage": str,
         "Statistics": WorkflowRunStatisticsTypeDef,
         "Graph": WorkflowGraphTypeDef,
         "StartingEventBatchCondition": StartingEventBatchConditionTypeDef,
     },
-    total=False,
 )
 
 GetWorkflowRunResponseTypeDef = TypedDict(
     "GetWorkflowRunResponseTypeDef",
     {
         "Run": WorkflowRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -10090,15 +11451,14 @@
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
         "LastRun": WorkflowRunTypeDef,
         "Graph": WorkflowGraphTypeDef,
         "MaxConcurrentRuns": int,
         "BlueprintDetails": BlueprintDetailsTypeDef,
     },
-    total=False,
 )
 
 BatchGetWorkflowsResponseTypeDef = TypedDict(
     "BatchGetWorkflowsResponseTypeDef",
     {
         "Workflows": List[WorkflowTypeDef],
         "MissingWorkflows": List[str],
```

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue/type_defs.pyi` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 Type annotations for glue service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_glue.type_defs import NotificationPropertyTypeDef
+    from mypy_boto3_glue.type_defs import NotificationPropertyOutputTypeDef
 
-    data: NotificationPropertyTypeDef = {...}
+    data: NotificationPropertyOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
+
+from botocore.response import StreamingBody
 
 from .literals import (
     AggFunctionType,
     BackfillErrorCodeType,
     BlueprintRunStateType,
     BlueprintStatusType,
     CatalogEncryptionModeType,
@@ -104,63 +106,103 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "NotificationPropertyOutputTypeDef",
     "NotificationPropertyTypeDef",
+    "AggregateOperationOutputTypeDef",
     "AggregateOperationTypeDef",
+    "AmazonRedshiftAdvancedOptionOutputTypeDef",
     "AmazonRedshiftAdvancedOptionTypeDef",
+    "OptionOutputTypeDef",
     "OptionTypeDef",
+    "ApplyMappingOutputTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
-    "PartitionValueListTypeDef",
+    "PartitionValueListOutputTypeDef",
+    "BasicCatalogTargetOutputTypeDef",
     "BasicCatalogTargetTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteConnectionRequestRequestTypeDef",
     "ErrorDetailTypeDef",
+    "PartitionValueListTypeDef",
     "BatchDeleteTableRequestRequestTypeDef",
     "BatchDeleteTableVersionRequestRequestTypeDef",
     "BatchGetBlueprintsRequestRequestTypeDef",
     "BatchGetCrawlersRequestRequestTypeDef",
     "BatchGetCustomEntityTypesRequestRequestTypeDef",
     "CustomEntityTypeTypeDef",
     "BatchGetDataQualityResultRequestRequestTypeDef",
     "BatchGetDevEndpointsRequestRequestTypeDef",
     "DevEndpointTypeDef",
     "BatchGetJobsRequestRequestTypeDef",
     "BatchGetTriggersRequestRequestTypeDef",
     "BatchGetWorkflowsRequestRequestTypeDef",
     "BatchStopJobRunRequestRequestTypeDef",
     "BatchStopJobRunSuccessfulSubmissionTypeDef",
+    "BinaryColumnStatisticsDataOutputTypeDef",
     "BinaryColumnStatisticsDataTypeDef",
     "BlueprintDetailsTypeDef",
     "BlueprintRunTypeDef",
     "LastActiveDefinitionTypeDef",
+    "BooleanColumnStatisticsDataOutputTypeDef",
     "BooleanColumnStatisticsDataTypeDef",
     "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
     "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CancelMLTaskRunRequestRequestTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "CatalogEntryTypeDef",
     "CatalogImportStatusTypeDef",
+    "KafkaStreamingSourceOptionsOutputTypeDef",
+    "StreamingDataPreviewOptionsOutputTypeDef",
     "KafkaStreamingSourceOptionsTypeDef",
     "StreamingDataPreviewOptionsTypeDef",
+    "KinesisStreamingSourceOptionsOutputTypeDef",
     "KinesisStreamingSourceOptionsTypeDef",
+    "CatalogSchemaChangePolicyOutputTypeDef",
     "CatalogSchemaChangePolicyTypeDef",
+    "CatalogSourceOutputTypeDef",
     "CatalogSourceTypeDef",
+    "CatalogTargetOutputTypeDef",
     "CatalogTargetTypeDef",
     "CheckSchemaVersionValidityInputRequestTypeDef",
     "CsvClassifierTypeDef",
     "GrokClassifierTypeDef",
     "JsonClassifierTypeDef",
     "XMLClassifierTypeDef",
+    "CloudWatchEncryptionOutputTypeDef",
     "CloudWatchEncryptionTypeDef",
+    "DirectJDBCSourceOutputTypeDef",
+    "DropDuplicatesOutputTypeDef",
+    "DropFieldsOutputTypeDef",
+    "DynamoDBCatalogSourceOutputTypeDef",
+    "FillMissingValuesOutputTypeDef",
+    "MergeOutputTypeDef",
+    "MicrosoftSQLServerCatalogSourceOutputTypeDef",
+    "MicrosoftSQLServerCatalogTargetOutputTypeDef",
+    "MySQLCatalogSourceOutputTypeDef",
+    "MySQLCatalogTargetOutputTypeDef",
+    "OracleSQLCatalogSourceOutputTypeDef",
+    "OracleSQLCatalogTargetOutputTypeDef",
+    "PIIDetectionOutputTypeDef",
+    "PostgreSQLCatalogSourceOutputTypeDef",
+    "PostgreSQLCatalogTargetOutputTypeDef",
+    "RedshiftSourceOutputTypeDef",
+    "RelationalCatalogSourceOutputTypeDef",
+    "RenameFieldOutputTypeDef",
+    "SelectFieldsOutputTypeDef",
+    "SelectFromCollectionOutputTypeDef",
+    "SpigotOutputTypeDef",
+    "SplitFieldsOutputTypeDef",
+    "UnionOutputTypeDef",
     "DirectJDBCSourceTypeDef",
     "DropDuplicatesTypeDef",
     "DropFieldsTypeDef",
     "DynamoDBCatalogSourceTypeDef",
     "FillMissingValuesTypeDef",
     "MergeTypeDef",
     "MicrosoftSQLServerCatalogSourceTypeDef",
@@ -176,71 +218,103 @@
     "RelationalCatalogSourceTypeDef",
     "RenameFieldTypeDef",
     "SelectFieldsTypeDef",
     "SelectFromCollectionTypeDef",
     "SpigotTypeDef",
     "SplitFieldsTypeDef",
     "UnionTypeDef",
+    "CodeGenEdgeOutputTypeDef",
     "CodeGenEdgeTypeDef",
+    "CodeGenNodeArgOutputTypeDef",
     "CodeGenNodeArgTypeDef",
     "ColumnImportanceTypeDef",
+    "ColumnOutputTypeDef",
     "ColumnRowFilterTypeDef",
+    "DateColumnStatisticsDataOutputTypeDef",
+    "DoubleColumnStatisticsDataOutputTypeDef",
+    "LongColumnStatisticsDataOutputTypeDef",
+    "StringColumnStatisticsDataOutputTypeDef",
     "DateColumnStatisticsDataTypeDef",
     "DoubleColumnStatisticsDataTypeDef",
     "LongColumnStatisticsDataTypeDef",
     "StringColumnStatisticsDataTypeDef",
     "ColumnTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "ConfusionMatrixTypeDef",
     "PhysicalConnectionRequirementsTypeDef",
+    "ConnectionPasswordEncryptionOutputTypeDef",
     "ConnectionPasswordEncryptionTypeDef",
+    "PhysicalConnectionRequirementsOutputTypeDef",
+    "ConnectionsListOutputTypeDef",
     "ConnectionsListTypeDef",
     "CrawlTypeDef",
     "CrawlerHistoryTypeDef",
     "CrawlerMetricsTypeDef",
+    "DeltaTargetOutputTypeDef",
+    "DynamoDBTargetOutputTypeDef",
+    "IcebergTargetOutputTypeDef",
+    "JdbcTargetOutputTypeDef",
+    "MongoDBTargetOutputTypeDef",
+    "S3TargetOutputTypeDef",
     "DeltaTargetTypeDef",
     "DynamoDBTargetTypeDef",
     "IcebergTargetTypeDef",
     "JdbcTargetTypeDef",
     "MongoDBTargetTypeDef",
     "S3TargetTypeDef",
-    "LakeFormationConfigurationTypeDef",
+    "LakeFormationConfigurationOutputTypeDef",
     "LastCrawlInfoTypeDef",
-    "LineageConfigurationTypeDef",
-    "RecrawlPolicyTypeDef",
+    "LineageConfigurationOutputTypeDef",
+    "RecrawlPolicyOutputTypeDef",
     "ScheduleTypeDef",
-    "SchemaChangePolicyTypeDef",
+    "SchemaChangePolicyOutputTypeDef",
     "CrawlsFilterTypeDef",
     "CreateBlueprintRequestRequestTypeDef",
     "CreateCsvClassifierRequestTypeDef",
     "CreateGrokClassifierRequestTypeDef",
     "CreateJsonClassifierRequestTypeDef",
     "CreateXMLClassifierRequestTypeDef",
+    "LakeFormationConfigurationTypeDef",
+    "LineageConfigurationTypeDef",
+    "RecrawlPolicyTypeDef",
+    "SchemaChangePolicyTypeDef",
     "CreateCustomEntityTypeRequestRequestTypeDef",
     "DataQualityTargetTableTypeDef",
     "CreateDevEndpointRequestRequestTypeDef",
     "ExecutionPropertyTypeDef",
     "JobCommandTypeDef",
     "SourceControlDetailsTypeDef",
     "GlueTableTypeDef",
     "PartitionIndexTypeDef",
     "CreateRegistryInputRequestTypeDef",
     "RegistryIdTypeDef",
     "SessionCommandTypeDef",
     "EventBatchingConditionTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
+    "DQResultsPublishingOptionsOutputTypeDef",
     "DQResultsPublishingOptionsTypeDef",
+    "DQStopJobOnFailureOptionsOutputTypeDef",
     "DQStopJobOnFailureOptionsTypeDef",
+    "EncryptionAtRestOutputTypeDef",
     "EncryptionAtRestTypeDef",
+    "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
+    "DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef",
     "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
     "DataQualityRuleResultTypeDef",
+    "DataQualityTargetTableOutputTypeDef",
+    "GlueTableOutputTypeDef",
+    "DatabaseIdentifierOutputTypeDef",
     "DatabaseIdentifierTypeDef",
     "FederatedDatabaseTypeDef",
+    "FederatedDatabaseOutputTypeDef",
+    "DatatypeOutputTypeDef",
     "DatatypeTypeDef",
+    "DecimalNumberOutputTypeDef",
     "DecimalNumberTypeDef",
     "DeleteBlueprintRequestRequestTypeDef",
     "DeleteClassifierRequestRequestTypeDef",
     "DeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     "DeleteColumnStatisticsForTableRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteCrawlerRequestRequestTypeDef",
@@ -258,24 +332,33 @@
     "DeleteSessionRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DeleteTableVersionRequestRequestTypeDef",
     "DeleteTriggerRequestRequestTypeDef",
     "DeleteUserDefinedFunctionRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DevEndpointCustomLibrariesTypeDef",
+    "DirectSchemaChangePolicyOutputTypeDef",
     "DirectSchemaChangePolicyTypeDef",
+    "NullCheckBoxListOutputTypeDef",
     "NullCheckBoxListTypeDef",
+    "TransformConfigParameterOutputTypeDef",
     "TransformConfigParameterTypeDef",
     "EdgeTypeDef",
+    "JobBookmarksEncryptionOutputTypeDef",
+    "S3EncryptionOutputTypeDef",
     "JobBookmarksEncryptionTypeDef",
     "S3EncryptionTypeDef",
     "ErrorDetailsTypeDef",
+    "EventBatchingConditionOutputTypeDef",
+    "ExecutionPropertyOutputTypeDef",
     "ExportLabelsTaskRunPropertiesTypeDef",
     "FederatedTableTypeDef",
+    "FilterValueOutputTypeDef",
     "FilterValueTypeDef",
+    "FindMatchesParametersOutputTypeDef",
     "FindMatchesParametersTypeDef",
     "FindMatchesTaskRunPropertiesTypeDef",
     "GetBlueprintRequestRequestTypeDef",
     "GetBlueprintRunRequestRequestTypeDef",
     "GetBlueprintRunsRequestRequestTypeDef",
     "GetCatalogImportStatusRequestRequestTypeDef",
     "GetClassifierRequestRequestTypeDef",
@@ -305,20 +388,21 @@
     "GetJobRunRequestRequestTypeDef",
     "GetJobRunsRequestRequestTypeDef",
     "GetJobsRequestRequestTypeDef",
     "GetMLTaskRunRequestRequestTypeDef",
     "TaskRunFilterCriteriaTypeDef",
     "TaskRunSortCriteriaTypeDef",
     "GetMLTransformRequestRequestTypeDef",
-    "SchemaColumnTypeDef",
+    "SchemaColumnOutputTypeDef",
     "TransformSortCriteriaTypeDef",
-    "MappingEntryTypeDef",
+    "MappingEntryOutputTypeDef",
     "GetPartitionIndexesRequestRequestTypeDef",
     "GetPartitionRequestRequestTypeDef",
     "SegmentTypeDef",
+    "MappingEntryTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GluePolicyTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "SchemaVersionNumberTypeDef",
     "GetSecurityConfigurationRequestRequestTypeDef",
     "GetSecurityConfigurationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
@@ -332,21 +416,27 @@
     "GetTriggersRequestRequestTypeDef",
     "GetUserDefinedFunctionRequestRequestTypeDef",
     "GetUserDefinedFunctionsRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     "GetWorkflowRunRequestRequestTypeDef",
     "GetWorkflowRunsRequestRequestTypeDef",
+    "GlueStudioSchemaColumnOutputTypeDef",
     "GlueStudioSchemaColumnTypeDef",
+    "S3SourceAdditionalOptionsOutputTypeDef",
     "S3SourceAdditionalOptionsTypeDef",
     "IcebergInputTypeDef",
     "ImportCatalogToGlueRequestRequestTypeDef",
     "ImportLabelsTaskRunPropertiesTypeDef",
+    "JDBCConnectorOptionsOutputTypeDef",
     "JDBCConnectorOptionsTypeDef",
+    "JobCommandOutputTypeDef",
     "PredecessorTypeDef",
+    "SourceControlDetailsOutputTypeDef",
+    "JoinColumnOutputTypeDef",
     "JoinColumnTypeDef",
     "KeySchemaElementTypeDef",
     "LabelingSetGenerationTaskRunPropertiesTypeDef",
     "ListBlueprintsRequestRequestTypeDef",
     "ListCrawlersRequestRequestTypeDef",
     "ListCustomEntityTypesRequestRequestTypeDef",
     "ListDevEndpointsRequestRequestTypeDef",
@@ -355,31 +445,43 @@
     "RegistryListItemTypeDef",
     "SchemaVersionListItemTypeDef",
     "SchemaListItemTypeDef",
     "ListSessionsRequestRequestTypeDef",
     "ListStatementsRequestRequestTypeDef",
     "ListTriggersRequestRequestTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
+    "MLUserDataEncryptionOutputTypeDef",
     "MLUserDataEncryptionTypeDef",
+    "MappingOutputTypeDef",
     "MappingTypeDef",
     "OtherMetadataValueListItemTypeDef",
     "MetadataKeyValuePairTypeDef",
+    "OrderOutputTypeDef",
     "OrderTypeDef",
     "PropertyPredicateTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
+    "UpsertRedshiftTargetOptionsOutputTypeDef",
     "UpsertRedshiftTargetOptionsTypeDef",
     "ResetJobBookmarkRequestRequestTypeDef",
+    "ResourceUriOutputTypeDef",
     "ResourceUriTypeDef",
     "ResumeWorkflowRunRequestRequestTypeDef",
     "RunStatementRequestRequestTypeDef",
+    "S3DirectSourceAdditionalOptionsOutputTypeDef",
     "S3DirectSourceAdditionalOptionsTypeDef",
+    "SchemaColumnTypeDef",
+    "SchemaIdOutputTypeDef",
     "SortCriterionTypeDef",
+    "SerDeInfoOutputTypeDef",
     "SerDeInfoTypeDef",
+    "SessionCommandOutputTypeDef",
+    "SkewedInfoOutputTypeDef",
     "SkewedInfoTypeDef",
+    "SqlAliasOutputTypeDef",
     "SqlAliasTypeDef",
     "StartBlueprintRunRequestRequestTypeDef",
     "StartCrawlerRequestRequestTypeDef",
     "StartCrawlerScheduleRequestRequestTypeDef",
     "StartExportLabelsTaskRunRequestRequestTypeDef",
     "StartImportLabelsTaskRunRequestRequestTypeDef",
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
@@ -389,37 +491,39 @@
     "StartingEventBatchConditionTypeDef",
     "StatementOutputDataTypeDef",
     "StopCrawlerRequestRequestTypeDef",
     "StopCrawlerScheduleRequestRequestTypeDef",
     "StopSessionRequestRequestTypeDef",
     "StopTriggerRequestRequestTypeDef",
     "StopWorkflowRunRequestRequestTypeDef",
+    "TableIdentifierOutputTypeDef",
     "TableIdentifierTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBlueprintRequestRequestTypeDef",
     "UpdateCsvClassifierRequestTypeDef",
     "UpdateGrokClassifierRequestTypeDef",
     "UpdateJsonClassifierRequestTypeDef",
     "UpdateXMLClassifierRequestTypeDef",
     "UpdateCrawlerScheduleRequestRequestTypeDef",
     "UpdateDataQualityRulesetRequestRequestTypeDef",
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "WorkflowRunStatisticsTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
+    "AggregateOutputTypeDef",
     "AggregateTypeDef",
+    "AmazonRedshiftNodeDataOutputTypeDef",
     "AmazonRedshiftNodeDataTypeDef",
     "GetUnfilteredPartitionMetadataRequestRequestTypeDef",
     "GetUnfilteredTableMetadataRequestRequestTypeDef",
     "BackfillErrorTypeDef",
-    "BatchDeletePartitionRequestRequestTypeDef",
-    "BatchGetPartitionRequestRequestTypeDef",
     "CancelMLTaskRunResponseTypeDef",
     "CheckSchemaVersionValidityResponseTypeDef",
     "CreateBlueprintResponseTypeDef",
     "CreateCustomEntityTypeResponseTypeDef",
     "CreateDataQualityRulesetResponseTypeDef",
     "CreateDevEndpointResponseTypeDef",
     "CreateJobResponseTypeDef",
@@ -486,78 +590,104 @@
     "BatchDeleteConnectionResponseTypeDef",
     "BatchStopJobRunErrorTypeDef",
     "BatchUpdatePartitionFailureEntryTypeDef",
     "ColumnErrorTypeDef",
     "PartitionErrorTypeDef",
     "TableErrorTypeDef",
     "TableVersionErrorTypeDef",
+    "BatchDeletePartitionRequestRequestTypeDef",
+    "BatchGetPartitionRequestRequestTypeDef",
     "BatchGetCustomEntityTypesResponseTypeDef",
     "ListCustomEntityTypesResponseTypeDef",
     "BatchGetDevEndpointsResponseTypeDef",
     "GetDevEndpointResponseTypeDef",
     "GetDevEndpointsResponseTypeDef",
     "GetBlueprintRunResponseTypeDef",
     "GetBlueprintRunsResponseTypeDef",
     "BlueprintTypeDef",
     "GetCatalogImportStatusResponseTypeDef",
+    "CatalogKafkaSourceOutputTypeDef",
+    "DirectKafkaSourceOutputTypeDef",
     "CatalogKafkaSourceTypeDef",
     "DirectKafkaSourceTypeDef",
+    "CatalogKinesisSourceOutputTypeDef",
+    "DirectKinesisSourceOutputTypeDef",
     "CatalogKinesisSourceTypeDef",
     "DirectKinesisSourceTypeDef",
+    "GovernedCatalogTargetOutputTypeDef",
+    "S3CatalogTargetOutputTypeDef",
+    "S3DeltaCatalogTargetOutputTypeDef",
+    "S3HudiCatalogTargetOutputTypeDef",
     "GovernedCatalogTargetTypeDef",
     "S3CatalogTargetTypeDef",
     "S3DeltaCatalogTargetTypeDef",
     "S3HudiCatalogTargetTypeDef",
     "ClassifierTypeDef",
+    "CodeGenNodeOutputTypeDef",
     "CodeGenNodeTypeDef",
     "LocationTypeDef",
+    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "FindMatchesMetricsTypeDef",
     "ConnectionInputTypeDef",
     "ConnectionTypeDef",
     "CrawlerNodeDetailsTypeDef",
     "ListCrawlsResponseTypeDef",
     "GetCrawlerMetricsResponseTypeDef",
+    "CrawlerTargetsOutputTypeDef",
     "CrawlerTargetsTypeDef",
     "ListCrawlsRequestRequestTypeDef",
     "CreateClassifierRequestRequestTypeDef",
     "CreateDataQualityRulesetRequestRequestTypeDef",
     "DataQualityRulesetFilterCriteriaTypeDef",
-    "DataQualityRulesetListDetailsTypeDef",
-    "GetDataQualityRulesetResponseTypeDef",
     "DataSourceTypeDef",
     "CreatePartitionIndexRequestRequestTypeDef",
     "CreateSchemaInputRequestTypeDef",
     "DeleteRegistryInputRequestTypeDef",
     "GetRegistryInputRequestTypeDef",
     "ListSchemasInputRequestTypeDef",
     "UpdateRegistryInputRequestTypeDef",
     "CreateSessionRequestRequestTypeDef",
-    "SessionTypeDef",
+    "EvaluateDataQualityMultiFrameOutputTypeDef",
+    "EvaluateDataQualityOutputTypeDef",
     "EvaluateDataQualityMultiFrameTypeDef",
     "EvaluateDataQualityTypeDef",
+    "DataCatalogEncryptionSettingsOutputTypeDef",
     "DataCatalogEncryptionSettingsTypeDef",
+    "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
+    "DataQualityRulesetListDetailsTypeDef",
+    "GetDataQualityRulesetResponseTypeDef",
+    "DataSourceOutputTypeDef",
+    "NullValueFieldOutputTypeDef",
     "NullValueFieldTypeDef",
+    "DecimalColumnStatisticsDataOutputTypeDef",
     "DecimalColumnStatisticsDataTypeDef",
     "DeleteSchemaInputRequestTypeDef",
     "DeleteSchemaVersionsInputRequestTypeDef",
     "GetSchemaByDefinitionInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "ListSchemaVersionsInputRequestTypeDef",
     "RegisterSchemaVersionInputRequestTypeDef",
     "SchemaReferenceTypeDef",
     "UpdateDevEndpointRequestRequestTypeDef",
+    "S3DeltaDirectTargetOutputTypeDef",
+    "S3DirectTargetOutputTypeDef",
+    "S3GlueParquetTargetOutputTypeDef",
+    "S3HudiDirectTargetOutputTypeDef",
     "S3DeltaDirectTargetTypeDef",
     "S3DirectTargetTypeDef",
     "S3GlueParquetTargetTypeDef",
     "S3HudiDirectTargetTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "SchemaVersionErrorItemTypeDef",
+    "FilterExpressionOutputTypeDef",
     "FilterExpressionTypeDef",
+    "TransformParametersOutputTypeDef",
     "TransformParametersTypeDef",
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
     "GetCrawlersRequestGetCrawlersPaginateTypeDef",
     "GetDatabasesRequestGetDatabasesPaginateTypeDef",
     "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
     "GetJobRunsRequestGetJobRunsPaginateTypeDef",
@@ -573,103 +703,128 @@
     "ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
     "ListSchemasInputListSchemasPaginateTypeDef",
     "GetConnectionsRequestGetConnectionsPaginateTypeDef",
     "GetConnectionsRequestRequestTypeDef",
     "GetJobBookmarkResponseTypeDef",
     "ResetJobBookmarkResponseTypeDef",
     "GetMLTaskRunsRequestRequestTypeDef",
-    "TransformFilterCriteriaTypeDef",
     "GetMappingResponseTypeDef",
     "GetPartitionsRequestGetPartitionsPaginateTypeDef",
     "GetPartitionsRequestRequestTypeDef",
     "GetUnfilteredPartitionsMetadataRequestRequestTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetSchemaVersionInputRequestTypeDef",
     "GetSchemaVersionsDiffInputRequestTypeDef",
     "UpdateSchemaInputRequestTypeDef",
+    "GlueSchemaOutputTypeDef",
     "GlueSchemaTypeDef",
+    "GovernedCatalogSourceOutputTypeDef",
+    "S3CatalogSourceOutputTypeDef",
     "GovernedCatalogSourceTypeDef",
     "S3CatalogSourceTypeDef",
     "OpenTableFormatInputTypeDef",
     "JobRunTypeDef",
+    "JoinOutputTypeDef",
     "JoinTypeDef",
     "TaskRunPropertiesTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
+    "TransformEncryptionOutputTypeDef",
     "TransformEncryptionTypeDef",
     "MetadataInfoTypeDef",
     "PutSchemaVersionMetadataInputRequestTypeDef",
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     "RemoveSchemaVersionMetadataInputRequestTypeDef",
+    "RedshiftTargetOutputTypeDef",
     "RedshiftTargetTypeDef",
-    "UserDefinedFunctionInputTypeDef",
     "UserDefinedFunctionTypeDef",
+    "UserDefinedFunctionInputTypeDef",
+    "TransformFilterCriteriaTypeDef",
+    "SchemaReferenceOutputTypeDef",
     "SearchTablesRequestRequestTypeDef",
+    "SessionTypeDef",
     "StatementOutputTypeDef",
     "UpdateClassifierRequestRequestTypeDef",
+    "AmazonRedshiftSourceOutputTypeDef",
+    "AmazonRedshiftTargetOutputTypeDef",
     "AmazonRedshiftSourceTypeDef",
     "AmazonRedshiftTargetTypeDef",
     "PartitionIndexDescriptorTypeDef",
     "BatchStopJobRunResponseTypeDef",
     "BatchUpdatePartitionResponseTypeDef",
     "BatchCreatePartitionResponseTypeDef",
     "BatchDeletePartitionResponseTypeDef",
     "BatchDeleteTableResponseTypeDef",
     "BatchDeleteTableVersionResponseTypeDef",
     "BatchGetBlueprintsResponseTypeDef",
     "GetBlueprintResponseTypeDef",
     "GetClassifierResponseTypeDef",
     "GetClassifiersResponseTypeDef",
-    "CreateScriptRequestRequestTypeDef",
     "GetDataflowGraphResponseTypeDef",
+    "CreateScriptRequestRequestTypeDef",
     "GetMappingRequestRequestTypeDef",
     "GetPlanRequestRequestTypeDef",
-    "CreateTriggerRequestRequestTypeDef",
     "TriggerTypeDef",
+    "CreateTriggerRequestRequestTypeDef",
     "TriggerUpdateTypeDef",
     "EvaluationMetricsTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "GetConnectionResponseTypeDef",
     "GetConnectionsResponseTypeDef",
     "CrawlerTypeDef",
     "CreateCrawlerRequestRequestTypeDef",
     "UpdateCrawlerRequestRequestTypeDef",
     "ListDataQualityRulesetsRequestRequestTypeDef",
-    "ListDataQualityRulesetsResponseTypeDef",
-    "DataQualityResultDescriptionTypeDef",
     "DataQualityResultFilterCriteriaTypeDef",
-    "DataQualityResultTypeDef",
-    "DataQualityRuleRecommendationRunDescriptionTypeDef",
     "DataQualityRuleRecommendationRunFilterTypeDef",
-    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
     "DataQualityRulesetEvaluationRunFilterTypeDef",
-    "GetDataQualityResultResponseTypeDef",
-    "GetDataQualityRuleRecommendationRunResponseTypeDef",
-    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
     "StartDataQualityRuleRecommendationRunRequestRequestTypeDef",
     "StartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    "CreateSessionResponseTypeDef",
-    "GetSessionResponseTypeDef",
-    "ListSessionsResponseTypeDef",
     "GetDataCatalogEncryptionSettingsResponseTypeDef",
     "PutDataCatalogEncryptionSettingsRequestRequestTypeDef",
-    "DatabaseInputTypeDef",
     "DatabaseTypeDef",
+    "DatabaseInputTypeDef",
+    "ListDataQualityRulesetsResponseTypeDef",
+    "DataQualityResultDescriptionTypeDef",
+    "DataQualityResultTypeDef",
+    "DataQualityRuleRecommendationRunDescriptionTypeDef",
+    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
+    "GetDataQualityResultResponseTypeDef",
+    "GetDataQualityRuleRecommendationRunResponseTypeDef",
+    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
+    "DropNullFieldsOutputTypeDef",
     "DropNullFieldsTypeDef",
+    "ColumnStatisticsDataOutputTypeDef",
     "ColumnStatisticsDataTypeDef",
     "StorageDescriptorTypeDef",
-    "CreateSecurityConfigurationRequestRequestTypeDef",
     "SecurityConfigurationTypeDef",
+    "CreateSecurityConfigurationRequestRequestTypeDef",
     "DeleteSchemaVersionsResponseTypeDef",
+    "FilterOutputTypeDef",
     "FilterTypeDef",
     "UpdateMLTransformRequestRequestTypeDef",
-    "GetMLTransformsRequestRequestTypeDef",
-    "ListMLTransformsRequestRequestTypeDef",
+    "AthenaConnectorSourceOutputTypeDef",
+    "CatalogDeltaSourceOutputTypeDef",
+    "CatalogHudiSourceOutputTypeDef",
+    "CustomCodeOutputTypeDef",
+    "DynamicTransformOutputTypeDef",
+    "JDBCConnectorSourceOutputTypeDef",
+    "JDBCConnectorTargetOutputTypeDef",
+    "S3CatalogDeltaSourceOutputTypeDef",
+    "S3CatalogHudiSourceOutputTypeDef",
+    "S3CsvSourceOutputTypeDef",
+    "S3DeltaSourceOutputTypeDef",
+    "S3HudiSourceOutputTypeDef",
+    "S3JsonSourceOutputTypeDef",
+    "S3ParquetSourceOutputTypeDef",
+    "SparkConnectorSourceOutputTypeDef",
+    "SparkConnectorTargetOutputTypeDef",
+    "SparkSQLOutputTypeDef",
     "AthenaConnectorSourceTypeDef",
     "CatalogDeltaSourceTypeDef",
     "CatalogHudiSourceTypeDef",
     "CustomCodeTypeDef",
     "DynamicTransformTypeDef",
     "JDBCConnectorSourceTypeDef",
     "JDBCConnectorTargetTypeDef",
@@ -686,164 +841,223 @@
     "GetJobRunResponseTypeDef",
     "GetJobRunsResponseTypeDef",
     "JobNodeDetailsTypeDef",
     "GetMLTaskRunResponseTypeDef",
     "TaskRunTypeDef",
     "CreateMLTransformRequestRequestTypeDef",
     "QuerySchemaVersionMetadataResponseTypeDef",
-    "CreateUserDefinedFunctionRequestRequestTypeDef",
-    "UpdateUserDefinedFunctionRequestRequestTypeDef",
     "GetUserDefinedFunctionResponseTypeDef",
     "GetUserDefinedFunctionsResponseTypeDef",
+    "CreateUserDefinedFunctionRequestRequestTypeDef",
+    "UpdateUserDefinedFunctionRequestRequestTypeDef",
+    "GetMLTransformsRequestRequestTypeDef",
+    "ListMLTransformsRequestRequestTypeDef",
+    "StorageDescriptorOutputTypeDef",
+    "CreateSessionResponseTypeDef",
+    "GetSessionResponseTypeDef",
+    "ListSessionsResponseTypeDef",
     "StatementTypeDef",
     "GetPartitionIndexesResponseTypeDef",
     "BatchGetTriggersResponseTypeDef",
     "GetTriggerResponseTypeDef",
     "GetTriggersResponseTypeDef",
     "TriggerNodeDetailsTypeDef",
     "UpdateTriggerResponseTypeDef",
     "UpdateTriggerRequestRequestTypeDef",
     "GetMLTransformResponseTypeDef",
     "MLTransformTypeDef",
     "BatchGetCrawlersResponseTypeDef",
     "GetCrawlerResponseTypeDef",
     "GetCrawlersResponseTypeDef",
-    "ListDataQualityResultsResponseTypeDef",
     "ListDataQualityResultsRequestRequestTypeDef",
-    "BatchGetDataQualityResultResponseTypeDef",
-    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
     "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
     "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
-    "CreateDatabaseRequestRequestTypeDef",
-    "UpdateDatabaseRequestRequestTypeDef",
     "GetDatabaseResponseTypeDef",
     "GetDatabasesResponseTypeDef",
+    "CreateDatabaseRequestRequestTypeDef",
+    "UpdateDatabaseRequestRequestTypeDef",
+    "ListDataQualityResultsResponseTypeDef",
+    "BatchGetDataQualityResultResponseTypeDef",
+    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+    "ColumnStatisticsOutputTypeDef",
     "ColumnStatisticsTypeDef",
     "PartitionInputTypeDef",
-    "PartitionTypeDef",
     "TableInputTypeDef",
-    "TableTypeDef",
     "GetSecurityConfigurationResponseTypeDef",
     "GetSecurityConfigurationsResponseTypeDef",
+    "CodeGenConfigurationNodeOutputTypeDef",
     "CodeGenConfigurationNodeTypeDef",
     "GetMLTaskRunsResponseTypeDef",
+    "PartitionTypeDef",
+    "TableTypeDef",
     "GetStatementResponseTypeDef",
     "ListStatementsResponseTypeDef",
     "NodeTypeDef",
     "GetMLTransformsResponseTypeDef",
     "ColumnStatisticsErrorTypeDef",
     "GetColumnStatisticsForPartitionResponseTypeDef",
     "GetColumnStatisticsForTableResponseTypeDef",
     "UpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     "UpdateColumnStatisticsForTableRequestRequestTypeDef",
     "BatchCreatePartitionRequestRequestTypeDef",
     "BatchUpdatePartitionRequestEntryTypeDef",
     "CreatePartitionRequestRequestTypeDef",
     "UpdatePartitionRequestRequestTypeDef",
+    "CreateTableRequestRequestTypeDef",
+    "UpdateTableRequestRequestTypeDef",
+    "JobTypeDef",
+    "CreateJobRequestRequestTypeDef",
+    "JobUpdateTypeDef",
     "BatchGetPartitionResponseTypeDef",
     "GetPartitionResponseTypeDef",
     "GetPartitionsResponseTypeDef",
     "GetUnfilteredPartitionMetadataResponseTypeDef",
     "UnfilteredPartitionTypeDef",
-    "CreateTableRequestRequestTypeDef",
-    "UpdateTableRequestRequestTypeDef",
     "GetTableResponseTypeDef",
     "GetTablesResponseTypeDef",
     "GetUnfilteredTableMetadataResponseTypeDef",
     "SearchTablesResponseTypeDef",
     "TableVersionTypeDef",
-    "CreateJobRequestRequestTypeDef",
-    "JobTypeDef",
-    "JobUpdateTypeDef",
     "WorkflowGraphTypeDef",
     "UpdateColumnStatisticsForPartitionResponseTypeDef",
     "UpdateColumnStatisticsForTableResponseTypeDef",
     "BatchUpdatePartitionRequestRequestTypeDef",
-    "GetUnfilteredPartitionsMetadataResponseTypeDef",
-    "GetTableVersionResponseTypeDef",
-    "GetTableVersionsResponseTypeDef",
     "BatchGetJobsResponseTypeDef",
     "GetJobResponseTypeDef",
     "GetJobsResponseTypeDef",
     "UpdateJobRequestRequestTypeDef",
+    "GetUnfilteredPartitionsMetadataResponseTypeDef",
+    "GetTableVersionResponseTypeDef",
+    "GetTableVersionsResponseTypeDef",
     "WorkflowRunTypeDef",
     "GetWorkflowRunResponseTypeDef",
     "GetWorkflowRunsResponseTypeDef",
     "WorkflowTypeDef",
     "BatchGetWorkflowsResponseTypeDef",
     "GetWorkflowResponseTypeDef",
 )
 
+NotificationPropertyOutputTypeDef = TypedDict(
+    "NotificationPropertyOutputTypeDef",
+    {
+        "NotifyDelayAfter": int,
+    },
+)
+
 NotificationPropertyTypeDef = TypedDict(
     "NotificationPropertyTypeDef",
     {
         "NotifyDelayAfter": int,
     },
     total=False,
 )
 
+AggregateOperationOutputTypeDef = TypedDict(
+    "AggregateOperationOutputTypeDef",
+    {
+        "Column": List[str],
+        "AggFunc": AggFunctionType,
+    },
+)
+
 AggregateOperationTypeDef = TypedDict(
     "AggregateOperationTypeDef",
     {
-        "Column": List[str],
+        "Column": Sequence[str],
         "AggFunc": AggFunctionType,
     },
 )
 
+AmazonRedshiftAdvancedOptionOutputTypeDef = TypedDict(
+    "AmazonRedshiftAdvancedOptionOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 AmazonRedshiftAdvancedOptionTypeDef = TypedDict(
     "AmazonRedshiftAdvancedOptionTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+OptionOutputTypeDef = TypedDict(
+    "OptionOutputTypeDef",
+    {
+        "Value": str,
+        "Label": str,
+        "Description": str,
+    },
+)
+
 OptionTypeDef = TypedDict(
     "OptionTypeDef",
     {
         "Value": str,
         "Label": str,
         "Description": str,
     },
     total=False,
 )
 
+ApplyMappingOutputTypeDef = TypedDict(
+    "ApplyMappingOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Mapping": List["MappingOutputTypeDef"],
+    },
+)
+
 ApplyMappingTypeDef = TypedDict(
     "ApplyMappingTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "Mapping": List["MappingTypeDef"],
+        "Inputs": Sequence[str],
+        "Mapping": Sequence["MappingTypeDef"],
     },
 )
 
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
         "RequestedColumns": Sequence[str],
         "AllColumnsRequested": bool,
     },
     total=False,
 )
 
-PartitionValueListTypeDef = TypedDict(
-    "PartitionValueListTypeDef",
+PartitionValueListOutputTypeDef = TypedDict(
+    "PartitionValueListOutputTypeDef",
     {
-        "Values": Sequence[str],
+        "Values": List[str],
+    },
+)
+
+BasicCatalogTargetOutputTypeDef = TypedDict(
+    "BasicCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
     },
 )
 
 BasicCatalogTargetTypeDef = TypedDict(
     "BasicCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
@@ -866,27 +1080,35 @@
     "_OptionalBatchDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteConnectionRequestRequestTypeDef(
     _RequiredBatchDeleteConnectionRequestRequestTypeDef,
     _OptionalBatchDeleteConnectionRequestRequestTypeDef,
 ):
     pass
 
+
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+PartitionValueListTypeDef = TypedDict(
+    "PartitionValueListTypeDef",
+    {
+        "Values": Sequence[str],
+    },
 )
 
 _RequiredBatchDeleteTableRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TablesToDelete": Sequence[str],
@@ -897,19 +1119,21 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteTableRequestRequestTypeDef(
     _RequiredBatchDeleteTableRequestRequestTypeDef, _OptionalBatchDeleteTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredBatchDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionIds": Sequence[str],
     },
@@ -918,20 +1142,22 @@
     "_OptionalBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteTableVersionRequestRequestTypeDef(
     _RequiredBatchDeleteTableVersionRequestRequestTypeDef,
     _OptionalBatchDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetBlueprintsRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 _OptionalBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
@@ -939,52 +1165,45 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
+
 class BatchGetBlueprintsRequestRequestTypeDef(
     _RequiredBatchGetBlueprintsRequestRequestTypeDef,
     _OptionalBatchGetBlueprintsRequestRequestTypeDef,
 ):
     pass
 
+
 BatchGetCrawlersRequestRequestTypeDef = TypedDict(
     "BatchGetCrawlersRequestRequestTypeDef",
     {
         "CrawlerNames": Sequence[str],
     },
 )
 
 BatchGetCustomEntityTypesRequestRequestTypeDef = TypedDict(
     "BatchGetCustomEntityTypesRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 
-_RequiredCustomEntityTypeTypeDef = TypedDict(
-    "_RequiredCustomEntityTypeTypeDef",
+CustomEntityTypeTypeDef = TypedDict(
+    "CustomEntityTypeTypeDef",
     {
         "Name": str,
         "RegexString": str,
-    },
-)
-_OptionalCustomEntityTypeTypeDef = TypedDict(
-    "_OptionalCustomEntityTypeTypeDef",
-    {
         "ContextWords": List[str],
     },
-    total=False,
 )
 
-class CustomEntityTypeTypeDef(_RequiredCustomEntityTypeTypeDef, _OptionalCustomEntityTypeTypeDef):
-    pass
-
 BatchGetDataQualityResultRequestRequestTypeDef = TypedDict(
     "BatchGetDataQualityResultRequestRequestTypeDef",
     {
         "ResultIds": Sequence[str],
     },
 )
 
@@ -1020,15 +1239,14 @@
         "CreatedTimestamp": datetime,
         "LastModifiedTimestamp": datetime,
         "PublicKey": str,
         "PublicKeys": List[str],
         "SecurityConfiguration": str,
         "Arguments": Dict[str, str],
     },
-    total=False,
 )
 
 BatchGetJobsRequestRequestTypeDef = TypedDict(
     "BatchGetJobsRequestRequestTypeDef",
     {
         "JobNames": Sequence[str],
     },
@@ -1051,34 +1269,44 @@
     "_OptionalBatchGetWorkflowsRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
+
 class BatchGetWorkflowsRequestRequestTypeDef(
     _RequiredBatchGetWorkflowsRequestRequestTypeDef, _OptionalBatchGetWorkflowsRequestRequestTypeDef
 ):
     pass
 
+
 BatchStopJobRunRequestRequestTypeDef = TypedDict(
     "BatchStopJobRunRequestRequestTypeDef",
     {
         "JobName": str,
         "JobRunIds": Sequence[str],
     },
 )
 
 BatchStopJobRunSuccessfulSubmissionTypeDef = TypedDict(
     "BatchStopJobRunSuccessfulSubmissionTypeDef",
     {
         "JobName": str,
         "JobRunId": str,
     },
-    total=False,
+)
+
+BinaryColumnStatisticsDataOutputTypeDef = TypedDict(
+    "BinaryColumnStatisticsDataOutputTypeDef",
+    {
+        "MaximumLength": int,
+        "AverageLength": float,
+        "NumberOfNulls": int,
+    },
 )
 
 BinaryColumnStatisticsDataTypeDef = TypedDict(
     "BinaryColumnStatisticsDataTypeDef",
     {
         "MaximumLength": int,
         "AverageLength": float,
@@ -1088,15 +1316,14 @@
 
 BlueprintDetailsTypeDef = TypedDict(
     "BlueprintDetailsTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
     },
-    total=False,
 )
 
 BlueprintRunTypeDef = TypedDict(
     "BlueprintRunTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
@@ -1105,27 +1332,34 @@
         "StartedOn": datetime,
         "CompletedOn": datetime,
         "ErrorMessage": str,
         "RollbackErrorMessage": str,
         "Parameters": str,
         "RoleArn": str,
     },
-    total=False,
 )
 
 LastActiveDefinitionTypeDef = TypedDict(
     "LastActiveDefinitionTypeDef",
     {
         "Description": str,
         "LastModifiedOn": datetime,
         "ParameterSpec": str,
         "BlueprintLocation": str,
         "BlueprintServiceLocation": str,
     },
-    total=False,
+)
+
+BooleanColumnStatisticsDataOutputTypeDef = TypedDict(
+    "BooleanColumnStatisticsDataOutputTypeDef",
+    {
+        "NumberOfTrues": int,
+        "NumberOfFalses": int,
+        "NumberOfNulls": int,
+    },
 )
 
 BooleanColumnStatisticsDataTypeDef = TypedDict(
     "BooleanColumnStatisticsDataTypeDef",
     {
         "NumberOfTrues": int,
         "NumberOfFalses": int,
@@ -1166,19 +1400,21 @@
     "_OptionalCancelStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class CancelStatementRequestRequestTypeDef(
     _RequiredCancelStatementRequestRequestTypeDef, _OptionalCancelStatementRequestRequestTypeDef
 ):
     pass
 
+
 CatalogEntryTypeDef = TypedDict(
     "CatalogEntryTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1186,15 +1422,47 @@
 CatalogImportStatusTypeDef = TypedDict(
     "CatalogImportStatusTypeDef",
     {
         "ImportCompleted": bool,
         "ImportTime": datetime,
         "ImportedBy": str,
     },
-    total=False,
+)
+
+KafkaStreamingSourceOptionsOutputTypeDef = TypedDict(
+    "KafkaStreamingSourceOptionsOutputTypeDef",
+    {
+        "BootstrapServers": str,
+        "SecurityProtocol": str,
+        "ConnectionName": str,
+        "TopicName": str,
+        "Assign": str,
+        "SubscribePattern": str,
+        "Classification": str,
+        "Delimiter": str,
+        "StartingOffsets": str,
+        "EndingOffsets": str,
+        "PollTimeoutMs": int,
+        "NumRetries": int,
+        "RetryIntervalMs": int,
+        "MaxOffsetsPerTrigger": int,
+        "MinPartitions": int,
+        "IncludeHeaders": bool,
+        "AddRecordTimestamp": str,
+        "EmitConsumerLagMetrics": str,
+        "StartingTimestamp": datetime,
+    },
+)
+
+StreamingDataPreviewOptionsOutputTypeDef = TypedDict(
+    "StreamingDataPreviewOptionsOutputTypeDef",
+    {
+        "PollingTime": int,
+        "RecordPollingLimit": int,
+    },
 )
 
 KafkaStreamingSourceOptionsTypeDef = TypedDict(
     "KafkaStreamingSourceOptionsTypeDef",
     {
         "BootstrapServers": str,
         "SecurityProtocol": str,
@@ -1210,28 +1478,55 @@
         "NumRetries": int,
         "RetryIntervalMs": int,
         "MaxOffsetsPerTrigger": int,
         "MinPartitions": int,
         "IncludeHeaders": bool,
         "AddRecordTimestamp": str,
         "EmitConsumerLagMetrics": str,
-        "StartingTimestamp": datetime,
+        "StartingTimestamp": Union[datetime, str],
     },
     total=False,
 )
 
 StreamingDataPreviewOptionsTypeDef = TypedDict(
     "StreamingDataPreviewOptionsTypeDef",
     {
         "PollingTime": int,
         "RecordPollingLimit": int,
     },
     total=False,
 )
 
+KinesisStreamingSourceOptionsOutputTypeDef = TypedDict(
+    "KinesisStreamingSourceOptionsOutputTypeDef",
+    {
+        "EndpointUrl": str,
+        "StreamName": str,
+        "Classification": str,
+        "Delimiter": str,
+        "StartingPosition": StartingPositionType,
+        "MaxFetchTimeInMs": int,
+        "MaxFetchRecordsPerShard": int,
+        "MaxRecordPerRead": int,
+        "AddIdleTimeBetweenReads": bool,
+        "IdleTimeBetweenReadsInMs": int,
+        "DescribeShardInterval": int,
+        "NumRetries": int,
+        "RetryIntervalMs": int,
+        "MaxRetryIntervalMs": int,
+        "AvoidEmptyBatches": bool,
+        "StreamArn": str,
+        "RoleArn": str,
+        "RoleSessionName": str,
+        "AddRecordTimestamp": str,
+        "EmitConsumerLagMetrics": str,
+        "StartingTimestamp": datetime,
+    },
+)
+
 KinesisStreamingSourceOptionsTypeDef = TypedDict(
     "KinesisStreamingSourceOptionsTypeDef",
     {
         "EndpointUrl": str,
         "StreamName": str,
         "Classification": str,
         "Delimiter": str,
@@ -1247,164 +1542,392 @@
         "MaxRetryIntervalMs": int,
         "AvoidEmptyBatches": bool,
         "StreamArn": str,
         "RoleArn": str,
         "RoleSessionName": str,
         "AddRecordTimestamp": str,
         "EmitConsumerLagMetrics": str,
-        "StartingTimestamp": datetime,
+        "StartingTimestamp": Union[datetime, str],
     },
     total=False,
 )
 
+CatalogSchemaChangePolicyOutputTypeDef = TypedDict(
+    "CatalogSchemaChangePolicyOutputTypeDef",
+    {
+        "EnableUpdateCatalog": bool,
+        "UpdateBehavior": UpdateCatalogBehaviorType,
+    },
+)
+
 CatalogSchemaChangePolicyTypeDef = TypedDict(
     "CatalogSchemaChangePolicyTypeDef",
     {
         "EnableUpdateCatalog": bool,
         "UpdateBehavior": UpdateCatalogBehaviorType,
     },
     total=False,
 )
 
+CatalogSourceOutputTypeDef = TypedDict(
+    "CatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+
 CatalogSourceTypeDef = TypedDict(
     "CatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
+CatalogTargetOutputTypeDef = TypedDict(
+    "CatalogTargetOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "Tables": List[str],
+        "ConnectionName": str,
+        "EventQueueArn": str,
+        "DlqEventQueueArn": str,
+    },
+)
+
 _RequiredCatalogTargetTypeDef = TypedDict(
     "_RequiredCatalogTargetTypeDef",
     {
         "DatabaseName": str,
-        "Tables": List[str],
+        "Tables": Sequence[str],
     },
 )
 _OptionalCatalogTargetTypeDef = TypedDict(
     "_OptionalCatalogTargetTypeDef",
     {
         "ConnectionName": str,
         "EventQueueArn": str,
         "DlqEventQueueArn": str,
     },
     total=False,
 )
 
+
 class CatalogTargetTypeDef(_RequiredCatalogTargetTypeDef, _OptionalCatalogTargetTypeDef):
     pass
 
+
 CheckSchemaVersionValidityInputRequestTypeDef = TypedDict(
     "CheckSchemaVersionValidityInputRequestTypeDef",
     {
         "DataFormat": DataFormatType,
         "SchemaDefinition": str,
     },
 )
 
-_RequiredCsvClassifierTypeDef = TypedDict(
-    "_RequiredCsvClassifierTypeDef",
+CsvClassifierTypeDef = TypedDict(
+    "CsvClassifierTypeDef",
     {
         "Name": str,
-    },
-)
-_OptionalCsvClassifierTypeDef = TypedDict(
-    "_OptionalCsvClassifierTypeDef",
-    {
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "Version": int,
         "Delimiter": str,
         "QuoteSymbol": str,
         "ContainsHeader": CsvHeaderOptionType,
         "Header": List[str],
         "DisableValueTrimming": bool,
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": List[str],
     },
-    total=False,
 )
 
-class CsvClassifierTypeDef(_RequiredCsvClassifierTypeDef, _OptionalCsvClassifierTypeDef):
-    pass
-
-_RequiredGrokClassifierTypeDef = TypedDict(
-    "_RequiredGrokClassifierTypeDef",
+GrokClassifierTypeDef = TypedDict(
+    "GrokClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
-        "GrokPattern": str,
-    },
-)
-_OptionalGrokClassifierTypeDef = TypedDict(
-    "_OptionalGrokClassifierTypeDef",
-    {
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "Version": int,
+        "GrokPattern": str,
         "CustomPatterns": str,
     },
-    total=False,
 )
 
-class GrokClassifierTypeDef(_RequiredGrokClassifierTypeDef, _OptionalGrokClassifierTypeDef):
-    pass
-
-_RequiredJsonClassifierTypeDef = TypedDict(
-    "_RequiredJsonClassifierTypeDef",
+JsonClassifierTypeDef = TypedDict(
+    "JsonClassifierTypeDef",
     {
         "Name": str,
-        "JsonPath": str,
-    },
-)
-_OptionalJsonClassifierTypeDef = TypedDict(
-    "_OptionalJsonClassifierTypeDef",
-    {
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "Version": int,
+        "JsonPath": str,
     },
-    total=False,
 )
 
-class JsonClassifierTypeDef(_RequiredJsonClassifierTypeDef, _OptionalJsonClassifierTypeDef):
-    pass
-
-_RequiredXMLClassifierTypeDef = TypedDict(
-    "_RequiredXMLClassifierTypeDef",
+XMLClassifierTypeDef = TypedDict(
+    "XMLClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
-    },
-)
-_OptionalXMLClassifierTypeDef = TypedDict(
-    "_OptionalXMLClassifierTypeDef",
-    {
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "Version": int,
         "RowTag": str,
     },
-    total=False,
 )
 
-class XMLClassifierTypeDef(_RequiredXMLClassifierTypeDef, _OptionalXMLClassifierTypeDef):
-    pass
+CloudWatchEncryptionOutputTypeDef = TypedDict(
+    "CloudWatchEncryptionOutputTypeDef",
+    {
+        "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
+        "KmsKeyArn": str,
+    },
+)
 
 CloudWatchEncryptionTypeDef = TypedDict(
     "CloudWatchEncryptionTypeDef",
     {
         "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+DirectJDBCSourceOutputTypeDef = TypedDict(
+    "DirectJDBCSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "ConnectionName": str,
+        "ConnectionType": JDBCConnectionTypeType,
+        "RedshiftTmpDir": str,
+    },
+)
+
+DropDuplicatesOutputTypeDef = TypedDict(
+    "DropDuplicatesOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Columns": List[List[str]],
+    },
+)
+
+DropFieldsOutputTypeDef = TypedDict(
+    "DropFieldsOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Paths": List[List[str]],
+    },
+)
+
+DynamoDBCatalogSourceOutputTypeDef = TypedDict(
+    "DynamoDBCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+
+FillMissingValuesOutputTypeDef = TypedDict(
+    "FillMissingValuesOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "ImputedPath": str,
+        "FilledPath": str,
+    },
+)
+
+MergeOutputTypeDef = TypedDict(
+    "MergeOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Source": str,
+        "PrimaryKeys": List[List[str]],
+    },
+)
+
+MicrosoftSQLServerCatalogSourceOutputTypeDef = TypedDict(
+    "MicrosoftSQLServerCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+
+MicrosoftSQLServerCatalogTargetOutputTypeDef = TypedDict(
+    "MicrosoftSQLServerCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
+    },
+)
+
+MySQLCatalogSourceOutputTypeDef = TypedDict(
+    "MySQLCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+
+MySQLCatalogTargetOutputTypeDef = TypedDict(
+    "MySQLCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
+    },
+)
+
+OracleSQLCatalogSourceOutputTypeDef = TypedDict(
+    "OracleSQLCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+
+OracleSQLCatalogTargetOutputTypeDef = TypedDict(
+    "OracleSQLCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
+    },
+)
+
+PIIDetectionOutputTypeDef = TypedDict(
+    "PIIDetectionOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PiiType": PiiTypeType,
+        "EntityTypesToDetect": List[str],
+        "OutputColumnName": str,
+        "SampleFraction": float,
+        "ThresholdFraction": float,
+        "MaskValue": str,
+    },
+)
+
+PostgreSQLCatalogSourceOutputTypeDef = TypedDict(
+    "PostgreSQLCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+
+PostgreSQLCatalogTargetOutputTypeDef = TypedDict(
+    "PostgreSQLCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
+    },
+)
+
+RedshiftSourceOutputTypeDef = TypedDict(
+    "RedshiftSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "RedshiftTmpDir": str,
+        "TmpDirIAMRole": str,
+    },
+)
+
+RelationalCatalogSourceOutputTypeDef = TypedDict(
+    "RelationalCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+
+RenameFieldOutputTypeDef = TypedDict(
+    "RenameFieldOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "SourcePath": List[str],
+        "TargetPath": List[str],
+    },
+)
+
+SelectFieldsOutputTypeDef = TypedDict(
+    "SelectFieldsOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Paths": List[List[str]],
+    },
+)
+
+SelectFromCollectionOutputTypeDef = TypedDict(
+    "SelectFromCollectionOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Index": int,
+    },
+)
+
+SpigotOutputTypeDef = TypedDict(
+    "SpigotOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Path": str,
+        "Topk": int,
+        "Prob": float,
+    },
+)
+
+SplitFieldsOutputTypeDef = TypedDict(
+    "SplitFieldsOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Paths": List[List[str]],
+    },
+)
+
+UnionOutputTypeDef = TypedDict(
+    "UnionOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "UnionType": UnionTypeType,
+    },
+)
+
 _RequiredDirectJDBCSourceTypeDef = TypedDict(
     "_RequiredDirectJDBCSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
         "ConnectionName": str,
@@ -1415,41 +1938,45 @@
     "_OptionalDirectJDBCSourceTypeDef",
     {
         "RedshiftTmpDir": str,
     },
     total=False,
 )
 
+
 class DirectJDBCSourceTypeDef(_RequiredDirectJDBCSourceTypeDef, _OptionalDirectJDBCSourceTypeDef):
     pass
 
+
 _RequiredDropDuplicatesTypeDef = TypedDict(
     "_RequiredDropDuplicatesTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
     },
 )
 _OptionalDropDuplicatesTypeDef = TypedDict(
     "_OptionalDropDuplicatesTypeDef",
     {
-        "Columns": List[List[str]],
+        "Columns": Sequence[Sequence[str]],
     },
     total=False,
 )
 
+
 class DropDuplicatesTypeDef(_RequiredDropDuplicatesTypeDef, _OptionalDropDuplicatesTypeDef):
     pass
 
+
 DropFieldsTypeDef = TypedDict(
     "DropFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "Paths": List[List[str]],
+        "Inputs": Sequence[str],
+        "Paths": Sequence[Sequence[str]],
     },
 )
 
 DynamoDBCatalogSourceTypeDef = TypedDict(
     "DynamoDBCatalogSourceTypeDef",
     {
         "Name": str,
@@ -1458,38 +1985,40 @@
     },
 )
 
 _RequiredFillMissingValuesTypeDef = TypedDict(
     "_RequiredFillMissingValuesTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "ImputedPath": str,
     },
 )
 _OptionalFillMissingValuesTypeDef = TypedDict(
     "_OptionalFillMissingValuesTypeDef",
     {
         "FilledPath": str,
     },
     total=False,
 )
 
+
 class FillMissingValuesTypeDef(
     _RequiredFillMissingValuesTypeDef, _OptionalFillMissingValuesTypeDef
 ):
     pass
 
+
 MergeTypeDef = TypedDict(
     "MergeTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Source": str,
-        "PrimaryKeys": List[List[str]],
+        "PrimaryKeys": Sequence[Sequence[str]],
     },
 )
 
 MicrosoftSQLServerCatalogSourceTypeDef = TypedDict(
     "MicrosoftSQLServerCatalogSourceTypeDef",
     {
         "Name": str,
@@ -1498,15 +2027,15 @@
     },
 )
 
 MicrosoftSQLServerCatalogTargetTypeDef = TypedDict(
     "MicrosoftSQLServerCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 
 MySQLCatalogSourceTypeDef = TypedDict(
     "MySQLCatalogSourceTypeDef",
@@ -1517,15 +2046,15 @@
     },
 )
 
 MySQLCatalogTargetTypeDef = TypedDict(
     "MySQLCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 
 OracleSQLCatalogSourceTypeDef = TypedDict(
     "OracleSQLCatalogSourceTypeDef",
@@ -1536,57 +2065,59 @@
     },
 )
 
 OracleSQLCatalogTargetTypeDef = TypedDict(
     "OracleSQLCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 
 _RequiredPIIDetectionTypeDef = TypedDict(
     "_RequiredPIIDetectionTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "PiiType": PiiTypeType,
-        "EntityTypesToDetect": List[str],
+        "EntityTypesToDetect": Sequence[str],
     },
 )
 _OptionalPIIDetectionTypeDef = TypedDict(
     "_OptionalPIIDetectionTypeDef",
     {
         "OutputColumnName": str,
         "SampleFraction": float,
         "ThresholdFraction": float,
         "MaskValue": str,
     },
     total=False,
 )
 
+
 class PIIDetectionTypeDef(_RequiredPIIDetectionTypeDef, _OptionalPIIDetectionTypeDef):
     pass
 
+
 PostgreSQLCatalogSourceTypeDef = TypedDict(
     "PostgreSQLCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
 PostgreSQLCatalogTargetTypeDef = TypedDict(
     "PostgreSQLCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 
 _RequiredRedshiftSourceTypeDef = TypedDict(
     "_RequiredRedshiftSourceTypeDef",
@@ -1601,92 +2132,105 @@
     {
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
     },
     total=False,
 )
 
+
 class RedshiftSourceTypeDef(_RequiredRedshiftSourceTypeDef, _OptionalRedshiftSourceTypeDef):
     pass
 
+
 RelationalCatalogSourceTypeDef = TypedDict(
     "RelationalCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 
 RenameFieldTypeDef = TypedDict(
     "RenameFieldTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "SourcePath": List[str],
-        "TargetPath": List[str],
+        "Inputs": Sequence[str],
+        "SourcePath": Sequence[str],
+        "TargetPath": Sequence[str],
     },
 )
 
 SelectFieldsTypeDef = TypedDict(
     "SelectFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "Paths": List[List[str]],
+        "Inputs": Sequence[str],
+        "Paths": Sequence[Sequence[str]],
     },
 )
 
 SelectFromCollectionTypeDef = TypedDict(
     "SelectFromCollectionTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Index": int,
     },
 )
 
 _RequiredSpigotTypeDef = TypedDict(
     "_RequiredSpigotTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Path": str,
     },
 )
 _OptionalSpigotTypeDef = TypedDict(
     "_OptionalSpigotTypeDef",
     {
         "Topk": int,
         "Prob": float,
     },
     total=False,
 )
 
+
 class SpigotTypeDef(_RequiredSpigotTypeDef, _OptionalSpigotTypeDef):
     pass
 
+
 SplitFieldsTypeDef = TypedDict(
     "SplitFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
-        "Paths": List[List[str]],
+        "Inputs": Sequence[str],
+        "Paths": Sequence[Sequence[str]],
     },
 )
 
 UnionTypeDef = TypedDict(
     "UnionTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "UnionType": UnionTypeType,
     },
 )
 
+CodeGenEdgeOutputTypeDef = TypedDict(
+    "CodeGenEdgeOutputTypeDef",
+    {
+        "Source": str,
+        "Target": str,
+        "TargetParameter": str,
+    },
+)
+
 _RequiredCodeGenEdgeTypeDef = TypedDict(
     "_RequiredCodeGenEdgeTypeDef",
     {
         "Source": str,
         "Target": str,
     },
 )
@@ -1694,17 +2238,28 @@
     "_OptionalCodeGenEdgeTypeDef",
     {
         "TargetParameter": str,
     },
     total=False,
 )
 
+
 class CodeGenEdgeTypeDef(_RequiredCodeGenEdgeTypeDef, _OptionalCodeGenEdgeTypeDef):
     pass
 
+
+CodeGenNodeArgOutputTypeDef = TypedDict(
+    "CodeGenNodeArgOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+        "Param": bool,
+    },
+)
+
 _RequiredCodeGenNodeArgTypeDef = TypedDict(
     "_RequiredCodeGenNodeArgTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1712,56 +2267,108 @@
     "_OptionalCodeGenNodeArgTypeDef",
     {
         "Param": bool,
     },
     total=False,
 )
 
+
 class CodeGenNodeArgTypeDef(_RequiredCodeGenNodeArgTypeDef, _OptionalCodeGenNodeArgTypeDef):
     pass
 
+
 ColumnImportanceTypeDef = TypedDict(
     "ColumnImportanceTypeDef",
     {
         "ColumnName": str,
         "Importance": float,
     },
-    total=False,
+)
+
+ColumnOutputTypeDef = TypedDict(
+    "ColumnOutputTypeDef",
+    {
+        "Name": str,
+        "Type": str,
+        "Comment": str,
+        "Parameters": Dict[str, str],
+    },
 )
 
 ColumnRowFilterTypeDef = TypedDict(
     "ColumnRowFilterTypeDef",
     {
         "ColumnName": str,
         "RowFilterExpression": str,
     },
-    total=False,
+)
+
+DateColumnStatisticsDataOutputTypeDef = TypedDict(
+    "DateColumnStatisticsDataOutputTypeDef",
+    {
+        "MinimumValue": datetime,
+        "MaximumValue": datetime,
+        "NumberOfNulls": int,
+        "NumberOfDistinctValues": int,
+    },
+)
+
+DoubleColumnStatisticsDataOutputTypeDef = TypedDict(
+    "DoubleColumnStatisticsDataOutputTypeDef",
+    {
+        "MinimumValue": float,
+        "MaximumValue": float,
+        "NumberOfNulls": int,
+        "NumberOfDistinctValues": int,
+    },
+)
+
+LongColumnStatisticsDataOutputTypeDef = TypedDict(
+    "LongColumnStatisticsDataOutputTypeDef",
+    {
+        "MinimumValue": int,
+        "MaximumValue": int,
+        "NumberOfNulls": int,
+        "NumberOfDistinctValues": int,
+    },
+)
+
+StringColumnStatisticsDataOutputTypeDef = TypedDict(
+    "StringColumnStatisticsDataOutputTypeDef",
+    {
+        "MaximumLength": int,
+        "AverageLength": float,
+        "NumberOfNulls": int,
+        "NumberOfDistinctValues": int,
+    },
 )
 
 _RequiredDateColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDateColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
 _OptionalDateColumnStatisticsDataTypeDef = TypedDict(
     "_OptionalDateColumnStatisticsDataTypeDef",
     {
-        "MinimumValue": datetime,
-        "MaximumValue": datetime,
+        "MinimumValue": Union[datetime, str],
+        "MaximumValue": Union[datetime, str],
     },
     total=False,
 )
 
+
 class DateColumnStatisticsDataTypeDef(
     _RequiredDateColumnStatisticsDataTypeDef, _OptionalDateColumnStatisticsDataTypeDef
 ):
     pass
 
+
 _RequiredDoubleColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDoubleColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1770,19 +2377,21 @@
     {
         "MinimumValue": float,
         "MaximumValue": float,
     },
     total=False,
 )
 
+
 class DoubleColumnStatisticsDataTypeDef(
     _RequiredDoubleColumnStatisticsDataTypeDef, _OptionalDoubleColumnStatisticsDataTypeDef
 ):
     pass
 
+
 _RequiredLongColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredLongColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1791,19 +2400,21 @@
     {
         "MinimumValue": int,
         "MaximumValue": int,
     },
     total=False,
 )
 
+
 class LongColumnStatisticsDataTypeDef(
     _RequiredLongColumnStatisticsDataTypeDef, _OptionalLongColumnStatisticsDataTypeDef
 ):
     pass
 
+
 StringColumnStatisticsDataTypeDef = TypedDict(
     "StringColumnStatisticsDataTypeDef",
     {
         "MaximumLength": int,
         "AverageLength": float,
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
@@ -1822,17 +2433,30 @@
         "Type": str,
         "Comment": str,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ColumnTypeDef(_RequiredColumnTypeDef, _OptionalColumnTypeDef):
     pass
 
+
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "LogicalOperator": Literal["EQUALS"],
+        "JobName": str,
+        "State": JobRunStateType,
+        "CrawlerName": str,
+        "CrawlState": CrawlStateType,
+    },
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "LogicalOperator": Literal["EQUALS"],
         "JobName": str,
         "State": JobRunStateType,
         "CrawlerName": str,
@@ -1845,65 +2469,89 @@
     "ConfusionMatrixTypeDef",
     {
         "NumTruePositives": int,
         "NumFalsePositives": int,
         "NumTrueNegatives": int,
         "NumFalseNegatives": int,
     },
-    total=False,
 )
 
 PhysicalConnectionRequirementsTypeDef = TypedDict(
     "PhysicalConnectionRequirementsTypeDef",
     {
         "SubnetId": str,
         "SecurityGroupIdList": Sequence[str],
         "AvailabilityZone": str,
     },
     total=False,
 )
 
+ConnectionPasswordEncryptionOutputTypeDef = TypedDict(
+    "ConnectionPasswordEncryptionOutputTypeDef",
+    {
+        "ReturnConnectionPasswordEncrypted": bool,
+        "AwsKmsKeyId": str,
+    },
+)
+
 _RequiredConnectionPasswordEncryptionTypeDef = TypedDict(
     "_RequiredConnectionPasswordEncryptionTypeDef",
     {
         "ReturnConnectionPasswordEncrypted": bool,
     },
 )
 _OptionalConnectionPasswordEncryptionTypeDef = TypedDict(
     "_OptionalConnectionPasswordEncryptionTypeDef",
     {
         "AwsKmsKeyId": str,
     },
     total=False,
 )
 
+
 class ConnectionPasswordEncryptionTypeDef(
     _RequiredConnectionPasswordEncryptionTypeDef, _OptionalConnectionPasswordEncryptionTypeDef
 ):
     pass
 
+
+PhysicalConnectionRequirementsOutputTypeDef = TypedDict(
+    "PhysicalConnectionRequirementsOutputTypeDef",
+    {
+        "SubnetId": str,
+        "SecurityGroupIdList": List[str],
+        "AvailabilityZone": str,
+    },
+)
+
+ConnectionsListOutputTypeDef = TypedDict(
+    "ConnectionsListOutputTypeDef",
+    {
+        "Connections": List[str],
+    },
+)
+
 ConnectionsListTypeDef = TypedDict(
     "ConnectionsListTypeDef",
     {
-        "Connections": List[str],
+        "Connections": Sequence[str],
     },
     total=False,
 )
 
 CrawlTypeDef = TypedDict(
     "CrawlTypeDef",
     {
         "State": CrawlStateType,
         "StartedOn": datetime,
         "CompletedOn": datetime,
         "ErrorMessage": str,
         "LogGroup": str,
         "LogStream": str,
     },
-    total=False,
 )
 
 CrawlerHistoryTypeDef = TypedDict(
     "CrawlerHistoryTypeDef",
     {
         "CrawlId": str,
         "State": CrawlerHistoryStateType,
@@ -1912,36 +2560,94 @@
         "Summary": str,
         "ErrorMessage": str,
         "LogGroup": str,
         "LogStream": str,
         "MessagePrefix": str,
         "DPUHour": float,
     },
-    total=False,
 )
 
 CrawlerMetricsTypeDef = TypedDict(
     "CrawlerMetricsTypeDef",
     {
         "CrawlerName": str,
         "TimeLeftSeconds": float,
         "StillEstimating": bool,
         "LastRuntimeSeconds": float,
         "MedianRuntimeSeconds": float,
         "TablesCreated": int,
         "TablesUpdated": int,
         "TablesDeleted": int,
     },
-    total=False,
+)
+
+DeltaTargetOutputTypeDef = TypedDict(
+    "DeltaTargetOutputTypeDef",
+    {
+        "DeltaTables": List[str],
+        "ConnectionName": str,
+        "WriteManifest": bool,
+        "CreateNativeDeltaTable": bool,
+    },
+)
+
+DynamoDBTargetOutputTypeDef = TypedDict(
+    "DynamoDBTargetOutputTypeDef",
+    {
+        "Path": str,
+        "scanAll": bool,
+        "scanRate": float,
+    },
+)
+
+IcebergTargetOutputTypeDef = TypedDict(
+    "IcebergTargetOutputTypeDef",
+    {
+        "Paths": List[str],
+        "ConnectionName": str,
+        "Exclusions": List[str],
+        "MaximumTraversalDepth": int,
+    },
+)
+
+JdbcTargetOutputTypeDef = TypedDict(
+    "JdbcTargetOutputTypeDef",
+    {
+        "ConnectionName": str,
+        "Path": str,
+        "Exclusions": List[str],
+        "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
+    },
+)
+
+MongoDBTargetOutputTypeDef = TypedDict(
+    "MongoDBTargetOutputTypeDef",
+    {
+        "ConnectionName": str,
+        "Path": str,
+        "ScanAll": bool,
+    },
+)
+
+S3TargetOutputTypeDef = TypedDict(
+    "S3TargetOutputTypeDef",
+    {
+        "Path": str,
+        "Exclusions": List[str],
+        "ConnectionName": str,
+        "SampleSize": int,
+        "EventQueueArn": str,
+        "DlqEventQueueArn": str,
+    },
 )
 
 DeltaTargetTypeDef = TypedDict(
     "DeltaTargetTypeDef",
     {
-        "DeltaTables": List[str],
+        "DeltaTables": Sequence[str],
         "ConnectionName": str,
         "WriteManifest": bool,
         "CreateNativeDeltaTable": bool,
     },
     total=False,
 )
 
@@ -1954,29 +2660,29 @@
     },
     total=False,
 )
 
 IcebergTargetTypeDef = TypedDict(
     "IcebergTargetTypeDef",
     {
-        "Paths": List[str],
+        "Paths": Sequence[str],
         "ConnectionName": str,
-        "Exclusions": List[str],
+        "Exclusions": Sequence[str],
         "MaximumTraversalDepth": int,
     },
     total=False,
 )
 
 JdbcTargetTypeDef = TypedDict(
     "JdbcTargetTypeDef",
     {
         "ConnectionName": str,
         "Path": str,
-        "Exclusions": List[str],
-        "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
+        "Exclusions": Sequence[str],
+        "EnableAdditionalMetadata": Sequence[JdbcMetadataEntryType],
     },
     total=False,
 )
 
 MongoDBTargetTypeDef = TypedDict(
     "MongoDBTargetTypeDef",
     {
@@ -1987,77 +2693,71 @@
     total=False,
 )
 
 S3TargetTypeDef = TypedDict(
     "S3TargetTypeDef",
     {
         "Path": str,
-        "Exclusions": List[str],
+        "Exclusions": Sequence[str],
         "ConnectionName": str,
         "SampleSize": int,
         "EventQueueArn": str,
         "DlqEventQueueArn": str,
     },
     total=False,
 )
 
-LakeFormationConfigurationTypeDef = TypedDict(
-    "LakeFormationConfigurationTypeDef",
+LakeFormationConfigurationOutputTypeDef = TypedDict(
+    "LakeFormationConfigurationOutputTypeDef",
     {
         "UseLakeFormationCredentials": bool,
         "AccountId": str,
     },
-    total=False,
 )
 
 LastCrawlInfoTypeDef = TypedDict(
     "LastCrawlInfoTypeDef",
     {
         "Status": LastCrawlStatusType,
         "ErrorMessage": str,
         "LogGroup": str,
         "LogStream": str,
         "MessagePrefix": str,
         "StartTime": datetime,
     },
-    total=False,
 )
 
-LineageConfigurationTypeDef = TypedDict(
-    "LineageConfigurationTypeDef",
+LineageConfigurationOutputTypeDef = TypedDict(
+    "LineageConfigurationOutputTypeDef",
     {
         "CrawlerLineageSettings": CrawlerLineageSettingsType,
     },
-    total=False,
 )
 
-RecrawlPolicyTypeDef = TypedDict(
-    "RecrawlPolicyTypeDef",
+RecrawlPolicyOutputTypeDef = TypedDict(
+    "RecrawlPolicyOutputTypeDef",
     {
         "RecrawlBehavior": RecrawlBehaviorType,
     },
-    total=False,
 )
 
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
         "ScheduleExpression": str,
         "State": ScheduleStateType,
     },
-    total=False,
 )
 
-SchemaChangePolicyTypeDef = TypedDict(
-    "SchemaChangePolicyTypeDef",
+SchemaChangePolicyOutputTypeDef = TypedDict(
+    "SchemaChangePolicyOutputTypeDef",
     {
         "UpdateBehavior": UpdateBehaviorType,
         "DeleteBehavior": DeleteBehaviorType,
     },
-    total=False,
 )
 
 CrawlsFilterTypeDef = TypedDict(
     "CrawlsFilterTypeDef",
     {
         "FieldName": FieldNameType,
         "FilterOperator": FilterOperatorType,
@@ -2078,19 +2778,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateBlueprintRequestRequestTypeDef(
     _RequiredCreateBlueprintRequestRequestTypeDef, _OptionalCreateBlueprintRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateCsvClassifierRequestTypeDef = TypedDict(
@@ -2104,19 +2806,21 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateCsvClassifierRequestTypeDef(
     _RequiredCreateCsvClassifierRequestTypeDef, _OptionalCreateCsvClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateGrokClassifierRequestTypeDef",
     {
         "Classification": str,
         "Name": str,
         "GrokPattern": str,
     },
@@ -2125,19 +2829,21 @@
     "_OptionalCreateGrokClassifierRequestTypeDef",
     {
         "CustomPatterns": str,
     },
     total=False,
 )
 
+
 class CreateGrokClassifierRequestTypeDef(
     _RequiredCreateGrokClassifierRequestTypeDef, _OptionalCreateGrokClassifierRequestTypeDef
 ):
     pass
 
+
 CreateJsonClassifierRequestTypeDef = TypedDict(
     "CreateJsonClassifierRequestTypeDef",
     {
         "Name": str,
         "JsonPath": str,
     },
 )
@@ -2153,19 +2859,55 @@
     "_OptionalCreateXMLClassifierRequestTypeDef",
     {
         "RowTag": str,
     },
     total=False,
 )
 
+
 class CreateXMLClassifierRequestTypeDef(
     _RequiredCreateXMLClassifierRequestTypeDef, _OptionalCreateXMLClassifierRequestTypeDef
 ):
     pass
 
+
+LakeFormationConfigurationTypeDef = TypedDict(
+    "LakeFormationConfigurationTypeDef",
+    {
+        "UseLakeFormationCredentials": bool,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+LineageConfigurationTypeDef = TypedDict(
+    "LineageConfigurationTypeDef",
+    {
+        "CrawlerLineageSettings": CrawlerLineageSettingsType,
+    },
+    total=False,
+)
+
+RecrawlPolicyTypeDef = TypedDict(
+    "RecrawlPolicyTypeDef",
+    {
+        "RecrawlBehavior": RecrawlBehaviorType,
+    },
+    total=False,
+)
+
+SchemaChangePolicyTypeDef = TypedDict(
+    "SchemaChangePolicyTypeDef",
+    {
+        "UpdateBehavior": UpdateBehaviorType,
+        "DeleteBehavior": DeleteBehaviorType,
+    },
+    total=False,
+)
+
 _RequiredCreateCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
         "RegexString": str,
     },
 )
@@ -2174,20 +2916,22 @@
     {
         "ContextWords": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateCustomEntityTypeRequestRequestTypeDef(
     _RequiredCreateCustomEntityTypeRequestRequestTypeDef,
     _OptionalCreateCustomEntityTypeRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDataQualityTargetTableTypeDef = TypedDict(
     "_RequiredDataQualityTargetTableTypeDef",
     {
         "TableName": str,
         "DatabaseName": str,
     },
 )
@@ -2195,19 +2939,21 @@
     "_OptionalDataQualityTargetTableTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DataQualityTargetTableTypeDef(
     _RequiredDataQualityTargetTableTypeDef, _OptionalDataQualityTargetTableTypeDef
 ):
     pass
 
+
 _RequiredCreateDevEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
         "RoleArn": str,
     },
 )
@@ -2227,19 +2973,21 @@
         "SecurityConfiguration": str,
         "Tags": Mapping[str, str],
         "Arguments": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDevEndpointRequestRequestTypeDef(
     _RequiredCreateDevEndpointRequestRequestTypeDef, _OptionalCreateDevEndpointRequestRequestTypeDef
 ):
     pass
 
+
 ExecutionPropertyTypeDef = TypedDict(
     "ExecutionPropertyTypeDef",
     {
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
@@ -2278,22 +3026,24 @@
     },
 )
 _OptionalGlueTableTypeDef = TypedDict(
     "_OptionalGlueTableTypeDef",
     {
         "CatalogId": str,
         "ConnectionName": str,
-        "AdditionalOptions": Dict[str, str],
+        "AdditionalOptions": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
     pass
 
+
 PartitionIndexTypeDef = TypedDict(
     "PartitionIndexTypeDef",
     {
         "Keys": Sequence[str],
         "IndexName": str,
     },
 )
@@ -2309,19 +3059,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateRegistryInputRequestTypeDef(
     _RequiredCreateRegistryInputRequestTypeDef, _OptionalCreateRegistryInputRequestTypeDef
 ):
     pass
 
+
 RegistryIdTypeDef = TypedDict(
     "RegistryIdTypeDef",
     {
         "RegistryName": str,
         "RegistryArn": str,
     },
     total=False,
@@ -2346,19 +3098,21 @@
     "_OptionalEventBatchingConditionTypeDef",
     {
         "BatchWindow": int,
     },
     total=False,
 )
 
+
 class EventBatchingConditionTypeDef(
     _RequiredEventBatchingConditionTypeDef, _OptionalEventBatchingConditionTypeDef
 ):
     pass
 
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2368,63 +3122,107 @@
         "DefaultRunProperties": Mapping[str, str],
         "Tags": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
+
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
+
+DQResultsPublishingOptionsOutputTypeDef = TypedDict(
+    "DQResultsPublishingOptionsOutputTypeDef",
+    {
+        "EvaluationContext": str,
+        "ResultsS3Prefix": str,
+        "CloudWatchMetricsEnabled": bool,
+        "ResultsPublishingEnabled": bool,
+    },
+)
+
 DQResultsPublishingOptionsTypeDef = TypedDict(
     "DQResultsPublishingOptionsTypeDef",
     {
         "EvaluationContext": str,
         "ResultsS3Prefix": str,
         "CloudWatchMetricsEnabled": bool,
         "ResultsPublishingEnabled": bool,
     },
     total=False,
 )
 
+DQStopJobOnFailureOptionsOutputTypeDef = TypedDict(
+    "DQStopJobOnFailureOptionsOutputTypeDef",
+    {
+        "StopJobOnFailureTiming": DQStopJobOnFailureTimingType,
+    },
+)
+
 DQStopJobOnFailureOptionsTypeDef = TypedDict(
     "DQStopJobOnFailureOptionsTypeDef",
     {
         "StopJobOnFailureTiming": DQStopJobOnFailureTimingType,
     },
     total=False,
 )
 
+EncryptionAtRestOutputTypeDef = TypedDict(
+    "EncryptionAtRestOutputTypeDef",
+    {
+        "CatalogEncryptionMode": CatalogEncryptionModeType,
+        "SseAwsKmsKeyId": str,
+    },
+)
+
 _RequiredEncryptionAtRestTypeDef = TypedDict(
     "_RequiredEncryptionAtRestTypeDef",
     {
         "CatalogEncryptionMode": CatalogEncryptionModeType,
     },
 )
 _OptionalEncryptionAtRestTypeDef = TypedDict(
     "_OptionalEncryptionAtRestTypeDef",
     {
         "SseAwsKmsKeyId": str,
     },
     total=False,
 )
 
+
 class EncryptionAtRestTypeDef(_RequiredEncryptionAtRestTypeDef, _OptionalEncryptionAtRestTypeDef):
     pass
 
+
+DataLakePrincipalOutputTypeDef = TypedDict(
+    "DataLakePrincipalOutputTypeDef",
+    {
+        "DataLakePrincipalIdentifier": str,
+    },
+)
+
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
     total=False,
 )
 
+DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef = TypedDict(
+    "DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef",
+    {
+        "CloudWatchMetricsEnabled": bool,
+        "ResultsS3Prefix": str,
+    },
+)
+
 DataQualityEvaluationRunAdditionalRunOptionsTypeDef = TypedDict(
     "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
     {
         "CloudWatchMetricsEnabled": bool,
         "ResultsS3Prefix": str,
     },
     total=False,
@@ -2435,15 +3233,43 @@
     {
         "Name": str,
         "Description": str,
         "EvaluationMessage": str,
         "Result": DataQualityRuleResultStatusType,
         "EvaluatedMetrics": Dict[str, float],
     },
-    total=False,
+)
+
+DataQualityTargetTableOutputTypeDef = TypedDict(
+    "DataQualityTargetTableOutputTypeDef",
+    {
+        "TableName": str,
+        "DatabaseName": str,
+        "CatalogId": str,
+    },
+)
+
+GlueTableOutputTypeDef = TypedDict(
+    "GlueTableOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "CatalogId": str,
+        "ConnectionName": str,
+        "AdditionalOptions": Dict[str, str],
+    },
+)
+
+DatabaseIdentifierOutputTypeDef = TypedDict(
+    "DatabaseIdentifierOutputTypeDef",
+    {
+        "CatalogId": str,
+        "DatabaseName": str,
+        "Region": str,
+    },
 )
 
 DatabaseIdentifierTypeDef = TypedDict(
     "DatabaseIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
@@ -2457,26 +3283,50 @@
     {
         "Identifier": str,
         "ConnectionName": str,
     },
     total=False,
 )
 
+FederatedDatabaseOutputTypeDef = TypedDict(
+    "FederatedDatabaseOutputTypeDef",
+    {
+        "Identifier": str,
+        "ConnectionName": str,
+    },
+)
+
+DatatypeOutputTypeDef = TypedDict(
+    "DatatypeOutputTypeDef",
+    {
+        "Id": str,
+        "Label": str,
+    },
+)
+
 DatatypeTypeDef = TypedDict(
     "DatatypeTypeDef",
     {
         "Id": str,
         "Label": str,
     },
 )
 
+DecimalNumberOutputTypeDef = TypedDict(
+    "DecimalNumberOutputTypeDef",
+    {
+        "UnscaledValue": bytes,
+        "Scale": int,
+    },
+)
+
 DecimalNumberTypeDef = TypedDict(
     "DecimalNumberTypeDef",
     {
-        "UnscaledValue": bytes,
+        "UnscaledValue": Union[str, bytes, IO[Any], StreamingBody],
         "Scale": int,
     },
 )
 
 DeleteBlueprintRequestRequestTypeDef = TypedDict(
     "DeleteBlueprintRequestRequestTypeDef",
     {
@@ -2504,20 +3354,22 @@
     "_OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnName": str,
     },
@@ -2526,39 +3378,43 @@
     "_OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionName": str,
     },
 )
 _OptionalDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteConnectionRequestRequestTypeDef(
     _RequiredDeleteConnectionRequestRequestTypeDef, _OptionalDeleteConnectionRequestRequestTypeDef
 ):
     pass
 
+
 DeleteCrawlerRequestRequestTypeDef = TypedDict(
     "DeleteCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2586,19 +3442,21 @@
     "_OptionalDeleteDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteDatabaseRequestRequestTypeDef(
     _RequiredDeleteDatabaseRequestRequestTypeDef, _OptionalDeleteDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 DeleteDevEndpointRequestRequestTypeDef = TypedDict(
     "DeleteDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 
@@ -2628,20 +3486,22 @@
     "_OptionalDeletePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeletePartitionIndexRequestRequestTypeDef(
     _RequiredDeletePartitionIndexRequestRequestTypeDef,
     _OptionalDeletePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeletePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -2650,19 +3510,21 @@
     "_OptionalDeletePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeletePartitionRequestRequestTypeDef(
     _RequiredDeletePartitionRequestRequestTypeDef, _OptionalDeletePartitionRequestRequestTypeDef
 ):
     pass
 
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyHashCondition": str,
         "ResourceArn": str,
     },
     total=False,
@@ -2695,19 +3557,21 @@
     "_OptionalDeleteSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class DeleteSessionRequestRequestTypeDef(
     _RequiredDeleteSessionRequestRequestTypeDef, _OptionalDeleteSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -2716,19 +3580,21 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
+
 class DeleteTableRequestRequestTypeDef(
     _RequiredDeleteTableRequestRequestTypeDef, _OptionalDeleteTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionId": str,
     },
@@ -2737,20 +3603,22 @@
     "_OptionalDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteTableVersionRequestRequestTypeDef(
     _RequiredDeleteTableVersionRequestRequestTypeDef,
     _OptionalDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteTriggerRequestRequestTypeDef = TypedDict(
     "DeleteTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2765,20 +3633,22 @@
     "_OptionalDeleteUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteUserDefinedFunctionRequestRequestTypeDef(
     _RequiredDeleteUserDefinedFunctionRequestRequestTypeDef,
     _OptionalDeleteUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2787,66 +3657,115 @@
     {
         "ExtraPythonLibsS3Path": str,
         "ExtraJarsS3Path": str,
     },
     total=False,
 )
 
+DirectSchemaChangePolicyOutputTypeDef = TypedDict(
+    "DirectSchemaChangePolicyOutputTypeDef",
+    {
+        "EnableUpdateCatalog": bool,
+        "UpdateBehavior": UpdateCatalogBehaviorType,
+        "Table": str,
+        "Database": str,
+    },
+)
+
 DirectSchemaChangePolicyTypeDef = TypedDict(
     "DirectSchemaChangePolicyTypeDef",
     {
         "EnableUpdateCatalog": bool,
         "UpdateBehavior": UpdateCatalogBehaviorType,
         "Table": str,
         "Database": str,
     },
     total=False,
 )
 
+NullCheckBoxListOutputTypeDef = TypedDict(
+    "NullCheckBoxListOutputTypeDef",
+    {
+        "IsEmpty": bool,
+        "IsNullString": bool,
+        "IsNegOne": bool,
+    },
+)
+
 NullCheckBoxListTypeDef = TypedDict(
     "NullCheckBoxListTypeDef",
     {
         "IsEmpty": bool,
         "IsNullString": bool,
         "IsNegOne": bool,
     },
     total=False,
 )
 
+TransformConfigParameterOutputTypeDef = TypedDict(
+    "TransformConfigParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Type": ParamTypeType,
+        "ValidationRule": str,
+        "ValidationMessage": str,
+        "Value": List[str],
+        "ListType": ParamTypeType,
+        "IsOptional": bool,
+    },
+)
+
 _RequiredTransformConfigParameterTypeDef = TypedDict(
     "_RequiredTransformConfigParameterTypeDef",
     {
         "Name": str,
         "Type": ParamTypeType,
     },
 )
 _OptionalTransformConfigParameterTypeDef = TypedDict(
     "_OptionalTransformConfigParameterTypeDef",
     {
         "ValidationRule": str,
         "ValidationMessage": str,
-        "Value": List[str],
+        "Value": Sequence[str],
         "ListType": ParamTypeType,
         "IsOptional": bool,
     },
     total=False,
 )
 
+
 class TransformConfigParameterTypeDef(
     _RequiredTransformConfigParameterTypeDef, _OptionalTransformConfigParameterTypeDef
 ):
     pass
 
+
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "SourceId": str,
         "DestinationId": str,
     },
-    total=False,
+)
+
+JobBookmarksEncryptionOutputTypeDef = TypedDict(
+    "JobBookmarksEncryptionOutputTypeDef",
+    {
+        "JobBookmarksEncryptionMode": JobBookmarksEncryptionModeType,
+        "KmsKeyArn": str,
+    },
+)
+
+S3EncryptionOutputTypeDef = TypedDict(
+    "S3EncryptionOutputTypeDef",
+    {
+        "S3EncryptionMode": S3EncryptionModeType,
+        "KmsKeyArn": str,
+    },
 )
 
 JobBookmarksEncryptionTypeDef = TypedDict(
     "JobBookmarksEncryptionTypeDef",
     {
         "JobBookmarksEncryptionMode": JobBookmarksEncryptionModeType,
         "KmsKeyArn": str,
@@ -2865,40 +3784,70 @@
 
 ErrorDetailsTypeDef = TypedDict(
     "ErrorDetailsTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+EventBatchingConditionOutputTypeDef = TypedDict(
+    "EventBatchingConditionOutputTypeDef",
+    {
+        "BatchSize": int,
+        "BatchWindow": int,
+    },
+)
+
+ExecutionPropertyOutputTypeDef = TypedDict(
+    "ExecutionPropertyOutputTypeDef",
+    {
+        "MaxConcurrentRuns": int,
+    },
 )
 
 ExportLabelsTaskRunPropertiesTypeDef = TypedDict(
     "ExportLabelsTaskRunPropertiesTypeDef",
     {
         "OutputS3Path": str,
     },
-    total=False,
 )
 
 FederatedTableTypeDef = TypedDict(
     "FederatedTableTypeDef",
     {
         "Identifier": str,
         "DatabaseIdentifier": str,
         "ConnectionName": str,
     },
-    total=False,
+)
+
+FilterValueOutputTypeDef = TypedDict(
+    "FilterValueOutputTypeDef",
+    {
+        "Type": FilterValueTypeType,
+        "Value": List[str],
+    },
 )
 
 FilterValueTypeDef = TypedDict(
     "FilterValueTypeDef",
     {
         "Type": FilterValueTypeType,
-        "Value": List[str],
+        "Value": Sequence[str],
+    },
+)
+
+FindMatchesParametersOutputTypeDef = TypedDict(
+    "FindMatchesParametersOutputTypeDef",
+    {
+        "PrimaryKeyColumnName": str,
+        "PrecisionRecallTradeoff": float,
+        "AccuracyCostTradeoff": float,
+        "EnforceProvidedLabels": bool,
     },
 )
 
 FindMatchesParametersTypeDef = TypedDict(
     "FindMatchesParametersTypeDef",
     {
         "PrimaryKeyColumnName": str,
@@ -2912,15 +3861,14 @@
 FindMatchesTaskRunPropertiesTypeDef = TypedDict(
     "FindMatchesTaskRunPropertiesTypeDef",
     {
         "JobId": str,
         "JobName": str,
         "JobRunId": str,
     },
-    total=False,
 )
 
 _RequiredGetBlueprintRequestRequestTypeDef = TypedDict(
     "_RequiredGetBlueprintRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -2930,19 +3878,21 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
+
 class GetBlueprintRequestRequestTypeDef(
     _RequiredGetBlueprintRequestRequestTypeDef, _OptionalGetBlueprintRequestRequestTypeDef
 ):
     pass
 
+
 GetBlueprintRunRequestRequestTypeDef = TypedDict(
     "GetBlueprintRunRequestRequestTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
     },
 )
@@ -2958,19 +3908,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetBlueprintRunsRequestRequestTypeDef(
     _RequiredGetBlueprintRunsRequestRequestTypeDef, _OptionalGetBlueprintRunsRequestRequestTypeDef
 ):
     pass
 
+
 GetCatalogImportStatusRequestRequestTypeDef = TypedDict(
     "GetCatalogImportStatusRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
@@ -3014,20 +3966,22 @@
     "_OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnNames": Sequence[str],
     },
@@ -3036,20 +3990,22 @@
     "_OptionalGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetConnectionRequestRequestTypeDef = TypedDict(
@@ -3057,19 +4013,21 @@
     {
         "CatalogId": str,
         "HidePassword": bool,
     },
     total=False,
 )
 
+
 class GetConnectionRequestRequestTypeDef(
     _RequiredGetConnectionRequestRequestTypeDef, _OptionalGetConnectionRequestRequestTypeDef
 ):
     pass
 
+
 GetConnectionsFilterTypeDef = TypedDict(
     "GetConnectionsFilterTypeDef",
     {
         "MatchCriteria": Sequence[str],
         "ConnectionType": ConnectionTypeType,
     },
     total=False,
@@ -3154,19 +4112,21 @@
     "_OptionalGetDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetDatabaseRequestRequestTypeDef(
     _RequiredGetDatabaseRequestRequestTypeDef, _OptionalGetDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 GetDatabasesRequestRequestTypeDef = TypedDict(
     "GetDatabasesRequestRequestTypeDef",
     {
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
         "ResourceShareType": ResourceShareTypeType,
@@ -3208,31 +4168,32 @@
     "_OptionalGetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
+
 class GetJobBookmarkRequestRequestTypeDef(
     _RequiredGetJobBookmarkRequestRequestTypeDef, _OptionalGetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
+
 JobBookmarkEntryTypeDef = TypedDict(
     "JobBookmarkEntryTypeDef",
     {
         "JobName": str,
         "Version": int,
         "Run": int,
         "Attempt": int,
         "PreviousRunId": str,
         "RunId": str,
         "JobBookmark": str,
     },
-    total=False,
 )
 
 GetJobRequestRequestTypeDef = TypedDict(
     "GetJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
@@ -3249,19 +4210,21 @@
     "_OptionalGetJobRunRequestRequestTypeDef",
     {
         "PredecessorsIncluded": bool,
     },
     total=False,
 )
 
+
 class GetJobRunRequestRequestTypeDef(
     _RequiredGetJobRunRequestRequestTypeDef, _OptionalGetJobRunRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJobRunsRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 _OptionalGetJobRunsRequestRequestTypeDef = TypedDict(
@@ -3269,19 +4232,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetJobRunsRequestRequestTypeDef(
     _RequiredGetJobRunsRequestRequestTypeDef, _OptionalGetJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 GetJobsRequestRequestTypeDef = TypedDict(
     "GetJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3317,42 +4282,40 @@
 GetMLTransformRequestRequestTypeDef = TypedDict(
     "GetMLTransformRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
-SchemaColumnTypeDef = TypedDict(
-    "SchemaColumnTypeDef",
+SchemaColumnOutputTypeDef = TypedDict(
+    "SchemaColumnOutputTypeDef",
     {
         "Name": str,
         "DataType": str,
     },
-    total=False,
 )
 
 TransformSortCriteriaTypeDef = TypedDict(
     "TransformSortCriteriaTypeDef",
     {
         "Column": TransformSortColumnTypeType,
         "SortDirection": SortDirectionTypeType,
     },
 )
 
-MappingEntryTypeDef = TypedDict(
-    "MappingEntryTypeDef",
+MappingEntryOutputTypeDef = TypedDict(
+    "MappingEntryOutputTypeDef",
     {
         "SourceTable": str,
         "SourcePath": str,
         "SourceType": str,
         "TargetTable": str,
         "TargetPath": str,
         "TargetType": str,
     },
-    total=False,
 )
 
 _RequiredGetPartitionIndexesRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionIndexesRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
@@ -3363,20 +4326,22 @@
     {
         "CatalogId": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetPartitionIndexesRequestRequestTypeDef(
     _RequiredGetPartitionIndexesRequestRequestTypeDef,
     _OptionalGetPartitionIndexesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -3385,27 +4350,42 @@
     "_OptionalGetPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetPartitionRequestRequestTypeDef(
     _RequiredGetPartitionRequestRequestTypeDef, _OptionalGetPartitionRequestRequestTypeDef
 ):
     pass
 
+
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentNumber": int,
         "TotalSegments": int,
     },
 )
 
+MappingEntryTypeDef = TypedDict(
+    "MappingEntryTypeDef",
+    {
+        "SourceTable": str,
+        "SourcePath": str,
+        "SourceType": str,
+        "TargetTable": str,
+        "TargetPath": str,
+        "TargetType": str,
+    },
+    total=False,
+)
+
 GetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "GetResourcePoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3415,15 +4395,14 @@
     "GluePolicyTypeDef",
     {
         "PolicyInJson": str,
         "PolicyHash": str,
         "CreateTime": datetime,
         "UpdateTime": datetime,
     },
-    total=False,
 )
 
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
@@ -3465,19 +4444,21 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetStatementRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementRequestRequestTypeDef",
     {
         "SessionId": str,
         "Id": int,
     },
 )
@@ -3485,19 +4466,21 @@
     "_OptionalGetStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class GetStatementRequestRequestTypeDef(
     _RequiredGetStatementRequestRequestTypeDef, _OptionalGetStatementRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTableRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -3507,19 +4490,21 @@
         "CatalogId": str,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetTableRequestRequestTypeDef(
     _RequiredGetTableRequestRequestTypeDef, _OptionalGetTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3528,19 +4513,21 @@
     {
         "CatalogId": str,
         "VersionId": str,
     },
     total=False,
 )
 
+
 class GetTableVersionRequestRequestTypeDef(
     _RequiredGetTableVersionRequestRequestTypeDef, _OptionalGetTableVersionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTableVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3550,19 +4537,21 @@
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetTableVersionsRequestRequestTypeDef(
     _RequiredGetTableVersionsRequestRequestTypeDef, _OptionalGetTableVersionsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTablesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTablesRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestRequestTypeDef = TypedDict(
@@ -3574,19 +4563,21 @@
         "MaxResults": int,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetTablesRequestRequestTypeDef(
     _RequiredGetTablesRequestRequestTypeDef, _OptionalGetTablesRequestRequestTypeDef
 ):
     pass
 
+
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -3618,20 +4609,22 @@
     "_OptionalGetUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetUserDefinedFunctionRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUserDefinedFunctionsRequestRequestTypeDef",
     {
         "Pattern": str,
     },
 )
 _OptionalGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
@@ -3641,39 +4634,43 @@
         "DatabaseName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetUserDefinedFunctionsRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionsRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalGetWorkflowRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
+
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
+
 GetWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -3689,19 +4686,21 @@
     "_OptionalGetWorkflowRunRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
+
 class GetWorkflowRunRequestRequestTypeDef(
     _RequiredGetWorkflowRunRequestRequestTypeDef, _OptionalGetWorkflowRunRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetWorkflowRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRunsRequestRequestTypeDef = TypedDict(
@@ -3710,38 +4709,58 @@
         "IncludeGraph": bool,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetWorkflowRunsRequestRequestTypeDef(
     _RequiredGetWorkflowRunsRequestRequestTypeDef, _OptionalGetWorkflowRunsRequestRequestTypeDef
 ):
     pass
 
+
+GlueStudioSchemaColumnOutputTypeDef = TypedDict(
+    "GlueStudioSchemaColumnOutputTypeDef",
+    {
+        "Name": str,
+        "Type": str,
+    },
+)
+
 _RequiredGlueStudioSchemaColumnTypeDef = TypedDict(
     "_RequiredGlueStudioSchemaColumnTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGlueStudioSchemaColumnTypeDef = TypedDict(
     "_OptionalGlueStudioSchemaColumnTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
+
 class GlueStudioSchemaColumnTypeDef(
     _RequiredGlueStudioSchemaColumnTypeDef, _OptionalGlueStudioSchemaColumnTypeDef
 ):
     pass
 
+
+S3SourceAdditionalOptionsOutputTypeDef = TypedDict(
+    "S3SourceAdditionalOptionsOutputTypeDef",
+    {
+        "BoundedSize": int,
+        "BoundedFiles": int,
+    },
+)
+
 S3SourceAdditionalOptionsTypeDef = TypedDict(
     "S3SourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
     },
     total=False,
@@ -3757,63 +4776,109 @@
     "_OptionalIcebergInputTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class IcebergInputTypeDef(_RequiredIcebergInputTypeDef, _OptionalIcebergInputTypeDef):
     pass
 
+
 ImportCatalogToGlueRequestRequestTypeDef = TypedDict(
     "ImportCatalogToGlueRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
 ImportLabelsTaskRunPropertiesTypeDef = TypedDict(
     "ImportLabelsTaskRunPropertiesTypeDef",
     {
         "InputS3Path": str,
         "Replace": bool,
     },
-    total=False,
 )
 
-JDBCConnectorOptionsTypeDef = TypedDict(
-    "JDBCConnectorOptionsTypeDef",
+JDBCConnectorOptionsOutputTypeDef = TypedDict(
+    "JDBCConnectorOptionsOutputTypeDef",
     {
         "FilterPredicate": str,
         "PartitionColumn": str,
         "LowerBound": int,
         "UpperBound": int,
         "NumPartitions": int,
         "JobBookmarkKeys": List[str],
         "JobBookmarkKeysSortOrder": str,
         "DataTypeMapping": Dict[JDBCDataTypeType, GlueRecordTypeType],
     },
+)
+
+JDBCConnectorOptionsTypeDef = TypedDict(
+    "JDBCConnectorOptionsTypeDef",
+    {
+        "FilterPredicate": str,
+        "PartitionColumn": str,
+        "LowerBound": int,
+        "UpperBound": int,
+        "NumPartitions": int,
+        "JobBookmarkKeys": Sequence[str],
+        "JobBookmarkKeysSortOrder": str,
+        "DataTypeMapping": Mapping[JDBCDataTypeType, GlueRecordTypeType],
+    },
     total=False,
 )
 
+JobCommandOutputTypeDef = TypedDict(
+    "JobCommandOutputTypeDef",
+    {
+        "Name": str,
+        "ScriptLocation": str,
+        "PythonVersion": str,
+        "Runtime": str,
+    },
+)
+
 PredecessorTypeDef = TypedDict(
     "PredecessorTypeDef",
     {
         "JobName": str,
         "RunId": str,
     },
-    total=False,
+)
+
+SourceControlDetailsOutputTypeDef = TypedDict(
+    "SourceControlDetailsOutputTypeDef",
+    {
+        "Provider": SourceControlProviderType,
+        "Repository": str,
+        "Owner": str,
+        "Branch": str,
+        "Folder": str,
+        "LastCommitId": str,
+        "AuthStrategy": SourceControlAuthStrategyType,
+        "AuthToken": str,
+    },
+)
+
+JoinColumnOutputTypeDef = TypedDict(
+    "JoinColumnOutputTypeDef",
+    {
+        "From": str,
+        "Keys": List[List[str]],
+    },
 )
 
 JoinColumnTypeDef = TypedDict(
     "JoinColumnTypeDef",
     {
         "From": str,
-        "Keys": List[List[str]],
+        "Keys": Sequence[Sequence[str]],
     },
 )
 
 KeySchemaElementTypeDef = TypedDict(
     "KeySchemaElementTypeDef",
     {
         "Name": str,
@@ -3822,15 +4887,14 @@
 )
 
 LabelingSetGenerationTaskRunPropertiesTypeDef = TypedDict(
     "LabelingSetGenerationTaskRunPropertiesTypeDef",
     {
         "OutputS3Path": str,
     },
-    total=False,
 )
 
 ListBlueprintsRequestRequestTypeDef = TypedDict(
     "ListBlueprintsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -3894,41 +4958,38 @@
         "RegistryName": str,
         "RegistryArn": str,
         "Description": str,
         "Status": RegistryStatusType,
         "CreatedTime": str,
         "UpdatedTime": str,
     },
-    total=False,
 )
 
 SchemaVersionListItemTypeDef = TypedDict(
     "SchemaVersionListItemTypeDef",
     {
         "SchemaArn": str,
         "SchemaVersionId": str,
         "VersionNumber": int,
         "Status": SchemaVersionStatusType,
         "CreatedTime": str,
     },
-    total=False,
 )
 
 SchemaListItemTypeDef = TypedDict(
     "SchemaListItemTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
         "SchemaArn": str,
         "Description": str,
         "SchemaStatus": SchemaStatusType,
         "CreatedTime": str,
         "UpdatedTime": str,
     },
-    total=False,
 )
 
 ListSessionsRequestRequestTypeDef = TypedDict(
     "ListSessionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -3949,19 +5010,21 @@
     {
         "RequestOrigin": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStatementsRequestRequestTypeDef(
     _RequiredListStatementsRequestRequestTypeDef, _OptionalListStatementsRequestRequestTypeDef
 ):
     pass
 
+
 ListTriggersRequestRequestTypeDef = TypedDict(
     "ListTriggersRequestRequestTypeDef",
     {
         "NextToken": str,
         "DependentJobName": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
@@ -3974,64 +5037,93 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+MLUserDataEncryptionOutputTypeDef = TypedDict(
+    "MLUserDataEncryptionOutputTypeDef",
+    {
+        "MlUserDataEncryptionMode": MLUserDataEncryptionModeStringType,
+        "KmsKeyId": str,
+    },
+)
+
 _RequiredMLUserDataEncryptionTypeDef = TypedDict(
     "_RequiredMLUserDataEncryptionTypeDef",
     {
         "MlUserDataEncryptionMode": MLUserDataEncryptionModeStringType,
     },
 )
 _OptionalMLUserDataEncryptionTypeDef = TypedDict(
     "_OptionalMLUserDataEncryptionTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class MLUserDataEncryptionTypeDef(
     _RequiredMLUserDataEncryptionTypeDef, _OptionalMLUserDataEncryptionTypeDef
 ):
     pass
 
-MappingTypeDef = TypedDict(
-    "MappingTypeDef",
+
+MappingOutputTypeDef = TypedDict(
+    "MappingOutputTypeDef",
     {
         "ToKey": str,
         "FromPath": List[str],
         "FromType": str,
         "ToType": str,
         "Dropped": bool,
         "Children": List[Dict[str, Any]],
     },
+)
+
+MappingTypeDef = TypedDict(
+    "MappingTypeDef",
+    {
+        "ToKey": str,
+        "FromPath": Sequence[str],
+        "FromType": str,
+        "ToType": str,
+        "Dropped": bool,
+        "Children": Sequence[Dict[str, Any]],
+    },
     total=False,
 )
 
 OtherMetadataValueListItemTypeDef = TypedDict(
     "OtherMetadataValueListItemTypeDef",
     {
         "MetadataValue": str,
         "CreatedTime": str,
     },
-    total=False,
 )
 
 MetadataKeyValuePairTypeDef = TypedDict(
     "MetadataKeyValuePairTypeDef",
     {
         "MetadataKey": str,
         "MetadataValue": str,
     },
     total=False,
 )
 
+OrderOutputTypeDef = TypedDict(
+    "OrderOutputTypeDef",
+    {
+        "Column": str,
+        "SortOrder": int,
+    },
+)
+
 OrderTypeDef = TypedDict(
     "OrderTypeDef",
     {
         "Column": str,
         "SortOrder": int,
     },
 )
@@ -4059,34 +5151,45 @@
         "PolicyHashCondition": str,
         "PolicyExistsCondition": ExistConditionType,
         "EnableHybrid": EnableHybridValuesType,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+
 PutWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
         "RunProperties": Mapping[str, str],
     },
 )
 
+UpsertRedshiftTargetOptionsOutputTypeDef = TypedDict(
+    "UpsertRedshiftTargetOptionsOutputTypeDef",
+    {
+        "TableLocation": str,
+        "ConnectionName": str,
+        "UpsertKeys": List[str],
+    },
+)
+
 UpsertRedshiftTargetOptionsTypeDef = TypedDict(
     "UpsertRedshiftTargetOptionsTypeDef",
     {
         "TableLocation": str,
         "ConnectionName": str,
-        "UpsertKeys": List[str],
+        "UpsertKeys": Sequence[str],
     },
     total=False,
 )
 
 _RequiredResetJobBookmarkRequestRequestTypeDef = TypedDict(
     "_RequiredResetJobBookmarkRequestRequestTypeDef",
     {
@@ -4097,19 +5200,29 @@
     "_OptionalResetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
+
 class ResetJobBookmarkRequestRequestTypeDef(
     _RequiredResetJobBookmarkRequestRequestTypeDef, _OptionalResetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
+
+ResourceUriOutputTypeDef = TypedDict(
+    "ResourceUriOutputTypeDef",
+    {
+        "ResourceType": ResourceTypeType,
+        "Uri": str,
+    },
+)
+
 ResourceUriTypeDef = TypedDict(
     "ResourceUriTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Uri": str,
     },
     total=False,
@@ -4135,59 +5248,123 @@
     "_OptionalRunStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class RunStatementRequestRequestTypeDef(
     _RequiredRunStatementRequestRequestTypeDef, _OptionalRunStatementRequestRequestTypeDef
 ):
     pass
 
+
+S3DirectSourceAdditionalOptionsOutputTypeDef = TypedDict(
+    "S3DirectSourceAdditionalOptionsOutputTypeDef",
+    {
+        "BoundedSize": int,
+        "BoundedFiles": int,
+        "EnableSamplePath": bool,
+        "SamplePath": str,
+    },
+)
+
 S3DirectSourceAdditionalOptionsTypeDef = TypedDict(
     "S3DirectSourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
         "EnableSamplePath": bool,
         "SamplePath": str,
     },
     total=False,
 )
 
+SchemaColumnTypeDef = TypedDict(
+    "SchemaColumnTypeDef",
+    {
+        "Name": str,
+        "DataType": str,
+    },
+    total=False,
+)
+
+SchemaIdOutputTypeDef = TypedDict(
+    "SchemaIdOutputTypeDef",
+    {
+        "SchemaArn": str,
+        "SchemaName": str,
+        "RegistryName": str,
+    },
+)
+
 SortCriterionTypeDef = TypedDict(
     "SortCriterionTypeDef",
     {
         "FieldName": str,
         "Sort": SortType,
     },
     total=False,
 )
 
+SerDeInfoOutputTypeDef = TypedDict(
+    "SerDeInfoOutputTypeDef",
+    {
+        "Name": str,
+        "SerializationLibrary": str,
+        "Parameters": Dict[str, str],
+    },
+)
+
 SerDeInfoTypeDef = TypedDict(
     "SerDeInfoTypeDef",
     {
         "Name": str,
         "SerializationLibrary": str,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+SessionCommandOutputTypeDef = TypedDict(
+    "SessionCommandOutputTypeDef",
+    {
+        "Name": str,
+        "PythonVersion": str,
+    },
+)
+
+SkewedInfoOutputTypeDef = TypedDict(
+    "SkewedInfoOutputTypeDef",
+    {
+        "SkewedColumnNames": List[str],
+        "SkewedColumnValues": List[str],
+        "SkewedColumnValueLocationMaps": Dict[str, str],
+    },
+)
+
 SkewedInfoTypeDef = TypedDict(
     "SkewedInfoTypeDef",
     {
         "SkewedColumnNames": Sequence[str],
         "SkewedColumnValues": Sequence[str],
         "SkewedColumnValueLocationMaps": Mapping[str, str],
     },
     total=False,
 )
 
+SqlAliasOutputTypeDef = TypedDict(
+    "SqlAliasOutputTypeDef",
+    {
+        "From": str,
+        "Alias": str,
+    },
+)
+
 SqlAliasTypeDef = TypedDict(
     "SqlAliasTypeDef",
     {
         "From": str,
         "Alias": str,
     },
 )
@@ -4203,19 +5380,21 @@
     "_OptionalStartBlueprintRunRequestRequestTypeDef",
     {
         "Parameters": str,
     },
     total=False,
 )
 
+
 class StartBlueprintRunRequestRequestTypeDef(
     _RequiredStartBlueprintRunRequestRequestTypeDef, _OptionalStartBlueprintRunRequestRequestTypeDef
 ):
     pass
 
+
 StartCrawlerRequestRequestTypeDef = TypedDict(
     "StartCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4245,20 +5424,22 @@
     "_OptionalStartImportLabelsTaskRunRequestRequestTypeDef",
     {
         "ReplaceAllLabels": bool,
     },
     total=False,
 )
 
+
 class StartImportLabelsTaskRunRequestRequestTypeDef(
     _RequiredStartImportLabelsTaskRunRequestRequestTypeDef,
     _OptionalStartImportLabelsTaskRunRequestRequestTypeDef,
 ):
     pass
 
+
 StartMLEvaluationTaskRunRequestRequestTypeDef = TypedDict(
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
@@ -4287,34 +5468,34 @@
     "_OptionalStartWorkflowRunRequestRequestTypeDef",
     {
         "RunProperties": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartWorkflowRunRequestRequestTypeDef(
     _RequiredStartWorkflowRunRequestRequestTypeDef, _OptionalStartWorkflowRunRequestRequestTypeDef
 ):
     pass
 
+
 StartingEventBatchConditionTypeDef = TypedDict(
     "StartingEventBatchConditionTypeDef",
     {
         "BatchSize": int,
         "BatchWindow": int,
     },
-    total=False,
 )
 
 StatementOutputDataTypeDef = TypedDict(
     "StatementOutputDataTypeDef",
     {
         "TextPlain": str,
     },
-    total=False,
 )
 
 StopCrawlerRequestRequestTypeDef = TypedDict(
     "StopCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -4337,19 +5518,21 @@
     "_OptionalStopSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class StopSessionRequestRequestTypeDef(
     _RequiredStopSessionRequestRequestTypeDef, _OptionalStopSessionRequestRequestTypeDef
 ):
     pass
 
+
 StopTriggerRequestRequestTypeDef = TypedDict(
     "StopTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4357,14 +5540,24 @@
     "StopWorkflowRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
 
+TableIdentifierOutputTypeDef = TypedDict(
+    "TableIdentifierOutputTypeDef",
+    {
+        "CatalogId": str,
+        "DatabaseName": str,
+        "Name": str,
+        "Region": str,
+    },
+)
+
 TableIdentifierTypeDef = TypedDict(
     "TableIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
         "Region": str,
@@ -4399,19 +5592,21 @@
     "_OptionalUpdateBlueprintRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateBlueprintRequestRequestTypeDef(
     _RequiredUpdateBlueprintRequestRequestTypeDef, _OptionalUpdateBlueprintRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCsvClassifierRequestTypeDef = TypedDict(
@@ -4425,19 +5620,21 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateCsvClassifierRequestTypeDef(
     _RequiredUpdateCsvClassifierRequestTypeDef, _OptionalUpdateCsvClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateGrokClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateGrokClassifierRequestTypeDef = TypedDict(
@@ -4446,38 +5643,42 @@
         "Classification": str,
         "GrokPattern": str,
         "CustomPatterns": str,
     },
     total=False,
 )
 
+
 class UpdateGrokClassifierRequestTypeDef(
     _RequiredUpdateGrokClassifierRequestTypeDef, _OptionalUpdateGrokClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateJsonClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_OptionalUpdateJsonClassifierRequestTypeDef",
     {
         "JsonPath": str,
     },
     total=False,
 )
 
+
 class UpdateJsonClassifierRequestTypeDef(
     _RequiredUpdateJsonClassifierRequestTypeDef, _OptionalUpdateJsonClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateXMLClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateXMLClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateXMLClassifierRequestTypeDef = TypedDict(
@@ -4485,39 +5686,43 @@
     {
         "Classification": str,
         "RowTag": str,
     },
     total=False,
 )
 
+
 class UpdateXMLClassifierRequestTypeDef(
     _RequiredUpdateXMLClassifierRequestTypeDef, _OptionalUpdateXMLClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "CrawlerName": str,
     },
 )
 _OptionalUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "Schedule": str,
     },
     total=False,
 )
 
+
 class UpdateCrawlerScheduleRequestRequestTypeDef(
     _RequiredUpdateCrawlerScheduleRequestRequestTypeDef,
     _OptionalUpdateCrawlerScheduleRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataQualityRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
@@ -4525,20 +5730,22 @@
     {
         "Description": str,
         "Ruleset": str,
     },
     total=False,
 )
 
+
 class UpdateDataQualityRulesetRequestRequestTypeDef(
     _RequiredUpdateDataQualityRulesetRequestRequestTypeDef,
     _OptionalUpdateDataQualityRulesetRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateJobFromSourceControlRequestRequestTypeDef = TypedDict(
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     {
         "JobName": str,
         "Provider": SourceControlProviderType,
         "RepositoryName": str,
         "RepositoryOwner": str,
@@ -4579,39 +5786,52 @@
         "Description": str,
         "DefaultRunProperties": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
+
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
+
 WorkflowRunStatisticsTypeDef = TypedDict(
     "WorkflowRunStatisticsTypeDef",
     {
         "TotalActions": int,
         "TimeoutActions": int,
         "FailedActions": int,
         "StoppedActions": int,
         "SucceededActions": int,
         "RunningActions": int,
         "ErroredActions": int,
         "WaitingActions": int,
     },
-    total=False,
+)
+
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "JobName": str,
+        "Arguments": Dict[str, str],
+        "Timeout": int,
+        "SecurityConfiguration": str,
+        "NotificationProperty": NotificationPropertyOutputTypeDef,
+        "CrawlerName": str,
+    },
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "JobName": str,
-        "Arguments": Dict[str, str],
+        "Arguments": Mapping[str, str],
         "Timeout": int,
         "SecurityConfiguration": str,
         "NotificationProperty": NotificationPropertyTypeDef,
         "CrawlerName": str,
     },
     total=False,
 )
@@ -4635,26 +5855,70 @@
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "ExecutionClass": ExecutionClassType,
     },
     total=False,
 )
 
+
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
-AggregateTypeDef = TypedDict(
-    "AggregateTypeDef",
+
+AggregateOutputTypeDef = TypedDict(
+    "AggregateOutputTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Groups": List[List[str]],
-        "Aggs": List[AggregateOperationTypeDef],
+        "Aggs": List[AggregateOperationOutputTypeDef],
+    },
+)
+
+AggregateTypeDef = TypedDict(
+    "AggregateTypeDef",
+    {
+        "Name": str,
+        "Inputs": Sequence[str],
+        "Groups": Sequence[Sequence[str]],
+        "Aggs": Sequence[AggregateOperationTypeDef],
+    },
+)
+
+AmazonRedshiftNodeDataOutputTypeDef = TypedDict(
+    "AmazonRedshiftNodeDataOutputTypeDef",
+    {
+        "AccessType": str,
+        "SourceType": str,
+        "Connection": OptionOutputTypeDef,
+        "Schema": OptionOutputTypeDef,
+        "Table": OptionOutputTypeDef,
+        "CatalogDatabase": OptionOutputTypeDef,
+        "CatalogTable": OptionOutputTypeDef,
+        "CatalogRedshiftSchema": str,
+        "CatalogRedshiftTable": str,
+        "TempDir": str,
+        "IamRole": OptionOutputTypeDef,
+        "AdvancedOptions": List[AmazonRedshiftAdvancedOptionOutputTypeDef],
+        "SampleQuery": str,
+        "PreAction": str,
+        "PostAction": str,
+        "Action": str,
+        "TablePrefix": str,
+        "Upsert": bool,
+        "MergeAction": str,
+        "MergeWhenMatched": str,
+        "MergeWhenNotMatched": str,
+        "MergeClause": str,
+        "CrawlerConnection": str,
+        "TableSchema": List[OptionOutputTypeDef],
+        "StagingTable": str,
+        "SelectedColumns": List[OptionOutputTypeDef],
     },
 )
 
 AmazonRedshiftNodeDataTypeDef = TypedDict(
     "AmazonRedshiftNodeDataTypeDef",
     {
         "AccessType": str,
@@ -4664,29 +5928,29 @@
         "Table": OptionTypeDef,
         "CatalogDatabase": OptionTypeDef,
         "CatalogTable": OptionTypeDef,
         "CatalogRedshiftSchema": str,
         "CatalogRedshiftTable": str,
         "TempDir": str,
         "IamRole": OptionTypeDef,
-        "AdvancedOptions": List[AmazonRedshiftAdvancedOptionTypeDef],
+        "AdvancedOptions": Sequence[AmazonRedshiftAdvancedOptionTypeDef],
         "SampleQuery": str,
         "PreAction": str,
         "PostAction": str,
         "Action": str,
         "TablePrefix": str,
         "Upsert": bool,
         "MergeAction": str,
         "MergeWhenMatched": str,
         "MergeWhenNotMatched": str,
         "MergeClause": str,
         "CrawlerConnection": str,
-        "TableSchema": List[OptionTypeDef],
+        "TableSchema": Sequence[OptionTypeDef],
         "StagingTable": str,
-        "SelectedColumns": List[OptionTypeDef],
+        "SelectedColumns": Sequence[OptionTypeDef],
     },
     total=False,
 )
 
 _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
@@ -4701,20 +5965,22 @@
     "_OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
+
 class GetUnfilteredPartitionMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -4724,72 +5990,30 @@
     "_OptionalGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
+
 class GetUnfilteredTableMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredTableMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 BackfillErrorTypeDef = TypedDict(
     "BackfillErrorTypeDef",
     {
         "Code": BackfillErrorCodeType,
-        "Partitions": List[PartitionValueListTypeDef],
+        "Partitions": List[PartitionValueListOutputTypeDef],
     },
-    total=False,
 )
 
-_RequiredBatchDeletePartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchDeletePartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "PartitionsToDelete": Sequence[PartitionValueListTypeDef],
-    },
-)
-_OptionalBatchDeletePartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchDeletePartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class BatchDeletePartitionRequestRequestTypeDef(
-    _RequiredBatchDeletePartitionRequestRequestTypeDef,
-    _OptionalBatchDeletePartitionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetPartitionRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "PartitionsToGet": Sequence[PartitionValueListTypeDef],
-    },
-)
-_OptionalBatchGetPartitionRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetPartitionRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class BatchGetPartitionRequestRequestTypeDef(
-    _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
-):
-    pass
-
 CancelMLTaskRunResponseTypeDef = TypedDict(
     "CancelMLTaskRunResponseTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
         "Status": TaskStatusTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5439,63 +6663,104 @@
 BatchStopJobRunErrorTypeDef = TypedDict(
     "BatchStopJobRunErrorTypeDef",
     {
         "JobName": str,
         "JobRunId": str,
         "ErrorDetail": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 BatchUpdatePartitionFailureEntryTypeDef = TypedDict(
     "BatchUpdatePartitionFailureEntryTypeDef",
     {
         "PartitionValueList": List[str],
         "ErrorDetail": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 ColumnErrorTypeDef = TypedDict(
     "ColumnErrorTypeDef",
     {
         "ColumnName": str,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 PartitionErrorTypeDef = TypedDict(
     "PartitionErrorTypeDef",
     {
         "PartitionValues": List[str],
         "ErrorDetail": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 TableErrorTypeDef = TypedDict(
     "TableErrorTypeDef",
     {
         "TableName": str,
         "ErrorDetail": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 TableVersionErrorTypeDef = TypedDict(
     "TableVersionErrorTypeDef",
     {
         "TableName": str,
         "VersionId": str,
         "ErrorDetail": ErrorDetailTypeDef,
     },
+)
+
+_RequiredBatchDeletePartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchDeletePartitionRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "PartitionsToDelete": Sequence[PartitionValueListTypeDef],
+    },
+)
+_OptionalBatchDeletePartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchDeletePartitionRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class BatchDeletePartitionRequestRequestTypeDef(
+    _RequiredBatchDeletePartitionRequestRequestTypeDef,
+    _OptionalBatchDeletePartitionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetPartitionRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "PartitionsToGet": Sequence[PartitionValueListTypeDef],
+    },
+)
+_OptionalBatchGetPartitionRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetPartitionRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
     total=False,
 )
 
+
+class BatchGetPartitionRequestRequestTypeDef(
+    _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
+):
+    pass
+
+
 BatchGetCustomEntityTypesResponseTypeDef = TypedDict(
     "BatchGetCustomEntityTypesResponseTypeDef",
     {
         "CustomEntityTypes": List[CustomEntityTypeTypeDef],
         "CustomEntityTypesNotFound": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -5563,25 +6828,48 @@
         "ParameterSpec": str,
         "BlueprintLocation": str,
         "BlueprintServiceLocation": str,
         "Status": BlueprintStatusType,
         "ErrorMessage": str,
         "LastActiveDefinition": LastActiveDefinitionTypeDef,
     },
-    total=False,
 )
 
 GetCatalogImportStatusResponseTypeDef = TypedDict(
     "GetCatalogImportStatusResponseTypeDef",
     {
         "ImportStatus": CatalogImportStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CatalogKafkaSourceOutputTypeDef = TypedDict(
+    "CatalogKafkaSourceOutputTypeDef",
+    {
+        "Name": str,
+        "WindowSize": int,
+        "DetectSchema": bool,
+        "Table": str,
+        "Database": str,
+        "StreamingOptions": KafkaStreamingSourceOptionsOutputTypeDef,
+        "DataPreviewOptions": StreamingDataPreviewOptionsOutputTypeDef,
+    },
+)
+
+DirectKafkaSourceOutputTypeDef = TypedDict(
+    "DirectKafkaSourceOutputTypeDef",
+    {
+        "Name": str,
+        "StreamingOptions": KafkaStreamingSourceOptionsOutputTypeDef,
+        "WindowSize": int,
+        "DetectSchema": bool,
+        "DataPreviewOptions": StreamingDataPreviewOptionsOutputTypeDef,
+    },
+)
+
 _RequiredCatalogKafkaSourceTypeDef = TypedDict(
     "_RequiredCatalogKafkaSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
@@ -5593,19 +6881,21 @@
         "DetectSchema": bool,
         "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class CatalogKafkaSourceTypeDef(
     _RequiredCatalogKafkaSourceTypeDef, _OptionalCatalogKafkaSourceTypeDef
 ):
     pass
 
+
 _RequiredDirectKafkaSourceTypeDef = TypedDict(
     "_RequiredDirectKafkaSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKafkaSourceTypeDef = TypedDict(
@@ -5615,19 +6905,45 @@
         "WindowSize": int,
         "DetectSchema": bool,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class DirectKafkaSourceTypeDef(
     _RequiredDirectKafkaSourceTypeDef, _OptionalDirectKafkaSourceTypeDef
 ):
     pass
 
+
+CatalogKinesisSourceOutputTypeDef = TypedDict(
+    "CatalogKinesisSourceOutputTypeDef",
+    {
+        "Name": str,
+        "WindowSize": int,
+        "DetectSchema": bool,
+        "Table": str,
+        "Database": str,
+        "StreamingOptions": KinesisStreamingSourceOptionsOutputTypeDef,
+        "DataPreviewOptions": StreamingDataPreviewOptionsOutputTypeDef,
+    },
+)
+
+DirectKinesisSourceOutputTypeDef = TypedDict(
+    "DirectKinesisSourceOutputTypeDef",
+    {
+        "Name": str,
+        "WindowSize": int,
+        "DetectSchema": bool,
+        "StreamingOptions": KinesisStreamingSourceOptionsOutputTypeDef,
+        "DataPreviewOptions": StreamingDataPreviewOptionsOutputTypeDef,
+    },
+)
+
 _RequiredCatalogKinesisSourceTypeDef = TypedDict(
     "_RequiredCatalogKinesisSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
@@ -5639,19 +6955,21 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class CatalogKinesisSourceTypeDef(
     _RequiredCatalogKinesisSourceTypeDef, _OptionalCatalogKinesisSourceTypeDef
 ):
     pass
 
+
 _RequiredDirectKinesisSourceTypeDef = TypedDict(
     "_RequiredDirectKinesisSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKinesisSourceTypeDef = TypedDict(
@@ -5661,120 +6979,189 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class DirectKinesisSourceTypeDef(
     _RequiredDirectKinesisSourceTypeDef, _OptionalDirectKinesisSourceTypeDef
 ):
     pass
 
+
+GovernedCatalogTargetOutputTypeDef = TypedDict(
+    "GovernedCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Table": str,
+        "Database": str,
+        "SchemaChangePolicy": CatalogSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3CatalogTargetOutputTypeDef = TypedDict(
+    "S3CatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Table": str,
+        "Database": str,
+        "SchemaChangePolicy": CatalogSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3DeltaCatalogTargetOutputTypeDef = TypedDict(
+    "S3DeltaCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Table": str,
+        "Database": str,
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": CatalogSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3HudiCatalogTargetOutputTypeDef = TypedDict(
+    "S3HudiCatalogTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Table": str,
+        "Database": str,
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": CatalogSchemaChangePolicyOutputTypeDef,
+    },
+)
+
 _RequiredGovernedCatalogTargetTypeDef = TypedDict(
     "_RequiredGovernedCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalGovernedCatalogTargetTypeDef = TypedDict(
     "_OptionalGovernedCatalogTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class GovernedCatalogTargetTypeDef(
     _RequiredGovernedCatalogTargetTypeDef, _OptionalGovernedCatalogTargetTypeDef
 ):
     pass
 
+
 _RequiredS3CatalogTargetTypeDef = TypedDict(
     "_RequiredS3CatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalS3CatalogTargetTypeDef = TypedDict(
     "_OptionalS3CatalogTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
     pass
 
+
 _RequiredS3DeltaCatalogTargetTypeDef = TypedDict(
     "_RequiredS3DeltaCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Table": str,
         "Database": str,
     },
 )
 _OptionalS3DeltaCatalogTargetTypeDef = TypedDict(
     "_OptionalS3DeltaCatalogTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
+        "PartitionKeys": Sequence[Sequence[str]],
+        "AdditionalOptions": Mapping[str, str],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3DeltaCatalogTargetTypeDef(
     _RequiredS3DeltaCatalogTargetTypeDef, _OptionalS3DeltaCatalogTargetTypeDef
 ):
     pass
 
+
 _RequiredS3HudiCatalogTargetTypeDef = TypedDict(
     "_RequiredS3HudiCatalogTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Table": str,
         "Database": str,
-        "AdditionalOptions": Dict[str, str],
+        "AdditionalOptions": Mapping[str, str],
     },
 )
 _OptionalS3HudiCatalogTargetTypeDef = TypedDict(
     "_OptionalS3HudiCatalogTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3HudiCatalogTargetTypeDef(
     _RequiredS3HudiCatalogTargetTypeDef, _OptionalS3HudiCatalogTargetTypeDef
 ):
     pass
 
+
 ClassifierTypeDef = TypedDict(
     "ClassifierTypeDef",
     {
         "GrokClassifier": GrokClassifierTypeDef,
         "XMLClassifier": XMLClassifierTypeDef,
         "JsonClassifier": JsonClassifierTypeDef,
         "CsvClassifier": CsvClassifierTypeDef,
     },
-    total=False,
+)
+
+CodeGenNodeOutputTypeDef = TypedDict(
+    "CodeGenNodeOutputTypeDef",
+    {
+        "Id": str,
+        "NodeType": str,
+        "Args": List[CodeGenNodeArgOutputTypeDef],
+        "LineNumber": int,
+    },
 )
 
 _RequiredCodeGenNodeTypeDef = TypedDict(
     "_RequiredCodeGenNodeTypeDef",
     {
         "Id": str,
         "NodeType": str,
@@ -5785,47 +7172,56 @@
     "_OptionalCodeGenNodeTypeDef",
     {
         "LineNumber": int,
     },
     total=False,
 )
 
+
 class CodeGenNodeTypeDef(_RequiredCodeGenNodeTypeDef, _OptionalCodeGenNodeTypeDef):
     pass
 
+
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "Jdbc": Sequence[CodeGenNodeArgTypeDef],
         "S3": Sequence[CodeGenNodeArgTypeDef],
         "DynamoDB": Sequence[CodeGenNodeArgTypeDef],
     },
     total=False,
 )
 
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
+    {
+        "Logical": LogicalType,
+        "Conditions": List[ConditionOutputTypeDef],
+    },
+)
+
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Logical": LogicalType,
-        "Conditions": List[ConditionTypeDef],
+        "Conditions": Sequence[ConditionTypeDef],
     },
     total=False,
 )
 
 FindMatchesMetricsTypeDef = TypedDict(
     "FindMatchesMetricsTypeDef",
     {
         "AreaUnderPRCurve": float,
         "Precision": float,
         "Recall": float,
         "F1": float,
         "ConfusionMatrix": ConfusionMatrixTypeDef,
         "ColumnImportances": List[ColumnImportanceTypeDef],
     },
-    total=False,
 )
 
 _RequiredConnectionInputTypeDef = TypedDict(
     "_RequiredConnectionInputTypeDef",
     {
         "Name": str,
         "ConnectionType": ConnectionTypeType,
@@ -5838,39 +7234,39 @@
         "Description": str,
         "MatchCriteria": Sequence[str],
         "PhysicalConnectionRequirements": PhysicalConnectionRequirementsTypeDef,
     },
     total=False,
 )
 
+
 class ConnectionInputTypeDef(_RequiredConnectionInputTypeDef, _OptionalConnectionInputTypeDef):
     pass
 
+
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "Name": str,
         "Description": str,
         "ConnectionType": ConnectionTypeType,
         "MatchCriteria": List[str],
         "ConnectionProperties": Dict[ConnectionPropertyKeyType, str],
-        "PhysicalConnectionRequirements": PhysicalConnectionRequirementsTypeDef,
+        "PhysicalConnectionRequirements": PhysicalConnectionRequirementsOutputTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "LastUpdatedBy": str,
     },
-    total=False,
 )
 
 CrawlerNodeDetailsTypeDef = TypedDict(
     "CrawlerNodeDetailsTypeDef",
     {
         "Crawls": List[CrawlTypeDef],
     },
-    total=False,
 )
 
 ListCrawlsResponseTypeDef = TypedDict(
     "ListCrawlsResponseTypeDef",
     {
         "Crawls": List[CrawlerHistoryTypeDef],
         "NextToken": str,
@@ -5883,24 +7279,37 @@
     {
         "CrawlerMetricsList": List[CrawlerMetricsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CrawlerTargetsOutputTypeDef = TypedDict(
+    "CrawlerTargetsOutputTypeDef",
+    {
+        "S3Targets": List[S3TargetOutputTypeDef],
+        "JdbcTargets": List[JdbcTargetOutputTypeDef],
+        "MongoDBTargets": List[MongoDBTargetOutputTypeDef],
+        "DynamoDBTargets": List[DynamoDBTargetOutputTypeDef],
+        "CatalogTargets": List[CatalogTargetOutputTypeDef],
+        "DeltaTargets": List[DeltaTargetOutputTypeDef],
+        "IcebergTargets": List[IcebergTargetOutputTypeDef],
+    },
+)
+
 CrawlerTargetsTypeDef = TypedDict(
     "CrawlerTargetsTypeDef",
     {
-        "S3Targets": List[S3TargetTypeDef],
-        "JdbcTargets": List[JdbcTargetTypeDef],
-        "MongoDBTargets": List[MongoDBTargetTypeDef],
-        "DynamoDBTargets": List[DynamoDBTargetTypeDef],
-        "CatalogTargets": List[CatalogTargetTypeDef],
-        "DeltaTargets": List[DeltaTargetTypeDef],
-        "IcebergTargets": List[IcebergTargetTypeDef],
+        "S3Targets": Sequence[S3TargetTypeDef],
+        "JdbcTargets": Sequence[JdbcTargetTypeDef],
+        "MongoDBTargets": Sequence[MongoDBTargetTypeDef],
+        "DynamoDBTargets": Sequence[DynamoDBTargetTypeDef],
+        "CatalogTargets": Sequence[CatalogTargetTypeDef],
+        "DeltaTargets": Sequence[DeltaTargetTypeDef],
+        "IcebergTargets": Sequence[IcebergTargetTypeDef],
     },
     total=False,
 )
 
 _RequiredListCrawlsRequestRequestTypeDef = TypedDict(
     "_RequiredListCrawlsRequestRequestTypeDef",
     {
@@ -5913,19 +7322,21 @@
         "MaxResults": int,
         "Filters": Sequence[CrawlsFilterTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListCrawlsRequestRequestTypeDef(
     _RequiredListCrawlsRequestRequestTypeDef, _OptionalListCrawlsRequestRequestTypeDef
 ):
     pass
 
+
 CreateClassifierRequestRequestTypeDef = TypedDict(
     "CreateClassifierRequestRequestTypeDef",
     {
         "GrokClassifier": CreateGrokClassifierRequestTypeDef,
         "XMLClassifier": CreateXMLClassifierRequestTypeDef,
         "JsonClassifier": CreateJsonClassifierRequestTypeDef,
         "CsvClassifier": CreateCsvClassifierRequestTypeDef,
@@ -5947,62 +7358,36 @@
         "Tags": Mapping[str, str],
         "TargetTable": DataQualityTargetTableTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateDataQualityRulesetRequestRequestTypeDef(
     _RequiredCreateDataQualityRulesetRequestRequestTypeDef,
     _OptionalCreateDataQualityRulesetRequestRequestTypeDef,
 ):
     pass
 
+
 DataQualityRulesetFilterCriteriaTypeDef = TypedDict(
     "DataQualityRulesetFilterCriteriaTypeDef",
     {
         "Name": str,
         "Description": str,
         "CreatedBefore": Union[datetime, str],
         "CreatedAfter": Union[datetime, str],
         "LastModifiedBefore": Union[datetime, str],
         "LastModifiedAfter": Union[datetime, str],
         "TargetTable": DataQualityTargetTableTypeDef,
     },
     total=False,
 )
 
-DataQualityRulesetListDetailsTypeDef = TypedDict(
-    "DataQualityRulesetListDetailsTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "CreatedOn": datetime,
-        "LastModifiedOn": datetime,
-        "TargetTable": DataQualityTargetTableTypeDef,
-        "RecommendationRunId": str,
-        "RuleCount": int,
-    },
-    total=False,
-)
-
-GetDataQualityRulesetResponseTypeDef = TypedDict(
-    "GetDataQualityRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Ruleset": str,
-        "TargetTable": DataQualityTargetTableTypeDef,
-        "CreatedOn": datetime,
-        "LastModifiedOn": datetime,
-        "RecommendationRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "GlueTable": GlueTableTypeDef,
     },
 )
 
@@ -6018,20 +7403,22 @@
     "_OptionalCreatePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class CreatePartitionIndexRequestRequestTypeDef(
     _RequiredCreatePartitionIndexRequestRequestTypeDef,
     _OptionalCreatePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSchemaInputRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaInputRequestTypeDef",
     {
         "SchemaName": str,
         "DataFormat": DataFormatType,
     },
 )
@@ -6043,19 +7430,21 @@
         "Description": str,
         "Tags": Mapping[str, str],
         "SchemaDefinition": str,
     },
     total=False,
 )
 
+
 class CreateSchemaInputRequestTypeDef(
     _RequiredCreateSchemaInputRequestTypeDef, _OptionalCreateSchemaInputRequestTypeDef
 ):
     pass
 
+
 DeleteRegistryInputRequestTypeDef = TypedDict(
     "DeleteRegistryInputRequestTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
     },
 )
 
@@ -6107,112 +7496,191 @@
         "GlueVersion": str,
         "Tags": Mapping[str, str],
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class CreateSessionRequestRequestTypeDef(
     _RequiredCreateSessionRequestRequestTypeDef, _OptionalCreateSessionRequestRequestTypeDef
 ):
     pass
 
-SessionTypeDef = TypedDict(
-    "SessionTypeDef",
+
+EvaluateDataQualityMultiFrameOutputTypeDef = TypedDict(
+    "EvaluateDataQualityMultiFrameOutputTypeDef",
     {
-        "Id": str,
-        "CreatedOn": datetime,
-        "Status": SessionStatusType,
-        "ErrorMessage": str,
-        "Description": str,
-        "Role": str,
-        "Command": SessionCommandTypeDef,
-        "DefaultArguments": Dict[str, str],
-        "Connections": ConnectionsListTypeDef,
-        "Progress": float,
-        "MaxCapacity": float,
-        "SecurityConfiguration": str,
-        "GlueVersion": str,
+        "Name": str,
+        "Inputs": List[str],
+        "AdditionalDataSources": Dict[str, str],
+        "Ruleset": str,
+        "PublishingOptions": DQResultsPublishingOptionsOutputTypeDef,
+        "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
+        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsOutputTypeDef,
+    },
+)
+
+EvaluateDataQualityOutputTypeDef = TypedDict(
+    "EvaluateDataQualityOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Ruleset": str,
+        "Output": DQTransformOutputType,
+        "PublishingOptions": DQResultsPublishingOptionsOutputTypeDef,
+        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredEvaluateDataQualityMultiFrameTypeDef = TypedDict(
     "_RequiredEvaluateDataQualityMultiFrameTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Ruleset": str,
     },
 )
 _OptionalEvaluateDataQualityMultiFrameTypeDef = TypedDict(
     "_OptionalEvaluateDataQualityMultiFrameTypeDef",
     {
-        "AdditionalDataSources": Dict[str, str],
+        "AdditionalDataSources": Mapping[str, str],
         "PublishingOptions": DQResultsPublishingOptionsTypeDef,
-        "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
+        "AdditionalOptions": Mapping[Literal["performanceTuning.caching"], str],
         "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
     },
     total=False,
 )
 
+
 class EvaluateDataQualityMultiFrameTypeDef(
     _RequiredEvaluateDataQualityMultiFrameTypeDef, _OptionalEvaluateDataQualityMultiFrameTypeDef
 ):
     pass
 
+
 _RequiredEvaluateDataQualityTypeDef = TypedDict(
     "_RequiredEvaluateDataQualityTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Ruleset": str,
     },
 )
 _OptionalEvaluateDataQualityTypeDef = TypedDict(
     "_OptionalEvaluateDataQualityTypeDef",
     {
         "Output": DQTransformOutputType,
         "PublishingOptions": DQResultsPublishingOptionsTypeDef,
         "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
     },
     total=False,
 )
 
+
 class EvaluateDataQualityTypeDef(
     _RequiredEvaluateDataQualityTypeDef, _OptionalEvaluateDataQualityTypeDef
 ):
     pass
 
+
+DataCatalogEncryptionSettingsOutputTypeDef = TypedDict(
+    "DataCatalogEncryptionSettingsOutputTypeDef",
+    {
+        "EncryptionAtRest": EncryptionAtRestOutputTypeDef,
+        "ConnectionPasswordEncryption": ConnectionPasswordEncryptionOutputTypeDef,
+    },
+)
+
 DataCatalogEncryptionSettingsTypeDef = TypedDict(
     "DataCatalogEncryptionSettingsTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "ConnectionPasswordEncryption": ConnectionPasswordEncryptionTypeDef,
     },
     total=False,
 )
 
+PrincipalPermissionsOutputTypeDef = TypedDict(
+    "PrincipalPermissionsOutputTypeDef",
+    {
+        "Principal": DataLakePrincipalOutputTypeDef,
+        "Permissions": List[PermissionType],
+    },
+)
+
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Permissions": Sequence[PermissionType],
     },
     total=False,
 )
 
+DataQualityRulesetListDetailsTypeDef = TypedDict(
+    "DataQualityRulesetListDetailsTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "CreatedOn": datetime,
+        "LastModifiedOn": datetime,
+        "TargetTable": DataQualityTargetTableOutputTypeDef,
+        "RecommendationRunId": str,
+        "RuleCount": int,
+    },
+)
+
+GetDataQualityRulesetResponseTypeDef = TypedDict(
+    "GetDataQualityRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Ruleset": str,
+        "TargetTable": DataQualityTargetTableOutputTypeDef,
+        "CreatedOn": datetime,
+        "LastModifiedOn": datetime,
+        "RecommendationRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
+    {
+        "GlueTable": GlueTableOutputTypeDef,
+    },
+)
+
+NullValueFieldOutputTypeDef = TypedDict(
+    "NullValueFieldOutputTypeDef",
+    {
+        "Value": str,
+        "Datatype": DatatypeOutputTypeDef,
+    },
+)
+
 NullValueFieldTypeDef = TypedDict(
     "NullValueFieldTypeDef",
     {
         "Value": str,
         "Datatype": DatatypeTypeDef,
     },
 )
 
+DecimalColumnStatisticsDataOutputTypeDef = TypedDict(
+    "DecimalColumnStatisticsDataOutputTypeDef",
+    {
+        "MinimumValue": DecimalNumberOutputTypeDef,
+        "MaximumValue": DecimalNumberOutputTypeDef,
+        "NumberOfNulls": int,
+        "NumberOfDistinctValues": int,
+    },
+)
+
 _RequiredDecimalColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDecimalColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -6221,19 +7689,21 @@
     {
         "MinimumValue": DecimalNumberTypeDef,
         "MaximumValue": DecimalNumberTypeDef,
     },
     total=False,
 )
 
+
 class DecimalColumnStatisticsDataTypeDef(
     _RequiredDecimalColumnStatisticsDataTypeDef, _OptionalDecimalColumnStatisticsDataTypeDef
 ):
     pass
 
+
 DeleteSchemaInputRequestTypeDef = TypedDict(
     "DeleteSchemaInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
     },
 )
 
@@ -6271,19 +7741,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListSchemaVersionsInputRequestTypeDef(
     _RequiredListSchemaVersionsInputRequestTypeDef, _OptionalListSchemaVersionsInputRequestTypeDef
 ):
     pass
 
+
 RegisterSchemaVersionInputRequestTypeDef = TypedDict(
     "RegisterSchemaVersionInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaDefinition": str,
     },
 )
@@ -6314,114 +7786,186 @@
         "UpdateEtlLibraries": bool,
         "DeleteArguments": Sequence[str],
         "AddArguments": Mapping[str, str],
     },
     total=False,
 )
 
+
 class UpdateDevEndpointRequestRequestTypeDef(
     _RequiredUpdateDevEndpointRequestRequestTypeDef, _OptionalUpdateDevEndpointRequestRequestTypeDef
 ):
     pass
 
+
+S3DeltaDirectTargetOutputTypeDef = TypedDict(
+    "S3DeltaDirectTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Path": str,
+        "Compression": DeltaTargetCompressionTypeType,
+        "Format": TargetFormatType,
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": DirectSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3DirectTargetOutputTypeDef = TypedDict(
+    "S3DirectTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Path": str,
+        "Compression": str,
+        "Format": TargetFormatType,
+        "SchemaChangePolicy": DirectSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3GlueParquetTargetOutputTypeDef = TypedDict(
+    "S3GlueParquetTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "PartitionKeys": List[List[str]],
+        "Path": str,
+        "Compression": ParquetCompressionTypeType,
+        "SchemaChangePolicy": DirectSchemaChangePolicyOutputTypeDef,
+    },
+)
+
+S3HudiDirectTargetOutputTypeDef = TypedDict(
+    "S3HudiDirectTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Path": str,
+        "Compression": HudiTargetCompressionTypeType,
+        "PartitionKeys": List[List[str]],
+        "Format": TargetFormatType,
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": DirectSchemaChangePolicyOutputTypeDef,
+    },
+)
+
 _RequiredS3DeltaDirectTargetTypeDef = TypedDict(
     "_RequiredS3DeltaDirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Path": str,
         "Compression": DeltaTargetCompressionTypeType,
         "Format": TargetFormatType,
     },
 )
 _OptionalS3DeltaDirectTargetTypeDef = TypedDict(
     "_OptionalS3DeltaDirectTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
+        "PartitionKeys": Sequence[Sequence[str]],
+        "AdditionalOptions": Mapping[str, str],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3DeltaDirectTargetTypeDef(
     _RequiredS3DeltaDirectTargetTypeDef, _OptionalS3DeltaDirectTargetTypeDef
 ):
     pass
 
+
 _RequiredS3DirectTargetTypeDef = TypedDict(
     "_RequiredS3DirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Path": str,
         "Format": TargetFormatType,
     },
 )
 _OptionalS3DirectTargetTypeDef = TypedDict(
     "_OptionalS3DirectTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "Compression": str,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3DirectTargetTypeDef(_RequiredS3DirectTargetTypeDef, _OptionalS3DirectTargetTypeDef):
     pass
 
+
 _RequiredS3GlueParquetTargetTypeDef = TypedDict(
     "_RequiredS3GlueParquetTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Path": str,
     },
 )
 _OptionalS3GlueParquetTargetTypeDef = TypedDict(
     "_OptionalS3GlueParquetTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "Compression": ParquetCompressionTypeType,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3GlueParquetTargetTypeDef(
     _RequiredS3GlueParquetTargetTypeDef, _OptionalS3GlueParquetTargetTypeDef
 ):
     pass
 
+
 _RequiredS3HudiDirectTargetTypeDef = TypedDict(
     "_RequiredS3HudiDirectTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Path": str,
         "Compression": HudiTargetCompressionTypeType,
         "Format": TargetFormatType,
-        "AdditionalOptions": Dict[str, str],
+        "AdditionalOptions": Mapping[str, str],
     },
 )
 _OptionalS3HudiDirectTargetTypeDef = TypedDict(
     "_OptionalS3HudiDirectTargetTypeDef",
     {
-        "PartitionKeys": List[List[str]],
+        "PartitionKeys": Sequence[Sequence[str]],
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3HudiDirectTargetTypeDef(
     _RequiredS3HudiDirectTargetTypeDef, _OptionalS3HudiDirectTargetTypeDef
 ):
     pass
 
+
+EncryptionConfigurationOutputTypeDef = TypedDict(
+    "EncryptionConfigurationOutputTypeDef",
+    {
+        "S3Encryption": List[S3EncryptionOutputTypeDef],
+        "CloudWatchEncryption": CloudWatchEncryptionOutputTypeDef,
+        "JobBookmarksEncryption": JobBookmarksEncryptionOutputTypeDef,
+    },
+)
+
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "S3Encryption": Sequence[S3EncryptionTypeDef],
         "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
         "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
     },
@@ -6430,54 +7974,74 @@
 
 SchemaVersionErrorItemTypeDef = TypedDict(
     "SchemaVersionErrorItemTypeDef",
     {
         "VersionNumber": int,
         "ErrorDetails": ErrorDetailsTypeDef,
     },
-    total=False,
+)
+
+FilterExpressionOutputTypeDef = TypedDict(
+    "FilterExpressionOutputTypeDef",
+    {
+        "Operation": FilterOperationType,
+        "Negated": bool,
+        "Values": List[FilterValueOutputTypeDef],
+    },
 )
 
 _RequiredFilterExpressionTypeDef = TypedDict(
     "_RequiredFilterExpressionTypeDef",
     {
         "Operation": FilterOperationType,
-        "Values": List[FilterValueTypeDef],
+        "Values": Sequence[FilterValueTypeDef],
     },
 )
 _OptionalFilterExpressionTypeDef = TypedDict(
     "_OptionalFilterExpressionTypeDef",
     {
         "Negated": bool,
     },
     total=False,
 )
 
+
 class FilterExpressionTypeDef(_RequiredFilterExpressionTypeDef, _OptionalFilterExpressionTypeDef):
     pass
 
+
+TransformParametersOutputTypeDef = TypedDict(
+    "TransformParametersOutputTypeDef",
+    {
+        "TransformType": Literal["FIND_MATCHES"],
+        "FindMatchesParameters": FindMatchesParametersOutputTypeDef,
+    },
+)
+
 _RequiredTransformParametersTypeDef = TypedDict(
     "_RequiredTransformParametersTypeDef",
     {
         "TransformType": Literal["FIND_MATCHES"],
     },
 )
 _OptionalTransformParametersTypeDef = TypedDict(
     "_OptionalTransformParametersTypeDef",
     {
         "FindMatchesParameters": FindMatchesParametersTypeDef,
     },
     total=False,
 )
 
+
 class TransformParametersTypeDef(
     _RequiredTransformParametersTypeDef, _OptionalTransformParametersTypeDef
 ):
     pass
 
+
 GetClassifiersRequestGetClassifiersPaginateTypeDef = TypedDict(
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6527,20 +8091,22 @@
     "_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetJobRunsRequestGetJobRunsPaginateTypeDef(
     _RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef,
     _OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef,
 ):
     pass
 
+
 GetJobsRequestGetJobsPaginateTypeDef = TypedDict(
     "GetJobsRequestGetJobsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6557,20 +8123,22 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(
     _RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
     _OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
 ):
     pass
 
+
 GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6595,20 +8163,22 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(
     _RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
     _OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
     "_RequiredGetTablesRequestGetTablesPaginateTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
@@ -6619,20 +8189,22 @@
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetTablesRequestGetTablesPaginateTypeDef(
     _RequiredGetTablesRequestGetTablesPaginateTypeDef,
     _OptionalGetTablesRequestGetTablesPaginateTypeDef,
 ):
     pass
 
+
 GetTriggersRequestGetTriggersPaginateTypeDef = TypedDict(
     "GetTriggersRequestGetTriggersPaginateTypeDef",
     {
         "DependentJobName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6650,20 +8222,22 @@
         "CatalogId": str,
         "DatabaseName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(
     _RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
     _OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
 ):
     pass
 
+
 ListRegistriesInputListRegistriesPaginateTypeDef = TypedDict(
     "ListRegistriesInputListRegistriesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6678,20 +8252,22 @@
     "_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(
     _RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     _OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListSchemasInputListSchemasPaginateTypeDef = TypedDict(
     "ListSchemasInputListSchemasPaginateTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6749,39 +8325,25 @@
         "MaxResults": int,
         "Filter": TaskRunFilterCriteriaTypeDef,
         "Sort": TaskRunSortCriteriaTypeDef,
     },
     total=False,
 )
 
+
 class GetMLTaskRunsRequestRequestTypeDef(
     _RequiredGetMLTaskRunsRequestRequestTypeDef, _OptionalGetMLTaskRunsRequestRequestTypeDef
 ):
     pass
 
-TransformFilterCriteriaTypeDef = TypedDict(
-    "TransformFilterCriteriaTypeDef",
-    {
-        "Name": str,
-        "TransformType": Literal["FIND_MATCHES"],
-        "Status": TransformStatusTypeType,
-        "GlueVersion": str,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
-        "LastModifiedBefore": Union[datetime, str],
-        "LastModifiedAfter": Union[datetime, str],
-        "Schema": Sequence[SchemaColumnTypeDef],
-    },
-    total=False,
-)
 
 GetMappingResponseTypeDef = TypedDict(
     "GetMappingResponseTypeDef",
     {
-        "Mapping": List[MappingEntryTypeDef],
+        "Mapping": List[MappingEntryOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef = TypedDict(
     "_RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef",
     {
@@ -6799,20 +8361,22 @@
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetPartitionsRequestGetPartitionsPaginateTypeDef(
     _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef,
     _OptionalGetPartitionsRequestGetPartitionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetPartitionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -6827,19 +8391,21 @@
         "ExcludeColumnSchema": bool,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetPartitionsRequestRequestTypeDef(
     _RequiredGetPartitionsRequestRequestTypeDef, _OptionalGetPartitionsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -6853,20 +8419,22 @@
         "NextToken": str,
         "Segment": SegmentTypeDef,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetUnfilteredPartitionsMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "GetResourcePoliciesResponseList": List[GluePolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6904,27 +8472,58 @@
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "Compatibility": CompatibilityType,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateSchemaInputRequestTypeDef(
     _RequiredUpdateSchemaInputRequestTypeDef, _OptionalUpdateSchemaInputRequestTypeDef
 ):
     pass
 
+
+GlueSchemaOutputTypeDef = TypedDict(
+    "GlueSchemaOutputTypeDef",
+    {
+        "Columns": List[GlueStudioSchemaColumnOutputTypeDef],
+    },
+)
+
 GlueSchemaTypeDef = TypedDict(
     "GlueSchemaTypeDef",
     {
-        "Columns": List[GlueStudioSchemaColumnTypeDef],
+        "Columns": Sequence[GlueStudioSchemaColumnTypeDef],
     },
     total=False,
 )
 
+GovernedCatalogSourceOutputTypeDef = TypedDict(
+    "GovernedCatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "PartitionPredicate": str,
+        "AdditionalOptions": S3SourceAdditionalOptionsOutputTypeDef,
+    },
+)
+
+S3CatalogSourceOutputTypeDef = TypedDict(
+    "S3CatalogSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "PartitionPredicate": str,
+        "AdditionalOptions": S3SourceAdditionalOptionsOutputTypeDef,
+    },
+)
+
 _RequiredGovernedCatalogSourceTypeDef = TypedDict(
     "_RequiredGovernedCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -6934,19 +8533,21 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
+
 class GovernedCatalogSourceTypeDef(
     _RequiredGovernedCatalogSourceTypeDef, _OptionalGovernedCatalogSourceTypeDef
 ):
     pass
 
+
 _RequiredS3CatalogSourceTypeDef = TypedDict(
     "_RequiredS3CatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -6956,17 +8557,19 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
+
 class S3CatalogSourceTypeDef(_RequiredS3CatalogSourceTypeDef, _OptionalS3CatalogSourceTypeDef):
     pass
 
+
 OpenTableFormatInputTypeDef = TypedDict(
     "OpenTableFormatInputTypeDef",
     {
         "IcebergInput": IcebergInputTypeDef,
     },
     total=False,
 )
@@ -6990,42 +8593,50 @@
         "ExecutionTime": int,
         "Timeout": int,
         "MaxCapacity": float,
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "SecurityConfiguration": str,
         "LogGroupName": str,
-        "NotificationProperty": NotificationPropertyTypeDef,
+        "NotificationProperty": NotificationPropertyOutputTypeDef,
         "GlueVersion": str,
         "DPUSeconds": float,
         "ExecutionClass": ExecutionClassType,
     },
-    total=False,
+)
+
+JoinOutputTypeDef = TypedDict(
+    "JoinOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "JoinType": JoinTypeType,
+        "Columns": List[JoinColumnOutputTypeDef],
+    },
 )
 
 JoinTypeDef = TypedDict(
     "JoinTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "JoinType": JoinTypeType,
-        "Columns": List[JoinColumnTypeDef],
+        "Columns": Sequence[JoinColumnTypeDef],
     },
 )
 
 TaskRunPropertiesTypeDef = TypedDict(
     "TaskRunPropertiesTypeDef",
     {
         "TaskType": TaskTypeType,
         "ImportLabelsTaskRunProperties": ImportLabelsTaskRunPropertiesTypeDef,
         "ExportLabelsTaskRunProperties": ExportLabelsTaskRunPropertiesTypeDef,
         "LabelingSetGenerationTaskRunProperties": LabelingSetGenerationTaskRunPropertiesTypeDef,
         "FindMatchesTaskRunProperties": FindMatchesTaskRunPropertiesTypeDef,
     },
-    total=False,
 )
 
 ListRegistriesResponseTypeDef = TypedDict(
     "ListRegistriesResponseTypeDef",
     {
         "Registries": List[RegistryListItemTypeDef],
         "NextToken": str,
@@ -7047,14 +8658,22 @@
     {
         "Schemas": List[SchemaListItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TransformEncryptionOutputTypeDef = TypedDict(
+    "TransformEncryptionOutputTypeDef",
+    {
+        "MlUserDataEncryption": MLUserDataEncryptionOutputTypeDef,
+        "TaskRunSecurityConfigurationName": str,
+    },
+)
+
 TransformEncryptionTypeDef = TypedDict(
     "TransformEncryptionTypeDef",
     {
         "MlUserDataEncryption": MLUserDataEncryptionTypeDef,
         "TaskRunSecurityConfigurationName": str,
     },
     total=False,
@@ -7063,15 +8682,14 @@
 MetadataInfoTypeDef = TypedDict(
     "MetadataInfoTypeDef",
     {
         "MetadataValue": str,
         "CreatedTime": str,
         "OtherMetadataValueList": List[OtherMetadataValueListItemTypeDef],
     },
-    total=False,
 )
 
 _RequiredPutSchemaVersionMetadataInputRequestTypeDef = TypedDict(
     "_RequiredPutSchemaVersionMetadataInputRequestTypeDef",
     {
         "MetadataKeyValue": MetadataKeyValuePairTypeDef,
     },
@@ -7082,20 +8700,22 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
+
 class PutSchemaVersionMetadataInputRequestTypeDef(
     _RequiredPutSchemaVersionMetadataInputRequestTypeDef,
     _OptionalPutSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
+
 QuerySchemaVersionMetadataInputRequestTypeDef = TypedDict(
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
         "MetadataList": Sequence[MetadataKeyValuePairTypeDef],
@@ -7117,147 +8737,212 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
+
 class RemoveSchemaVersionMetadataInputRequestTypeDef(
     _RequiredRemoveSchemaVersionMetadataInputRequestTypeDef,
     _OptionalRemoveSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
+
+RedshiftTargetOutputTypeDef = TypedDict(
+    "RedshiftTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Database": str,
+        "Table": str,
+        "RedshiftTmpDir": str,
+        "TmpDirIAMRole": str,
+        "UpsertRedshiftOptions": UpsertRedshiftTargetOptionsOutputTypeDef,
+    },
+)
+
 _RequiredRedshiftTargetTypeDef = TypedDict(
     "_RequiredRedshiftTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Database": str,
         "Table": str,
     },
 )
 _OptionalRedshiftTargetTypeDef = TypedDict(
     "_OptionalRedshiftTargetTypeDef",
     {
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
         "UpsertRedshiftOptions": UpsertRedshiftTargetOptionsTypeDef,
     },
     total=False,
 )
 
+
 class RedshiftTargetTypeDef(_RequiredRedshiftTargetTypeDef, _OptionalRedshiftTargetTypeDef):
     pass
 
-UserDefinedFunctionInputTypeDef = TypedDict(
-    "UserDefinedFunctionInputTypeDef",
+
+UserDefinedFunctionTypeDef = TypedDict(
+    "UserDefinedFunctionTypeDef",
     {
         "FunctionName": str,
+        "DatabaseName": str,
         "ClassName": str,
         "OwnerName": str,
         "OwnerType": PrincipalTypeType,
-        "ResourceUris": Sequence[ResourceUriTypeDef],
+        "CreateTime": datetime,
+        "ResourceUris": List[ResourceUriOutputTypeDef],
+        "CatalogId": str,
     },
-    total=False,
 )
 
-UserDefinedFunctionTypeDef = TypedDict(
-    "UserDefinedFunctionTypeDef",
+UserDefinedFunctionInputTypeDef = TypedDict(
+    "UserDefinedFunctionInputTypeDef",
     {
         "FunctionName": str,
-        "DatabaseName": str,
         "ClassName": str,
         "OwnerName": str,
         "OwnerType": PrincipalTypeType,
-        "CreateTime": datetime,
-        "ResourceUris": List[ResourceUriTypeDef],
-        "CatalogId": str,
+        "ResourceUris": Sequence[ResourceUriTypeDef],
+    },
+    total=False,
+)
+
+TransformFilterCriteriaTypeDef = TypedDict(
+    "TransformFilterCriteriaTypeDef",
+    {
+        "Name": str,
+        "TransformType": Literal["FIND_MATCHES"],
+        "Status": TransformStatusTypeType,
+        "GlueVersion": str,
+        "CreatedBefore": Union[datetime, str],
+        "CreatedAfter": Union[datetime, str],
+        "LastModifiedBefore": Union[datetime, str],
+        "LastModifiedAfter": Union[datetime, str],
+        "Schema": Sequence[SchemaColumnTypeDef],
     },
     total=False,
 )
 
+SchemaReferenceOutputTypeDef = TypedDict(
+    "SchemaReferenceOutputTypeDef",
+    {
+        "SchemaId": SchemaIdOutputTypeDef,
+        "SchemaVersionId": str,
+        "SchemaVersionNumber": int,
+    },
+)
+
 SearchTablesRequestRequestTypeDef = TypedDict(
     "SearchTablesRequestRequestTypeDef",
     {
         "CatalogId": str,
         "NextToken": str,
         "Filters": Sequence[PropertyPredicateTypeDef],
         "SearchText": str,
         "SortCriteria": Sequence[SortCriterionTypeDef],
         "MaxResults": int,
         "ResourceShareType": ResourceShareTypeType,
     },
     total=False,
 )
 
+SessionTypeDef = TypedDict(
+    "SessionTypeDef",
+    {
+        "Id": str,
+        "CreatedOn": datetime,
+        "Status": SessionStatusType,
+        "ErrorMessage": str,
+        "Description": str,
+        "Role": str,
+        "Command": SessionCommandOutputTypeDef,
+        "DefaultArguments": Dict[str, str],
+        "Connections": ConnectionsListOutputTypeDef,
+        "Progress": float,
+        "MaxCapacity": float,
+        "SecurityConfiguration": str,
+        "GlueVersion": str,
+    },
+)
+
 StatementOutputTypeDef = TypedDict(
     "StatementOutputTypeDef",
     {
         "Data": StatementOutputDataTypeDef,
         "ExecutionCount": int,
         "Status": StatementStateType,
         "ErrorName": str,
         "ErrorValue": str,
         "Traceback": List[str],
     },
-    total=False,
 )
 
 UpdateClassifierRequestRequestTypeDef = TypedDict(
     "UpdateClassifierRequestRequestTypeDef",
     {
         "GrokClassifier": UpdateGrokClassifierRequestTypeDef,
         "XMLClassifier": UpdateXMLClassifierRequestTypeDef,
         "JsonClassifier": UpdateJsonClassifierRequestTypeDef,
         "CsvClassifier": UpdateCsvClassifierRequestTypeDef,
     },
     total=False,
 )
 
+AmazonRedshiftSourceOutputTypeDef = TypedDict(
+    "AmazonRedshiftSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Data": AmazonRedshiftNodeDataOutputTypeDef,
+    },
+)
+
+AmazonRedshiftTargetOutputTypeDef = TypedDict(
+    "AmazonRedshiftTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Data": AmazonRedshiftNodeDataOutputTypeDef,
+        "Inputs": List[str],
+    },
+)
+
 AmazonRedshiftSourceTypeDef = TypedDict(
     "AmazonRedshiftSourceTypeDef",
     {
         "Name": str,
         "Data": AmazonRedshiftNodeDataTypeDef,
     },
     total=False,
 )
 
 AmazonRedshiftTargetTypeDef = TypedDict(
     "AmazonRedshiftTargetTypeDef",
     {
         "Name": str,
         "Data": AmazonRedshiftNodeDataTypeDef,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
     },
     total=False,
 )
 
-_RequiredPartitionIndexDescriptorTypeDef = TypedDict(
-    "_RequiredPartitionIndexDescriptorTypeDef",
+PartitionIndexDescriptorTypeDef = TypedDict(
+    "PartitionIndexDescriptorTypeDef",
     {
         "IndexName": str,
         "Keys": List[KeySchemaElementTypeDef],
         "IndexStatus": PartitionIndexStatusType,
-    },
-)
-_OptionalPartitionIndexDescriptorTypeDef = TypedDict(
-    "_OptionalPartitionIndexDescriptorTypeDef",
-    {
         "BackfillErrors": List[BackfillErrorTypeDef],
     },
-    total=False,
 )
 
-class PartitionIndexDescriptorTypeDef(
-    _RequiredPartitionIndexDescriptorTypeDef, _OptionalPartitionIndexDescriptorTypeDef
-):
-    pass
-
 BatchStopJobRunResponseTypeDef = TypedDict(
     "BatchStopJobRunResponseTypeDef",
     {
         "SuccessfulSubmissions": List[BatchStopJobRunSuccessfulSubmissionTypeDef],
         "Errors": List[BatchStopJobRunErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7333,33 +9018,33 @@
     {
         "Classifiers": List[ClassifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetDataflowGraphResponseTypeDef = TypedDict(
+    "GetDataflowGraphResponseTypeDef",
+    {
+        "DagNodes": List[CodeGenNodeOutputTypeDef],
+        "DagEdges": List[CodeGenEdgeOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateScriptRequestRequestTypeDef = TypedDict(
     "CreateScriptRequestRequestTypeDef",
     {
         "DagNodes": Sequence[CodeGenNodeTypeDef],
         "DagEdges": Sequence[CodeGenEdgeTypeDef],
         "Language": LanguageType,
     },
     total=False,
 )
 
-GetDataflowGraphResponseTypeDef = TypedDict(
-    "GetDataflowGraphResponseTypeDef",
-    {
-        "DagNodes": List[CodeGenNodeTypeDef],
-        "DagEdges": List[CodeGenEdgeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredGetMappingRequestRequestTypeDef = TypedDict(
     "_RequiredGetMappingRequestRequestTypeDef",
     {
         "Source": CatalogEntryTypeDef,
     },
 )
 _OptionalGetMappingRequestRequestTypeDef = TypedDict(
@@ -7367,19 +9052,21 @@
     {
         "Sinks": Sequence[CatalogEntryTypeDef],
         "Location": LocationTypeDef,
     },
     total=False,
 )
 
+
 class GetMappingRequestRequestTypeDef(
     _RequiredGetMappingRequestRequestTypeDef, _OptionalGetMappingRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPlanRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlanRequestRequestTypeDef",
     {
         "Mapping": Sequence[MappingEntryTypeDef],
         "Source": CatalogEntryTypeDef,
     },
 )
@@ -7390,19 +9077,37 @@
         "Location": LocationTypeDef,
         "Language": LanguageType,
         "AdditionalPlanOptionsMap": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetPlanRequestRequestTypeDef(
     _RequiredGetPlanRequestRequestTypeDef, _OptionalGetPlanRequestRequestTypeDef
 ):
     pass
 
+
+TriggerTypeDef = TypedDict(
+    "TriggerTypeDef",
+    {
+        "Name": str,
+        "WorkflowName": str,
+        "Id": str,
+        "Type": TriggerTypeType,
+        "State": TriggerStateType,
+        "Description": str,
+        "Schedule": str,
+        "Actions": List[ActionOutputTypeDef],
+        "Predicate": PredicateOutputTypeDef,
+        "EventBatchingCondition": EventBatchingConditionOutputTypeDef,
+    },
+)
+
 _RequiredCreateTriggerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTriggerRequestRequestTypeDef",
     {
         "Name": str,
         "Type": TriggerTypeType,
         "Actions": Sequence[ActionTypeDef],
     },
@@ -7417,68 +9122,42 @@
         "StartOnCreation": bool,
         "Tags": Mapping[str, str],
         "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
+
 class CreateTriggerRequestRequestTypeDef(
     _RequiredCreateTriggerRequestRequestTypeDef, _OptionalCreateTriggerRequestRequestTypeDef
 ):
     pass
 
-TriggerTypeDef = TypedDict(
-    "TriggerTypeDef",
-    {
-        "Name": str,
-        "WorkflowName": str,
-        "Id": str,
-        "Type": TriggerTypeType,
-        "State": TriggerStateType,
-        "Description": str,
-        "Schedule": str,
-        "Actions": List[ActionTypeDef],
-        "Predicate": PredicateTypeDef,
-        "EventBatchingCondition": EventBatchingConditionTypeDef,
-    },
-    total=False,
-)
 
 TriggerUpdateTypeDef = TypedDict(
     "TriggerUpdateTypeDef",
     {
         "Name": str,
         "Description": str,
         "Schedule": str,
         "Actions": Sequence[ActionTypeDef],
         "Predicate": PredicateTypeDef,
         "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
-_RequiredEvaluationMetricsTypeDef = TypedDict(
-    "_RequiredEvaluationMetricsTypeDef",
+EvaluationMetricsTypeDef = TypedDict(
+    "EvaluationMetricsTypeDef",
     {
         "TransformType": Literal["FIND_MATCHES"],
-    },
-)
-_OptionalEvaluationMetricsTypeDef = TypedDict(
-    "_OptionalEvaluationMetricsTypeDef",
-    {
         "FindMatchesMetrics": FindMatchesMetricsTypeDef,
     },
-    total=False,
 )
 
-class EvaluationMetricsTypeDef(
-    _RequiredEvaluationMetricsTypeDef, _OptionalEvaluationMetricsTypeDef
-):
-    pass
-
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
 _OptionalCreateConnectionRequestRequestTypeDef = TypedDict(
@@ -7486,19 +9165,21 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectionRequestRequestTypeDef",
     {
         "Name": str,
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
@@ -7506,19 +9187,21 @@
     "_OptionalUpdateConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateConnectionRequestRequestTypeDef(
     _RequiredUpdateConnectionRequestRequestTypeDef, _OptionalUpdateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7533,34 +9216,33 @@
 )
 
 CrawlerTypeDef = TypedDict(
     "CrawlerTypeDef",
     {
         "Name": str,
         "Role": str,
-        "Targets": CrawlerTargetsTypeDef,
+        "Targets": CrawlerTargetsOutputTypeDef,
         "DatabaseName": str,
         "Description": str,
         "Classifiers": List[str],
-        "RecrawlPolicy": RecrawlPolicyTypeDef,
-        "SchemaChangePolicy": SchemaChangePolicyTypeDef,
-        "LineageConfiguration": LineageConfigurationTypeDef,
+        "RecrawlPolicy": RecrawlPolicyOutputTypeDef,
+        "SchemaChangePolicy": SchemaChangePolicyOutputTypeDef,
+        "LineageConfiguration": LineageConfigurationOutputTypeDef,
         "State": CrawlerStateType,
         "TablePrefix": str,
         "Schedule": ScheduleTypeDef,
         "CrawlElapsedTime": int,
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "LastCrawl": LastCrawlInfoTypeDef,
         "Version": int,
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
-        "LakeFormationConfiguration": LakeFormationConfigurationTypeDef,
+        "LakeFormationConfiguration": LakeFormationConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateCrawlerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCrawlerRequestRequestTypeDef",
     {
         "Name": str,
         "Role": str,
@@ -7582,19 +9264,21 @@
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateCrawlerRequestRequestTypeDef(
     _RequiredCreateCrawlerRequestRequestTypeDef, _OptionalCreateCrawlerRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateCrawlerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCrawlerRequestRequestTypeDef = TypedDict(
@@ -7613,92 +9297,44 @@
         "LakeFormationConfiguration": LakeFormationConfigurationTypeDef,
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
     },
     total=False,
 )
 
+
 class UpdateCrawlerRequestRequestTypeDef(
     _RequiredUpdateCrawlerRequestRequestTypeDef, _OptionalUpdateCrawlerRequestRequestTypeDef
 ):
     pass
 
+
 ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
     "ListDataQualityRulesetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filter": DataQualityRulesetFilterCriteriaTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-ListDataQualityRulesetsResponseTypeDef = TypedDict(
-    "ListDataQualityRulesetsResponseTypeDef",
-    {
-        "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DataQualityResultDescriptionTypeDef = TypedDict(
-    "DataQualityResultDescriptionTypeDef",
-    {
-        "ResultId": str,
-        "DataSource": DataSourceTypeDef,
-        "JobName": str,
-        "JobRunId": str,
-        "StartedOn": datetime,
-    },
-    total=False,
-)
-
 DataQualityResultFilterCriteriaTypeDef = TypedDict(
     "DataQualityResultFilterCriteriaTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "JobName": str,
         "JobRunId": str,
         "StartedAfter": Union[datetime, str],
         "StartedBefore": Union[datetime, str],
     },
     total=False,
 )
 
-DataQualityResultTypeDef = TypedDict(
-    "DataQualityResultTypeDef",
-    {
-        "ResultId": str,
-        "Score": float,
-        "DataSource": DataSourceTypeDef,
-        "RulesetName": str,
-        "EvaluationContext": str,
-        "StartedOn": datetime,
-        "CompletedOn": datetime,
-        "JobName": str,
-        "JobRunId": str,
-        "RulesetEvaluationRunId": str,
-        "RuleResults": List[DataQualityRuleResultTypeDef],
-    },
-    total=False,
-)
-
-DataQualityRuleRecommendationRunDescriptionTypeDef = TypedDict(
-    "DataQualityRuleRecommendationRunDescriptionTypeDef",
-    {
-        "RunId": str,
-        "Status": TaskStatusTypeType,
-        "StartedOn": datetime,
-        "DataSource": DataSourceTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
     "_RequiredDataQualityRuleRecommendationRunFilterTypeDef",
     {
         "DataSource": DataSourceTypeDef,
     },
 )
 _OptionalDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
@@ -7706,30 +9342,21 @@
     {
         "StartedBefore": Union[datetime, str],
         "StartedAfter": Union[datetime, str],
     },
     total=False,
 )
 
+
 class DataQualityRuleRecommendationRunFilterTypeDef(
     _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
     _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
 ):
     pass
 
-DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
-    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
-    {
-        "RunId": str,
-        "Status": TaskStatusTypeType,
-        "StartedOn": datetime,
-        "DataSource": DataSourceTypeDef,
-    },
-    total=False,
-)
 
 _RequiredDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
     "_RequiredDataQualityRulesetEvaluationRunFilterTypeDef",
     {
         "DataSource": DataSourceTypeDef,
     },
 )
@@ -7738,79 +9365,21 @@
     {
         "StartedBefore": Union[datetime, str],
         "StartedAfter": Union[datetime, str],
     },
     total=False,
 )
 
+
 class DataQualityRulesetEvaluationRunFilterTypeDef(
     _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
     _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
 ):
     pass
 
-GetDataQualityResultResponseTypeDef = TypedDict(
-    "GetDataQualityResultResponseTypeDef",
-    {
-        "ResultId": str,
-        "Score": float,
-        "DataSource": DataSourceTypeDef,
-        "RulesetName": str,
-        "EvaluationContext": str,
-        "StartedOn": datetime,
-        "CompletedOn": datetime,
-        "JobName": str,
-        "JobRunId": str,
-        "RulesetEvaluationRunId": str,
-        "RuleResults": List[DataQualityRuleResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
-    "GetDataQualityRuleRecommendationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "Status": TaskStatusTypeType,
-        "ErrorString": str,
-        "StartedOn": datetime,
-        "LastModifiedOn": datetime,
-        "CompletedOn": datetime,
-        "ExecutionTime": int,
-        "RecommendedRuleset": str,
-        "CreatedRulesetName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
-    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-        "Status": TaskStatusTypeType,
-        "ErrorString": str,
-        "StartedOn": datetime,
-        "LastModifiedOn": datetime,
-        "CompletedOn": datetime,
-        "ExecutionTime": int,
-        "RulesetNames": List[str],
-        "ResultIds": List[str],
-        "AdditionalDataSources": Dict[str, DataSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Role": str,
     },
@@ -7822,20 +9391,22 @@
         "Timeout": int,
         "CreatedRulesetName": str,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
     _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
     _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Role": str,
         "RulesetNames": Sequence[str],
     },
@@ -7848,50 +9419,26 @@
         "ClientToken": str,
         "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
         "AdditionalDataSources": Mapping[str, DataSourceTypeDef],
     },
     total=False,
 )
 
+
 class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
     _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
 ):
     pass
 
-CreateSessionResponseTypeDef = TypedDict(
-    "CreateSessionResponseTypeDef",
-    {
-        "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListSessionsResponseTypeDef = TypedDict(
-    "ListSessionsResponseTypeDef",
-    {
-        "Ids": List[str],
-        "Sessions": List[SessionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 GetDataCatalogEncryptionSettingsResponseTypeDef = TypedDict(
     "GetDataCatalogEncryptionSettingsResponseTypeDef",
     {
-        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
+        "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
@@ -7902,20 +9449,37 @@
     "_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(
     _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     _OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
 ):
     pass
 
+
+DatabaseTypeDef = TypedDict(
+    "DatabaseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "LocationUri": str,
+        "Parameters": Dict[str, str],
+        "CreateTime": datetime,
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "TargetDatabase": DatabaseIdentifierOutputTypeDef,
+        "CatalogId": str,
+        "FederatedDatabase": FederatedDatabaseOutputTypeDef,
+    },
+)
+
 _RequiredDatabaseInputTypeDef = TypedDict(
     "_RequiredDatabaseInputTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseInputTypeDef = TypedDict(
@@ -7927,60 +9491,181 @@
         "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
         "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
+
 class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
     pass
 
-_RequiredDatabaseTypeDef = TypedDict(
-    "_RequiredDatabaseTypeDef",
+
+ListDataQualityRulesetsResponseTypeDef = TypedDict(
+    "ListDataQualityRulesetsResponseTypeDef",
     {
-        "Name": str,
+        "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDatabaseTypeDef = TypedDict(
-    "_OptionalDatabaseTypeDef",
+
+DataQualityResultDescriptionTypeDef = TypedDict(
+    "DataQualityResultDescriptionTypeDef",
     {
-        "Description": str,
-        "LocationUri": str,
-        "Parameters": Dict[str, str],
-        "CreateTime": datetime,
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
-        "TargetDatabase": DatabaseIdentifierTypeDef,
-        "CatalogId": str,
-        "FederatedDatabase": FederatedDatabaseTypeDef,
+        "ResultId": str,
+        "DataSource": DataSourceOutputTypeDef,
+        "JobName": str,
+        "JobRunId": str,
+        "StartedOn": datetime,
     },
-    total=False,
 )
 
-class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
-    pass
+DataQualityResultTypeDef = TypedDict(
+    "DataQualityResultTypeDef",
+    {
+        "ResultId": str,
+        "Score": float,
+        "DataSource": DataSourceOutputTypeDef,
+        "RulesetName": str,
+        "EvaluationContext": str,
+        "StartedOn": datetime,
+        "CompletedOn": datetime,
+        "JobName": str,
+        "JobRunId": str,
+        "RulesetEvaluationRunId": str,
+        "RuleResults": List[DataQualityRuleResultTypeDef],
+    },
+)
+
+DataQualityRuleRecommendationRunDescriptionTypeDef = TypedDict(
+    "DataQualityRuleRecommendationRunDescriptionTypeDef",
+    {
+        "RunId": str,
+        "Status": TaskStatusTypeType,
+        "StartedOn": datetime,
+        "DataSource": DataSourceOutputTypeDef,
+    },
+)
+
+DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
+    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
+    {
+        "RunId": str,
+        "Status": TaskStatusTypeType,
+        "StartedOn": datetime,
+        "DataSource": DataSourceOutputTypeDef,
+    },
+)
+
+GetDataQualityResultResponseTypeDef = TypedDict(
+    "GetDataQualityResultResponseTypeDef",
+    {
+        "ResultId": str,
+        "Score": float,
+        "DataSource": DataSourceOutputTypeDef,
+        "RulesetName": str,
+        "EvaluationContext": str,
+        "StartedOn": datetime,
+        "CompletedOn": datetime,
+        "JobName": str,
+        "JobRunId": str,
+        "RulesetEvaluationRunId": str,
+        "RuleResults": List[DataQualityRuleResultTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
+    "GetDataQualityRuleRecommendationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "DataSource": DataSourceOutputTypeDef,
+        "Role": str,
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "Status": TaskStatusTypeType,
+        "ErrorString": str,
+        "StartedOn": datetime,
+        "LastModifiedOn": datetime,
+        "CompletedOn": datetime,
+        "ExecutionTime": int,
+        "RecommendedRuleset": str,
+        "CreatedRulesetName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
+    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "DataSource": DataSourceOutputTypeDef,
+        "Role": str,
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef,
+        "Status": TaskStatusTypeType,
+        "ErrorString": str,
+        "StartedOn": datetime,
+        "LastModifiedOn": datetime,
+        "CompletedOn": datetime,
+        "ExecutionTime": int,
+        "RulesetNames": List[str],
+        "ResultIds": List[str],
+        "AdditionalDataSources": Dict[str, DataSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DropNullFieldsOutputTypeDef = TypedDict(
+    "DropNullFieldsOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "NullCheckBoxList": NullCheckBoxListOutputTypeDef,
+        "NullTextList": List[NullValueFieldOutputTypeDef],
+    },
+)
 
 _RequiredDropNullFieldsTypeDef = TypedDict(
     "_RequiredDropNullFieldsTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
     },
 )
 _OptionalDropNullFieldsTypeDef = TypedDict(
     "_OptionalDropNullFieldsTypeDef",
     {
         "NullCheckBoxList": NullCheckBoxListTypeDef,
-        "NullTextList": List[NullValueFieldTypeDef],
+        "NullTextList": Sequence[NullValueFieldTypeDef],
     },
     total=False,
 )
 
+
 class DropNullFieldsTypeDef(_RequiredDropNullFieldsTypeDef, _OptionalDropNullFieldsTypeDef):
     pass
 
+
+ColumnStatisticsDataOutputTypeDef = TypedDict(
+    "ColumnStatisticsDataOutputTypeDef",
+    {
+        "Type": ColumnStatisticsTypeType,
+        "BooleanColumnStatisticsData": BooleanColumnStatisticsDataOutputTypeDef,
+        "DateColumnStatisticsData": DateColumnStatisticsDataOutputTypeDef,
+        "DecimalColumnStatisticsData": DecimalColumnStatisticsDataOutputTypeDef,
+        "DoubleColumnStatisticsData": DoubleColumnStatisticsDataOutputTypeDef,
+        "LongColumnStatisticsData": LongColumnStatisticsDataOutputTypeDef,
+        "StringColumnStatisticsData": StringColumnStatisticsDataOutputTypeDef,
+        "BinaryColumnStatisticsData": BinaryColumnStatisticsDataOutputTypeDef,
+    },
+)
+
 _RequiredColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredColumnStatisticsDataTypeDef",
     {
         "Type": ColumnStatisticsTypeType,
     },
 )
 _OptionalColumnStatisticsDataTypeDef = TypedDict(
@@ -7993,19 +9678,21 @@
         "LongColumnStatisticsData": LongColumnStatisticsDataTypeDef,
         "StringColumnStatisticsData": StringColumnStatisticsDataTypeDef,
         "BinaryColumnStatisticsData": BinaryColumnStatisticsDataTypeDef,
     },
     total=False,
 )
 
+
 class ColumnStatisticsDataTypeDef(
     _RequiredColumnStatisticsDataTypeDef, _OptionalColumnStatisticsDataTypeDef
 ):
     pass
 
+
 StorageDescriptorTypeDef = TypedDict(
     "StorageDescriptorTypeDef",
     {
         "Columns": Sequence[ColumnTypeDef],
         "Location": str,
         "AdditionalLocations": Sequence[str],
         "InputFormat": str,
@@ -8019,47 +9706,56 @@
         "SkewedInfo": SkewedInfoTypeDef,
         "StoredAsSubDirectories": bool,
         "SchemaReference": SchemaReferenceTypeDef,
     },
     total=False,
 )
 
-CreateSecurityConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateSecurityConfigurationRequestRequestTypeDef",
+SecurityConfigurationTypeDef = TypedDict(
+    "SecurityConfigurationTypeDef",
     {
         "Name": str,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+        "CreatedTimeStamp": datetime,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
     },
 )
 
-SecurityConfigurationTypeDef = TypedDict(
-    "SecurityConfigurationTypeDef",
+CreateSecurityConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateSecurityConfigurationRequestRequestTypeDef",
     {
         "Name": str,
-        "CreatedTimeStamp": datetime,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
-    total=False,
 )
 
 DeleteSchemaVersionsResponseTypeDef = TypedDict(
     "DeleteSchemaVersionsResponseTypeDef",
     {
         "SchemaVersionErrors": List[SchemaVersionErrorItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "LogicalOperator": FilterLogicalOperatorType,
+        "Filters": List[FilterExpressionOutputTypeDef],
+    },
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "LogicalOperator": FilterLogicalOperatorType,
-        "Filters": List[FilterExpressionTypeDef],
+        "Filters": Sequence[FilterExpressionTypeDef],
     },
 )
 
 _RequiredUpdateMLTransformRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMLTransformRequestRequestTypeDef",
     {
         "TransformId": str,
@@ -8078,40 +9774,248 @@
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
     },
     total=False,
 )
 
+
 class UpdateMLTransformRequestRequestTypeDef(
     _RequiredUpdateMLTransformRequestRequestTypeDef, _OptionalUpdateMLTransformRequestRequestTypeDef
 ):
     pass
 
-GetMLTransformsRequestRequestTypeDef = TypedDict(
-    "GetMLTransformsRequestRequestTypeDef",
+
+AthenaConnectorSourceOutputTypeDef = TypedDict(
+    "AthenaConnectorSourceOutputTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filter": TransformFilterCriteriaTypeDef,
-        "Sort": TransformSortCriteriaTypeDef,
+        "Name": str,
+        "ConnectionName": str,
+        "ConnectorName": str,
+        "ConnectionType": str,
+        "ConnectionTable": str,
+        "SchemaName": str,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
     },
-    total=False,
 )
 
-ListMLTransformsRequestRequestTypeDef = TypedDict(
-    "ListMLTransformsRequestRequestTypeDef",
+CatalogDeltaSourceOutputTypeDef = TypedDict(
+    "CatalogDeltaSourceOutputTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filter": TransformFilterCriteriaTypeDef,
-        "Sort": TransformSortCriteriaTypeDef,
-        "Tags": Mapping[str, str],
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+CatalogHudiSourceOutputTypeDef = TypedDict(
+    "CatalogHudiSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+CustomCodeOutputTypeDef = TypedDict(
+    "CustomCodeOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Code": str,
+        "ClassName": str,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+DynamicTransformOutputTypeDef = TypedDict(
+    "DynamicTransformOutputTypeDef",
+    {
+        "Name": str,
+        "TransformName": str,
+        "Inputs": List[str],
+        "Parameters": List[TransformConfigParameterOutputTypeDef],
+        "FunctionName": str,
+        "Path": str,
+        "Version": str,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+JDBCConnectorSourceOutputTypeDef = TypedDict(
+    "JDBCConnectorSourceOutputTypeDef",
+    {
+        "Name": str,
+        "ConnectionName": str,
+        "ConnectorName": str,
+        "ConnectionType": str,
+        "AdditionalOptions": JDBCConnectorOptionsOutputTypeDef,
+        "ConnectionTable": str,
+        "Query": str,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+JDBCConnectorTargetOutputTypeDef = TypedDict(
+    "JDBCConnectorTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "ConnectionName": str,
+        "ConnectionTable": str,
+        "ConnectorName": str,
+        "ConnectionType": str,
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3CatalogDeltaSourceOutputTypeDef = TypedDict(
+    "S3CatalogDeltaSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3CatalogHudiSourceOutputTypeDef = TypedDict(
+    "S3CatalogHudiSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3CsvSourceOutputTypeDef = TypedDict(
+    "S3CsvSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+        "CompressionType": CompressionTypeType,
+        "Exclusions": List[str],
+        "GroupSize": str,
+        "GroupFiles": str,
+        "Recurse": bool,
+        "MaxBand": int,
+        "MaxFilesInBand": int,
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsOutputTypeDef,
+        "Separator": SeparatorType,
+        "Escaper": str,
+        "QuoteChar": QuoteCharType,
+        "Multiline": bool,
+        "WithHeader": bool,
+        "WriteHeader": bool,
+        "SkipFirst": bool,
+        "OptimizePerformance": bool,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3DeltaSourceOutputTypeDef = TypedDict(
+    "S3DeltaSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+        "AdditionalDeltaOptions": Dict[str, str],
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsOutputTypeDef,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3HudiSourceOutputTypeDef = TypedDict(
+    "S3HudiSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+        "AdditionalHudiOptions": Dict[str, str],
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsOutputTypeDef,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3JsonSourceOutputTypeDef = TypedDict(
+    "S3JsonSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+        "CompressionType": CompressionTypeType,
+        "Exclusions": List[str],
+        "GroupSize": str,
+        "GroupFiles": str,
+        "Recurse": bool,
+        "MaxBand": int,
+        "MaxFilesInBand": int,
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsOutputTypeDef,
+        "JsonPath": str,
+        "Multiline": bool,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+S3ParquetSourceOutputTypeDef = TypedDict(
+    "S3ParquetSourceOutputTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+        "CompressionType": ParquetCompressionTypeType,
+        "Exclusions": List[str],
+        "GroupSize": str,
+        "GroupFiles": str,
+        "Recurse": bool,
+        "MaxBand": int,
+        "MaxFilesInBand": int,
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsOutputTypeDef,
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+SparkConnectorSourceOutputTypeDef = TypedDict(
+    "SparkConnectorSourceOutputTypeDef",
+    {
+        "Name": str,
+        "ConnectionName": str,
+        "ConnectorName": str,
+        "ConnectionType": str,
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+SparkConnectorTargetOutputTypeDef = TypedDict(
+    "SparkConnectorTargetOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "ConnectionName": str,
+        "ConnectorName": str,
+        "ConnectionType": str,
+        "AdditionalOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
+    },
+)
+
+SparkSQLOutputTypeDef = TypedDict(
+    "SparkSQLOutputTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "SqlQuery": str,
+        "SqlAliases": List[SqlAliasOutputTypeDef],
+        "OutputSchemas": List[GlueSchemaOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredAthenaConnectorSourceTypeDef = TypedDict(
     "_RequiredAthenaConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
@@ -8120,111 +10024,121 @@
         "SchemaName": str,
     },
 )
 _OptionalAthenaConnectorSourceTypeDef = TypedDict(
     "_OptionalAthenaConnectorSourceTypeDef",
     {
         "ConnectionTable": str,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class AthenaConnectorSourceTypeDef(
     _RequiredAthenaConnectorSourceTypeDef, _OptionalAthenaConnectorSourceTypeDef
 ):
     pass
 
+
 _RequiredCatalogDeltaSourceTypeDef = TypedDict(
     "_RequiredCatalogDeltaSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 _OptionalCatalogDeltaSourceTypeDef = TypedDict(
     "_OptionalCatalogDeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalDeltaOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class CatalogDeltaSourceTypeDef(
     _RequiredCatalogDeltaSourceTypeDef, _OptionalCatalogDeltaSourceTypeDef
 ):
     pass
 
+
 _RequiredCatalogHudiSourceTypeDef = TypedDict(
     "_RequiredCatalogHudiSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 _OptionalCatalogHudiSourceTypeDef = TypedDict(
     "_OptionalCatalogHudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalHudiOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class CatalogHudiSourceTypeDef(
     _RequiredCatalogHudiSourceTypeDef, _OptionalCatalogHudiSourceTypeDef
 ):
     pass
 
+
 _RequiredCustomCodeTypeDef = TypedDict(
     "_RequiredCustomCodeTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "Code": str,
         "ClassName": str,
     },
 )
 _OptionalCustomCodeTypeDef = TypedDict(
     "_OptionalCustomCodeTypeDef",
     {
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class CustomCodeTypeDef(_RequiredCustomCodeTypeDef, _OptionalCustomCodeTypeDef):
     pass
 
+
 _RequiredDynamicTransformTypeDef = TypedDict(
     "_RequiredDynamicTransformTypeDef",
     {
         "Name": str,
         "TransformName": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "FunctionName": str,
         "Path": str,
     },
 )
 _OptionalDynamicTransformTypeDef = TypedDict(
     "_OptionalDynamicTransformTypeDef",
     {
-        "Parameters": List[TransformConfigParameterTypeDef],
+        "Parameters": Sequence[TransformConfigParameterTypeDef],
         "Version": str,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class DynamicTransformTypeDef(_RequiredDynamicTransformTypeDef, _OptionalDynamicTransformTypeDef):
     pass
 
+
 _RequiredJDBCConnectorSourceTypeDef = TypedDict(
     "_RequiredJDBCConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -8232,288 +10146,312 @@
 )
 _OptionalJDBCConnectorSourceTypeDef = TypedDict(
     "_OptionalJDBCConnectorSourceTypeDef",
     {
         "AdditionalOptions": JDBCConnectorOptionsTypeDef,
         "ConnectionTable": str,
         "Query": str,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class JDBCConnectorSourceTypeDef(
     _RequiredJDBCConnectorSourceTypeDef, _OptionalJDBCConnectorSourceTypeDef
 ):
     pass
 
+
 _RequiredJDBCConnectorTargetTypeDef = TypedDict(
     "_RequiredJDBCConnectorTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "ConnectionName": str,
         "ConnectionTable": str,
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalJDBCConnectorTargetTypeDef = TypedDict(
     "_OptionalJDBCConnectorTargetTypeDef",
     {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class JDBCConnectorTargetTypeDef(
     _RequiredJDBCConnectorTargetTypeDef, _OptionalJDBCConnectorTargetTypeDef
 ):
     pass
 
+
 _RequiredS3CatalogDeltaSourceTypeDef = TypedDict(
     "_RequiredS3CatalogDeltaSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 _OptionalS3CatalogDeltaSourceTypeDef = TypedDict(
     "_OptionalS3CatalogDeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalDeltaOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3CatalogDeltaSourceTypeDef(
     _RequiredS3CatalogDeltaSourceTypeDef, _OptionalS3CatalogDeltaSourceTypeDef
 ):
     pass
 
+
 _RequiredS3CatalogHudiSourceTypeDef = TypedDict(
     "_RequiredS3CatalogHudiSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
 )
 _OptionalS3CatalogHudiSourceTypeDef = TypedDict(
     "_OptionalS3CatalogHudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalHudiOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3CatalogHudiSourceTypeDef(
     _RequiredS3CatalogHudiSourceTypeDef, _OptionalS3CatalogHudiSourceTypeDef
 ):
     pass
 
+
 _RequiredS3CsvSourceTypeDef = TypedDict(
     "_RequiredS3CsvSourceTypeDef",
     {
         "Name": str,
-        "Paths": List[str],
+        "Paths": Sequence[str],
         "Separator": SeparatorType,
         "QuoteChar": QuoteCharType,
     },
 )
 _OptionalS3CsvSourceTypeDef = TypedDict(
     "_OptionalS3CsvSourceTypeDef",
     {
         "CompressionType": CompressionTypeType,
-        "Exclusions": List[str],
+        "Exclusions": Sequence[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "Escaper": str,
         "Multiline": bool,
         "WithHeader": bool,
         "WriteHeader": bool,
         "SkipFirst": bool,
         "OptimizePerformance": bool,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
     pass
 
+
 _RequiredS3DeltaSourceTypeDef = TypedDict(
     "_RequiredS3DeltaSourceTypeDef",
     {
         "Name": str,
-        "Paths": List[str],
+        "Paths": Sequence[str],
     },
 )
 _OptionalS3DeltaSourceTypeDef = TypedDict(
     "_OptionalS3DeltaSourceTypeDef",
     {
-        "AdditionalDeltaOptions": Dict[str, str],
+        "AdditionalDeltaOptions": Mapping[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3DeltaSourceTypeDef(_RequiredS3DeltaSourceTypeDef, _OptionalS3DeltaSourceTypeDef):
     pass
 
+
 _RequiredS3HudiSourceTypeDef = TypedDict(
     "_RequiredS3HudiSourceTypeDef",
     {
         "Name": str,
-        "Paths": List[str],
+        "Paths": Sequence[str],
     },
 )
 _OptionalS3HudiSourceTypeDef = TypedDict(
     "_OptionalS3HudiSourceTypeDef",
     {
-        "AdditionalHudiOptions": Dict[str, str],
+        "AdditionalHudiOptions": Mapping[str, str],
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3HudiSourceTypeDef(_RequiredS3HudiSourceTypeDef, _OptionalS3HudiSourceTypeDef):
     pass
 
+
 _RequiredS3JsonSourceTypeDef = TypedDict(
     "_RequiredS3JsonSourceTypeDef",
     {
         "Name": str,
-        "Paths": List[str],
+        "Paths": Sequence[str],
     },
 )
 _OptionalS3JsonSourceTypeDef = TypedDict(
     "_OptionalS3JsonSourceTypeDef",
     {
         "CompressionType": CompressionTypeType,
-        "Exclusions": List[str],
+        "Exclusions": Sequence[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "JsonPath": str,
         "Multiline": bool,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3JsonSourceTypeDef(_RequiredS3JsonSourceTypeDef, _OptionalS3JsonSourceTypeDef):
     pass
 
+
 _RequiredS3ParquetSourceTypeDef = TypedDict(
     "_RequiredS3ParquetSourceTypeDef",
     {
         "Name": str,
-        "Paths": List[str],
+        "Paths": Sequence[str],
     },
 )
 _OptionalS3ParquetSourceTypeDef = TypedDict(
     "_OptionalS3ParquetSourceTypeDef",
     {
         "CompressionType": ParquetCompressionTypeType,
-        "Exclusions": List[str],
+        "Exclusions": Sequence[str],
         "GroupSize": str,
         "GroupFiles": str,
         "Recurse": bool,
         "MaxBand": int,
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3ParquetSourceTypeDef(_RequiredS3ParquetSourceTypeDef, _OptionalS3ParquetSourceTypeDef):
     pass
 
+
 _RequiredSparkConnectorSourceTypeDef = TypedDict(
     "_RequiredSparkConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalSparkConnectorSourceTypeDef = TypedDict(
     "_OptionalSparkConnectorSourceTypeDef",
     {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class SparkConnectorSourceTypeDef(
     _RequiredSparkConnectorSourceTypeDef, _OptionalSparkConnectorSourceTypeDef
 ):
     pass
 
+
 _RequiredSparkConnectorTargetTypeDef = TypedDict(
     "_RequiredSparkConnectorTargetTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
     },
 )
 _OptionalSparkConnectorTargetTypeDef = TypedDict(
     "_OptionalSparkConnectorTargetTypeDef",
     {
-        "AdditionalOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "AdditionalOptions": Mapping[str, str],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class SparkConnectorTargetTypeDef(
     _RequiredSparkConnectorTargetTypeDef, _OptionalSparkConnectorTargetTypeDef
 ):
     pass
 
+
 _RequiredSparkSQLTypeDef = TypedDict(
     "_RequiredSparkSQLTypeDef",
     {
         "Name": str,
-        "Inputs": List[str],
+        "Inputs": Sequence[str],
         "SqlQuery": str,
-        "SqlAliases": List[SqlAliasTypeDef],
+        "SqlAliases": Sequence[SqlAliasTypeDef],
     },
 )
 _OptionalSparkSQLTypeDef = TypedDict(
     "_OptionalSparkSQLTypeDef",
     {
-        "OutputSchemas": List[GlueSchemaTypeDef],
+        "OutputSchemas": Sequence[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class SparkSQLTypeDef(_RequiredSparkSQLTypeDef, _OptionalSparkSQLTypeDef):
     pass
 
+
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "JobRun": JobRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8528,15 +10466,14 @@
 )
 
 JobNodeDetailsTypeDef = TypedDict(
     "JobNodeDetailsTypeDef",
     {
         "JobRuns": List[JobRunTypeDef],
     },
-    total=False,
 )
 
 GetMLTaskRunResponseTypeDef = TypedDict(
     "GetMLTaskRunResponseTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
@@ -8562,15 +10499,14 @@
         "Properties": TaskRunPropertiesTypeDef,
         "ErrorString": str,
         "StartedOn": datetime,
         "LastModifiedOn": datetime,
         "CompletedOn": datetime,
         "ExecutionTime": int,
     },
-    total=False,
 )
 
 _RequiredCreateMLTransformRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMLTransformRequestRequestTypeDef",
     {
         "Name": str,
         "InputRecordTables": Sequence[GlueTableTypeDef],
@@ -8590,29 +10526,48 @@
         "MaxRetries": int,
         "Tags": Mapping[str, str],
         "TransformEncryption": TransformEncryptionTypeDef,
     },
     total=False,
 )
 
+
 class CreateMLTransformRequestRequestTypeDef(
     _RequiredCreateMLTransformRequestRequestTypeDef, _OptionalCreateMLTransformRequestRequestTypeDef
 ):
     pass
 
+
 QuerySchemaVersionMetadataResponseTypeDef = TypedDict(
     "QuerySchemaVersionMetadataResponseTypeDef",
     {
         "MetadataInfoMap": Dict[str, MetadataInfoTypeDef],
         "SchemaVersionId": str,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetUserDefinedFunctionResponseTypeDef = TypedDict(
+    "GetUserDefinedFunctionResponseTypeDef",
+    {
+        "UserDefinedFunction": UserDefinedFunctionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUserDefinedFunctionsResponseTypeDef = TypedDict(
+    "GetUserDefinedFunctionsResponseTypeDef",
+    {
+        "UserDefinedFunctions": List[UserDefinedFunctionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionInput": UserDefinedFunctionInputTypeDef,
     },
 )
@@ -8620,20 +10575,22 @@
     "_OptionalCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class CreateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredCreateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalCreateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionName": str,
         "FunctionInput": UserDefinedFunctionInputTypeDef,
     },
@@ -8642,32 +10599,86 @@
     "_OptionalUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalUpdateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-GetUserDefinedFunctionResponseTypeDef = TypedDict(
-    "GetUserDefinedFunctionResponseTypeDef",
+
+GetMLTransformsRequestRequestTypeDef = TypedDict(
+    "GetMLTransformsRequestRequestTypeDef",
     {
-        "UserDefinedFunction": UserDefinedFunctionTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "Filter": TransformFilterCriteriaTypeDef,
+        "Sort": TransformSortCriteriaTypeDef,
+    },
+    total=False,
+)
+
+ListMLTransformsRequestRequestTypeDef = TypedDict(
+    "ListMLTransformsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "Filter": TransformFilterCriteriaTypeDef,
+        "Sort": TransformSortCriteriaTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+StorageDescriptorOutputTypeDef = TypedDict(
+    "StorageDescriptorOutputTypeDef",
+    {
+        "Columns": List[ColumnOutputTypeDef],
+        "Location": str,
+        "AdditionalLocations": List[str],
+        "InputFormat": str,
+        "OutputFormat": str,
+        "Compressed": bool,
+        "NumberOfBuckets": int,
+        "SerdeInfo": SerDeInfoOutputTypeDef,
+        "BucketColumns": List[str],
+        "SortColumns": List[OrderOutputTypeDef],
+        "Parameters": Dict[str, str],
+        "SkewedInfo": SkewedInfoOutputTypeDef,
+        "StoredAsSubDirectories": bool,
+        "SchemaReference": SchemaReferenceOutputTypeDef,
+    },
+)
+
+CreateSessionResponseTypeDef = TypedDict(
+    "CreateSessionResponseTypeDef",
+    {
+        "Session": SessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetUserDefinedFunctionsResponseTypeDef = TypedDict(
-    "GetUserDefinedFunctionsResponseTypeDef",
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
     {
-        "UserDefinedFunctions": List[UserDefinedFunctionTypeDef],
+        "Session": SessionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSessionsResponseTypeDef = TypedDict(
+    "ListSessionsResponseTypeDef",
+    {
+        "Ids": List[str],
+        "Sessions": List[SessionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StatementTypeDef = TypedDict(
     "StatementTypeDef",
@@ -8676,15 +10687,14 @@
         "Code": str,
         "State": StatementStateType,
         "Output": StatementOutputTypeDef,
         "Progress": float,
         "StartedOn": int,
         "CompletedOn": int,
     },
-    total=False,
 )
 
 GetPartitionIndexesResponseTypeDef = TypedDict(
     "GetPartitionIndexesResponseTypeDef",
     {
         "PartitionIndexDescriptorList": List[PartitionIndexDescriptorTypeDef],
         "NextToken": str,
@@ -8719,15 +10729,14 @@
 )
 
 TriggerNodeDetailsTypeDef = TypedDict(
     "TriggerNodeDetailsTypeDef",
     {
         "Trigger": TriggerTypeDef,
     },
-    total=False,
 )
 
 UpdateTriggerResponseTypeDef = TypedDict(
     "UpdateTriggerResponseTypeDef",
     {
         "Trigger": TriggerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -8747,55 +10756,54 @@
     {
         "TransformId": str,
         "Name": str,
         "Description": str,
         "Status": TransformStatusTypeType,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
-        "InputRecordTables": List[GlueTableTypeDef],
-        "Parameters": TransformParametersTypeDef,
+        "InputRecordTables": List[GlueTableOutputTypeDef],
+        "Parameters": TransformParametersOutputTypeDef,
         "EvaluationMetrics": EvaluationMetricsTypeDef,
         "LabelCount": int,
-        "Schema": List[SchemaColumnTypeDef],
+        "Schema": List[SchemaColumnOutputTypeDef],
         "Role": str,
         "GlueVersion": str,
         "MaxCapacity": float,
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
-        "TransformEncryption": TransformEncryptionTypeDef,
+        "TransformEncryption": TransformEncryptionOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MLTransformTypeDef = TypedDict(
     "MLTransformTypeDef",
     {
         "TransformId": str,
         "Name": str,
         "Description": str,
         "Status": TransformStatusTypeType,
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
-        "InputRecordTables": List[GlueTableTypeDef],
-        "Parameters": TransformParametersTypeDef,
+        "InputRecordTables": List[GlueTableOutputTypeDef],
+        "Parameters": TransformParametersOutputTypeDef,
         "EvaluationMetrics": EvaluationMetricsTypeDef,
         "LabelCount": int,
-        "Schema": List[SchemaColumnTypeDef],
+        "Schema": List[SchemaColumnOutputTypeDef],
         "Role": str,
         "GlueVersion": str,
         "MaxCapacity": float,
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
-        "TransformEncryption": TransformEncryptionTypeDef,
+        "TransformEncryption": TransformEncryptionOutputTypeDef,
     },
-    total=False,
 )
 
 BatchGetCrawlersResponseTypeDef = TypedDict(
     "BatchGetCrawlersResponseTypeDef",
     {
         "Crawlers": List[CrawlerTypeDef],
         "CrawlersNotFound": List[str],
@@ -8816,78 +10824,59 @@
     {
         "Crawlers": List[CrawlerTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDataQualityResultsResponseTypeDef = TypedDict(
-    "ListDataQualityResultsResponseTypeDef",
-    {
-        "Results": List[DataQualityResultDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListDataQualityResultsRequestRequestTypeDef = TypedDict(
     "ListDataQualityResultsRequestRequestTypeDef",
     {
         "Filter": DataQualityResultFilterCriteriaTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-BatchGetDataQualityResultResponseTypeDef = TypedDict(
-    "BatchGetDataQualityResultResponseTypeDef",
-    {
-        "Results": List[DataQualityResultTypeDef],
-        "ResultsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityRuleRecommendationRunsResponseTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
     {
-        "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
+        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxResults": int,
     },
+    total=False,
 )
 
-ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
     {
-        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
+        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+GetDatabaseResponseTypeDef = TypedDict(
+    "GetDatabaseResponseTypeDef",
     {
-        "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
-        "NextToken": str,
+        "Database": DatabaseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
+GetDatabasesResponseTypeDef = TypedDict(
+    "GetDatabasesResponseTypeDef",
     {
-        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
+        "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
-        "MaxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseInput": DatabaseInputTypeDef,
     },
@@ -8897,19 +10886,21 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatabaseRequestRequestTypeDef",
     {
         "Name": str,
         "DatabaseInput": DatabaseInputTypeDef,
     },
 )
@@ -8917,42 +10908,73 @@
     "_OptionalUpdateDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateDatabaseRequestRequestTypeDef(
     _RequiredUpdateDatabaseRequestRequestTypeDef, _OptionalUpdateDatabaseRequestRequestTypeDef
 ):
     pass
 
-GetDatabaseResponseTypeDef = TypedDict(
-    "GetDatabaseResponseTypeDef",
+
+ListDataQualityResultsResponseTypeDef = TypedDict(
+    "ListDataQualityResultsResponseTypeDef",
     {
-        "Database": DatabaseTypeDef,
+        "Results": List[DataQualityResultDescriptionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDatabasesResponseTypeDef = TypedDict(
-    "GetDatabasesResponseTypeDef",
+BatchGetDataQualityResultResponseTypeDef = TypedDict(
+    "BatchGetDataQualityResultResponseTypeDef",
     {
-        "DatabaseList": List[DatabaseTypeDef],
+        "Results": List[DataQualityResultTypeDef],
+        "ResultsNotFound": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDataQualityRuleRecommendationRunsResponseTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+    {
+        "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+    {
+        "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ColumnStatisticsOutputTypeDef = TypedDict(
+    "ColumnStatisticsOutputTypeDef",
+    {
+        "ColumnName": str,
+        "ColumnType": str,
+        "AnalyzedTime": datetime,
+        "StatisticsData": ColumnStatisticsDataOutputTypeDef,
+    },
+)
+
 ColumnStatisticsTypeDef = TypedDict(
     "ColumnStatisticsTypeDef",
     {
         "ColumnName": str,
         "ColumnType": str,
-        "AnalyzedTime": datetime,
+        "AnalyzedTime": Union[datetime, str],
         "StatisticsData": ColumnStatisticsDataTypeDef,
     },
 )
 
 PartitionInputTypeDef = TypedDict(
     "PartitionInputTypeDef",
     {
@@ -8961,30 +10983,14 @@
         "StorageDescriptor": StorageDescriptorTypeDef,
         "Parameters": Mapping[str, str],
         "LastAnalyzedTime": Union[datetime, str],
     },
     total=False,
 )
 
-PartitionTypeDef = TypedDict(
-    "PartitionTypeDef",
-    {
-        "Values": List[str],
-        "DatabaseName": str,
-        "TableName": str,
-        "CreationTime": datetime,
-        "LastAccessTime": datetime,
-        "StorageDescriptor": StorageDescriptorTypeDef,
-        "Parameters": Dict[str, str],
-        "LastAnalyzedTime": datetime,
-        "CatalogId": str,
-    },
-    total=False,
-)
-
 _RequiredTableInputTypeDef = TypedDict(
     "_RequiredTableInputTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalTableInputTypeDef = TypedDict(
@@ -9002,52 +11008,18 @@
         "TableType": str,
         "Parameters": Mapping[str, str],
         "TargetTable": TableIdentifierTypeDef,
     },
     total=False,
 )
 
+
 class TableInputTypeDef(_RequiredTableInputTypeDef, _OptionalTableInputTypeDef):
     pass
 
-_RequiredTableTypeDef = TypedDict(
-    "_RequiredTableTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalTableTypeDef = TypedDict(
-    "_OptionalTableTypeDef",
-    {
-        "DatabaseName": str,
-        "Description": str,
-        "Owner": str,
-        "CreateTime": datetime,
-        "UpdateTime": datetime,
-        "LastAccessTime": datetime,
-        "LastAnalyzedTime": datetime,
-        "Retention": int,
-        "StorageDescriptor": StorageDescriptorTypeDef,
-        "PartitionKeys": List[ColumnTypeDef],
-        "ViewOriginalText": str,
-        "ViewExpandedText": str,
-        "TableType": str,
-        "Parameters": Dict[str, str],
-        "CreatedBy": str,
-        "IsRegisteredWithLakeFormation": bool,
-        "TargetTable": TableIdentifierTypeDef,
-        "CatalogId": str,
-        "VersionId": str,
-        "FederatedTable": FederatedTableTypeDef,
-    },
-    total=False,
-)
-
-class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
-    pass
 
 GetSecurityConfigurationResponseTypeDef = TypedDict(
     "GetSecurityConfigurationResponseTypeDef",
     {
         "SecurityConfiguration": SecurityConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -9058,14 +11030,86 @@
     {
         "SecurityConfigurations": List[SecurityConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CodeGenConfigurationNodeOutputTypeDef = TypedDict(
+    "CodeGenConfigurationNodeOutputTypeDef",
+    {
+        "AthenaConnectorSource": AthenaConnectorSourceOutputTypeDef,
+        "JDBCConnectorSource": JDBCConnectorSourceOutputTypeDef,
+        "SparkConnectorSource": SparkConnectorSourceOutputTypeDef,
+        "CatalogSource": CatalogSourceOutputTypeDef,
+        "RedshiftSource": RedshiftSourceOutputTypeDef,
+        "S3CatalogSource": S3CatalogSourceOutputTypeDef,
+        "S3CsvSource": S3CsvSourceOutputTypeDef,
+        "S3JsonSource": S3JsonSourceOutputTypeDef,
+        "S3ParquetSource": S3ParquetSourceOutputTypeDef,
+        "RelationalCatalogSource": RelationalCatalogSourceOutputTypeDef,
+        "DynamoDBCatalogSource": DynamoDBCatalogSourceOutputTypeDef,
+        "JDBCConnectorTarget": JDBCConnectorTargetOutputTypeDef,
+        "SparkConnectorTarget": SparkConnectorTargetOutputTypeDef,
+        "CatalogTarget": BasicCatalogTargetOutputTypeDef,
+        "RedshiftTarget": RedshiftTargetOutputTypeDef,
+        "S3CatalogTarget": S3CatalogTargetOutputTypeDef,
+        "S3GlueParquetTarget": S3GlueParquetTargetOutputTypeDef,
+        "S3DirectTarget": S3DirectTargetOutputTypeDef,
+        "ApplyMapping": ApplyMappingOutputTypeDef,
+        "SelectFields": SelectFieldsOutputTypeDef,
+        "DropFields": DropFieldsOutputTypeDef,
+        "RenameField": RenameFieldOutputTypeDef,
+        "Spigot": SpigotOutputTypeDef,
+        "Join": JoinOutputTypeDef,
+        "SplitFields": SplitFieldsOutputTypeDef,
+        "SelectFromCollection": SelectFromCollectionOutputTypeDef,
+        "FillMissingValues": FillMissingValuesOutputTypeDef,
+        "Filter": FilterOutputTypeDef,
+        "CustomCode": CustomCodeOutputTypeDef,
+        "SparkSQL": SparkSQLOutputTypeDef,
+        "DirectKinesisSource": DirectKinesisSourceOutputTypeDef,
+        "DirectKafkaSource": DirectKafkaSourceOutputTypeDef,
+        "CatalogKinesisSource": CatalogKinesisSourceOutputTypeDef,
+        "CatalogKafkaSource": CatalogKafkaSourceOutputTypeDef,
+        "DropNullFields": DropNullFieldsOutputTypeDef,
+        "Merge": MergeOutputTypeDef,
+        "Union": UnionOutputTypeDef,
+        "PIIDetection": PIIDetectionOutputTypeDef,
+        "Aggregate": AggregateOutputTypeDef,
+        "DropDuplicates": DropDuplicatesOutputTypeDef,
+        "GovernedCatalogTarget": GovernedCatalogTargetOutputTypeDef,
+        "GovernedCatalogSource": GovernedCatalogSourceOutputTypeDef,
+        "MicrosoftSQLServerCatalogSource": MicrosoftSQLServerCatalogSourceOutputTypeDef,
+        "MySQLCatalogSource": MySQLCatalogSourceOutputTypeDef,
+        "OracleSQLCatalogSource": OracleSQLCatalogSourceOutputTypeDef,
+        "PostgreSQLCatalogSource": PostgreSQLCatalogSourceOutputTypeDef,
+        "MicrosoftSQLServerCatalogTarget": MicrosoftSQLServerCatalogTargetOutputTypeDef,
+        "MySQLCatalogTarget": MySQLCatalogTargetOutputTypeDef,
+        "OracleSQLCatalogTarget": OracleSQLCatalogTargetOutputTypeDef,
+        "PostgreSQLCatalogTarget": PostgreSQLCatalogTargetOutputTypeDef,
+        "DynamicTransform": DynamicTransformOutputTypeDef,
+        "EvaluateDataQuality": EvaluateDataQualityOutputTypeDef,
+        "S3CatalogHudiSource": S3CatalogHudiSourceOutputTypeDef,
+        "CatalogHudiSource": CatalogHudiSourceOutputTypeDef,
+        "S3HudiSource": S3HudiSourceOutputTypeDef,
+        "S3HudiCatalogTarget": S3HudiCatalogTargetOutputTypeDef,
+        "S3HudiDirectTarget": S3HudiDirectTargetOutputTypeDef,
+        "DirectJDBCSource": DirectJDBCSourceOutputTypeDef,
+        "S3CatalogDeltaSource": S3CatalogDeltaSourceOutputTypeDef,
+        "CatalogDeltaSource": CatalogDeltaSourceOutputTypeDef,
+        "S3DeltaSource": S3DeltaSourceOutputTypeDef,
+        "S3DeltaCatalogTarget": S3DeltaCatalogTargetOutputTypeDef,
+        "S3DeltaDirectTarget": S3DeltaDirectTargetOutputTypeDef,
+        "AmazonRedshiftSource": AmazonRedshiftSourceOutputTypeDef,
+        "AmazonRedshiftTarget": AmazonRedshiftTargetOutputTypeDef,
+        "EvaluateDataQualityMultiFrame": EvaluateDataQualityMultiFrameOutputTypeDef,
+    },
+)
+
 CodeGenConfigurationNodeTypeDef = TypedDict(
     "CodeGenConfigurationNodeTypeDef",
     {
         "AthenaConnectorSource": AthenaConnectorSourceTypeDef,
         "JDBCConnectorSource": JDBCConnectorSourceTypeDef,
         "SparkConnectorSource": SparkConnectorSourceTypeDef,
         "CatalogSource": CatalogSourceTypeDef,
@@ -9140,14 +11184,56 @@
     {
         "TaskRuns": List[TaskRunTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PartitionTypeDef = TypedDict(
+    "PartitionTypeDef",
+    {
+        "Values": List[str],
+        "DatabaseName": str,
+        "TableName": str,
+        "CreationTime": datetime,
+        "LastAccessTime": datetime,
+        "StorageDescriptor": StorageDescriptorOutputTypeDef,
+        "Parameters": Dict[str, str],
+        "LastAnalyzedTime": datetime,
+        "CatalogId": str,
+    },
+)
+
+TableTypeDef = TypedDict(
+    "TableTypeDef",
+    {
+        "Name": str,
+        "DatabaseName": str,
+        "Description": str,
+        "Owner": str,
+        "CreateTime": datetime,
+        "UpdateTime": datetime,
+        "LastAccessTime": datetime,
+        "LastAnalyzedTime": datetime,
+        "Retention": int,
+        "StorageDescriptor": StorageDescriptorOutputTypeDef,
+        "PartitionKeys": List[ColumnOutputTypeDef],
+        "ViewOriginalText": str,
+        "ViewExpandedText": str,
+        "TableType": str,
+        "Parameters": Dict[str, str],
+        "CreatedBy": str,
+        "IsRegisteredWithLakeFormation": bool,
+        "TargetTable": TableIdentifierOutputTypeDef,
+        "CatalogId": str,
+        "VersionId": str,
+        "FederatedTable": FederatedTableTypeDef,
+    },
+)
+
 GetStatementResponseTypeDef = TypedDict(
     "GetStatementResponseTypeDef",
     {
         "Statement": StatementTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9167,48 +11253,46 @@
         "Type": NodeTypeType,
         "Name": str,
         "UniqueId": str,
         "TriggerDetails": TriggerNodeDetailsTypeDef,
         "JobDetails": JobNodeDetailsTypeDef,
         "CrawlerDetails": CrawlerNodeDetailsTypeDef,
     },
-    total=False,
 )
 
 GetMLTransformsResponseTypeDef = TypedDict(
     "GetMLTransformsResponseTypeDef",
     {
         "Transforms": List[MLTransformTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ColumnStatisticsErrorTypeDef = TypedDict(
     "ColumnStatisticsErrorTypeDef",
     {
-        "ColumnStatistics": ColumnStatisticsTypeDef,
+        "ColumnStatistics": ColumnStatisticsOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 GetColumnStatisticsForPartitionResponseTypeDef = TypedDict(
     "GetColumnStatisticsForPartitionResponseTypeDef",
     {
-        "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
+        "ColumnStatisticsList": List[ColumnStatisticsOutputTypeDef],
         "Errors": List[ColumnErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetColumnStatisticsForTableResponseTypeDef = TypedDict(
     "GetColumnStatisticsForTableResponseTypeDef",
     {
-        "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
+        "ColumnStatisticsList": List[ColumnStatisticsOutputTypeDef],
         "Errors": List[ColumnErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
@@ -9223,20 +11307,22 @@
     "_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnStatisticsList": Sequence[ColumnStatisticsTypeDef],
     },
@@ -9245,20 +11331,22 @@
     "_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchCreatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionInputList": Sequence[PartitionInputTypeDef],
     },
@@ -9267,20 +11355,22 @@
     "_OptionalBatchCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchCreatePartitionRequestRequestTypeDef(
     _RequiredBatchCreatePartitionRequestRequestTypeDef,
     _OptionalBatchCreatePartitionRequestRequestTypeDef,
 ):
     pass
 
+
 BatchUpdatePartitionRequestEntryTypeDef = TypedDict(
     "BatchUpdatePartitionRequestEntryTypeDef",
     {
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
     },
 )
@@ -9297,19 +11387,21 @@
     "_OptionalCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class CreatePartitionRequestRequestTypeDef(
     _RequiredCreatePartitionRequestRequestTypeDef, _OptionalCreatePartitionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
@@ -9319,64 +11411,20 @@
     "_OptionalUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdatePartitionRequestRequestTypeDef(
     _RequiredUpdatePartitionRequestRequestTypeDef, _OptionalUpdatePartitionRequestRequestTypeDef
 ):
     pass
 
-BatchGetPartitionResponseTypeDef = TypedDict(
-    "BatchGetPartitionResponseTypeDef",
-    {
-        "Partitions": List[PartitionTypeDef],
-        "UnprocessedKeys": List[PartitionValueListTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPartitionResponseTypeDef = TypedDict(
-    "GetPartitionResponseTypeDef",
-    {
-        "Partition": PartitionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPartitionsResponseTypeDef = TypedDict(
-    "GetPartitionsResponseTypeDef",
-    {
-        "Partitions": List[PartitionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUnfilteredPartitionMetadataResponseTypeDef = TypedDict(
-    "GetUnfilteredPartitionMetadataResponseTypeDef",
-    {
-        "Partition": PartitionTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UnfilteredPartitionTypeDef = TypedDict(
-    "UnfilteredPartitionTypeDef",
-    {
-        "Partition": PartitionTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-    },
-    total=False,
-)
 
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableInput": TableInputTypeDef,
     },
@@ -9388,19 +11436,21 @@
         "PartitionIndexes": Sequence[PartitionIndexTypeDef],
         "TransactionId": str,
         "OpenTableFormatInput": OpenTableFormatInputTypeDef,
     },
     total=False,
 )
 
+
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableInput": TableInputTypeDef,
     },
 )
@@ -9411,63 +11461,48 @@
         "SkipArchive": bool,
         "TransactionId": str,
         "VersionId": str,
     },
     total=False,
 )
 
+
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
-GetTableResponseTypeDef = TypedDict(
-    "GetTableResponseTypeDef",
-    {
-        "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTablesResponseTypeDef = TypedDict(
-    "GetTablesResponseTypeDef",
-    {
-        "TableList": List[TableTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetUnfilteredTableMetadataResponseTypeDef = TypedDict(
-    "GetUnfilteredTableMetadataResponseTypeDef",
-    {
-        "Table": TableTypeDef,
-        "AuthorizedColumns": List[str],
-        "IsRegisteredWithLakeFormation": bool,
-        "CellFilters": List[ColumnRowFilterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-SearchTablesResponseTypeDef = TypedDict(
-    "SearchTablesResponseTypeDef",
-    {
-        "NextToken": str,
-        "TableList": List[TableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TableVersionTypeDef = TypedDict(
-    "TableVersionTypeDef",
+JobTypeDef = TypedDict(
+    "JobTypeDef",
     {
-        "Table": TableTypeDef,
-        "VersionId": str,
+        "Name": str,
+        "Description": str,
+        "LogUri": str,
+        "Role": str,
+        "CreatedOn": datetime,
+        "LastModifiedOn": datetime,
+        "ExecutionProperty": ExecutionPropertyOutputTypeDef,
+        "Command": JobCommandOutputTypeDef,
+        "DefaultArguments": Dict[str, str],
+        "NonOverridableArguments": Dict[str, str],
+        "Connections": ConnectionsListOutputTypeDef,
+        "MaxRetries": int,
+        "AllocatedCapacity": int,
+        "Timeout": int,
+        "MaxCapacity": float,
+        "WorkerType": WorkerTypeType,
+        "NumberOfWorkers": int,
+        "SecurityConfiguration": str,
+        "NotificationProperty": NotificationPropertyOutputTypeDef,
+        "GlueVersion": str,
+        "CodeGenConfigurationNodes": Dict[str, CodeGenConfigurationNodeOutputTypeDef],
+        "ExecutionClass": ExecutionClassType,
+        "SourceControlDetails": SourceControlDetailsOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "Name": str,
         "Role": str,
@@ -9496,48 +11531,20 @@
         "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
+
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-JobTypeDef = TypedDict(
-    "JobTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "LogUri": str,
-        "Role": str,
-        "CreatedOn": datetime,
-        "LastModifiedOn": datetime,
-        "ExecutionProperty": ExecutionPropertyTypeDef,
-        "Command": JobCommandTypeDef,
-        "DefaultArguments": Dict[str, str],
-        "NonOverridableArguments": Dict[str, str],
-        "Connections": ConnectionsListTypeDef,
-        "MaxRetries": int,
-        "AllocatedCapacity": int,
-        "Timeout": int,
-        "MaxCapacity": float,
-        "WorkerType": WorkerTypeType,
-        "NumberOfWorkers": int,
-        "SecurityConfiguration": str,
-        "NotificationProperty": NotificationPropertyTypeDef,
-        "GlueVersion": str,
-        "CodeGenConfigurationNodes": Dict[str, CodeGenConfigurationNodeTypeDef],
-        "ExecutionClass": ExecutionClassType,
-        "SourceControlDetails": SourceControlDetailsTypeDef,
-    },
-    total=False,
-)
 
 JobUpdateTypeDef = TypedDict(
     "JobUpdateTypeDef",
     {
         "Description": str,
         "LogUri": str,
         "Role": str,
@@ -9558,21 +11565,110 @@
         "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
+BatchGetPartitionResponseTypeDef = TypedDict(
+    "BatchGetPartitionResponseTypeDef",
+    {
+        "Partitions": List[PartitionTypeDef],
+        "UnprocessedKeys": List[PartitionValueListOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPartitionResponseTypeDef = TypedDict(
+    "GetPartitionResponseTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPartitionsResponseTypeDef = TypedDict(
+    "GetPartitionsResponseTypeDef",
+    {
+        "Partitions": List[PartitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUnfilteredPartitionMetadataResponseTypeDef = TypedDict(
+    "GetUnfilteredPartitionMetadataResponseTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnfilteredPartitionTypeDef = TypedDict(
+    "UnfilteredPartitionTypeDef",
+    {
+        "Partition": PartitionTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+    },
+)
+
+GetTableResponseTypeDef = TypedDict(
+    "GetTableResponseTypeDef",
+    {
+        "Table": TableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTablesResponseTypeDef = TypedDict(
+    "GetTablesResponseTypeDef",
+    {
+        "TableList": List[TableTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUnfilteredTableMetadataResponseTypeDef = TypedDict(
+    "GetUnfilteredTableMetadataResponseTypeDef",
+    {
+        "Table": TableTypeDef,
+        "AuthorizedColumns": List[str],
+        "IsRegisteredWithLakeFormation": bool,
+        "CellFilters": List[ColumnRowFilterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchTablesResponseTypeDef = TypedDict(
+    "SearchTablesResponseTypeDef",
+    {
+        "NextToken": str,
+        "TableList": List[TableTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TableVersionTypeDef = TypedDict(
+    "TableVersionTypeDef",
+    {
+        "Table": TableTypeDef,
+        "VersionId": str,
+    },
+)
+
 WorkflowGraphTypeDef = TypedDict(
     "WorkflowGraphTypeDef",
     {
         "Nodes": List[NodeTypeDef],
         "Edges": List[EdgeTypeDef],
     },
-    total=False,
 )
 
 UpdateColumnStatisticsForPartitionResponseTypeDef = TypedDict(
     "UpdateColumnStatisticsForPartitionResponseTypeDef",
     {
         "Errors": List[ColumnStatisticsErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -9599,45 +11695,21 @@
     "_OptionalBatchUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchUpdatePartitionRequestRequestTypeDef(
     _RequiredBatchUpdatePartitionRequestRequestTypeDef,
     _OptionalBatchUpdatePartitionRequestRequestTypeDef,
 ):
     pass
 
-GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
-    "GetUnfilteredPartitionsMetadataResponseTypeDef",
-    {
-        "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTableVersionResponseTypeDef = TypedDict(
-    "GetTableVersionResponseTypeDef",
-    {
-        "TableVersion": TableVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTableVersionsResponseTypeDef = TypedDict(
-    "GetTableVersionsResponseTypeDef",
-    {
-        "TableVersions": List[TableVersionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 BatchGetJobsResponseTypeDef = TypedDict(
     "BatchGetJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "JobsNotFound": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -9665,14 +11737,40 @@
     "UpdateJobRequestRequestTypeDef",
     {
         "JobName": str,
         "JobUpdate": JobUpdateTypeDef,
     },
 )
 
+GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
+    "GetUnfilteredPartitionsMetadataResponseTypeDef",
+    {
+        "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTableVersionResponseTypeDef = TypedDict(
+    "GetTableVersionResponseTypeDef",
+    {
+        "TableVersion": TableVersionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTableVersionsResponseTypeDef = TypedDict(
+    "GetTableVersionsResponseTypeDef",
+    {
+        "TableVersions": List[TableVersionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 WorkflowRunTypeDef = TypedDict(
     "WorkflowRunTypeDef",
     {
         "Name": str,
         "WorkflowRunId": str,
         "PreviousRunId": str,
         "WorkflowRunProperties": Dict[str, str],
@@ -9680,15 +11778,14 @@
         "CompletedOn": datetime,
         "Status": WorkflowRunStatusType,
         "ErrorMessage": str,
         "Statistics": WorkflowRunStatisticsTypeDef,
         "Graph": WorkflowGraphTypeDef,
         "StartingEventBatchCondition": StartingEventBatchConditionTypeDef,
     },
-    total=False,
 )
 
 GetWorkflowRunResponseTypeDef = TypedDict(
     "GetWorkflowRunResponseTypeDef",
     {
         "Run": WorkflowRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -9713,15 +11810,14 @@
         "CreatedOn": datetime,
         "LastModifiedOn": datetime,
         "LastRun": WorkflowRunTypeDef,
         "Graph": WorkflowGraphTypeDef,
         "MaxConcurrentRuns": int,
         "BlueprintDetails": BlueprintDetailsTypeDef,
     },
-    total=False,
 )
 
 BatchGetWorkflowsResponseTypeDef = TypedDict(
     "BatchGetWorkflowsResponseTypeDef",
     {
         "Workflows": List[WorkflowTypeDef],
         "MissingWorkflows": List[str],
```

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue.egg-info/PKG-INFO` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.28.1
-Summary: Type annotations for boto3.Glue 1.28.1 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.4
+Summary: Type annotations for boto3.Glue 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.28.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
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
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
 
@@ -472,62 +472,101 @@
 ### Typed dictionaries
 
 `mypy_boto3_glue.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glue.type_defs import (
+    NotificationPropertyOutputTypeDef,
     NotificationPropertyTypeDef,
+    AggregateOperationOutputTypeDef,
     AggregateOperationTypeDef,
+    AmazonRedshiftAdvancedOptionOutputTypeDef,
     AmazonRedshiftAdvancedOptionTypeDef,
+    OptionOutputTypeDef,
     OptionTypeDef,
+    ApplyMappingOutputTypeDef,
     ApplyMappingTypeDef,
     AuditContextTypeDef,
-    PartitionValueListTypeDef,
+    PartitionValueListOutputTypeDef,
+    BasicCatalogTargetOutputTypeDef,
     BasicCatalogTargetTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteConnectionRequestRequestTypeDef,
     ErrorDetailTypeDef,
+    PartitionValueListTypeDef,
     BatchDeleteTableRequestRequestTypeDef,
     BatchDeleteTableVersionRequestRequestTypeDef,
     BatchGetBlueprintsRequestRequestTypeDef,
     BatchGetCrawlersRequestRequestTypeDef,
     BatchGetCustomEntityTypesRequestRequestTypeDef,
     CustomEntityTypeTypeDef,
     BatchGetDataQualityResultRequestRequestTypeDef,
     BatchGetDevEndpointsRequestRequestTypeDef,
     DevEndpointTypeDef,
     BatchGetJobsRequestRequestTypeDef,
     BatchGetTriggersRequestRequestTypeDef,
     BatchGetWorkflowsRequestRequestTypeDef,
     BatchStopJobRunRequestRequestTypeDef,
     BatchStopJobRunSuccessfulSubmissionTypeDef,
+    BinaryColumnStatisticsDataOutputTypeDef,
     BinaryColumnStatisticsDataTypeDef,
     BlueprintDetailsTypeDef,
     BlueprintRunTypeDef,
     LastActiveDefinitionTypeDef,
+    BooleanColumnStatisticsDataOutputTypeDef,
     BooleanColumnStatisticsDataTypeDef,
     CancelDataQualityRuleRecommendationRunRequestRequestTypeDef,
     CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CancelMLTaskRunRequestRequestTypeDef,
     CancelStatementRequestRequestTypeDef,
     CatalogEntryTypeDef,
     CatalogImportStatusTypeDef,
+    KafkaStreamingSourceOptionsOutputTypeDef,
+    StreamingDataPreviewOptionsOutputTypeDef,
     KafkaStreamingSourceOptionsTypeDef,
     StreamingDataPreviewOptionsTypeDef,
+    KinesisStreamingSourceOptionsOutputTypeDef,
     KinesisStreamingSourceOptionsTypeDef,
+    CatalogSchemaChangePolicyOutputTypeDef,
     CatalogSchemaChangePolicyTypeDef,
+    CatalogSourceOutputTypeDef,
     CatalogSourceTypeDef,
+    CatalogTargetOutputTypeDef,
     CatalogTargetTypeDef,
     CheckSchemaVersionValidityInputRequestTypeDef,
     CsvClassifierTypeDef,
     GrokClassifierTypeDef,
     JsonClassifierTypeDef,
     XMLClassifierTypeDef,
+    CloudWatchEncryptionOutputTypeDef,
     CloudWatchEncryptionTypeDef,
+    DirectJDBCSourceOutputTypeDef,
+    DropDuplicatesOutputTypeDef,
+    DropFieldsOutputTypeDef,
+    DynamoDBCatalogSourceOutputTypeDef,
+    FillMissingValuesOutputTypeDef,
+    MergeOutputTypeDef,
+    MicrosoftSQLServerCatalogSourceOutputTypeDef,
+    MicrosoftSQLServerCatalogTargetOutputTypeDef,
+    MySQLCatalogSourceOutputTypeDef,
+    MySQLCatalogTargetOutputTypeDef,
+    OracleSQLCatalogSourceOutputTypeDef,
+    OracleSQLCatalogTargetOutputTypeDef,
+    PIIDetectionOutputTypeDef,
+    PostgreSQLCatalogSourceOutputTypeDef,
+    PostgreSQLCatalogTargetOutputTypeDef,
+    RedshiftSourceOutputTypeDef,
+    RelationalCatalogSourceOutputTypeDef,
+    RenameFieldOutputTypeDef,
+    SelectFieldsOutputTypeDef,
+    SelectFromCollectionOutputTypeDef,
+    SpigotOutputTypeDef,
+    SplitFieldsOutputTypeDef,
+    UnionOutputTypeDef,
     DirectJDBCSourceTypeDef,
     DropDuplicatesTypeDef,
     DropFieldsTypeDef,
     DynamoDBCatalogSourceTypeDef,
     FillMissingValuesTypeDef,
     MergeTypeDef,
     MicrosoftSQLServerCatalogSourceTypeDef,
@@ -543,71 +582,103 @@
     RelationalCatalogSourceTypeDef,
     RenameFieldTypeDef,
     SelectFieldsTypeDef,
     SelectFromCollectionTypeDef,
     SpigotTypeDef,
     SplitFieldsTypeDef,
     UnionTypeDef,
+    CodeGenEdgeOutputTypeDef,
     CodeGenEdgeTypeDef,
+    CodeGenNodeArgOutputTypeDef,
     CodeGenNodeArgTypeDef,
     ColumnImportanceTypeDef,
+    ColumnOutputTypeDef,
     ColumnRowFilterTypeDef,
+    DateColumnStatisticsDataOutputTypeDef,
+    DoubleColumnStatisticsDataOutputTypeDef,
+    LongColumnStatisticsDataOutputTypeDef,
+    StringColumnStatisticsDataOutputTypeDef,
     DateColumnStatisticsDataTypeDef,
     DoubleColumnStatisticsDataTypeDef,
     LongColumnStatisticsDataTypeDef,
     StringColumnStatisticsDataTypeDef,
     ColumnTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     ConfusionMatrixTypeDef,
     PhysicalConnectionRequirementsTypeDef,
+    ConnectionPasswordEncryptionOutputTypeDef,
     ConnectionPasswordEncryptionTypeDef,
+    PhysicalConnectionRequirementsOutputTypeDef,
+    ConnectionsListOutputTypeDef,
     ConnectionsListTypeDef,
     CrawlTypeDef,
     CrawlerHistoryTypeDef,
     CrawlerMetricsTypeDef,
+    DeltaTargetOutputTypeDef,
+    DynamoDBTargetOutputTypeDef,
+    IcebergTargetOutputTypeDef,
+    JdbcTargetOutputTypeDef,
+    MongoDBTargetOutputTypeDef,
+    S3TargetOutputTypeDef,
     DeltaTargetTypeDef,
     DynamoDBTargetTypeDef,
     IcebergTargetTypeDef,
     JdbcTargetTypeDef,
     MongoDBTargetTypeDef,
     S3TargetTypeDef,
-    LakeFormationConfigurationTypeDef,
+    LakeFormationConfigurationOutputTypeDef,
     LastCrawlInfoTypeDef,
-    LineageConfigurationTypeDef,
-    RecrawlPolicyTypeDef,
+    LineageConfigurationOutputTypeDef,
+    RecrawlPolicyOutputTypeDef,
     ScheduleTypeDef,
-    SchemaChangePolicyTypeDef,
+    SchemaChangePolicyOutputTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintRequestRequestTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateXMLClassifierRequestTypeDef,
+    LakeFormationConfigurationTypeDef,
+    LineageConfigurationTypeDef,
+    RecrawlPolicyTypeDef,
+    SchemaChangePolicyTypeDef,
     CreateCustomEntityTypeRequestRequestTypeDef,
     DataQualityTargetTableTypeDef,
     CreateDevEndpointRequestRequestTypeDef,
     ExecutionPropertyTypeDef,
     JobCommandTypeDef,
     SourceControlDetailsTypeDef,
     GlueTableTypeDef,
     PartitionIndexTypeDef,
     CreateRegistryInputRequestTypeDef,
     RegistryIdTypeDef,
     SessionCommandTypeDef,
     EventBatchingConditionTypeDef,
     CreateWorkflowRequestRequestTypeDef,
+    DQResultsPublishingOptionsOutputTypeDef,
     DQResultsPublishingOptionsTypeDef,
+    DQStopJobOnFailureOptionsOutputTypeDef,
     DQStopJobOnFailureOptionsTypeDef,
+    EncryptionAtRestOutputTypeDef,
     EncryptionAtRestTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
+    DataQualityEvaluationRunAdditionalRunOptionsOutputTypeDef,
     DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
     DataQualityRuleResultTypeDef,
+    DataQualityTargetTableOutputTypeDef,
+    GlueTableOutputTypeDef,
+    DatabaseIdentifierOutputTypeDef,
     DatabaseIdentifierTypeDef,
     FederatedDatabaseTypeDef,
+    FederatedDatabaseOutputTypeDef,
+    DatatypeOutputTypeDef,
     DatatypeTypeDef,
+    DecimalNumberOutputTypeDef,
     DecimalNumberTypeDef,
     DeleteBlueprintRequestRequestTypeDef,
     DeleteClassifierRequestRequestTypeDef,
     DeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     DeleteColumnStatisticsForTableRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteCrawlerRequestRequestTypeDef,
@@ -625,24 +696,33 @@
     DeleteSessionRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DeleteTableVersionRequestRequestTypeDef,
     DeleteTriggerRequestRequestTypeDef,
     DeleteUserDefinedFunctionRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DevEndpointCustomLibrariesTypeDef,
+    DirectSchemaChangePolicyOutputTypeDef,
     DirectSchemaChangePolicyTypeDef,
+    NullCheckBoxListOutputTypeDef,
     NullCheckBoxListTypeDef,
+    TransformConfigParameterOutputTypeDef,
     TransformConfigParameterTypeDef,
     EdgeTypeDef,
+    JobBookmarksEncryptionOutputTypeDef,
+    S3EncryptionOutputTypeDef,
     JobBookmarksEncryptionTypeDef,
     S3EncryptionTypeDef,
     ErrorDetailsTypeDef,
+    EventBatchingConditionOutputTypeDef,
+    ExecutionPropertyOutputTypeDef,
     ExportLabelsTaskRunPropertiesTypeDef,
     FederatedTableTypeDef,
+    FilterValueOutputTypeDef,
     FilterValueTypeDef,
+    FindMatchesParametersOutputTypeDef,
     FindMatchesParametersTypeDef,
     FindMatchesTaskRunPropertiesTypeDef,
     GetBlueprintRequestRequestTypeDef,
     GetBlueprintRunRequestRequestTypeDef,
     GetBlueprintRunsRequestRequestTypeDef,
     GetCatalogImportStatusRequestRequestTypeDef,
     GetClassifierRequestRequestTypeDef,
@@ -672,20 +752,21 @@
     GetJobRunRequestRequestTypeDef,
     GetJobRunsRequestRequestTypeDef,
     GetJobsRequestRequestTypeDef,
     GetMLTaskRunRequestRequestTypeDef,
     TaskRunFilterCriteriaTypeDef,
     TaskRunSortCriteriaTypeDef,
     GetMLTransformRequestRequestTypeDef,
-    SchemaColumnTypeDef,
+    SchemaColumnOutputTypeDef,
     TransformSortCriteriaTypeDef,
-    MappingEntryTypeDef,
+    MappingEntryOutputTypeDef,
     GetPartitionIndexesRequestRequestTypeDef,
     GetPartitionRequestRequestTypeDef,
     SegmentTypeDef,
+    MappingEntryTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GluePolicyTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     SchemaVersionNumberTypeDef,
     GetSecurityConfigurationRequestRequestTypeDef,
     GetSecurityConfigurationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
@@ -699,21 +780,27 @@
     GetTriggersRequestRequestTypeDef,
     GetUserDefinedFunctionRequestRequestTypeDef,
     GetUserDefinedFunctionsRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowRunPropertiesRequestRequestTypeDef,
     GetWorkflowRunRequestRequestTypeDef,
     GetWorkflowRunsRequestRequestTypeDef,
+    GlueStudioSchemaColumnOutputTypeDef,
     GlueStudioSchemaColumnTypeDef,
+    S3SourceAdditionalOptionsOutputTypeDef,
     S3SourceAdditionalOptionsTypeDef,
     IcebergInputTypeDef,
     ImportCatalogToGlueRequestRequestTypeDef,
     ImportLabelsTaskRunPropertiesTypeDef,
+    JDBCConnectorOptionsOutputTypeDef,
     JDBCConnectorOptionsTypeDef,
+    JobCommandOutputTypeDef,
     PredecessorTypeDef,
+    SourceControlDetailsOutputTypeDef,
+    JoinColumnOutputTypeDef,
     JoinColumnTypeDef,
     KeySchemaElementTypeDef,
     LabelingSetGenerationTaskRunPropertiesTypeDef,
     ListBlueprintsRequestRequestTypeDef,
     ListCrawlersRequestRequestTypeDef,
     ListCustomEntityTypesRequestRequestTypeDef,
     ListDevEndpointsRequestRequestTypeDef,
@@ -722,31 +809,43 @@
     RegistryListItemTypeDef,
     SchemaVersionListItemTypeDef,
     SchemaListItemTypeDef,
     ListSessionsRequestRequestTypeDef,
     ListStatementsRequestRequestTypeDef,
     ListTriggersRequestRequestTypeDef,
     ListWorkflowsRequestRequestTypeDef,
+    MLUserDataEncryptionOutputTypeDef,
     MLUserDataEncryptionTypeDef,
+    MappingOutputTypeDef,
     MappingTypeDef,
     OtherMetadataValueListItemTypeDef,
     MetadataKeyValuePairTypeDef,
+    OrderOutputTypeDef,
     OrderTypeDef,
     PropertyPredicateTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutWorkflowRunPropertiesRequestRequestTypeDef,
+    UpsertRedshiftTargetOptionsOutputTypeDef,
     UpsertRedshiftTargetOptionsTypeDef,
     ResetJobBookmarkRequestRequestTypeDef,
+    ResourceUriOutputTypeDef,
     ResourceUriTypeDef,
     ResumeWorkflowRunRequestRequestTypeDef,
     RunStatementRequestRequestTypeDef,
+    S3DirectSourceAdditionalOptionsOutputTypeDef,
     S3DirectSourceAdditionalOptionsTypeDef,
+    SchemaColumnTypeDef,
+    SchemaIdOutputTypeDef,
     SortCriterionTypeDef,
+    SerDeInfoOutputTypeDef,
     SerDeInfoTypeDef,
+    SessionCommandOutputTypeDef,
+    SkewedInfoOutputTypeDef,
     SkewedInfoTypeDef,
+    SqlAliasOutputTypeDef,
     SqlAliasTypeDef,
     StartBlueprintRunRequestRequestTypeDef,
     StartCrawlerRequestRequestTypeDef,
     StartCrawlerScheduleRequestRequestTypeDef,
     StartExportLabelsTaskRunRequestRequestTypeDef,
     StartImportLabelsTaskRunRequestRequestTypeDef,
     StartMLEvaluationTaskRunRequestRequestTypeDef,
@@ -756,37 +855,39 @@
     StartingEventBatchConditionTypeDef,
     StatementOutputDataTypeDef,
     StopCrawlerRequestRequestTypeDef,
     StopCrawlerScheduleRequestRequestTypeDef,
     StopSessionRequestRequestTypeDef,
     StopTriggerRequestRequestTypeDef,
     StopWorkflowRunRequestRequestTypeDef,
+    TableIdentifierOutputTypeDef,
     TableIdentifierTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBlueprintRequestRequestTypeDef,
     UpdateCsvClassifierRequestTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateXMLClassifierRequestTypeDef,
     UpdateCrawlerScheduleRequestRequestTypeDef,
     UpdateDataQualityRulesetRequestRequestTypeDef,
     UpdateJobFromSourceControlRequestRequestTypeDef,
     UpdateSourceControlFromJobRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     WorkflowRunStatisticsTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     StartJobRunRequestRequestTypeDef,
+    AggregateOutputTypeDef,
     AggregateTypeDef,
+    AmazonRedshiftNodeDataOutputTypeDef,
     AmazonRedshiftNodeDataTypeDef,
     GetUnfilteredPartitionMetadataRequestRequestTypeDef,
     GetUnfilteredTableMetadataRequestRequestTypeDef,
     BackfillErrorTypeDef,
-    BatchDeletePartitionRequestRequestTypeDef,
-    BatchGetPartitionRequestRequestTypeDef,
     CancelMLTaskRunResponseTypeDef,
     CheckSchemaVersionValidityResponseTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
     CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateJobResponseTypeDef,
@@ -853,78 +954,104 @@
     BatchDeleteConnectionResponseTypeDef,
     BatchStopJobRunErrorTypeDef,
     BatchUpdatePartitionFailureEntryTypeDef,
     ColumnErrorTypeDef,
     PartitionErrorTypeDef,
     TableErrorTypeDef,
     TableVersionErrorTypeDef,
+    BatchDeletePartitionRequestRequestTypeDef,
+    BatchGetPartitionRequestRequestTypeDef,
     BatchGetCustomEntityTypesResponseTypeDef,
     ListCustomEntityTypesResponseTypeDef,
     BatchGetDevEndpointsResponseTypeDef,
     GetDevEndpointResponseTypeDef,
     GetDevEndpointsResponseTypeDef,
     GetBlueprintRunResponseTypeDef,
     GetBlueprintRunsResponseTypeDef,
     BlueprintTypeDef,
     GetCatalogImportStatusResponseTypeDef,
+    CatalogKafkaSourceOutputTypeDef,
+    DirectKafkaSourceOutputTypeDef,
     CatalogKafkaSourceTypeDef,
     DirectKafkaSourceTypeDef,
+    CatalogKinesisSourceOutputTypeDef,
+    DirectKinesisSourceOutputTypeDef,
     CatalogKinesisSourceTypeDef,
     DirectKinesisSourceTypeDef,
+    GovernedCatalogTargetOutputTypeDef,
+    S3CatalogTargetOutputTypeDef,
+    S3DeltaCatalogTargetOutputTypeDef,
+    S3HudiCatalogTargetOutputTypeDef,
     GovernedCatalogTargetTypeDef,
     S3CatalogTargetTypeDef,
     S3DeltaCatalogTargetTypeDef,
     S3HudiCatalogTargetTypeDef,
     ClassifierTypeDef,
+    CodeGenNodeOutputTypeDef,
     CodeGenNodeTypeDef,
     LocationTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     FindMatchesMetricsTypeDef,
     ConnectionInputTypeDef,
     ConnectionTypeDef,
     CrawlerNodeDetailsTypeDef,
     ListCrawlsResponseTypeDef,
     GetCrawlerMetricsResponseTypeDef,
+    CrawlerTargetsOutputTypeDef,
     CrawlerTargetsTypeDef,
     ListCrawlsRequestRequestTypeDef,
     CreateClassifierRequestRequestTypeDef,
     CreateDataQualityRulesetRequestRequestTypeDef,
     DataQualityRulesetFilterCriteriaTypeDef,
-    DataQualityRulesetListDetailsTypeDef,
-    GetDataQualityRulesetResponseTypeDef,
     DataSourceTypeDef,
     CreatePartitionIndexRequestRequestTypeDef,
     CreateSchemaInputRequestTypeDef,
     DeleteRegistryInputRequestTypeDef,
     GetRegistryInputRequestTypeDef,
     ListSchemasInputRequestTypeDef,
     UpdateRegistryInputRequestTypeDef,
     CreateSessionRequestRequestTypeDef,
-    SessionTypeDef,
+    EvaluateDataQualityMultiFrameOutputTypeDef,
+    EvaluateDataQualityOutputTypeDef,
     EvaluateDataQualityMultiFrameTypeDef,
     EvaluateDataQualityTypeDef,
+    DataCatalogEncryptionSettingsOutputTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
+    PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    DataQualityRulesetListDetailsTypeDef,
+    GetDataQualityRulesetResponseTypeDef,
+    DataSourceOutputTypeDef,
+    NullValueFieldOutputTypeDef,
     NullValueFieldTypeDef,
+    DecimalColumnStatisticsDataOutputTypeDef,
     DecimalColumnStatisticsDataTypeDef,
     DeleteSchemaInputRequestTypeDef,
     DeleteSchemaVersionsInputRequestTypeDef,
     GetSchemaByDefinitionInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     ListSchemaVersionsInputRequestTypeDef,
     RegisterSchemaVersionInputRequestTypeDef,
     SchemaReferenceTypeDef,
     UpdateDevEndpointRequestRequestTypeDef,
+    S3DeltaDirectTargetOutputTypeDef,
+    S3DirectTargetOutputTypeDef,
+    S3GlueParquetTargetOutputTypeDef,
+    S3HudiDirectTargetOutputTypeDef,
     S3DeltaDirectTargetTypeDef,
     S3DirectTargetTypeDef,
     S3GlueParquetTargetTypeDef,
     S3HudiDirectTargetTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     SchemaVersionErrorItemTypeDef,
+    FilterExpressionOutputTypeDef,
     FilterExpressionTypeDef,
+    TransformParametersOutputTypeDef,
     TransformParametersTypeDef,
     GetClassifiersRequestGetClassifiersPaginateTypeDef,
     GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
     GetCrawlersRequestGetCrawlersPaginateTypeDef,
     GetDatabasesRequestGetDatabasesPaginateTypeDef,
     GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef,
     GetJobRunsRequestGetJobRunsPaginateTypeDef,
@@ -940,103 +1067,128 @@
     ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     ListSchemasInputListSchemasPaginateTypeDef,
     GetConnectionsRequestGetConnectionsPaginateTypeDef,
     GetConnectionsRequestRequestTypeDef,
     GetJobBookmarkResponseTypeDef,
     ResetJobBookmarkResponseTypeDef,
     GetMLTaskRunsRequestRequestTypeDef,
-    TransformFilterCriteriaTypeDef,
     GetMappingResponseTypeDef,
     GetPartitionsRequestGetPartitionsPaginateTypeDef,
     GetPartitionsRequestRequestTypeDef,
     GetUnfilteredPartitionsMetadataRequestRequestTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetSchemaVersionInputRequestTypeDef,
     GetSchemaVersionsDiffInputRequestTypeDef,
     UpdateSchemaInputRequestTypeDef,
+    GlueSchemaOutputTypeDef,
     GlueSchemaTypeDef,
+    GovernedCatalogSourceOutputTypeDef,
+    S3CatalogSourceOutputTypeDef,
     GovernedCatalogSourceTypeDef,
     S3CatalogSourceTypeDef,
     OpenTableFormatInputTypeDef,
     JobRunTypeDef,
+    JoinOutputTypeDef,
     JoinTypeDef,
     TaskRunPropertiesTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
+    TransformEncryptionOutputTypeDef,
     TransformEncryptionTypeDef,
     MetadataInfoTypeDef,
     PutSchemaVersionMetadataInputRequestTypeDef,
     QuerySchemaVersionMetadataInputRequestTypeDef,
     RemoveSchemaVersionMetadataInputRequestTypeDef,
+    RedshiftTargetOutputTypeDef,
     RedshiftTargetTypeDef,
-    UserDefinedFunctionInputTypeDef,
     UserDefinedFunctionTypeDef,
+    UserDefinedFunctionInputTypeDef,
+    TransformFilterCriteriaTypeDef,
+    SchemaReferenceOutputTypeDef,
     SearchTablesRequestRequestTypeDef,
+    SessionTypeDef,
     StatementOutputTypeDef,
     UpdateClassifierRequestRequestTypeDef,
+    AmazonRedshiftSourceOutputTypeDef,
+    AmazonRedshiftTargetOutputTypeDef,
     AmazonRedshiftSourceTypeDef,
     AmazonRedshiftTargetTypeDef,
     PartitionIndexDescriptorTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionResponseTypeDef,
     BatchCreatePartitionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
     BatchGetBlueprintsResponseTypeDef,
     GetBlueprintResponseTypeDef,
     GetClassifierResponseTypeDef,
     GetClassifiersResponseTypeDef,
-    CreateScriptRequestRequestTypeDef,
     GetDataflowGraphResponseTypeDef,
+    CreateScriptRequestRequestTypeDef,
     GetMappingRequestRequestTypeDef,
     GetPlanRequestRequestTypeDef,
-    CreateTriggerRequestRequestTypeDef,
     TriggerTypeDef,
+    CreateTriggerRequestRequestTypeDef,
     TriggerUpdateTypeDef,
     EvaluationMetricsTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     GetConnectionResponseTypeDef,
     GetConnectionsResponseTypeDef,
     CrawlerTypeDef,
     CreateCrawlerRequestRequestTypeDef,
     UpdateCrawlerRequestRequestTypeDef,
     ListDataQualityRulesetsRequestRequestTypeDef,
-    ListDataQualityRulesetsResponseTypeDef,
-    DataQualityResultDescriptionTypeDef,
     DataQualityResultFilterCriteriaTypeDef,
-    DataQualityResultTypeDef,
-    DataQualityRuleRecommendationRunDescriptionTypeDef,
     DataQualityRuleRecommendationRunFilterTypeDef,
-    DataQualityRulesetEvaluationRunDescriptionTypeDef,
     DataQualityRulesetEvaluationRunFilterTypeDef,
-    GetDataQualityResultResponseTypeDef,
-    GetDataQualityRuleRecommendationRunResponseTypeDef,
-    GetDataQualityRulesetEvaluationRunResponseTypeDef,
     StartDataQualityRuleRecommendationRunRequestRequestTypeDef,
     StartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-    CreateSessionResponseTypeDef,
-    GetSessionResponseTypeDef,
-    ListSessionsResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     PutDataCatalogEncryptionSettingsRequestRequestTypeDef,
-    DatabaseInputTypeDef,
     DatabaseTypeDef,
+    DatabaseInputTypeDef,
+    ListDataQualityRulesetsResponseTypeDef,
+    DataQualityResultDescriptionTypeDef,
+    DataQualityResultTypeDef,
+    DataQualityRuleRecommendationRunDescriptionTypeDef,
+    DataQualityRulesetEvaluationRunDescriptionTypeDef,
+    GetDataQualityResultResponseTypeDef,
+    GetDataQualityRuleRecommendationRunResponseTypeDef,
+    GetDataQualityRulesetEvaluationRunResponseTypeDef,
+    DropNullFieldsOutputTypeDef,
     DropNullFieldsTypeDef,
+    ColumnStatisticsDataOutputTypeDef,
     ColumnStatisticsDataTypeDef,
     StorageDescriptorTypeDef,
-    CreateSecurityConfigurationRequestRequestTypeDef,
     SecurityConfigurationTypeDef,
+    CreateSecurityConfigurationRequestRequestTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
     UpdateMLTransformRequestRequestTypeDef,
-    GetMLTransformsRequestRequestTypeDef,
-    ListMLTransformsRequestRequestTypeDef,
+    AthenaConnectorSourceOutputTypeDef,
+    CatalogDeltaSourceOutputTypeDef,
+    CatalogHudiSourceOutputTypeDef,
+    CustomCodeOutputTypeDef,
+    DynamicTransformOutputTypeDef,
+    JDBCConnectorSourceOutputTypeDef,
+    JDBCConnectorTargetOutputTypeDef,
+    S3CatalogDeltaSourceOutputTypeDef,
+    S3CatalogHudiSourceOutputTypeDef,
+    S3CsvSourceOutputTypeDef,
+    S3DeltaSourceOutputTypeDef,
+    S3HudiSourceOutputTypeDef,
+    S3JsonSourceOutputTypeDef,
+    S3ParquetSourceOutputTypeDef,
+    SparkConnectorSourceOutputTypeDef,
+    SparkConnectorTargetOutputTypeDef,
+    SparkSQLOutputTypeDef,
     AthenaConnectorSourceTypeDef,
     CatalogDeltaSourceTypeDef,
     CatalogHudiSourceTypeDef,
     CustomCodeTypeDef,
     DynamicTransformTypeDef,
     JDBCConnectorSourceTypeDef,
     JDBCConnectorTargetTypeDef,
@@ -1053,100 +1205,108 @@
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
     JobNodeDetailsTypeDef,
     GetMLTaskRunResponseTypeDef,
     TaskRunTypeDef,
     CreateMLTransformRequestRequestTypeDef,
     QuerySchemaVersionMetadataResponseTypeDef,
-    CreateUserDefinedFunctionRequestRequestTypeDef,
-    UpdateUserDefinedFunctionRequestRequestTypeDef,
     GetUserDefinedFunctionResponseTypeDef,
     GetUserDefinedFunctionsResponseTypeDef,
+    CreateUserDefinedFunctionRequestRequestTypeDef,
+    UpdateUserDefinedFunctionRequestRequestTypeDef,
+    GetMLTransformsRequestRequestTypeDef,
+    ListMLTransformsRequestRequestTypeDef,
+    StorageDescriptorOutputTypeDef,
+    CreateSessionResponseTypeDef,
+    GetSessionResponseTypeDef,
+    ListSessionsResponseTypeDef,
     StatementTypeDef,
     GetPartitionIndexesResponseTypeDef,
     BatchGetTriggersResponseTypeDef,
     GetTriggerResponseTypeDef,
     GetTriggersResponseTypeDef,
     TriggerNodeDetailsTypeDef,
     UpdateTriggerResponseTypeDef,
     UpdateTriggerRequestRequestTypeDef,
     GetMLTransformResponseTypeDef,
     MLTransformTypeDef,
     BatchGetCrawlersResponseTypeDef,
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
-    ListDataQualityResultsResponseTypeDef,
     ListDataQualityResultsRequestRequestTypeDef,
-    BatchGetDataQualityResultResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsResponseTypeDef,
     ListDataQualityRuleRecommendationRunsRequestRequestTypeDef,
-    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
     ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef,
-    CreateDatabaseRequestRequestTypeDef,
-    UpdateDatabaseRequestRequestTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
+    CreateDatabaseRequestRequestTypeDef,
+    UpdateDatabaseRequestRequestTypeDef,
+    ListDataQualityResultsResponseTypeDef,
+    BatchGetDataQualityResultResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsResponseTypeDef,
+    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
+    ColumnStatisticsOutputTypeDef,
     ColumnStatisticsTypeDef,
     PartitionInputTypeDef,
-    PartitionTypeDef,
     TableInputTypeDef,
-    TableTypeDef,
     GetSecurityConfigurationResponseTypeDef,
     GetSecurityConfigurationsResponseTypeDef,
+    CodeGenConfigurationNodeOutputTypeDef,
     CodeGenConfigurationNodeTypeDef,
     GetMLTaskRunsResponseTypeDef,
+    PartitionTypeDef,
+    TableTypeDef,
     GetStatementResponseTypeDef,
     ListStatementsResponseTypeDef,
     NodeTypeDef,
     GetMLTransformsResponseTypeDef,
     ColumnStatisticsErrorTypeDef,
     GetColumnStatisticsForPartitionResponseTypeDef,
     GetColumnStatisticsForTableResponseTypeDef,
     UpdateColumnStatisticsForPartitionRequestRequestTypeDef,
     UpdateColumnStatisticsForTableRequestRequestTypeDef,
     BatchCreatePartitionRequestRequestTypeDef,
     BatchUpdatePartitionRequestEntryTypeDef,
     CreatePartitionRequestRequestTypeDef,
     UpdatePartitionRequestRequestTypeDef,
+    CreateTableRequestRequestTypeDef,
+    UpdateTableRequestRequestTypeDef,
+    JobTypeDef,
+    CreateJobRequestRequestTypeDef,
+    JobUpdateTypeDef,
     BatchGetPartitionResponseTypeDef,
     GetPartitionResponseTypeDef,
     GetPartitionsResponseTypeDef,
     GetUnfilteredPartitionMetadataResponseTypeDef,
     UnfilteredPartitionTypeDef,
-    CreateTableRequestRequestTypeDef,
-    UpdateTableRequestRequestTypeDef,
     GetTableResponseTypeDef,
     GetTablesResponseTypeDef,
     GetUnfilteredTableMetadataResponseTypeDef,
     SearchTablesResponseTypeDef,
     TableVersionTypeDef,
-    CreateJobRequestRequestTypeDef,
-    JobTypeDef,
-    JobUpdateTypeDef,
     WorkflowGraphTypeDef,
     UpdateColumnStatisticsForPartitionResponseTypeDef,
     UpdateColumnStatisticsForTableResponseTypeDef,
     BatchUpdatePartitionRequestRequestTypeDef,
-    GetUnfilteredPartitionsMetadataResponseTypeDef,
-    GetTableVersionResponseTypeDef,
-    GetTableVersionsResponseTypeDef,
     BatchGetJobsResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobsResponseTypeDef,
     UpdateJobRequestRequestTypeDef,
+    GetUnfilteredPartitionsMetadataResponseTypeDef,
+    GetTableVersionResponseTypeDef,
+    GetTableVersionsResponseTypeDef,
     WorkflowRunTypeDef,
     GetWorkflowRunResponseTypeDef,
     GetWorkflowRunsResponseTypeDef,
     WorkflowTypeDef,
     BatchGetWorkflowsResponseTypeDef,
     GetWorkflowResponseTypeDef,
 )
 
 
-def get_structure() -> NotificationPropertyTypeDef:
+def get_structure() -> NotificationPropertyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-glue-1.28.1/mypy_boto3_glue.egg-info/SOURCES.txt` & `mypy-boto3-glue-1.28.4/mypy_boto3_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.28.1/setup.py` & `mypy-boto3-glue-1.28.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glue",
-    version="1.28.1",
+    version="1.28.4",
     packages=["mypy_boto3_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Glue 1.28.1 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Glue 1.28.4 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

