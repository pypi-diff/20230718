# Comparing `tmp/mypy-boto3-lexv2-models-1.28.0.tar.gz` & `tmp/mypy-boto3-lexv2-models-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lexv2-models-1.28.0.tar", last modified: Thu Jul  6 20:59:57 2023, max compression
+gzip compressed data, was "mypy-boto3-lexv2-models-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-lexv2-models-1.28.0.tar` & `mypy-boto3-lexv2-models-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.934351 mypy-boto3-lexv2-models-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:45:31.000000 mypy-boto3-lexv2-models-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29882 2023-07-06 20:59:57.934351 mypy-boto3-lexv2-models-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-07-06 20:45:31.000000 mypy-boto3-lexv2-models-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.922351 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:45:31.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-06 20:45:31.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:45:31.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66201 2023-07-06 20:45:32.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66101 2023-07-06 20:45:31.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15877 2023-07-06 20:45:32.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15875 2023-07-06 20:45:32.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:45:31.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   150419 2023-07-06 20:45:38.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   150222 2023-07-06 20:45:36.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:45:31.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-06 20:45:32.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-06 20:45:32.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.934351 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29882 2023-07-06 20:59:57.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 20:59:57.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:57.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:57.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:57.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:57.000000 mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:57.934351 mypy-boto3-lexv2-models-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:45:31.000000 mypy-boto3-lexv2-models-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-lexv2-models-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37086 2023-07-18 19:32:41.750719 mypy-boto3-lexv2-models-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35582 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73416 2023-07-18 19:32:19.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73309 2023-07-18 19:32:19.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19542 2023-07-18 19:32:20.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19540 2023-07-18 19:32:20.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   196677 2023-07-18 19:32:24.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   196483 2023-07-18 19:32:22.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-18 19:32:19.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-18 19:32:19.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37086 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 19:32:41.000000 mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.750719 mypy-boto3-lexv2-models-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-18 19:32:18.000000 mypy-boto3-lexv2-models-1.28.5/setup.py
```

### Comparing `mypy-boto3-lexv2-models-1.28.0/LICENSE` & `mypy-boto3-lexv2-models-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.0/PKG-INFO` & `mypy-boto3-lexv2-models-1.28.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-models
-Version: 1.28.0
-Summary: Type annotations for boto3.LexModelsV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.5
+Summary: Type annotations for boto3.LexModelsV2 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelsV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[boto3.LexModelsV2 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
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
 [mypy-boto3-lexv2-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,19 +318,43 @@
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_lexv2_models.literals import (
     AggregatedUtterancesFilterNameType,
     AggregatedUtterancesFilterOperatorType,
     AggregatedUtterancesSortAttributeType,
+    AnalyticsBinByNameType,
+    AnalyticsCommonFilterNameType,
+    AnalyticsFilterOperatorType,
+    AnalyticsIntentFieldType,
+    AnalyticsIntentFilterNameType,
+    AnalyticsIntentMetricNameType,
+    AnalyticsIntentStageFieldType,
+    AnalyticsIntentStageFilterNameType,
+    AnalyticsIntentStageMetricNameType,
+    AnalyticsIntervalType,
+    AnalyticsMetricStatisticType,
+    AnalyticsModalityType,
+    AnalyticsNodeTypeType,
+    AnalyticsSessionFieldType,
+    AnalyticsSessionFilterNameType,
+    AnalyticsSessionMetricNameType,
+    AnalyticsSessionSortByNameType,
+    AnalyticsSortOrderType,
+    AnalyticsUtteranceAttributeNameType,
+    AnalyticsUtteranceFieldType,
+    AnalyticsUtteranceFilterNameType,
+    AnalyticsUtteranceMetricNameType,
+    AnalyticsUtteranceSortByNameType,
     AssociatedTranscriptFilterNameType,
     AudioRecognitionStrategyType,
     BotAliasAvailableWaiterName,
     BotAliasStatusType,
     BotAvailableWaiterName,
+    BotChannelTypeType,
     BotExportCompletedWaiterName,
     BotFilterNameType,
     BotFilterOperatorType,
     BotImportCompletedWaiterName,
     BotLocaleBuiltWaiterName,
     BotLocaleCreatedWaiterName,
     BotLocaleExpressTestingAvailableWaiterName,
@@ -342,14 +366,15 @@
     BotSortAttributeType,
     BotStatusType,
     BotTypeType,
     BotVersionAvailableWaiterName,
     BotVersionSortAttributeType,
     BuiltInIntentSortAttributeType,
     BuiltInSlotTypeSortAttributeType,
+    ConversationEndStateType,
     ConversationLogsInputModeFilterType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
     ErrorCodeType,
     ExportFilterNameType,
     ExportFilterOperatorType,
@@ -360,14 +385,15 @@
     ImportFilterOperatorType,
     ImportResourceTypeType,
     ImportSortAttributeType,
     ImportStatusType,
     IntentFilterNameType,
     IntentFilterOperatorType,
     IntentSortAttributeType,
+    IntentStateType,
     MergeStrategyType,
     MessageSelectionStrategyType,
     ObfuscationSettingTypeType,
     PromptAttemptType,
     SearchOrderType,
     SlotConstraintType,
     SlotFilterNameType,
@@ -389,14 +415,15 @@
     TestSetDiscrepancyReportStatusType,
     TestSetGenerationStatusType,
     TestSetModalityType,
     TestSetSortAttributeType,
     TestSetStatusType,
     TimeDimensionType,
     TranscriptFormatType,
+    UtteranceContentTypeType,
     VoiceEngineType,
     LexModelsV2ServiceName,
     ServiceName,
     ResourceServiceName,
     WaiterName,
     RegionName,
 )
@@ -412,83 +439,140 @@
 
 `mypy_boto3_lexv2_models.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_models.type_defs import (
     ActiveContextTypeDef,
+    AdvancedRecognitionSettingOutputTypeDef,
     AdvancedRecognitionSettingTypeDef,
     ExecutionErrorDetailsTypeDef,
     AgentTurnSpecificationTypeDef,
     AggregatedUtterancesFilterTypeDef,
     AggregatedUtterancesSortByTypeDef,
     AggregatedUtterancesSummaryTypeDef,
+    AllowedInputTypesOutputTypeDef,
     AllowedInputTypesTypeDef,
+    AnalyticsBinBySpecificationTypeDef,
+    AnalyticsBinKeyTypeDef,
+    AnalyticsIntentFilterTypeDef,
+    AnalyticsIntentGroupByKeyTypeDef,
+    AnalyticsIntentGroupBySpecificationTypeDef,
+    AnalyticsIntentMetricResultTypeDef,
+    AnalyticsIntentMetricTypeDef,
+    AnalyticsIntentNodeSummaryTypeDef,
+    AnalyticsIntentStageFilterTypeDef,
+    AnalyticsIntentStageGroupByKeyTypeDef,
+    AnalyticsIntentStageGroupBySpecificationTypeDef,
+    AnalyticsIntentStageMetricResultTypeDef,
+    AnalyticsIntentStageMetricTypeDef,
+    AnalyticsPathFilterTypeDef,
+    AnalyticsSessionFilterTypeDef,
+    AnalyticsSessionGroupByKeyTypeDef,
+    AnalyticsSessionGroupBySpecificationTypeDef,
+    AnalyticsSessionMetricResultTypeDef,
+    AnalyticsSessionMetricTypeDef,
+    AnalyticsUtteranceAttributeResultTypeDef,
+    AnalyticsUtteranceAttributeTypeDef,
+    AnalyticsUtteranceFilterTypeDef,
+    AnalyticsUtteranceGroupByKeyTypeDef,
+    AnalyticsUtteranceGroupBySpecificationTypeDef,
+    AnalyticsUtteranceMetricResultTypeDef,
+    AnalyticsUtteranceMetricTypeDef,
     AssociatedTranscriptFilterTypeDef,
     AssociatedTranscriptTypeDef,
+    AudioSpecificationOutputTypeDef,
+    DTMFSpecificationOutputTypeDef,
     AudioSpecificationTypeDef,
     DTMFSpecificationTypeDef,
+    S3BucketLogDestinationOutputTypeDef,
     S3BucketLogDestinationTypeDef,
     NewCustomVocabularyItemTypeDef,
-    CustomVocabularyItemTypeDef,
+    CustomVocabularyItemOutputTypeDef,
     FailedCustomVocabularyItemTypeDef,
     CustomVocabularyEntryIdTypeDef,
+    CustomVocabularyItemTypeDef,
     BotAliasHistoryEventTypeDef,
     BotAliasSummaryTypeDef,
+    BotAliasTestExecutionTargetOutputTypeDef,
     BotAliasTestExecutionTargetTypeDef,
+    BotExportSpecificationOutputTypeDef,
     BotExportSpecificationTypeDef,
     BotFilterTypeDef,
+    DataPrivacyOutputTypeDef,
     DataPrivacyTypeDef,
+    BotLocaleExportSpecificationOutputTypeDef,
     BotLocaleExportSpecificationTypeDef,
     BotLocaleFilterTypeDef,
     BotLocaleHistoryEventTypeDef,
+    VoiceSettingsOutputTypeDef,
     VoiceSettingsTypeDef,
     BotLocaleSortByTypeDef,
     BotLocaleSummaryTypeDef,
+    BotMemberOutputTypeDef,
     BotMemberTypeDef,
     IntentStatisticsTypeDef,
     SlotTypeStatisticsTypeDef,
     BotRecommendationSummaryTypeDef,
     BotSortByTypeDef,
     BotSummaryTypeDef,
+    BotVersionLocaleDetailsOutputTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BotVersionSummaryTypeDef,
     BuildBotLocaleRequestRequestTypeDef,
     BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInIntentSummaryTypeDef,
     BuiltInSlotTypeSortByTypeDef,
     BuiltInSlotTypeSummaryTypeDef,
+    ButtonOutputTypeDef,
     ButtonTypeDef,
+    CloudWatchLogGroupLogDestinationOutputTypeDef,
     CloudWatchLogGroupLogDestinationTypeDef,
+    LambdaCodeHookOutputTypeDef,
     LambdaCodeHookTypeDef,
+    SubSlotTypeCompositionOutputTypeDef,
     SubSlotTypeCompositionTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     ConversationLevelIntentClassificationResultItemTypeDef,
     ConversationLevelResultDetailTypeDef,
     ConversationLevelSlotResolutionResultItemTypeDef,
     ConversationLevelTestResultsFilterByTypeDef,
+    ConversationLogsDataSourceFilterByOutputTypeDef,
     ConversationLogsDataSourceFilterByTypeDef,
     SentimentAnalysisSettingsTypeDef,
+    SentimentAnalysisSettingsOutputTypeDef,
     DialogCodeHookSettingsTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     SampleUtteranceTypeDef,
+    DialogCodeHookSettingsOutputTypeDef,
+    InputContextOutputTypeDef,
+    KendraConfigurationOutputTypeDef,
+    OutputContextOutputTypeDef,
+    SampleUtteranceOutputTypeDef,
     CreateResourcePolicyRequestRequestTypeDef,
     CreateResourcePolicyResponseTypeDef,
     PrincipalTypeDef,
     CreateResourcePolicyStatementResponseTypeDef,
     MultipleValuesSettingTypeDef,
     ObfuscationSettingTypeDef,
+    MultipleValuesSettingOutputTypeDef,
+    ObfuscationSettingOutputTypeDef,
     CreateUploadUrlResponseTypeDef,
+    CustomPayloadOutputTypeDef,
     CustomPayloadTypeDef,
+    CustomVocabularyExportSpecificationOutputTypeDef,
     CustomVocabularyExportSpecificationTypeDef,
+    CustomVocabularyImportSpecificationOutputTypeDef,
     CustomVocabularyImportSpecificationTypeDef,
+    DateRangeFilterOutputTypeDef,
     DateRangeFilterTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotAliasResponseTypeDef,
     DeleteBotLocaleRequestRequestTypeDef,
     DeleteBotLocaleResponseTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotResponseTypeDef,
@@ -510,285 +594,384 @@
     DeleteTestSetRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
     ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
-    EncryptionSettingTypeDef,
+    EncryptionSettingOutputTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataResponseTypeDef,
     DescribeExportRequestRequestTypeDef,
     DescribeImportRequestRequestTypeDef,
     DescribeIntentRequestRequestTypeDef,
-    SlotPriorityTypeDef,
+    SlotPriorityOutputTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeSlotRequestRequestTypeDef,
     DescribeSlotTypeRequestRequestTypeDef,
     DescribeTestExecutionRequestRequestTypeDef,
     DescribeTestSetDiscrepancyReportRequestRequestTypeDef,
     DescribeTestSetGenerationRequestRequestTypeDef,
-    TestSetStorageLocationTypeDef,
+    TestSetStorageLocationOutputTypeDef,
     DescribeTestSetRequestRequestTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
+    IntentOverrideOutputTypeDef,
     IntentOverrideTypeDef,
+    ElicitationCodeHookInvocationSettingOutputTypeDef,
     ElicitationCodeHookInvocationSettingTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionSettingTypeDef,
     ExportFilterTypeDef,
+    TestSetExportSpecificationOutputTypeDef,
     TestSetExportSpecificationTypeDef,
     ExportSortByTypeDef,
     GetTestExecutionArtifactsUrlRequestRequestTypeDef,
     GetTestExecutionArtifactsUrlResponseTypeDef,
+    GrammarSlotTypeSourceOutputTypeDef,
     GrammarSlotTypeSourceTypeDef,
     ImportFilterTypeDef,
     ImportSortByTypeDef,
     ImportSummaryTypeDef,
     RuntimeHintsTypeDef,
     IntentClassificationTestResultItemCountsTypeDef,
     IntentFilterTypeDef,
     IntentSortByTypeDef,
+    InvokedIntentSampleTypeDef,
     ListBotAliasesRequestRequestTypeDef,
     ListBotRecommendationsRequestRequestTypeDef,
     ListCustomVocabularyItemsRequestRequestTypeDef,
     ListRecommendedIntentsRequestRequestTypeDef,
     RecommendedIntentSummaryTypeDef,
+    SessionDataSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
     SlotTypeSummaryTypeDef,
     SlotFilterTypeDef,
     SlotSortByTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TestExecutionSortByTypeDef,
     ListTestSetRecordsRequestRequestTypeDef,
     TestSetSortByTypeDef,
+    UtteranceDataSortByTypeDef,
+    PlainTextMessageOutputTypeDef,
+    SSMLMessageOutputTypeDef,
     PlainTextMessageTypeDef,
     SSMLMessageTypeDef,
     OverallTestResultItemTypeDef,
+    PathFormatOutputTypeDef,
     PathFormatTypeDef,
+    TextInputSpecificationOutputTypeDef,
     TextInputSpecificationTypeDef,
+    RelativeAggregationDurationOutputTypeDef,
     RelativeAggregationDurationTypeDef,
     ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
+    SampleValueOutputTypeDef,
     SampleValueTypeDef,
+    SlotDefaultValueOutputTypeDef,
     SlotDefaultValueTypeDef,
+    SlotPriorityTypeDef,
     SlotResolutionTestResultItemCountsTypeDef,
+    SlotValueOutputTypeDef,
     SlotValueTypeDef,
+    SlotValueRegexFilterOutputTypeDef,
     SlotValueRegexFilterTypeDef,
+    TestSetStorageLocationTypeDef,
     StopBotRecommendationRequestRequestTypeDef,
     StopBotRecommendationResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSetIntentDiscrepancyItemTypeDef,
     TestSetSlotDiscrepancyItemTypeDef,
+    TestSetDiscrepancyReportBotAliasTargetOutputTypeDef,
     TestSetDiscrepancyReportBotAliasTargetTypeDef,
+    TestSetImportInputLocationOutputTypeDef,
     TestSetImportInputLocationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExportRequestRequestTypeDef,
     UpdateResourcePolicyRequestRequestTypeDef,
     UpdateResourcePolicyResponseTypeDef,
     UpdateTestSetRequestRequestTypeDef,
     UserTurnIntentOutputTypeDef,
     UserTurnSlotOutputTypeDef,
     UtteranceAudioInputSpecificationTypeDef,
     AgentTurnResultTypeDef,
+    AnalyticsIntentResultTypeDef,
+    ListIntentMetricsRequestRequestTypeDef,
+    ListIntentPathsResponseTypeDef,
+    AnalyticsIntentStageResultTypeDef,
+    ListIntentStageMetricsRequestRequestTypeDef,
+    ListIntentPathsRequestRequestTypeDef,
+    AnalyticsSessionResultTypeDef,
+    ListSessionMetricsRequestRequestTypeDef,
+    AnalyticsUtteranceResultTypeDef,
+    ListUtteranceMetricsRequestRequestTypeDef,
     SearchAssociatedTranscriptsRequestRequestTypeDef,
     SearchAssociatedTranscriptsResponseTypeDef,
+    AudioAndDTMFInputSpecificationOutputTypeDef,
     AudioAndDTMFInputSpecificationTypeDef,
+    AudioLogDestinationOutputTypeDef,
     AudioLogDestinationTypeDef,
     BatchCreateCustomVocabularyItemRequestRequestTypeDef,
-    BatchUpdateCustomVocabularyItemRequestRequestTypeDef,
     ListCustomVocabularyItemsResponseTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
+    BatchUpdateCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
+    TestExecutionTargetOutputTypeDef,
     TestExecutionTargetTypeDef,
+    BotImportSpecificationOutputTypeDef,
     BotImportSpecificationTypeDef,
-    BotLocaleImportSpecificationTypeDef,
-    CreateBotLocaleRequestRequestTypeDef,
+    BotLocaleImportSpecificationOutputTypeDef,
     CreateBotLocaleResponseTypeDef,
     DescribeBotLocaleResponseTypeDef,
-    UpdateBotLocaleRequestRequestTypeDef,
     UpdateBotLocaleResponseTypeDef,
+    BotLocaleImportSpecificationTypeDef,
+    CreateBotLocaleRequestRequestTypeDef,
+    UpdateBotLocaleRequestRequestTypeDef,
     ListBotLocalesRequestRequestTypeDef,
     ListBotLocalesResponseTypeDef,
-    CreateBotRequestRequestTypeDef,
     CreateBotResponseTypeDef,
     DescribeBotResponseTypeDef,
-    UpdateBotRequestRequestTypeDef,
     UpdateBotResponseTypeDef,
+    CreateBotRequestRequestTypeDef,
+    UpdateBotRequestRequestTypeDef,
     BotRecommendationResultStatisticsTypeDef,
     ListBotRecommendationsResponseTypeDef,
     ListBotsRequestRequestTypeDef,
     ListBotsResponseTypeDef,
-    CreateBotVersionRequestRequestTypeDef,
     CreateBotVersionResponseTypeDef,
+    CreateBotVersionRequestRequestTypeDef,
     ListBotVersionsRequestRequestTypeDef,
     ListBotVersionsResponseTypeDef,
     ListBuiltInIntentsRequestRequestTypeDef,
     ListBuiltInIntentsResponseTypeDef,
     ListBuiltInSlotTypesRequestRequestTypeDef,
     ListBuiltInSlotTypesResponseTypeDef,
+    ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
+    TextLogDestinationOutputTypeDef,
     TextLogDestinationTypeDef,
+    CodeHookSpecificationOutputTypeDef,
     CodeHookSpecificationTypeDef,
+    CompositeSlotTypeSettingOutputTypeDef,
     CompositeSlotTypeSettingTypeDef,
     ConversationLevelTestResultItemTypeDef,
     TestExecutionResultFilterByTypeDef,
+    ConversationLogsDataSourceOutputTypeDef,
     ConversationLogsDataSourceTypeDef,
     IntentSummaryTypeDef,
     CreateResourcePolicyStatementRequestRequestTypeDef,
+    LexTranscriptFilterOutputTypeDef,
     LexTranscriptFilterTypeDef,
     DescribeBotAliasRequestBotAliasAvailableWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
     DescribeBotRequestBotAvailableWaitTypeDef,
     DescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
     DescribeExportRequestBotExportCompletedWaitTypeDef,
     DescribeImportRequestBotImportCompletedWaitTypeDef,
     DescribeBotVersionResponseTypeDef,
-    UpdateBotRecommendationRequestRequestTypeDef,
     DescribeTestSetResponseTypeDef,
     TestSetSummaryTypeDef,
     UpdateTestSetResponseTypeDef,
+    DialogStateOutputTypeDef,
     DialogStateTypeDef,
+    UpdateBotRecommendationRequestRequestTypeDef,
+    ExportResourceSpecificationOutputTypeDef,
     ExportResourceSpecificationTypeDef,
     ListExportsRequestRequestTypeDef,
+    GrammarSlotTypeSettingOutputTypeDef,
     GrammarSlotTypeSettingTypeDef,
     ListImportsRequestRequestTypeDef,
     ListImportsResponseTypeDef,
     InputSessionStateSpecificationTypeDef,
     IntentClassificationTestResultItemTypeDef,
     ListIntentsRequestRequestTypeDef,
+    SessionSpecificationTypeDef,
     ListRecommendedIntentsResponseTypeDef,
+    ListSessionAnalyticsDataRequestRequestTypeDef,
     ListSlotTypesRequestRequestTypeDef,
     ListSlotTypesResponseTypeDef,
     ListSlotsRequestRequestTypeDef,
     ListTestExecutionsRequestRequestTypeDef,
     ListTestSetsRequestRequestTypeDef,
+    ListUtteranceAnalyticsDataRequestRequestTypeDef,
     OverallTestResultsTypeDef,
+    UtteranceAggregationDurationOutputTypeDef,
     UtteranceAggregationDurationTypeDef,
     RuntimeHintDetailsTypeDef,
+    SlotTypeValueOutputTypeDef,
     SlotTypeValueTypeDef,
+    SlotDefaultValueSpecificationOutputTypeDef,
     SlotDefaultValueSpecificationTypeDef,
     SlotResolutionTestResultItemTypeDef,
+    SlotValueOverrideOutputTypeDef,
     SlotValueOverrideTypeDef,
+    SlotValueSelectionSettingOutputTypeDef,
     SlotValueSelectionSettingTypeDef,
     TestSetDiscrepancyErrorsTypeDef,
+    TestSetDiscrepancyReportResourceTargetOutputTypeDef,
     TestSetDiscrepancyReportResourceTargetTypeDef,
+    TestSetImportResourceSpecificationOutputTypeDef,
     TestSetImportResourceSpecificationTypeDef,
     UserTurnOutputSpecificationTypeDef,
     UtteranceInputSpecificationTypeDef,
+    ListIntentMetricsResponseTypeDef,
+    ListIntentStageMetricsResponseTypeDef,
+    ListSessionMetricsResponseTypeDef,
+    ListUtteranceMetricsResponseTypeDef,
+    PromptAttemptSpecificationOutputTypeDef,
     PromptAttemptSpecificationTypeDef,
+    AudioLogSettingOutputTypeDef,
     AudioLogSettingTypeDef,
     DescribeTestExecutionResponseTypeDef,
-    StartTestExecutionRequestRequestTypeDef,
     StartTestExecutionResponseTypeDef,
     TestExecutionSummaryTypeDef,
+    StartTestExecutionRequestRequestTypeDef,
     BotRecommendationResultsTypeDef,
+    MessageOutputTypeDef,
+    UtteranceBotResponseTypeDef,
     MessageTypeDef,
+    TextLogSettingOutputTypeDef,
     TextLogSettingTypeDef,
+    BotAliasLocaleSettingsOutputTypeDef,
     BotAliasLocaleSettingsTypeDef,
     ConversationLevelTestResultsTypeDef,
     ListTestExecutionResultItemsRequestRequestTypeDef,
+    TestSetGenerationDataSourceOutputTypeDef,
     TestSetGenerationDataSourceTypeDef,
     ListIntentsResponseTypeDef,
+    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListTestSetsResponseTypeDef,
-    CreateExportRequestRequestTypeDef,
     CreateExportResponseTypeDef,
     DescribeExportResponseTypeDef,
     ExportSummaryTypeDef,
     UpdateExportResponseTypeDef,
+    CreateExportRequestRequestTypeDef,
+    ExternalSourceSettingOutputTypeDef,
     ExternalSourceSettingTypeDef,
     IntentClassificationTestResultsTypeDef,
-    ListAggregatedUtterancesRequestRequestTypeDef,
+    ListSessionAnalyticsDataResponseTypeDef,
     ListAggregatedUtterancesResponseTypeDef,
+    ListAggregatedUtterancesRequestRequestTypeDef,
     IntentLevelSlotResolutionTestResultItemTypeDef,
-    CreateTestSetDiscrepancyReportRequestRequestTypeDef,
     CreateTestSetDiscrepancyReportResponseTypeDef,
     DescribeTestSetDiscrepancyReportResponseTypeDef,
+    CreateTestSetDiscrepancyReportRequestRequestTypeDef,
+    ImportResourceSpecificationOutputTypeDef,
     ImportResourceSpecificationTypeDef,
     UserTurnInputSpecificationTypeDef,
     ListTestExecutionsResponseTypeDef,
+    MessageGroupOutputTypeDef,
+    UtteranceSpecificationTypeDef,
     MessageGroupTypeDef,
+    ConversationLogSettingsOutputTypeDef,
     ConversationLogSettingsTypeDef,
     DescribeTestSetGenerationResponseTypeDef,
-    StartTestSetGenerationRequestRequestTypeDef,
     StartTestSetGenerationResponseTypeDef,
+    StartTestSetGenerationRequestRequestTypeDef,
+    S3BucketTranscriptSourceOutputTypeDef,
     S3BucketTranscriptSourceTypeDef,
     ListExportsResponseTypeDef,
-    CreateSlotTypeRequestRequestTypeDef,
     CreateSlotTypeResponseTypeDef,
     DescribeSlotTypeResponseTypeDef,
-    UpdateSlotTypeRequestRequestTypeDef,
     UpdateSlotTypeResponseTypeDef,
+    CreateSlotTypeRequestRequestTypeDef,
+    UpdateSlotTypeRequestRequestTypeDef,
     IntentLevelSlotResolutionTestResultsTypeDef,
     DescribeImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     UserTurnResultTypeDef,
     UserTurnSpecificationTypeDef,
+    FulfillmentStartResponseSpecificationOutputTypeDef,
+    FulfillmentUpdateResponseSpecificationOutputTypeDef,
+    PromptSpecificationOutputTypeDef,
+    ResponseSpecificationOutputTypeDef,
+    StillWaitingResponseSpecificationOutputTypeDef,
+    ListUtteranceAnalyticsDataResponseTypeDef,
     FulfillmentStartResponseSpecificationTypeDef,
     FulfillmentUpdateResponseSpecificationTypeDef,
     PromptSpecificationTypeDef,
     ResponseSpecificationTypeDef,
     StillWaitingResponseSpecificationTypeDef,
-    CreateBotAliasRequestRequestTypeDef,
     CreateBotAliasResponseTypeDef,
     DescribeBotAliasResponseTypeDef,
-    UpdateBotAliasRequestRequestTypeDef,
     UpdateBotAliasResponseTypeDef,
+    CreateBotAliasRequestRequestTypeDef,
+    UpdateBotAliasRequestRequestTypeDef,
+    TranscriptSourceSettingOutputTypeDef,
     TranscriptSourceSettingTypeDef,
     TestSetTurnResultTypeDef,
     TurnSpecificationTypeDef,
-    FulfillmentUpdatesSpecificationTypeDef,
+    FulfillmentUpdatesSpecificationOutputTypeDef,
     SlotSummaryTypeDef,
+    ConditionalBranchOutputTypeDef,
+    DefaultConditionalBranchOutputTypeDef,
+    WaitAndContinueSpecificationOutputTypeDef,
+    FulfillmentUpdatesSpecificationTypeDef,
     ConditionalBranchTypeDef,
     DefaultConditionalBranchTypeDef,
     WaitAndContinueSpecificationTypeDef,
     DescribeBotRecommendationResponseTypeDef,
-    StartBotRecommendationRequestRequestTypeDef,
     StartBotRecommendationResponseTypeDef,
     UpdateBotRecommendationResponseTypeDef,
+    StartBotRecommendationRequestRequestTypeDef,
     UtteranceLevelTestResultItemTypeDef,
     TestSetTurnRecordTypeDef,
     ListSlotsResponseTypeDef,
+    ConditionalSpecificationOutputTypeDef,
+    SubSlotValueElicitationSettingOutputTypeDef,
     ConditionalSpecificationTypeDef,
     SubSlotValueElicitationSettingTypeDef,
     UtteranceLevelTestResultsTypeDef,
     ListTestSetRecordsResponseTypeDef,
+    IntentClosingSettingOutputTypeDef,
+    PostDialogCodeHookInvocationSpecificationOutputTypeDef,
+    PostFulfillmentStatusSpecificationOutputTypeDef,
+    SpecificationsOutputTypeDef,
     IntentClosingSettingTypeDef,
     PostDialogCodeHookInvocationSpecificationTypeDef,
     PostFulfillmentStatusSpecificationTypeDef,
     SpecificationsTypeDef,
     TestExecutionResultItemsTypeDef,
+    DialogCodeHookInvocationSettingOutputTypeDef,
+    FulfillmentCodeHookSettingsOutputTypeDef,
+    SubSlotSettingOutputTypeDef,
     DialogCodeHookInvocationSettingTypeDef,
     FulfillmentCodeHookSettingsTypeDef,
     SubSlotSettingTypeDef,
     ListTestExecutionResultItemsResponseTypeDef,
+    InitialResponseSettingOutputTypeDef,
+    IntentConfirmationSettingOutputTypeDef,
+    SlotCaptureSettingOutputTypeDef,
     InitialResponseSettingTypeDef,
     IntentConfirmationSettingTypeDef,
     SlotCaptureSettingTypeDef,
-    CreateIntentRequestRequestTypeDef,
     CreateIntentResponseTypeDef,
     DescribeIntentResponseTypeDef,
-    UpdateIntentRequestRequestTypeDef,
     UpdateIntentResponseTypeDef,
+    SlotValueElicitationSettingOutputTypeDef,
+    CreateIntentRequestRequestTypeDef,
+    UpdateIntentRequestRequestTypeDef,
     SlotValueElicitationSettingTypeDef,
-    CreateSlotRequestRequestTypeDef,
     CreateSlotResponseTypeDef,
     DescribeSlotResponseTypeDef,
-    UpdateSlotRequestRequestTypeDef,
     UpdateSlotResponseTypeDef,
+    CreateSlotRequestRequestTypeDef,
+    UpdateSlotRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ActiveContextTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-lexv2-models-1.28.0/README.md` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-lexv2-models
+Version: 1.28.5
+Summary: Type annotations for boto3.LexModelsV2 1.28.5 service generated with mypy-boto3-builder 7.15.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 lexv2-models type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-lexv2-models"></a>
 
 # mypy-boto3-lexv2-models
 
 [![PyPI - mypy-boto3-lexv2-models](https://img.shields.io/pypi/v/mypy-boto3-lexv2-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lexv2-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lexv2-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelsV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
+[boto3.LexModelsV2 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2)
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
 [mypy-boto3-lexv2-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,19 +318,43 @@
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_lexv2_models.literals import (
     AggregatedUtterancesFilterNameType,
     AggregatedUtterancesFilterOperatorType,
     AggregatedUtterancesSortAttributeType,
+    AnalyticsBinByNameType,
+    AnalyticsCommonFilterNameType,
+    AnalyticsFilterOperatorType,
+    AnalyticsIntentFieldType,
+    AnalyticsIntentFilterNameType,
+    AnalyticsIntentMetricNameType,
+    AnalyticsIntentStageFieldType,
+    AnalyticsIntentStageFilterNameType,
+    AnalyticsIntentStageMetricNameType,
+    AnalyticsIntervalType,
+    AnalyticsMetricStatisticType,
+    AnalyticsModalityType,
+    AnalyticsNodeTypeType,
+    AnalyticsSessionFieldType,
+    AnalyticsSessionFilterNameType,
+    AnalyticsSessionMetricNameType,
+    AnalyticsSessionSortByNameType,
+    AnalyticsSortOrderType,
+    AnalyticsUtteranceAttributeNameType,
+    AnalyticsUtteranceFieldType,
+    AnalyticsUtteranceFilterNameType,
+    AnalyticsUtteranceMetricNameType,
+    AnalyticsUtteranceSortByNameType,
     AssociatedTranscriptFilterNameType,
     AudioRecognitionStrategyType,
     BotAliasAvailableWaiterName,
     BotAliasStatusType,
     BotAvailableWaiterName,
+    BotChannelTypeType,
     BotExportCompletedWaiterName,
     BotFilterNameType,
     BotFilterOperatorType,
     BotImportCompletedWaiterName,
     BotLocaleBuiltWaiterName,
     BotLocaleCreatedWaiterName,
     BotLocaleExpressTestingAvailableWaiterName,
@@ -310,14 +366,15 @@
     BotSortAttributeType,
     BotStatusType,
     BotTypeType,
     BotVersionAvailableWaiterName,
     BotVersionSortAttributeType,
     BuiltInIntentSortAttributeType,
     BuiltInSlotTypeSortAttributeType,
+    ConversationEndStateType,
     ConversationLogsInputModeFilterType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
     ErrorCodeType,
     ExportFilterNameType,
     ExportFilterOperatorType,
@@ -328,14 +385,15 @@
     ImportFilterOperatorType,
     ImportResourceTypeType,
     ImportSortAttributeType,
     ImportStatusType,
     IntentFilterNameType,
     IntentFilterOperatorType,
     IntentSortAttributeType,
+    IntentStateType,
     MergeStrategyType,
     MessageSelectionStrategyType,
     ObfuscationSettingTypeType,
     PromptAttemptType,
     SearchOrderType,
     SlotConstraintType,
     SlotFilterNameType,
@@ -357,14 +415,15 @@
     TestSetDiscrepancyReportStatusType,
     TestSetGenerationStatusType,
     TestSetModalityType,
     TestSetSortAttributeType,
     TestSetStatusType,
     TimeDimensionType,
     TranscriptFormatType,
+    UtteranceContentTypeType,
     VoiceEngineType,
     LexModelsV2ServiceName,
     ServiceName,
     ResourceServiceName,
     WaiterName,
     RegionName,
 )
@@ -380,83 +439,140 @@
 
 `mypy_boto3_lexv2_models.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_models.type_defs import (
     ActiveContextTypeDef,
+    AdvancedRecognitionSettingOutputTypeDef,
     AdvancedRecognitionSettingTypeDef,
     ExecutionErrorDetailsTypeDef,
     AgentTurnSpecificationTypeDef,
     AggregatedUtterancesFilterTypeDef,
     AggregatedUtterancesSortByTypeDef,
     AggregatedUtterancesSummaryTypeDef,
+    AllowedInputTypesOutputTypeDef,
     AllowedInputTypesTypeDef,
+    AnalyticsBinBySpecificationTypeDef,
+    AnalyticsBinKeyTypeDef,
+    AnalyticsIntentFilterTypeDef,
+    AnalyticsIntentGroupByKeyTypeDef,
+    AnalyticsIntentGroupBySpecificationTypeDef,
+    AnalyticsIntentMetricResultTypeDef,
+    AnalyticsIntentMetricTypeDef,
+    AnalyticsIntentNodeSummaryTypeDef,
+    AnalyticsIntentStageFilterTypeDef,
+    AnalyticsIntentStageGroupByKeyTypeDef,
+    AnalyticsIntentStageGroupBySpecificationTypeDef,
+    AnalyticsIntentStageMetricResultTypeDef,
+    AnalyticsIntentStageMetricTypeDef,
+    AnalyticsPathFilterTypeDef,
+    AnalyticsSessionFilterTypeDef,
+    AnalyticsSessionGroupByKeyTypeDef,
+    AnalyticsSessionGroupBySpecificationTypeDef,
+    AnalyticsSessionMetricResultTypeDef,
+    AnalyticsSessionMetricTypeDef,
+    AnalyticsUtteranceAttributeResultTypeDef,
+    AnalyticsUtteranceAttributeTypeDef,
+    AnalyticsUtteranceFilterTypeDef,
+    AnalyticsUtteranceGroupByKeyTypeDef,
+    AnalyticsUtteranceGroupBySpecificationTypeDef,
+    AnalyticsUtteranceMetricResultTypeDef,
+    AnalyticsUtteranceMetricTypeDef,
     AssociatedTranscriptFilterTypeDef,
     AssociatedTranscriptTypeDef,
+    AudioSpecificationOutputTypeDef,
+    DTMFSpecificationOutputTypeDef,
     AudioSpecificationTypeDef,
     DTMFSpecificationTypeDef,
+    S3BucketLogDestinationOutputTypeDef,
     S3BucketLogDestinationTypeDef,
     NewCustomVocabularyItemTypeDef,
-    CustomVocabularyItemTypeDef,
+    CustomVocabularyItemOutputTypeDef,
     FailedCustomVocabularyItemTypeDef,
     CustomVocabularyEntryIdTypeDef,
+    CustomVocabularyItemTypeDef,
     BotAliasHistoryEventTypeDef,
     BotAliasSummaryTypeDef,
+    BotAliasTestExecutionTargetOutputTypeDef,
     BotAliasTestExecutionTargetTypeDef,
+    BotExportSpecificationOutputTypeDef,
     BotExportSpecificationTypeDef,
     BotFilterTypeDef,
+    DataPrivacyOutputTypeDef,
     DataPrivacyTypeDef,
+    BotLocaleExportSpecificationOutputTypeDef,
     BotLocaleExportSpecificationTypeDef,
     BotLocaleFilterTypeDef,
     BotLocaleHistoryEventTypeDef,
+    VoiceSettingsOutputTypeDef,
     VoiceSettingsTypeDef,
     BotLocaleSortByTypeDef,
     BotLocaleSummaryTypeDef,
+    BotMemberOutputTypeDef,
     BotMemberTypeDef,
     IntentStatisticsTypeDef,
     SlotTypeStatisticsTypeDef,
     BotRecommendationSummaryTypeDef,
     BotSortByTypeDef,
     BotSummaryTypeDef,
+    BotVersionLocaleDetailsOutputTypeDef,
     BotVersionLocaleDetailsTypeDef,
     BotVersionSortByTypeDef,
     BotVersionSummaryTypeDef,
     BuildBotLocaleRequestRequestTypeDef,
     BuildBotLocaleResponseTypeDef,
     BuiltInIntentSortByTypeDef,
     BuiltInIntentSummaryTypeDef,
     BuiltInSlotTypeSortByTypeDef,
     BuiltInSlotTypeSummaryTypeDef,
+    ButtonOutputTypeDef,
     ButtonTypeDef,
+    CloudWatchLogGroupLogDestinationOutputTypeDef,
     CloudWatchLogGroupLogDestinationTypeDef,
+    LambdaCodeHookOutputTypeDef,
     LambdaCodeHookTypeDef,
+    SubSlotTypeCompositionOutputTypeDef,
     SubSlotTypeCompositionTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     ConversationLevelIntentClassificationResultItemTypeDef,
     ConversationLevelResultDetailTypeDef,
     ConversationLevelSlotResolutionResultItemTypeDef,
     ConversationLevelTestResultsFilterByTypeDef,
+    ConversationLogsDataSourceFilterByOutputTypeDef,
     ConversationLogsDataSourceFilterByTypeDef,
     SentimentAnalysisSettingsTypeDef,
+    SentimentAnalysisSettingsOutputTypeDef,
     DialogCodeHookSettingsTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     SampleUtteranceTypeDef,
+    DialogCodeHookSettingsOutputTypeDef,
+    InputContextOutputTypeDef,
+    KendraConfigurationOutputTypeDef,
+    OutputContextOutputTypeDef,
+    SampleUtteranceOutputTypeDef,
     CreateResourcePolicyRequestRequestTypeDef,
     CreateResourcePolicyResponseTypeDef,
     PrincipalTypeDef,
     CreateResourcePolicyStatementResponseTypeDef,
     MultipleValuesSettingTypeDef,
     ObfuscationSettingTypeDef,
+    MultipleValuesSettingOutputTypeDef,
+    ObfuscationSettingOutputTypeDef,
     CreateUploadUrlResponseTypeDef,
+    CustomPayloadOutputTypeDef,
     CustomPayloadTypeDef,
+    CustomVocabularyExportSpecificationOutputTypeDef,
     CustomVocabularyExportSpecificationTypeDef,
+    CustomVocabularyImportSpecificationOutputTypeDef,
     CustomVocabularyImportSpecificationTypeDef,
+    DateRangeFilterOutputTypeDef,
     DateRangeFilterTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotAliasResponseTypeDef,
     DeleteBotLocaleRequestRequestTypeDef,
     DeleteBotLocaleResponseTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotResponseTypeDef,
@@ -478,285 +594,384 @@
     DeleteTestSetRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeBotAliasRequestRequestTypeDef,
     ParentBotNetworkTypeDef,
     DescribeBotLocaleRequestRequestTypeDef,
     DescribeBotRecommendationRequestRequestTypeDef,
-    EncryptionSettingTypeDef,
+    EncryptionSettingOutputTypeDef,
     DescribeBotRequestRequestTypeDef,
     DescribeBotVersionRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataRequestRequestTypeDef,
     DescribeCustomVocabularyMetadataResponseTypeDef,
     DescribeExportRequestRequestTypeDef,
     DescribeImportRequestRequestTypeDef,
     DescribeIntentRequestRequestTypeDef,
-    SlotPriorityTypeDef,
+    SlotPriorityOutputTypeDef,
     DescribeResourcePolicyRequestRequestTypeDef,
     DescribeResourcePolicyResponseTypeDef,
     DescribeSlotRequestRequestTypeDef,
     DescribeSlotTypeRequestRequestTypeDef,
     DescribeTestExecutionRequestRequestTypeDef,
     DescribeTestSetDiscrepancyReportRequestRequestTypeDef,
     DescribeTestSetGenerationRequestRequestTypeDef,
-    TestSetStorageLocationTypeDef,
+    TestSetStorageLocationOutputTypeDef,
     DescribeTestSetRequestRequestTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
+    IntentOverrideOutputTypeDef,
     IntentOverrideTypeDef,
+    ElicitationCodeHookInvocationSettingOutputTypeDef,
     ElicitationCodeHookInvocationSettingTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionSettingTypeDef,
     ExportFilterTypeDef,
+    TestSetExportSpecificationOutputTypeDef,
     TestSetExportSpecificationTypeDef,
     ExportSortByTypeDef,
     GetTestExecutionArtifactsUrlRequestRequestTypeDef,
     GetTestExecutionArtifactsUrlResponseTypeDef,
+    GrammarSlotTypeSourceOutputTypeDef,
     GrammarSlotTypeSourceTypeDef,
     ImportFilterTypeDef,
     ImportSortByTypeDef,
     ImportSummaryTypeDef,
     RuntimeHintsTypeDef,
     IntentClassificationTestResultItemCountsTypeDef,
     IntentFilterTypeDef,
     IntentSortByTypeDef,
+    InvokedIntentSampleTypeDef,
     ListBotAliasesRequestRequestTypeDef,
     ListBotRecommendationsRequestRequestTypeDef,
     ListCustomVocabularyItemsRequestRequestTypeDef,
     ListRecommendedIntentsRequestRequestTypeDef,
     RecommendedIntentSummaryTypeDef,
+    SessionDataSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
     SlotTypeSummaryTypeDef,
     SlotFilterTypeDef,
     SlotSortByTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TestExecutionSortByTypeDef,
     ListTestSetRecordsRequestRequestTypeDef,
     TestSetSortByTypeDef,
+    UtteranceDataSortByTypeDef,
+    PlainTextMessageOutputTypeDef,
+    SSMLMessageOutputTypeDef,
     PlainTextMessageTypeDef,
     SSMLMessageTypeDef,
     OverallTestResultItemTypeDef,
+    PathFormatOutputTypeDef,
     PathFormatTypeDef,
+    TextInputSpecificationOutputTypeDef,
     TextInputSpecificationTypeDef,
+    RelativeAggregationDurationOutputTypeDef,
     RelativeAggregationDurationTypeDef,
     ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
+    SampleValueOutputTypeDef,
     SampleValueTypeDef,
+    SlotDefaultValueOutputTypeDef,
     SlotDefaultValueTypeDef,
+    SlotPriorityTypeDef,
     SlotResolutionTestResultItemCountsTypeDef,
+    SlotValueOutputTypeDef,
     SlotValueTypeDef,
+    SlotValueRegexFilterOutputTypeDef,
     SlotValueRegexFilterTypeDef,
+    TestSetStorageLocationTypeDef,
     StopBotRecommendationRequestRequestTypeDef,
     StopBotRecommendationResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSetIntentDiscrepancyItemTypeDef,
     TestSetSlotDiscrepancyItemTypeDef,
+    TestSetDiscrepancyReportBotAliasTargetOutputTypeDef,
     TestSetDiscrepancyReportBotAliasTargetTypeDef,
+    TestSetImportInputLocationOutputTypeDef,
     TestSetImportInputLocationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExportRequestRequestTypeDef,
     UpdateResourcePolicyRequestRequestTypeDef,
     UpdateResourcePolicyResponseTypeDef,
     UpdateTestSetRequestRequestTypeDef,
     UserTurnIntentOutputTypeDef,
     UserTurnSlotOutputTypeDef,
     UtteranceAudioInputSpecificationTypeDef,
     AgentTurnResultTypeDef,
+    AnalyticsIntentResultTypeDef,
+    ListIntentMetricsRequestRequestTypeDef,
+    ListIntentPathsResponseTypeDef,
+    AnalyticsIntentStageResultTypeDef,
+    ListIntentStageMetricsRequestRequestTypeDef,
+    ListIntentPathsRequestRequestTypeDef,
+    AnalyticsSessionResultTypeDef,
+    ListSessionMetricsRequestRequestTypeDef,
+    AnalyticsUtteranceResultTypeDef,
+    ListUtteranceMetricsRequestRequestTypeDef,
     SearchAssociatedTranscriptsRequestRequestTypeDef,
     SearchAssociatedTranscriptsResponseTypeDef,
+    AudioAndDTMFInputSpecificationOutputTypeDef,
     AudioAndDTMFInputSpecificationTypeDef,
+    AudioLogDestinationOutputTypeDef,
     AudioLogDestinationTypeDef,
     BatchCreateCustomVocabularyItemRequestRequestTypeDef,
-    BatchUpdateCustomVocabularyItemRequestRequestTypeDef,
     ListCustomVocabularyItemsResponseTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemRequestRequestTypeDef,
+    BatchUpdateCustomVocabularyItemRequestRequestTypeDef,
     ListBotAliasesResponseTypeDef,
+    TestExecutionTargetOutputTypeDef,
     TestExecutionTargetTypeDef,
+    BotImportSpecificationOutputTypeDef,
     BotImportSpecificationTypeDef,
-    BotLocaleImportSpecificationTypeDef,
-    CreateBotLocaleRequestRequestTypeDef,
+    BotLocaleImportSpecificationOutputTypeDef,
     CreateBotLocaleResponseTypeDef,
     DescribeBotLocaleResponseTypeDef,
-    UpdateBotLocaleRequestRequestTypeDef,
     UpdateBotLocaleResponseTypeDef,
+    BotLocaleImportSpecificationTypeDef,
+    CreateBotLocaleRequestRequestTypeDef,
+    UpdateBotLocaleRequestRequestTypeDef,
     ListBotLocalesRequestRequestTypeDef,
     ListBotLocalesResponseTypeDef,
-    CreateBotRequestRequestTypeDef,
     CreateBotResponseTypeDef,
     DescribeBotResponseTypeDef,
-    UpdateBotRequestRequestTypeDef,
     UpdateBotResponseTypeDef,
+    CreateBotRequestRequestTypeDef,
+    UpdateBotRequestRequestTypeDef,
     BotRecommendationResultStatisticsTypeDef,
     ListBotRecommendationsResponseTypeDef,
     ListBotsRequestRequestTypeDef,
     ListBotsResponseTypeDef,
-    CreateBotVersionRequestRequestTypeDef,
     CreateBotVersionResponseTypeDef,
+    CreateBotVersionRequestRequestTypeDef,
     ListBotVersionsRequestRequestTypeDef,
     ListBotVersionsResponseTypeDef,
     ListBuiltInIntentsRequestRequestTypeDef,
     ListBuiltInIntentsResponseTypeDef,
     ListBuiltInSlotTypesRequestRequestTypeDef,
     ListBuiltInSlotTypesResponseTypeDef,
+    ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
+    TextLogDestinationOutputTypeDef,
     TextLogDestinationTypeDef,
+    CodeHookSpecificationOutputTypeDef,
     CodeHookSpecificationTypeDef,
+    CompositeSlotTypeSettingOutputTypeDef,
     CompositeSlotTypeSettingTypeDef,
     ConversationLevelTestResultItemTypeDef,
     TestExecutionResultFilterByTypeDef,
+    ConversationLogsDataSourceOutputTypeDef,
     ConversationLogsDataSourceTypeDef,
     IntentSummaryTypeDef,
     CreateResourcePolicyStatementRequestRequestTypeDef,
+    LexTranscriptFilterOutputTypeDef,
     LexTranscriptFilterTypeDef,
     DescribeBotAliasRequestBotAliasAvailableWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef,
     DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef,
     DescribeBotRequestBotAvailableWaitTypeDef,
     DescribeBotVersionRequestBotVersionAvailableWaitTypeDef,
     DescribeExportRequestBotExportCompletedWaitTypeDef,
     DescribeImportRequestBotImportCompletedWaitTypeDef,
     DescribeBotVersionResponseTypeDef,
-    UpdateBotRecommendationRequestRequestTypeDef,
     DescribeTestSetResponseTypeDef,
     TestSetSummaryTypeDef,
     UpdateTestSetResponseTypeDef,
+    DialogStateOutputTypeDef,
     DialogStateTypeDef,
+    UpdateBotRecommendationRequestRequestTypeDef,
+    ExportResourceSpecificationOutputTypeDef,
     ExportResourceSpecificationTypeDef,
     ListExportsRequestRequestTypeDef,
+    GrammarSlotTypeSettingOutputTypeDef,
     GrammarSlotTypeSettingTypeDef,
     ListImportsRequestRequestTypeDef,
     ListImportsResponseTypeDef,
     InputSessionStateSpecificationTypeDef,
     IntentClassificationTestResultItemTypeDef,
     ListIntentsRequestRequestTypeDef,
+    SessionSpecificationTypeDef,
     ListRecommendedIntentsResponseTypeDef,
+    ListSessionAnalyticsDataRequestRequestTypeDef,
     ListSlotTypesRequestRequestTypeDef,
     ListSlotTypesResponseTypeDef,
     ListSlotsRequestRequestTypeDef,
     ListTestExecutionsRequestRequestTypeDef,
     ListTestSetsRequestRequestTypeDef,
+    ListUtteranceAnalyticsDataRequestRequestTypeDef,
     OverallTestResultsTypeDef,
+    UtteranceAggregationDurationOutputTypeDef,
     UtteranceAggregationDurationTypeDef,
     RuntimeHintDetailsTypeDef,
+    SlotTypeValueOutputTypeDef,
     SlotTypeValueTypeDef,
+    SlotDefaultValueSpecificationOutputTypeDef,
     SlotDefaultValueSpecificationTypeDef,
     SlotResolutionTestResultItemTypeDef,
+    SlotValueOverrideOutputTypeDef,
     SlotValueOverrideTypeDef,
+    SlotValueSelectionSettingOutputTypeDef,
     SlotValueSelectionSettingTypeDef,
     TestSetDiscrepancyErrorsTypeDef,
+    TestSetDiscrepancyReportResourceTargetOutputTypeDef,
     TestSetDiscrepancyReportResourceTargetTypeDef,
+    TestSetImportResourceSpecificationOutputTypeDef,
     TestSetImportResourceSpecificationTypeDef,
     UserTurnOutputSpecificationTypeDef,
     UtteranceInputSpecificationTypeDef,
+    ListIntentMetricsResponseTypeDef,
+    ListIntentStageMetricsResponseTypeDef,
+    ListSessionMetricsResponseTypeDef,
+    ListUtteranceMetricsResponseTypeDef,
+    PromptAttemptSpecificationOutputTypeDef,
     PromptAttemptSpecificationTypeDef,
+    AudioLogSettingOutputTypeDef,
     AudioLogSettingTypeDef,
     DescribeTestExecutionResponseTypeDef,
-    StartTestExecutionRequestRequestTypeDef,
     StartTestExecutionResponseTypeDef,
     TestExecutionSummaryTypeDef,
+    StartTestExecutionRequestRequestTypeDef,
     BotRecommendationResultsTypeDef,
+    MessageOutputTypeDef,
+    UtteranceBotResponseTypeDef,
     MessageTypeDef,
+    TextLogSettingOutputTypeDef,
     TextLogSettingTypeDef,
+    BotAliasLocaleSettingsOutputTypeDef,
     BotAliasLocaleSettingsTypeDef,
     ConversationLevelTestResultsTypeDef,
     ListTestExecutionResultItemsRequestRequestTypeDef,
+    TestSetGenerationDataSourceOutputTypeDef,
     TestSetGenerationDataSourceTypeDef,
     ListIntentsResponseTypeDef,
+    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListTestSetsResponseTypeDef,
-    CreateExportRequestRequestTypeDef,
     CreateExportResponseTypeDef,
     DescribeExportResponseTypeDef,
     ExportSummaryTypeDef,
     UpdateExportResponseTypeDef,
+    CreateExportRequestRequestTypeDef,
+    ExternalSourceSettingOutputTypeDef,
     ExternalSourceSettingTypeDef,
     IntentClassificationTestResultsTypeDef,
-    ListAggregatedUtterancesRequestRequestTypeDef,
+    ListSessionAnalyticsDataResponseTypeDef,
     ListAggregatedUtterancesResponseTypeDef,
+    ListAggregatedUtterancesRequestRequestTypeDef,
     IntentLevelSlotResolutionTestResultItemTypeDef,
-    CreateTestSetDiscrepancyReportRequestRequestTypeDef,
     CreateTestSetDiscrepancyReportResponseTypeDef,
     DescribeTestSetDiscrepancyReportResponseTypeDef,
+    CreateTestSetDiscrepancyReportRequestRequestTypeDef,
+    ImportResourceSpecificationOutputTypeDef,
     ImportResourceSpecificationTypeDef,
     UserTurnInputSpecificationTypeDef,
     ListTestExecutionsResponseTypeDef,
+    MessageGroupOutputTypeDef,
+    UtteranceSpecificationTypeDef,
     MessageGroupTypeDef,
+    ConversationLogSettingsOutputTypeDef,
     ConversationLogSettingsTypeDef,
     DescribeTestSetGenerationResponseTypeDef,
-    StartTestSetGenerationRequestRequestTypeDef,
     StartTestSetGenerationResponseTypeDef,
+    StartTestSetGenerationRequestRequestTypeDef,
+    S3BucketTranscriptSourceOutputTypeDef,
     S3BucketTranscriptSourceTypeDef,
     ListExportsResponseTypeDef,
-    CreateSlotTypeRequestRequestTypeDef,
     CreateSlotTypeResponseTypeDef,
     DescribeSlotTypeResponseTypeDef,
-    UpdateSlotTypeRequestRequestTypeDef,
     UpdateSlotTypeResponseTypeDef,
+    CreateSlotTypeRequestRequestTypeDef,
+    UpdateSlotTypeRequestRequestTypeDef,
     IntentLevelSlotResolutionTestResultsTypeDef,
     DescribeImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     UserTurnResultTypeDef,
     UserTurnSpecificationTypeDef,
+    FulfillmentStartResponseSpecificationOutputTypeDef,
+    FulfillmentUpdateResponseSpecificationOutputTypeDef,
+    PromptSpecificationOutputTypeDef,
+    ResponseSpecificationOutputTypeDef,
+    StillWaitingResponseSpecificationOutputTypeDef,
+    ListUtteranceAnalyticsDataResponseTypeDef,
     FulfillmentStartResponseSpecificationTypeDef,
     FulfillmentUpdateResponseSpecificationTypeDef,
     PromptSpecificationTypeDef,
     ResponseSpecificationTypeDef,
     StillWaitingResponseSpecificationTypeDef,
-    CreateBotAliasRequestRequestTypeDef,
     CreateBotAliasResponseTypeDef,
     DescribeBotAliasResponseTypeDef,
-    UpdateBotAliasRequestRequestTypeDef,
     UpdateBotAliasResponseTypeDef,
+    CreateBotAliasRequestRequestTypeDef,
+    UpdateBotAliasRequestRequestTypeDef,
+    TranscriptSourceSettingOutputTypeDef,
     TranscriptSourceSettingTypeDef,
     TestSetTurnResultTypeDef,
     TurnSpecificationTypeDef,
-    FulfillmentUpdatesSpecificationTypeDef,
+    FulfillmentUpdatesSpecificationOutputTypeDef,
     SlotSummaryTypeDef,
+    ConditionalBranchOutputTypeDef,
+    DefaultConditionalBranchOutputTypeDef,
+    WaitAndContinueSpecificationOutputTypeDef,
+    FulfillmentUpdatesSpecificationTypeDef,
     ConditionalBranchTypeDef,
     DefaultConditionalBranchTypeDef,
     WaitAndContinueSpecificationTypeDef,
     DescribeBotRecommendationResponseTypeDef,
-    StartBotRecommendationRequestRequestTypeDef,
     StartBotRecommendationResponseTypeDef,
     UpdateBotRecommendationResponseTypeDef,
+    StartBotRecommendationRequestRequestTypeDef,
     UtteranceLevelTestResultItemTypeDef,
     TestSetTurnRecordTypeDef,
     ListSlotsResponseTypeDef,
+    ConditionalSpecificationOutputTypeDef,
+    SubSlotValueElicitationSettingOutputTypeDef,
     ConditionalSpecificationTypeDef,
     SubSlotValueElicitationSettingTypeDef,
     UtteranceLevelTestResultsTypeDef,
     ListTestSetRecordsResponseTypeDef,
+    IntentClosingSettingOutputTypeDef,
+    PostDialogCodeHookInvocationSpecificationOutputTypeDef,
+    PostFulfillmentStatusSpecificationOutputTypeDef,
+    SpecificationsOutputTypeDef,
     IntentClosingSettingTypeDef,
     PostDialogCodeHookInvocationSpecificationTypeDef,
     PostFulfillmentStatusSpecificationTypeDef,
     SpecificationsTypeDef,
     TestExecutionResultItemsTypeDef,
+    DialogCodeHookInvocationSettingOutputTypeDef,
+    FulfillmentCodeHookSettingsOutputTypeDef,
+    SubSlotSettingOutputTypeDef,
     DialogCodeHookInvocationSettingTypeDef,
     FulfillmentCodeHookSettingsTypeDef,
     SubSlotSettingTypeDef,
     ListTestExecutionResultItemsResponseTypeDef,
+    InitialResponseSettingOutputTypeDef,
+    IntentConfirmationSettingOutputTypeDef,
+    SlotCaptureSettingOutputTypeDef,
     InitialResponseSettingTypeDef,
     IntentConfirmationSettingTypeDef,
     SlotCaptureSettingTypeDef,
-    CreateIntentRequestRequestTypeDef,
     CreateIntentResponseTypeDef,
     DescribeIntentResponseTypeDef,
-    UpdateIntentRequestRequestTypeDef,
     UpdateIntentResponseTypeDef,
+    SlotValueElicitationSettingOutputTypeDef,
+    CreateIntentRequestRequestTypeDef,
+    UpdateIntentRequestRequestTypeDef,
     SlotValueElicitationSettingTypeDef,
-    CreateSlotRequestRequestTypeDef,
     CreateSlotResponseTypeDef,
     DescribeSlotResponseTypeDef,
-    UpdateSlotRequestRequestTypeDef,
     UpdateSlotResponseTypeDef,
+    CreateSlotRequestRequestTypeDef,
+    UpdateSlotRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ActiveContextTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/__init__.py` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/__init__.pyi` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/__main__.py` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexModelsV2 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.LexModelsV2 1.28.5\nVersion:         1.28.5\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2\nOther"
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

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/client.py` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_lexv2_models.client import LexModelsV2Client
 
     session = Session()
     client: LexModelsV2Client = session.client("lexv2-models")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BotTypeType,
     EffectType,
     ImportExportFileFormatType,
@@ -26,14 +27,29 @@
     SearchOrderType,
     TestExecutionApiModeType,
     TestExecutionModalityType,
 )
 from .type_defs import (
     AggregatedUtterancesFilterTypeDef,
     AggregatedUtterancesSortByTypeDef,
+    AnalyticsBinBySpecificationTypeDef,
+    AnalyticsIntentFilterTypeDef,
+    AnalyticsIntentGroupBySpecificationTypeDef,
+    AnalyticsIntentMetricTypeDef,
+    AnalyticsIntentStageFilterTypeDef,
+    AnalyticsIntentStageGroupBySpecificationTypeDef,
+    AnalyticsIntentStageMetricTypeDef,
+    AnalyticsPathFilterTypeDef,
+    AnalyticsSessionFilterTypeDef,
+    AnalyticsSessionGroupBySpecificationTypeDef,
+    AnalyticsSessionMetricTypeDef,
+    AnalyticsUtteranceAttributeTypeDef,
+    AnalyticsUtteranceFilterTypeDef,
+    AnalyticsUtteranceGroupBySpecificationTypeDef,
+    AnalyticsUtteranceMetricTypeDef,
     AssociatedTranscriptFilterTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
     BotAliasLocaleSettingsTypeDef,
     BotFilterTypeDef,
     BotLocaleFilterTypeDef,
@@ -113,31 +129,39 @@
     ListBotsResponseTypeDef,
     ListBotVersionsResponseTypeDef,
     ListBuiltInIntentsResponseTypeDef,
     ListBuiltInSlotTypesResponseTypeDef,
     ListCustomVocabularyItemsResponseTypeDef,
     ListExportsResponseTypeDef,
     ListImportsResponseTypeDef,
+    ListIntentMetricsResponseTypeDef,
+    ListIntentPathsResponseTypeDef,
     ListIntentsResponseTypeDef,
+    ListIntentStageMetricsResponseTypeDef,
     ListRecommendedIntentsResponseTypeDef,
+    ListSessionAnalyticsDataResponseTypeDef,
+    ListSessionMetricsResponseTypeDef,
     ListSlotsResponseTypeDef,
     ListSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestExecutionResultItemsResponseTypeDef,
     ListTestExecutionsResponseTypeDef,
     ListTestSetRecordsResponseTypeDef,
     ListTestSetsResponseTypeDef,
+    ListUtteranceAnalyticsDataResponseTypeDef,
+    ListUtteranceMetricsResponseTypeDef,
     MultipleValuesSettingTypeDef,
     NewCustomVocabularyItemTypeDef,
     ObfuscationSettingTypeDef,
     OutputContextTypeDef,
     PrincipalTypeDef,
     SampleUtteranceTypeDef,
     SearchAssociatedTranscriptsResponseTypeDef,
     SentimentAnalysisSettingsTypeDef,
+    SessionDataSortByTypeDef,
     SlotFilterTypeDef,
     SlotPriorityTypeDef,
     SlotSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
     SlotTypeValueTypeDef,
     SlotValueElicitationSettingTypeDef,
@@ -163,14 +187,15 @@
     UpdateExportResponseTypeDef,
     UpdateIntentResponseTypeDef,
     UpdateResourcePolicyResponseTypeDef,
     UpdateSlotResponseTypeDef,
     UpdateSlotTypeResponseTypeDef,
     UpdateTestSetResponseTypeDef,
     UtteranceAggregationDurationTypeDef,
+    UtteranceDataSortByTypeDef,
     VoiceSettingsTypeDef,
 )
 from .waiter import (
     BotAliasAvailableWaiter,
     BotAvailableWaiter,
     BotExportCompletedWaiter,
     BotImportCompletedWaiter,
@@ -181,37 +206,33 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LexModelsV2Client",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     PreconditionFailedException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class LexModelsV2Client(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/)
     """
 
     meta: ClientMeta
@@ -220,15 +241,14 @@
     def exceptions(self) -> Exceptions:
         """
         LexModelsV2Client exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#exceptions)
         """
-
     def batch_create_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[NewCustomVocabularyItemTypeDef]
@@ -236,15 +256,14 @@
         """
         Create a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_create_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_create_custom_vocabulary_item)
         """
-
     def batch_delete_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[CustomVocabularyEntryIdTypeDef]
@@ -252,15 +271,14 @@
         """
         Delete a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_delete_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_delete_custom_vocabulary_item)
         """
-
     def batch_update_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[CustomVocabularyItemTypeDef]
@@ -268,41 +286,37 @@
         """
         Update a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_update_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_update_custom_vocabulary_item)
         """
-
     def build_bot_locale(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> BuildBotLocaleResponseTypeDef:
         """
         Builds a bot, its intents, and its slot types into a specific locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.build_bot_locale)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#build_bot_locale)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#close)
         """
-
     def create_bot(
         self,
         *,
         botName: str,
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
         idleSessionTTLInSeconds: int,
@@ -314,15 +328,14 @@
     ) -> CreateBotResponseTypeDef:
         """
         Creates an Amazon Lex conversational bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_bot)
         """
-
     def create_bot_alias(
         self,
         *,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
@@ -333,15 +346,14 @@
     ) -> CreateBotAliasResponseTypeDef:
         """
         Creates an alias for the specified version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_bot_alias)
         """
-
     def create_bot_locale(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         nluIntentConfidenceThreshold: float,
@@ -350,43 +362,40 @@
     ) -> CreateBotLocaleResponseTypeDef:
         """
         Creates a locale in the bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_locale)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_bot_locale)
         """
-
     def create_bot_version(
         self,
         *,
         botId: str,
         botVersionLocaleSpecification: Mapping[str, BotVersionLocaleDetailsTypeDef],
         description: str = ...
     ) -> CreateBotVersionResponseTypeDef:
         """
         Creates a new version of the bot based on the `DRAFT` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_bot_version)
         """
-
     def create_export(
         self,
         *,
         resourceSpecification: ExportResourceSpecificationTypeDef,
         fileFormat: ImportExportFileFormatType,
         filePassword: str = ...
     ) -> CreateExportResponseTypeDef:
         """
         Creates a zip archive containing the contents of a bot or a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_export)
         """
-
     def create_intent(
         self,
         *,
         intentName: str,
         botId: str,
         botVersion: str,
         localeId: str,
@@ -404,25 +413,23 @@
     ) -> CreateIntentResponseTypeDef:
         """
         Creates an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_intent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_intent)
         """
-
     def create_resource_policy(
         self, *, resourceArn: str, policy: str
     ) -> CreateResourcePolicyResponseTypeDef:
         """
         Creates a new resource policy with the specified policy statements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_resource_policy)
         """
-
     def create_resource_policy_statement(
         self,
         *,
         resourceArn: str,
         statementId: str,
         effect: EffectType,
         principal: Sequence[PrincipalTypeDef],
@@ -432,15 +439,14 @@
     ) -> CreateResourcePolicyStatementResponseTypeDef:
         """
         Adds a new resource policy statement to a bot or bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_resource_policy_statement)
         """
-
     def create_slot(
         self,
         *,
         slotName: str,
         valueElicitationSetting: SlotValueElicitationSettingTypeDef,
         botId: str,
         botVersion: str,
@@ -454,15 +460,14 @@
     ) -> CreateSlotResponseTypeDef:
         """
         Creates a slot in an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_slot)
         """
-
     def create_slot_type(
         self,
         *,
         slotTypeName: str,
         botId: str,
         botVersion: str,
         localeId: str,
@@ -477,140 +482,126 @@
         Creates a custom slot type To create a custom slot type, specify a name for the
         slot type and a set of enumeration values, the values that a slot of this type
         can assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_slot_type)
         """
-
     def create_test_set_discrepancy_report(
         self, *, testSetId: str, target: TestSetDiscrepancyReportResourceTargetTypeDef
     ) -> CreateTestSetDiscrepancyReportResponseTypeDef:
         """
         Create a report that describes the differences between the bot and the test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_test_set_discrepancy_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_test_set_discrepancy_report)
         """
-
     def create_upload_url(self) -> CreateUploadUrlResponseTypeDef:
         """
         Gets a pre-signed S3 write URL that you use to upload the zip archive when
         importing a bot or a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_upload_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_upload_url)
         """
-
     def delete_bot(
         self, *, botId: str, skipResourceInUseCheck: bool = ...
     ) -> DeleteBotResponseTypeDef:
         """
         Deletes all versions of a bot, including the `Draft` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_bot)
         """
-
     def delete_bot_alias(
         self, *, botAliasId: str, botId: str, skipResourceInUseCheck: bool = ...
     ) -> DeleteBotAliasResponseTypeDef:
         """
         Deletes the specified bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_bot_alias)
         """
-
     def delete_bot_locale(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> DeleteBotLocaleResponseTypeDef:
         """
         Removes a locale from a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_locale)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_bot_locale)
         """
-
     def delete_bot_version(
         self, *, botId: str, botVersion: str, skipResourceInUseCheck: bool = ...
     ) -> DeleteBotVersionResponseTypeDef:
         """
         Deletes a specific version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_bot_version)
         """
-
     def delete_custom_vocabulary(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> DeleteCustomVocabularyResponseTypeDef:
         """
         Removes a custom vocabulary from the specified locale in the specified bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_custom_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_custom_vocabulary)
         """
-
     def delete_export(self, *, exportId: str) -> DeleteExportResponseTypeDef:
         """
         Removes a previous export and the associated files stored in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_export)
         """
-
     def delete_import(self, *, importId: str) -> DeleteImportResponseTypeDef:
         """
         Removes a previous import and the associated file stored in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_import)
         """
-
     def delete_intent(
         self, *, intentId: str, botId: str, botVersion: str, localeId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes the specified intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_intent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_intent)
         """
-
     def delete_resource_policy(
         self, *, resourceArn: str, expectedRevisionId: str = ...
     ) -> DeleteResourcePolicyResponseTypeDef:
         """
         Removes an existing policy from a bot or bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_resource_policy)
         """
-
     def delete_resource_policy_statement(
         self, *, resourceArn: str, statementId: str, expectedRevisionId: str = ...
     ) -> DeleteResourcePolicyStatementResponseTypeDef:
         """
         Deletes a policy statement from a resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_resource_policy_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_resource_policy_statement)
         """
-
     def delete_slot(
         self, *, slotId: str, botId: str, botVersion: str, localeId: str, intentId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified slot from an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_slot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_slot)
         """
-
     def delete_slot_type(
         self,
         *,
         slotTypeId: str,
         botId: str,
         botVersion: str,
         localeId: str,
@@ -618,207 +609,186 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a slot type from a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_slot_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_slot_type)
         """
-
     def delete_test_set(self, *, testSetId: str) -> EmptyResponseMetadataTypeDef:
         """
         The action to delete the selected test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_test_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_test_set)
         """
-
     def delete_utterances(
         self, *, botId: str, localeId: str = ..., sessionId: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes stored utterances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_utterances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_utterances)
         """
-
     def describe_bot(self, *, botId: str) -> DescribeBotResponseTypeDef:
         """
         Provides metadata information about a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_bot)
         """
-
     def describe_bot_alias(self, *, botAliasId: str, botId: str) -> DescribeBotAliasResponseTypeDef:
         """
         Get information about a specific bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_bot_alias)
         """
-
     def describe_bot_locale(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> DescribeBotLocaleResponseTypeDef:
         """
         Describes the settings that a bot has for a specific locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_locale)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_bot_locale)
         """
-
     def describe_bot_recommendation(
         self, *, botId: str, botVersion: str, localeId: str, botRecommendationId: str
     ) -> DescribeBotRecommendationResponseTypeDef:
         """
         Provides metadata information about a bot recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_bot_recommendation)
         """
-
     def describe_bot_version(
         self, *, botId: str, botVersion: str
     ) -> DescribeBotVersionResponseTypeDef:
         """
         Provides metadata about a version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_bot_version)
         """
-
     def describe_custom_vocabulary_metadata(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> DescribeCustomVocabularyMetadataResponseTypeDef:
         """
         Provides metadata information about a custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_custom_vocabulary_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_custom_vocabulary_metadata)
         """
-
     def describe_export(self, *, exportId: str) -> DescribeExportResponseTypeDef:
         """
         Gets information about a specific export.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_export)
         """
-
     def describe_import(self, *, importId: str) -> DescribeImportResponseTypeDef:
         """
         Gets information about a specific import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_import)
         """
-
     def describe_intent(
         self, *, intentId: str, botId: str, botVersion: str, localeId: str
     ) -> DescribeIntentResponseTypeDef:
         """
         Returns metadata about an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_intent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_intent)
         """
-
     def describe_resource_policy(
         self, *, resourceArn: str
     ) -> DescribeResourcePolicyResponseTypeDef:
         """
         Gets the resource policy and policy revision for a bot or bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_resource_policy)
         """
-
     def describe_slot(
         self, *, slotId: str, botId: str, botVersion: str, localeId: str, intentId: str
     ) -> DescribeSlotResponseTypeDef:
         """
         Gets metadata information about a slot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_slot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_slot)
         """
-
     def describe_slot_type(
         self, *, slotTypeId: str, botId: str, botVersion: str, localeId: str
     ) -> DescribeSlotTypeResponseTypeDef:
         """
         Gets metadata information about a slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_slot_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_slot_type)
         """
-
     def describe_test_execution(
         self, *, testExecutionId: str
     ) -> DescribeTestExecutionResponseTypeDef:
         """
         Gets metadata information about the test execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_test_execution)
         """
-
     def describe_test_set(self, *, testSetId: str) -> DescribeTestSetResponseTypeDef:
         """
         Gets metadata information about the test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_test_set)
         """
-
     def describe_test_set_discrepancy_report(
         self, *, testSetDiscrepancyReportId: str
     ) -> DescribeTestSetDiscrepancyReportResponseTypeDef:
         """
         Gets metadata information about the test set discrepancy report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_set_discrepancy_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_test_set_discrepancy_report)
         """
-
     def describe_test_set_generation(
         self, *, testSetGenerationId: str
     ) -> DescribeTestSetGenerationResponseTypeDef:
         """
         Gets metadata information about the test set generation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_set_generation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_test_set_generation)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#generate_presigned_url)
         """
-
     def get_test_execution_artifacts_url(
         self, *, testExecutionId: str
     ) -> GetTestExecutionArtifactsUrlResponseTypeDef:
         """
         The pre-signed Amazon S3 URL to download the test execution result artifacts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_test_execution_artifacts_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_test_execution_artifacts_url)
         """
-
     def list_aggregated_utterances(
         self,
         *,
         botId: str,
         localeId: str,
         aggregationDuration: UtteranceAggregationDurationTypeDef,
         botAliasId: str = ...,
@@ -830,25 +800,23 @@
     ) -> ListAggregatedUtterancesResponseTypeDef:
         """
         Provides a list of utterances that users have sent to the bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_aggregated_utterances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_aggregated_utterances)
         """
-
     def list_bot_aliases(
         self, *, botId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListBotAliasesResponseTypeDef:
         """
         Gets a list of aliases for the specified bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_bot_aliases)
         """
-
     def list_bot_locales(
         self,
         *,
         botId: str,
         botVersion: str,
         sortBy: BotLocaleSortByTypeDef = ...,
         filters: Sequence[BotLocaleFilterTypeDef] = ...,
@@ -857,15 +825,14 @@
     ) -> ListBotLocalesResponseTypeDef:
         """
         Gets a list of locales for the specified bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_locales)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_bot_locales)
         """
-
     def list_bot_recommendations(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         maxResults: int = ...,
@@ -873,45 +840,42 @@
     ) -> ListBotRecommendationsResponseTypeDef:
         """
         Get a list of bot recommendations that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_bot_recommendations)
         """
-
     def list_bot_versions(
         self,
         *,
         botId: str,
         sortBy: BotVersionSortByTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListBotVersionsResponseTypeDef:
         """
         Gets information about all of the versions of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_bot_versions)
         """
-
     def list_bots(
         self,
         *,
         sortBy: BotSortByTypeDef = ...,
         filters: Sequence[BotFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListBotsResponseTypeDef:
         """
         Gets a list of available bots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_bots)
         """
-
     def list_built_in_intents(
         self,
         *,
         localeId: str,
         sortBy: BuiltInIntentSortByTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
@@ -919,30 +883,28 @@
         """
         Gets a list of built-in intents provided by Amazon Lex that you can use in your
         bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_intents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_built_in_intents)
         """
-
     def list_built_in_slot_types(
         self,
         *,
         localeId: str,
         sortBy: BuiltInSlotTypeSortByTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListBuiltInSlotTypesResponseTypeDef:
         """
         Gets a list of built-in slot types that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_slot_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_built_in_slot_types)
         """
-
     def list_custom_vocabulary_items(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         maxResults: int = ...,
@@ -951,15 +913,14 @@
         """
         Paginated list of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_custom_vocabulary_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_custom_vocabulary_items)
         """
-
     def list_exports(
         self,
         *,
         botId: str = ...,
         botVersion: str = ...,
         sortBy: ExportSortByTypeDef = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
@@ -969,15 +930,14 @@
     ) -> ListExportsResponseTypeDef:
         """
         Lists the exports for a bot, bot locale, or custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_exports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_exports)
         """
-
     def list_imports(
         self,
         *,
         botId: str = ...,
         botVersion: str = ...,
         sortBy: ImportSortByTypeDef = ...,
         filters: Sequence[ImportFilterTypeDef] = ...,
@@ -987,15 +947,68 @@
     ) -> ListImportsResponseTypeDef:
         """
         Lists the imports for a bot, bot locale, or custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_imports)
         """
+    def list_intent_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        metrics: Sequence[AnalyticsIntentMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsIntentGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsIntentFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListIntentMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the intents in your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_intent_metrics)
+        """
+    def list_intent_paths(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        intentPath: str,
+        filters: Sequence[AnalyticsPathFilterTypeDef] = ...
+    ) -> ListIntentPathsResponseTypeDef:
+        """
+        Retrieves summary statistics for a path of intents that users take over sessions
+        with your bot.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_paths)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_intent_paths)
+        """
+    def list_intent_stage_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        metrics: Sequence[AnalyticsIntentStageMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsIntentStageFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListIntentStageMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the intent stages in your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_stage_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_intent_stage_metrics)
+        """
     def list_intents(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: IntentSortByTypeDef = ...,
@@ -1005,15 +1018,14 @@
     ) -> ListIntentsResponseTypeDef:
         """
         Get a list of intents that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_intents)
         """
-
     def list_recommended_intents(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
@@ -1023,15 +1035,50 @@
         """
         Gets a list of recommended intents provided by the bot recommendation that you
         can use in your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_recommended_intents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_recommended_intents)
         """
+    def list_session_analytics_data(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        sortBy: SessionDataSortByTypeDef = ...,
+        filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListSessionAnalyticsDataResponseTypeDef:
+        """
+        Retrieves a list of metadata for individual user sessions with your bot.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_analytics_data)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_session_analytics_data)
+        """
+    def list_session_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        metrics: Sequence[AnalyticsSessionMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsSessionGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListSessionMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the user sessions with your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_session_metrics)
+        """
     def list_slot_types(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: SlotTypeSortByTypeDef = ...,
@@ -1041,15 +1088,14 @@
     ) -> ListSlotTypesResponseTypeDef:
         """
         Gets a list of slot types that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slot_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_slot_types)
         """
-
     def list_slots(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
@@ -1060,73 +1106,104 @@
     ) -> ListSlotsResponseTypeDef:
         """
         Gets a list of slots that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_slots)
         """
-
     def list_tags_for_resource(self, *, resourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Gets a list of tags associated with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_tags_for_resource)
         """
-
     def list_test_execution_result_items(
         self,
         *,
         testExecutionId: str,
         resultFilterBy: TestExecutionResultFilterByTypeDef,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListTestExecutionResultItemsResponseTypeDef:
         """
         Gets a list of test execution result items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_execution_result_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_test_execution_result_items)
         """
-
     def list_test_executions(
         self,
         *,
         sortBy: TestExecutionSortByTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListTestExecutionsResponseTypeDef:
         """
         The list of test set executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_test_executions)
         """
-
     def list_test_set_records(
         self, *, testSetId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListTestSetRecordsResponseTypeDef:
         """
         The list of test set records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_set_records)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_test_set_records)
         """
-
     def list_test_sets(
         self, *, sortBy: TestSetSortByTypeDef = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListTestSetsResponseTypeDef:
         """
         The list of the test sets See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/models.lex.v2-2020-08-07/ListTestSets).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_test_sets)
         """
+    def list_utterance_analytics_data(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        sortBy: UtteranceDataSortByTypeDef = ...,
+        filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListUtteranceAnalyticsDataResponseTypeDef:
+        """
+        Retrieves a list of metadata for individual user utterances to your bot.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_analytics_data)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_utterance_analytics_data)
+        """
+    def list_utterance_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        metrics: Sequence[AnalyticsUtteranceMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef] = ...,
+        attributes: Sequence[AnalyticsUtteranceAttributeTypeDef] = ...,
+        filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListUtteranceMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the utterances in your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_utterance_metrics)
+        """
     def search_associated_transcripts(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
@@ -1137,15 +1214,14 @@
     ) -> SearchAssociatedTranscriptsResponseTypeDef:
         """
         Search for associated transcripts that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.search_associated_transcripts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#search_associated_transcripts)
         """
-
     def start_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         transcriptSourceSetting: TranscriptSourceSettingTypeDef,
@@ -1154,15 +1230,14 @@
         """
         Use this to provide your transcript data, and to start the bot recommendation
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#start_bot_recommendation)
         """
-
     def start_import(
         self,
         *,
         importId: str,
         resourceSpecification: ImportResourceSpecificationTypeDef,
         mergeStrategy: MergeStrategyType,
         filePassword: str = ...
@@ -1170,30 +1245,28 @@
         """
         Starts importing a bot, bot locale, or custom vocabulary from a zip archive that
         you uploaded to an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#start_import)
         """
-
     def start_test_execution(
         self,
         *,
         testSetId: str,
         target: TestExecutionTargetTypeDef,
         apiMode: TestExecutionApiModeType,
         testExecutionModality: TestExecutionModalityType = ...
     ) -> StartTestExecutionResponseTypeDef:
         """
         The action to start test set execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_test_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#start_test_execution)
         """
-
     def start_test_set_generation(
         self,
         *,
         testSetName: str,
         storageLocation: TestSetStorageLocationTypeDef,
         generationDataSource: TestSetGenerationDataSourceTypeDef,
         roleArn: str,
@@ -1202,41 +1275,37 @@
     ) -> StartTestSetGenerationResponseTypeDef:
         """
         The action to start the generation of test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_test_set_generation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#start_test_set_generation)
         """
-
     def stop_bot_recommendation(
         self, *, botId: str, botVersion: str, localeId: str, botRecommendationId: str
     ) -> StopBotRecommendationResponseTypeDef:
         """
         Stop an already running Bot Recommendation request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.stop_bot_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#stop_bot_recommendation)
         """
-
     def tag_resource(self, *, resourceARN: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceARN: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a bot, bot alias, or bot channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#untag_resource)
         """
-
     def update_bot(
         self,
         *,
         botId: str,
         botName: str,
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
@@ -1247,15 +1316,14 @@
     ) -> UpdateBotResponseTypeDef:
         """
         Updates the configuration of an existing bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_bot)
         """
-
     def update_bot_alias(
         self,
         *,
         botAliasId: str,
         botAliasName: str,
         botId: str,
         description: str = ...,
@@ -1266,15 +1334,14 @@
     ) -> UpdateBotAliasResponseTypeDef:
         """
         Updates the configuration of an existing bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_bot_alias)
         """
-
     def update_bot_locale(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         nluIntentConfidenceThreshold: float,
@@ -1283,15 +1350,14 @@
     ) -> UpdateBotLocaleResponseTypeDef:
         """
         Updates the settings that a bot has for a specific locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_locale)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_bot_locale)
         """
-
     def update_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
@@ -1299,25 +1365,23 @@
     ) -> UpdateBotRecommendationResponseTypeDef:
         """
         Updates an existing bot recommendation request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_bot_recommendation)
         """
-
     def update_export(
         self, *, exportId: str, filePassword: str = ...
     ) -> UpdateExportResponseTypeDef:
         """
         Updates the password used to protect an export zip archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_export)
         """
-
     def update_intent(
         self,
         *,
         intentId: str,
         intentName: str,
         botId: str,
         botVersion: str,
@@ -1337,25 +1401,23 @@
     ) -> UpdateIntentResponseTypeDef:
         """
         Updates the settings for an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_intent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_intent)
         """
-
     def update_resource_policy(
         self, *, resourceArn: str, policy: str, expectedRevisionId: str = ...
     ) -> UpdateResourcePolicyResponseTypeDef:
         """
         Replaces the existing resource policy for a bot or bot alias with a new one.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_resource_policy)
         """
-
     def update_slot(
         self,
         *,
         slotId: str,
         slotName: str,
         valueElicitationSetting: SlotValueElicitationSettingTypeDef,
         botId: str,
@@ -1370,15 +1432,14 @@
     ) -> UpdateSlotResponseTypeDef:
         """
         Updates the settings for a slot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_slot)
         """
-
     def update_slot_type(
         self,
         *,
         slotTypeId: str,
         slotTypeName: str,
         botId: str,
         botVersion: str,
@@ -1392,76 +1453,67 @@
     ) -> UpdateSlotTypeResponseTypeDef:
         """
         Updates the configuration of an existing slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_slot_type)
         """
-
     def update_test_set(
         self, *, testSetId: str, testSetName: str, description: str = ...
     ) -> UpdateTestSetResponseTypeDef:
         """
         The action to update the test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_test_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_test_set)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["bot_alias_available"]) -> BotAliasAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["bot_available"]) -> BotAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["bot_export_completed"]) -> BotExportCompletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["bot_import_completed"]) -> BotImportCompletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["bot_locale_built"]) -> BotLocaleBuiltWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["bot_locale_created"]) -> BotLocaleCreatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["bot_locale_express_testing_available"]
     ) -> BotLocaleExpressTestingAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["bot_version_available"]
     ) -> BotVersionAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
```

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/client.pyi` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_lexv2_models.client import LexModelsV2Client
 
     session = Session()
     client: LexModelsV2Client = session.client("lexv2-models")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BotTypeType,
     EffectType,
     ImportExportFileFormatType,
@@ -26,14 +27,29 @@
     SearchOrderType,
     TestExecutionApiModeType,
     TestExecutionModalityType,
 )
 from .type_defs import (
     AggregatedUtterancesFilterTypeDef,
     AggregatedUtterancesSortByTypeDef,
+    AnalyticsBinBySpecificationTypeDef,
+    AnalyticsIntentFilterTypeDef,
+    AnalyticsIntentGroupBySpecificationTypeDef,
+    AnalyticsIntentMetricTypeDef,
+    AnalyticsIntentStageFilterTypeDef,
+    AnalyticsIntentStageGroupBySpecificationTypeDef,
+    AnalyticsIntentStageMetricTypeDef,
+    AnalyticsPathFilterTypeDef,
+    AnalyticsSessionFilterTypeDef,
+    AnalyticsSessionGroupBySpecificationTypeDef,
+    AnalyticsSessionMetricTypeDef,
+    AnalyticsUtteranceAttributeTypeDef,
+    AnalyticsUtteranceFilterTypeDef,
+    AnalyticsUtteranceGroupBySpecificationTypeDef,
+    AnalyticsUtteranceMetricTypeDef,
     AssociatedTranscriptFilterTypeDef,
     BatchCreateCustomVocabularyItemResponseTypeDef,
     BatchDeleteCustomVocabularyItemResponseTypeDef,
     BatchUpdateCustomVocabularyItemResponseTypeDef,
     BotAliasLocaleSettingsTypeDef,
     BotFilterTypeDef,
     BotLocaleFilterTypeDef,
@@ -113,31 +129,39 @@
     ListBotsResponseTypeDef,
     ListBotVersionsResponseTypeDef,
     ListBuiltInIntentsResponseTypeDef,
     ListBuiltInSlotTypesResponseTypeDef,
     ListCustomVocabularyItemsResponseTypeDef,
     ListExportsResponseTypeDef,
     ListImportsResponseTypeDef,
+    ListIntentMetricsResponseTypeDef,
+    ListIntentPathsResponseTypeDef,
     ListIntentsResponseTypeDef,
+    ListIntentStageMetricsResponseTypeDef,
     ListRecommendedIntentsResponseTypeDef,
+    ListSessionAnalyticsDataResponseTypeDef,
+    ListSessionMetricsResponseTypeDef,
     ListSlotsResponseTypeDef,
     ListSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestExecutionResultItemsResponseTypeDef,
     ListTestExecutionsResponseTypeDef,
     ListTestSetRecordsResponseTypeDef,
     ListTestSetsResponseTypeDef,
+    ListUtteranceAnalyticsDataResponseTypeDef,
+    ListUtteranceMetricsResponseTypeDef,
     MultipleValuesSettingTypeDef,
     NewCustomVocabularyItemTypeDef,
     ObfuscationSettingTypeDef,
     OutputContextTypeDef,
     PrincipalTypeDef,
     SampleUtteranceTypeDef,
     SearchAssociatedTranscriptsResponseTypeDef,
     SentimentAnalysisSettingsTypeDef,
+    SessionDataSortByTypeDef,
     SlotFilterTypeDef,
     SlotPriorityTypeDef,
     SlotSortByTypeDef,
     SlotTypeFilterTypeDef,
     SlotTypeSortByTypeDef,
     SlotTypeValueTypeDef,
     SlotValueElicitationSettingTypeDef,
@@ -163,14 +187,15 @@
     UpdateExportResponseTypeDef,
     UpdateIntentResponseTypeDef,
     UpdateResourcePolicyResponseTypeDef,
     UpdateSlotResponseTypeDef,
     UpdateSlotTypeResponseTypeDef,
     UpdateTestSetResponseTypeDef,
     UtteranceAggregationDurationTypeDef,
+    UtteranceDataSortByTypeDef,
     VoiceSettingsTypeDef,
 )
 from .waiter import (
     BotAliasAvailableWaiter,
     BotAvailableWaiter,
     BotExportCompletedWaiter,
     BotImportCompletedWaiter,
@@ -181,33 +206,37 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("LexModelsV2Client",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     PreconditionFailedException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class LexModelsV2Client(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/)
     """
 
     meta: ClientMeta
@@ -216,14 +245,15 @@
     def exceptions(self) -> Exceptions:
         """
         LexModelsV2Client exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#exceptions)
         """
+
     def batch_create_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[NewCustomVocabularyItemTypeDef]
@@ -231,14 +261,15 @@
         """
         Create a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_create_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_create_custom_vocabulary_item)
         """
+
     def batch_delete_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[CustomVocabularyEntryIdTypeDef]
@@ -246,14 +277,15 @@
         """
         Delete a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_delete_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_delete_custom_vocabulary_item)
         """
+
     def batch_update_custom_vocabulary_item(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         customVocabularyItemList: Sequence[CustomVocabularyItemTypeDef]
@@ -261,37 +293,41 @@
         """
         Update a batch of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.batch_update_custom_vocabulary_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#batch_update_custom_vocabulary_item)
         """
+
     def build_bot_locale(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> BuildBotLocaleResponseTypeDef:
         """
         Builds a bot, its intents, and its slot types into a specific locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.build_bot_locale)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#build_bot_locale)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#close)
         """
+
     def create_bot(
         self,
         *,
         botName: str,
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
         idleSessionTTLInSeconds: int,
@@ -303,14 +339,15 @@
     ) -> CreateBotResponseTypeDef:
         """
         Creates an Amazon Lex conversational bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_bot)
         """
+
     def create_bot_alias(
         self,
         *,
         botAliasName: str,
         botId: str,
         description: str = ...,
         botVersion: str = ...,
@@ -321,14 +358,15 @@
     ) -> CreateBotAliasResponseTypeDef:
         """
         Creates an alias for the specified version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_bot_alias)
         """
+
     def create_bot_locale(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         nluIntentConfidenceThreshold: float,
@@ -337,40 +375,43 @@
     ) -> CreateBotLocaleResponseTypeDef:
         """
         Creates a locale in the bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_locale)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_bot_locale)
         """
+
     def create_bot_version(
         self,
         *,
         botId: str,
         botVersionLocaleSpecification: Mapping[str, BotVersionLocaleDetailsTypeDef],
         description: str = ...
     ) -> CreateBotVersionResponseTypeDef:
         """
         Creates a new version of the bot based on the `DRAFT` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_bot_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_bot_version)
         """
+
     def create_export(
         self,
         *,
         resourceSpecification: ExportResourceSpecificationTypeDef,
         fileFormat: ImportExportFileFormatType,
         filePassword: str = ...
     ) -> CreateExportResponseTypeDef:
         """
         Creates a zip archive containing the contents of a bot or a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_export)
         """
+
     def create_intent(
         self,
         *,
         intentName: str,
         botId: str,
         botVersion: str,
         localeId: str,
@@ -388,23 +429,25 @@
     ) -> CreateIntentResponseTypeDef:
         """
         Creates an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_intent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_intent)
         """
+
     def create_resource_policy(
         self, *, resourceArn: str, policy: str
     ) -> CreateResourcePolicyResponseTypeDef:
         """
         Creates a new resource policy with the specified policy statements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_resource_policy)
         """
+
     def create_resource_policy_statement(
         self,
         *,
         resourceArn: str,
         statementId: str,
         effect: EffectType,
         principal: Sequence[PrincipalTypeDef],
@@ -414,14 +457,15 @@
     ) -> CreateResourcePolicyStatementResponseTypeDef:
         """
         Adds a new resource policy statement to a bot or bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_resource_policy_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_resource_policy_statement)
         """
+
     def create_slot(
         self,
         *,
         slotName: str,
         valueElicitationSetting: SlotValueElicitationSettingTypeDef,
         botId: str,
         botVersion: str,
@@ -435,14 +479,15 @@
     ) -> CreateSlotResponseTypeDef:
         """
         Creates a slot in an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_slot)
         """
+
     def create_slot_type(
         self,
         *,
         slotTypeName: str,
         botId: str,
         botVersion: str,
         localeId: str,
@@ -457,126 +502,140 @@
         Creates a custom slot type To create a custom slot type, specify a name for the
         slot type and a set of enumeration values, the values that a slot of this type
         can assume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_slot_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_slot_type)
         """
+
     def create_test_set_discrepancy_report(
         self, *, testSetId: str, target: TestSetDiscrepancyReportResourceTargetTypeDef
     ) -> CreateTestSetDiscrepancyReportResponseTypeDef:
         """
         Create a report that describes the differences between the bot and the test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_test_set_discrepancy_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_test_set_discrepancy_report)
         """
+
     def create_upload_url(self) -> CreateUploadUrlResponseTypeDef:
         """
         Gets a pre-signed S3 write URL that you use to upload the zip archive when
         importing a bot or a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.create_upload_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#create_upload_url)
         """
+
     def delete_bot(
         self, *, botId: str, skipResourceInUseCheck: bool = ...
     ) -> DeleteBotResponseTypeDef:
         """
         Deletes all versions of a bot, including the `Draft` version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_bot)
         """
+
     def delete_bot_alias(
         self, *, botAliasId: str, botId: str, skipResourceInUseCheck: bool = ...
     ) -> DeleteBotAliasResponseTypeDef:
         """
         Deletes the specified bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_bot_alias)
         """
+
     def delete_bot_locale(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> DeleteBotLocaleResponseTypeDef:
         """
         Removes a locale from a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_locale)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_bot_locale)
         """
+
     def delete_bot_version(
         self, *, botId: str, botVersion: str, skipResourceInUseCheck: bool = ...
     ) -> DeleteBotVersionResponseTypeDef:
         """
         Deletes a specific version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_bot_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_bot_version)
         """
+
     def delete_custom_vocabulary(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> DeleteCustomVocabularyResponseTypeDef:
         """
         Removes a custom vocabulary from the specified locale in the specified bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_custom_vocabulary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_custom_vocabulary)
         """
+
     def delete_export(self, *, exportId: str) -> DeleteExportResponseTypeDef:
         """
         Removes a previous export and the associated files stored in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_export)
         """
+
     def delete_import(self, *, importId: str) -> DeleteImportResponseTypeDef:
         """
         Removes a previous import and the associated file stored in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_import)
         """
+
     def delete_intent(
         self, *, intentId: str, botId: str, botVersion: str, localeId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes the specified intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_intent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_intent)
         """
+
     def delete_resource_policy(
         self, *, resourceArn: str, expectedRevisionId: str = ...
     ) -> DeleteResourcePolicyResponseTypeDef:
         """
         Removes an existing policy from a bot or bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_resource_policy)
         """
+
     def delete_resource_policy_statement(
         self, *, resourceArn: str, statementId: str, expectedRevisionId: str = ...
     ) -> DeleteResourcePolicyStatementResponseTypeDef:
         """
         Deletes a policy statement from a resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_resource_policy_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_resource_policy_statement)
         """
+
     def delete_slot(
         self, *, slotId: str, botId: str, botVersion: str, localeId: str, intentId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified slot from an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_slot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_slot)
         """
+
     def delete_slot_type(
         self,
         *,
         slotTypeId: str,
         botId: str,
         botVersion: str,
         localeId: str,
@@ -584,186 +643,207 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a slot type from a bot locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_slot_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_slot_type)
         """
+
     def delete_test_set(self, *, testSetId: str) -> EmptyResponseMetadataTypeDef:
         """
         The action to delete the selected test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_test_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_test_set)
         """
+
     def delete_utterances(
         self, *, botId: str, localeId: str = ..., sessionId: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes stored utterances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.delete_utterances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#delete_utterances)
         """
+
     def describe_bot(self, *, botId: str) -> DescribeBotResponseTypeDef:
         """
         Provides metadata information about a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_bot)
         """
+
     def describe_bot_alias(self, *, botAliasId: str, botId: str) -> DescribeBotAliasResponseTypeDef:
         """
         Get information about a specific bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_bot_alias)
         """
+
     def describe_bot_locale(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> DescribeBotLocaleResponseTypeDef:
         """
         Describes the settings that a bot has for a specific locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_locale)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_bot_locale)
         """
+
     def describe_bot_recommendation(
         self, *, botId: str, botVersion: str, localeId: str, botRecommendationId: str
     ) -> DescribeBotRecommendationResponseTypeDef:
         """
         Provides metadata information about a bot recommendation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_bot_recommendation)
         """
+
     def describe_bot_version(
         self, *, botId: str, botVersion: str
     ) -> DescribeBotVersionResponseTypeDef:
         """
         Provides metadata about a version of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_bot_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_bot_version)
         """
+
     def describe_custom_vocabulary_metadata(
         self, *, botId: str, botVersion: str, localeId: str
     ) -> DescribeCustomVocabularyMetadataResponseTypeDef:
         """
         Provides metadata information about a custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_custom_vocabulary_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_custom_vocabulary_metadata)
         """
+
     def describe_export(self, *, exportId: str) -> DescribeExportResponseTypeDef:
         """
         Gets information about a specific export.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_export)
         """
+
     def describe_import(self, *, importId: str) -> DescribeImportResponseTypeDef:
         """
         Gets information about a specific import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_import)
         """
+
     def describe_intent(
         self, *, intentId: str, botId: str, botVersion: str, localeId: str
     ) -> DescribeIntentResponseTypeDef:
         """
         Returns metadata about an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_intent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_intent)
         """
+
     def describe_resource_policy(
         self, *, resourceArn: str
     ) -> DescribeResourcePolicyResponseTypeDef:
         """
         Gets the resource policy and policy revision for a bot or bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_resource_policy)
         """
+
     def describe_slot(
         self, *, slotId: str, botId: str, botVersion: str, localeId: str, intentId: str
     ) -> DescribeSlotResponseTypeDef:
         """
         Gets metadata information about a slot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_slot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_slot)
         """
+
     def describe_slot_type(
         self, *, slotTypeId: str, botId: str, botVersion: str, localeId: str
     ) -> DescribeSlotTypeResponseTypeDef:
         """
         Gets metadata information about a slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_slot_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_slot_type)
         """
+
     def describe_test_execution(
         self, *, testExecutionId: str
     ) -> DescribeTestExecutionResponseTypeDef:
         """
         Gets metadata information about the test execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_test_execution)
         """
+
     def describe_test_set(self, *, testSetId: str) -> DescribeTestSetResponseTypeDef:
         """
         Gets metadata information about the test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_test_set)
         """
+
     def describe_test_set_discrepancy_report(
         self, *, testSetDiscrepancyReportId: str
     ) -> DescribeTestSetDiscrepancyReportResponseTypeDef:
         """
         Gets metadata information about the test set discrepancy report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_set_discrepancy_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_test_set_discrepancy_report)
         """
+
     def describe_test_set_generation(
         self, *, testSetGenerationId: str
     ) -> DescribeTestSetGenerationResponseTypeDef:
         """
         Gets metadata information about the test set generation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.describe_test_set_generation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#describe_test_set_generation)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#generate_presigned_url)
         """
+
     def get_test_execution_artifacts_url(
         self, *, testExecutionId: str
     ) -> GetTestExecutionArtifactsUrlResponseTypeDef:
         """
         The pre-signed Amazon S3 URL to download the test execution result artifacts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_test_execution_artifacts_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_test_execution_artifacts_url)
         """
+
     def list_aggregated_utterances(
         self,
         *,
         botId: str,
         localeId: str,
         aggregationDuration: UtteranceAggregationDurationTypeDef,
         botAliasId: str = ...,
@@ -775,23 +855,25 @@
     ) -> ListAggregatedUtterancesResponseTypeDef:
         """
         Provides a list of utterances that users have sent to the bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_aggregated_utterances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_aggregated_utterances)
         """
+
     def list_bot_aliases(
         self, *, botId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListBotAliasesResponseTypeDef:
         """
         Gets a list of aliases for the specified bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_bot_aliases)
         """
+
     def list_bot_locales(
         self,
         *,
         botId: str,
         botVersion: str,
         sortBy: BotLocaleSortByTypeDef = ...,
         filters: Sequence[BotLocaleFilterTypeDef] = ...,
@@ -800,14 +882,15 @@
     ) -> ListBotLocalesResponseTypeDef:
         """
         Gets a list of locales for the specified bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_locales)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_bot_locales)
         """
+
     def list_bot_recommendations(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         maxResults: int = ...,
@@ -815,42 +898,45 @@
     ) -> ListBotRecommendationsResponseTypeDef:
         """
         Get a list of bot recommendations that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_bot_recommendations)
         """
+
     def list_bot_versions(
         self,
         *,
         botId: str,
         sortBy: BotVersionSortByTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListBotVersionsResponseTypeDef:
         """
         Gets information about all of the versions of a bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bot_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_bot_versions)
         """
+
     def list_bots(
         self,
         *,
         sortBy: BotSortByTypeDef = ...,
         filters: Sequence[BotFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListBotsResponseTypeDef:
         """
         Gets a list of available bots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_bots)
         """
+
     def list_built_in_intents(
         self,
         *,
         localeId: str,
         sortBy: BuiltInIntentSortByTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
@@ -858,28 +944,30 @@
         """
         Gets a list of built-in intents provided by Amazon Lex that you can use in your
         bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_intents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_built_in_intents)
         """
+
     def list_built_in_slot_types(
         self,
         *,
         localeId: str,
         sortBy: BuiltInSlotTypeSortByTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListBuiltInSlotTypesResponseTypeDef:
         """
         Gets a list of built-in slot types that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_built_in_slot_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_built_in_slot_types)
         """
+
     def list_custom_vocabulary_items(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         maxResults: int = ...,
@@ -888,14 +976,15 @@
         """
         Paginated list of custom vocabulary items for a given bot locale's custom
         vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_custom_vocabulary_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_custom_vocabulary_items)
         """
+
     def list_exports(
         self,
         *,
         botId: str = ...,
         botVersion: str = ...,
         sortBy: ExportSortByTypeDef = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
@@ -905,14 +994,15 @@
     ) -> ListExportsResponseTypeDef:
         """
         Lists the exports for a bot, bot locale, or custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_exports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_exports)
         """
+
     def list_imports(
         self,
         *,
         botId: str = ...,
         botVersion: str = ...,
         sortBy: ImportSortByTypeDef = ...,
         filters: Sequence[ImportFilterTypeDef] = ...,
@@ -922,14 +1012,72 @@
     ) -> ListImportsResponseTypeDef:
         """
         Lists the imports for a bot, bot locale, or custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_imports)
         """
+
+    def list_intent_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        metrics: Sequence[AnalyticsIntentMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsIntentGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsIntentFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListIntentMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the intents in your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_intent_metrics)
+        """
+
+    def list_intent_paths(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        intentPath: str,
+        filters: Sequence[AnalyticsPathFilterTypeDef] = ...
+    ) -> ListIntentPathsResponseTypeDef:
+        """
+        Retrieves summary statistics for a path of intents that users take over sessions
+        with your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_paths)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_intent_paths)
+        """
+
+    def list_intent_stage_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        metrics: Sequence[AnalyticsIntentStageMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsIntentStageFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListIntentStageMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the intent stages in your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intent_stage_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_intent_stage_metrics)
+        """
+
     def list_intents(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: IntentSortByTypeDef = ...,
@@ -939,14 +1087,15 @@
     ) -> ListIntentsResponseTypeDef:
         """
         Get a list of intents that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_intents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_intents)
         """
+
     def list_recommended_intents(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
@@ -956,14 +1105,53 @@
         """
         Gets a list of recommended intents provided by the bot recommendation that you
         can use in your bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_recommended_intents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_recommended_intents)
         """
+
+    def list_session_analytics_data(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        sortBy: SessionDataSortByTypeDef = ...,
+        filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListSessionAnalyticsDataResponseTypeDef:
+        """
+        Retrieves a list of metadata for individual user sessions with your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_analytics_data)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_session_analytics_data)
+        """
+
+    def list_session_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        metrics: Sequence[AnalyticsSessionMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsSessionGroupBySpecificationTypeDef] = ...,
+        filters: Sequence[AnalyticsSessionFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListSessionMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the user sessions with your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_session_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_session_metrics)
+        """
+
     def list_slot_types(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         sortBy: SlotTypeSortByTypeDef = ...,
@@ -973,14 +1161,15 @@
     ) -> ListSlotTypesResponseTypeDef:
         """
         Gets a list of slot types that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slot_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_slot_types)
         """
+
     def list_slots(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         intentId: str,
@@ -991,67 +1180,112 @@
     ) -> ListSlotsResponseTypeDef:
         """
         Gets a list of slots that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_slots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_slots)
         """
+
     def list_tags_for_resource(self, *, resourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Gets a list of tags associated with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_tags_for_resource)
         """
+
     def list_test_execution_result_items(
         self,
         *,
         testExecutionId: str,
         resultFilterBy: TestExecutionResultFilterByTypeDef,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListTestExecutionResultItemsResponseTypeDef:
         """
         Gets a list of test execution result items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_execution_result_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_test_execution_result_items)
         """
+
     def list_test_executions(
         self,
         *,
         sortBy: TestExecutionSortByTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListTestExecutionsResponseTypeDef:
         """
         The list of test set executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_test_executions)
         """
+
     def list_test_set_records(
         self, *, testSetId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListTestSetRecordsResponseTypeDef:
         """
         The list of test set records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_set_records)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_test_set_records)
         """
+
     def list_test_sets(
         self, *, sortBy: TestSetSortByTypeDef = ..., maxResults: int = ..., nextToken: str = ...
     ) -> ListTestSetsResponseTypeDef:
         """
         The list of the test sets See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/models.lex.v2-2020-08-07/ListTestSets).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_test_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_test_sets)
         """
+
+    def list_utterance_analytics_data(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        sortBy: UtteranceDataSortByTypeDef = ...,
+        filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListUtteranceAnalyticsDataResponseTypeDef:
+        """
+        Retrieves a list of metadata for individual user utterances to your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_analytics_data)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_utterance_analytics_data)
+        """
+
+    def list_utterance_metrics(
+        self,
+        *,
+        botId: str,
+        startDateTime: Union[datetime, str],
+        endDateTime: Union[datetime, str],
+        metrics: Sequence[AnalyticsUtteranceMetricTypeDef],
+        binBy: Sequence[AnalyticsBinBySpecificationTypeDef] = ...,
+        groupBy: Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef] = ...,
+        attributes: Sequence[AnalyticsUtteranceAttributeTypeDef] = ...,
+        filters: Sequence[AnalyticsUtteranceFilterTypeDef] = ...,
+        maxResults: int = ...,
+        nextToken: str = ...
+    ) -> ListUtteranceMetricsResponseTypeDef:
+        """
+        Retrieves summary metrics for the utterances in your bot.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.list_utterance_metrics)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#list_utterance_metrics)
+        """
+
     def search_associated_transcripts(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
@@ -1062,14 +1296,15 @@
     ) -> SearchAssociatedTranscriptsResponseTypeDef:
         """
         Search for associated transcripts that meet the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.search_associated_transcripts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#search_associated_transcripts)
         """
+
     def start_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         transcriptSourceSetting: TranscriptSourceSettingTypeDef,
@@ -1078,14 +1313,15 @@
         """
         Use this to provide your transcript data, and to start the bot recommendation
         process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_bot_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#start_bot_recommendation)
         """
+
     def start_import(
         self,
         *,
         importId: str,
         resourceSpecification: ImportResourceSpecificationTypeDef,
         mergeStrategy: MergeStrategyType,
         filePassword: str = ...
@@ -1093,28 +1329,30 @@
         """
         Starts importing a bot, bot locale, or custom vocabulary from a zip archive that
         you uploaded to an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#start_import)
         """
+
     def start_test_execution(
         self,
         *,
         testSetId: str,
         target: TestExecutionTargetTypeDef,
         apiMode: TestExecutionApiModeType,
         testExecutionModality: TestExecutionModalityType = ...
     ) -> StartTestExecutionResponseTypeDef:
         """
         The action to start test set execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_test_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#start_test_execution)
         """
+
     def start_test_set_generation(
         self,
         *,
         testSetName: str,
         storageLocation: TestSetStorageLocationTypeDef,
         generationDataSource: TestSetGenerationDataSourceTypeDef,
         roleArn: str,
@@ -1123,37 +1361,41 @@
     ) -> StartTestSetGenerationResponseTypeDef:
         """
         The action to start the generation of test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.start_test_set_generation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#start_test_set_generation)
         """
+
     def stop_bot_recommendation(
         self, *, botId: str, botVersion: str, localeId: str, botRecommendationId: str
     ) -> StopBotRecommendationResponseTypeDef:
         """
         Stop an already running Bot Recommendation request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.stop_bot_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#stop_bot_recommendation)
         """
+
     def tag_resource(self, *, resourceARN: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceARN: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a bot, bot alias, or bot channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#untag_resource)
         """
+
     def update_bot(
         self,
         *,
         botId: str,
         botName: str,
         roleArn: str,
         dataPrivacy: DataPrivacyTypeDef,
@@ -1164,14 +1406,15 @@
     ) -> UpdateBotResponseTypeDef:
         """
         Updates the configuration of an existing bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_bot)
         """
+
     def update_bot_alias(
         self,
         *,
         botAliasId: str,
         botAliasName: str,
         botId: str,
         description: str = ...,
@@ -1182,14 +1425,15 @@
     ) -> UpdateBotAliasResponseTypeDef:
         """
         Updates the configuration of an existing bot alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_bot_alias)
         """
+
     def update_bot_locale(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         nluIntentConfidenceThreshold: float,
@@ -1198,14 +1442,15 @@
     ) -> UpdateBotLocaleResponseTypeDef:
         """
         Updates the settings that a bot has for a specific locale.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_locale)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_bot_locale)
         """
+
     def update_bot_recommendation(
         self,
         *,
         botId: str,
         botVersion: str,
         localeId: str,
         botRecommendationId: str,
@@ -1213,23 +1458,25 @@
     ) -> UpdateBotRecommendationResponseTypeDef:
         """
         Updates an existing bot recommendation request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_bot_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_bot_recommendation)
         """
+
     def update_export(
         self, *, exportId: str, filePassword: str = ...
     ) -> UpdateExportResponseTypeDef:
         """
         Updates the password used to protect an export zip archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_export)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_export)
         """
+
     def update_intent(
         self,
         *,
         intentId: str,
         intentName: str,
         botId: str,
         botVersion: str,
@@ -1249,23 +1496,25 @@
     ) -> UpdateIntentResponseTypeDef:
         """
         Updates the settings for an intent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_intent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_intent)
         """
+
     def update_resource_policy(
         self, *, resourceArn: str, policy: str, expectedRevisionId: str = ...
     ) -> UpdateResourcePolicyResponseTypeDef:
         """
         Replaces the existing resource policy for a bot or bot alias with a new one.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_resource_policy)
         """
+
     def update_slot(
         self,
         *,
         slotId: str,
         slotName: str,
         valueElicitationSetting: SlotValueElicitationSettingTypeDef,
         botId: str,
@@ -1280,14 +1529,15 @@
     ) -> UpdateSlotResponseTypeDef:
         """
         Updates the settings for a slot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_slot)
         """
+
     def update_slot_type(
         self,
         *,
         slotTypeId: str,
         slotTypeName: str,
         botId: str,
         botVersion: str,
@@ -1301,67 +1551,76 @@
     ) -> UpdateSlotTypeResponseTypeDef:
         """
         Updates the configuration of an existing slot type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_slot_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_slot_type)
         """
+
     def update_test_set(
         self, *, testSetId: str, testSetName: str, description: str = ...
     ) -> UpdateTestSetResponseTypeDef:
         """
         The action to update the test set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.update_test_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#update_test_set)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["bot_alias_available"]) -> BotAliasAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["bot_available"]) -> BotAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["bot_export_completed"]) -> BotExportCompletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["bot_import_completed"]) -> BotImportCompletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["bot_locale_built"]) -> BotLocaleBuiltWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["bot_locale_created"]) -> BotLocaleCreatedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["bot_locale_express_testing_available"]
     ) -> BotLocaleExpressTestingAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["bot_version_available"]
     ) -> BotVersionAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#LexModelsV2.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_models/client/#get_waiter)
```

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/literals.py` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/literals.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,19 +19,43 @@
     from typing_extensions import Literal
 
 
 __all__ = (
     "AggregatedUtterancesFilterNameType",
     "AggregatedUtterancesFilterOperatorType",
     "AggregatedUtterancesSortAttributeType",
+    "AnalyticsBinByNameType",
+    "AnalyticsCommonFilterNameType",
+    "AnalyticsFilterOperatorType",
+    "AnalyticsIntentFieldType",
+    "AnalyticsIntentFilterNameType",
+    "AnalyticsIntentMetricNameType",
+    "AnalyticsIntentStageFieldType",
+    "AnalyticsIntentStageFilterNameType",
+    "AnalyticsIntentStageMetricNameType",
+    "AnalyticsIntervalType",
+    "AnalyticsMetricStatisticType",
+    "AnalyticsModalityType",
+    "AnalyticsNodeTypeType",
+    "AnalyticsSessionFieldType",
+    "AnalyticsSessionFilterNameType",
+    "AnalyticsSessionMetricNameType",
+    "AnalyticsSessionSortByNameType",
+    "AnalyticsSortOrderType",
+    "AnalyticsUtteranceAttributeNameType",
+    "AnalyticsUtteranceFieldType",
+    "AnalyticsUtteranceFilterNameType",
+    "AnalyticsUtteranceMetricNameType",
+    "AnalyticsUtteranceSortByNameType",
     "AssociatedTranscriptFilterNameType",
     "AudioRecognitionStrategyType",
     "BotAliasAvailableWaiterName",
     "BotAliasStatusType",
     "BotAvailableWaiterName",
+    "BotChannelTypeType",
     "BotExportCompletedWaiterName",
     "BotFilterNameType",
     "BotFilterOperatorType",
     "BotImportCompletedWaiterName",
     "BotLocaleBuiltWaiterName",
     "BotLocaleCreatedWaiterName",
     "BotLocaleExpressTestingAvailableWaiterName",
@@ -43,14 +67,15 @@
     "BotSortAttributeType",
     "BotStatusType",
     "BotTypeType",
     "BotVersionAvailableWaiterName",
     "BotVersionSortAttributeType",
     "BuiltInIntentSortAttributeType",
     "BuiltInSlotTypeSortAttributeType",
+    "ConversationEndStateType",
     "ConversationLogsInputModeFilterType",
     "CustomVocabularyStatusType",
     "DialogActionTypeType",
     "EffectType",
     "ErrorCodeType",
     "ExportFilterNameType",
     "ExportFilterOperatorType",
@@ -61,14 +86,15 @@
     "ImportFilterOperatorType",
     "ImportResourceTypeType",
     "ImportSortAttributeType",
     "ImportStatusType",
     "IntentFilterNameType",
     "IntentFilterOperatorType",
     "IntentSortAttributeType",
+    "IntentStateType",
     "MergeStrategyType",
     "MessageSelectionStrategyType",
     "ObfuscationSettingTypeType",
     "PromptAttemptType",
     "SearchOrderType",
     "SlotConstraintType",
     "SlotFilterNameType",
@@ -90,31 +116,101 @@
     "TestSetDiscrepancyReportStatusType",
     "TestSetGenerationStatusType",
     "TestSetModalityType",
     "TestSetSortAttributeType",
     "TestSetStatusType",
     "TimeDimensionType",
     "TranscriptFormatType",
+    "UtteranceContentTypeType",
     "VoiceEngineType",
     "LexModelsV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "WaiterName",
     "RegionName",
 )
 
 
 AggregatedUtterancesFilterNameType = Literal["Utterance"]
 AggregatedUtterancesFilterOperatorType = Literal["CO", "EQ"]
 AggregatedUtterancesSortAttributeType = Literal["HitCount", "MissedCount"]
+AnalyticsBinByNameType = Literal["ConversationStartTime", "UtteranceTimestamp"]
+AnalyticsCommonFilterNameType = Literal[
+    "BotAliasId", "BotVersion", "Channel", "LocaleId", "Modality"
+]
+AnalyticsFilterOperatorType = Literal["EQ", "GT", "LT"]
+AnalyticsIntentFieldType = Literal["IntentEndState", "IntentLevel", "IntentName"]
+AnalyticsIntentFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "IntentEndState",
+    "IntentName",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsIntentMetricNameType = Literal["Count", "Dropped", "Failure", "Success", "Switched"]
+AnalyticsIntentStageFieldType = Literal["IntentStageName", "SwitchedToIntent"]
+AnalyticsIntentStageFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "IntentName",
+    "IntentStageName",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsIntentStageMetricNameType = Literal["Count", "Dropped", "Failed", "Retry", "Success"]
+AnalyticsIntervalType = Literal["OneDay", "OneHour"]
+AnalyticsMetricStatisticType = Literal["Avg", "Max", "Sum"]
+AnalyticsModalityType = Literal["DTMF", "MultiMode", "Speech", "Text"]
+AnalyticsNodeTypeType = Literal["Exit", "Inner"]
+AnalyticsSessionFieldType = Literal["ConversationEndState", "LocaleId"]
+AnalyticsSessionFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "ConversationEndState",
+    "Duration",
+    "IntentPath",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsSessionMetricNameType = Literal[
+    "Concurrency", "Count", "Dropped", "Duration", "Failure", "Success", "TurnsPerConversation"
+]
+AnalyticsSessionSortByNameType = Literal["ConversationStartTime", "Duration", "NumberOfTurns"]
+AnalyticsSortOrderType = Literal["Ascending", "Descending"]
+AnalyticsUtteranceAttributeNameType = Literal["LastUsedIntent"]
+AnalyticsUtteranceFieldType = Literal["UtteranceState", "UtteranceText"]
+AnalyticsUtteranceFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+    "UtteranceState",
+    "UtteranceText",
+]
+AnalyticsUtteranceMetricNameType = Literal["Count", "Detected", "Missed", "UtteranceTimestamp"]
+AnalyticsUtteranceSortByNameType = Literal["UtteranceTimestamp"]
 AssociatedTranscriptFilterNameType = Literal["IntentId", "SlotTypeId"]
 AudioRecognitionStrategyType = Literal["UseSlotValuesAsCustomVocabulary"]
 BotAliasAvailableWaiterName = Literal["bot_alias_available"]
 BotAliasStatusType = Literal["Available", "Creating", "Deleting", "Failed"]
 BotAvailableWaiterName = Literal["bot_available"]
+BotChannelTypeType = Literal["Facebook", "Slack", "TwilioSms"]
 BotExportCompletedWaiterName = Literal["bot_export_completed"]
 BotFilterNameType = Literal["BotName", "BotType"]
 BotFilterOperatorType = Literal["CO", "EQ", "NE"]
 BotImportCompletedWaiterName = Literal["bot_import_completed"]
 BotLocaleBuiltWaiterName = Literal["bot_locale_built"]
 BotLocaleCreatedWaiterName = Literal["bot_locale_created"]
 BotLocaleExpressTestingAvailableWaiterName = Literal["bot_locale_express_testing_available"]
@@ -148,14 +244,15 @@
     "Available", "Creating", "Deleting", "Failed", "Importing", "Inactive", "Updating", "Versioning"
 ]
 BotTypeType = Literal["Bot", "BotNetwork"]
 BotVersionAvailableWaiterName = Literal["bot_version_available"]
 BotVersionSortAttributeType = Literal["BotVersion"]
 BuiltInIntentSortAttributeType = Literal["IntentSignature"]
 BuiltInSlotTypeSortAttributeType = Literal["SlotTypeSignature"]
+ConversationEndStateType = Literal["Dropped", "Failure", "Success"]
 ConversationLogsInputModeFilterType = Literal["Speech", "Text"]
 CustomVocabularyStatusType = Literal["Creating", "Deleting", "Exporting", "Importing", "Ready"]
 DialogActionTypeType = Literal[
     "CloseIntent",
     "ConfirmIntent",
     "ElicitIntent",
     "ElicitSlot",
@@ -181,14 +278,17 @@
 ImportFilterOperatorType = Literal["CO", "EQ"]
 ImportResourceTypeType = Literal["Bot", "BotLocale", "CustomVocabulary", "TestSet"]
 ImportSortAttributeType = Literal["LastUpdatedDateTime"]
 ImportStatusType = Literal["Completed", "Deleting", "Failed", "InProgress"]
 IntentFilterNameType = Literal["IntentName"]
 IntentFilterOperatorType = Literal["CO", "EQ"]
 IntentSortAttributeType = Literal["IntentName", "LastUpdatedDateTime"]
+IntentStateType = Literal[
+    "Failed", "Fulfilled", "FulfillmentInProgress", "InProgress", "ReadyForFulfillment", "Waiting"
+]
 MergeStrategyType = Literal["Append", "FailOnConflict", "Overwrite"]
 MessageSelectionStrategyType = Literal["Ordered", "Random"]
 ObfuscationSettingTypeType = Literal["DefaultObfuscation", "None"]
 PromptAttemptType = Literal["Initial", "Retry1", "Retry2", "Retry3", "Retry4", "Retry5"]
 SearchOrderType = Literal["Ascending", "Descending"]
 SlotConstraintType = Literal["Optional", "Required"]
 SlotFilterNameType = Literal["SlotName"]
@@ -220,14 +320,15 @@
 TestSetModalityType = Literal["Audio", "Text"]
 TestSetSortAttributeType = Literal["LastUpdatedDateTime", "TestSetName"]
 TestSetStatusType = Literal[
     "Deleting", "Importing", "PendingAnnotation", "Ready", "ValidationError"
 ]
 TimeDimensionType = Literal["Days", "Hours", "Weeks"]
 TranscriptFormatType = Literal["Lex"]
+UtteranceContentTypeType = Literal["CustomPayload", "ImageResponseCard", "PlainText", "SSML"]
 VoiceEngineType = Literal["neural", "standard"]
 LexModelsV2ServiceName = Literal["lexv2-models"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
```

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/literals.pyi` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/literals.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -18,19 +18,43 @@
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AggregatedUtterancesFilterNameType",
     "AggregatedUtterancesFilterOperatorType",
     "AggregatedUtterancesSortAttributeType",
+    "AnalyticsBinByNameType",
+    "AnalyticsCommonFilterNameType",
+    "AnalyticsFilterOperatorType",
+    "AnalyticsIntentFieldType",
+    "AnalyticsIntentFilterNameType",
+    "AnalyticsIntentMetricNameType",
+    "AnalyticsIntentStageFieldType",
+    "AnalyticsIntentStageFilterNameType",
+    "AnalyticsIntentStageMetricNameType",
+    "AnalyticsIntervalType",
+    "AnalyticsMetricStatisticType",
+    "AnalyticsModalityType",
+    "AnalyticsNodeTypeType",
+    "AnalyticsSessionFieldType",
+    "AnalyticsSessionFilterNameType",
+    "AnalyticsSessionMetricNameType",
+    "AnalyticsSessionSortByNameType",
+    "AnalyticsSortOrderType",
+    "AnalyticsUtteranceAttributeNameType",
+    "AnalyticsUtteranceFieldType",
+    "AnalyticsUtteranceFilterNameType",
+    "AnalyticsUtteranceMetricNameType",
+    "AnalyticsUtteranceSortByNameType",
     "AssociatedTranscriptFilterNameType",
     "AudioRecognitionStrategyType",
     "BotAliasAvailableWaiterName",
     "BotAliasStatusType",
     "BotAvailableWaiterName",
+    "BotChannelTypeType",
     "BotExportCompletedWaiterName",
     "BotFilterNameType",
     "BotFilterOperatorType",
     "BotImportCompletedWaiterName",
     "BotLocaleBuiltWaiterName",
     "BotLocaleCreatedWaiterName",
     "BotLocaleExpressTestingAvailableWaiterName",
@@ -42,14 +66,15 @@
     "BotSortAttributeType",
     "BotStatusType",
     "BotTypeType",
     "BotVersionAvailableWaiterName",
     "BotVersionSortAttributeType",
     "BuiltInIntentSortAttributeType",
     "BuiltInSlotTypeSortAttributeType",
+    "ConversationEndStateType",
     "ConversationLogsInputModeFilterType",
     "CustomVocabularyStatusType",
     "DialogActionTypeType",
     "EffectType",
     "ErrorCodeType",
     "ExportFilterNameType",
     "ExportFilterOperatorType",
@@ -60,14 +85,15 @@
     "ImportFilterOperatorType",
     "ImportResourceTypeType",
     "ImportSortAttributeType",
     "ImportStatusType",
     "IntentFilterNameType",
     "IntentFilterOperatorType",
     "IntentSortAttributeType",
+    "IntentStateType",
     "MergeStrategyType",
     "MessageSelectionStrategyType",
     "ObfuscationSettingTypeType",
     "PromptAttemptType",
     "SearchOrderType",
     "SlotConstraintType",
     "SlotFilterNameType",
@@ -89,30 +115,100 @@
     "TestSetDiscrepancyReportStatusType",
     "TestSetGenerationStatusType",
     "TestSetModalityType",
     "TestSetSortAttributeType",
     "TestSetStatusType",
     "TimeDimensionType",
     "TranscriptFormatType",
+    "UtteranceContentTypeType",
     "VoiceEngineType",
     "LexModelsV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "WaiterName",
     "RegionName",
 )
 
 AggregatedUtterancesFilterNameType = Literal["Utterance"]
 AggregatedUtterancesFilterOperatorType = Literal["CO", "EQ"]
 AggregatedUtterancesSortAttributeType = Literal["HitCount", "MissedCount"]
+AnalyticsBinByNameType = Literal["ConversationStartTime", "UtteranceTimestamp"]
+AnalyticsCommonFilterNameType = Literal[
+    "BotAliasId", "BotVersion", "Channel", "LocaleId", "Modality"
+]
+AnalyticsFilterOperatorType = Literal["EQ", "GT", "LT"]
+AnalyticsIntentFieldType = Literal["IntentEndState", "IntentLevel", "IntentName"]
+AnalyticsIntentFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "IntentEndState",
+    "IntentName",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsIntentMetricNameType = Literal["Count", "Dropped", "Failure", "Success", "Switched"]
+AnalyticsIntentStageFieldType = Literal["IntentStageName", "SwitchedToIntent"]
+AnalyticsIntentStageFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "IntentName",
+    "IntentStageName",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsIntentStageMetricNameType = Literal["Count", "Dropped", "Failed", "Retry", "Success"]
+AnalyticsIntervalType = Literal["OneDay", "OneHour"]
+AnalyticsMetricStatisticType = Literal["Avg", "Max", "Sum"]
+AnalyticsModalityType = Literal["DTMF", "MultiMode", "Speech", "Text"]
+AnalyticsNodeTypeType = Literal["Exit", "Inner"]
+AnalyticsSessionFieldType = Literal["ConversationEndState", "LocaleId"]
+AnalyticsSessionFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "ConversationEndState",
+    "Duration",
+    "IntentPath",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+]
+AnalyticsSessionMetricNameType = Literal[
+    "Concurrency", "Count", "Dropped", "Duration", "Failure", "Success", "TurnsPerConversation"
+]
+AnalyticsSessionSortByNameType = Literal["ConversationStartTime", "Duration", "NumberOfTurns"]
+AnalyticsSortOrderType = Literal["Ascending", "Descending"]
+AnalyticsUtteranceAttributeNameType = Literal["LastUsedIntent"]
+AnalyticsUtteranceFieldType = Literal["UtteranceState", "UtteranceText"]
+AnalyticsUtteranceFilterNameType = Literal[
+    "BotAliasId",
+    "BotVersion",
+    "Channel",
+    "LocaleId",
+    "Modality",
+    "OriginatingRequestId",
+    "SessionId",
+    "UtteranceState",
+    "UtteranceText",
+]
+AnalyticsUtteranceMetricNameType = Literal["Count", "Detected", "Missed", "UtteranceTimestamp"]
+AnalyticsUtteranceSortByNameType = Literal["UtteranceTimestamp"]
 AssociatedTranscriptFilterNameType = Literal["IntentId", "SlotTypeId"]
 AudioRecognitionStrategyType = Literal["UseSlotValuesAsCustomVocabulary"]
 BotAliasAvailableWaiterName = Literal["bot_alias_available"]
 BotAliasStatusType = Literal["Available", "Creating", "Deleting", "Failed"]
 BotAvailableWaiterName = Literal["bot_available"]
+BotChannelTypeType = Literal["Facebook", "Slack", "TwilioSms"]
 BotExportCompletedWaiterName = Literal["bot_export_completed"]
 BotFilterNameType = Literal["BotName", "BotType"]
 BotFilterOperatorType = Literal["CO", "EQ", "NE"]
 BotImportCompletedWaiterName = Literal["bot_import_completed"]
 BotLocaleBuiltWaiterName = Literal["bot_locale_built"]
 BotLocaleCreatedWaiterName = Literal["bot_locale_created"]
 BotLocaleExpressTestingAvailableWaiterName = Literal["bot_locale_express_testing_available"]
@@ -146,14 +242,15 @@
     "Available", "Creating", "Deleting", "Failed", "Importing", "Inactive", "Updating", "Versioning"
 ]
 BotTypeType = Literal["Bot", "BotNetwork"]
 BotVersionAvailableWaiterName = Literal["bot_version_available"]
 BotVersionSortAttributeType = Literal["BotVersion"]
 BuiltInIntentSortAttributeType = Literal["IntentSignature"]
 BuiltInSlotTypeSortAttributeType = Literal["SlotTypeSignature"]
+ConversationEndStateType = Literal["Dropped", "Failure", "Success"]
 ConversationLogsInputModeFilterType = Literal["Speech", "Text"]
 CustomVocabularyStatusType = Literal["Creating", "Deleting", "Exporting", "Importing", "Ready"]
 DialogActionTypeType = Literal[
     "CloseIntent",
     "ConfirmIntent",
     "ElicitIntent",
     "ElicitSlot",
@@ -179,14 +276,17 @@
 ImportFilterOperatorType = Literal["CO", "EQ"]
 ImportResourceTypeType = Literal["Bot", "BotLocale", "CustomVocabulary", "TestSet"]
 ImportSortAttributeType = Literal["LastUpdatedDateTime"]
 ImportStatusType = Literal["Completed", "Deleting", "Failed", "InProgress"]
 IntentFilterNameType = Literal["IntentName"]
 IntentFilterOperatorType = Literal["CO", "EQ"]
 IntentSortAttributeType = Literal["IntentName", "LastUpdatedDateTime"]
+IntentStateType = Literal[
+    "Failed", "Fulfilled", "FulfillmentInProgress", "InProgress", "ReadyForFulfillment", "Waiting"
+]
 MergeStrategyType = Literal["Append", "FailOnConflict", "Overwrite"]
 MessageSelectionStrategyType = Literal["Ordered", "Random"]
 ObfuscationSettingTypeType = Literal["DefaultObfuscation", "None"]
 PromptAttemptType = Literal["Initial", "Retry1", "Retry2", "Retry3", "Retry4", "Retry5"]
 SearchOrderType = Literal["Ascending", "Descending"]
 SlotConstraintType = Literal["Optional", "Required"]
 SlotFilterNameType = Literal["SlotName"]
@@ -218,14 +318,15 @@
 TestSetModalityType = Literal["Audio", "Text"]
 TestSetSortAttributeType = Literal["LastUpdatedDateTime", "TestSetName"]
 TestSetStatusType = Literal[
     "Deleting", "Importing", "PendingAnnotation", "Ready", "ValidationError"
 ]
 TimeDimensionType = Literal["Days", "Hours", "Weeks"]
 TranscriptFormatType = Literal["Lex"]
+UtteranceContentTypeType = Literal["CustomPayload", "ImageResponseCard", "PlainText", "SSML"]
 VoiceEngineType = Literal["neural", "standard"]
 LexModelsV2ServiceName = Literal["lexv2-models"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
```

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/type_defs.py` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,41 +9,65 @@
     from mypy_boto3_lexv2_models.type_defs import ActiveContextTypeDef
 
     data: ActiveContextTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregatedUtterancesFilterOperatorType,
     AggregatedUtterancesSortAttributeType,
+    AnalyticsBinByNameType,
+    AnalyticsCommonFilterNameType,
+    AnalyticsFilterOperatorType,
+    AnalyticsIntentFieldType,
+    AnalyticsIntentFilterNameType,
+    AnalyticsIntentMetricNameType,
+    AnalyticsIntentStageFieldType,
+    AnalyticsIntentStageFilterNameType,
+    AnalyticsIntentStageMetricNameType,
+    AnalyticsIntervalType,
+    AnalyticsMetricStatisticType,
+    AnalyticsModalityType,
+    AnalyticsNodeTypeType,
+    AnalyticsSessionFieldType,
+    AnalyticsSessionFilterNameType,
+    AnalyticsSessionMetricNameType,
+    AnalyticsSessionSortByNameType,
+    AnalyticsSortOrderType,
+    AnalyticsUtteranceFieldType,
+    AnalyticsUtteranceFilterNameType,
+    AnalyticsUtteranceMetricNameType,
     AssociatedTranscriptFilterNameType,
     BotAliasStatusType,
+    BotChannelTypeType,
     BotFilterNameType,
     BotFilterOperatorType,
     BotLocaleFilterOperatorType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotStatusType,
     BotTypeType,
+    ConversationEndStateType,
     ConversationLogsInputModeFilterType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
     ErrorCodeType,
     ExportFilterOperatorType,
     ExportStatusType,
     ImportExportFileFormatType,
     ImportFilterOperatorType,
     ImportResourceTypeType,
     ImportStatusType,
     IntentFilterOperatorType,
     IntentSortAttributeType,
+    IntentStateType,
     MergeStrategyType,
     MessageSelectionStrategyType,
     ObfuscationSettingTypeType,
     PromptAttemptType,
     SearchOrderType,
     SlotConstraintType,
     SlotFilterOperatorType,
@@ -63,14 +87,15 @@
     TestResultTypeFilterType,
     TestSetDiscrepancyReportStatusType,
     TestSetGenerationStatusType,
     TestSetModalityType,
     TestSetSortAttributeType,
     TestSetStatusType,
     TimeDimensionType,
+    UtteranceContentTypeType,
     VoiceEngineType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -78,83 +103,140 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActiveContextTypeDef",
+    "AdvancedRecognitionSettingOutputTypeDef",
     "AdvancedRecognitionSettingTypeDef",
     "ExecutionErrorDetailsTypeDef",
     "AgentTurnSpecificationTypeDef",
     "AggregatedUtterancesFilterTypeDef",
     "AggregatedUtterancesSortByTypeDef",
     "AggregatedUtterancesSummaryTypeDef",
+    "AllowedInputTypesOutputTypeDef",
     "AllowedInputTypesTypeDef",
+    "AnalyticsBinBySpecificationTypeDef",
+    "AnalyticsBinKeyTypeDef",
+    "AnalyticsIntentFilterTypeDef",
+    "AnalyticsIntentGroupByKeyTypeDef",
+    "AnalyticsIntentGroupBySpecificationTypeDef",
+    "AnalyticsIntentMetricResultTypeDef",
+    "AnalyticsIntentMetricTypeDef",
+    "AnalyticsIntentNodeSummaryTypeDef",
+    "AnalyticsIntentStageFilterTypeDef",
+    "AnalyticsIntentStageGroupByKeyTypeDef",
+    "AnalyticsIntentStageGroupBySpecificationTypeDef",
+    "AnalyticsIntentStageMetricResultTypeDef",
+    "AnalyticsIntentStageMetricTypeDef",
+    "AnalyticsPathFilterTypeDef",
+    "AnalyticsSessionFilterTypeDef",
+    "AnalyticsSessionGroupByKeyTypeDef",
+    "AnalyticsSessionGroupBySpecificationTypeDef",
+    "AnalyticsSessionMetricResultTypeDef",
+    "AnalyticsSessionMetricTypeDef",
+    "AnalyticsUtteranceAttributeResultTypeDef",
+    "AnalyticsUtteranceAttributeTypeDef",
+    "AnalyticsUtteranceFilterTypeDef",
+    "AnalyticsUtteranceGroupByKeyTypeDef",
+    "AnalyticsUtteranceGroupBySpecificationTypeDef",
+    "AnalyticsUtteranceMetricResultTypeDef",
+    "AnalyticsUtteranceMetricTypeDef",
     "AssociatedTranscriptFilterTypeDef",
     "AssociatedTranscriptTypeDef",
+    "AudioSpecificationOutputTypeDef",
+    "DTMFSpecificationOutputTypeDef",
     "AudioSpecificationTypeDef",
     "DTMFSpecificationTypeDef",
+    "S3BucketLogDestinationOutputTypeDef",
     "S3BucketLogDestinationTypeDef",
     "NewCustomVocabularyItemTypeDef",
-    "CustomVocabularyItemTypeDef",
+    "CustomVocabularyItemOutputTypeDef",
     "FailedCustomVocabularyItemTypeDef",
     "CustomVocabularyEntryIdTypeDef",
+    "CustomVocabularyItemTypeDef",
     "BotAliasHistoryEventTypeDef",
     "BotAliasSummaryTypeDef",
+    "BotAliasTestExecutionTargetOutputTypeDef",
     "BotAliasTestExecutionTargetTypeDef",
+    "BotExportSpecificationOutputTypeDef",
     "BotExportSpecificationTypeDef",
     "BotFilterTypeDef",
+    "DataPrivacyOutputTypeDef",
     "DataPrivacyTypeDef",
+    "BotLocaleExportSpecificationOutputTypeDef",
     "BotLocaleExportSpecificationTypeDef",
     "BotLocaleFilterTypeDef",
     "BotLocaleHistoryEventTypeDef",
+    "VoiceSettingsOutputTypeDef",
     "VoiceSettingsTypeDef",
     "BotLocaleSortByTypeDef",
     "BotLocaleSummaryTypeDef",
+    "BotMemberOutputTypeDef",
     "BotMemberTypeDef",
     "IntentStatisticsTypeDef",
     "SlotTypeStatisticsTypeDef",
     "BotRecommendationSummaryTypeDef",
     "BotSortByTypeDef",
     "BotSummaryTypeDef",
+    "BotVersionLocaleDetailsOutputTypeDef",
     "BotVersionLocaleDetailsTypeDef",
     "BotVersionSortByTypeDef",
     "BotVersionSummaryTypeDef",
     "BuildBotLocaleRequestRequestTypeDef",
     "BuildBotLocaleResponseTypeDef",
     "BuiltInIntentSortByTypeDef",
     "BuiltInIntentSummaryTypeDef",
     "BuiltInSlotTypeSortByTypeDef",
     "BuiltInSlotTypeSummaryTypeDef",
+    "ButtonOutputTypeDef",
     "ButtonTypeDef",
+    "CloudWatchLogGroupLogDestinationOutputTypeDef",
     "CloudWatchLogGroupLogDestinationTypeDef",
+    "LambdaCodeHookOutputTypeDef",
     "LambdaCodeHookTypeDef",
+    "SubSlotTypeCompositionOutputTypeDef",
     "SubSlotTypeCompositionTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "ConversationLevelIntentClassificationResultItemTypeDef",
     "ConversationLevelResultDetailTypeDef",
     "ConversationLevelSlotResolutionResultItemTypeDef",
     "ConversationLevelTestResultsFilterByTypeDef",
+    "ConversationLogsDataSourceFilterByOutputTypeDef",
     "ConversationLogsDataSourceFilterByTypeDef",
     "SentimentAnalysisSettingsTypeDef",
+    "SentimentAnalysisSettingsOutputTypeDef",
     "DialogCodeHookSettingsTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "SampleUtteranceTypeDef",
+    "DialogCodeHookSettingsOutputTypeDef",
+    "InputContextOutputTypeDef",
+    "KendraConfigurationOutputTypeDef",
+    "OutputContextOutputTypeDef",
+    "SampleUtteranceOutputTypeDef",
     "CreateResourcePolicyRequestRequestTypeDef",
     "CreateResourcePolicyResponseTypeDef",
     "PrincipalTypeDef",
     "CreateResourcePolicyStatementResponseTypeDef",
     "MultipleValuesSettingTypeDef",
     "ObfuscationSettingTypeDef",
+    "MultipleValuesSettingOutputTypeDef",
+    "ObfuscationSettingOutputTypeDef",
     "CreateUploadUrlResponseTypeDef",
+    "CustomPayloadOutputTypeDef",
     "CustomPayloadTypeDef",
+    "CustomVocabularyExportSpecificationOutputTypeDef",
     "CustomVocabularyExportSpecificationTypeDef",
+    "CustomVocabularyImportSpecificationOutputTypeDef",
     "CustomVocabularyImportSpecificationTypeDef",
+    "DateRangeFilterOutputTypeDef",
     "DateRangeFilterTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotAliasResponseTypeDef",
     "DeleteBotLocaleRequestRequestTypeDef",
     "DeleteBotLocaleResponseTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotResponseTypeDef",
@@ -176,294 +258,400 @@
     "DeleteTestSetRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeBotAliasRequestRequestTypeDef",
     "ParentBotNetworkTypeDef",
     "DescribeBotLocaleRequestRequestTypeDef",
     "DescribeBotRecommendationRequestRequestTypeDef",
-    "EncryptionSettingTypeDef",
+    "EncryptionSettingOutputTypeDef",
     "DescribeBotRequestRequestTypeDef",
     "DescribeBotVersionRequestRequestTypeDef",
     "DescribeCustomVocabularyMetadataRequestRequestTypeDef",
     "DescribeCustomVocabularyMetadataResponseTypeDef",
     "DescribeExportRequestRequestTypeDef",
     "DescribeImportRequestRequestTypeDef",
     "DescribeIntentRequestRequestTypeDef",
-    "SlotPriorityTypeDef",
+    "SlotPriorityOutputTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
     "DescribeResourcePolicyResponseTypeDef",
     "DescribeSlotRequestRequestTypeDef",
     "DescribeSlotTypeRequestRequestTypeDef",
     "DescribeTestExecutionRequestRequestTypeDef",
     "DescribeTestSetDiscrepancyReportRequestRequestTypeDef",
     "DescribeTestSetGenerationRequestRequestTypeDef",
-    "TestSetStorageLocationTypeDef",
+    "TestSetStorageLocationOutputTypeDef",
     "DescribeTestSetRequestRequestTypeDef",
+    "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
+    "IntentOverrideOutputTypeDef",
     "IntentOverrideTypeDef",
+    "ElicitationCodeHookInvocationSettingOutputTypeDef",
     "ElicitationCodeHookInvocationSettingTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionSettingTypeDef",
     "ExportFilterTypeDef",
+    "TestSetExportSpecificationOutputTypeDef",
     "TestSetExportSpecificationTypeDef",
     "ExportSortByTypeDef",
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
     "GetTestExecutionArtifactsUrlResponseTypeDef",
+    "GrammarSlotTypeSourceOutputTypeDef",
     "GrammarSlotTypeSourceTypeDef",
     "ImportFilterTypeDef",
     "ImportSortByTypeDef",
     "ImportSummaryTypeDef",
     "RuntimeHintsTypeDef",
     "IntentClassificationTestResultItemCountsTypeDef",
     "IntentFilterTypeDef",
     "IntentSortByTypeDef",
+    "InvokedIntentSampleTypeDef",
     "ListBotAliasesRequestRequestTypeDef",
     "ListBotRecommendationsRequestRequestTypeDef",
     "ListCustomVocabularyItemsRequestRequestTypeDef",
     "ListRecommendedIntentsRequestRequestTypeDef",
     "RecommendedIntentSummaryTypeDef",
+    "SessionDataSortByTypeDef",
     "SlotTypeFilterTypeDef",
     "SlotTypeSortByTypeDef",
     "SlotTypeSummaryTypeDef",
     "SlotFilterTypeDef",
     "SlotSortByTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TestExecutionSortByTypeDef",
     "ListTestSetRecordsRequestRequestTypeDef",
     "TestSetSortByTypeDef",
+    "UtteranceDataSortByTypeDef",
+    "PlainTextMessageOutputTypeDef",
+    "SSMLMessageOutputTypeDef",
     "PlainTextMessageTypeDef",
     "SSMLMessageTypeDef",
     "OverallTestResultItemTypeDef",
+    "PathFormatOutputTypeDef",
     "PathFormatTypeDef",
+    "TextInputSpecificationOutputTypeDef",
     "TextInputSpecificationTypeDef",
+    "RelativeAggregationDurationOutputTypeDef",
     "RelativeAggregationDurationTypeDef",
     "ResponseMetadataTypeDef",
     "RuntimeHintValueTypeDef",
+    "SampleValueOutputTypeDef",
     "SampleValueTypeDef",
+    "SlotDefaultValueOutputTypeDef",
     "SlotDefaultValueTypeDef",
+    "SlotPriorityTypeDef",
     "SlotResolutionTestResultItemCountsTypeDef",
+    "SlotValueOutputTypeDef",
     "SlotValueTypeDef",
+    "SlotValueRegexFilterOutputTypeDef",
     "SlotValueRegexFilterTypeDef",
+    "TestSetStorageLocationTypeDef",
     "StopBotRecommendationRequestRequestTypeDef",
     "StopBotRecommendationResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSetIntentDiscrepancyItemTypeDef",
     "TestSetSlotDiscrepancyItemTypeDef",
+    "TestSetDiscrepancyReportBotAliasTargetOutputTypeDef",
     "TestSetDiscrepancyReportBotAliasTargetTypeDef",
+    "TestSetImportInputLocationOutputTypeDef",
     "TestSetImportInputLocationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateExportRequestRequestTypeDef",
     "UpdateResourcePolicyRequestRequestTypeDef",
     "UpdateResourcePolicyResponseTypeDef",
     "UpdateTestSetRequestRequestTypeDef",
     "UserTurnIntentOutputTypeDef",
     "UserTurnSlotOutputTypeDef",
     "UtteranceAudioInputSpecificationTypeDef",
     "AgentTurnResultTypeDef",
+    "AnalyticsIntentResultTypeDef",
+    "ListIntentMetricsRequestRequestTypeDef",
+    "ListIntentPathsResponseTypeDef",
+    "AnalyticsIntentStageResultTypeDef",
+    "ListIntentStageMetricsRequestRequestTypeDef",
+    "ListIntentPathsRequestRequestTypeDef",
+    "AnalyticsSessionResultTypeDef",
+    "ListSessionMetricsRequestRequestTypeDef",
+    "AnalyticsUtteranceResultTypeDef",
+    "ListUtteranceMetricsRequestRequestTypeDef",
     "SearchAssociatedTranscriptsRequestRequestTypeDef",
     "SearchAssociatedTranscriptsResponseTypeDef",
+    "AudioAndDTMFInputSpecificationOutputTypeDef",
     "AudioAndDTMFInputSpecificationTypeDef",
+    "AudioLogDestinationOutputTypeDef",
     "AudioLogDestinationTypeDef",
     "BatchCreateCustomVocabularyItemRequestRequestTypeDef",
-    "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
     "ListCustomVocabularyItemsResponseTypeDef",
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
+    "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
     "ListBotAliasesResponseTypeDef",
+    "TestExecutionTargetOutputTypeDef",
     "TestExecutionTargetTypeDef",
+    "BotImportSpecificationOutputTypeDef",
     "BotImportSpecificationTypeDef",
-    "BotLocaleImportSpecificationTypeDef",
-    "CreateBotLocaleRequestRequestTypeDef",
+    "BotLocaleImportSpecificationOutputTypeDef",
     "CreateBotLocaleResponseTypeDef",
     "DescribeBotLocaleResponseTypeDef",
-    "UpdateBotLocaleRequestRequestTypeDef",
     "UpdateBotLocaleResponseTypeDef",
+    "BotLocaleImportSpecificationTypeDef",
+    "CreateBotLocaleRequestRequestTypeDef",
+    "UpdateBotLocaleRequestRequestTypeDef",
     "ListBotLocalesRequestRequestTypeDef",
     "ListBotLocalesResponseTypeDef",
-    "CreateBotRequestRequestTypeDef",
     "CreateBotResponseTypeDef",
     "DescribeBotResponseTypeDef",
-    "UpdateBotRequestRequestTypeDef",
     "UpdateBotResponseTypeDef",
+    "CreateBotRequestRequestTypeDef",
+    "UpdateBotRequestRequestTypeDef",
     "BotRecommendationResultStatisticsTypeDef",
     "ListBotRecommendationsResponseTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListBotsResponseTypeDef",
-    "CreateBotVersionRequestRequestTypeDef",
     "CreateBotVersionResponseTypeDef",
+    "CreateBotVersionRequestRequestTypeDef",
     "ListBotVersionsRequestRequestTypeDef",
     "ListBotVersionsResponseTypeDef",
     "ListBuiltInIntentsRequestRequestTypeDef",
     "ListBuiltInIntentsResponseTypeDef",
     "ListBuiltInSlotTypesRequestRequestTypeDef",
     "ListBuiltInSlotTypesResponseTypeDef",
+    "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
+    "TextLogDestinationOutputTypeDef",
     "TextLogDestinationTypeDef",
+    "CodeHookSpecificationOutputTypeDef",
     "CodeHookSpecificationTypeDef",
+    "CompositeSlotTypeSettingOutputTypeDef",
     "CompositeSlotTypeSettingTypeDef",
     "ConversationLevelTestResultItemTypeDef",
     "TestExecutionResultFilterByTypeDef",
+    "ConversationLogsDataSourceOutputTypeDef",
     "ConversationLogsDataSourceTypeDef",
     "IntentSummaryTypeDef",
     "CreateResourcePolicyStatementRequestRequestTypeDef",
+    "LexTranscriptFilterOutputTypeDef",
     "LexTranscriptFilterTypeDef",
     "DescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     "DescribeBotRequestBotAvailableWaitTypeDef",
     "DescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     "DescribeExportRequestBotExportCompletedWaitTypeDef",
     "DescribeImportRequestBotImportCompletedWaitTypeDef",
     "DescribeBotVersionResponseTypeDef",
-    "UpdateBotRecommendationRequestRequestTypeDef",
     "DescribeTestSetResponseTypeDef",
     "TestSetSummaryTypeDef",
     "UpdateTestSetResponseTypeDef",
+    "DialogStateOutputTypeDef",
     "DialogStateTypeDef",
+    "UpdateBotRecommendationRequestRequestTypeDef",
+    "ExportResourceSpecificationOutputTypeDef",
     "ExportResourceSpecificationTypeDef",
     "ListExportsRequestRequestTypeDef",
+    "GrammarSlotTypeSettingOutputTypeDef",
     "GrammarSlotTypeSettingTypeDef",
     "ListImportsRequestRequestTypeDef",
     "ListImportsResponseTypeDef",
     "InputSessionStateSpecificationTypeDef",
     "IntentClassificationTestResultItemTypeDef",
     "ListIntentsRequestRequestTypeDef",
+    "SessionSpecificationTypeDef",
     "ListRecommendedIntentsResponseTypeDef",
+    "ListSessionAnalyticsDataRequestRequestTypeDef",
     "ListSlotTypesRequestRequestTypeDef",
     "ListSlotTypesResponseTypeDef",
     "ListSlotsRequestRequestTypeDef",
     "ListTestExecutionsRequestRequestTypeDef",
     "ListTestSetsRequestRequestTypeDef",
+    "ListUtteranceAnalyticsDataRequestRequestTypeDef",
     "OverallTestResultsTypeDef",
+    "UtteranceAggregationDurationOutputTypeDef",
     "UtteranceAggregationDurationTypeDef",
     "RuntimeHintDetailsTypeDef",
+    "SlotTypeValueOutputTypeDef",
     "SlotTypeValueTypeDef",
+    "SlotDefaultValueSpecificationOutputTypeDef",
     "SlotDefaultValueSpecificationTypeDef",
     "SlotResolutionTestResultItemTypeDef",
+    "SlotValueOverrideOutputTypeDef",
     "SlotValueOverrideTypeDef",
+    "SlotValueSelectionSettingOutputTypeDef",
     "SlotValueSelectionSettingTypeDef",
     "TestSetDiscrepancyErrorsTypeDef",
+    "TestSetDiscrepancyReportResourceTargetOutputTypeDef",
     "TestSetDiscrepancyReportResourceTargetTypeDef",
+    "TestSetImportResourceSpecificationOutputTypeDef",
     "TestSetImportResourceSpecificationTypeDef",
     "UserTurnOutputSpecificationTypeDef",
     "UtteranceInputSpecificationTypeDef",
+    "ListIntentMetricsResponseTypeDef",
+    "ListIntentStageMetricsResponseTypeDef",
+    "ListSessionMetricsResponseTypeDef",
+    "ListUtteranceMetricsResponseTypeDef",
+    "PromptAttemptSpecificationOutputTypeDef",
     "PromptAttemptSpecificationTypeDef",
+    "AudioLogSettingOutputTypeDef",
     "AudioLogSettingTypeDef",
     "DescribeTestExecutionResponseTypeDef",
-    "StartTestExecutionRequestRequestTypeDef",
     "StartTestExecutionResponseTypeDef",
     "TestExecutionSummaryTypeDef",
+    "StartTestExecutionRequestRequestTypeDef",
     "BotRecommendationResultsTypeDef",
+    "MessageOutputTypeDef",
+    "UtteranceBotResponseTypeDef",
     "MessageTypeDef",
+    "TextLogSettingOutputTypeDef",
     "TextLogSettingTypeDef",
+    "BotAliasLocaleSettingsOutputTypeDef",
     "BotAliasLocaleSettingsTypeDef",
     "ConversationLevelTestResultsTypeDef",
     "ListTestExecutionResultItemsRequestRequestTypeDef",
+    "TestSetGenerationDataSourceOutputTypeDef",
     "TestSetGenerationDataSourceTypeDef",
     "ListIntentsResponseTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListTestSetsResponseTypeDef",
-    "CreateExportRequestRequestTypeDef",
     "CreateExportResponseTypeDef",
     "DescribeExportResponseTypeDef",
     "ExportSummaryTypeDef",
     "UpdateExportResponseTypeDef",
+    "CreateExportRequestRequestTypeDef",
+    "ExternalSourceSettingOutputTypeDef",
     "ExternalSourceSettingTypeDef",
     "IntentClassificationTestResultsTypeDef",
-    "ListAggregatedUtterancesRequestRequestTypeDef",
+    "ListSessionAnalyticsDataResponseTypeDef",
     "ListAggregatedUtterancesResponseTypeDef",
+    "ListAggregatedUtterancesRequestRequestTypeDef",
     "IntentLevelSlotResolutionTestResultItemTypeDef",
-    "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
+    "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
+    "ImportResourceSpecificationOutputTypeDef",
     "ImportResourceSpecificationTypeDef",
     "UserTurnInputSpecificationTypeDef",
     "ListTestExecutionsResponseTypeDef",
+    "MessageGroupOutputTypeDef",
+    "UtteranceSpecificationTypeDef",
     "MessageGroupTypeDef",
+    "ConversationLogSettingsOutputTypeDef",
     "ConversationLogSettingsTypeDef",
     "DescribeTestSetGenerationResponseTypeDef",
-    "StartTestSetGenerationRequestRequestTypeDef",
     "StartTestSetGenerationResponseTypeDef",
+    "StartTestSetGenerationRequestRequestTypeDef",
+    "S3BucketTranscriptSourceOutputTypeDef",
     "S3BucketTranscriptSourceTypeDef",
     "ListExportsResponseTypeDef",
-    "CreateSlotTypeRequestRequestTypeDef",
     "CreateSlotTypeResponseTypeDef",
     "DescribeSlotTypeResponseTypeDef",
-    "UpdateSlotTypeRequestRequestTypeDef",
     "UpdateSlotTypeResponseTypeDef",
+    "CreateSlotTypeRequestRequestTypeDef",
+    "UpdateSlotTypeRequestRequestTypeDef",
     "IntentLevelSlotResolutionTestResultsTypeDef",
     "DescribeImportResponseTypeDef",
-    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
+    "StartImportRequestRequestTypeDef",
     "UserTurnResultTypeDef",
     "UserTurnSpecificationTypeDef",
+    "FulfillmentStartResponseSpecificationOutputTypeDef",
+    "FulfillmentUpdateResponseSpecificationOutputTypeDef",
+    "PromptSpecificationOutputTypeDef",
+    "ResponseSpecificationOutputTypeDef",
+    "StillWaitingResponseSpecificationOutputTypeDef",
+    "ListUtteranceAnalyticsDataResponseTypeDef",
     "FulfillmentStartResponseSpecificationTypeDef",
     "FulfillmentUpdateResponseSpecificationTypeDef",
     "PromptSpecificationTypeDef",
     "ResponseSpecificationTypeDef",
     "StillWaitingResponseSpecificationTypeDef",
-    "CreateBotAliasRequestRequestTypeDef",
     "CreateBotAliasResponseTypeDef",
     "DescribeBotAliasResponseTypeDef",
-    "UpdateBotAliasRequestRequestTypeDef",
     "UpdateBotAliasResponseTypeDef",
+    "CreateBotAliasRequestRequestTypeDef",
+    "UpdateBotAliasRequestRequestTypeDef",
+    "TranscriptSourceSettingOutputTypeDef",
     "TranscriptSourceSettingTypeDef",
     "TestSetTurnResultTypeDef",
     "TurnSpecificationTypeDef",
-    "FulfillmentUpdatesSpecificationTypeDef",
+    "FulfillmentUpdatesSpecificationOutputTypeDef",
     "SlotSummaryTypeDef",
+    "ConditionalBranchOutputTypeDef",
+    "DefaultConditionalBranchOutputTypeDef",
+    "WaitAndContinueSpecificationOutputTypeDef",
+    "FulfillmentUpdatesSpecificationTypeDef",
     "ConditionalBranchTypeDef",
     "DefaultConditionalBranchTypeDef",
     "WaitAndContinueSpecificationTypeDef",
     "DescribeBotRecommendationResponseTypeDef",
-    "StartBotRecommendationRequestRequestTypeDef",
     "StartBotRecommendationResponseTypeDef",
     "UpdateBotRecommendationResponseTypeDef",
+    "StartBotRecommendationRequestRequestTypeDef",
     "UtteranceLevelTestResultItemTypeDef",
     "TestSetTurnRecordTypeDef",
     "ListSlotsResponseTypeDef",
+    "ConditionalSpecificationOutputTypeDef",
+    "SubSlotValueElicitationSettingOutputTypeDef",
     "ConditionalSpecificationTypeDef",
     "SubSlotValueElicitationSettingTypeDef",
     "UtteranceLevelTestResultsTypeDef",
     "ListTestSetRecordsResponseTypeDef",
+    "IntentClosingSettingOutputTypeDef",
+    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
+    "PostFulfillmentStatusSpecificationOutputTypeDef",
+    "SpecificationsOutputTypeDef",
     "IntentClosingSettingTypeDef",
     "PostDialogCodeHookInvocationSpecificationTypeDef",
     "PostFulfillmentStatusSpecificationTypeDef",
     "SpecificationsTypeDef",
     "TestExecutionResultItemsTypeDef",
+    "DialogCodeHookInvocationSettingOutputTypeDef",
+    "FulfillmentCodeHookSettingsOutputTypeDef",
+    "SubSlotSettingOutputTypeDef",
     "DialogCodeHookInvocationSettingTypeDef",
     "FulfillmentCodeHookSettingsTypeDef",
     "SubSlotSettingTypeDef",
     "ListTestExecutionResultItemsResponseTypeDef",
+    "InitialResponseSettingOutputTypeDef",
+    "IntentConfirmationSettingOutputTypeDef",
+    "SlotCaptureSettingOutputTypeDef",
     "InitialResponseSettingTypeDef",
     "IntentConfirmationSettingTypeDef",
     "SlotCaptureSettingTypeDef",
-    "CreateIntentRequestRequestTypeDef",
     "CreateIntentResponseTypeDef",
     "DescribeIntentResponseTypeDef",
-    "UpdateIntentRequestRequestTypeDef",
     "UpdateIntentResponseTypeDef",
+    "SlotValueElicitationSettingOutputTypeDef",
+    "CreateIntentRequestRequestTypeDef",
+    "UpdateIntentRequestRequestTypeDef",
     "SlotValueElicitationSettingTypeDef",
-    "CreateSlotRequestRequestTypeDef",
     "CreateSlotResponseTypeDef",
     "DescribeSlotResponseTypeDef",
-    "UpdateSlotRequestRequestTypeDef",
     "UpdateSlotResponseTypeDef",
+    "CreateSlotRequestRequestTypeDef",
+    "UpdateSlotRequestRequestTypeDef",
 )
 
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
     },
 )
 
+AdvancedRecognitionSettingOutputTypeDef = TypedDict(
+    "AdvancedRecognitionSettingOutputTypeDef",
+    {
+        "audioRecognitionStrategy": Literal["UseSlotValuesAsCustomVocabulary"],
+    },
+)
+
 AdvancedRecognitionSettingTypeDef = TypedDict(
     "AdvancedRecognitionSettingTypeDef",
     {
         "audioRecognitionStrategy": Literal["UseSlotValuesAsCustomVocabulary"],
     },
     total=False,
 )
@@ -506,39 +694,347 @@
         "utterance": str,
         "hitCount": int,
         "missedCount": int,
         "utteranceFirstRecordedInAggregationDuration": datetime,
         "utteranceLastRecordedInAggregationDuration": datetime,
         "containsDataFromDeletedResources": bool,
     },
-    total=False,
+)
+
+AllowedInputTypesOutputTypeDef = TypedDict(
+    "AllowedInputTypesOutputTypeDef",
+    {
+        "allowAudioInput": bool,
+        "allowDTMFInput": bool,
+    },
 )
 
 AllowedInputTypesTypeDef = TypedDict(
     "AllowedInputTypesTypeDef",
     {
         "allowAudioInput": bool,
         "allowDTMFInput": bool,
     },
 )
 
+_RequiredAnalyticsBinBySpecificationTypeDef = TypedDict(
+    "_RequiredAnalyticsBinBySpecificationTypeDef",
+    {
+        "name": AnalyticsBinByNameType,
+        "interval": AnalyticsIntervalType,
+    },
+)
+_OptionalAnalyticsBinBySpecificationTypeDef = TypedDict(
+    "_OptionalAnalyticsBinBySpecificationTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+
+class AnalyticsBinBySpecificationTypeDef(
+    _RequiredAnalyticsBinBySpecificationTypeDef, _OptionalAnalyticsBinBySpecificationTypeDef
+):
+    pass
+
+
+AnalyticsBinKeyTypeDef = TypedDict(
+    "AnalyticsBinKeyTypeDef",
+    {
+        "name": AnalyticsBinByNameType,
+        "value": int,
+    },
+)
+
+AnalyticsIntentFilterTypeDef = TypedDict(
+    "AnalyticsIntentFilterTypeDef",
+    {
+        "name": AnalyticsIntentFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsIntentGroupByKeyTypeDef = TypedDict(
+    "AnalyticsIntentGroupByKeyTypeDef",
+    {
+        "name": AnalyticsIntentFieldType,
+        "value": str,
+    },
+)
+
+AnalyticsIntentGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsIntentGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsIntentFieldType,
+    },
+)
+
+AnalyticsIntentMetricResultTypeDef = TypedDict(
+    "AnalyticsIntentMetricResultTypeDef",
+    {
+        "name": AnalyticsIntentMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+)
+
+_RequiredAnalyticsIntentMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsIntentMetricTypeDef",
+    {
+        "name": AnalyticsIntentMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsIntentMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsIntentMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+
+class AnalyticsIntentMetricTypeDef(
+    _RequiredAnalyticsIntentMetricTypeDef, _OptionalAnalyticsIntentMetricTypeDef
+):
+    pass
+
+
+AnalyticsIntentNodeSummaryTypeDef = TypedDict(
+    "AnalyticsIntentNodeSummaryTypeDef",
+    {
+        "intentName": str,
+        "intentPath": str,
+        "intentCount": int,
+        "intentLevel": int,
+        "nodeType": AnalyticsNodeTypeType,
+    },
+)
+
+AnalyticsIntentStageFilterTypeDef = TypedDict(
+    "AnalyticsIntentStageFilterTypeDef",
+    {
+        "name": AnalyticsIntentStageFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsIntentStageGroupByKeyTypeDef = TypedDict(
+    "AnalyticsIntentStageGroupByKeyTypeDef",
+    {
+        "name": AnalyticsIntentStageFieldType,
+        "value": str,
+    },
+)
+
+AnalyticsIntentStageGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsIntentStageGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsIntentStageFieldType,
+    },
+)
+
+AnalyticsIntentStageMetricResultTypeDef = TypedDict(
+    "AnalyticsIntentStageMetricResultTypeDef",
+    {
+        "name": AnalyticsIntentStageMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+)
+
+_RequiredAnalyticsIntentStageMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsIntentStageMetricTypeDef",
+    {
+        "name": AnalyticsIntentStageMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsIntentStageMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsIntentStageMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+
+class AnalyticsIntentStageMetricTypeDef(
+    _RequiredAnalyticsIntentStageMetricTypeDef, _OptionalAnalyticsIntentStageMetricTypeDef
+):
+    pass
+
+
+AnalyticsPathFilterTypeDef = TypedDict(
+    "AnalyticsPathFilterTypeDef",
+    {
+        "name": AnalyticsCommonFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsSessionFilterTypeDef = TypedDict(
+    "AnalyticsSessionFilterTypeDef",
+    {
+        "name": AnalyticsSessionFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsSessionGroupByKeyTypeDef = TypedDict(
+    "AnalyticsSessionGroupByKeyTypeDef",
+    {
+        "name": AnalyticsSessionFieldType,
+        "value": str,
+    },
+)
+
+AnalyticsSessionGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsSessionGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsSessionFieldType,
+    },
+)
+
+AnalyticsSessionMetricResultTypeDef = TypedDict(
+    "AnalyticsSessionMetricResultTypeDef",
+    {
+        "name": AnalyticsSessionMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+)
+
+_RequiredAnalyticsSessionMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsSessionMetricTypeDef",
+    {
+        "name": AnalyticsSessionMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsSessionMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsSessionMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+
+class AnalyticsSessionMetricTypeDef(
+    _RequiredAnalyticsSessionMetricTypeDef, _OptionalAnalyticsSessionMetricTypeDef
+):
+    pass
+
+
+AnalyticsUtteranceAttributeResultTypeDef = TypedDict(
+    "AnalyticsUtteranceAttributeResultTypeDef",
+    {
+        "lastUsedIntent": str,
+    },
+)
+
+AnalyticsUtteranceAttributeTypeDef = TypedDict(
+    "AnalyticsUtteranceAttributeTypeDef",
+    {
+        "name": Literal["LastUsedIntent"],
+    },
+)
+
+AnalyticsUtteranceFilterTypeDef = TypedDict(
+    "AnalyticsUtteranceFilterTypeDef",
+    {
+        "name": AnalyticsUtteranceFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsUtteranceGroupByKeyTypeDef = TypedDict(
+    "AnalyticsUtteranceGroupByKeyTypeDef",
+    {
+        "name": AnalyticsUtteranceFieldType,
+        "value": str,
+    },
+)
+
+AnalyticsUtteranceGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsUtteranceGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsUtteranceFieldType,
+    },
+)
+
+AnalyticsUtteranceMetricResultTypeDef = TypedDict(
+    "AnalyticsUtteranceMetricResultTypeDef",
+    {
+        "name": AnalyticsUtteranceMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+)
+
+_RequiredAnalyticsUtteranceMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsUtteranceMetricTypeDef",
+    {
+        "name": AnalyticsUtteranceMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsUtteranceMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsUtteranceMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+
+class AnalyticsUtteranceMetricTypeDef(
+    _RequiredAnalyticsUtteranceMetricTypeDef, _OptionalAnalyticsUtteranceMetricTypeDef
+):
+    pass
+
+
 AssociatedTranscriptFilterTypeDef = TypedDict(
     "AssociatedTranscriptFilterTypeDef",
     {
         "name": AssociatedTranscriptFilterNameType,
         "values": Sequence[str],
     },
 )
 
 AssociatedTranscriptTypeDef = TypedDict(
     "AssociatedTranscriptTypeDef",
     {
         "transcript": str,
     },
-    total=False,
+)
+
+AudioSpecificationOutputTypeDef = TypedDict(
+    "AudioSpecificationOutputTypeDef",
+    {
+        "maxLengthMs": int,
+        "endTimeoutMs": int,
+    },
+)
+
+DTMFSpecificationOutputTypeDef = TypedDict(
+    "DTMFSpecificationOutputTypeDef",
+    {
+        "maxLength": int,
+        "endTimeoutMs": int,
+        "deletionCharacter": str,
+        "endCharacter": str,
+    },
 )
 
 AudioSpecificationTypeDef = TypedDict(
     "AudioSpecificationTypeDef",
     {
         "maxLengthMs": int,
         "endTimeoutMs": int,
@@ -551,14 +1047,23 @@
         "maxLength": int,
         "endTimeoutMs": int,
         "deletionCharacter": str,
         "endCharacter": str,
     },
 )
 
+S3BucketLogDestinationOutputTypeDef = TypedDict(
+    "S3BucketLogDestinationOutputTypeDef",
+    {
+        "kmsKeyArn": str,
+        "s3BucketArn": str,
+        "logPrefix": str,
+    },
+)
+
 _RequiredS3BucketLogDestinationTypeDef = TypedDict(
     "_RequiredS3BucketLogDestinationTypeDef",
     {
         "s3BucketArn": str,
         "logPrefix": str,
     },
 )
@@ -595,87 +1100,111 @@
 
 class NewCustomVocabularyItemTypeDef(
     _RequiredNewCustomVocabularyItemTypeDef, _OptionalNewCustomVocabularyItemTypeDef
 ):
     pass
 
 
-_RequiredCustomVocabularyItemTypeDef = TypedDict(
-    "_RequiredCustomVocabularyItemTypeDef",
+CustomVocabularyItemOutputTypeDef = TypedDict(
+    "CustomVocabularyItemOutputTypeDef",
     {
         "itemId": str,
         "phrase": str,
-    },
-)
-_OptionalCustomVocabularyItemTypeDef = TypedDict(
-    "_OptionalCustomVocabularyItemTypeDef",
-    {
         "weight": int,
         "displayAs": str,
     },
-    total=False,
 )
 
-
-class CustomVocabularyItemTypeDef(
-    _RequiredCustomVocabularyItemTypeDef, _OptionalCustomVocabularyItemTypeDef
-):
-    pass
-
-
 FailedCustomVocabularyItemTypeDef = TypedDict(
     "FailedCustomVocabularyItemTypeDef",
     {
         "itemId": str,
         "errorMessage": str,
         "errorCode": ErrorCodeType,
     },
-    total=False,
 )
 
 CustomVocabularyEntryIdTypeDef = TypedDict(
     "CustomVocabularyEntryIdTypeDef",
     {
         "itemId": str,
     },
 )
 
+_RequiredCustomVocabularyItemTypeDef = TypedDict(
+    "_RequiredCustomVocabularyItemTypeDef",
+    {
+        "itemId": str,
+        "phrase": str,
+    },
+)
+_OptionalCustomVocabularyItemTypeDef = TypedDict(
+    "_OptionalCustomVocabularyItemTypeDef",
+    {
+        "weight": int,
+        "displayAs": str,
+    },
+    total=False,
+)
+
+
+class CustomVocabularyItemTypeDef(
+    _RequiredCustomVocabularyItemTypeDef, _OptionalCustomVocabularyItemTypeDef
+):
+    pass
+
+
 BotAliasHistoryEventTypeDef = TypedDict(
     "BotAliasHistoryEventTypeDef",
     {
         "botVersion": str,
         "startDate": datetime,
         "endDate": datetime,
     },
-    total=False,
 )
 
 BotAliasSummaryTypeDef = TypedDict(
     "BotAliasSummaryTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
         "botAliasStatus": BotAliasStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
+)
+
+BotAliasTestExecutionTargetOutputTypeDef = TypedDict(
+    "BotAliasTestExecutionTargetOutputTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+    },
 )
 
 BotAliasTestExecutionTargetTypeDef = TypedDict(
     "BotAliasTestExecutionTargetTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
     },
 )
 
+BotExportSpecificationOutputTypeDef = TypedDict(
+    "BotExportSpecificationOutputTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+    },
+)
+
 BotExportSpecificationTypeDef = TypedDict(
     "BotExportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
     },
 )
@@ -685,21 +1214,37 @@
     {
         "name": BotFilterNameType,
         "values": Sequence[str],
         "operator": BotFilterOperatorType,
     },
 )
 
+DataPrivacyOutputTypeDef = TypedDict(
+    "DataPrivacyOutputTypeDef",
+    {
+        "childDirected": bool,
+    },
+)
+
 DataPrivacyTypeDef = TypedDict(
     "DataPrivacyTypeDef",
     {
         "childDirected": bool,
     },
 )
 
+BotLocaleExportSpecificationOutputTypeDef = TypedDict(
+    "BotLocaleExportSpecificationOutputTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+
 BotLocaleExportSpecificationTypeDef = TypedDict(
     "BotLocaleExportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -718,14 +1263,22 @@
     "BotLocaleHistoryEventTypeDef",
     {
         "event": str,
         "eventDate": datetime,
     },
 )
 
+VoiceSettingsOutputTypeDef = TypedDict(
+    "VoiceSettingsOutputTypeDef",
+    {
+        "voiceId": str,
+        "engine": VoiceEngineType,
+    },
+)
+
 _RequiredVoiceSettingsTypeDef = TypedDict(
     "_RequiredVoiceSettingsTypeDef",
     {
         "voiceId": str,
     },
 )
 _OptionalVoiceSettingsTypeDef = TypedDict(
@@ -755,15 +1308,25 @@
         "localeId": str,
         "localeName": str,
         "description": str,
         "botLocaleStatus": BotLocaleStatusType,
         "lastUpdatedDateTime": datetime,
         "lastBuildSubmittedDateTime": datetime,
     },
-    total=False,
+)
+
+BotMemberOutputTypeDef = TypedDict(
+    "BotMemberOutputTypeDef",
+    {
+        "botMemberId": str,
+        "botMemberName": str,
+        "botMemberAliasId": str,
+        "botMemberAliasName": str,
+        "botMemberVersion": str,
+    },
 )
 
 BotMemberTypeDef = TypedDict(
     "BotMemberTypeDef",
     {
         "botMemberId": str,
         "botMemberName": str,
@@ -774,48 +1337,33 @@
 )
 
 IntentStatisticsTypeDef = TypedDict(
     "IntentStatisticsTypeDef",
     {
         "discoveredIntentCount": int,
     },
-    total=False,
 )
 
 SlotTypeStatisticsTypeDef = TypedDict(
     "SlotTypeStatisticsTypeDef",
     {
         "discoveredSlotTypeCount": int,
     },
-    total=False,
 )
 
-_RequiredBotRecommendationSummaryTypeDef = TypedDict(
-    "_RequiredBotRecommendationSummaryTypeDef",
+BotRecommendationSummaryTypeDef = TypedDict(
+    "BotRecommendationSummaryTypeDef",
     {
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
-    },
-)
-_OptionalBotRecommendationSummaryTypeDef = TypedDict(
-    "_OptionalBotRecommendationSummaryTypeDef",
-    {
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
-
-class BotRecommendationSummaryTypeDef(
-    _RequiredBotRecommendationSummaryTypeDef, _OptionalBotRecommendationSummaryTypeDef
-):
-    pass
-
-
 BotSortByTypeDef = TypedDict(
     "BotSortByTypeDef",
     {
         "attribute": Literal["BotName"],
         "order": SortOrderType,
     },
 )
@@ -827,15 +1375,21 @@
         "botName": str,
         "description": str,
         "botStatus": BotStatusType,
         "latestBotVersion": str,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
     },
-    total=False,
+)
+
+BotVersionLocaleDetailsOutputTypeDef = TypedDict(
+    "BotVersionLocaleDetailsOutputTypeDef",
+    {
+        "sourceBotVersion": str,
+    },
 )
 
 BotVersionLocaleDetailsTypeDef = TypedDict(
     "BotVersionLocaleDetailsTypeDef",
     {
         "sourceBotVersion": str,
     },
@@ -854,15 +1408,14 @@
     {
         "botName": str,
         "botVersion": str,
         "description": str,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
     },
-    total=False,
 )
 
 BuildBotLocaleRequestRequestTypeDef = TypedDict(
     "BuildBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
@@ -892,15 +1445,14 @@
 
 BuiltInIntentSummaryTypeDef = TypedDict(
     "BuiltInIntentSummaryTypeDef",
     {
         "intentSignature": str,
         "description": str,
     },
-    total=False,
 )
 
 BuiltInSlotTypeSortByTypeDef = TypedDict(
     "BuiltInSlotTypeSortByTypeDef",
     {
         "attribute": Literal["SlotTypeSignature"],
         "order": SortOrderType,
@@ -909,49 +1461,87 @@
 
 BuiltInSlotTypeSummaryTypeDef = TypedDict(
     "BuiltInSlotTypeSummaryTypeDef",
     {
         "slotTypeSignature": str,
         "description": str,
     },
-    total=False,
+)
+
+ButtonOutputTypeDef = TypedDict(
+    "ButtonOutputTypeDef",
+    {
+        "text": str,
+        "value": str,
+    },
 )
 
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
 
+CloudWatchLogGroupLogDestinationOutputTypeDef = TypedDict(
+    "CloudWatchLogGroupLogDestinationOutputTypeDef",
+    {
+        "cloudWatchLogGroupArn": str,
+        "logPrefix": str,
+    },
+)
+
 CloudWatchLogGroupLogDestinationTypeDef = TypedDict(
     "CloudWatchLogGroupLogDestinationTypeDef",
     {
         "cloudWatchLogGroupArn": str,
         "logPrefix": str,
     },
 )
 
+LambdaCodeHookOutputTypeDef = TypedDict(
+    "LambdaCodeHookOutputTypeDef",
+    {
+        "lambdaARN": str,
+        "codeHookInterfaceVersion": str,
+    },
+)
+
 LambdaCodeHookTypeDef = TypedDict(
     "LambdaCodeHookTypeDef",
     {
         "lambdaARN": str,
         "codeHookInterfaceVersion": str,
     },
 )
 
+SubSlotTypeCompositionOutputTypeDef = TypedDict(
+    "SubSlotTypeCompositionOutputTypeDef",
+    {
+        "name": str,
+        "slotTypeId": str,
+    },
+)
+
 SubSlotTypeCompositionTypeDef = TypedDict(
     "SubSlotTypeCompositionTypeDef",
     {
         "name": str,
         "slotTypeId": str,
     },
 )
 
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "expressionString": str,
+    },
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "expressionString": str,
     },
 )
 
@@ -959,35 +1549,22 @@
     "ConversationLevelIntentClassificationResultItemTypeDef",
     {
         "intentName": str,
         "matchResult": TestResultMatchStatusType,
     },
 )
 
-_RequiredConversationLevelResultDetailTypeDef = TypedDict(
-    "_RequiredConversationLevelResultDetailTypeDef",
+ConversationLevelResultDetailTypeDef = TypedDict(
+    "ConversationLevelResultDetailTypeDef",
     {
         "endToEndResult": TestResultMatchStatusType,
-    },
-)
-_OptionalConversationLevelResultDetailTypeDef = TypedDict(
-    "_OptionalConversationLevelResultDetailTypeDef",
-    {
         "speechTranscriptionResult": TestResultMatchStatusType,
     },
-    total=False,
 )
 
-
-class ConversationLevelResultDetailTypeDef(
-    _RequiredConversationLevelResultDetailTypeDef, _OptionalConversationLevelResultDetailTypeDef
-):
-    pass
-
-
 ConversationLevelSlotResolutionResultItemTypeDef = TypedDict(
     "ConversationLevelSlotResolutionResultItemTypeDef",
     {
         "intentName": str,
         "slotName": str,
         "matchResult": TestResultMatchStatusType,
     },
@@ -997,30 +1574,46 @@
     "ConversationLevelTestResultsFilterByTypeDef",
     {
         "endToEndResult": TestResultMatchStatusType,
     },
     total=False,
 )
 
-ConversationLogsDataSourceFilterByTypeDef = TypedDict(
-    "ConversationLogsDataSourceFilterByTypeDef",
+ConversationLogsDataSourceFilterByOutputTypeDef = TypedDict(
+    "ConversationLogsDataSourceFilterByOutputTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
         "inputMode": ConversationLogsInputModeFilterType,
     },
 )
 
+ConversationLogsDataSourceFilterByTypeDef = TypedDict(
+    "ConversationLogsDataSourceFilterByTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+        "inputMode": ConversationLogsInputModeFilterType,
+    },
+)
+
 SentimentAnalysisSettingsTypeDef = TypedDict(
     "SentimentAnalysisSettingsTypeDef",
     {
         "detectSentiment": bool,
     },
 )
 
+SentimentAnalysisSettingsOutputTypeDef = TypedDict(
+    "SentimentAnalysisSettingsOutputTypeDef",
+    {
+        "detectSentiment": bool,
+    },
+)
+
 DialogCodeHookSettingsTypeDef = TypedDict(
     "DialogCodeHookSettingsTypeDef",
     {
         "enabled": bool,
     },
 )
 
@@ -1065,14 +1658,53 @@
 SampleUtteranceTypeDef = TypedDict(
     "SampleUtteranceTypeDef",
     {
         "utterance": str,
     },
 )
 
+DialogCodeHookSettingsOutputTypeDef = TypedDict(
+    "DialogCodeHookSettingsOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+
+InputContextOutputTypeDef = TypedDict(
+    "InputContextOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
+KendraConfigurationOutputTypeDef = TypedDict(
+    "KendraConfigurationOutputTypeDef",
+    {
+        "kendraIndex": str,
+        "queryFilterStringEnabled": bool,
+        "queryFilterString": str,
+    },
+)
+
+OutputContextOutputTypeDef = TypedDict(
+    "OutputContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLiveInSeconds": int,
+        "turnsToLive": int,
+    },
+)
+
+SampleUtteranceOutputTypeDef = TypedDict(
+    "SampleUtteranceOutputTypeDef",
+    {
+        "utterance": str,
+    },
+)
+
 CreateResourcePolicyRequestRequestTypeDef = TypedDict(
     "CreateResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
         "policy": str,
     },
 )
@@ -1115,56 +1747,103 @@
 ObfuscationSettingTypeDef = TypedDict(
     "ObfuscationSettingTypeDef",
     {
         "obfuscationSettingType": ObfuscationSettingTypeType,
     },
 )
 
+MultipleValuesSettingOutputTypeDef = TypedDict(
+    "MultipleValuesSettingOutputTypeDef",
+    {
+        "allowMultipleValues": bool,
+    },
+)
+
+ObfuscationSettingOutputTypeDef = TypedDict(
+    "ObfuscationSettingOutputTypeDef",
+    {
+        "obfuscationSettingType": ObfuscationSettingTypeType,
+    },
+)
+
 CreateUploadUrlResponseTypeDef = TypedDict(
     "CreateUploadUrlResponseTypeDef",
     {
         "importId": str,
         "uploadUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CustomPayloadOutputTypeDef = TypedDict(
+    "CustomPayloadOutputTypeDef",
+    {
+        "value": str,
+    },
+)
+
 CustomPayloadTypeDef = TypedDict(
     "CustomPayloadTypeDef",
     {
         "value": str,
     },
 )
 
+CustomVocabularyExportSpecificationOutputTypeDef = TypedDict(
+    "CustomVocabularyExportSpecificationOutputTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+
 CustomVocabularyExportSpecificationTypeDef = TypedDict(
     "CustomVocabularyExportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
+CustomVocabularyImportSpecificationOutputTypeDef = TypedDict(
+    "CustomVocabularyImportSpecificationOutputTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+
 CustomVocabularyImportSpecificationTypeDef = TypedDict(
     "CustomVocabularyImportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DateRangeFilterTypeDef = TypedDict(
-    "DateRangeFilterTypeDef",
+DateRangeFilterOutputTypeDef = TypedDict(
+    "DateRangeFilterOutputTypeDef",
     {
         "startDateTime": datetime,
         "endDateTime": datetime,
     },
 )
 
+DateRangeFilterTypeDef = TypedDict(
+    "DateRangeFilterTypeDef",
+    {
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+    },
+)
+
 _RequiredDeleteBotAliasRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBotAliasRequestRequestTypeDef",
     {
         "botAliasId": str,
         "botId": str,
     },
 )
@@ -1504,22 +2183,21 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
     },
 )
 
-EncryptionSettingTypeDef = TypedDict(
-    "EncryptionSettingTypeDef",
+EncryptionSettingOutputTypeDef = TypedDict(
+    "EncryptionSettingOutputTypeDef",
     {
         "kmsKeyArn": str,
         "botLocaleExportPassword": str,
         "associatedTranscriptsPassword": str,
     },
-    total=False,
 )
 
 DescribeBotRequestRequestTypeDef = TypedDict(
     "DescribeBotRequestRequestTypeDef",
     {
         "botId": str,
     },
@@ -1575,16 +2253,16 @@
         "intentId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-SlotPriorityTypeDef = TypedDict(
-    "SlotPriorityTypeDef",
+SlotPriorityOutputTypeDef = TypedDict(
+    "SlotPriorityOutputTypeDef",
     {
         "priority": int,
         "slotId": str,
     },
 )
 
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
@@ -1642,43 +2320,39 @@
 DescribeTestSetGenerationRequestRequestTypeDef = TypedDict(
     "DescribeTestSetGenerationRequestRequestTypeDef",
     {
         "testSetGenerationId": str,
     },
 )
 
-_RequiredTestSetStorageLocationTypeDef = TypedDict(
-    "_RequiredTestSetStorageLocationTypeDef",
+TestSetStorageLocationOutputTypeDef = TypedDict(
+    "TestSetStorageLocationOutputTypeDef",
     {
         "s3BucketName": str,
         "s3Path": str,
-    },
-)
-_OptionalTestSetStorageLocationTypeDef = TypedDict(
-    "_OptionalTestSetStorageLocationTypeDef",
-    {
         "kmsKeyArn": str,
     },
-    total=False,
 )
 
-
-class TestSetStorageLocationTypeDef(
-    _RequiredTestSetStorageLocationTypeDef, _OptionalTestSetStorageLocationTypeDef
-):
-    pass
-
-
 DescribeTestSetRequestRequestTypeDef = TypedDict(
     "DescribeTestSetRequestRequestTypeDef",
     {
         "testSetId": str,
     },
 )
 
+DialogActionOutputTypeDef = TypedDict(
+    "DialogActionOutputTypeDef",
+    {
+        "type": DialogActionTypeType,
+        "slotToElicit": str,
+        "suppressNextMessage": bool,
+    },
+)
+
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
@@ -1691,23 +2365,39 @@
 )
 
 
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
 
+IntentOverrideOutputTypeDef = TypedDict(
+    "IntentOverrideOutputTypeDef",
+    {
+        "name": str,
+        "slots": Dict[str, "SlotValueOverrideOutputTypeDef"],
+    },
+)
+
 IntentOverrideTypeDef = TypedDict(
     "IntentOverrideTypeDef",
     {
         "name": str,
         "slots": Mapping[str, "SlotValueOverrideTypeDef"],
     },
     total=False,
 )
 
+ElicitationCodeHookInvocationSettingOutputTypeDef = TypedDict(
+    "ElicitationCodeHookInvocationSettingOutputTypeDef",
+    {
+        "enableCodeHookInvocation": bool,
+        "invocationLabel": str,
+    },
+)
+
 _RequiredElicitationCodeHookInvocationSettingTypeDef = TypedDict(
     "_RequiredElicitationCodeHookInvocationSettingTypeDef",
     {
         "enableCodeHookInvocation": bool,
     },
 )
 _OptionalElicitationCodeHookInvocationSettingTypeDef = TypedDict(
@@ -1729,23 +2419,40 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionSettingTypeDef = TypedDict(
+    "EncryptionSettingTypeDef",
+    {
+        "kmsKeyArn": str,
+        "botLocaleExportPassword": str,
+        "associatedTranscriptsPassword": str,
+    },
+    total=False,
+)
+
 ExportFilterTypeDef = TypedDict(
     "ExportFilterTypeDef",
     {
         "name": Literal["ExportResourceType"],
         "values": Sequence[str],
         "operator": ExportFilterOperatorType,
     },
 )
 
+TestSetExportSpecificationOutputTypeDef = TypedDict(
+    "TestSetExportSpecificationOutputTypeDef",
+    {
+        "testSetId": str,
+    },
+)
+
 TestSetExportSpecificationTypeDef = TypedDict(
     "TestSetExportSpecificationTypeDef",
     {
         "testSetId": str,
     },
 )
 
@@ -1769,14 +2476,23 @@
     {
         "testExecutionId": str,
         "downloadArtifactsUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GrammarSlotTypeSourceOutputTypeDef = TypedDict(
+    "GrammarSlotTypeSourceOutputTypeDef",
+    {
+        "s3BucketName": str,
+        "s3ObjectKey": str,
+        "kmsKeyArn": str,
+    },
+)
+
 _RequiredGrammarSlotTypeSourceTypeDef = TypedDict(
     "_RequiredGrammarSlotTypeSourceTypeDef",
     {
         "s3BucketName": str,
         "s3ObjectKey": str,
     },
 )
@@ -1820,48 +2536,32 @@
         "importedResourceName": str,
         "importStatus": ImportStatusType,
         "mergeStrategy": MergeStrategyType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "importedResourceType": ImportResourceTypeType,
     },
-    total=False,
 )
 
 RuntimeHintsTypeDef = TypedDict(
     "RuntimeHintsTypeDef",
     {
         "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsTypeDef"]],
     },
-    total=False,
 )
 
-_RequiredIntentClassificationTestResultItemCountsTypeDef = TypedDict(
-    "_RequiredIntentClassificationTestResultItemCountsTypeDef",
+IntentClassificationTestResultItemCountsTypeDef = TypedDict(
+    "IntentClassificationTestResultItemCountsTypeDef",
     {
         "totalResultCount": int,
-        "intentMatchResultCounts": Dict[TestResultMatchStatusType, int],
-    },
-)
-_OptionalIntentClassificationTestResultItemCountsTypeDef = TypedDict(
-    "_OptionalIntentClassificationTestResultItemCountsTypeDef",
-    {
         "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
+        "intentMatchResultCounts": Dict[TestResultMatchStatusType, int],
     },
-    total=False,
 )
 
-
-class IntentClassificationTestResultItemCountsTypeDef(
-    _RequiredIntentClassificationTestResultItemCountsTypeDef,
-    _OptionalIntentClassificationTestResultItemCountsTypeDef,
-):
-    pass
-
-
 IntentFilterTypeDef = TypedDict(
     "IntentFilterTypeDef",
     {
         "name": Literal["IntentName"],
         "values": Sequence[str],
         "operator": IntentFilterOperatorType,
     },
@@ -1871,14 +2571,21 @@
     "IntentSortByTypeDef",
     {
         "attribute": IntentSortAttributeType,
         "order": SortOrderType,
     },
 )
 
+InvokedIntentSampleTypeDef = TypedDict(
+    "InvokedIntentSampleTypeDef",
+    {
+        "intentName": str,
+    },
+)
+
 _RequiredListBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListBotAliasesRequestRequestTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalListBotAliasesRequestRequestTypeDef = TypedDict(
@@ -1976,15 +2683,22 @@
 RecommendedIntentSummaryTypeDef = TypedDict(
     "RecommendedIntentSummaryTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "sampleUtterancesCount": int,
     },
-    total=False,
+)
+
+SessionDataSortByTypeDef = TypedDict(
+    "SessionDataSortByTypeDef",
+    {
+        "name": AnalyticsSessionSortByNameType,
+        "order": AnalyticsSortOrderType,
+    },
 )
 
 SlotTypeFilterTypeDef = TypedDict(
     "SlotTypeFilterTypeDef",
     {
         "name": SlotTypeFilterNameType,
         "values": Sequence[str],
@@ -2006,15 +2720,14 @@
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
         "parentSlotTypeSignature": str,
         "lastUpdatedDateTime": datetime,
         "slotTypeCategory": SlotTypeCategoryType,
     },
-    total=False,
 )
 
 SlotFilterTypeDef = TypedDict(
     "SlotFilterTypeDef",
     {
         "name": Literal["SlotName"],
         "values": Sequence[str],
@@ -2080,66 +2793,97 @@
     "TestSetSortByTypeDef",
     {
         "attribute": TestSetSortAttributeType,
         "order": SortOrderType,
     },
 )
 
+UtteranceDataSortByTypeDef = TypedDict(
+    "UtteranceDataSortByTypeDef",
+    {
+        "name": Literal["UtteranceTimestamp"],
+        "order": AnalyticsSortOrderType,
+    },
+)
+
+PlainTextMessageOutputTypeDef = TypedDict(
+    "PlainTextMessageOutputTypeDef",
+    {
+        "value": str,
+    },
+)
+
+SSMLMessageOutputTypeDef = TypedDict(
+    "SSMLMessageOutputTypeDef",
+    {
+        "value": str,
+    },
+)
+
 PlainTextMessageTypeDef = TypedDict(
     "PlainTextMessageTypeDef",
     {
         "value": str,
     },
 )
 
 SSMLMessageTypeDef = TypedDict(
     "SSMLMessageTypeDef",
     {
         "value": str,
     },
 )
 
-_RequiredOverallTestResultItemTypeDef = TypedDict(
-    "_RequiredOverallTestResultItemTypeDef",
+OverallTestResultItemTypeDef = TypedDict(
+    "OverallTestResultItemTypeDef",
     {
         "multiTurnConversation": bool,
         "totalResultCount": int,
+        "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
         "endToEndResultCounts": Dict[TestResultMatchStatusType, int],
     },
 )
-_OptionalOverallTestResultItemTypeDef = TypedDict(
-    "_OptionalOverallTestResultItemTypeDef",
+
+PathFormatOutputTypeDef = TypedDict(
+    "PathFormatOutputTypeDef",
     {
-        "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
+        "objectPrefixes": List[str],
     },
-    total=False,
 )
 
-
-class OverallTestResultItemTypeDef(
-    _RequiredOverallTestResultItemTypeDef, _OptionalOverallTestResultItemTypeDef
-):
-    pass
-
-
 PathFormatTypeDef = TypedDict(
     "PathFormatTypeDef",
     {
-        "objectPrefixes": List[str],
+        "objectPrefixes": Sequence[str],
     },
     total=False,
 )
 
+TextInputSpecificationOutputTypeDef = TypedDict(
+    "TextInputSpecificationOutputTypeDef",
+    {
+        "startTimeoutMs": int,
+    },
+)
+
 TextInputSpecificationTypeDef = TypedDict(
     "TextInputSpecificationTypeDef",
     {
         "startTimeoutMs": int,
     },
 )
 
+RelativeAggregationDurationOutputTypeDef = TypedDict(
+    "RelativeAggregationDurationOutputTypeDef",
+    {
+        "timeDimension": TimeDimensionType,
+        "timeValue": int,
+    },
+)
+
 RelativeAggregationDurationTypeDef = TypedDict(
     "RelativeAggregationDurationTypeDef",
     {
         "timeDimension": TimeDimensionType,
         "timeValue": int,
     },
 )
@@ -2158,66 +2902,110 @@
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
+SampleValueOutputTypeDef = TypedDict(
+    "SampleValueOutputTypeDef",
+    {
+        "value": str,
+    },
+)
+
 SampleValueTypeDef = TypedDict(
     "SampleValueTypeDef",
     {
         "value": str,
     },
 )
 
+SlotDefaultValueOutputTypeDef = TypedDict(
+    "SlotDefaultValueOutputTypeDef",
+    {
+        "defaultValue": str,
+    },
+)
+
 SlotDefaultValueTypeDef = TypedDict(
     "SlotDefaultValueTypeDef",
     {
         "defaultValue": str,
     },
 )
 
-_RequiredSlotResolutionTestResultItemCountsTypeDef = TypedDict(
-    "_RequiredSlotResolutionTestResultItemCountsTypeDef",
+SlotPriorityTypeDef = TypedDict(
+    "SlotPriorityTypeDef",
     {
-        "totalResultCount": int,
-        "slotMatchResultCounts": Dict[TestResultMatchStatusType, int],
+        "priority": int,
+        "slotId": str,
     },
 )
-_OptionalSlotResolutionTestResultItemCountsTypeDef = TypedDict(
-    "_OptionalSlotResolutionTestResultItemCountsTypeDef",
+
+SlotResolutionTestResultItemCountsTypeDef = TypedDict(
+    "SlotResolutionTestResultItemCountsTypeDef",
     {
+        "totalResultCount": int,
         "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
+        "slotMatchResultCounts": Dict[TestResultMatchStatusType, int],
     },
-    total=False,
 )
 
-
-class SlotResolutionTestResultItemCountsTypeDef(
-    _RequiredSlotResolutionTestResultItemCountsTypeDef,
-    _OptionalSlotResolutionTestResultItemCountsTypeDef,
-):
-    pass
-
+SlotValueOutputTypeDef = TypedDict(
+    "SlotValueOutputTypeDef",
+    {
+        "interpretedValue": str,
+    },
+)
 
 SlotValueTypeDef = TypedDict(
     "SlotValueTypeDef",
     {
         "interpretedValue": str,
     },
     total=False,
 )
 
+SlotValueRegexFilterOutputTypeDef = TypedDict(
+    "SlotValueRegexFilterOutputTypeDef",
+    {
+        "pattern": str,
+    },
+)
+
 SlotValueRegexFilterTypeDef = TypedDict(
     "SlotValueRegexFilterTypeDef",
     {
         "pattern": str,
     },
 )
 
+_RequiredTestSetStorageLocationTypeDef = TypedDict(
+    "_RequiredTestSetStorageLocationTypeDef",
+    {
+        "s3BucketName": str,
+        "s3Path": str,
+    },
+)
+_OptionalTestSetStorageLocationTypeDef = TypedDict(
+    "_OptionalTestSetStorageLocationTypeDef",
+    {
+        "kmsKeyArn": str,
+    },
+    total=False,
+)
+
+
+class TestSetStorageLocationTypeDef(
+    _RequiredTestSetStorageLocationTypeDef, _OptionalTestSetStorageLocationTypeDef
+):
+    pass
+
+
 StopBotRecommendationRequestRequestTypeDef = TypedDict(
     "StopBotRecommendationRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -2257,23 +3045,40 @@
     {
         "intentName": str,
         "slotName": str,
         "errorMessage": str,
     },
 )
 
+TestSetDiscrepancyReportBotAliasTargetOutputTypeDef = TypedDict(
+    "TestSetDiscrepancyReportBotAliasTargetOutputTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+    },
+)
+
 TestSetDiscrepancyReportBotAliasTargetTypeDef = TypedDict(
     "TestSetDiscrepancyReportBotAliasTargetTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
     },
 )
 
+TestSetImportInputLocationOutputTypeDef = TypedDict(
+    "TestSetImportInputLocationOutputTypeDef",
+    {
+        "s3BucketName": str,
+        "s3Path": str,
+    },
+)
+
 TestSetImportInputLocationTypeDef = TypedDict(
     "TestSetImportInputLocationTypeDef",
     {
         "s3BucketName": str,
         "s3Path": str,
     },
 )
@@ -2357,71 +3162,231 @@
 
 class UpdateTestSetRequestRequestTypeDef(
     _RequiredUpdateTestSetRequestRequestTypeDef, _OptionalUpdateTestSetRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUserTurnIntentOutputTypeDef = TypedDict(
-    "_RequiredUserTurnIntentOutputTypeDef",
+UserTurnIntentOutputTypeDef = TypedDict(
+    "UserTurnIntentOutputTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalUserTurnIntentOutputTypeDef = TypedDict(
-    "_OptionalUserTurnIntentOutputTypeDef",
-    {
         "slots": Dict[str, "UserTurnSlotOutputTypeDef"],
     },
-    total=False,
 )
 
-
-class UserTurnIntentOutputTypeDef(
-    _RequiredUserTurnIntentOutputTypeDef, _OptionalUserTurnIntentOutputTypeDef
-):
-    pass
-
-
 UserTurnSlotOutputTypeDef = TypedDict(
     "UserTurnSlotOutputTypeDef",
     {
         "value": str,
         "values": List[Dict[str, Any]],
         "subSlots": Dict[str, Dict[str, Any]],
     },
-    total=False,
 )
 
 UtteranceAudioInputSpecificationTypeDef = TypedDict(
     "UtteranceAudioInputSpecificationTypeDef",
     {
         "audioFileS3Location": str,
     },
 )
 
-_RequiredAgentTurnResultTypeDef = TypedDict(
-    "_RequiredAgentTurnResultTypeDef",
+AgentTurnResultTypeDef = TypedDict(
+    "AgentTurnResultTypeDef",
     {
         "expectedAgentPrompt": str,
-    },
-)
-_OptionalAgentTurnResultTypeDef = TypedDict(
-    "_OptionalAgentTurnResultTypeDef",
-    {
         "actualAgentPrompt": str,
         "errorDetails": ExecutionErrorDetailsTypeDef,
         "actualElicitedSlot": str,
         "actualIntent": str,
     },
+)
+
+AnalyticsIntentResultTypeDef = TypedDict(
+    "AnalyticsIntentResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsIntentGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsIntentMetricResultTypeDef],
+    },
+)
+
+_RequiredListIntentMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+        "metrics": Sequence[AnalyticsIntentMetricTypeDef],
+    },
+)
+_OptionalListIntentMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsIntentGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsIntentFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
     total=False,
 )
 
 
-class AgentTurnResultTypeDef(_RequiredAgentTurnResultTypeDef, _OptionalAgentTurnResultTypeDef):
+class ListIntentMetricsRequestRequestTypeDef(
+    _RequiredListIntentMetricsRequestRequestTypeDef, _OptionalListIntentMetricsRequestRequestTypeDef
+):
+    pass
+
+
+ListIntentPathsResponseTypeDef = TypedDict(
+    "ListIntentPathsResponseTypeDef",
+    {
+        "nodeSummaries": List[AnalyticsIntentNodeSummaryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AnalyticsIntentStageResultTypeDef = TypedDict(
+    "AnalyticsIntentStageResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsIntentStageGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsIntentStageMetricResultTypeDef],
+    },
+)
+
+_RequiredListIntentStageMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentStageMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+        "metrics": Sequence[AnalyticsIntentStageMetricTypeDef],
+    },
+)
+_OptionalListIntentStageMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentStageMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsIntentStageFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListIntentStageMetricsRequestRequestTypeDef(
+    _RequiredListIntentStageMetricsRequestRequestTypeDef,
+    _OptionalListIntentStageMetricsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListIntentPathsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentPathsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+        "intentPath": str,
+    },
+)
+_OptionalListIntentPathsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentPathsRequestRequestTypeDef",
+    {
+        "filters": Sequence[AnalyticsPathFilterTypeDef],
+    },
+    total=False,
+)
+
+
+class ListIntentPathsRequestRequestTypeDef(
+    _RequiredListIntentPathsRequestRequestTypeDef, _OptionalListIntentPathsRequestRequestTypeDef
+):
+    pass
+
+
+AnalyticsSessionResultTypeDef = TypedDict(
+    "AnalyticsSessionResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsSessionGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsSessionMetricResultTypeDef],
+    },
+)
+
+_RequiredListSessionMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListSessionMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+        "metrics": Sequence[AnalyticsSessionMetricTypeDef],
+    },
+)
+_OptionalListSessionMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListSessionMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsSessionGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsSessionFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListSessionMetricsRequestRequestTypeDef(
+    _RequiredListSessionMetricsRequestRequestTypeDef,
+    _OptionalListSessionMetricsRequestRequestTypeDef,
+):
+    pass
+
+
+AnalyticsUtteranceResultTypeDef = TypedDict(
+    "AnalyticsUtteranceResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsUtteranceGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsUtteranceMetricResultTypeDef],
+        "attributeResults": List[AnalyticsUtteranceAttributeResultTypeDef],
+    },
+)
+
+_RequiredListUtteranceMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListUtteranceMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+        "metrics": Sequence[AnalyticsUtteranceMetricTypeDef],
+    },
+)
+_OptionalListUtteranceMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListUtteranceMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef],
+        "attributes": Sequence[AnalyticsUtteranceAttributeTypeDef],
+        "filters": Sequence[AnalyticsUtteranceFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListUtteranceMetricsRequestRequestTypeDef(
+    _RequiredListUtteranceMetricsRequestRequestTypeDef,
+    _OptionalListUtteranceMetricsRequestRequestTypeDef,
+):
     pass
 
 
 _RequiredSearchAssociatedTranscriptsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchAssociatedTranscriptsRequestRequestTypeDef",
     {
         "botId": str,
@@ -2459,14 +3424,23 @@
         "nextIndex": int,
         "associatedTranscripts": List[AssociatedTranscriptTypeDef],
         "totalResults": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AudioAndDTMFInputSpecificationOutputTypeDef = TypedDict(
+    "AudioAndDTMFInputSpecificationOutputTypeDef",
+    {
+        "startTimeoutMs": int,
+        "audioSpecification": AudioSpecificationOutputTypeDef,
+        "dtmfSpecification": DTMFSpecificationOutputTypeDef,
+    },
+)
+
 _RequiredAudioAndDTMFInputSpecificationTypeDef = TypedDict(
     "_RequiredAudioAndDTMFInputSpecificationTypeDef",
     {
         "startTimeoutMs": int,
     },
 )
 _OptionalAudioAndDTMFInputSpecificationTypeDef = TypedDict(
@@ -2481,14 +3455,21 @@
 
 class AudioAndDTMFInputSpecificationTypeDef(
     _RequiredAudioAndDTMFInputSpecificationTypeDef, _OptionalAudioAndDTMFInputSpecificationTypeDef
 ):
     pass
 
 
+AudioLogDestinationOutputTypeDef = TypedDict(
+    "AudioLogDestinationOutputTypeDef",
+    {
+        "s3Bucket": S3BucketLogDestinationOutputTypeDef,
+    },
+)
+
 AudioLogDestinationTypeDef = TypedDict(
     "AudioLogDestinationTypeDef",
     {
         "s3Bucket": S3BucketLogDestinationTypeDef,
     },
 )
 
@@ -2498,125 +3479,213 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "customVocabularyItemList": Sequence[NewCustomVocabularyItemTypeDef],
     },
 )
 
-BatchUpdateCustomVocabularyItemRequestRequestTypeDef = TypedDict(
-    "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyItemList": Sequence[CustomVocabularyItemTypeDef],
-    },
-)
-
 ListCustomVocabularyItemsResponseTypeDef = TypedDict(
     "ListCustomVocabularyItemsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
-        "customVocabularyItems": List[CustomVocabularyItemTypeDef],
+        "customVocabularyItems": List[CustomVocabularyItemOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
-        "resources": List[CustomVocabularyItemTypeDef],
+        "resources": List[CustomVocabularyItemOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
-        "resources": List[CustomVocabularyItemTypeDef],
+        "resources": List[CustomVocabularyItemOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
-        "resources": List[CustomVocabularyItemTypeDef],
+        "resources": List[CustomVocabularyItemOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteCustomVocabularyItemRequestRequestTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "customVocabularyItemList": Sequence[CustomVocabularyEntryIdTypeDef],
     },
 )
 
+BatchUpdateCustomVocabularyItemRequestRequestTypeDef = TypedDict(
+    "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyItemList": Sequence[CustomVocabularyItemTypeDef],
+    },
+)
+
 ListBotAliasesResponseTypeDef = TypedDict(
     "ListBotAliasesResponseTypeDef",
     {
         "botAliasSummaries": List[BotAliasSummaryTypeDef],
         "nextToken": str,
         "botId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TestExecutionTargetOutputTypeDef = TypedDict(
+    "TestExecutionTargetOutputTypeDef",
+    {
+        "botAliasTarget": BotAliasTestExecutionTargetOutputTypeDef,
+    },
+)
+
 TestExecutionTargetTypeDef = TypedDict(
     "TestExecutionTargetTypeDef",
     {
         "botAliasTarget": BotAliasTestExecutionTargetTypeDef,
     },
     total=False,
 )
 
+BotImportSpecificationOutputTypeDef = TypedDict(
+    "BotImportSpecificationOutputTypeDef",
+    {
+        "botName": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyOutputTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botTags": Dict[str, str],
+        "testBotAliasTags": Dict[str, str],
+    },
+)
+
 _RequiredBotImportSpecificationTypeDef = TypedDict(
     "_RequiredBotImportSpecificationTypeDef",
     {
         "botName": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
     },
 )
 _OptionalBotImportSpecificationTypeDef = TypedDict(
     "_OptionalBotImportSpecificationTypeDef",
     {
         "idleSessionTTLInSeconds": int,
-        "botTags": Dict[str, str],
-        "testBotAliasTags": Dict[str, str],
+        "botTags": Mapping[str, str],
+        "testBotAliasTags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class BotImportSpecificationTypeDef(
     _RequiredBotImportSpecificationTypeDef, _OptionalBotImportSpecificationTypeDef
 ):
     pass
 
 
+BotLocaleImportSpecificationOutputTypeDef = TypedDict(
+    "BotLocaleImportSpecificationOutputTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "nluIntentConfidenceThreshold": float,
+        "voiceSettings": VoiceSettingsOutputTypeDef,
+    },
+)
+
+CreateBotLocaleResponseTypeDef = TypedDict(
+    "CreateBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeName": str,
+        "localeId": str,
+        "description": str,
+        "nluIntentConfidenceThreshold": float,
+        "voiceSettings": VoiceSettingsOutputTypeDef,
+        "botLocaleStatus": BotLocaleStatusType,
+        "creationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeBotLocaleResponseTypeDef = TypedDict(
+    "DescribeBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "localeName": str,
+        "description": str,
+        "nluIntentConfidenceThreshold": float,
+        "voiceSettings": VoiceSettingsOutputTypeDef,
+        "intentsCount": int,
+        "slotTypesCount": int,
+        "botLocaleStatus": BotLocaleStatusType,
+        "failureReasons": List[str],
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "lastBuildSubmittedDateTime": datetime,
+        "botLocaleHistoryEvents": List[BotLocaleHistoryEventTypeDef],
+        "recommendedActions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateBotLocaleResponseTypeDef = TypedDict(
+    "UpdateBotLocaleResponseTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "localeName": str,
+        "description": str,
+        "nluIntentConfidenceThreshold": float,
+        "voiceSettings": VoiceSettingsOutputTypeDef,
+        "botLocaleStatus": BotLocaleStatusType,
+        "failureReasons": List[str],
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "recommendedActions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredBotLocaleImportSpecificationTypeDef = TypedDict(
     "_RequiredBotLocaleImportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -2658,53 +3727,14 @@
 
 class CreateBotLocaleRequestRequestTypeDef(
     _RequiredCreateBotLocaleRequestRequestTypeDef, _OptionalCreateBotLocaleRequestRequestTypeDef
 ):
     pass
 
 
-CreateBotLocaleResponseTypeDef = TypedDict(
-    "CreateBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeName": str,
-        "localeId": str,
-        "description": str,
-        "nluIntentConfidenceThreshold": float,
-        "voiceSettings": VoiceSettingsTypeDef,
-        "botLocaleStatus": BotLocaleStatusType,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeBotLocaleResponseTypeDef = TypedDict(
-    "DescribeBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "localeName": str,
-        "description": str,
-        "nluIntentConfidenceThreshold": float,
-        "voiceSettings": VoiceSettingsTypeDef,
-        "intentsCount": int,
-        "slotTypesCount": int,
-        "botLocaleStatus": BotLocaleStatusType,
-        "failureReasons": List[str],
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "lastBuildSubmittedDateTime": datetime,
-        "botLocaleHistoryEvents": List[BotLocaleHistoryEventTypeDef],
-        "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBotLocaleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "nluIntentConfidenceThreshold": float,
@@ -2722,33 +3752,14 @@
 
 class UpdateBotLocaleRequestRequestTypeDef(
     _RequiredUpdateBotLocaleRequestRequestTypeDef, _OptionalUpdateBotLocaleRequestRequestTypeDef
 ):
     pass
 
 
-UpdateBotLocaleResponseTypeDef = TypedDict(
-    "UpdateBotLocaleResponseTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "localeName": str,
-        "description": str,
-        "nluIntentConfidenceThreshold": float,
-        "voiceSettings": VoiceSettingsTypeDef,
-        "botLocaleStatus": BotLocaleStatusType,
-        "failureReasons": List[str],
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListBotLocalesRequestRequestTypeDef = TypedDict(
     "_RequiredListBotLocalesRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
     },
 )
@@ -2777,132 +3788,131 @@
         "botVersion": str,
         "nextToken": str,
         "botLocaleSummaries": List[BotLocaleSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateBotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotRequestRequestTypeDef",
-    {
-        "botName": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-    },
-)
-_OptionalCreateBotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotRequestRequestTypeDef",
-    {
-        "description": str,
-        "botTags": Mapping[str, str],
-        "testBotAliasTags": Mapping[str, str],
-        "botType": BotTypeType,
-        "botMembers": Sequence[BotMemberTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateBotRequestRequestTypeDef(
-    _RequiredCreateBotRequestRequestTypeDef, _OptionalCreateBotRequestRequestTypeDef
-):
-    pass
-
-
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "description": str,
         "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
+        "dataPrivacy": DataPrivacyOutputTypeDef,
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "botTags": Dict[str, str],
         "testBotAliasTags": Dict[str, str],
         "botType": BotTypeType,
-        "botMembers": List[BotMemberTypeDef],
+        "botMembers": List[BotMemberOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBotResponseTypeDef = TypedDict(
     "DescribeBotResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "description": str,
         "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
+        "dataPrivacy": DataPrivacyOutputTypeDef,
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
-        "botMembers": List[BotMemberTypeDef],
+        "botMembers": List[BotMemberOutputTypeDef],
         "failureReasons": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateBotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateBotRequestRequestTypeDef",
+UpdateBotResponseTypeDef = TypedDict(
+    "UpdateBotResponseTypeDef",
     {
         "botId": str,
         "botName": str,
+        "description": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyOutputTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botStatus": BotStatusType,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "botType": BotTypeType,
+        "botMembers": List[BotMemberOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateBotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotRequestRequestTypeDef",
+    {
+        "botName": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
         "idleSessionTTLInSeconds": int,
     },
 )
-_OptionalUpdateBotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateBotRequestRequestTypeDef",
+_OptionalCreateBotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotRequestRequestTypeDef",
     {
         "description": str,
+        "botTags": Mapping[str, str],
+        "testBotAliasTags": Mapping[str, str],
         "botType": BotTypeType,
         "botMembers": Sequence[BotMemberTypeDef],
     },
     total=False,
 )
 
 
-class UpdateBotRequestRequestTypeDef(
-    _RequiredUpdateBotRequestRequestTypeDef, _OptionalUpdateBotRequestRequestTypeDef
+class CreateBotRequestRequestTypeDef(
+    _RequiredCreateBotRequestRequestTypeDef, _OptionalCreateBotRequestRequestTypeDef
 ):
     pass
 
 
-UpdateBotResponseTypeDef = TypedDict(
-    "UpdateBotResponseTypeDef",
+_RequiredUpdateBotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBotRequestRequestTypeDef",
     {
         "botId": str,
         "botName": str,
-        "description": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
         "idleSessionTTLInSeconds": int,
-        "botStatus": BotStatusType,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+    },
+)
+_OptionalUpdateBotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBotRequestRequestTypeDef",
+    {
+        "description": str,
         "botType": BotTypeType,
-        "botMembers": List[BotMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "botMembers": Sequence[BotMemberTypeDef],
     },
+    total=False,
 )
 
+
+class UpdateBotRequestRequestTypeDef(
+    _RequiredUpdateBotRequestRequestTypeDef, _OptionalUpdateBotRequestRequestTypeDef
+):
+    pass
+
+
 BotRecommendationResultStatisticsTypeDef = TypedDict(
     "BotRecommendationResultStatisticsTypeDef",
     {
         "intents": IntentStatisticsTypeDef,
         "slotTypes": SlotTypeStatisticsTypeDef,
     },
-    total=False,
 )
 
 ListBotRecommendationsResponseTypeDef = TypedDict(
     "ListBotRecommendationsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
@@ -2929,14 +3939,27 @@
     {
         "botSummaries": List[BotSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateBotVersionResponseTypeDef = TypedDict(
+    "CreateBotVersionResponseTypeDef",
+    {
+        "botId": str,
+        "description": str,
+        "botVersion": str,
+        "botVersionLocaleSpecification": Dict[str, BotVersionLocaleDetailsOutputTypeDef],
+        "botStatus": BotStatusType,
+        "creationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBotVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotVersionRequestRequestTypeDef",
     {
         "botId": str,
         "botVersionLocaleSpecification": Mapping[str, BotVersionLocaleDetailsTypeDef],
     },
 )
@@ -2951,27 +3974,14 @@
 
 class CreateBotVersionRequestRequestTypeDef(
     _RequiredCreateBotVersionRequestRequestTypeDef, _OptionalCreateBotVersionRequestRequestTypeDef
 ):
     pass
 
 
-CreateBotVersionResponseTypeDef = TypedDict(
-    "CreateBotVersionResponseTypeDef",
-    {
-        "botId": str,
-        "description": str,
-        "botVersion": str,
-        "botVersionLocaleSpecification": Dict[str, BotVersionLocaleDetailsTypeDef],
-        "botStatus": BotStatusType,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBotVersionsRequestRequestTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalListBotVersionsRequestRequestTypeDef = TypedDict(
@@ -3065,14 +4075,24 @@
         "builtInSlotTypeSummaries": List[BuiltInSlotTypeSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ImageResponseCardOutputTypeDef = TypedDict(
+    "ImageResponseCardOutputTypeDef",
+    {
+        "title": str,
+        "subtitle": str,
+        "imageUrl": str,
+        "buttons": List[ButtonOutputTypeDef],
+    },
+)
+
 _RequiredImageResponseCardTypeDef = TypedDict(
     "_RequiredImageResponseCardTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardTypeDef = TypedDict(
@@ -3088,59 +4108,67 @@
 
 class ImageResponseCardTypeDef(
     _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
 ):
     pass
 
 
+TextLogDestinationOutputTypeDef = TypedDict(
+    "TextLogDestinationOutputTypeDef",
+    {
+        "cloudWatch": CloudWatchLogGroupLogDestinationOutputTypeDef,
+    },
+)
+
 TextLogDestinationTypeDef = TypedDict(
     "TextLogDestinationTypeDef",
     {
         "cloudWatch": CloudWatchLogGroupLogDestinationTypeDef,
     },
 )
 
+CodeHookSpecificationOutputTypeDef = TypedDict(
+    "CodeHookSpecificationOutputTypeDef",
+    {
+        "lambdaCodeHook": LambdaCodeHookOutputTypeDef,
+    },
+)
+
 CodeHookSpecificationTypeDef = TypedDict(
     "CodeHookSpecificationTypeDef",
     {
         "lambdaCodeHook": LambdaCodeHookTypeDef,
     },
 )
 
+CompositeSlotTypeSettingOutputTypeDef = TypedDict(
+    "CompositeSlotTypeSettingOutputTypeDef",
+    {
+        "subSlots": List[SubSlotTypeCompositionOutputTypeDef],
+    },
+)
+
 CompositeSlotTypeSettingTypeDef = TypedDict(
     "CompositeSlotTypeSettingTypeDef",
     {
         "subSlots": Sequence[SubSlotTypeCompositionTypeDef],
     },
     total=False,
 )
 
-_RequiredConversationLevelTestResultItemTypeDef = TypedDict(
-    "_RequiredConversationLevelTestResultItemTypeDef",
+ConversationLevelTestResultItemTypeDef = TypedDict(
+    "ConversationLevelTestResultItemTypeDef",
     {
         "conversationId": str,
         "endToEndResult": TestResultMatchStatusType,
+        "speechTranscriptionResult": TestResultMatchStatusType,
         "intentClassificationResults": List[ConversationLevelIntentClassificationResultItemTypeDef],
         "slotResolutionResults": List[ConversationLevelSlotResolutionResultItemTypeDef],
     },
 )
-_OptionalConversationLevelTestResultItemTypeDef = TypedDict(
-    "_OptionalConversationLevelTestResultItemTypeDef",
-    {
-        "speechTranscriptionResult": TestResultMatchStatusType,
-    },
-    total=False,
-)
-
-
-class ConversationLevelTestResultItemTypeDef(
-    _RequiredConversationLevelTestResultItemTypeDef, _OptionalConversationLevelTestResultItemTypeDef
-):
-    pass
-
 
 _RequiredTestExecutionResultFilterByTypeDef = TypedDict(
     "_RequiredTestExecutionResultFilterByTypeDef",
     {
         "resultTypeFilter": TestResultTypeFilterType,
     },
 )
@@ -3155,14 +4183,24 @@
 
 class TestExecutionResultFilterByTypeDef(
     _RequiredTestExecutionResultFilterByTypeDef, _OptionalTestExecutionResultFilterByTypeDef
 ):
     pass
 
 
+ConversationLogsDataSourceOutputTypeDef = TypedDict(
+    "ConversationLogsDataSourceOutputTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "filter": ConversationLogsDataSourceFilterByOutputTypeDef,
+    },
+)
+
 ConversationLogsDataSourceTypeDef = TypedDict(
     "ConversationLogsDataSourceTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "filter": ConversationLogsDataSourceFilterByTypeDef,
@@ -3172,19 +4210,18 @@
 IntentSummaryTypeDef = TypedDict(
     "IntentSummaryTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateResourcePolicyStatementRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourcePolicyStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "statementId": str,
@@ -3206,14 +4243,21 @@
 class CreateResourcePolicyStatementRequestRequestTypeDef(
     _RequiredCreateResourcePolicyStatementRequestRequestTypeDef,
     _OptionalCreateResourcePolicyStatementRequestRequestTypeDef,
 ):
     pass
 
 
+LexTranscriptFilterOutputTypeDef = TypedDict(
+    "LexTranscriptFilterOutputTypeDef",
+    {
+        "dateRangeFilter": DateRangeFilterOutputTypeDef,
+    },
+)
+
 LexTranscriptFilterTypeDef = TypedDict(
     "LexTranscriptFilterTypeDef",
     {
         "dateRangeFilter": DateRangeFilterTypeDef,
     },
     total=False,
 )
@@ -3406,48 +4450,37 @@
     "DescribeBotVersionResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "botVersion": str,
         "description": str,
         "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
+        "dataPrivacy": DataPrivacyOutputTypeDef,
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
         "botType": BotTypeType,
-        "botMembers": List[BotMemberTypeDef],
+        "botMembers": List[BotMemberOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateBotRecommendationRequestRequestTypeDef = TypedDict(
-    "UpdateBotRecommendationRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botRecommendationId": str,
-        "encryptionSetting": EncryptionSettingTypeDef,
-    },
-)
-
 DescribeTestSetResponseTypeDef = TypedDict(
     "DescribeTestSetResponseTypeDef",
     {
         "testSetId": str,
         "testSetName": str,
         "description": str,
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
-        "storageLocation": TestSetStorageLocationTypeDef,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestSetSummaryTypeDef = TypedDict(
@@ -3456,48 +4489,77 @@
         "testSetId": str,
         "testSetName": str,
         "description": str,
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
-        "storageLocation": TestSetStorageLocationTypeDef,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 UpdateTestSetResponseTypeDef = TypedDict(
     "UpdateTestSetResponseTypeDef",
     {
         "testSetId": str,
         "testSetName": str,
         "description": str,
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
-        "storageLocation": TestSetStorageLocationTypeDef,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DialogStateOutputTypeDef = TypedDict(
+    "DialogStateOutputTypeDef",
+    {
+        "dialogAction": DialogActionOutputTypeDef,
+        "intent": IntentOverrideOutputTypeDef,
+        "sessionAttributes": Dict[str, str],
+    },
+)
+
 DialogStateTypeDef = TypedDict(
     "DialogStateTypeDef",
     {
         "dialogAction": DialogActionTypeDef,
         "intent": IntentOverrideTypeDef,
         "sessionAttributes": Mapping[str, str],
     },
     total=False,
 )
 
+UpdateBotRecommendationRequestRequestTypeDef = TypedDict(
+    "UpdateBotRecommendationRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botRecommendationId": str,
+        "encryptionSetting": EncryptionSettingTypeDef,
+    },
+)
+
+ExportResourceSpecificationOutputTypeDef = TypedDict(
+    "ExportResourceSpecificationOutputTypeDef",
+    {
+        "botExportSpecification": BotExportSpecificationOutputTypeDef,
+        "botLocaleExportSpecification": BotLocaleExportSpecificationOutputTypeDef,
+        "customVocabularyExportSpecification": CustomVocabularyExportSpecificationOutputTypeDef,
+        "testSetExportSpecification": TestSetExportSpecificationOutputTypeDef,
+    },
+)
+
 ExportResourceSpecificationTypeDef = TypedDict(
     "ExportResourceSpecificationTypeDef",
     {
         "botExportSpecification": BotExportSpecificationTypeDef,
         "botLocaleExportSpecification": BotLocaleExportSpecificationTypeDef,
         "customVocabularyExportSpecification": CustomVocabularyExportSpecificationTypeDef,
         "testSetExportSpecification": TestSetExportSpecificationTypeDef,
@@ -3515,14 +4577,21 @@
         "maxResults": int,
         "nextToken": str,
         "localeId": str,
     },
     total=False,
 )
 
+GrammarSlotTypeSettingOutputTypeDef = TypedDict(
+    "GrammarSlotTypeSettingOutputTypeDef",
+    {
+        "source": GrammarSlotTypeSourceOutputTypeDef,
+    },
+)
+
 GrammarSlotTypeSettingTypeDef = TypedDict(
     "GrammarSlotTypeSettingTypeDef",
     {
         "source": GrammarSlotTypeSourceTypeDef,
     },
     total=False,
 )
@@ -3556,15 +4625,14 @@
 InputSessionStateSpecificationTypeDef = TypedDict(
     "InputSessionStateSpecificationTypeDef",
     {
         "sessionAttributes": Dict[str, str],
         "activeContexts": List[ActiveContextTypeDef],
         "runtimeHints": RuntimeHintsTypeDef,
     },
-    total=False,
 )
 
 IntentClassificationTestResultItemTypeDef = TypedDict(
     "IntentClassificationTestResultItemTypeDef",
     {
         "intentName": str,
         "multiTurnConversation": bool,
@@ -3594,27 +4662,73 @@
 
 class ListIntentsRequestRequestTypeDef(
     _RequiredListIntentsRequestRequestTypeDef, _OptionalListIntentsRequestRequestTypeDef
 ):
     pass
 
 
+SessionSpecificationTypeDef = TypedDict(
+    "SessionSpecificationTypeDef",
+    {
+        "botAliasId": str,
+        "botVersion": str,
+        "localeId": str,
+        "channel": BotChannelTypeType,
+        "sessionId": str,
+        "conversationStartTime": datetime,
+        "conversationEndTime": datetime,
+        "conversationDurationSeconds": int,
+        "conversationEndState": ConversationEndStateType,
+        "mode": AnalyticsModalityType,
+        "numberOfTurns": int,
+        "invokedIntentSamples": List[InvokedIntentSampleTypeDef],
+        "originatingRequestId": str,
+    },
+)
+
 ListRecommendedIntentsResponseTypeDef = TypedDict(
     "ListRecommendedIntentsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
         "summaryList": List[RecommendedIntentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredListSessionAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_RequiredListSessionAnalyticsDataRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+    },
+)
+_OptionalListSessionAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_OptionalListSessionAnalyticsDataRequestRequestTypeDef",
+    {
+        "sortBy": SessionDataSortByTypeDef,
+        "filters": Sequence[AnalyticsSessionFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListSessionAnalyticsDataRequestRequestTypeDef(
+    _RequiredListSessionAnalyticsDataRequestRequestTypeDef,
+    _OptionalListSessionAnalyticsDataRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredListSlotTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListSlotTypesRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -3692,46 +4806,94 @@
         "sortBy": TestSetSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListUtteranceAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_RequiredListUtteranceAnalyticsDataRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+    },
+)
+_OptionalListUtteranceAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_OptionalListUtteranceAnalyticsDataRequestRequestTypeDef",
+    {
+        "sortBy": UtteranceDataSortByTypeDef,
+        "filters": Sequence[AnalyticsUtteranceFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListUtteranceAnalyticsDataRequestRequestTypeDef(
+    _RequiredListUtteranceAnalyticsDataRequestRequestTypeDef,
+    _OptionalListUtteranceAnalyticsDataRequestRequestTypeDef,
+):
+    pass
+
+
 OverallTestResultsTypeDef = TypedDict(
     "OverallTestResultsTypeDef",
     {
         "items": List[OverallTestResultItemTypeDef],
     },
 )
 
+UtteranceAggregationDurationOutputTypeDef = TypedDict(
+    "UtteranceAggregationDurationOutputTypeDef",
+    {
+        "relativeAggregationDuration": RelativeAggregationDurationOutputTypeDef,
+    },
+)
+
 UtteranceAggregationDurationTypeDef = TypedDict(
     "UtteranceAggregationDurationTypeDef",
     {
         "relativeAggregationDuration": RelativeAggregationDurationTypeDef,
     },
 )
 
 RuntimeHintDetailsTypeDef = TypedDict(
     "RuntimeHintDetailsTypeDef",
     {
         "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
-    total=False,
+)
+
+SlotTypeValueOutputTypeDef = TypedDict(
+    "SlotTypeValueOutputTypeDef",
+    {
+        "sampleValue": SampleValueOutputTypeDef,
+        "synonyms": List[SampleValueOutputTypeDef],
+    },
 )
 
 SlotTypeValueTypeDef = TypedDict(
     "SlotTypeValueTypeDef",
     {
         "sampleValue": SampleValueTypeDef,
         "synonyms": Sequence[SampleValueTypeDef],
     },
     total=False,
 )
 
+SlotDefaultValueSpecificationOutputTypeDef = TypedDict(
+    "SlotDefaultValueSpecificationOutputTypeDef",
+    {
+        "defaultValueList": List[SlotDefaultValueOutputTypeDef],
+    },
+)
+
 SlotDefaultValueSpecificationTypeDef = TypedDict(
     "SlotDefaultValueSpecificationTypeDef",
     {
         "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
@@ -3739,24 +4901,42 @@
     "SlotResolutionTestResultItemTypeDef",
     {
         "slotName": str,
         "resultCounts": SlotResolutionTestResultItemCountsTypeDef,
     },
 )
 
+SlotValueOverrideOutputTypeDef = TypedDict(
+    "SlotValueOverrideOutputTypeDef",
+    {
+        "shape": SlotShapeType,
+        "value": SlotValueOutputTypeDef,
+        "values": List[Dict[str, Any]],
+    },
+)
+
 SlotValueOverrideTypeDef = TypedDict(
     "SlotValueOverrideTypeDef",
     {
         "shape": SlotShapeType,
         "value": SlotValueTypeDef,
         "values": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+SlotValueSelectionSettingOutputTypeDef = TypedDict(
+    "SlotValueSelectionSettingOutputTypeDef",
+    {
+        "resolutionStrategy": SlotValueResolutionStrategyType,
+        "regexFilter": SlotValueRegexFilterOutputTypeDef,
+        "advancedRecognitionSetting": AdvancedRecognitionSettingOutputTypeDef,
+    },
+)
+
 _RequiredSlotValueSelectionSettingTypeDef = TypedDict(
     "_RequiredSlotValueSelectionSettingTypeDef",
     {
         "resolutionStrategy": SlotValueResolutionStrategyType,
     },
 )
 _OptionalSlotValueSelectionSettingTypeDef = TypedDict(
@@ -3779,78 +4959,134 @@
     "TestSetDiscrepancyErrorsTypeDef",
     {
         "intentDiscrepancies": List[TestSetIntentDiscrepancyItemTypeDef],
         "slotDiscrepancies": List[TestSetSlotDiscrepancyItemTypeDef],
     },
 )
 
+TestSetDiscrepancyReportResourceTargetOutputTypeDef = TypedDict(
+    "TestSetDiscrepancyReportResourceTargetOutputTypeDef",
+    {
+        "botAliasTarget": TestSetDiscrepancyReportBotAliasTargetOutputTypeDef,
+    },
+)
+
 TestSetDiscrepancyReportResourceTargetTypeDef = TypedDict(
     "TestSetDiscrepancyReportResourceTargetTypeDef",
     {
         "botAliasTarget": TestSetDiscrepancyReportBotAliasTargetTypeDef,
     },
     total=False,
 )
 
+TestSetImportResourceSpecificationOutputTypeDef = TypedDict(
+    "TestSetImportResourceSpecificationOutputTypeDef",
+    {
+        "testSetName": str,
+        "description": str,
+        "roleArn": str,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
+        "importInputLocation": TestSetImportInputLocationOutputTypeDef,
+        "modality": TestSetModalityType,
+        "testSetTags": Dict[str, str],
+    },
+)
+
 _RequiredTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_RequiredTestSetImportResourceSpecificationTypeDef",
     {
         "testSetName": str,
         "roleArn": str,
         "storageLocation": TestSetStorageLocationTypeDef,
         "importInputLocation": TestSetImportInputLocationTypeDef,
         "modality": TestSetModalityType,
     },
 )
 _OptionalTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_OptionalTestSetImportResourceSpecificationTypeDef",
     {
         "description": str,
-        "testSetTags": Dict[str, str],
+        "testSetTags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class TestSetImportResourceSpecificationTypeDef(
     _RequiredTestSetImportResourceSpecificationTypeDef,
     _OptionalTestSetImportResourceSpecificationTypeDef,
 ):
     pass
 
 
-_RequiredUserTurnOutputSpecificationTypeDef = TypedDict(
-    "_RequiredUserTurnOutputSpecificationTypeDef",
+UserTurnOutputSpecificationTypeDef = TypedDict(
+    "UserTurnOutputSpecificationTypeDef",
     {
         "intent": UserTurnIntentOutputTypeDef,
-    },
-)
-_OptionalUserTurnOutputSpecificationTypeDef = TypedDict(
-    "_OptionalUserTurnOutputSpecificationTypeDef",
-    {
         "activeContexts": List[ActiveContextTypeDef],
         "transcript": str,
     },
-    total=False,
 )
 
-
-class UserTurnOutputSpecificationTypeDef(
-    _RequiredUserTurnOutputSpecificationTypeDef, _OptionalUserTurnOutputSpecificationTypeDef
-):
-    pass
-
-
 UtteranceInputSpecificationTypeDef = TypedDict(
     "UtteranceInputSpecificationTypeDef",
     {
         "textInput": str,
         "audioInput": UtteranceAudioInputSpecificationTypeDef,
     },
-    total=False,
+)
+
+ListIntentMetricsResponseTypeDef = TypedDict(
+    "ListIntentMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsIntentResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListIntentStageMetricsResponseTypeDef = TypedDict(
+    "ListIntentStageMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsIntentStageResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSessionMetricsResponseTypeDef = TypedDict(
+    "ListSessionMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsSessionResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListUtteranceMetricsResponseTypeDef = TypedDict(
+    "ListUtteranceMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsUtteranceResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PromptAttemptSpecificationOutputTypeDef = TypedDict(
+    "PromptAttemptSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+        "allowedInputTypes": AllowedInputTypesOutputTypeDef,
+        "audioAndDTMFInputSpecification": AudioAndDTMFInputSpecificationOutputTypeDef,
+        "textInputSpecification": TextInputSpecificationOutputTypeDef,
+    },
 )
 
 _RequiredPromptAttemptSpecificationTypeDef = TypedDict(
     "_RequiredPromptAttemptSpecificationTypeDef",
     {
         "allowedInputTypes": AllowedInputTypesTypeDef,
     },
@@ -3868,14 +5104,22 @@
 
 class PromptAttemptSpecificationTypeDef(
     _RequiredPromptAttemptSpecificationTypeDef, _OptionalPromptAttemptSpecificationTypeDef
 ):
     pass
 
 
+AudioLogSettingOutputTypeDef = TypedDict(
+    "AudioLogSettingOutputTypeDef",
+    {
+        "enabled": bool,
+        "destination": AudioLogDestinationOutputTypeDef,
+    },
+)
+
 AudioLogSettingTypeDef = TypedDict(
     "AudioLogSettingTypeDef",
     {
         "enabled": bool,
         "destination": AudioLogDestinationTypeDef,
     },
 )
@@ -3885,53 +5129,29 @@
     {
         "testExecutionId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "testExecutionStatus": TestExecutionStatusType,
         "testSetId": str,
         "testSetName": str,
-        "target": TestExecutionTargetTypeDef,
+        "target": TestExecutionTargetOutputTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
         "failureReasons": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartTestExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartTestExecutionRequestRequestTypeDef",
-    {
-        "testSetId": str,
-        "target": TestExecutionTargetTypeDef,
-        "apiMode": TestExecutionApiModeType,
-    },
-)
-_OptionalStartTestExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartTestExecutionRequestRequestTypeDef",
-    {
-        "testExecutionModality": TestExecutionModalityType,
-    },
-    total=False,
-)
-
-
-class StartTestExecutionRequestRequestTypeDef(
-    _RequiredStartTestExecutionRequestRequestTypeDef,
-    _OptionalStartTestExecutionRequestRequestTypeDef,
-):
-    pass
-
-
 StartTestExecutionResponseTypeDef = TypedDict(
     "StartTestExecutionResponseTypeDef",
     {
         "testExecutionId": str,
         "creationDateTime": datetime,
         "testSetId": str,
-        "target": TestExecutionTargetTypeDef,
+        "target": TestExecutionTargetOutputTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestExecutionSummaryTypeDef = TypedDict(
@@ -3939,50 +5159,107 @@
     {
         "testExecutionId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "testExecutionStatus": TestExecutionStatusType,
         "testSetId": str,
         "testSetName": str,
+        "target": TestExecutionTargetOutputTypeDef,
+        "apiMode": TestExecutionApiModeType,
+        "testExecutionModality": TestExecutionModalityType,
+    },
+)
+
+_RequiredStartTestExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartTestExecutionRequestRequestTypeDef",
+    {
+        "testSetId": str,
         "target": TestExecutionTargetTypeDef,
         "apiMode": TestExecutionApiModeType,
+    },
+)
+_OptionalStartTestExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartTestExecutionRequestRequestTypeDef",
+    {
         "testExecutionModality": TestExecutionModalityType,
     },
     total=False,
 )
 
+
+class StartTestExecutionRequestRequestTypeDef(
+    _RequiredStartTestExecutionRequestRequestTypeDef,
+    _OptionalStartTestExecutionRequestRequestTypeDef,
+):
+    pass
+
+
 BotRecommendationResultsTypeDef = TypedDict(
     "BotRecommendationResultsTypeDef",
     {
         "botLocaleExportUrl": str,
         "associatedTranscriptsUrl": str,
         "statistics": BotRecommendationResultStatisticsTypeDef,
     },
-    total=False,
+)
+
+MessageOutputTypeDef = TypedDict(
+    "MessageOutputTypeDef",
+    {
+        "plainTextMessage": PlainTextMessageOutputTypeDef,
+        "customPayload": CustomPayloadOutputTypeDef,
+        "ssmlMessage": SSMLMessageOutputTypeDef,
+        "imageResponseCard": ImageResponseCardOutputTypeDef,
+    },
+)
+
+UtteranceBotResponseTypeDef = TypedDict(
+    "UtteranceBotResponseTypeDef",
+    {
+        "content": str,
+        "contentType": UtteranceContentTypeType,
+        "imageResponseCard": ImageResponseCardOutputTypeDef,
+    },
 )
 
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "plainTextMessage": PlainTextMessageTypeDef,
         "customPayload": CustomPayloadTypeDef,
         "ssmlMessage": SSMLMessageTypeDef,
         "imageResponseCard": ImageResponseCardTypeDef,
     },
     total=False,
 )
 
+TextLogSettingOutputTypeDef = TypedDict(
+    "TextLogSettingOutputTypeDef",
+    {
+        "enabled": bool,
+        "destination": TextLogDestinationOutputTypeDef,
+    },
+)
+
 TextLogSettingTypeDef = TypedDict(
     "TextLogSettingTypeDef",
     {
         "enabled": bool,
         "destination": TextLogDestinationTypeDef,
     },
 )
 
+BotAliasLocaleSettingsOutputTypeDef = TypedDict(
+    "BotAliasLocaleSettingsOutputTypeDef",
+    {
+        "enabled": bool,
+        "codeHookSpecification": CodeHookSpecificationOutputTypeDef,
+    },
+)
+
 _RequiredBotAliasLocaleSettingsTypeDef = TypedDict(
     "_RequiredBotAliasLocaleSettingsTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalBotAliasLocaleSettingsTypeDef = TypedDict(
@@ -4027,14 +5304,21 @@
 class ListTestExecutionResultItemsRequestRequestTypeDef(
     _RequiredListTestExecutionResultItemsRequestRequestTypeDef,
     _OptionalListTestExecutionResultItemsRequestRequestTypeDef,
 ):
     pass
 
 
+TestSetGenerationDataSourceOutputTypeDef = TypedDict(
+    "TestSetGenerationDataSourceOutputTypeDef",
+    {
+        "conversationLogsDataSource": ConversationLogsDataSourceOutputTypeDef,
+    },
+)
+
 TestSetGenerationDataSourceTypeDef = TypedDict(
     "TestSetGenerationDataSourceTypeDef",
     {
         "conversationLogsDataSource": ConversationLogsDataSourceTypeDef,
     },
     total=False,
 )
@@ -4047,14 +5331,21 @@
         "localeId": str,
         "intentSummaries": List[IntentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
+    {
+        "lexTranscriptFilter": LexTranscriptFilterOutputTypeDef,
+    },
+)
+
 TranscriptFilterTypeDef = TypedDict(
     "TranscriptFilterTypeDef",
     {
         "lexTranscriptFilter": LexTranscriptFilterTypeDef,
     },
     total=False,
 )
@@ -4064,89 +5355,95 @@
     {
         "testSets": List[TestSetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateExportRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateExportRequestRequestTypeDef",
-    {
-        "resourceSpecification": ExportResourceSpecificationTypeDef,
-        "fileFormat": ImportExportFileFormatType,
-    },
-)
-_OptionalCreateExportRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateExportRequestRequestTypeDef",
-    {
-        "filePassword": str,
-    },
-    total=False,
-)
-
-
-class CreateExportRequestRequestTypeDef(
-    _RequiredCreateExportRequestRequestTypeDef, _OptionalCreateExportRequestRequestTypeDef
-):
-    pass
-
-
 CreateExportResponseTypeDef = TypedDict(
     "CreateExportResponseTypeDef",
     {
         "exportId": str,
-        "resourceSpecification": ExportResourceSpecificationTypeDef,
+        "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExportResponseTypeDef = TypedDict(
     "DescribeExportResponseTypeDef",
     {
         "exportId": str,
-        "resourceSpecification": ExportResourceSpecificationTypeDef,
+        "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "failureReasons": List[str],
         "downloadUrl": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "exportId": str,
-        "resourceSpecification": ExportResourceSpecificationTypeDef,
+        "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 UpdateExportResponseTypeDef = TypedDict(
     "UpdateExportResponseTypeDef",
     {
         "exportId": str,
-        "resourceSpecification": ExportResourceSpecificationTypeDef,
+        "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateExportRequestRequestTypeDef",
+    {
+        "resourceSpecification": ExportResourceSpecificationTypeDef,
+        "fileFormat": ImportExportFileFormatType,
+    },
+)
+_OptionalCreateExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateExportRequestRequestTypeDef",
+    {
+        "filePassword": str,
+    },
+    total=False,
+)
+
+
+class CreateExportRequestRequestTypeDef(
+    _RequiredCreateExportRequestRequestTypeDef, _OptionalCreateExportRequestRequestTypeDef
+):
+    pass
+
+
+ExternalSourceSettingOutputTypeDef = TypedDict(
+    "ExternalSourceSettingOutputTypeDef",
+    {
+        "grammarSlotTypeSetting": GrammarSlotTypeSettingOutputTypeDef,
+    },
+)
+
 ExternalSourceSettingTypeDef = TypedDict(
     "ExternalSourceSettingTypeDef",
     {
         "grammarSlotTypeSetting": GrammarSlotTypeSettingTypeDef,
     },
     total=False,
 )
@@ -4154,14 +5451,41 @@
 IntentClassificationTestResultsTypeDef = TypedDict(
     "IntentClassificationTestResultsTypeDef",
     {
         "items": List[IntentClassificationTestResultItemTypeDef],
     },
 )
 
+ListSessionAnalyticsDataResponseTypeDef = TypedDict(
+    "ListSessionAnalyticsDataResponseTypeDef",
+    {
+        "botId": str,
+        "nextToken": str,
+        "sessions": List[SessionSpecificationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAggregatedUtterancesResponseTypeDef = TypedDict(
+    "ListAggregatedUtterancesResponseTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "botVersion": str,
+        "localeId": str,
+        "aggregationDuration": UtteranceAggregationDurationOutputTypeDef,
+        "aggregationWindowStartTime": datetime,
+        "aggregationWindowEndTime": datetime,
+        "aggregationLastRefreshedDateTime": datetime,
+        "aggregatedUtterancesSummaries": List[AggregatedUtterancesSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListAggregatedUtterancesRequestRequestTypeDef = TypedDict(
     "_RequiredListAggregatedUtterancesRequestRequestTypeDef",
     {
         "botId": str,
         "localeId": str,
         "aggregationDuration": UtteranceAggregationDurationTypeDef,
     },
@@ -4183,117 +5507,133 @@
 class ListAggregatedUtterancesRequestRequestTypeDef(
     _RequiredListAggregatedUtterancesRequestRequestTypeDef,
     _OptionalListAggregatedUtterancesRequestRequestTypeDef,
 ):
     pass
 
 
-ListAggregatedUtterancesResponseTypeDef = TypedDict(
-    "ListAggregatedUtterancesResponseTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "botVersion": str,
-        "localeId": str,
-        "aggregationDuration": UtteranceAggregationDurationTypeDef,
-        "aggregationWindowStartTime": datetime,
-        "aggregationWindowEndTime": datetime,
-        "aggregationLastRefreshedDateTime": datetime,
-        "aggregatedUtterancesSummaries": List[AggregatedUtterancesSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IntentLevelSlotResolutionTestResultItemTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultItemTypeDef",
     {
         "intentName": str,
         "multiTurnConversation": bool,
         "slotResolutionResults": List[SlotResolutionTestResultItemTypeDef],
     },
 )
 
-CreateTestSetDiscrepancyReportRequestRequestTypeDef = TypedDict(
-    "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
-    {
-        "testSetId": str,
-        "target": TestSetDiscrepancyReportResourceTargetTypeDef,
-    },
-)
-
 CreateTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
         "creationDateTime": datetime,
         "testSetId": str,
-        "target": TestSetDiscrepancyReportResourceTargetTypeDef,
+        "target": TestSetDiscrepancyReportResourceTargetOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
         "testSetId": str,
         "creationDateTime": datetime,
-        "target": TestSetDiscrepancyReportResourceTargetTypeDef,
+        "target": TestSetDiscrepancyReportResourceTargetOutputTypeDef,
         "testSetDiscrepancyReportStatus": TestSetDiscrepancyReportStatusType,
         "lastUpdatedDataTime": datetime,
         "testSetDiscrepancyTopErrors": TestSetDiscrepancyErrorsTypeDef,
         "testSetDiscrepancyRawOutputUrl": str,
         "failureReasons": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateTestSetDiscrepancyReportRequestRequestTypeDef = TypedDict(
+    "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
+    {
+        "testSetId": str,
+        "target": TestSetDiscrepancyReportResourceTargetTypeDef,
+    },
+)
+
+ImportResourceSpecificationOutputTypeDef = TypedDict(
+    "ImportResourceSpecificationOutputTypeDef",
+    {
+        "botImportSpecification": BotImportSpecificationOutputTypeDef,
+        "botLocaleImportSpecification": BotLocaleImportSpecificationOutputTypeDef,
+        "customVocabularyImportSpecification": CustomVocabularyImportSpecificationOutputTypeDef,
+        "testSetImportResourceSpecification": TestSetImportResourceSpecificationOutputTypeDef,
+    },
+)
+
 ImportResourceSpecificationTypeDef = TypedDict(
     "ImportResourceSpecificationTypeDef",
     {
         "botImportSpecification": BotImportSpecificationTypeDef,
         "botLocaleImportSpecification": BotLocaleImportSpecificationTypeDef,
         "customVocabularyImportSpecification": CustomVocabularyImportSpecificationTypeDef,
         "testSetImportResourceSpecification": TestSetImportResourceSpecificationTypeDef,
     },
     total=False,
 )
 
-_RequiredUserTurnInputSpecificationTypeDef = TypedDict(
-    "_RequiredUserTurnInputSpecificationTypeDef",
+UserTurnInputSpecificationTypeDef = TypedDict(
+    "UserTurnInputSpecificationTypeDef",
     {
         "utteranceInput": UtteranceInputSpecificationTypeDef,
-    },
-)
-_OptionalUserTurnInputSpecificationTypeDef = TypedDict(
-    "_OptionalUserTurnInputSpecificationTypeDef",
-    {
         "requestAttributes": Dict[str, str],
         "sessionState": InputSessionStateSpecificationTypeDef,
     },
-    total=False,
 )
 
-
-class UserTurnInputSpecificationTypeDef(
-    _RequiredUserTurnInputSpecificationTypeDef, _OptionalUserTurnInputSpecificationTypeDef
-):
-    pass
-
-
 ListTestExecutionsResponseTypeDef = TypedDict(
     "ListTestExecutionsResponseTypeDef",
     {
         "testExecutions": List[TestExecutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MessageGroupOutputTypeDef = TypedDict(
+    "MessageGroupOutputTypeDef",
+    {
+        "message": MessageOutputTypeDef,
+        "variations": List[MessageOutputTypeDef],
+    },
+)
+
+UtteranceSpecificationTypeDef = TypedDict(
+    "UtteranceSpecificationTypeDef",
+    {
+        "botAliasId": str,
+        "botVersion": str,
+        "localeId": str,
+        "sessionId": str,
+        "channel": BotChannelTypeType,
+        "mode": AnalyticsModalityType,
+        "conversationStartTime": datetime,
+        "conversationEndTime": datetime,
+        "utterance": str,
+        "utteranceTimestamp": datetime,
+        "audioVoiceDurationMillis": int,
+        "utteranceUnderstood": bool,
+        "inputType": str,
+        "outputType": str,
+        "associatedIntentName": str,
+        "associatedSlotName": str,
+        "intentState": IntentStateType,
+        "dialogActionType": str,
+        "botResponseAudioVoiceId": str,
+        "slotsFilledInSession": str,
+        "utteranceRequestId": str,
+        "botResponses": List[UtteranceBotResponseTypeDef],
+    },
+)
+
 _RequiredMessageGroupTypeDef = TypedDict(
     "_RequiredMessageGroupTypeDef",
     {
         "message": MessageTypeDef,
     },
 )
 _OptionalMessageGroupTypeDef = TypedDict(
@@ -4305,14 +5645,22 @@
 )
 
 
 class MessageGroupTypeDef(_RequiredMessageGroupTypeDef, _OptionalMessageGroupTypeDef):
     pass
 
 
+ConversationLogSettingsOutputTypeDef = TypedDict(
+    "ConversationLogSettingsOutputTypeDef",
+    {
+        "textLogSettings": List[TextLogSettingOutputTypeDef],
+        "audioLogSettings": List[AudioLogSettingOutputTypeDef],
+    },
+)
+
 ConversationLogSettingsTypeDef = TypedDict(
     "ConversationLogSettingsTypeDef",
     {
         "textLogSettings": Sequence[TextLogSettingTypeDef],
         "audioLogSettings": Sequence[AudioLogSettingTypeDef],
     },
     total=False,
@@ -4323,23 +5671,39 @@
     {
         "testSetGenerationId": str,
         "testSetGenerationStatus": TestSetGenerationStatusType,
         "failureReasons": List[str],
         "testSetId": str,
         "testSetName": str,
         "description": str,
-        "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StartTestSetGenerationResponseTypeDef = TypedDict(
+    "StartTestSetGenerationResponseTypeDef",
+    {
+        "testSetGenerationId": str,
+        "creationDateTime": datetime,
+        "testSetGenerationStatus": TestSetGenerationStatusType,
+        "testSetName": str,
+        "description": str,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
+        "roleArn": str,
+        "testSetTags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
     "_RequiredStartTestSetGenerationRequestRequestTypeDef",
     {
         "testSetName": str,
         "storageLocation": TestSetStorageLocationTypeDef,
         "generationDataSource": TestSetGenerationDataSourceTypeDef,
         "roleArn": str,
@@ -4358,27 +5722,22 @@
 class StartTestSetGenerationRequestRequestTypeDef(
     _RequiredStartTestSetGenerationRequestRequestTypeDef,
     _OptionalStartTestSetGenerationRequestRequestTypeDef,
 ):
     pass
 
 
-StartTestSetGenerationResponseTypeDef = TypedDict(
-    "StartTestSetGenerationResponseTypeDef",
+S3BucketTranscriptSourceOutputTypeDef = TypedDict(
+    "S3BucketTranscriptSourceOutputTypeDef",
     {
-        "testSetGenerationId": str,
-        "creationDateTime": datetime,
-        "testSetGenerationStatus": TestSetGenerationStatusType,
-        "testSetName": str,
-        "description": str,
-        "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
-        "roleArn": str,
-        "testSetTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "s3BucketName": str,
+        "pathFormat": PathFormatOutputTypeDef,
+        "transcriptFormat": Literal["Lex"],
+        "transcriptFilter": TranscriptFilterOutputTypeDef,
+        "kmsKeyArn": str,
     },
 )
 
 _RequiredS3BucketTranscriptSourceTypeDef = TypedDict(
     "_RequiredS3BucketTranscriptSourceTypeDef",
     {
         "s3BucketName": str,
@@ -4410,155 +5769,167 @@
         "exportSummaries": List[ExportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotTypeRequestRequestTypeDef",
+CreateSlotTypeResponseTypeDef = TypedDict(
+    "CreateSlotTypeResponseTypeDef",
     {
+        "slotTypeId": str,
         "slotTypeName": str,
+        "description": str,
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingOutputTypeDef,
+        "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
+        "creationDateTime": datetime,
+        "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotTypeRequestRequestTypeDef",
-    {
-        "description": str,
-        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
-        "parentSlotTypeSignature": str,
-        "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateSlotTypeRequestRequestTypeDef(
-    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
-):
-    pass
-
 
-CreateSlotTypeResponseTypeDef = TypedDict(
-    "CreateSlotTypeResponseTypeDef",
+DescribeSlotTypeResponseTypeDef = TypedDict(
+    "DescribeSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingOutputTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
-        "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
+        "lastUpdatedDateTime": datetime,
+        "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSlotTypeResponseTypeDef = TypedDict(
-    "DescribeSlotTypeResponseTypeDef",
+UpdateSlotTypeResponseTypeDef = TypedDict(
+    "UpdateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingOutputTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
+        "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
+_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotTypeRequestRequestTypeDef",
     {
-        "slotTypeId": str,
         "slotTypeName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
+_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotTypeRequestRequestTypeDef",
     {
         "description": str,
         "slotTypeValues": Sequence[SlotTypeValueTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
     },
     total=False,
 )
 
 
-class UpdateSlotTypeRequestRequestTypeDef(
-    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
+class CreateSlotTypeRequestRequestTypeDef(
+    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
 ):
     pass
 
 
-UpdateSlotTypeResponseTypeDef = TypedDict(
-    "UpdateSlotTypeResponseTypeDef",
+_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
-        "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
-        "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+    },
+)
+_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
+        "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+
+class UpdateSlotTypeRequestRequestTypeDef(
+    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
+):
+    pass
+
+
 IntentLevelSlotResolutionTestResultsTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultsTypeDef",
     {
         "items": List[IntentLevelSlotResolutionTestResultItemTypeDef],
     },
 )
 
 DescribeImportResponseTypeDef = TypedDict(
     "DescribeImportResponseTypeDef",
     {
         "importId": str,
-        "resourceSpecification": ImportResourceSpecificationTypeDef,
+        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
         "importedResourceId": str,
         "importedResourceName": str,
         "mergeStrategy": MergeStrategyType,
         "importStatus": ImportStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StartImportResponseTypeDef = TypedDict(
+    "StartImportResponseTypeDef",
+    {
+        "importId": str,
+        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
+        "mergeStrategy": MergeStrategyType,
+        "importStatus": ImportStatusType,
+        "creationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
         "importId": str,
         "resourceSpecification": ImportResourceSpecificationTypeDef,
         "mergeStrategy": MergeStrategyType,
     },
@@ -4574,60 +5945,96 @@
 
 class StartImportRequestRequestTypeDef(
     _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
 ):
     pass
 
 
-StartImportResponseTypeDef = TypedDict(
-    "StartImportResponseTypeDef",
-    {
-        "importId": str,
-        "resourceSpecification": ImportResourceSpecificationTypeDef,
-        "mergeStrategy": MergeStrategyType,
-        "importStatus": ImportStatusType,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUserTurnResultTypeDef = TypedDict(
-    "_RequiredUserTurnResultTypeDef",
+UserTurnResultTypeDef = TypedDict(
+    "UserTurnResultTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expectedOutput": UserTurnOutputSpecificationTypeDef,
-    },
-)
-_OptionalUserTurnResultTypeDef = TypedDict(
-    "_OptionalUserTurnResultTypeDef",
-    {
         "actualOutput": UserTurnOutputSpecificationTypeDef,
         "errorDetails": ExecutionErrorDetailsTypeDef,
         "endToEndResult": TestResultMatchStatusType,
         "intentMatchResult": TestResultMatchStatusType,
         "slotMatchResult": TestResultMatchStatusType,
         "speechTranscriptionResult": TestResultMatchStatusType,
         "conversationLevelResult": ConversationLevelResultDetailTypeDef,
     },
-    total=False,
 )
 
-
-class UserTurnResultTypeDef(_RequiredUserTurnResultTypeDef, _OptionalUserTurnResultTypeDef):
-    pass
-
-
 UserTurnSpecificationTypeDef = TypedDict(
     "UserTurnSpecificationTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expected": UserTurnOutputSpecificationTypeDef,
     },
 )
 
+FulfillmentStartResponseSpecificationOutputTypeDef = TypedDict(
+    "FulfillmentStartResponseSpecificationOutputTypeDef",
+    {
+        "delayInSeconds": int,
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "allowInterrupt": bool,
+    },
+)
+
+FulfillmentUpdateResponseSpecificationOutputTypeDef = TypedDict(
+    "FulfillmentUpdateResponseSpecificationOutputTypeDef",
+    {
+        "frequencyInSeconds": int,
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "allowInterrupt": bool,
+    },
+)
+
+PromptSpecificationOutputTypeDef = TypedDict(
+    "PromptSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "maxRetries": int,
+        "allowInterrupt": bool,
+        "messageSelectionStrategy": MessageSelectionStrategyType,
+        "promptAttemptsSpecification": Dict[
+            PromptAttemptType, PromptAttemptSpecificationOutputTypeDef
+        ],
+    },
+)
+
+ResponseSpecificationOutputTypeDef = TypedDict(
+    "ResponseSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "allowInterrupt": bool,
+    },
+)
+
+StillWaitingResponseSpecificationOutputTypeDef = TypedDict(
+    "StillWaitingResponseSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "frequencyInSeconds": int,
+        "timeoutInSeconds": int,
+        "allowInterrupt": bool,
+    },
+)
+
+ListUtteranceAnalyticsDataResponseTypeDef = TypedDict(
+    "ListUtteranceAnalyticsDataResponseTypeDef",
+    {
+        "botId": str,
+        "nextToken": str,
+        "utterances": List[UtteranceSpecificationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFulfillmentStartResponseSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentStartResponseSpecificationTypeDef",
     {
         "delayInSeconds": int,
         "messageGroups": Sequence[MessageGroupTypeDef],
     },
 )
@@ -4737,51 +6144,24 @@
 class StillWaitingResponseSpecificationTypeDef(
     _RequiredStillWaitingResponseSpecificationTypeDef,
     _OptionalStillWaitingResponseSpecificationTypeDef,
 ):
     pass
 
 
-_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotAliasRequestRequestTypeDef",
-    {
-        "botAliasName": str,
-        "botId": str,
-    },
-)
-_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotAliasRequestRequestTypeDef",
-    {
-        "description": str,
-        "botVersion": str,
-        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateBotAliasRequestRequestTypeDef(
-    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
-):
-    pass
-
-
 CreateBotAliasResponseTypeDef = TypedDict(
     "CreateBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsOutputTypeDef],
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4789,69 +6169,103 @@
 DescribeBotAliasResponseTypeDef = TypedDict(
     "DescribeBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsOutputTypeDef],
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
         "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateBotAliasRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateBotAliasRequestRequestTypeDef",
+UpdateBotAliasResponseTypeDef = TypedDict(
+    "UpdateBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
+        "description": str,
+        "botVersion": str,
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsOutputTypeDef],
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
+        "botAliasStatus": BotAliasStatusType,
         "botId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalUpdateBotAliasRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateBotAliasRequestRequestTypeDef",
+
+_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotAliasRequestRequestTypeDef",
+    {
+        "botAliasName": str,
+        "botId": str,
+    },
+)
+_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotAliasRequestRequestTypeDef",
     {
         "description": str,
         "botVersion": str,
         "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
         "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class UpdateBotAliasRequestRequestTypeDef(
-    _RequiredUpdateBotAliasRequestRequestTypeDef, _OptionalUpdateBotAliasRequestRequestTypeDef
+class CreateBotAliasRequestRequestTypeDef(
+    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
 ):
     pass
 
 
-UpdateBotAliasResponseTypeDef = TypedDict(
-    "UpdateBotAliasResponseTypeDef",
+_RequiredUpdateBotAliasRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBotAliasRequestRequestTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
+        "botId": str,
+    },
+)
+_OptionalUpdateBotAliasRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBotAliasRequestRequestTypeDef",
+    {
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
+        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
         "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "botAliasStatus": BotAliasStatusType,
-        "botId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+    total=False,
+)
+
+
+class UpdateBotAliasRequestRequestTypeDef(
+    _RequiredUpdateBotAliasRequestRequestTypeDef, _OptionalUpdateBotAliasRequestRequestTypeDef
+):
+    pass
+
+
+TranscriptSourceSettingOutputTypeDef = TypedDict(
+    "TranscriptSourceSettingOutputTypeDef",
+    {
+        "s3BucketTranscriptSource": S3BucketTranscriptSourceOutputTypeDef,
     },
 )
 
 TranscriptSourceSettingTypeDef = TypedDict(
     "TranscriptSourceSettingTypeDef",
     {
         "s3BucketTranscriptSource": S3BucketTranscriptSourceTypeDef,
@@ -4861,24 +6275,73 @@
 
 TestSetTurnResultTypeDef = TypedDict(
     "TestSetTurnResultTypeDef",
     {
         "agent": AgentTurnResultTypeDef,
         "user": UserTurnResultTypeDef,
     },
-    total=False,
 )
 
 TurnSpecificationTypeDef = TypedDict(
     "TurnSpecificationTypeDef",
     {
         "agentTurn": AgentTurnSpecificationTypeDef,
         "userTurn": UserTurnSpecificationTypeDef,
     },
-    total=False,
+)
+
+FulfillmentUpdatesSpecificationOutputTypeDef = TypedDict(
+    "FulfillmentUpdatesSpecificationOutputTypeDef",
+    {
+        "active": bool,
+        "startResponse": FulfillmentStartResponseSpecificationOutputTypeDef,
+        "updateResponse": FulfillmentUpdateResponseSpecificationOutputTypeDef,
+        "timeoutInSeconds": int,
+    },
+)
+
+SlotSummaryTypeDef = TypedDict(
+    "SlotSummaryTypeDef",
+    {
+        "slotId": str,
+        "slotName": str,
+        "description": str,
+        "slotConstraint": SlotConstraintType,
+        "slotTypeId": str,
+        "valueElicitationPromptSpecification": PromptSpecificationOutputTypeDef,
+        "lastUpdatedDateTime": datetime,
+    },
+)
+
+ConditionalBranchOutputTypeDef = TypedDict(
+    "ConditionalBranchOutputTypeDef",
+    {
+        "name": str,
+        "condition": ConditionOutputTypeDef,
+        "nextStep": DialogStateOutputTypeDef,
+        "response": ResponseSpecificationOutputTypeDef,
+    },
+)
+
+DefaultConditionalBranchOutputTypeDef = TypedDict(
+    "DefaultConditionalBranchOutputTypeDef",
+    {
+        "nextStep": DialogStateOutputTypeDef,
+        "response": ResponseSpecificationOutputTypeDef,
+    },
+)
+
+WaitAndContinueSpecificationOutputTypeDef = TypedDict(
+    "WaitAndContinueSpecificationOutputTypeDef",
+    {
+        "waitingResponse": ResponseSpecificationOutputTypeDef,
+        "continueResponse": ResponseSpecificationOutputTypeDef,
+        "stillWaitingResponse": StillWaitingResponseSpecificationOutputTypeDef,
+        "active": bool,
+    },
 )
 
 _RequiredFulfillmentUpdatesSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentUpdatesSpecificationTypeDef",
     {
         "active": bool,
     },
@@ -4896,28 +6359,14 @@
 
 class FulfillmentUpdatesSpecificationTypeDef(
     _RequiredFulfillmentUpdatesSpecificationTypeDef, _OptionalFulfillmentUpdatesSpecificationTypeDef
 ):
     pass
 
 
-SlotSummaryTypeDef = TypedDict(
-    "SlotSummaryTypeDef",
-    {
-        "slotId": str,
-        "slotName": str,
-        "description": str,
-        "slotConstraint": SlotConstraintType,
-        "slotTypeId": str,
-        "valueElicitationPromptSpecification": PromptSpecificationTypeDef,
-        "lastUpdatedDateTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredConditionalBranchTypeDef = TypedDict(
     "_RequiredConditionalBranchTypeDef",
     {
         "name": str,
         "condition": ConditionTypeDef,
         "nextStep": DialogStateTypeDef,
     },
@@ -4976,135 +6425,128 @@
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-        "encryptionSetting": EncryptionSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "encryptionSetting": EncryptionSettingOutputTypeDef,
         "botRecommendationResults": BotRecommendationResultsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartBotRecommendationRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-    },
-)
-_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartBotRecommendationRequestRequestTypeDef",
-    {
-        "encryptionSetting": EncryptionSettingTypeDef,
-    },
-    total=False,
-)
-
-
-class StartBotRecommendationRequestRequestTypeDef(
-    _RequiredStartBotRecommendationRequestRequestTypeDef,
-    _OptionalStartBotRecommendationRequestRequestTypeDef,
-):
-    pass
-
-
 StartBotRecommendationResponseTypeDef = TypedDict(
     "StartBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-        "encryptionSetting": EncryptionSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "encryptionSetting": EncryptionSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBotRecommendationResponseTypeDef = TypedDict(
     "UpdateBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-        "encryptionSetting": EncryptionSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "encryptionSetting": EncryptionSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUtteranceLevelTestResultItemTypeDef = TypedDict(
-    "_RequiredUtteranceLevelTestResultItemTypeDef",
+_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartBotRecommendationRequestRequestTypeDef",
     {
-        "recordNumber": int,
-        "turnResult": TestSetTurnResultTypeDef,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
     },
 )
-_OptionalUtteranceLevelTestResultItemTypeDef = TypedDict(
-    "_OptionalUtteranceLevelTestResultItemTypeDef",
+_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartBotRecommendationRequestRequestTypeDef",
     {
-        "conversationId": str,
+        "encryptionSetting": EncryptionSettingTypeDef,
     },
     total=False,
 )
 
 
-class UtteranceLevelTestResultItemTypeDef(
-    _RequiredUtteranceLevelTestResultItemTypeDef, _OptionalUtteranceLevelTestResultItemTypeDef
+class StartBotRecommendationRequestRequestTypeDef(
+    _RequiredStartBotRecommendationRequestRequestTypeDef,
+    _OptionalStartBotRecommendationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredTestSetTurnRecordTypeDef = TypedDict(
-    "_RequiredTestSetTurnRecordTypeDef",
+UtteranceLevelTestResultItemTypeDef = TypedDict(
+    "UtteranceLevelTestResultItemTypeDef",
     {
         "recordNumber": int,
-        "turnSpecification": TurnSpecificationTypeDef,
+        "conversationId": str,
+        "turnResult": TestSetTurnResultTypeDef,
     },
 )
-_OptionalTestSetTurnRecordTypeDef = TypedDict(
-    "_OptionalTestSetTurnRecordTypeDef",
+
+TestSetTurnRecordTypeDef = TypedDict(
+    "TestSetTurnRecordTypeDef",
     {
+        "recordNumber": int,
         "conversationId": str,
         "turnNumber": int,
+        "turnSpecification": TurnSpecificationTypeDef,
     },
-    total=False,
 )
 
-
-class TestSetTurnRecordTypeDef(
-    _RequiredTestSetTurnRecordTypeDef, _OptionalTestSetTurnRecordTypeDef
-):
-    pass
-
-
 ListSlotsResponseTypeDef = TypedDict(
     "ListSlotsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "slotSummaries": List[SlotSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConditionalSpecificationOutputTypeDef = TypedDict(
+    "ConditionalSpecificationOutputTypeDef",
+    {
+        "active": bool,
+        "conditionalBranches": List[ConditionalBranchOutputTypeDef],
+        "defaultBranch": DefaultConditionalBranchOutputTypeDef,
+    },
+)
+
+SubSlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "SubSlotValueElicitationSettingOutputTypeDef",
+    {
+        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
+        "promptSpecification": PromptSpecificationOutputTypeDef,
+        "sampleUtterances": List[SampleUtteranceOutputTypeDef],
+        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
+    },
+)
+
 ConditionalSpecificationTypeDef = TypedDict(
     "ConditionalSpecificationTypeDef",
     {
         "active": bool,
         "conditionalBranches": Sequence[ConditionalBranchTypeDef],
         "defaultBranch": DefaultConditionalBranchTypeDef,
     },
@@ -5145,14 +6587,62 @@
     {
         "testSetRecords": List[TestSetTurnRecordTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IntentClosingSettingOutputTypeDef = TypedDict(
+    "IntentClosingSettingOutputTypeDef",
+    {
+        "closingResponse": ResponseSpecificationOutputTypeDef,
+        "active": bool,
+        "nextStep": DialogStateOutputTypeDef,
+        "conditional": ConditionalSpecificationOutputTypeDef,
+    },
+)
+
+PostDialogCodeHookInvocationSpecificationOutputTypeDef = TypedDict(
+    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
+    {
+        "successResponse": ResponseSpecificationOutputTypeDef,
+        "successNextStep": DialogStateOutputTypeDef,
+        "successConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "timeoutResponse": ResponseSpecificationOutputTypeDef,
+        "timeoutNextStep": DialogStateOutputTypeDef,
+        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
+    },
+)
+
+PostFulfillmentStatusSpecificationOutputTypeDef = TypedDict(
+    "PostFulfillmentStatusSpecificationOutputTypeDef",
+    {
+        "successResponse": ResponseSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "timeoutResponse": ResponseSpecificationOutputTypeDef,
+        "successNextStep": DialogStateOutputTypeDef,
+        "successConditional": ConditionalSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "timeoutNextStep": DialogStateOutputTypeDef,
+        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
+    },
+)
+
+SpecificationsOutputTypeDef = TypedDict(
+    "SpecificationsOutputTypeDef",
+    {
+        "slotTypeId": str,
+        "valueElicitationSetting": SubSlotValueElicitationSettingOutputTypeDef,
+    },
+)
+
 IntentClosingSettingTypeDef = TypedDict(
     "IntentClosingSettingTypeDef",
     {
         "closingResponse": ResponseSpecificationTypeDef,
         "active": bool,
         "nextStep": DialogStateTypeDef,
         "conditional": ConditionalSpecificationTypeDef,
@@ -5205,15 +6695,42 @@
     {
         "overallTestResults": OverallTestResultsTypeDef,
         "conversationLevelTestResults": ConversationLevelTestResultsTypeDef,
         "intentClassificationTestResults": IntentClassificationTestResultsTypeDef,
         "intentLevelSlotResolutionTestResults": IntentLevelSlotResolutionTestResultsTypeDef,
         "utteranceLevelTestResults": UtteranceLevelTestResultsTypeDef,
     },
-    total=False,
+)
+
+DialogCodeHookInvocationSettingOutputTypeDef = TypedDict(
+    "DialogCodeHookInvocationSettingOutputTypeDef",
+    {
+        "enableCodeHookInvocation": bool,
+        "active": bool,
+        "invocationLabel": str,
+        "postCodeHookSpecification": PostDialogCodeHookInvocationSpecificationOutputTypeDef,
+    },
+)
+
+FulfillmentCodeHookSettingsOutputTypeDef = TypedDict(
+    "FulfillmentCodeHookSettingsOutputTypeDef",
+    {
+        "enabled": bool,
+        "postFulfillmentStatusSpecification": PostFulfillmentStatusSpecificationOutputTypeDef,
+        "fulfillmentUpdatesSpecification": FulfillmentUpdatesSpecificationOutputTypeDef,
+        "active": bool,
+    },
+)
+
+SubSlotSettingOutputTypeDef = TypedDict(
+    "SubSlotSettingOutputTypeDef",
+    {
+        "expression": str,
+        "slotSpecifications": Dict[str, SpecificationsOutputTypeDef],
+    },
 )
 
 _RequiredDialogCodeHookInvocationSettingTypeDef = TypedDict(
     "_RequiredDialogCodeHookInvocationSettingTypeDef",
     {
         "enableCodeHookInvocation": bool,
         "active": bool,
@@ -5272,14 +6789,57 @@
     {
         "testExecutionResults": TestExecutionResultItemsTypeDef,
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InitialResponseSettingOutputTypeDef = TypedDict(
+    "InitialResponseSettingOutputTypeDef",
+    {
+        "initialResponse": ResponseSpecificationOutputTypeDef,
+        "nextStep": DialogStateOutputTypeDef,
+        "conditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+    },
+)
+
+IntentConfirmationSettingOutputTypeDef = TypedDict(
+    "IntentConfirmationSettingOutputTypeDef",
+    {
+        "promptSpecification": PromptSpecificationOutputTypeDef,
+        "declinationResponse": ResponseSpecificationOutputTypeDef,
+        "active": bool,
+        "confirmationResponse": ResponseSpecificationOutputTypeDef,
+        "confirmationNextStep": DialogStateOutputTypeDef,
+        "confirmationConditional": ConditionalSpecificationOutputTypeDef,
+        "declinationNextStep": DialogStateOutputTypeDef,
+        "declinationConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+        "elicitationCodeHook": ElicitationCodeHookInvocationSettingOutputTypeDef,
+    },
+)
+
+SlotCaptureSettingOutputTypeDef = TypedDict(
+    "SlotCaptureSettingOutputTypeDef",
+    {
+        "captureResponse": ResponseSpecificationOutputTypeDef,
+        "captureNextStep": DialogStateOutputTypeDef,
+        "captureConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+        "elicitationCodeHook": ElicitationCodeHookInvocationSettingOutputTypeDef,
+    },
+)
+
 InitialResponseSettingTypeDef = TypedDict(
     "InitialResponseSettingTypeDef",
     {
         "initialResponse": ResponseSpecificationTypeDef,
         "nextStep": DialogStateTypeDef,
         "conditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
@@ -5330,160 +6890,172 @@
         "failureConditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
         "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIntentRequestRequestTypeDef",
+CreateIntentResponseTypeDef = TypedDict(
+    "CreateIntentResponseTypeDef",
     {
+        "intentId": str,
         "intentName": str,
+        "description": str,
+        "parentIntentSignature": str,
+        "sampleUtterances": List[SampleUtteranceOutputTypeDef],
+        "dialogCodeHook": DialogCodeHookSettingsOutputTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
+        "creationDateTime": datetime,
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIntentRequestRequestTypeDef",
-    {
-        "description": str,
-        "parentIntentSignature": str,
-        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
-        "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": Sequence[InputContextTypeDef],
-        "outputContexts": Sequence[OutputContextTypeDef],
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateIntentRequestRequestTypeDef(
-    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
-):
-    pass
-
 
-CreateIntentResponseTypeDef = TypedDict(
-    "CreateIntentResponseTypeDef",
+DescribeIntentResponseTypeDef = TypedDict(
+    "DescribeIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
-        "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
-        "kendraConfiguration": KendraConfigurationTypeDef,
+        "sampleUtterances": List[SampleUtteranceOutputTypeDef],
+        "dialogCodeHook": DialogCodeHookSettingsOutputTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "slotPriorities": List[SlotPriorityOutputTypeDef],
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
+        "lastUpdatedDateTime": datetime,
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeIntentResponseTypeDef = TypedDict(
-    "DescribeIntentResponseTypeDef",
+UpdateIntentResponseTypeDef = TypedDict(
+    "UpdateIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
-        "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": List[SlotPriorityTypeDef],
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
-        "kendraConfiguration": KendraConfigurationTypeDef,
+        "sampleUtterances": List[SampleUtteranceOutputTypeDef],
+        "dialogCodeHook": DialogCodeHookSettingsOutputTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "slotPriorities": List[SlotPriorityOutputTypeDef],
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateIntentRequestRequestTypeDef",
+SlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "SlotValueElicitationSettingOutputTypeDef",
+    {
+        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
+        "slotConstraint": SlotConstraintType,
+        "promptSpecification": PromptSpecificationOutputTypeDef,
+        "sampleUtterances": List[SampleUtteranceOutputTypeDef],
+        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
+        "slotCaptureSetting": SlotCaptureSettingOutputTypeDef,
+    },
+)
+
+_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIntentRequestRequestTypeDef",
     {
-        "intentId": str,
         "intentName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateIntentRequestRequestTypeDef",
+_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIntentRequestRequestTypeDef",
     {
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": Sequence[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "initialResponseSetting": InitialResponseSettingTypeDef,
     },
     total=False,
 )
 
 
-class UpdateIntentRequestRequestTypeDef(
-    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
+class CreateIntentRequestRequestTypeDef(
+    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
 ):
     pass
 
 
-UpdateIntentResponseTypeDef = TypedDict(
-    "UpdateIntentResponseTypeDef",
+_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIntentRequestRequestTypeDef",
     {
         "intentId": str,
         "intentName": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIntentRequestRequestTypeDef",
+    {
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
+        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": List[SlotPriorityTypeDef],
+        "slotPriorities": Sequence[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "inputContexts": Sequence[InputContextTypeDef],
+        "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+
+class UpdateIntentRequestRequestTypeDef(
+    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredSlotValueElicitationSettingTypeDef = TypedDict(
     "_RequiredSlotValueElicitationSettingTypeDef",
     {
         "slotConstraint": SlotConstraintType,
     },
 )
 _OptionalSlotValueElicitationSettingTypeDef = TypedDict(
@@ -5501,129 +7073,128 @@
 
 class SlotValueElicitationSettingTypeDef(
     _RequiredSlotValueElicitationSettingTypeDef, _OptionalSlotValueElicitationSettingTypeDef
 ):
     pass
 
 
-_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotRequestRequestTypeDef",
+CreateSlotResponseTypeDef = TypedDict(
+    "CreateSlotResponseTypeDef",
     {
+        "slotId": str,
         "slotName": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
+        "description": str,
+        "slotTypeId": str,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "obfuscationSetting": ObfuscationSettingOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
+        "creationDateTime": datetime,
+        "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotRequestRequestTypeDef",
-    {
-        "description": str,
-        "slotTypeId": str,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
-        "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateSlotRequestRequestTypeDef(
-    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
-):
-    pass
 
-
-CreateSlotResponseTypeDef = TypedDict(
-    "CreateSlotResponseTypeDef",
+DescribeSlotResponseTypeDef = TypedDict(
+    "DescribeSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "obfuscationSetting": ObfuscationSettingOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
-        "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
+        "lastUpdatedDateTime": datetime,
+        "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSlotResponseTypeDef = TypedDict(
-    "DescribeSlotResponseTypeDef",
+UpdateSlotResponseTypeDef = TypedDict(
+    "UpdateSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "obfuscationSetting": ObfuscationSettingOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
+        "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotRequestRequestTypeDef",
+_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotRequestRequestTypeDef",
     {
-        "slotId": str,
         "slotName": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
     },
 )
-_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotRequestRequestTypeDef",
+_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotRequestRequestTypeDef",
     {
         "description": str,
         "slotTypeId": str,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
     },
     total=False,
 )
 
 
-class UpdateSlotRequestRequestTypeDef(
-    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
+class CreateSlotRequestRequestTypeDef(
+    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
 ):
     pass
 
 
-UpdateSlotResponseTypeDef = TypedDict(
-    "UpdateSlotResponseTypeDef",
+_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "slotName": str,
-        "description": str,
-        "slotTypeId": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+    },
+)
+_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeId": str,
+        "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
+
+
+class UpdateSlotRequestRequestTypeDef(
+    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/type_defs.pyi` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -9,41 +9,65 @@
     from mypy_boto3_lexv2_models.type_defs import ActiveContextTypeDef
 
     data: ActiveContextTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregatedUtterancesFilterOperatorType,
     AggregatedUtterancesSortAttributeType,
+    AnalyticsBinByNameType,
+    AnalyticsCommonFilterNameType,
+    AnalyticsFilterOperatorType,
+    AnalyticsIntentFieldType,
+    AnalyticsIntentFilterNameType,
+    AnalyticsIntentMetricNameType,
+    AnalyticsIntentStageFieldType,
+    AnalyticsIntentStageFilterNameType,
+    AnalyticsIntentStageMetricNameType,
+    AnalyticsIntervalType,
+    AnalyticsMetricStatisticType,
+    AnalyticsModalityType,
+    AnalyticsNodeTypeType,
+    AnalyticsSessionFieldType,
+    AnalyticsSessionFilterNameType,
+    AnalyticsSessionMetricNameType,
+    AnalyticsSessionSortByNameType,
+    AnalyticsSortOrderType,
+    AnalyticsUtteranceFieldType,
+    AnalyticsUtteranceFilterNameType,
+    AnalyticsUtteranceMetricNameType,
     AssociatedTranscriptFilterNameType,
     BotAliasStatusType,
+    BotChannelTypeType,
     BotFilterNameType,
     BotFilterOperatorType,
     BotLocaleFilterOperatorType,
     BotLocaleStatusType,
     BotRecommendationStatusType,
     BotStatusType,
     BotTypeType,
+    ConversationEndStateType,
     ConversationLogsInputModeFilterType,
     CustomVocabularyStatusType,
     DialogActionTypeType,
     EffectType,
     ErrorCodeType,
     ExportFilterOperatorType,
     ExportStatusType,
     ImportExportFileFormatType,
     ImportFilterOperatorType,
     ImportResourceTypeType,
     ImportStatusType,
     IntentFilterOperatorType,
     IntentSortAttributeType,
+    IntentStateType,
     MergeStrategyType,
     MessageSelectionStrategyType,
     ObfuscationSettingTypeType,
     PromptAttemptType,
     SearchOrderType,
     SlotConstraintType,
     SlotFilterOperatorType,
@@ -63,97 +87,155 @@
     TestResultTypeFilterType,
     TestSetDiscrepancyReportStatusType,
     TestSetGenerationStatusType,
     TestSetModalityType,
     TestSetSortAttributeType,
     TestSetStatusType,
     TimeDimensionType,
+    UtteranceContentTypeType,
     VoiceEngineType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActiveContextTypeDef",
+    "AdvancedRecognitionSettingOutputTypeDef",
     "AdvancedRecognitionSettingTypeDef",
     "ExecutionErrorDetailsTypeDef",
     "AgentTurnSpecificationTypeDef",
     "AggregatedUtterancesFilterTypeDef",
     "AggregatedUtterancesSortByTypeDef",
     "AggregatedUtterancesSummaryTypeDef",
+    "AllowedInputTypesOutputTypeDef",
     "AllowedInputTypesTypeDef",
+    "AnalyticsBinBySpecificationTypeDef",
+    "AnalyticsBinKeyTypeDef",
+    "AnalyticsIntentFilterTypeDef",
+    "AnalyticsIntentGroupByKeyTypeDef",
+    "AnalyticsIntentGroupBySpecificationTypeDef",
+    "AnalyticsIntentMetricResultTypeDef",
+    "AnalyticsIntentMetricTypeDef",
+    "AnalyticsIntentNodeSummaryTypeDef",
+    "AnalyticsIntentStageFilterTypeDef",
+    "AnalyticsIntentStageGroupByKeyTypeDef",
+    "AnalyticsIntentStageGroupBySpecificationTypeDef",
+    "AnalyticsIntentStageMetricResultTypeDef",
+    "AnalyticsIntentStageMetricTypeDef",
+    "AnalyticsPathFilterTypeDef",
+    "AnalyticsSessionFilterTypeDef",
+    "AnalyticsSessionGroupByKeyTypeDef",
+    "AnalyticsSessionGroupBySpecificationTypeDef",
+    "AnalyticsSessionMetricResultTypeDef",
+    "AnalyticsSessionMetricTypeDef",
+    "AnalyticsUtteranceAttributeResultTypeDef",
+    "AnalyticsUtteranceAttributeTypeDef",
+    "AnalyticsUtteranceFilterTypeDef",
+    "AnalyticsUtteranceGroupByKeyTypeDef",
+    "AnalyticsUtteranceGroupBySpecificationTypeDef",
+    "AnalyticsUtteranceMetricResultTypeDef",
+    "AnalyticsUtteranceMetricTypeDef",
     "AssociatedTranscriptFilterTypeDef",
     "AssociatedTranscriptTypeDef",
+    "AudioSpecificationOutputTypeDef",
+    "DTMFSpecificationOutputTypeDef",
     "AudioSpecificationTypeDef",
     "DTMFSpecificationTypeDef",
+    "S3BucketLogDestinationOutputTypeDef",
     "S3BucketLogDestinationTypeDef",
     "NewCustomVocabularyItemTypeDef",
-    "CustomVocabularyItemTypeDef",
+    "CustomVocabularyItemOutputTypeDef",
     "FailedCustomVocabularyItemTypeDef",
     "CustomVocabularyEntryIdTypeDef",
+    "CustomVocabularyItemTypeDef",
     "BotAliasHistoryEventTypeDef",
     "BotAliasSummaryTypeDef",
+    "BotAliasTestExecutionTargetOutputTypeDef",
     "BotAliasTestExecutionTargetTypeDef",
+    "BotExportSpecificationOutputTypeDef",
     "BotExportSpecificationTypeDef",
     "BotFilterTypeDef",
+    "DataPrivacyOutputTypeDef",
     "DataPrivacyTypeDef",
+    "BotLocaleExportSpecificationOutputTypeDef",
     "BotLocaleExportSpecificationTypeDef",
     "BotLocaleFilterTypeDef",
     "BotLocaleHistoryEventTypeDef",
+    "VoiceSettingsOutputTypeDef",
     "VoiceSettingsTypeDef",
     "BotLocaleSortByTypeDef",
     "BotLocaleSummaryTypeDef",
+    "BotMemberOutputTypeDef",
     "BotMemberTypeDef",
     "IntentStatisticsTypeDef",
     "SlotTypeStatisticsTypeDef",
     "BotRecommendationSummaryTypeDef",
     "BotSortByTypeDef",
     "BotSummaryTypeDef",
+    "BotVersionLocaleDetailsOutputTypeDef",
     "BotVersionLocaleDetailsTypeDef",
     "BotVersionSortByTypeDef",
     "BotVersionSummaryTypeDef",
     "BuildBotLocaleRequestRequestTypeDef",
     "BuildBotLocaleResponseTypeDef",
     "BuiltInIntentSortByTypeDef",
     "BuiltInIntentSummaryTypeDef",
     "BuiltInSlotTypeSortByTypeDef",
     "BuiltInSlotTypeSummaryTypeDef",
+    "ButtonOutputTypeDef",
     "ButtonTypeDef",
+    "CloudWatchLogGroupLogDestinationOutputTypeDef",
     "CloudWatchLogGroupLogDestinationTypeDef",
+    "LambdaCodeHookOutputTypeDef",
     "LambdaCodeHookTypeDef",
+    "SubSlotTypeCompositionOutputTypeDef",
     "SubSlotTypeCompositionTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "ConversationLevelIntentClassificationResultItemTypeDef",
     "ConversationLevelResultDetailTypeDef",
     "ConversationLevelSlotResolutionResultItemTypeDef",
     "ConversationLevelTestResultsFilterByTypeDef",
+    "ConversationLogsDataSourceFilterByOutputTypeDef",
     "ConversationLogsDataSourceFilterByTypeDef",
     "SentimentAnalysisSettingsTypeDef",
+    "SentimentAnalysisSettingsOutputTypeDef",
     "DialogCodeHookSettingsTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "SampleUtteranceTypeDef",
+    "DialogCodeHookSettingsOutputTypeDef",
+    "InputContextOutputTypeDef",
+    "KendraConfigurationOutputTypeDef",
+    "OutputContextOutputTypeDef",
+    "SampleUtteranceOutputTypeDef",
     "CreateResourcePolicyRequestRequestTypeDef",
     "CreateResourcePolicyResponseTypeDef",
     "PrincipalTypeDef",
     "CreateResourcePolicyStatementResponseTypeDef",
     "MultipleValuesSettingTypeDef",
     "ObfuscationSettingTypeDef",
+    "MultipleValuesSettingOutputTypeDef",
+    "ObfuscationSettingOutputTypeDef",
     "CreateUploadUrlResponseTypeDef",
+    "CustomPayloadOutputTypeDef",
     "CustomPayloadTypeDef",
+    "CustomVocabularyExportSpecificationOutputTypeDef",
     "CustomVocabularyExportSpecificationTypeDef",
+    "CustomVocabularyImportSpecificationOutputTypeDef",
     "CustomVocabularyImportSpecificationTypeDef",
+    "DateRangeFilterOutputTypeDef",
     "DateRangeFilterTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotAliasResponseTypeDef",
     "DeleteBotLocaleRequestRequestTypeDef",
     "DeleteBotLocaleResponseTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotResponseTypeDef",
@@ -175,294 +257,400 @@
     "DeleteTestSetRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeBotAliasRequestRequestTypeDef",
     "ParentBotNetworkTypeDef",
     "DescribeBotLocaleRequestRequestTypeDef",
     "DescribeBotRecommendationRequestRequestTypeDef",
-    "EncryptionSettingTypeDef",
+    "EncryptionSettingOutputTypeDef",
     "DescribeBotRequestRequestTypeDef",
     "DescribeBotVersionRequestRequestTypeDef",
     "DescribeCustomVocabularyMetadataRequestRequestTypeDef",
     "DescribeCustomVocabularyMetadataResponseTypeDef",
     "DescribeExportRequestRequestTypeDef",
     "DescribeImportRequestRequestTypeDef",
     "DescribeIntentRequestRequestTypeDef",
-    "SlotPriorityTypeDef",
+    "SlotPriorityOutputTypeDef",
     "DescribeResourcePolicyRequestRequestTypeDef",
     "DescribeResourcePolicyResponseTypeDef",
     "DescribeSlotRequestRequestTypeDef",
     "DescribeSlotTypeRequestRequestTypeDef",
     "DescribeTestExecutionRequestRequestTypeDef",
     "DescribeTestSetDiscrepancyReportRequestRequestTypeDef",
     "DescribeTestSetGenerationRequestRequestTypeDef",
-    "TestSetStorageLocationTypeDef",
+    "TestSetStorageLocationOutputTypeDef",
     "DescribeTestSetRequestRequestTypeDef",
+    "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
+    "IntentOverrideOutputTypeDef",
     "IntentOverrideTypeDef",
+    "ElicitationCodeHookInvocationSettingOutputTypeDef",
     "ElicitationCodeHookInvocationSettingTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionSettingTypeDef",
     "ExportFilterTypeDef",
+    "TestSetExportSpecificationOutputTypeDef",
     "TestSetExportSpecificationTypeDef",
     "ExportSortByTypeDef",
     "GetTestExecutionArtifactsUrlRequestRequestTypeDef",
     "GetTestExecutionArtifactsUrlResponseTypeDef",
+    "GrammarSlotTypeSourceOutputTypeDef",
     "GrammarSlotTypeSourceTypeDef",
     "ImportFilterTypeDef",
     "ImportSortByTypeDef",
     "ImportSummaryTypeDef",
     "RuntimeHintsTypeDef",
     "IntentClassificationTestResultItemCountsTypeDef",
     "IntentFilterTypeDef",
     "IntentSortByTypeDef",
+    "InvokedIntentSampleTypeDef",
     "ListBotAliasesRequestRequestTypeDef",
     "ListBotRecommendationsRequestRequestTypeDef",
     "ListCustomVocabularyItemsRequestRequestTypeDef",
     "ListRecommendedIntentsRequestRequestTypeDef",
     "RecommendedIntentSummaryTypeDef",
+    "SessionDataSortByTypeDef",
     "SlotTypeFilterTypeDef",
     "SlotTypeSortByTypeDef",
     "SlotTypeSummaryTypeDef",
     "SlotFilterTypeDef",
     "SlotSortByTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TestExecutionSortByTypeDef",
     "ListTestSetRecordsRequestRequestTypeDef",
     "TestSetSortByTypeDef",
+    "UtteranceDataSortByTypeDef",
+    "PlainTextMessageOutputTypeDef",
+    "SSMLMessageOutputTypeDef",
     "PlainTextMessageTypeDef",
     "SSMLMessageTypeDef",
     "OverallTestResultItemTypeDef",
+    "PathFormatOutputTypeDef",
     "PathFormatTypeDef",
+    "TextInputSpecificationOutputTypeDef",
     "TextInputSpecificationTypeDef",
+    "RelativeAggregationDurationOutputTypeDef",
     "RelativeAggregationDurationTypeDef",
     "ResponseMetadataTypeDef",
     "RuntimeHintValueTypeDef",
+    "SampleValueOutputTypeDef",
     "SampleValueTypeDef",
+    "SlotDefaultValueOutputTypeDef",
     "SlotDefaultValueTypeDef",
+    "SlotPriorityTypeDef",
     "SlotResolutionTestResultItemCountsTypeDef",
+    "SlotValueOutputTypeDef",
     "SlotValueTypeDef",
+    "SlotValueRegexFilterOutputTypeDef",
     "SlotValueRegexFilterTypeDef",
+    "TestSetStorageLocationTypeDef",
     "StopBotRecommendationRequestRequestTypeDef",
     "StopBotRecommendationResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSetIntentDiscrepancyItemTypeDef",
     "TestSetSlotDiscrepancyItemTypeDef",
+    "TestSetDiscrepancyReportBotAliasTargetOutputTypeDef",
     "TestSetDiscrepancyReportBotAliasTargetTypeDef",
+    "TestSetImportInputLocationOutputTypeDef",
     "TestSetImportInputLocationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateExportRequestRequestTypeDef",
     "UpdateResourcePolicyRequestRequestTypeDef",
     "UpdateResourcePolicyResponseTypeDef",
     "UpdateTestSetRequestRequestTypeDef",
     "UserTurnIntentOutputTypeDef",
     "UserTurnSlotOutputTypeDef",
     "UtteranceAudioInputSpecificationTypeDef",
     "AgentTurnResultTypeDef",
+    "AnalyticsIntentResultTypeDef",
+    "ListIntentMetricsRequestRequestTypeDef",
+    "ListIntentPathsResponseTypeDef",
+    "AnalyticsIntentStageResultTypeDef",
+    "ListIntentStageMetricsRequestRequestTypeDef",
+    "ListIntentPathsRequestRequestTypeDef",
+    "AnalyticsSessionResultTypeDef",
+    "ListSessionMetricsRequestRequestTypeDef",
+    "AnalyticsUtteranceResultTypeDef",
+    "ListUtteranceMetricsRequestRequestTypeDef",
     "SearchAssociatedTranscriptsRequestRequestTypeDef",
     "SearchAssociatedTranscriptsResponseTypeDef",
+    "AudioAndDTMFInputSpecificationOutputTypeDef",
     "AudioAndDTMFInputSpecificationTypeDef",
+    "AudioLogDestinationOutputTypeDef",
     "AudioLogDestinationTypeDef",
     "BatchCreateCustomVocabularyItemRequestRequestTypeDef",
-    "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
     "ListCustomVocabularyItemsResponseTypeDef",
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
+    "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
     "ListBotAliasesResponseTypeDef",
+    "TestExecutionTargetOutputTypeDef",
     "TestExecutionTargetTypeDef",
+    "BotImportSpecificationOutputTypeDef",
     "BotImportSpecificationTypeDef",
-    "BotLocaleImportSpecificationTypeDef",
-    "CreateBotLocaleRequestRequestTypeDef",
+    "BotLocaleImportSpecificationOutputTypeDef",
     "CreateBotLocaleResponseTypeDef",
     "DescribeBotLocaleResponseTypeDef",
-    "UpdateBotLocaleRequestRequestTypeDef",
     "UpdateBotLocaleResponseTypeDef",
+    "BotLocaleImportSpecificationTypeDef",
+    "CreateBotLocaleRequestRequestTypeDef",
+    "UpdateBotLocaleRequestRequestTypeDef",
     "ListBotLocalesRequestRequestTypeDef",
     "ListBotLocalesResponseTypeDef",
-    "CreateBotRequestRequestTypeDef",
     "CreateBotResponseTypeDef",
     "DescribeBotResponseTypeDef",
-    "UpdateBotRequestRequestTypeDef",
     "UpdateBotResponseTypeDef",
+    "CreateBotRequestRequestTypeDef",
+    "UpdateBotRequestRequestTypeDef",
     "BotRecommendationResultStatisticsTypeDef",
     "ListBotRecommendationsResponseTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListBotsResponseTypeDef",
-    "CreateBotVersionRequestRequestTypeDef",
     "CreateBotVersionResponseTypeDef",
+    "CreateBotVersionRequestRequestTypeDef",
     "ListBotVersionsRequestRequestTypeDef",
     "ListBotVersionsResponseTypeDef",
     "ListBuiltInIntentsRequestRequestTypeDef",
     "ListBuiltInIntentsResponseTypeDef",
     "ListBuiltInSlotTypesRequestRequestTypeDef",
     "ListBuiltInSlotTypesResponseTypeDef",
+    "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
+    "TextLogDestinationOutputTypeDef",
     "TextLogDestinationTypeDef",
+    "CodeHookSpecificationOutputTypeDef",
     "CodeHookSpecificationTypeDef",
+    "CompositeSlotTypeSettingOutputTypeDef",
     "CompositeSlotTypeSettingTypeDef",
     "ConversationLevelTestResultItemTypeDef",
     "TestExecutionResultFilterByTypeDef",
+    "ConversationLogsDataSourceOutputTypeDef",
     "ConversationLogsDataSourceTypeDef",
     "IntentSummaryTypeDef",
     "CreateResourcePolicyStatementRequestRequestTypeDef",
+    "LexTranscriptFilterOutputTypeDef",
     "LexTranscriptFilterTypeDef",
     "DescribeBotAliasRequestBotAliasAvailableWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleBuiltWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleCreatedWaitTypeDef",
     "DescribeBotLocaleRequestBotLocaleExpressTestingAvailableWaitTypeDef",
     "DescribeBotRequestBotAvailableWaitTypeDef",
     "DescribeBotVersionRequestBotVersionAvailableWaitTypeDef",
     "DescribeExportRequestBotExportCompletedWaitTypeDef",
     "DescribeImportRequestBotImportCompletedWaitTypeDef",
     "DescribeBotVersionResponseTypeDef",
-    "UpdateBotRecommendationRequestRequestTypeDef",
     "DescribeTestSetResponseTypeDef",
     "TestSetSummaryTypeDef",
     "UpdateTestSetResponseTypeDef",
+    "DialogStateOutputTypeDef",
     "DialogStateTypeDef",
+    "UpdateBotRecommendationRequestRequestTypeDef",
+    "ExportResourceSpecificationOutputTypeDef",
     "ExportResourceSpecificationTypeDef",
     "ListExportsRequestRequestTypeDef",
+    "GrammarSlotTypeSettingOutputTypeDef",
     "GrammarSlotTypeSettingTypeDef",
     "ListImportsRequestRequestTypeDef",
     "ListImportsResponseTypeDef",
     "InputSessionStateSpecificationTypeDef",
     "IntentClassificationTestResultItemTypeDef",
     "ListIntentsRequestRequestTypeDef",
+    "SessionSpecificationTypeDef",
     "ListRecommendedIntentsResponseTypeDef",
+    "ListSessionAnalyticsDataRequestRequestTypeDef",
     "ListSlotTypesRequestRequestTypeDef",
     "ListSlotTypesResponseTypeDef",
     "ListSlotsRequestRequestTypeDef",
     "ListTestExecutionsRequestRequestTypeDef",
     "ListTestSetsRequestRequestTypeDef",
+    "ListUtteranceAnalyticsDataRequestRequestTypeDef",
     "OverallTestResultsTypeDef",
+    "UtteranceAggregationDurationOutputTypeDef",
     "UtteranceAggregationDurationTypeDef",
     "RuntimeHintDetailsTypeDef",
+    "SlotTypeValueOutputTypeDef",
     "SlotTypeValueTypeDef",
+    "SlotDefaultValueSpecificationOutputTypeDef",
     "SlotDefaultValueSpecificationTypeDef",
     "SlotResolutionTestResultItemTypeDef",
+    "SlotValueOverrideOutputTypeDef",
     "SlotValueOverrideTypeDef",
+    "SlotValueSelectionSettingOutputTypeDef",
     "SlotValueSelectionSettingTypeDef",
     "TestSetDiscrepancyErrorsTypeDef",
+    "TestSetDiscrepancyReportResourceTargetOutputTypeDef",
     "TestSetDiscrepancyReportResourceTargetTypeDef",
+    "TestSetImportResourceSpecificationOutputTypeDef",
     "TestSetImportResourceSpecificationTypeDef",
     "UserTurnOutputSpecificationTypeDef",
     "UtteranceInputSpecificationTypeDef",
+    "ListIntentMetricsResponseTypeDef",
+    "ListIntentStageMetricsResponseTypeDef",
+    "ListSessionMetricsResponseTypeDef",
+    "ListUtteranceMetricsResponseTypeDef",
+    "PromptAttemptSpecificationOutputTypeDef",
     "PromptAttemptSpecificationTypeDef",
+    "AudioLogSettingOutputTypeDef",
     "AudioLogSettingTypeDef",
     "DescribeTestExecutionResponseTypeDef",
-    "StartTestExecutionRequestRequestTypeDef",
     "StartTestExecutionResponseTypeDef",
     "TestExecutionSummaryTypeDef",
+    "StartTestExecutionRequestRequestTypeDef",
     "BotRecommendationResultsTypeDef",
+    "MessageOutputTypeDef",
+    "UtteranceBotResponseTypeDef",
     "MessageTypeDef",
+    "TextLogSettingOutputTypeDef",
     "TextLogSettingTypeDef",
+    "BotAliasLocaleSettingsOutputTypeDef",
     "BotAliasLocaleSettingsTypeDef",
     "ConversationLevelTestResultsTypeDef",
     "ListTestExecutionResultItemsRequestRequestTypeDef",
+    "TestSetGenerationDataSourceOutputTypeDef",
     "TestSetGenerationDataSourceTypeDef",
     "ListIntentsResponseTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListTestSetsResponseTypeDef",
-    "CreateExportRequestRequestTypeDef",
     "CreateExportResponseTypeDef",
     "DescribeExportResponseTypeDef",
     "ExportSummaryTypeDef",
     "UpdateExportResponseTypeDef",
+    "CreateExportRequestRequestTypeDef",
+    "ExternalSourceSettingOutputTypeDef",
     "ExternalSourceSettingTypeDef",
     "IntentClassificationTestResultsTypeDef",
-    "ListAggregatedUtterancesRequestRequestTypeDef",
+    "ListSessionAnalyticsDataResponseTypeDef",
     "ListAggregatedUtterancesResponseTypeDef",
+    "ListAggregatedUtterancesRequestRequestTypeDef",
     "IntentLevelSlotResolutionTestResultItemTypeDef",
-    "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
+    "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
+    "ImportResourceSpecificationOutputTypeDef",
     "ImportResourceSpecificationTypeDef",
     "UserTurnInputSpecificationTypeDef",
     "ListTestExecutionsResponseTypeDef",
+    "MessageGroupOutputTypeDef",
+    "UtteranceSpecificationTypeDef",
     "MessageGroupTypeDef",
+    "ConversationLogSettingsOutputTypeDef",
     "ConversationLogSettingsTypeDef",
     "DescribeTestSetGenerationResponseTypeDef",
-    "StartTestSetGenerationRequestRequestTypeDef",
     "StartTestSetGenerationResponseTypeDef",
+    "StartTestSetGenerationRequestRequestTypeDef",
+    "S3BucketTranscriptSourceOutputTypeDef",
     "S3BucketTranscriptSourceTypeDef",
     "ListExportsResponseTypeDef",
-    "CreateSlotTypeRequestRequestTypeDef",
     "CreateSlotTypeResponseTypeDef",
     "DescribeSlotTypeResponseTypeDef",
-    "UpdateSlotTypeRequestRequestTypeDef",
     "UpdateSlotTypeResponseTypeDef",
+    "CreateSlotTypeRequestRequestTypeDef",
+    "UpdateSlotTypeRequestRequestTypeDef",
     "IntentLevelSlotResolutionTestResultsTypeDef",
     "DescribeImportResponseTypeDef",
-    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
+    "StartImportRequestRequestTypeDef",
     "UserTurnResultTypeDef",
     "UserTurnSpecificationTypeDef",
+    "FulfillmentStartResponseSpecificationOutputTypeDef",
+    "FulfillmentUpdateResponseSpecificationOutputTypeDef",
+    "PromptSpecificationOutputTypeDef",
+    "ResponseSpecificationOutputTypeDef",
+    "StillWaitingResponseSpecificationOutputTypeDef",
+    "ListUtteranceAnalyticsDataResponseTypeDef",
     "FulfillmentStartResponseSpecificationTypeDef",
     "FulfillmentUpdateResponseSpecificationTypeDef",
     "PromptSpecificationTypeDef",
     "ResponseSpecificationTypeDef",
     "StillWaitingResponseSpecificationTypeDef",
-    "CreateBotAliasRequestRequestTypeDef",
     "CreateBotAliasResponseTypeDef",
     "DescribeBotAliasResponseTypeDef",
-    "UpdateBotAliasRequestRequestTypeDef",
     "UpdateBotAliasResponseTypeDef",
+    "CreateBotAliasRequestRequestTypeDef",
+    "UpdateBotAliasRequestRequestTypeDef",
+    "TranscriptSourceSettingOutputTypeDef",
     "TranscriptSourceSettingTypeDef",
     "TestSetTurnResultTypeDef",
     "TurnSpecificationTypeDef",
-    "FulfillmentUpdatesSpecificationTypeDef",
+    "FulfillmentUpdatesSpecificationOutputTypeDef",
     "SlotSummaryTypeDef",
+    "ConditionalBranchOutputTypeDef",
+    "DefaultConditionalBranchOutputTypeDef",
+    "WaitAndContinueSpecificationOutputTypeDef",
+    "FulfillmentUpdatesSpecificationTypeDef",
     "ConditionalBranchTypeDef",
     "DefaultConditionalBranchTypeDef",
     "WaitAndContinueSpecificationTypeDef",
     "DescribeBotRecommendationResponseTypeDef",
-    "StartBotRecommendationRequestRequestTypeDef",
     "StartBotRecommendationResponseTypeDef",
     "UpdateBotRecommendationResponseTypeDef",
+    "StartBotRecommendationRequestRequestTypeDef",
     "UtteranceLevelTestResultItemTypeDef",
     "TestSetTurnRecordTypeDef",
     "ListSlotsResponseTypeDef",
+    "ConditionalSpecificationOutputTypeDef",
+    "SubSlotValueElicitationSettingOutputTypeDef",
     "ConditionalSpecificationTypeDef",
     "SubSlotValueElicitationSettingTypeDef",
     "UtteranceLevelTestResultsTypeDef",
     "ListTestSetRecordsResponseTypeDef",
+    "IntentClosingSettingOutputTypeDef",
+    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
+    "PostFulfillmentStatusSpecificationOutputTypeDef",
+    "SpecificationsOutputTypeDef",
     "IntentClosingSettingTypeDef",
     "PostDialogCodeHookInvocationSpecificationTypeDef",
     "PostFulfillmentStatusSpecificationTypeDef",
     "SpecificationsTypeDef",
     "TestExecutionResultItemsTypeDef",
+    "DialogCodeHookInvocationSettingOutputTypeDef",
+    "FulfillmentCodeHookSettingsOutputTypeDef",
+    "SubSlotSettingOutputTypeDef",
     "DialogCodeHookInvocationSettingTypeDef",
     "FulfillmentCodeHookSettingsTypeDef",
     "SubSlotSettingTypeDef",
     "ListTestExecutionResultItemsResponseTypeDef",
+    "InitialResponseSettingOutputTypeDef",
+    "IntentConfirmationSettingOutputTypeDef",
+    "SlotCaptureSettingOutputTypeDef",
     "InitialResponseSettingTypeDef",
     "IntentConfirmationSettingTypeDef",
     "SlotCaptureSettingTypeDef",
-    "CreateIntentRequestRequestTypeDef",
     "CreateIntentResponseTypeDef",
     "DescribeIntentResponseTypeDef",
-    "UpdateIntentRequestRequestTypeDef",
     "UpdateIntentResponseTypeDef",
+    "SlotValueElicitationSettingOutputTypeDef",
+    "CreateIntentRequestRequestTypeDef",
+    "UpdateIntentRequestRequestTypeDef",
     "SlotValueElicitationSettingTypeDef",
-    "CreateSlotRequestRequestTypeDef",
     "CreateSlotResponseTypeDef",
     "DescribeSlotResponseTypeDef",
-    "UpdateSlotRequestRequestTypeDef",
     "UpdateSlotResponseTypeDef",
+    "CreateSlotRequestRequestTypeDef",
+    "UpdateSlotRequestRequestTypeDef",
 )
 
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
     },
 )
 
+AdvancedRecognitionSettingOutputTypeDef = TypedDict(
+    "AdvancedRecognitionSettingOutputTypeDef",
+    {
+        "audioRecognitionStrategy": Literal["UseSlotValuesAsCustomVocabulary"],
+    },
+)
+
 AdvancedRecognitionSettingTypeDef = TypedDict(
     "AdvancedRecognitionSettingTypeDef",
     {
         "audioRecognitionStrategy": Literal["UseSlotValuesAsCustomVocabulary"],
     },
     total=False,
 )
@@ -505,39 +693,337 @@
         "utterance": str,
         "hitCount": int,
         "missedCount": int,
         "utteranceFirstRecordedInAggregationDuration": datetime,
         "utteranceLastRecordedInAggregationDuration": datetime,
         "containsDataFromDeletedResources": bool,
     },
-    total=False,
+)
+
+AllowedInputTypesOutputTypeDef = TypedDict(
+    "AllowedInputTypesOutputTypeDef",
+    {
+        "allowAudioInput": bool,
+        "allowDTMFInput": bool,
+    },
 )
 
 AllowedInputTypesTypeDef = TypedDict(
     "AllowedInputTypesTypeDef",
     {
         "allowAudioInput": bool,
         "allowDTMFInput": bool,
     },
 )
 
+_RequiredAnalyticsBinBySpecificationTypeDef = TypedDict(
+    "_RequiredAnalyticsBinBySpecificationTypeDef",
+    {
+        "name": AnalyticsBinByNameType,
+        "interval": AnalyticsIntervalType,
+    },
+)
+_OptionalAnalyticsBinBySpecificationTypeDef = TypedDict(
+    "_OptionalAnalyticsBinBySpecificationTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+class AnalyticsBinBySpecificationTypeDef(
+    _RequiredAnalyticsBinBySpecificationTypeDef, _OptionalAnalyticsBinBySpecificationTypeDef
+):
+    pass
+
+AnalyticsBinKeyTypeDef = TypedDict(
+    "AnalyticsBinKeyTypeDef",
+    {
+        "name": AnalyticsBinByNameType,
+        "value": int,
+    },
+)
+
+AnalyticsIntentFilterTypeDef = TypedDict(
+    "AnalyticsIntentFilterTypeDef",
+    {
+        "name": AnalyticsIntentFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsIntentGroupByKeyTypeDef = TypedDict(
+    "AnalyticsIntentGroupByKeyTypeDef",
+    {
+        "name": AnalyticsIntentFieldType,
+        "value": str,
+    },
+)
+
+AnalyticsIntentGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsIntentGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsIntentFieldType,
+    },
+)
+
+AnalyticsIntentMetricResultTypeDef = TypedDict(
+    "AnalyticsIntentMetricResultTypeDef",
+    {
+        "name": AnalyticsIntentMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+)
+
+_RequiredAnalyticsIntentMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsIntentMetricTypeDef",
+    {
+        "name": AnalyticsIntentMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsIntentMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsIntentMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+class AnalyticsIntentMetricTypeDef(
+    _RequiredAnalyticsIntentMetricTypeDef, _OptionalAnalyticsIntentMetricTypeDef
+):
+    pass
+
+AnalyticsIntentNodeSummaryTypeDef = TypedDict(
+    "AnalyticsIntentNodeSummaryTypeDef",
+    {
+        "intentName": str,
+        "intentPath": str,
+        "intentCount": int,
+        "intentLevel": int,
+        "nodeType": AnalyticsNodeTypeType,
+    },
+)
+
+AnalyticsIntentStageFilterTypeDef = TypedDict(
+    "AnalyticsIntentStageFilterTypeDef",
+    {
+        "name": AnalyticsIntentStageFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsIntentStageGroupByKeyTypeDef = TypedDict(
+    "AnalyticsIntentStageGroupByKeyTypeDef",
+    {
+        "name": AnalyticsIntentStageFieldType,
+        "value": str,
+    },
+)
+
+AnalyticsIntentStageGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsIntentStageGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsIntentStageFieldType,
+    },
+)
+
+AnalyticsIntentStageMetricResultTypeDef = TypedDict(
+    "AnalyticsIntentStageMetricResultTypeDef",
+    {
+        "name": AnalyticsIntentStageMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+)
+
+_RequiredAnalyticsIntentStageMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsIntentStageMetricTypeDef",
+    {
+        "name": AnalyticsIntentStageMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsIntentStageMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsIntentStageMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+class AnalyticsIntentStageMetricTypeDef(
+    _RequiredAnalyticsIntentStageMetricTypeDef, _OptionalAnalyticsIntentStageMetricTypeDef
+):
+    pass
+
+AnalyticsPathFilterTypeDef = TypedDict(
+    "AnalyticsPathFilterTypeDef",
+    {
+        "name": AnalyticsCommonFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsSessionFilterTypeDef = TypedDict(
+    "AnalyticsSessionFilterTypeDef",
+    {
+        "name": AnalyticsSessionFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsSessionGroupByKeyTypeDef = TypedDict(
+    "AnalyticsSessionGroupByKeyTypeDef",
+    {
+        "name": AnalyticsSessionFieldType,
+        "value": str,
+    },
+)
+
+AnalyticsSessionGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsSessionGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsSessionFieldType,
+    },
+)
+
+AnalyticsSessionMetricResultTypeDef = TypedDict(
+    "AnalyticsSessionMetricResultTypeDef",
+    {
+        "name": AnalyticsSessionMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+)
+
+_RequiredAnalyticsSessionMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsSessionMetricTypeDef",
+    {
+        "name": AnalyticsSessionMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsSessionMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsSessionMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+class AnalyticsSessionMetricTypeDef(
+    _RequiredAnalyticsSessionMetricTypeDef, _OptionalAnalyticsSessionMetricTypeDef
+):
+    pass
+
+AnalyticsUtteranceAttributeResultTypeDef = TypedDict(
+    "AnalyticsUtteranceAttributeResultTypeDef",
+    {
+        "lastUsedIntent": str,
+    },
+)
+
+AnalyticsUtteranceAttributeTypeDef = TypedDict(
+    "AnalyticsUtteranceAttributeTypeDef",
+    {
+        "name": Literal["LastUsedIntent"],
+    },
+)
+
+AnalyticsUtteranceFilterTypeDef = TypedDict(
+    "AnalyticsUtteranceFilterTypeDef",
+    {
+        "name": AnalyticsUtteranceFilterNameType,
+        "operator": AnalyticsFilterOperatorType,
+        "values": Sequence[str],
+    },
+)
+
+AnalyticsUtteranceGroupByKeyTypeDef = TypedDict(
+    "AnalyticsUtteranceGroupByKeyTypeDef",
+    {
+        "name": AnalyticsUtteranceFieldType,
+        "value": str,
+    },
+)
+
+AnalyticsUtteranceGroupBySpecificationTypeDef = TypedDict(
+    "AnalyticsUtteranceGroupBySpecificationTypeDef",
+    {
+        "name": AnalyticsUtteranceFieldType,
+    },
+)
+
+AnalyticsUtteranceMetricResultTypeDef = TypedDict(
+    "AnalyticsUtteranceMetricResultTypeDef",
+    {
+        "name": AnalyticsUtteranceMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+        "value": float,
+    },
+)
+
+_RequiredAnalyticsUtteranceMetricTypeDef = TypedDict(
+    "_RequiredAnalyticsUtteranceMetricTypeDef",
+    {
+        "name": AnalyticsUtteranceMetricNameType,
+        "statistic": AnalyticsMetricStatisticType,
+    },
+)
+_OptionalAnalyticsUtteranceMetricTypeDef = TypedDict(
+    "_OptionalAnalyticsUtteranceMetricTypeDef",
+    {
+        "order": AnalyticsSortOrderType,
+    },
+    total=False,
+)
+
+class AnalyticsUtteranceMetricTypeDef(
+    _RequiredAnalyticsUtteranceMetricTypeDef, _OptionalAnalyticsUtteranceMetricTypeDef
+):
+    pass
+
 AssociatedTranscriptFilterTypeDef = TypedDict(
     "AssociatedTranscriptFilterTypeDef",
     {
         "name": AssociatedTranscriptFilterNameType,
         "values": Sequence[str],
     },
 )
 
 AssociatedTranscriptTypeDef = TypedDict(
     "AssociatedTranscriptTypeDef",
     {
         "transcript": str,
     },
-    total=False,
+)
+
+AudioSpecificationOutputTypeDef = TypedDict(
+    "AudioSpecificationOutputTypeDef",
+    {
+        "maxLengthMs": int,
+        "endTimeoutMs": int,
+    },
+)
+
+DTMFSpecificationOutputTypeDef = TypedDict(
+    "DTMFSpecificationOutputTypeDef",
+    {
+        "maxLength": int,
+        "endTimeoutMs": int,
+        "deletionCharacter": str,
+        "endCharacter": str,
+    },
 )
 
 AudioSpecificationTypeDef = TypedDict(
     "AudioSpecificationTypeDef",
     {
         "maxLengthMs": int,
         "endTimeoutMs": int,
@@ -550,14 +1036,23 @@
         "maxLength": int,
         "endTimeoutMs": int,
         "deletionCharacter": str,
         "endCharacter": str,
     },
 )
 
+S3BucketLogDestinationOutputTypeDef = TypedDict(
+    "S3BucketLogDestinationOutputTypeDef",
+    {
+        "kmsKeyArn": str,
+        "s3BucketArn": str,
+        "logPrefix": str,
+    },
+)
+
 _RequiredS3BucketLogDestinationTypeDef = TypedDict(
     "_RequiredS3BucketLogDestinationTypeDef",
     {
         "s3BucketArn": str,
         "logPrefix": str,
     },
 )
@@ -590,85 +1085,109 @@
 )
 
 class NewCustomVocabularyItemTypeDef(
     _RequiredNewCustomVocabularyItemTypeDef, _OptionalNewCustomVocabularyItemTypeDef
 ):
     pass
 
-_RequiredCustomVocabularyItemTypeDef = TypedDict(
-    "_RequiredCustomVocabularyItemTypeDef",
+CustomVocabularyItemOutputTypeDef = TypedDict(
+    "CustomVocabularyItemOutputTypeDef",
     {
         "itemId": str,
         "phrase": str,
-    },
-)
-_OptionalCustomVocabularyItemTypeDef = TypedDict(
-    "_OptionalCustomVocabularyItemTypeDef",
-    {
         "weight": int,
         "displayAs": str,
     },
-    total=False,
 )
 
-class CustomVocabularyItemTypeDef(
-    _RequiredCustomVocabularyItemTypeDef, _OptionalCustomVocabularyItemTypeDef
-):
-    pass
-
 FailedCustomVocabularyItemTypeDef = TypedDict(
     "FailedCustomVocabularyItemTypeDef",
     {
         "itemId": str,
         "errorMessage": str,
         "errorCode": ErrorCodeType,
     },
-    total=False,
 )
 
 CustomVocabularyEntryIdTypeDef = TypedDict(
     "CustomVocabularyEntryIdTypeDef",
     {
         "itemId": str,
     },
 )
 
+_RequiredCustomVocabularyItemTypeDef = TypedDict(
+    "_RequiredCustomVocabularyItemTypeDef",
+    {
+        "itemId": str,
+        "phrase": str,
+    },
+)
+_OptionalCustomVocabularyItemTypeDef = TypedDict(
+    "_OptionalCustomVocabularyItemTypeDef",
+    {
+        "weight": int,
+        "displayAs": str,
+    },
+    total=False,
+)
+
+class CustomVocabularyItemTypeDef(
+    _RequiredCustomVocabularyItemTypeDef, _OptionalCustomVocabularyItemTypeDef
+):
+    pass
+
 BotAliasHistoryEventTypeDef = TypedDict(
     "BotAliasHistoryEventTypeDef",
     {
         "botVersion": str,
         "startDate": datetime,
         "endDate": datetime,
     },
-    total=False,
 )
 
 BotAliasSummaryTypeDef = TypedDict(
     "BotAliasSummaryTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
         "botAliasStatus": BotAliasStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
+)
+
+BotAliasTestExecutionTargetOutputTypeDef = TypedDict(
+    "BotAliasTestExecutionTargetOutputTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+    },
 )
 
 BotAliasTestExecutionTargetTypeDef = TypedDict(
     "BotAliasTestExecutionTargetTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
     },
 )
 
+BotExportSpecificationOutputTypeDef = TypedDict(
+    "BotExportSpecificationOutputTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+    },
+)
+
 BotExportSpecificationTypeDef = TypedDict(
     "BotExportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
     },
 )
@@ -678,21 +1197,37 @@
     {
         "name": BotFilterNameType,
         "values": Sequence[str],
         "operator": BotFilterOperatorType,
     },
 )
 
+DataPrivacyOutputTypeDef = TypedDict(
+    "DataPrivacyOutputTypeDef",
+    {
+        "childDirected": bool,
+    },
+)
+
 DataPrivacyTypeDef = TypedDict(
     "DataPrivacyTypeDef",
     {
         "childDirected": bool,
     },
 )
 
+BotLocaleExportSpecificationOutputTypeDef = TypedDict(
+    "BotLocaleExportSpecificationOutputTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+
 BotLocaleExportSpecificationTypeDef = TypedDict(
     "BotLocaleExportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -711,14 +1246,22 @@
     "BotLocaleHistoryEventTypeDef",
     {
         "event": str,
         "eventDate": datetime,
     },
 )
 
+VoiceSettingsOutputTypeDef = TypedDict(
+    "VoiceSettingsOutputTypeDef",
+    {
+        "voiceId": str,
+        "engine": VoiceEngineType,
+    },
+)
+
 _RequiredVoiceSettingsTypeDef = TypedDict(
     "_RequiredVoiceSettingsTypeDef",
     {
         "voiceId": str,
     },
 )
 _OptionalVoiceSettingsTypeDef = TypedDict(
@@ -746,15 +1289,25 @@
         "localeId": str,
         "localeName": str,
         "description": str,
         "botLocaleStatus": BotLocaleStatusType,
         "lastUpdatedDateTime": datetime,
         "lastBuildSubmittedDateTime": datetime,
     },
-    total=False,
+)
+
+BotMemberOutputTypeDef = TypedDict(
+    "BotMemberOutputTypeDef",
+    {
+        "botMemberId": str,
+        "botMemberName": str,
+        "botMemberAliasId": str,
+        "botMemberAliasName": str,
+        "botMemberVersion": str,
+    },
 )
 
 BotMemberTypeDef = TypedDict(
     "BotMemberTypeDef",
     {
         "botMemberId": str,
         "botMemberName": str,
@@ -765,46 +1318,33 @@
 )
 
 IntentStatisticsTypeDef = TypedDict(
     "IntentStatisticsTypeDef",
     {
         "discoveredIntentCount": int,
     },
-    total=False,
 )
 
 SlotTypeStatisticsTypeDef = TypedDict(
     "SlotTypeStatisticsTypeDef",
     {
         "discoveredSlotTypeCount": int,
     },
-    total=False,
 )
 
-_RequiredBotRecommendationSummaryTypeDef = TypedDict(
-    "_RequiredBotRecommendationSummaryTypeDef",
+BotRecommendationSummaryTypeDef = TypedDict(
+    "BotRecommendationSummaryTypeDef",
     {
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
-    },
-)
-_OptionalBotRecommendationSummaryTypeDef = TypedDict(
-    "_OptionalBotRecommendationSummaryTypeDef",
-    {
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
-class BotRecommendationSummaryTypeDef(
-    _RequiredBotRecommendationSummaryTypeDef, _OptionalBotRecommendationSummaryTypeDef
-):
-    pass
-
 BotSortByTypeDef = TypedDict(
     "BotSortByTypeDef",
     {
         "attribute": Literal["BotName"],
         "order": SortOrderType,
     },
 )
@@ -816,15 +1356,21 @@
         "botName": str,
         "description": str,
         "botStatus": BotStatusType,
         "latestBotVersion": str,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
     },
-    total=False,
+)
+
+BotVersionLocaleDetailsOutputTypeDef = TypedDict(
+    "BotVersionLocaleDetailsOutputTypeDef",
+    {
+        "sourceBotVersion": str,
+    },
 )
 
 BotVersionLocaleDetailsTypeDef = TypedDict(
     "BotVersionLocaleDetailsTypeDef",
     {
         "sourceBotVersion": str,
     },
@@ -843,15 +1389,14 @@
     {
         "botName": str,
         "botVersion": str,
         "description": str,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
     },
-    total=False,
 )
 
 BuildBotLocaleRequestRequestTypeDef = TypedDict(
     "BuildBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
@@ -881,15 +1426,14 @@
 
 BuiltInIntentSummaryTypeDef = TypedDict(
     "BuiltInIntentSummaryTypeDef",
     {
         "intentSignature": str,
         "description": str,
     },
-    total=False,
 )
 
 BuiltInSlotTypeSortByTypeDef = TypedDict(
     "BuiltInSlotTypeSortByTypeDef",
     {
         "attribute": Literal["SlotTypeSignature"],
         "order": SortOrderType,
@@ -898,49 +1442,87 @@
 
 BuiltInSlotTypeSummaryTypeDef = TypedDict(
     "BuiltInSlotTypeSummaryTypeDef",
     {
         "slotTypeSignature": str,
         "description": str,
     },
-    total=False,
+)
+
+ButtonOutputTypeDef = TypedDict(
+    "ButtonOutputTypeDef",
+    {
+        "text": str,
+        "value": str,
+    },
 )
 
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
 
+CloudWatchLogGroupLogDestinationOutputTypeDef = TypedDict(
+    "CloudWatchLogGroupLogDestinationOutputTypeDef",
+    {
+        "cloudWatchLogGroupArn": str,
+        "logPrefix": str,
+    },
+)
+
 CloudWatchLogGroupLogDestinationTypeDef = TypedDict(
     "CloudWatchLogGroupLogDestinationTypeDef",
     {
         "cloudWatchLogGroupArn": str,
         "logPrefix": str,
     },
 )
 
+LambdaCodeHookOutputTypeDef = TypedDict(
+    "LambdaCodeHookOutputTypeDef",
+    {
+        "lambdaARN": str,
+        "codeHookInterfaceVersion": str,
+    },
+)
+
 LambdaCodeHookTypeDef = TypedDict(
     "LambdaCodeHookTypeDef",
     {
         "lambdaARN": str,
         "codeHookInterfaceVersion": str,
     },
 )
 
+SubSlotTypeCompositionOutputTypeDef = TypedDict(
+    "SubSlotTypeCompositionOutputTypeDef",
+    {
+        "name": str,
+        "slotTypeId": str,
+    },
+)
+
 SubSlotTypeCompositionTypeDef = TypedDict(
     "SubSlotTypeCompositionTypeDef",
     {
         "name": str,
         "slotTypeId": str,
     },
 )
 
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "expressionString": str,
+    },
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "expressionString": str,
     },
 )
 
@@ -948,33 +1530,22 @@
     "ConversationLevelIntentClassificationResultItemTypeDef",
     {
         "intentName": str,
         "matchResult": TestResultMatchStatusType,
     },
 )
 
-_RequiredConversationLevelResultDetailTypeDef = TypedDict(
-    "_RequiredConversationLevelResultDetailTypeDef",
+ConversationLevelResultDetailTypeDef = TypedDict(
+    "ConversationLevelResultDetailTypeDef",
     {
         "endToEndResult": TestResultMatchStatusType,
-    },
-)
-_OptionalConversationLevelResultDetailTypeDef = TypedDict(
-    "_OptionalConversationLevelResultDetailTypeDef",
-    {
         "speechTranscriptionResult": TestResultMatchStatusType,
     },
-    total=False,
 )
 
-class ConversationLevelResultDetailTypeDef(
-    _RequiredConversationLevelResultDetailTypeDef, _OptionalConversationLevelResultDetailTypeDef
-):
-    pass
-
 ConversationLevelSlotResolutionResultItemTypeDef = TypedDict(
     "ConversationLevelSlotResolutionResultItemTypeDef",
     {
         "intentName": str,
         "slotName": str,
         "matchResult": TestResultMatchStatusType,
     },
@@ -984,30 +1555,46 @@
     "ConversationLevelTestResultsFilterByTypeDef",
     {
         "endToEndResult": TestResultMatchStatusType,
     },
     total=False,
 )
 
-ConversationLogsDataSourceFilterByTypeDef = TypedDict(
-    "ConversationLogsDataSourceFilterByTypeDef",
+ConversationLogsDataSourceFilterByOutputTypeDef = TypedDict(
+    "ConversationLogsDataSourceFilterByOutputTypeDef",
     {
         "startTime": datetime,
         "endTime": datetime,
         "inputMode": ConversationLogsInputModeFilterType,
     },
 )
 
+ConversationLogsDataSourceFilterByTypeDef = TypedDict(
+    "ConversationLogsDataSourceFilterByTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+        "inputMode": ConversationLogsInputModeFilterType,
+    },
+)
+
 SentimentAnalysisSettingsTypeDef = TypedDict(
     "SentimentAnalysisSettingsTypeDef",
     {
         "detectSentiment": bool,
     },
 )
 
+SentimentAnalysisSettingsOutputTypeDef = TypedDict(
+    "SentimentAnalysisSettingsOutputTypeDef",
+    {
+        "detectSentiment": bool,
+    },
+)
+
 DialogCodeHookSettingsTypeDef = TypedDict(
     "DialogCodeHookSettingsTypeDef",
     {
         "enabled": bool,
     },
 )
 
@@ -1050,14 +1637,53 @@
 SampleUtteranceTypeDef = TypedDict(
     "SampleUtteranceTypeDef",
     {
         "utterance": str,
     },
 )
 
+DialogCodeHookSettingsOutputTypeDef = TypedDict(
+    "DialogCodeHookSettingsOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+
+InputContextOutputTypeDef = TypedDict(
+    "InputContextOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
+KendraConfigurationOutputTypeDef = TypedDict(
+    "KendraConfigurationOutputTypeDef",
+    {
+        "kendraIndex": str,
+        "queryFilterStringEnabled": bool,
+        "queryFilterString": str,
+    },
+)
+
+OutputContextOutputTypeDef = TypedDict(
+    "OutputContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLiveInSeconds": int,
+        "turnsToLive": int,
+    },
+)
+
+SampleUtteranceOutputTypeDef = TypedDict(
+    "SampleUtteranceOutputTypeDef",
+    {
+        "utterance": str,
+    },
+)
+
 CreateResourcePolicyRequestRequestTypeDef = TypedDict(
     "CreateResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
         "policy": str,
     },
 )
@@ -1100,56 +1726,103 @@
 ObfuscationSettingTypeDef = TypedDict(
     "ObfuscationSettingTypeDef",
     {
         "obfuscationSettingType": ObfuscationSettingTypeType,
     },
 )
 
+MultipleValuesSettingOutputTypeDef = TypedDict(
+    "MultipleValuesSettingOutputTypeDef",
+    {
+        "allowMultipleValues": bool,
+    },
+)
+
+ObfuscationSettingOutputTypeDef = TypedDict(
+    "ObfuscationSettingOutputTypeDef",
+    {
+        "obfuscationSettingType": ObfuscationSettingTypeType,
+    },
+)
+
 CreateUploadUrlResponseTypeDef = TypedDict(
     "CreateUploadUrlResponseTypeDef",
     {
         "importId": str,
         "uploadUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CustomPayloadOutputTypeDef = TypedDict(
+    "CustomPayloadOutputTypeDef",
+    {
+        "value": str,
+    },
+)
+
 CustomPayloadTypeDef = TypedDict(
     "CustomPayloadTypeDef",
     {
         "value": str,
     },
 )
 
+CustomVocabularyExportSpecificationOutputTypeDef = TypedDict(
+    "CustomVocabularyExportSpecificationOutputTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+
 CustomVocabularyExportSpecificationTypeDef = TypedDict(
     "CustomVocabularyExportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
+CustomVocabularyImportSpecificationOutputTypeDef = TypedDict(
+    "CustomVocabularyImportSpecificationOutputTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+
 CustomVocabularyImportSpecificationTypeDef = TypedDict(
     "CustomVocabularyImportSpecificationTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-DateRangeFilterTypeDef = TypedDict(
-    "DateRangeFilterTypeDef",
+DateRangeFilterOutputTypeDef = TypedDict(
+    "DateRangeFilterOutputTypeDef",
     {
         "startDateTime": datetime,
         "endDateTime": datetime,
     },
 )
 
+DateRangeFilterTypeDef = TypedDict(
+    "DateRangeFilterTypeDef",
+    {
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+    },
+)
+
 _RequiredDeleteBotAliasRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBotAliasRequestRequestTypeDef",
     {
         "botAliasId": str,
         "botId": str,
     },
 )
@@ -1475,22 +2148,21 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
     },
 )
 
-EncryptionSettingTypeDef = TypedDict(
-    "EncryptionSettingTypeDef",
+EncryptionSettingOutputTypeDef = TypedDict(
+    "EncryptionSettingOutputTypeDef",
     {
         "kmsKeyArn": str,
         "botLocaleExportPassword": str,
         "associatedTranscriptsPassword": str,
     },
-    total=False,
 )
 
 DescribeBotRequestRequestTypeDef = TypedDict(
     "DescribeBotRequestRequestTypeDef",
     {
         "botId": str,
     },
@@ -1546,16 +2218,16 @@
         "intentId": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
 
-SlotPriorityTypeDef = TypedDict(
-    "SlotPriorityTypeDef",
+SlotPriorityOutputTypeDef = TypedDict(
+    "SlotPriorityOutputTypeDef",
     {
         "priority": int,
         "slotId": str,
     },
 )
 
 DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
@@ -1613,41 +2285,39 @@
 DescribeTestSetGenerationRequestRequestTypeDef = TypedDict(
     "DescribeTestSetGenerationRequestRequestTypeDef",
     {
         "testSetGenerationId": str,
     },
 )
 
-_RequiredTestSetStorageLocationTypeDef = TypedDict(
-    "_RequiredTestSetStorageLocationTypeDef",
+TestSetStorageLocationOutputTypeDef = TypedDict(
+    "TestSetStorageLocationOutputTypeDef",
     {
         "s3BucketName": str,
         "s3Path": str,
-    },
-)
-_OptionalTestSetStorageLocationTypeDef = TypedDict(
-    "_OptionalTestSetStorageLocationTypeDef",
-    {
         "kmsKeyArn": str,
     },
-    total=False,
 )
 
-class TestSetStorageLocationTypeDef(
-    _RequiredTestSetStorageLocationTypeDef, _OptionalTestSetStorageLocationTypeDef
-):
-    pass
-
 DescribeTestSetRequestRequestTypeDef = TypedDict(
     "DescribeTestSetRequestRequestTypeDef",
     {
         "testSetId": str,
     },
 )
 
+DialogActionOutputTypeDef = TypedDict(
+    "DialogActionOutputTypeDef",
+    {
+        "type": DialogActionTypeType,
+        "slotToElicit": str,
+        "suppressNextMessage": bool,
+    },
+)
+
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
@@ -1658,23 +2328,39 @@
     },
     total=False,
 )
 
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
+IntentOverrideOutputTypeDef = TypedDict(
+    "IntentOverrideOutputTypeDef",
+    {
+        "name": str,
+        "slots": Dict[str, "SlotValueOverrideOutputTypeDef"],
+    },
+)
+
 IntentOverrideTypeDef = TypedDict(
     "IntentOverrideTypeDef",
     {
         "name": str,
         "slots": Mapping[str, "SlotValueOverrideTypeDef"],
     },
     total=False,
 )
 
+ElicitationCodeHookInvocationSettingOutputTypeDef = TypedDict(
+    "ElicitationCodeHookInvocationSettingOutputTypeDef",
+    {
+        "enableCodeHookInvocation": bool,
+        "invocationLabel": str,
+    },
+)
+
 _RequiredElicitationCodeHookInvocationSettingTypeDef = TypedDict(
     "_RequiredElicitationCodeHookInvocationSettingTypeDef",
     {
         "enableCodeHookInvocation": bool,
     },
 )
 _OptionalElicitationCodeHookInvocationSettingTypeDef = TypedDict(
@@ -1694,23 +2380,40 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionSettingTypeDef = TypedDict(
+    "EncryptionSettingTypeDef",
+    {
+        "kmsKeyArn": str,
+        "botLocaleExportPassword": str,
+        "associatedTranscriptsPassword": str,
+    },
+    total=False,
+)
+
 ExportFilterTypeDef = TypedDict(
     "ExportFilterTypeDef",
     {
         "name": Literal["ExportResourceType"],
         "values": Sequence[str],
         "operator": ExportFilterOperatorType,
     },
 )
 
+TestSetExportSpecificationOutputTypeDef = TypedDict(
+    "TestSetExportSpecificationOutputTypeDef",
+    {
+        "testSetId": str,
+    },
+)
+
 TestSetExportSpecificationTypeDef = TypedDict(
     "TestSetExportSpecificationTypeDef",
     {
         "testSetId": str,
     },
 )
 
@@ -1734,14 +2437,23 @@
     {
         "testExecutionId": str,
         "downloadArtifactsUrl": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GrammarSlotTypeSourceOutputTypeDef = TypedDict(
+    "GrammarSlotTypeSourceOutputTypeDef",
+    {
+        "s3BucketName": str,
+        "s3ObjectKey": str,
+        "kmsKeyArn": str,
+    },
+)
+
 _RequiredGrammarSlotTypeSourceTypeDef = TypedDict(
     "_RequiredGrammarSlotTypeSourceTypeDef",
     {
         "s3BucketName": str,
         "s3ObjectKey": str,
     },
 )
@@ -1783,46 +2495,32 @@
         "importedResourceName": str,
         "importStatus": ImportStatusType,
         "mergeStrategy": MergeStrategyType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "importedResourceType": ImportResourceTypeType,
     },
-    total=False,
 )
 
 RuntimeHintsTypeDef = TypedDict(
     "RuntimeHintsTypeDef",
     {
         "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsTypeDef"]],
     },
-    total=False,
 )
 
-_RequiredIntentClassificationTestResultItemCountsTypeDef = TypedDict(
-    "_RequiredIntentClassificationTestResultItemCountsTypeDef",
+IntentClassificationTestResultItemCountsTypeDef = TypedDict(
+    "IntentClassificationTestResultItemCountsTypeDef",
     {
         "totalResultCount": int,
-        "intentMatchResultCounts": Dict[TestResultMatchStatusType, int],
-    },
-)
-_OptionalIntentClassificationTestResultItemCountsTypeDef = TypedDict(
-    "_OptionalIntentClassificationTestResultItemCountsTypeDef",
-    {
         "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
+        "intentMatchResultCounts": Dict[TestResultMatchStatusType, int],
     },
-    total=False,
 )
 
-class IntentClassificationTestResultItemCountsTypeDef(
-    _RequiredIntentClassificationTestResultItemCountsTypeDef,
-    _OptionalIntentClassificationTestResultItemCountsTypeDef,
-):
-    pass
-
 IntentFilterTypeDef = TypedDict(
     "IntentFilterTypeDef",
     {
         "name": Literal["IntentName"],
         "values": Sequence[str],
         "operator": IntentFilterOperatorType,
     },
@@ -1832,14 +2530,21 @@
     "IntentSortByTypeDef",
     {
         "attribute": IntentSortAttributeType,
         "order": SortOrderType,
     },
 )
 
+InvokedIntentSampleTypeDef = TypedDict(
+    "InvokedIntentSampleTypeDef",
+    {
+        "intentName": str,
+    },
+)
+
 _RequiredListBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListBotAliasesRequestRequestTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalListBotAliasesRequestRequestTypeDef = TypedDict(
@@ -1929,15 +2634,22 @@
 RecommendedIntentSummaryTypeDef = TypedDict(
     "RecommendedIntentSummaryTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "sampleUtterancesCount": int,
     },
-    total=False,
+)
+
+SessionDataSortByTypeDef = TypedDict(
+    "SessionDataSortByTypeDef",
+    {
+        "name": AnalyticsSessionSortByNameType,
+        "order": AnalyticsSortOrderType,
+    },
 )
 
 SlotTypeFilterTypeDef = TypedDict(
     "SlotTypeFilterTypeDef",
     {
         "name": SlotTypeFilterNameType,
         "values": Sequence[str],
@@ -1959,15 +2671,14 @@
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
         "parentSlotTypeSignature": str,
         "lastUpdatedDateTime": datetime,
         "slotTypeCategory": SlotTypeCategoryType,
     },
-    total=False,
 )
 
 SlotFilterTypeDef = TypedDict(
     "SlotFilterTypeDef",
     {
         "name": Literal["SlotName"],
         "values": Sequence[str],
@@ -2031,64 +2742,97 @@
     "TestSetSortByTypeDef",
     {
         "attribute": TestSetSortAttributeType,
         "order": SortOrderType,
     },
 )
 
+UtteranceDataSortByTypeDef = TypedDict(
+    "UtteranceDataSortByTypeDef",
+    {
+        "name": Literal["UtteranceTimestamp"],
+        "order": AnalyticsSortOrderType,
+    },
+)
+
+PlainTextMessageOutputTypeDef = TypedDict(
+    "PlainTextMessageOutputTypeDef",
+    {
+        "value": str,
+    },
+)
+
+SSMLMessageOutputTypeDef = TypedDict(
+    "SSMLMessageOutputTypeDef",
+    {
+        "value": str,
+    },
+)
+
 PlainTextMessageTypeDef = TypedDict(
     "PlainTextMessageTypeDef",
     {
         "value": str,
     },
 )
 
 SSMLMessageTypeDef = TypedDict(
     "SSMLMessageTypeDef",
     {
         "value": str,
     },
 )
 
-_RequiredOverallTestResultItemTypeDef = TypedDict(
-    "_RequiredOverallTestResultItemTypeDef",
+OverallTestResultItemTypeDef = TypedDict(
+    "OverallTestResultItemTypeDef",
     {
         "multiTurnConversation": bool,
         "totalResultCount": int,
+        "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
         "endToEndResultCounts": Dict[TestResultMatchStatusType, int],
     },
 )
-_OptionalOverallTestResultItemTypeDef = TypedDict(
-    "_OptionalOverallTestResultItemTypeDef",
+
+PathFormatOutputTypeDef = TypedDict(
+    "PathFormatOutputTypeDef",
     {
-        "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
+        "objectPrefixes": List[str],
     },
-    total=False,
 )
 
-class OverallTestResultItemTypeDef(
-    _RequiredOverallTestResultItemTypeDef, _OptionalOverallTestResultItemTypeDef
-):
-    pass
-
 PathFormatTypeDef = TypedDict(
     "PathFormatTypeDef",
     {
-        "objectPrefixes": List[str],
+        "objectPrefixes": Sequence[str],
     },
     total=False,
 )
 
+TextInputSpecificationOutputTypeDef = TypedDict(
+    "TextInputSpecificationOutputTypeDef",
+    {
+        "startTimeoutMs": int,
+    },
+)
+
 TextInputSpecificationTypeDef = TypedDict(
     "TextInputSpecificationTypeDef",
     {
         "startTimeoutMs": int,
     },
 )
 
+RelativeAggregationDurationOutputTypeDef = TypedDict(
+    "RelativeAggregationDurationOutputTypeDef",
+    {
+        "timeDimension": TimeDimensionType,
+        "timeValue": int,
+    },
+)
+
 RelativeAggregationDurationTypeDef = TypedDict(
     "RelativeAggregationDurationTypeDef",
     {
         "timeDimension": TimeDimensionType,
         "timeValue": int,
     },
 )
@@ -2107,64 +2851,108 @@
 RuntimeHintValueTypeDef = TypedDict(
     "RuntimeHintValueTypeDef",
     {
         "phrase": str,
     },
 )
 
+SampleValueOutputTypeDef = TypedDict(
+    "SampleValueOutputTypeDef",
+    {
+        "value": str,
+    },
+)
+
 SampleValueTypeDef = TypedDict(
     "SampleValueTypeDef",
     {
         "value": str,
     },
 )
 
+SlotDefaultValueOutputTypeDef = TypedDict(
+    "SlotDefaultValueOutputTypeDef",
+    {
+        "defaultValue": str,
+    },
+)
+
 SlotDefaultValueTypeDef = TypedDict(
     "SlotDefaultValueTypeDef",
     {
         "defaultValue": str,
     },
 )
 
-_RequiredSlotResolutionTestResultItemCountsTypeDef = TypedDict(
-    "_RequiredSlotResolutionTestResultItemCountsTypeDef",
+SlotPriorityTypeDef = TypedDict(
+    "SlotPriorityTypeDef",
     {
-        "totalResultCount": int,
-        "slotMatchResultCounts": Dict[TestResultMatchStatusType, int],
+        "priority": int,
+        "slotId": str,
     },
 )
-_OptionalSlotResolutionTestResultItemCountsTypeDef = TypedDict(
-    "_OptionalSlotResolutionTestResultItemCountsTypeDef",
+
+SlotResolutionTestResultItemCountsTypeDef = TypedDict(
+    "SlotResolutionTestResultItemCountsTypeDef",
     {
+        "totalResultCount": int,
         "speechTranscriptionResultCounts": Dict[TestResultMatchStatusType, int],
+        "slotMatchResultCounts": Dict[TestResultMatchStatusType, int],
     },
-    total=False,
 )
 
-class SlotResolutionTestResultItemCountsTypeDef(
-    _RequiredSlotResolutionTestResultItemCountsTypeDef,
-    _OptionalSlotResolutionTestResultItemCountsTypeDef,
-):
-    pass
+SlotValueOutputTypeDef = TypedDict(
+    "SlotValueOutputTypeDef",
+    {
+        "interpretedValue": str,
+    },
+)
 
 SlotValueTypeDef = TypedDict(
     "SlotValueTypeDef",
     {
         "interpretedValue": str,
     },
     total=False,
 )
 
+SlotValueRegexFilterOutputTypeDef = TypedDict(
+    "SlotValueRegexFilterOutputTypeDef",
+    {
+        "pattern": str,
+    },
+)
+
 SlotValueRegexFilterTypeDef = TypedDict(
     "SlotValueRegexFilterTypeDef",
     {
         "pattern": str,
     },
 )
 
+_RequiredTestSetStorageLocationTypeDef = TypedDict(
+    "_RequiredTestSetStorageLocationTypeDef",
+    {
+        "s3BucketName": str,
+        "s3Path": str,
+    },
+)
+_OptionalTestSetStorageLocationTypeDef = TypedDict(
+    "_OptionalTestSetStorageLocationTypeDef",
+    {
+        "kmsKeyArn": str,
+    },
+    total=False,
+)
+
+class TestSetStorageLocationTypeDef(
+    _RequiredTestSetStorageLocationTypeDef, _OptionalTestSetStorageLocationTypeDef
+):
+    pass
+
 StopBotRecommendationRequestRequestTypeDef = TypedDict(
     "StopBotRecommendationRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
@@ -2204,23 +2992,40 @@
     {
         "intentName": str,
         "slotName": str,
         "errorMessage": str,
     },
 )
 
+TestSetDiscrepancyReportBotAliasTargetOutputTypeDef = TypedDict(
+    "TestSetDiscrepancyReportBotAliasTargetOutputTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+    },
+)
+
 TestSetDiscrepancyReportBotAliasTargetTypeDef = TypedDict(
     "TestSetDiscrepancyReportBotAliasTargetTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
     },
 )
 
+TestSetImportInputLocationOutputTypeDef = TypedDict(
+    "TestSetImportInputLocationOutputTypeDef",
+    {
+        "s3BucketName": str,
+        "s3Path": str,
+    },
+)
+
 TestSetImportInputLocationTypeDef = TypedDict(
     "TestSetImportInputLocationTypeDef",
     {
         "s3BucketName": str,
         "s3Path": str,
     },
 )
@@ -2298,68 +3103,222 @@
 )
 
 class UpdateTestSetRequestRequestTypeDef(
     _RequiredUpdateTestSetRequestRequestTypeDef, _OptionalUpdateTestSetRequestRequestTypeDef
 ):
     pass
 
-_RequiredUserTurnIntentOutputTypeDef = TypedDict(
-    "_RequiredUserTurnIntentOutputTypeDef",
+UserTurnIntentOutputTypeDef = TypedDict(
+    "UserTurnIntentOutputTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalUserTurnIntentOutputTypeDef = TypedDict(
-    "_OptionalUserTurnIntentOutputTypeDef",
-    {
         "slots": Dict[str, "UserTurnSlotOutputTypeDef"],
     },
-    total=False,
 )
 
-class UserTurnIntentOutputTypeDef(
-    _RequiredUserTurnIntentOutputTypeDef, _OptionalUserTurnIntentOutputTypeDef
-):
-    pass
-
 UserTurnSlotOutputTypeDef = TypedDict(
     "UserTurnSlotOutputTypeDef",
     {
         "value": str,
         "values": List[Dict[str, Any]],
         "subSlots": Dict[str, Dict[str, Any]],
     },
-    total=False,
 )
 
 UtteranceAudioInputSpecificationTypeDef = TypedDict(
     "UtteranceAudioInputSpecificationTypeDef",
     {
         "audioFileS3Location": str,
     },
 )
 
-_RequiredAgentTurnResultTypeDef = TypedDict(
-    "_RequiredAgentTurnResultTypeDef",
+AgentTurnResultTypeDef = TypedDict(
+    "AgentTurnResultTypeDef",
     {
         "expectedAgentPrompt": str,
-    },
-)
-_OptionalAgentTurnResultTypeDef = TypedDict(
-    "_OptionalAgentTurnResultTypeDef",
-    {
         "actualAgentPrompt": str,
         "errorDetails": ExecutionErrorDetailsTypeDef,
         "actualElicitedSlot": str,
         "actualIntent": str,
     },
+)
+
+AnalyticsIntentResultTypeDef = TypedDict(
+    "AnalyticsIntentResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsIntentGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsIntentMetricResultTypeDef],
+    },
+)
+
+_RequiredListIntentMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+        "metrics": Sequence[AnalyticsIntentMetricTypeDef],
+    },
+)
+_OptionalListIntentMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsIntentGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsIntentFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListIntentMetricsRequestRequestTypeDef(
+    _RequiredListIntentMetricsRequestRequestTypeDef, _OptionalListIntentMetricsRequestRequestTypeDef
+):
+    pass
+
+ListIntentPathsResponseTypeDef = TypedDict(
+    "ListIntentPathsResponseTypeDef",
+    {
+        "nodeSummaries": List[AnalyticsIntentNodeSummaryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AnalyticsIntentStageResultTypeDef = TypedDict(
+    "AnalyticsIntentStageResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsIntentStageGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsIntentStageMetricResultTypeDef],
+    },
+)
+
+_RequiredListIntentStageMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentStageMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+        "metrics": Sequence[AnalyticsIntentStageMetricTypeDef],
+    },
+)
+_OptionalListIntentStageMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentStageMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsIntentStageGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsIntentStageFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListIntentStageMetricsRequestRequestTypeDef(
+    _RequiredListIntentStageMetricsRequestRequestTypeDef,
+    _OptionalListIntentStageMetricsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListIntentPathsRequestRequestTypeDef = TypedDict(
+    "_RequiredListIntentPathsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+        "intentPath": str,
+    },
+)
+_OptionalListIntentPathsRequestRequestTypeDef = TypedDict(
+    "_OptionalListIntentPathsRequestRequestTypeDef",
+    {
+        "filters": Sequence[AnalyticsPathFilterTypeDef],
+    },
+    total=False,
+)
+
+class ListIntentPathsRequestRequestTypeDef(
+    _RequiredListIntentPathsRequestRequestTypeDef, _OptionalListIntentPathsRequestRequestTypeDef
+):
+    pass
+
+AnalyticsSessionResultTypeDef = TypedDict(
+    "AnalyticsSessionResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsSessionGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsSessionMetricResultTypeDef],
+    },
+)
+
+_RequiredListSessionMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListSessionMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+        "metrics": Sequence[AnalyticsSessionMetricTypeDef],
+    },
+)
+_OptionalListSessionMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListSessionMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsSessionGroupBySpecificationTypeDef],
+        "filters": Sequence[AnalyticsSessionFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
     total=False,
 )
 
-class AgentTurnResultTypeDef(_RequiredAgentTurnResultTypeDef, _OptionalAgentTurnResultTypeDef):
+class ListSessionMetricsRequestRequestTypeDef(
+    _RequiredListSessionMetricsRequestRequestTypeDef,
+    _OptionalListSessionMetricsRequestRequestTypeDef,
+):
+    pass
+
+AnalyticsUtteranceResultTypeDef = TypedDict(
+    "AnalyticsUtteranceResultTypeDef",
+    {
+        "binKeys": List[AnalyticsBinKeyTypeDef],
+        "groupByKeys": List[AnalyticsUtteranceGroupByKeyTypeDef],
+        "metricsResults": List[AnalyticsUtteranceMetricResultTypeDef],
+        "attributeResults": List[AnalyticsUtteranceAttributeResultTypeDef],
+    },
+)
+
+_RequiredListUtteranceMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredListUtteranceMetricsRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+        "metrics": Sequence[AnalyticsUtteranceMetricTypeDef],
+    },
+)
+_OptionalListUtteranceMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalListUtteranceMetricsRequestRequestTypeDef",
+    {
+        "binBy": Sequence[AnalyticsBinBySpecificationTypeDef],
+        "groupBy": Sequence[AnalyticsUtteranceGroupBySpecificationTypeDef],
+        "attributes": Sequence[AnalyticsUtteranceAttributeTypeDef],
+        "filters": Sequence[AnalyticsUtteranceFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListUtteranceMetricsRequestRequestTypeDef(
+    _RequiredListUtteranceMetricsRequestRequestTypeDef,
+    _OptionalListUtteranceMetricsRequestRequestTypeDef,
+):
     pass
 
 _RequiredSearchAssociatedTranscriptsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchAssociatedTranscriptsRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
@@ -2394,14 +3353,23 @@
         "nextIndex": int,
         "associatedTranscripts": List[AssociatedTranscriptTypeDef],
         "totalResults": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AudioAndDTMFInputSpecificationOutputTypeDef = TypedDict(
+    "AudioAndDTMFInputSpecificationOutputTypeDef",
+    {
+        "startTimeoutMs": int,
+        "audioSpecification": AudioSpecificationOutputTypeDef,
+        "dtmfSpecification": DTMFSpecificationOutputTypeDef,
+    },
+)
+
 _RequiredAudioAndDTMFInputSpecificationTypeDef = TypedDict(
     "_RequiredAudioAndDTMFInputSpecificationTypeDef",
     {
         "startTimeoutMs": int,
     },
 )
 _OptionalAudioAndDTMFInputSpecificationTypeDef = TypedDict(
@@ -2414,14 +3382,21 @@
 )
 
 class AudioAndDTMFInputSpecificationTypeDef(
     _RequiredAudioAndDTMFInputSpecificationTypeDef, _OptionalAudioAndDTMFInputSpecificationTypeDef
 ):
     pass
 
+AudioLogDestinationOutputTypeDef = TypedDict(
+    "AudioLogDestinationOutputTypeDef",
+    {
+        "s3Bucket": S3BucketLogDestinationOutputTypeDef,
+    },
+)
+
 AudioLogDestinationTypeDef = TypedDict(
     "AudioLogDestinationTypeDef",
     {
         "s3Bucket": S3BucketLogDestinationTypeDef,
     },
 )
 
@@ -2431,178 +3406,163 @@
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "customVocabularyItemList": Sequence[NewCustomVocabularyItemTypeDef],
     },
 )
 
-BatchUpdateCustomVocabularyItemRequestRequestTypeDef = TypedDict(
-    "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "customVocabularyItemList": Sequence[CustomVocabularyItemTypeDef],
-    },
-)
-
 ListCustomVocabularyItemsResponseTypeDef = TypedDict(
     "ListCustomVocabularyItemsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
-        "customVocabularyItems": List[CustomVocabularyItemTypeDef],
+        "customVocabularyItems": List[CustomVocabularyItemOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchCreateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
-        "resources": List[CustomVocabularyItemTypeDef],
+        "resources": List[CustomVocabularyItemOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
-        "resources": List[CustomVocabularyItemTypeDef],
+        "resources": List[CustomVocabularyItemOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateCustomVocabularyItemResponseTypeDef = TypedDict(
     "BatchUpdateCustomVocabularyItemResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "errors": List[FailedCustomVocabularyItemTypeDef],
-        "resources": List[CustomVocabularyItemTypeDef],
+        "resources": List[CustomVocabularyItemOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteCustomVocabularyItemRequestRequestTypeDef = TypedDict(
     "BatchDeleteCustomVocabularyItemRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "customVocabularyItemList": Sequence[CustomVocabularyEntryIdTypeDef],
     },
 )
 
+BatchUpdateCustomVocabularyItemRequestRequestTypeDef = TypedDict(
+    "BatchUpdateCustomVocabularyItemRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "customVocabularyItemList": Sequence[CustomVocabularyItemTypeDef],
+    },
+)
+
 ListBotAliasesResponseTypeDef = TypedDict(
     "ListBotAliasesResponseTypeDef",
     {
         "botAliasSummaries": List[BotAliasSummaryTypeDef],
         "nextToken": str,
         "botId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TestExecutionTargetOutputTypeDef = TypedDict(
+    "TestExecutionTargetOutputTypeDef",
+    {
+        "botAliasTarget": BotAliasTestExecutionTargetOutputTypeDef,
+    },
+)
+
 TestExecutionTargetTypeDef = TypedDict(
     "TestExecutionTargetTypeDef",
     {
         "botAliasTarget": BotAliasTestExecutionTargetTypeDef,
     },
     total=False,
 )
 
+BotImportSpecificationOutputTypeDef = TypedDict(
+    "BotImportSpecificationOutputTypeDef",
+    {
+        "botName": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyOutputTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botTags": Dict[str, str],
+        "testBotAliasTags": Dict[str, str],
+    },
+)
+
 _RequiredBotImportSpecificationTypeDef = TypedDict(
     "_RequiredBotImportSpecificationTypeDef",
     {
         "botName": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
     },
 )
 _OptionalBotImportSpecificationTypeDef = TypedDict(
     "_OptionalBotImportSpecificationTypeDef",
     {
         "idleSessionTTLInSeconds": int,
-        "botTags": Dict[str, str],
-        "testBotAliasTags": Dict[str, str],
+        "botTags": Mapping[str, str],
+        "testBotAliasTags": Mapping[str, str],
     },
     total=False,
 )
 
 class BotImportSpecificationTypeDef(
     _RequiredBotImportSpecificationTypeDef, _OptionalBotImportSpecificationTypeDef
 ):
     pass
 
-_RequiredBotLocaleImportSpecificationTypeDef = TypedDict(
-    "_RequiredBotLocaleImportSpecificationTypeDef",
+BotLocaleImportSpecificationOutputTypeDef = TypedDict(
+    "BotLocaleImportSpecificationOutputTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
-    },
-)
-_OptionalBotLocaleImportSpecificationTypeDef = TypedDict(
-    "_OptionalBotLocaleImportSpecificationTypeDef",
-    {
         "nluIntentConfidenceThreshold": float,
-        "voiceSettings": VoiceSettingsTypeDef,
+        "voiceSettings": VoiceSettingsOutputTypeDef,
     },
-    total=False,
 )
 
-class BotLocaleImportSpecificationTypeDef(
-    _RequiredBotLocaleImportSpecificationTypeDef, _OptionalBotLocaleImportSpecificationTypeDef
-):
-    pass
-
-_RequiredCreateBotLocaleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotLocaleRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "nluIntentConfidenceThreshold": float,
-    },
-)
-_OptionalCreateBotLocaleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotLocaleRequestRequestTypeDef",
-    {
-        "description": str,
-        "voiceSettings": VoiceSettingsTypeDef,
-    },
-    total=False,
-)
-
-class CreateBotLocaleRequestRequestTypeDef(
-    _RequiredCreateBotLocaleRequestRequestTypeDef, _OptionalCreateBotLocaleRequestRequestTypeDef
-):
-    pass
-
 CreateBotLocaleResponseTypeDef = TypedDict(
     "CreateBotLocaleResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeName": str,
         "localeId": str,
         "description": str,
         "nluIntentConfidenceThreshold": float,
-        "voiceSettings": VoiceSettingsTypeDef,
+        "voiceSettings": VoiceSettingsOutputTypeDef,
         "botLocaleStatus": BotLocaleStatusType,
         "creationDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBotLocaleResponseTypeDef = TypedDict(
@@ -2610,70 +3570,115 @@
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "localeName": str,
         "description": str,
         "nluIntentConfidenceThreshold": float,
-        "voiceSettings": VoiceSettingsTypeDef,
+        "voiceSettings": VoiceSettingsOutputTypeDef,
         "intentsCount": int,
         "slotTypesCount": int,
         "botLocaleStatus": BotLocaleStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "lastBuildSubmittedDateTime": datetime,
         "botLocaleHistoryEvents": List[BotLocaleHistoryEventTypeDef],
         "recommendedActions": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateBotLocaleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateBotLocaleRequestRequestTypeDef",
+UpdateBotLocaleResponseTypeDef = TypedDict(
+    "UpdateBotLocaleResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
+        "localeName": str,
+        "description": str,
         "nluIntentConfidenceThreshold": float,
+        "voiceSettings": VoiceSettingsOutputTypeDef,
+        "botLocaleStatus": BotLocaleStatusType,
+        "failureReasons": List[str],
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "recommendedActions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalUpdateBotLocaleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateBotLocaleRequestRequestTypeDef",
+
+_RequiredBotLocaleImportSpecificationTypeDef = TypedDict(
+    "_RequiredBotLocaleImportSpecificationTypeDef",
     {
-        "description": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+_OptionalBotLocaleImportSpecificationTypeDef = TypedDict(
+    "_OptionalBotLocaleImportSpecificationTypeDef",
+    {
+        "nluIntentConfidenceThreshold": float,
         "voiceSettings": VoiceSettingsTypeDef,
     },
     total=False,
 )
 
-class UpdateBotLocaleRequestRequestTypeDef(
-    _RequiredUpdateBotLocaleRequestRequestTypeDef, _OptionalUpdateBotLocaleRequestRequestTypeDef
+class BotLocaleImportSpecificationTypeDef(
+    _RequiredBotLocaleImportSpecificationTypeDef, _OptionalBotLocaleImportSpecificationTypeDef
 ):
     pass
 
-UpdateBotLocaleResponseTypeDef = TypedDict(
-    "UpdateBotLocaleResponseTypeDef",
+_RequiredCreateBotLocaleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotLocaleRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
-        "localeName": str,
+        "nluIntentConfidenceThreshold": float,
+    },
+)
+_OptionalCreateBotLocaleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotLocaleRequestRequestTypeDef",
+    {
         "description": str,
+        "voiceSettings": VoiceSettingsTypeDef,
+    },
+    total=False,
+)
+
+class CreateBotLocaleRequestRequestTypeDef(
+    _RequiredCreateBotLocaleRequestRequestTypeDef, _OptionalCreateBotLocaleRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateBotLocaleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBotLocaleRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
         "nluIntentConfidenceThreshold": float,
+    },
+)
+_OptionalUpdateBotLocaleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBotLocaleRequestRequestTypeDef",
+    {
+        "description": str,
         "voiceSettings": VoiceSettingsTypeDef,
-        "botLocaleStatus": BotLocaleStatusType,
-        "failureReasons": List[str],
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "recommendedActions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+class UpdateBotLocaleRequestRequestTypeDef(
+    _RequiredUpdateBotLocaleRequestRequestTypeDef, _OptionalUpdateBotLocaleRequestRequestTypeDef
+):
+    pass
+
 _RequiredListBotLocalesRequestRequestTypeDef = TypedDict(
     "_RequiredListBotLocalesRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
     },
 )
@@ -2700,128 +3705,127 @@
         "botVersion": str,
         "nextToken": str,
         "botLocaleSummaries": List[BotLocaleSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateBotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotRequestRequestTypeDef",
-    {
-        "botName": str,
-        "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
-        "idleSessionTTLInSeconds": int,
-    },
-)
-_OptionalCreateBotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotRequestRequestTypeDef",
-    {
-        "description": str,
-        "botTags": Mapping[str, str],
-        "testBotAliasTags": Mapping[str, str],
-        "botType": BotTypeType,
-        "botMembers": Sequence[BotMemberTypeDef],
-    },
-    total=False,
-)
-
-class CreateBotRequestRequestTypeDef(
-    _RequiredCreateBotRequestRequestTypeDef, _OptionalCreateBotRequestRequestTypeDef
-):
-    pass
-
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "description": str,
         "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
+        "dataPrivacy": DataPrivacyOutputTypeDef,
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "botTags": Dict[str, str],
         "testBotAliasTags": Dict[str, str],
         "botType": BotTypeType,
-        "botMembers": List[BotMemberTypeDef],
+        "botMembers": List[BotMemberOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBotResponseTypeDef = TypedDict(
     "DescribeBotResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "description": str,
         "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
+        "dataPrivacy": DataPrivacyOutputTypeDef,
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "botType": BotTypeType,
-        "botMembers": List[BotMemberTypeDef],
+        "botMembers": List[BotMemberOutputTypeDef],
         "failureReasons": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateBotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateBotRequestRequestTypeDef",
+UpdateBotResponseTypeDef = TypedDict(
+    "UpdateBotResponseTypeDef",
     {
         "botId": str,
         "botName": str,
+        "description": str,
+        "roleArn": str,
+        "dataPrivacy": DataPrivacyOutputTypeDef,
+        "idleSessionTTLInSeconds": int,
+        "botStatus": BotStatusType,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "botType": BotTypeType,
+        "botMembers": List[BotMemberOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateBotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotRequestRequestTypeDef",
+    {
+        "botName": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
         "idleSessionTTLInSeconds": int,
     },
 )
-_OptionalUpdateBotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateBotRequestRequestTypeDef",
+_OptionalCreateBotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotRequestRequestTypeDef",
     {
         "description": str,
+        "botTags": Mapping[str, str],
+        "testBotAliasTags": Mapping[str, str],
         "botType": BotTypeType,
         "botMembers": Sequence[BotMemberTypeDef],
     },
     total=False,
 )
 
-class UpdateBotRequestRequestTypeDef(
-    _RequiredUpdateBotRequestRequestTypeDef, _OptionalUpdateBotRequestRequestTypeDef
+class CreateBotRequestRequestTypeDef(
+    _RequiredCreateBotRequestRequestTypeDef, _OptionalCreateBotRequestRequestTypeDef
 ):
     pass
 
-UpdateBotResponseTypeDef = TypedDict(
-    "UpdateBotResponseTypeDef",
+_RequiredUpdateBotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBotRequestRequestTypeDef",
     {
         "botId": str,
         "botName": str,
-        "description": str,
         "roleArn": str,
         "dataPrivacy": DataPrivacyTypeDef,
         "idleSessionTTLInSeconds": int,
-        "botStatus": BotStatusType,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+    },
+)
+_OptionalUpdateBotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBotRequestRequestTypeDef",
+    {
+        "description": str,
         "botType": BotTypeType,
-        "botMembers": List[BotMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "botMembers": Sequence[BotMemberTypeDef],
     },
+    total=False,
 )
 
+class UpdateBotRequestRequestTypeDef(
+    _RequiredUpdateBotRequestRequestTypeDef, _OptionalUpdateBotRequestRequestTypeDef
+):
+    pass
+
 BotRecommendationResultStatisticsTypeDef = TypedDict(
     "BotRecommendationResultStatisticsTypeDef",
     {
         "intents": IntentStatisticsTypeDef,
         "slotTypes": SlotTypeStatisticsTypeDef,
     },
-    total=False,
 )
 
 ListBotRecommendationsResponseTypeDef = TypedDict(
     "ListBotRecommendationsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
@@ -2848,14 +3852,27 @@
     {
         "botSummaries": List[BotSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateBotVersionResponseTypeDef = TypedDict(
+    "CreateBotVersionResponseTypeDef",
+    {
+        "botId": str,
+        "description": str,
+        "botVersion": str,
+        "botVersionLocaleSpecification": Dict[str, BotVersionLocaleDetailsOutputTypeDef],
+        "botStatus": BotStatusType,
+        "creationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBotVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotVersionRequestRequestTypeDef",
     {
         "botId": str,
         "botVersionLocaleSpecification": Mapping[str, BotVersionLocaleDetailsTypeDef],
     },
 )
@@ -2868,27 +3885,14 @@
 )
 
 class CreateBotVersionRequestRequestTypeDef(
     _RequiredCreateBotVersionRequestRequestTypeDef, _OptionalCreateBotVersionRequestRequestTypeDef
 ):
     pass
 
-CreateBotVersionResponseTypeDef = TypedDict(
-    "CreateBotVersionResponseTypeDef",
-    {
-        "botId": str,
-        "description": str,
-        "botVersion": str,
-        "botVersionLocaleSpecification": Dict[str, BotVersionLocaleDetailsTypeDef],
-        "botStatus": BotStatusType,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBotVersionsRequestRequestTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalListBotVersionsRequestRequestTypeDef = TypedDict(
@@ -2976,14 +3980,24 @@
         "builtInSlotTypeSummaries": List[BuiltInSlotTypeSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ImageResponseCardOutputTypeDef = TypedDict(
+    "ImageResponseCardOutputTypeDef",
+    {
+        "title": str,
+        "subtitle": str,
+        "imageUrl": str,
+        "buttons": List[ButtonOutputTypeDef],
+    },
+)
+
 _RequiredImageResponseCardTypeDef = TypedDict(
     "_RequiredImageResponseCardTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardTypeDef = TypedDict(
@@ -2997,57 +4011,67 @@
 )
 
 class ImageResponseCardTypeDef(
     _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
 ):
     pass
 
+TextLogDestinationOutputTypeDef = TypedDict(
+    "TextLogDestinationOutputTypeDef",
+    {
+        "cloudWatch": CloudWatchLogGroupLogDestinationOutputTypeDef,
+    },
+)
+
 TextLogDestinationTypeDef = TypedDict(
     "TextLogDestinationTypeDef",
     {
         "cloudWatch": CloudWatchLogGroupLogDestinationTypeDef,
     },
 )
 
+CodeHookSpecificationOutputTypeDef = TypedDict(
+    "CodeHookSpecificationOutputTypeDef",
+    {
+        "lambdaCodeHook": LambdaCodeHookOutputTypeDef,
+    },
+)
+
 CodeHookSpecificationTypeDef = TypedDict(
     "CodeHookSpecificationTypeDef",
     {
         "lambdaCodeHook": LambdaCodeHookTypeDef,
     },
 )
 
+CompositeSlotTypeSettingOutputTypeDef = TypedDict(
+    "CompositeSlotTypeSettingOutputTypeDef",
+    {
+        "subSlots": List[SubSlotTypeCompositionOutputTypeDef],
+    },
+)
+
 CompositeSlotTypeSettingTypeDef = TypedDict(
     "CompositeSlotTypeSettingTypeDef",
     {
         "subSlots": Sequence[SubSlotTypeCompositionTypeDef],
     },
     total=False,
 )
 
-_RequiredConversationLevelTestResultItemTypeDef = TypedDict(
-    "_RequiredConversationLevelTestResultItemTypeDef",
+ConversationLevelTestResultItemTypeDef = TypedDict(
+    "ConversationLevelTestResultItemTypeDef",
     {
         "conversationId": str,
         "endToEndResult": TestResultMatchStatusType,
+        "speechTranscriptionResult": TestResultMatchStatusType,
         "intentClassificationResults": List[ConversationLevelIntentClassificationResultItemTypeDef],
         "slotResolutionResults": List[ConversationLevelSlotResolutionResultItemTypeDef],
     },
 )
-_OptionalConversationLevelTestResultItemTypeDef = TypedDict(
-    "_OptionalConversationLevelTestResultItemTypeDef",
-    {
-        "speechTranscriptionResult": TestResultMatchStatusType,
-    },
-    total=False,
-)
-
-class ConversationLevelTestResultItemTypeDef(
-    _RequiredConversationLevelTestResultItemTypeDef, _OptionalConversationLevelTestResultItemTypeDef
-):
-    pass
 
 _RequiredTestExecutionResultFilterByTypeDef = TypedDict(
     "_RequiredTestExecutionResultFilterByTypeDef",
     {
         "resultTypeFilter": TestResultTypeFilterType,
     },
 )
@@ -3060,14 +4084,24 @@
 )
 
 class TestExecutionResultFilterByTypeDef(
     _RequiredTestExecutionResultFilterByTypeDef, _OptionalTestExecutionResultFilterByTypeDef
 ):
     pass
 
+ConversationLogsDataSourceOutputTypeDef = TypedDict(
+    "ConversationLogsDataSourceOutputTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "filter": ConversationLogsDataSourceFilterByOutputTypeDef,
+    },
+)
+
 ConversationLogsDataSourceTypeDef = TypedDict(
     "ConversationLogsDataSourceTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "filter": ConversationLogsDataSourceFilterByTypeDef,
@@ -3077,19 +4111,18 @@
 IntentSummaryTypeDef = TypedDict(
     "IntentSummaryTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 _RequiredCreateResourcePolicyStatementRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourcePolicyStatementRequestRequestTypeDef",
     {
         "resourceArn": str,
         "statementId": str,
@@ -3109,14 +4142,21 @@
 
 class CreateResourcePolicyStatementRequestRequestTypeDef(
     _RequiredCreateResourcePolicyStatementRequestRequestTypeDef,
     _OptionalCreateResourcePolicyStatementRequestRequestTypeDef,
 ):
     pass
 
+LexTranscriptFilterOutputTypeDef = TypedDict(
+    "LexTranscriptFilterOutputTypeDef",
+    {
+        "dateRangeFilter": DateRangeFilterOutputTypeDef,
+    },
+)
+
 LexTranscriptFilterTypeDef = TypedDict(
     "LexTranscriptFilterTypeDef",
     {
         "dateRangeFilter": DateRangeFilterTypeDef,
     },
     total=False,
 )
@@ -3293,48 +4333,37 @@
     "DescribeBotVersionResponseTypeDef",
     {
         "botId": str,
         "botName": str,
         "botVersion": str,
         "description": str,
         "roleArn": str,
-        "dataPrivacy": DataPrivacyTypeDef,
+        "dataPrivacy": DataPrivacyOutputTypeDef,
         "idleSessionTTLInSeconds": int,
         "botStatus": BotStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
         "botType": BotTypeType,
-        "botMembers": List[BotMemberTypeDef],
+        "botMembers": List[BotMemberOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateBotRecommendationRequestRequestTypeDef = TypedDict(
-    "UpdateBotRecommendationRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "botRecommendationId": str,
-        "encryptionSetting": EncryptionSettingTypeDef,
-    },
-)
-
 DescribeTestSetResponseTypeDef = TypedDict(
     "DescribeTestSetResponseTypeDef",
     {
         "testSetId": str,
         "testSetName": str,
         "description": str,
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
-        "storageLocation": TestSetStorageLocationTypeDef,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestSetSummaryTypeDef = TypedDict(
@@ -3343,48 +4372,77 @@
         "testSetId": str,
         "testSetName": str,
         "description": str,
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
-        "storageLocation": TestSetStorageLocationTypeDef,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 UpdateTestSetResponseTypeDef = TypedDict(
     "UpdateTestSetResponseTypeDef",
     {
         "testSetId": str,
         "testSetName": str,
         "description": str,
         "modality": TestSetModalityType,
         "status": TestSetStatusType,
         "roleArn": str,
         "numTurns": int,
-        "storageLocation": TestSetStorageLocationTypeDef,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DialogStateOutputTypeDef = TypedDict(
+    "DialogStateOutputTypeDef",
+    {
+        "dialogAction": DialogActionOutputTypeDef,
+        "intent": IntentOverrideOutputTypeDef,
+        "sessionAttributes": Dict[str, str],
+    },
+)
+
 DialogStateTypeDef = TypedDict(
     "DialogStateTypeDef",
     {
         "dialogAction": DialogActionTypeDef,
         "intent": IntentOverrideTypeDef,
         "sessionAttributes": Mapping[str, str],
     },
     total=False,
 )
 
+UpdateBotRecommendationRequestRequestTypeDef = TypedDict(
+    "UpdateBotRecommendationRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "botRecommendationId": str,
+        "encryptionSetting": EncryptionSettingTypeDef,
+    },
+)
+
+ExportResourceSpecificationOutputTypeDef = TypedDict(
+    "ExportResourceSpecificationOutputTypeDef",
+    {
+        "botExportSpecification": BotExportSpecificationOutputTypeDef,
+        "botLocaleExportSpecification": BotLocaleExportSpecificationOutputTypeDef,
+        "customVocabularyExportSpecification": CustomVocabularyExportSpecificationOutputTypeDef,
+        "testSetExportSpecification": TestSetExportSpecificationOutputTypeDef,
+    },
+)
+
 ExportResourceSpecificationTypeDef = TypedDict(
     "ExportResourceSpecificationTypeDef",
     {
         "botExportSpecification": BotExportSpecificationTypeDef,
         "botLocaleExportSpecification": BotLocaleExportSpecificationTypeDef,
         "customVocabularyExportSpecification": CustomVocabularyExportSpecificationTypeDef,
         "testSetExportSpecification": TestSetExportSpecificationTypeDef,
@@ -3402,14 +4460,21 @@
         "maxResults": int,
         "nextToken": str,
         "localeId": str,
     },
     total=False,
 )
 
+GrammarSlotTypeSettingOutputTypeDef = TypedDict(
+    "GrammarSlotTypeSettingOutputTypeDef",
+    {
+        "source": GrammarSlotTypeSourceOutputTypeDef,
+    },
+)
+
 GrammarSlotTypeSettingTypeDef = TypedDict(
     "GrammarSlotTypeSettingTypeDef",
     {
         "source": GrammarSlotTypeSourceTypeDef,
     },
     total=False,
 )
@@ -3443,15 +4508,14 @@
 InputSessionStateSpecificationTypeDef = TypedDict(
     "InputSessionStateSpecificationTypeDef",
     {
         "sessionAttributes": Dict[str, str],
         "activeContexts": List[ActiveContextTypeDef],
         "runtimeHints": RuntimeHintsTypeDef,
     },
-    total=False,
 )
 
 IntentClassificationTestResultItemTypeDef = TypedDict(
     "IntentClassificationTestResultItemTypeDef",
     {
         "intentName": str,
         "multiTurnConversation": bool,
@@ -3479,27 +4543,71 @@
 )
 
 class ListIntentsRequestRequestTypeDef(
     _RequiredListIntentsRequestRequestTypeDef, _OptionalListIntentsRequestRequestTypeDef
 ):
     pass
 
+SessionSpecificationTypeDef = TypedDict(
+    "SessionSpecificationTypeDef",
+    {
+        "botAliasId": str,
+        "botVersion": str,
+        "localeId": str,
+        "channel": BotChannelTypeType,
+        "sessionId": str,
+        "conversationStartTime": datetime,
+        "conversationEndTime": datetime,
+        "conversationDurationSeconds": int,
+        "conversationEndState": ConversationEndStateType,
+        "mode": AnalyticsModalityType,
+        "numberOfTurns": int,
+        "invokedIntentSamples": List[InvokedIntentSampleTypeDef],
+        "originatingRequestId": str,
+    },
+)
+
 ListRecommendedIntentsResponseTypeDef = TypedDict(
     "ListRecommendedIntentsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationId": str,
         "summaryList": List[RecommendedIntentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredListSessionAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_RequiredListSessionAnalyticsDataRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+    },
+)
+_OptionalListSessionAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_OptionalListSessionAnalyticsDataRequestRequestTypeDef",
+    {
+        "sortBy": SessionDataSortByTypeDef,
+        "filters": Sequence[AnalyticsSessionFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListSessionAnalyticsDataRequestRequestTypeDef(
+    _RequiredListSessionAnalyticsDataRequestRequestTypeDef,
+    _OptionalListSessionAnalyticsDataRequestRequestTypeDef,
+):
+    pass
+
 _RequiredListSlotTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListSlotTypesRequestRequestTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
@@ -3573,46 +4681,92 @@
         "sortBy": TestSetSortByTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListUtteranceAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_RequiredListUtteranceAnalyticsDataRequestRequestTypeDef",
+    {
+        "botId": str,
+        "startDateTime": Union[datetime, str],
+        "endDateTime": Union[datetime, str],
+    },
+)
+_OptionalListUtteranceAnalyticsDataRequestRequestTypeDef = TypedDict(
+    "_OptionalListUtteranceAnalyticsDataRequestRequestTypeDef",
+    {
+        "sortBy": UtteranceDataSortByTypeDef,
+        "filters": Sequence[AnalyticsUtteranceFilterTypeDef],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListUtteranceAnalyticsDataRequestRequestTypeDef(
+    _RequiredListUtteranceAnalyticsDataRequestRequestTypeDef,
+    _OptionalListUtteranceAnalyticsDataRequestRequestTypeDef,
+):
+    pass
+
 OverallTestResultsTypeDef = TypedDict(
     "OverallTestResultsTypeDef",
     {
         "items": List[OverallTestResultItemTypeDef],
     },
 )
 
+UtteranceAggregationDurationOutputTypeDef = TypedDict(
+    "UtteranceAggregationDurationOutputTypeDef",
+    {
+        "relativeAggregationDuration": RelativeAggregationDurationOutputTypeDef,
+    },
+)
+
 UtteranceAggregationDurationTypeDef = TypedDict(
     "UtteranceAggregationDurationTypeDef",
     {
         "relativeAggregationDuration": RelativeAggregationDurationTypeDef,
     },
 )
 
 RuntimeHintDetailsTypeDef = TypedDict(
     "RuntimeHintDetailsTypeDef",
     {
         "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
-    total=False,
+)
+
+SlotTypeValueOutputTypeDef = TypedDict(
+    "SlotTypeValueOutputTypeDef",
+    {
+        "sampleValue": SampleValueOutputTypeDef,
+        "synonyms": List[SampleValueOutputTypeDef],
+    },
 )
 
 SlotTypeValueTypeDef = TypedDict(
     "SlotTypeValueTypeDef",
     {
         "sampleValue": SampleValueTypeDef,
         "synonyms": Sequence[SampleValueTypeDef],
     },
     total=False,
 )
 
+SlotDefaultValueSpecificationOutputTypeDef = TypedDict(
+    "SlotDefaultValueSpecificationOutputTypeDef",
+    {
+        "defaultValueList": List[SlotDefaultValueOutputTypeDef],
+    },
+)
+
 SlotDefaultValueSpecificationTypeDef = TypedDict(
     "SlotDefaultValueSpecificationTypeDef",
     {
         "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
@@ -3620,24 +4774,42 @@
     "SlotResolutionTestResultItemTypeDef",
     {
         "slotName": str,
         "resultCounts": SlotResolutionTestResultItemCountsTypeDef,
     },
 )
 
+SlotValueOverrideOutputTypeDef = TypedDict(
+    "SlotValueOverrideOutputTypeDef",
+    {
+        "shape": SlotShapeType,
+        "value": SlotValueOutputTypeDef,
+        "values": List[Dict[str, Any]],
+    },
+)
+
 SlotValueOverrideTypeDef = TypedDict(
     "SlotValueOverrideTypeDef",
     {
         "shape": SlotShapeType,
         "value": SlotValueTypeDef,
         "values": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+SlotValueSelectionSettingOutputTypeDef = TypedDict(
+    "SlotValueSelectionSettingOutputTypeDef",
+    {
+        "resolutionStrategy": SlotValueResolutionStrategyType,
+        "regexFilter": SlotValueRegexFilterOutputTypeDef,
+        "advancedRecognitionSetting": AdvancedRecognitionSettingOutputTypeDef,
+    },
+)
+
 _RequiredSlotValueSelectionSettingTypeDef = TypedDict(
     "_RequiredSlotValueSelectionSettingTypeDef",
     {
         "resolutionStrategy": SlotValueResolutionStrategyType,
     },
 )
 _OptionalSlotValueSelectionSettingTypeDef = TypedDict(
@@ -3658,74 +4830,132 @@
     "TestSetDiscrepancyErrorsTypeDef",
     {
         "intentDiscrepancies": List[TestSetIntentDiscrepancyItemTypeDef],
         "slotDiscrepancies": List[TestSetSlotDiscrepancyItemTypeDef],
     },
 )
 
+TestSetDiscrepancyReportResourceTargetOutputTypeDef = TypedDict(
+    "TestSetDiscrepancyReportResourceTargetOutputTypeDef",
+    {
+        "botAliasTarget": TestSetDiscrepancyReportBotAliasTargetOutputTypeDef,
+    },
+)
+
 TestSetDiscrepancyReportResourceTargetTypeDef = TypedDict(
     "TestSetDiscrepancyReportResourceTargetTypeDef",
     {
         "botAliasTarget": TestSetDiscrepancyReportBotAliasTargetTypeDef,
     },
     total=False,
 )
 
+TestSetImportResourceSpecificationOutputTypeDef = TypedDict(
+    "TestSetImportResourceSpecificationOutputTypeDef",
+    {
+        "testSetName": str,
+        "description": str,
+        "roleArn": str,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
+        "importInputLocation": TestSetImportInputLocationOutputTypeDef,
+        "modality": TestSetModalityType,
+        "testSetTags": Dict[str, str],
+    },
+)
+
 _RequiredTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_RequiredTestSetImportResourceSpecificationTypeDef",
     {
         "testSetName": str,
         "roleArn": str,
         "storageLocation": TestSetStorageLocationTypeDef,
         "importInputLocation": TestSetImportInputLocationTypeDef,
         "modality": TestSetModalityType,
     },
 )
 _OptionalTestSetImportResourceSpecificationTypeDef = TypedDict(
     "_OptionalTestSetImportResourceSpecificationTypeDef",
     {
         "description": str,
-        "testSetTags": Dict[str, str],
+        "testSetTags": Mapping[str, str],
     },
     total=False,
 )
 
 class TestSetImportResourceSpecificationTypeDef(
     _RequiredTestSetImportResourceSpecificationTypeDef,
     _OptionalTestSetImportResourceSpecificationTypeDef,
 ):
     pass
 
-_RequiredUserTurnOutputSpecificationTypeDef = TypedDict(
-    "_RequiredUserTurnOutputSpecificationTypeDef",
+UserTurnOutputSpecificationTypeDef = TypedDict(
+    "UserTurnOutputSpecificationTypeDef",
     {
         "intent": UserTurnIntentOutputTypeDef,
-    },
-)
-_OptionalUserTurnOutputSpecificationTypeDef = TypedDict(
-    "_OptionalUserTurnOutputSpecificationTypeDef",
-    {
         "activeContexts": List[ActiveContextTypeDef],
         "transcript": str,
     },
-    total=False,
 )
 
-class UserTurnOutputSpecificationTypeDef(
-    _RequiredUserTurnOutputSpecificationTypeDef, _OptionalUserTurnOutputSpecificationTypeDef
-):
-    pass
-
 UtteranceInputSpecificationTypeDef = TypedDict(
     "UtteranceInputSpecificationTypeDef",
     {
         "textInput": str,
         "audioInput": UtteranceAudioInputSpecificationTypeDef,
     },
-    total=False,
+)
+
+ListIntentMetricsResponseTypeDef = TypedDict(
+    "ListIntentMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsIntentResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListIntentStageMetricsResponseTypeDef = TypedDict(
+    "ListIntentStageMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsIntentStageResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSessionMetricsResponseTypeDef = TypedDict(
+    "ListSessionMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsSessionResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListUtteranceMetricsResponseTypeDef = TypedDict(
+    "ListUtteranceMetricsResponseTypeDef",
+    {
+        "botId": str,
+        "results": List[AnalyticsUtteranceResultTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PromptAttemptSpecificationOutputTypeDef = TypedDict(
+    "PromptAttemptSpecificationOutputTypeDef",
+    {
+        "allowInterrupt": bool,
+        "allowedInputTypes": AllowedInputTypesOutputTypeDef,
+        "audioAndDTMFInputSpecification": AudioAndDTMFInputSpecificationOutputTypeDef,
+        "textInputSpecification": TextInputSpecificationOutputTypeDef,
+    },
 )
 
 _RequiredPromptAttemptSpecificationTypeDef = TypedDict(
     "_RequiredPromptAttemptSpecificationTypeDef",
     {
         "allowedInputTypes": AllowedInputTypesTypeDef,
     },
@@ -3741,14 +4971,22 @@
 )
 
 class PromptAttemptSpecificationTypeDef(
     _RequiredPromptAttemptSpecificationTypeDef, _OptionalPromptAttemptSpecificationTypeDef
 ):
     pass
 
+AudioLogSettingOutputTypeDef = TypedDict(
+    "AudioLogSettingOutputTypeDef",
+    {
+        "enabled": bool,
+        "destination": AudioLogDestinationOutputTypeDef,
+    },
+)
+
 AudioLogSettingTypeDef = TypedDict(
     "AudioLogSettingTypeDef",
     {
         "enabled": bool,
         "destination": AudioLogDestinationTypeDef,
     },
 )
@@ -3758,51 +4996,29 @@
     {
         "testExecutionId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "testExecutionStatus": TestExecutionStatusType,
         "testSetId": str,
         "testSetName": str,
-        "target": TestExecutionTargetTypeDef,
+        "target": TestExecutionTargetOutputTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
         "failureReasons": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartTestExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartTestExecutionRequestRequestTypeDef",
-    {
-        "testSetId": str,
-        "target": TestExecutionTargetTypeDef,
-        "apiMode": TestExecutionApiModeType,
-    },
-)
-_OptionalStartTestExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartTestExecutionRequestRequestTypeDef",
-    {
-        "testExecutionModality": TestExecutionModalityType,
-    },
-    total=False,
-)
-
-class StartTestExecutionRequestRequestTypeDef(
-    _RequiredStartTestExecutionRequestRequestTypeDef,
-    _OptionalStartTestExecutionRequestRequestTypeDef,
-):
-    pass
-
 StartTestExecutionResponseTypeDef = TypedDict(
     "StartTestExecutionResponseTypeDef",
     {
         "testExecutionId": str,
         "creationDateTime": datetime,
         "testSetId": str,
-        "target": TestExecutionTargetTypeDef,
+        "target": TestExecutionTargetOutputTypeDef,
         "apiMode": TestExecutionApiModeType,
         "testExecutionModality": TestExecutionModalityType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestExecutionSummaryTypeDef = TypedDict(
@@ -3810,50 +5026,105 @@
     {
         "testExecutionId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "testExecutionStatus": TestExecutionStatusType,
         "testSetId": str,
         "testSetName": str,
+        "target": TestExecutionTargetOutputTypeDef,
+        "apiMode": TestExecutionApiModeType,
+        "testExecutionModality": TestExecutionModalityType,
+    },
+)
+
+_RequiredStartTestExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartTestExecutionRequestRequestTypeDef",
+    {
+        "testSetId": str,
         "target": TestExecutionTargetTypeDef,
         "apiMode": TestExecutionApiModeType,
+    },
+)
+_OptionalStartTestExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartTestExecutionRequestRequestTypeDef",
+    {
         "testExecutionModality": TestExecutionModalityType,
     },
     total=False,
 )
 
+class StartTestExecutionRequestRequestTypeDef(
+    _RequiredStartTestExecutionRequestRequestTypeDef,
+    _OptionalStartTestExecutionRequestRequestTypeDef,
+):
+    pass
+
 BotRecommendationResultsTypeDef = TypedDict(
     "BotRecommendationResultsTypeDef",
     {
         "botLocaleExportUrl": str,
         "associatedTranscriptsUrl": str,
         "statistics": BotRecommendationResultStatisticsTypeDef,
     },
-    total=False,
+)
+
+MessageOutputTypeDef = TypedDict(
+    "MessageOutputTypeDef",
+    {
+        "plainTextMessage": PlainTextMessageOutputTypeDef,
+        "customPayload": CustomPayloadOutputTypeDef,
+        "ssmlMessage": SSMLMessageOutputTypeDef,
+        "imageResponseCard": ImageResponseCardOutputTypeDef,
+    },
+)
+
+UtteranceBotResponseTypeDef = TypedDict(
+    "UtteranceBotResponseTypeDef",
+    {
+        "content": str,
+        "contentType": UtteranceContentTypeType,
+        "imageResponseCard": ImageResponseCardOutputTypeDef,
+    },
 )
 
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "plainTextMessage": PlainTextMessageTypeDef,
         "customPayload": CustomPayloadTypeDef,
         "ssmlMessage": SSMLMessageTypeDef,
         "imageResponseCard": ImageResponseCardTypeDef,
     },
     total=False,
 )
 
+TextLogSettingOutputTypeDef = TypedDict(
+    "TextLogSettingOutputTypeDef",
+    {
+        "enabled": bool,
+        "destination": TextLogDestinationOutputTypeDef,
+    },
+)
+
 TextLogSettingTypeDef = TypedDict(
     "TextLogSettingTypeDef",
     {
         "enabled": bool,
         "destination": TextLogDestinationTypeDef,
     },
 )
 
+BotAliasLocaleSettingsOutputTypeDef = TypedDict(
+    "BotAliasLocaleSettingsOutputTypeDef",
+    {
+        "enabled": bool,
+        "codeHookSpecification": CodeHookSpecificationOutputTypeDef,
+    },
+)
+
 _RequiredBotAliasLocaleSettingsTypeDef = TypedDict(
     "_RequiredBotAliasLocaleSettingsTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalBotAliasLocaleSettingsTypeDef = TypedDict(
@@ -3894,14 +5165,21 @@
 
 class ListTestExecutionResultItemsRequestRequestTypeDef(
     _RequiredListTestExecutionResultItemsRequestRequestTypeDef,
     _OptionalListTestExecutionResultItemsRequestRequestTypeDef,
 ):
     pass
 
+TestSetGenerationDataSourceOutputTypeDef = TypedDict(
+    "TestSetGenerationDataSourceOutputTypeDef",
+    {
+        "conversationLogsDataSource": ConversationLogsDataSourceOutputTypeDef,
+    },
+)
+
 TestSetGenerationDataSourceTypeDef = TypedDict(
     "TestSetGenerationDataSourceTypeDef",
     {
         "conversationLogsDataSource": ConversationLogsDataSourceTypeDef,
     },
     total=False,
 )
@@ -3914,14 +5192,21 @@
         "localeId": str,
         "intentSummaries": List[IntentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
+    {
+        "lexTranscriptFilter": LexTranscriptFilterOutputTypeDef,
+    },
+)
+
 TranscriptFilterTypeDef = TypedDict(
     "TranscriptFilterTypeDef",
     {
         "lexTranscriptFilter": LexTranscriptFilterTypeDef,
     },
     total=False,
 )
@@ -3931,87 +5216,93 @@
     {
         "testSets": List[TestSetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateExportRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateExportRequestRequestTypeDef",
-    {
-        "resourceSpecification": ExportResourceSpecificationTypeDef,
-        "fileFormat": ImportExportFileFormatType,
-    },
-)
-_OptionalCreateExportRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateExportRequestRequestTypeDef",
-    {
-        "filePassword": str,
-    },
-    total=False,
-)
-
-class CreateExportRequestRequestTypeDef(
-    _RequiredCreateExportRequestRequestTypeDef, _OptionalCreateExportRequestRequestTypeDef
-):
-    pass
-
 CreateExportResponseTypeDef = TypedDict(
     "CreateExportResponseTypeDef",
     {
         "exportId": str,
-        "resourceSpecification": ExportResourceSpecificationTypeDef,
+        "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExportResponseTypeDef = TypedDict(
     "DescribeExportResponseTypeDef",
     {
         "exportId": str,
-        "resourceSpecification": ExportResourceSpecificationTypeDef,
+        "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "failureReasons": List[str],
         "downloadUrl": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "exportId": str,
-        "resourceSpecification": ExportResourceSpecificationTypeDef,
+        "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
     },
-    total=False,
 )
 
 UpdateExportResponseTypeDef = TypedDict(
     "UpdateExportResponseTypeDef",
     {
         "exportId": str,
-        "resourceSpecification": ExportResourceSpecificationTypeDef,
+        "resourceSpecification": ExportResourceSpecificationOutputTypeDef,
         "fileFormat": ImportExportFileFormatType,
         "exportStatus": ExportStatusType,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateExportRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateExportRequestRequestTypeDef",
+    {
+        "resourceSpecification": ExportResourceSpecificationTypeDef,
+        "fileFormat": ImportExportFileFormatType,
+    },
+)
+_OptionalCreateExportRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateExportRequestRequestTypeDef",
+    {
+        "filePassword": str,
+    },
+    total=False,
+)
+
+class CreateExportRequestRequestTypeDef(
+    _RequiredCreateExportRequestRequestTypeDef, _OptionalCreateExportRequestRequestTypeDef
+):
+    pass
+
+ExternalSourceSettingOutputTypeDef = TypedDict(
+    "ExternalSourceSettingOutputTypeDef",
+    {
+        "grammarSlotTypeSetting": GrammarSlotTypeSettingOutputTypeDef,
+    },
+)
+
 ExternalSourceSettingTypeDef = TypedDict(
     "ExternalSourceSettingTypeDef",
     {
         "grammarSlotTypeSetting": GrammarSlotTypeSettingTypeDef,
     },
     total=False,
 )
@@ -4019,14 +5310,41 @@
 IntentClassificationTestResultsTypeDef = TypedDict(
     "IntentClassificationTestResultsTypeDef",
     {
         "items": List[IntentClassificationTestResultItemTypeDef],
     },
 )
 
+ListSessionAnalyticsDataResponseTypeDef = TypedDict(
+    "ListSessionAnalyticsDataResponseTypeDef",
+    {
+        "botId": str,
+        "nextToken": str,
+        "sessions": List[SessionSpecificationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAggregatedUtterancesResponseTypeDef = TypedDict(
+    "ListAggregatedUtterancesResponseTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "botVersion": str,
+        "localeId": str,
+        "aggregationDuration": UtteranceAggregationDurationOutputTypeDef,
+        "aggregationWindowStartTime": datetime,
+        "aggregationWindowEndTime": datetime,
+        "aggregationLastRefreshedDateTime": datetime,
+        "aggregatedUtterancesSummaries": List[AggregatedUtterancesSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListAggregatedUtterancesRequestRequestTypeDef = TypedDict(
     "_RequiredListAggregatedUtterancesRequestRequestTypeDef",
     {
         "botId": str,
         "localeId": str,
         "aggregationDuration": UtteranceAggregationDurationTypeDef,
     },
@@ -4046,115 +5364,133 @@
 
 class ListAggregatedUtterancesRequestRequestTypeDef(
     _RequiredListAggregatedUtterancesRequestRequestTypeDef,
     _OptionalListAggregatedUtterancesRequestRequestTypeDef,
 ):
     pass
 
-ListAggregatedUtterancesResponseTypeDef = TypedDict(
-    "ListAggregatedUtterancesResponseTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "botVersion": str,
-        "localeId": str,
-        "aggregationDuration": UtteranceAggregationDurationTypeDef,
-        "aggregationWindowStartTime": datetime,
-        "aggregationWindowEndTime": datetime,
-        "aggregationLastRefreshedDateTime": datetime,
-        "aggregatedUtterancesSummaries": List[AggregatedUtterancesSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IntentLevelSlotResolutionTestResultItemTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultItemTypeDef",
     {
         "intentName": str,
         "multiTurnConversation": bool,
         "slotResolutionResults": List[SlotResolutionTestResultItemTypeDef],
     },
 )
 
-CreateTestSetDiscrepancyReportRequestRequestTypeDef = TypedDict(
-    "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
-    {
-        "testSetId": str,
-        "target": TestSetDiscrepancyReportResourceTargetTypeDef,
-    },
-)
-
 CreateTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "CreateTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
         "creationDateTime": datetime,
         "testSetId": str,
-        "target": TestSetDiscrepancyReportResourceTargetTypeDef,
+        "target": TestSetDiscrepancyReportResourceTargetOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTestSetDiscrepancyReportResponseTypeDef = TypedDict(
     "DescribeTestSetDiscrepancyReportResponseTypeDef",
     {
         "testSetDiscrepancyReportId": str,
         "testSetId": str,
         "creationDateTime": datetime,
-        "target": TestSetDiscrepancyReportResourceTargetTypeDef,
+        "target": TestSetDiscrepancyReportResourceTargetOutputTypeDef,
         "testSetDiscrepancyReportStatus": TestSetDiscrepancyReportStatusType,
         "lastUpdatedDataTime": datetime,
         "testSetDiscrepancyTopErrors": TestSetDiscrepancyErrorsTypeDef,
         "testSetDiscrepancyRawOutputUrl": str,
         "failureReasons": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateTestSetDiscrepancyReportRequestRequestTypeDef = TypedDict(
+    "CreateTestSetDiscrepancyReportRequestRequestTypeDef",
+    {
+        "testSetId": str,
+        "target": TestSetDiscrepancyReportResourceTargetTypeDef,
+    },
+)
+
+ImportResourceSpecificationOutputTypeDef = TypedDict(
+    "ImportResourceSpecificationOutputTypeDef",
+    {
+        "botImportSpecification": BotImportSpecificationOutputTypeDef,
+        "botLocaleImportSpecification": BotLocaleImportSpecificationOutputTypeDef,
+        "customVocabularyImportSpecification": CustomVocabularyImportSpecificationOutputTypeDef,
+        "testSetImportResourceSpecification": TestSetImportResourceSpecificationOutputTypeDef,
+    },
+)
+
 ImportResourceSpecificationTypeDef = TypedDict(
     "ImportResourceSpecificationTypeDef",
     {
         "botImportSpecification": BotImportSpecificationTypeDef,
         "botLocaleImportSpecification": BotLocaleImportSpecificationTypeDef,
         "customVocabularyImportSpecification": CustomVocabularyImportSpecificationTypeDef,
         "testSetImportResourceSpecification": TestSetImportResourceSpecificationTypeDef,
     },
     total=False,
 )
 
-_RequiredUserTurnInputSpecificationTypeDef = TypedDict(
-    "_RequiredUserTurnInputSpecificationTypeDef",
+UserTurnInputSpecificationTypeDef = TypedDict(
+    "UserTurnInputSpecificationTypeDef",
     {
         "utteranceInput": UtteranceInputSpecificationTypeDef,
-    },
-)
-_OptionalUserTurnInputSpecificationTypeDef = TypedDict(
-    "_OptionalUserTurnInputSpecificationTypeDef",
-    {
         "requestAttributes": Dict[str, str],
         "sessionState": InputSessionStateSpecificationTypeDef,
     },
-    total=False,
 )
 
-class UserTurnInputSpecificationTypeDef(
-    _RequiredUserTurnInputSpecificationTypeDef, _OptionalUserTurnInputSpecificationTypeDef
-):
-    pass
-
 ListTestExecutionsResponseTypeDef = TypedDict(
     "ListTestExecutionsResponseTypeDef",
     {
         "testExecutions": List[TestExecutionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MessageGroupOutputTypeDef = TypedDict(
+    "MessageGroupOutputTypeDef",
+    {
+        "message": MessageOutputTypeDef,
+        "variations": List[MessageOutputTypeDef],
+    },
+)
+
+UtteranceSpecificationTypeDef = TypedDict(
+    "UtteranceSpecificationTypeDef",
+    {
+        "botAliasId": str,
+        "botVersion": str,
+        "localeId": str,
+        "sessionId": str,
+        "channel": BotChannelTypeType,
+        "mode": AnalyticsModalityType,
+        "conversationStartTime": datetime,
+        "conversationEndTime": datetime,
+        "utterance": str,
+        "utteranceTimestamp": datetime,
+        "audioVoiceDurationMillis": int,
+        "utteranceUnderstood": bool,
+        "inputType": str,
+        "outputType": str,
+        "associatedIntentName": str,
+        "associatedSlotName": str,
+        "intentState": IntentStateType,
+        "dialogActionType": str,
+        "botResponseAudioVoiceId": str,
+        "slotsFilledInSession": str,
+        "utteranceRequestId": str,
+        "botResponses": List[UtteranceBotResponseTypeDef],
+    },
+)
+
 _RequiredMessageGroupTypeDef = TypedDict(
     "_RequiredMessageGroupTypeDef",
     {
         "message": MessageTypeDef,
     },
 )
 _OptionalMessageGroupTypeDef = TypedDict(
@@ -4164,14 +5500,22 @@
     },
     total=False,
 )
 
 class MessageGroupTypeDef(_RequiredMessageGroupTypeDef, _OptionalMessageGroupTypeDef):
     pass
 
+ConversationLogSettingsOutputTypeDef = TypedDict(
+    "ConversationLogSettingsOutputTypeDef",
+    {
+        "textLogSettings": List[TextLogSettingOutputTypeDef],
+        "audioLogSettings": List[AudioLogSettingOutputTypeDef],
+    },
+)
+
 ConversationLogSettingsTypeDef = TypedDict(
     "ConversationLogSettingsTypeDef",
     {
         "textLogSettings": Sequence[TextLogSettingTypeDef],
         "audioLogSettings": Sequence[AudioLogSettingTypeDef],
     },
     total=False,
@@ -4182,23 +5526,39 @@
     {
         "testSetGenerationId": str,
         "testSetGenerationStatus": TestSetGenerationStatusType,
         "failureReasons": List[str],
         "testSetId": str,
         "testSetName": str,
         "description": str,
-        "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
         "roleArn": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StartTestSetGenerationResponseTypeDef = TypedDict(
+    "StartTestSetGenerationResponseTypeDef",
+    {
+        "testSetGenerationId": str,
+        "creationDateTime": datetime,
+        "testSetGenerationStatus": TestSetGenerationStatusType,
+        "testSetName": str,
+        "description": str,
+        "storageLocation": TestSetStorageLocationOutputTypeDef,
+        "generationDataSource": TestSetGenerationDataSourceOutputTypeDef,
+        "roleArn": str,
+        "testSetTags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartTestSetGenerationRequestRequestTypeDef = TypedDict(
     "_RequiredStartTestSetGenerationRequestRequestTypeDef",
     {
         "testSetName": str,
         "storageLocation": TestSetStorageLocationTypeDef,
         "generationDataSource": TestSetGenerationDataSourceTypeDef,
         "roleArn": str,
@@ -4215,27 +5575,22 @@
 
 class StartTestSetGenerationRequestRequestTypeDef(
     _RequiredStartTestSetGenerationRequestRequestTypeDef,
     _OptionalStartTestSetGenerationRequestRequestTypeDef,
 ):
     pass
 
-StartTestSetGenerationResponseTypeDef = TypedDict(
-    "StartTestSetGenerationResponseTypeDef",
+S3BucketTranscriptSourceOutputTypeDef = TypedDict(
+    "S3BucketTranscriptSourceOutputTypeDef",
     {
-        "testSetGenerationId": str,
-        "creationDateTime": datetime,
-        "testSetGenerationStatus": TestSetGenerationStatusType,
-        "testSetName": str,
-        "description": str,
-        "storageLocation": TestSetStorageLocationTypeDef,
-        "generationDataSource": TestSetGenerationDataSourceTypeDef,
-        "roleArn": str,
-        "testSetTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "s3BucketName": str,
+        "pathFormat": PathFormatOutputTypeDef,
+        "transcriptFormat": Literal["Lex"],
+        "transcriptFilter": TranscriptFilterOutputTypeDef,
+        "kmsKeyArn": str,
     },
 )
 
 _RequiredS3BucketTranscriptSourceTypeDef = TypedDict(
     "_RequiredS3BucketTranscriptSourceTypeDef",
     {
         "s3BucketName": str,
@@ -4265,151 +5620,163 @@
         "exportSummaries": List[ExportSummaryTypeDef],
         "nextToken": str,
         "localeId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotTypeRequestRequestTypeDef",
+CreateSlotTypeResponseTypeDef = TypedDict(
+    "CreateSlotTypeResponseTypeDef",
     {
+        "slotTypeId": str,
         "slotTypeName": str,
+        "description": str,
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingOutputTypeDef,
+        "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
+        "creationDateTime": datetime,
+        "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotTypeRequestRequestTypeDef",
-    {
-        "description": str,
-        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
-        "parentSlotTypeSignature": str,
-        "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
-    },
-    total=False,
-)
 
-class CreateSlotTypeRequestRequestTypeDef(
-    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
-):
-    pass
-
-CreateSlotTypeResponseTypeDef = TypedDict(
-    "CreateSlotTypeResponseTypeDef",
+DescribeSlotTypeResponseTypeDef = TypedDict(
+    "DescribeSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingOutputTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
-        "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
+        "lastUpdatedDateTime": datetime,
+        "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSlotTypeResponseTypeDef = TypedDict(
-    "DescribeSlotTypeResponseTypeDef",
+UpdateSlotTypeResponseTypeDef = TypedDict(
+    "UpdateSlotTypeResponseTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
         "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
+        "slotTypeValues": List[SlotTypeValueOutputTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingOutputTypeDef,
         "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "externalSourceSetting": ExternalSourceSettingTypeDef,
-        "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
+        "externalSourceSetting": ExternalSourceSettingOutputTypeDef,
+        "compositeSlotTypeSetting": CompositeSlotTypeSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
+_RequiredCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotTypeRequestRequestTypeDef",
     {
-        "slotTypeId": str,
         "slotTypeName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
+_OptionalCreateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotTypeRequestRequestTypeDef",
     {
         "description": str,
         "slotTypeValues": Sequence[SlotTypeValueTypeDef],
         "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
         "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
     },
     total=False,
 )
 
-class UpdateSlotTypeRequestRequestTypeDef(
-    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
+class CreateSlotTypeRequestRequestTypeDef(
+    _RequiredCreateSlotTypeRequestRequestTypeDef, _OptionalCreateSlotTypeRequestRequestTypeDef
 ):
     pass
 
-UpdateSlotTypeResponseTypeDef = TypedDict(
-    "UpdateSlotTypeResponseTypeDef",
+_RequiredUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotTypeRequestRequestTypeDef",
     {
         "slotTypeId": str,
         "slotTypeName": str,
-        "description": str,
-        "slotTypeValues": List[SlotTypeValueTypeDef],
-        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
-        "parentSlotTypeSignature": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+    },
+)
+_OptionalUpdateSlotTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotTypeRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeValues": Sequence[SlotTypeValueTypeDef],
+        "valueSelectionSetting": SlotValueSelectionSettingTypeDef,
+        "parentSlotTypeSignature": str,
         "externalSourceSetting": ExternalSourceSettingTypeDef,
         "compositeSlotTypeSetting": CompositeSlotTypeSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+class UpdateSlotTypeRequestRequestTypeDef(
+    _RequiredUpdateSlotTypeRequestRequestTypeDef, _OptionalUpdateSlotTypeRequestRequestTypeDef
+):
+    pass
+
 IntentLevelSlotResolutionTestResultsTypeDef = TypedDict(
     "IntentLevelSlotResolutionTestResultsTypeDef",
     {
         "items": List[IntentLevelSlotResolutionTestResultItemTypeDef],
     },
 )
 
 DescribeImportResponseTypeDef = TypedDict(
     "DescribeImportResponseTypeDef",
     {
         "importId": str,
-        "resourceSpecification": ImportResourceSpecificationTypeDef,
+        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
         "importedResourceId": str,
         "importedResourceName": str,
         "mergeStrategy": MergeStrategyType,
         "importStatus": ImportStatusType,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StartImportResponseTypeDef = TypedDict(
+    "StartImportResponseTypeDef",
+    {
+        "importId": str,
+        "resourceSpecification": ImportResourceSpecificationOutputTypeDef,
+        "mergeStrategy": MergeStrategyType,
+        "importStatus": ImportStatusType,
+        "creationDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
         "importId": str,
         "resourceSpecification": ImportResourceSpecificationTypeDef,
         "mergeStrategy": MergeStrategyType,
     },
@@ -4423,58 +5790,96 @@
 )
 
 class StartImportRequestRequestTypeDef(
     _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
 ):
     pass
 
-StartImportResponseTypeDef = TypedDict(
-    "StartImportResponseTypeDef",
-    {
-        "importId": str,
-        "resourceSpecification": ImportResourceSpecificationTypeDef,
-        "mergeStrategy": MergeStrategyType,
-        "importStatus": ImportStatusType,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUserTurnResultTypeDef = TypedDict(
-    "_RequiredUserTurnResultTypeDef",
+UserTurnResultTypeDef = TypedDict(
+    "UserTurnResultTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expectedOutput": UserTurnOutputSpecificationTypeDef,
-    },
-)
-_OptionalUserTurnResultTypeDef = TypedDict(
-    "_OptionalUserTurnResultTypeDef",
-    {
         "actualOutput": UserTurnOutputSpecificationTypeDef,
         "errorDetails": ExecutionErrorDetailsTypeDef,
         "endToEndResult": TestResultMatchStatusType,
         "intentMatchResult": TestResultMatchStatusType,
         "slotMatchResult": TestResultMatchStatusType,
         "speechTranscriptionResult": TestResultMatchStatusType,
         "conversationLevelResult": ConversationLevelResultDetailTypeDef,
     },
-    total=False,
 )
 
-class UserTurnResultTypeDef(_RequiredUserTurnResultTypeDef, _OptionalUserTurnResultTypeDef):
-    pass
-
 UserTurnSpecificationTypeDef = TypedDict(
     "UserTurnSpecificationTypeDef",
     {
         "input": UserTurnInputSpecificationTypeDef,
         "expected": UserTurnOutputSpecificationTypeDef,
     },
 )
 
+FulfillmentStartResponseSpecificationOutputTypeDef = TypedDict(
+    "FulfillmentStartResponseSpecificationOutputTypeDef",
+    {
+        "delayInSeconds": int,
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "allowInterrupt": bool,
+    },
+)
+
+FulfillmentUpdateResponseSpecificationOutputTypeDef = TypedDict(
+    "FulfillmentUpdateResponseSpecificationOutputTypeDef",
+    {
+        "frequencyInSeconds": int,
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "allowInterrupt": bool,
+    },
+)
+
+PromptSpecificationOutputTypeDef = TypedDict(
+    "PromptSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "maxRetries": int,
+        "allowInterrupt": bool,
+        "messageSelectionStrategy": MessageSelectionStrategyType,
+        "promptAttemptsSpecification": Dict[
+            PromptAttemptType, PromptAttemptSpecificationOutputTypeDef
+        ],
+    },
+)
+
+ResponseSpecificationOutputTypeDef = TypedDict(
+    "ResponseSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "allowInterrupt": bool,
+    },
+)
+
+StillWaitingResponseSpecificationOutputTypeDef = TypedDict(
+    "StillWaitingResponseSpecificationOutputTypeDef",
+    {
+        "messageGroups": List[MessageGroupOutputTypeDef],
+        "frequencyInSeconds": int,
+        "timeoutInSeconds": int,
+        "allowInterrupt": bool,
+    },
+)
+
+ListUtteranceAnalyticsDataResponseTypeDef = TypedDict(
+    "ListUtteranceAnalyticsDataResponseTypeDef",
+    {
+        "botId": str,
+        "nextToken": str,
+        "utterances": List[UtteranceSpecificationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFulfillmentStartResponseSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentStartResponseSpecificationTypeDef",
     {
         "delayInSeconds": int,
         "messageGroups": Sequence[MessageGroupTypeDef],
     },
 )
@@ -4574,49 +5979,24 @@
 
 class StillWaitingResponseSpecificationTypeDef(
     _RequiredStillWaitingResponseSpecificationTypeDef,
     _OptionalStillWaitingResponseSpecificationTypeDef,
 ):
     pass
 
-_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBotAliasRequestRequestTypeDef",
-    {
-        "botAliasName": str,
-        "botId": str,
-    },
-)
-_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBotAliasRequestRequestTypeDef",
-    {
-        "description": str,
-        "botVersion": str,
-        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateBotAliasRequestRequestTypeDef(
-    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
-):
-    pass
-
 CreateBotAliasResponseTypeDef = TypedDict(
     "CreateBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsOutputTypeDef],
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4624,67 +6004,99 @@
 DescribeBotAliasResponseTypeDef = TypedDict(
     "DescribeBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
-        "conversationLogSettings": ConversationLogSettingsTypeDef,
-        "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsOutputTypeDef],
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
         "botAliasHistoryEvents": List[BotAliasHistoryEventTypeDef],
         "botAliasStatus": BotAliasStatusType,
         "botId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
         "parentBotNetworks": List[ParentBotNetworkTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateBotAliasRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateBotAliasRequestRequestTypeDef",
+UpdateBotAliasResponseTypeDef = TypedDict(
+    "UpdateBotAliasResponseTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
+        "description": str,
+        "botVersion": str,
+        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsOutputTypeDef],
+        "conversationLogSettings": ConversationLogSettingsOutputTypeDef,
+        "sentimentAnalysisSettings": SentimentAnalysisSettingsOutputTypeDef,
+        "botAliasStatus": BotAliasStatusType,
         "botId": str,
+        "creationDateTime": datetime,
+        "lastUpdatedDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalUpdateBotAliasRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateBotAliasRequestRequestTypeDef",
+
+_RequiredCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBotAliasRequestRequestTypeDef",
+    {
+        "botAliasName": str,
+        "botId": str,
+    },
+)
+_OptionalCreateBotAliasRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBotAliasRequestRequestTypeDef",
     {
         "description": str,
         "botVersion": str,
         "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
         "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class UpdateBotAliasRequestRequestTypeDef(
-    _RequiredUpdateBotAliasRequestRequestTypeDef, _OptionalUpdateBotAliasRequestRequestTypeDef
+class CreateBotAliasRequestRequestTypeDef(
+    _RequiredCreateBotAliasRequestRequestTypeDef, _OptionalCreateBotAliasRequestRequestTypeDef
 ):
     pass
 
-UpdateBotAliasResponseTypeDef = TypedDict(
-    "UpdateBotAliasResponseTypeDef",
+_RequiredUpdateBotAliasRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateBotAliasRequestRequestTypeDef",
     {
         "botAliasId": str,
         "botAliasName": str,
+        "botId": str,
+    },
+)
+_OptionalUpdateBotAliasRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateBotAliasRequestRequestTypeDef",
+    {
         "description": str,
         "botVersion": str,
-        "botAliasLocaleSettings": Dict[str, BotAliasLocaleSettingsTypeDef],
+        "botAliasLocaleSettings": Mapping[str, BotAliasLocaleSettingsTypeDef],
         "conversationLogSettings": ConversationLogSettingsTypeDef,
         "sentimentAnalysisSettings": SentimentAnalysisSettingsTypeDef,
-        "botAliasStatus": BotAliasStatusType,
-        "botId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+    total=False,
+)
+
+class UpdateBotAliasRequestRequestTypeDef(
+    _RequiredUpdateBotAliasRequestRequestTypeDef, _OptionalUpdateBotAliasRequestRequestTypeDef
+):
+    pass
+
+TranscriptSourceSettingOutputTypeDef = TypedDict(
+    "TranscriptSourceSettingOutputTypeDef",
+    {
+        "s3BucketTranscriptSource": S3BucketTranscriptSourceOutputTypeDef,
     },
 )
 
 TranscriptSourceSettingTypeDef = TypedDict(
     "TranscriptSourceSettingTypeDef",
     {
         "s3BucketTranscriptSource": S3BucketTranscriptSourceTypeDef,
@@ -4694,24 +6106,73 @@
 
 TestSetTurnResultTypeDef = TypedDict(
     "TestSetTurnResultTypeDef",
     {
         "agent": AgentTurnResultTypeDef,
         "user": UserTurnResultTypeDef,
     },
-    total=False,
 )
 
 TurnSpecificationTypeDef = TypedDict(
     "TurnSpecificationTypeDef",
     {
         "agentTurn": AgentTurnSpecificationTypeDef,
         "userTurn": UserTurnSpecificationTypeDef,
     },
-    total=False,
+)
+
+FulfillmentUpdatesSpecificationOutputTypeDef = TypedDict(
+    "FulfillmentUpdatesSpecificationOutputTypeDef",
+    {
+        "active": bool,
+        "startResponse": FulfillmentStartResponseSpecificationOutputTypeDef,
+        "updateResponse": FulfillmentUpdateResponseSpecificationOutputTypeDef,
+        "timeoutInSeconds": int,
+    },
+)
+
+SlotSummaryTypeDef = TypedDict(
+    "SlotSummaryTypeDef",
+    {
+        "slotId": str,
+        "slotName": str,
+        "description": str,
+        "slotConstraint": SlotConstraintType,
+        "slotTypeId": str,
+        "valueElicitationPromptSpecification": PromptSpecificationOutputTypeDef,
+        "lastUpdatedDateTime": datetime,
+    },
+)
+
+ConditionalBranchOutputTypeDef = TypedDict(
+    "ConditionalBranchOutputTypeDef",
+    {
+        "name": str,
+        "condition": ConditionOutputTypeDef,
+        "nextStep": DialogStateOutputTypeDef,
+        "response": ResponseSpecificationOutputTypeDef,
+    },
+)
+
+DefaultConditionalBranchOutputTypeDef = TypedDict(
+    "DefaultConditionalBranchOutputTypeDef",
+    {
+        "nextStep": DialogStateOutputTypeDef,
+        "response": ResponseSpecificationOutputTypeDef,
+    },
+)
+
+WaitAndContinueSpecificationOutputTypeDef = TypedDict(
+    "WaitAndContinueSpecificationOutputTypeDef",
+    {
+        "waitingResponse": ResponseSpecificationOutputTypeDef,
+        "continueResponse": ResponseSpecificationOutputTypeDef,
+        "stillWaitingResponse": StillWaitingResponseSpecificationOutputTypeDef,
+        "active": bool,
+    },
 )
 
 _RequiredFulfillmentUpdatesSpecificationTypeDef = TypedDict(
     "_RequiredFulfillmentUpdatesSpecificationTypeDef",
     {
         "active": bool,
     },
@@ -4727,28 +6188,14 @@
 )
 
 class FulfillmentUpdatesSpecificationTypeDef(
     _RequiredFulfillmentUpdatesSpecificationTypeDef, _OptionalFulfillmentUpdatesSpecificationTypeDef
 ):
     pass
 
-SlotSummaryTypeDef = TypedDict(
-    "SlotSummaryTypeDef",
-    {
-        "slotId": str,
-        "slotName": str,
-        "description": str,
-        "slotConstraint": SlotConstraintType,
-        "slotTypeId": str,
-        "valueElicitationPromptSpecification": PromptSpecificationTypeDef,
-        "lastUpdatedDateTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredConditionalBranchTypeDef = TypedDict(
     "_RequiredConditionalBranchTypeDef",
     {
         "name": str,
         "condition": ConditionTypeDef,
         "nextStep": DialogStateTypeDef,
     },
@@ -4803,129 +6250,126 @@
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "failureReasons": List[str],
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-        "encryptionSetting": EncryptionSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "encryptionSetting": EncryptionSettingOutputTypeDef,
         "botRecommendationResults": BotRecommendationResultsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_RequiredStartBotRecommendationRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-    },
-)
-_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
-    "_OptionalStartBotRecommendationRequestRequestTypeDef",
-    {
-        "encryptionSetting": EncryptionSettingTypeDef,
-    },
-    total=False,
-)
-
-class StartBotRecommendationRequestRequestTypeDef(
-    _RequiredStartBotRecommendationRequestRequestTypeDef,
-    _OptionalStartBotRecommendationRequestRequestTypeDef,
-):
-    pass
-
 StartBotRecommendationResponseTypeDef = TypedDict(
     "StartBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-        "encryptionSetting": EncryptionSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "encryptionSetting": EncryptionSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBotRecommendationResponseTypeDef = TypedDict(
     "UpdateBotRecommendationResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "botRecommendationStatus": BotRecommendationStatusType,
         "botRecommendationId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
-        "encryptionSetting": EncryptionSettingTypeDef,
+        "transcriptSourceSetting": TranscriptSourceSettingOutputTypeDef,
+        "encryptionSetting": EncryptionSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUtteranceLevelTestResultItemTypeDef = TypedDict(
-    "_RequiredUtteranceLevelTestResultItemTypeDef",
+_RequiredStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartBotRecommendationRequestRequestTypeDef",
     {
-        "recordNumber": int,
-        "turnResult": TestSetTurnResultTypeDef,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+        "transcriptSourceSetting": TranscriptSourceSettingTypeDef,
     },
 )
-_OptionalUtteranceLevelTestResultItemTypeDef = TypedDict(
-    "_OptionalUtteranceLevelTestResultItemTypeDef",
+_OptionalStartBotRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartBotRecommendationRequestRequestTypeDef",
     {
-        "conversationId": str,
+        "encryptionSetting": EncryptionSettingTypeDef,
     },
     total=False,
 )
 
-class UtteranceLevelTestResultItemTypeDef(
-    _RequiredUtteranceLevelTestResultItemTypeDef, _OptionalUtteranceLevelTestResultItemTypeDef
+class StartBotRecommendationRequestRequestTypeDef(
+    _RequiredStartBotRecommendationRequestRequestTypeDef,
+    _OptionalStartBotRecommendationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredTestSetTurnRecordTypeDef = TypedDict(
-    "_RequiredTestSetTurnRecordTypeDef",
+UtteranceLevelTestResultItemTypeDef = TypedDict(
+    "UtteranceLevelTestResultItemTypeDef",
     {
         "recordNumber": int,
-        "turnSpecification": TurnSpecificationTypeDef,
+        "conversationId": str,
+        "turnResult": TestSetTurnResultTypeDef,
     },
 )
-_OptionalTestSetTurnRecordTypeDef = TypedDict(
-    "_OptionalTestSetTurnRecordTypeDef",
+
+TestSetTurnRecordTypeDef = TypedDict(
+    "TestSetTurnRecordTypeDef",
     {
+        "recordNumber": int,
         "conversationId": str,
         "turnNumber": int,
+        "turnSpecification": TurnSpecificationTypeDef,
     },
-    total=False,
 )
 
-class TestSetTurnRecordTypeDef(
-    _RequiredTestSetTurnRecordTypeDef, _OptionalTestSetTurnRecordTypeDef
-):
-    pass
-
 ListSlotsResponseTypeDef = TypedDict(
     "ListSlotsResponseTypeDef",
     {
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "slotSummaries": List[SlotSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConditionalSpecificationOutputTypeDef = TypedDict(
+    "ConditionalSpecificationOutputTypeDef",
+    {
+        "active": bool,
+        "conditionalBranches": List[ConditionalBranchOutputTypeDef],
+        "defaultBranch": DefaultConditionalBranchOutputTypeDef,
+    },
+)
+
+SubSlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "SubSlotValueElicitationSettingOutputTypeDef",
+    {
+        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
+        "promptSpecification": PromptSpecificationOutputTypeDef,
+        "sampleUtterances": List[SampleUtteranceOutputTypeDef],
+        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
+    },
+)
+
 ConditionalSpecificationTypeDef = TypedDict(
     "ConditionalSpecificationTypeDef",
     {
         "active": bool,
         "conditionalBranches": Sequence[ConditionalBranchTypeDef],
         "defaultBranch": DefaultConditionalBranchTypeDef,
     },
@@ -4964,14 +6408,62 @@
     {
         "testSetRecords": List[TestSetTurnRecordTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IntentClosingSettingOutputTypeDef = TypedDict(
+    "IntentClosingSettingOutputTypeDef",
+    {
+        "closingResponse": ResponseSpecificationOutputTypeDef,
+        "active": bool,
+        "nextStep": DialogStateOutputTypeDef,
+        "conditional": ConditionalSpecificationOutputTypeDef,
+    },
+)
+
+PostDialogCodeHookInvocationSpecificationOutputTypeDef = TypedDict(
+    "PostDialogCodeHookInvocationSpecificationOutputTypeDef",
+    {
+        "successResponse": ResponseSpecificationOutputTypeDef,
+        "successNextStep": DialogStateOutputTypeDef,
+        "successConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "timeoutResponse": ResponseSpecificationOutputTypeDef,
+        "timeoutNextStep": DialogStateOutputTypeDef,
+        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
+    },
+)
+
+PostFulfillmentStatusSpecificationOutputTypeDef = TypedDict(
+    "PostFulfillmentStatusSpecificationOutputTypeDef",
+    {
+        "successResponse": ResponseSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "timeoutResponse": ResponseSpecificationOutputTypeDef,
+        "successNextStep": DialogStateOutputTypeDef,
+        "successConditional": ConditionalSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "timeoutNextStep": DialogStateOutputTypeDef,
+        "timeoutConditional": ConditionalSpecificationOutputTypeDef,
+    },
+)
+
+SpecificationsOutputTypeDef = TypedDict(
+    "SpecificationsOutputTypeDef",
+    {
+        "slotTypeId": str,
+        "valueElicitationSetting": SubSlotValueElicitationSettingOutputTypeDef,
+    },
+)
+
 IntentClosingSettingTypeDef = TypedDict(
     "IntentClosingSettingTypeDef",
     {
         "closingResponse": ResponseSpecificationTypeDef,
         "active": bool,
         "nextStep": DialogStateTypeDef,
         "conditional": ConditionalSpecificationTypeDef,
@@ -5024,15 +6516,42 @@
     {
         "overallTestResults": OverallTestResultsTypeDef,
         "conversationLevelTestResults": ConversationLevelTestResultsTypeDef,
         "intentClassificationTestResults": IntentClassificationTestResultsTypeDef,
         "intentLevelSlotResolutionTestResults": IntentLevelSlotResolutionTestResultsTypeDef,
         "utteranceLevelTestResults": UtteranceLevelTestResultsTypeDef,
     },
-    total=False,
+)
+
+DialogCodeHookInvocationSettingOutputTypeDef = TypedDict(
+    "DialogCodeHookInvocationSettingOutputTypeDef",
+    {
+        "enableCodeHookInvocation": bool,
+        "active": bool,
+        "invocationLabel": str,
+        "postCodeHookSpecification": PostDialogCodeHookInvocationSpecificationOutputTypeDef,
+    },
+)
+
+FulfillmentCodeHookSettingsOutputTypeDef = TypedDict(
+    "FulfillmentCodeHookSettingsOutputTypeDef",
+    {
+        "enabled": bool,
+        "postFulfillmentStatusSpecification": PostFulfillmentStatusSpecificationOutputTypeDef,
+        "fulfillmentUpdatesSpecification": FulfillmentUpdatesSpecificationOutputTypeDef,
+        "active": bool,
+    },
+)
+
+SubSlotSettingOutputTypeDef = TypedDict(
+    "SubSlotSettingOutputTypeDef",
+    {
+        "expression": str,
+        "slotSpecifications": Dict[str, SpecificationsOutputTypeDef],
+    },
 )
 
 _RequiredDialogCodeHookInvocationSettingTypeDef = TypedDict(
     "_RequiredDialogCodeHookInvocationSettingTypeDef",
     {
         "enableCodeHookInvocation": bool,
         "active": bool,
@@ -5087,14 +6606,57 @@
     {
         "testExecutionResults": TestExecutionResultItemsTypeDef,
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InitialResponseSettingOutputTypeDef = TypedDict(
+    "InitialResponseSettingOutputTypeDef",
+    {
+        "initialResponse": ResponseSpecificationOutputTypeDef,
+        "nextStep": DialogStateOutputTypeDef,
+        "conditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+    },
+)
+
+IntentConfirmationSettingOutputTypeDef = TypedDict(
+    "IntentConfirmationSettingOutputTypeDef",
+    {
+        "promptSpecification": PromptSpecificationOutputTypeDef,
+        "declinationResponse": ResponseSpecificationOutputTypeDef,
+        "active": bool,
+        "confirmationResponse": ResponseSpecificationOutputTypeDef,
+        "confirmationNextStep": DialogStateOutputTypeDef,
+        "confirmationConditional": ConditionalSpecificationOutputTypeDef,
+        "declinationNextStep": DialogStateOutputTypeDef,
+        "declinationConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+        "elicitationCodeHook": ElicitationCodeHookInvocationSettingOutputTypeDef,
+    },
+)
+
+SlotCaptureSettingOutputTypeDef = TypedDict(
+    "SlotCaptureSettingOutputTypeDef",
+    {
+        "captureResponse": ResponseSpecificationOutputTypeDef,
+        "captureNextStep": DialogStateOutputTypeDef,
+        "captureConditional": ConditionalSpecificationOutputTypeDef,
+        "failureResponse": ResponseSpecificationOutputTypeDef,
+        "failureNextStep": DialogStateOutputTypeDef,
+        "failureConditional": ConditionalSpecificationOutputTypeDef,
+        "codeHook": DialogCodeHookInvocationSettingOutputTypeDef,
+        "elicitationCodeHook": ElicitationCodeHookInvocationSettingOutputTypeDef,
+    },
+)
+
 InitialResponseSettingTypeDef = TypedDict(
     "InitialResponseSettingTypeDef",
     {
         "initialResponse": ResponseSpecificationTypeDef,
         "nextStep": DialogStateTypeDef,
         "conditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
@@ -5143,156 +6705,168 @@
         "failureConditional": ConditionalSpecificationTypeDef,
         "codeHook": DialogCodeHookInvocationSettingTypeDef,
         "elicitationCodeHook": ElicitationCodeHookInvocationSettingTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIntentRequestRequestTypeDef",
+CreateIntentResponseTypeDef = TypedDict(
+    "CreateIntentResponseTypeDef",
     {
+        "intentId": str,
         "intentName": str,
+        "description": str,
+        "parentIntentSignature": str,
+        "sampleUtterances": List[SampleUtteranceOutputTypeDef],
+        "dialogCodeHook": DialogCodeHookSettingsOutputTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
+        "creationDateTime": datetime,
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIntentRequestRequestTypeDef",
-    {
-        "description": str,
-        "parentIntentSignature": str,
-        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
-        "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": Sequence[InputContextTypeDef],
-        "outputContexts": Sequence[OutputContextTypeDef],
-        "kendraConfiguration": KendraConfigurationTypeDef,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
-    },
-    total=False,
-)
-
-class CreateIntentRequestRequestTypeDef(
-    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
-):
-    pass
 
-CreateIntentResponseTypeDef = TypedDict(
-    "CreateIntentResponseTypeDef",
+DescribeIntentResponseTypeDef = TypedDict(
+    "DescribeIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
-        "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
-        "kendraConfiguration": KendraConfigurationTypeDef,
+        "sampleUtterances": List[SampleUtteranceOutputTypeDef],
+        "dialogCodeHook": DialogCodeHookSettingsOutputTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "slotPriorities": List[SlotPriorityOutputTypeDef],
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
+        "lastUpdatedDateTime": datetime,
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeIntentResponseTypeDef = TypedDict(
-    "DescribeIntentResponseTypeDef",
+UpdateIntentResponseTypeDef = TypedDict(
+    "UpdateIntentResponseTypeDef",
     {
         "intentId": str,
         "intentName": str,
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
-        "dialogCodeHook": DialogCodeHookSettingsTypeDef,
-        "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": List[SlotPriorityTypeDef],
-        "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
-        "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
-        "kendraConfiguration": KendraConfigurationTypeDef,
+        "sampleUtterances": List[SampleUtteranceOutputTypeDef],
+        "dialogCodeHook": DialogCodeHookSettingsOutputTypeDef,
+        "fulfillmentCodeHook": FulfillmentCodeHookSettingsOutputTypeDef,
+        "slotPriorities": List[SlotPriorityOutputTypeDef],
+        "intentConfirmationSetting": IntentConfirmationSettingOutputTypeDef,
+        "intentClosingSetting": IntentClosingSettingOutputTypeDef,
+        "inputContexts": List[InputContextOutputTypeDef],
+        "outputContexts": List[OutputContextOutputTypeDef],
+        "kendraConfiguration": KendraConfigurationOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "initialResponseSetting": InitialResponseSettingTypeDef,
+        "initialResponseSetting": InitialResponseSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateIntentRequestRequestTypeDef",
+SlotValueElicitationSettingOutputTypeDef = TypedDict(
+    "SlotValueElicitationSettingOutputTypeDef",
+    {
+        "defaultValueSpecification": SlotDefaultValueSpecificationOutputTypeDef,
+        "slotConstraint": SlotConstraintType,
+        "promptSpecification": PromptSpecificationOutputTypeDef,
+        "sampleUtterances": List[SampleUtteranceOutputTypeDef],
+        "waitAndContinueSpecification": WaitAndContinueSpecificationOutputTypeDef,
+        "slotCaptureSetting": SlotCaptureSettingOutputTypeDef,
+    },
+)
+
+_RequiredCreateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIntentRequestRequestTypeDef",
     {
-        "intentId": str,
         "intentName": str,
         "botId": str,
         "botVersion": str,
         "localeId": str,
     },
 )
-_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateIntentRequestRequestTypeDef",
+_OptionalCreateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIntentRequestRequestTypeDef",
     {
         "description": str,
         "parentIntentSignature": str,
         "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": Sequence[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
         "initialResponseSetting": InitialResponseSettingTypeDef,
     },
     total=False,
 )
 
-class UpdateIntentRequestRequestTypeDef(
-    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
+class CreateIntentRequestRequestTypeDef(
+    _RequiredCreateIntentRequestRequestTypeDef, _OptionalCreateIntentRequestRequestTypeDef
 ):
     pass
 
-UpdateIntentResponseTypeDef = TypedDict(
-    "UpdateIntentResponseTypeDef",
+_RequiredUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateIntentRequestRequestTypeDef",
     {
         "intentId": str,
         "intentName": str,
+        "botId": str,
+        "botVersion": str,
+        "localeId": str,
+    },
+)
+_OptionalUpdateIntentRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateIntentRequestRequestTypeDef",
+    {
         "description": str,
         "parentIntentSignature": str,
-        "sampleUtterances": List[SampleUtteranceTypeDef],
+        "sampleUtterances": Sequence[SampleUtteranceTypeDef],
         "dialogCodeHook": DialogCodeHookSettingsTypeDef,
         "fulfillmentCodeHook": FulfillmentCodeHookSettingsTypeDef,
-        "slotPriorities": List[SlotPriorityTypeDef],
+        "slotPriorities": Sequence[SlotPriorityTypeDef],
         "intentConfirmationSetting": IntentConfirmationSettingTypeDef,
         "intentClosingSetting": IntentClosingSettingTypeDef,
-        "inputContexts": List[InputContextTypeDef],
-        "outputContexts": List[OutputContextTypeDef],
+        "inputContexts": Sequence[InputContextTypeDef],
+        "outputContexts": Sequence[OutputContextTypeDef],
         "kendraConfiguration": KendraConfigurationTypeDef,
-        "botId": str,
-        "botVersion": str,
-        "localeId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
         "initialResponseSetting": InitialResponseSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+class UpdateIntentRequestRequestTypeDef(
+    _RequiredUpdateIntentRequestRequestTypeDef, _OptionalUpdateIntentRequestRequestTypeDef
+):
+    pass
+
 _RequiredSlotValueElicitationSettingTypeDef = TypedDict(
     "_RequiredSlotValueElicitationSettingTypeDef",
     {
         "slotConstraint": SlotConstraintType,
     },
 )
 _OptionalSlotValueElicitationSettingTypeDef = TypedDict(
@@ -5308,125 +6882,125 @@
 )
 
 class SlotValueElicitationSettingTypeDef(
     _RequiredSlotValueElicitationSettingTypeDef, _OptionalSlotValueElicitationSettingTypeDef
 ):
     pass
 
-_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSlotRequestRequestTypeDef",
+CreateSlotResponseTypeDef = TypedDict(
+    "CreateSlotResponseTypeDef",
     {
+        "slotId": str,
         "slotName": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
+        "description": str,
+        "slotTypeId": str,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "obfuscationSetting": ObfuscationSettingOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
+        "creationDateTime": datetime,
+        "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSlotRequestRequestTypeDef",
-    {
-        "description": str,
-        "slotTypeId": str,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
-        "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
-    },
-    total=False,
-)
-
-class CreateSlotRequestRequestTypeDef(
-    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
-):
-    pass
 
-CreateSlotResponseTypeDef = TypedDict(
-    "CreateSlotResponseTypeDef",
+DescribeSlotResponseTypeDef = TypedDict(
+    "DescribeSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "obfuscationSetting": ObfuscationSettingOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
-        "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
+        "lastUpdatedDateTime": datetime,
+        "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSlotResponseTypeDef = TypedDict(
-    "DescribeSlotResponseTypeDef",
+UpdateSlotResponseTypeDef = TypedDict(
+    "UpdateSlotResponseTypeDef",
     {
         "slotId": str,
         "slotName": str,
         "description": str,
         "slotTypeId": str,
-        "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
+        "valueElicitationSetting": SlotValueElicitationSettingOutputTypeDef,
+        "obfuscationSetting": ObfuscationSettingOutputTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
         "creationDateTime": datetime,
         "lastUpdatedDateTime": datetime,
-        "multipleValuesSetting": MultipleValuesSettingTypeDef,
-        "subSlotSetting": SubSlotSettingTypeDef,
+        "multipleValuesSetting": MultipleValuesSettingOutputTypeDef,
+        "subSlotSetting": SubSlotSettingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSlotRequestRequestTypeDef",
+_RequiredCreateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSlotRequestRequestTypeDef",
     {
-        "slotId": str,
         "slotName": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
     },
 )
-_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSlotRequestRequestTypeDef",
+_OptionalCreateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSlotRequestRequestTypeDef",
     {
         "description": str,
         "slotTypeId": str,
         "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
     },
     total=False,
 )
 
-class UpdateSlotRequestRequestTypeDef(
-    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
+class CreateSlotRequestRequestTypeDef(
+    _RequiredCreateSlotRequestRequestTypeDef, _OptionalCreateSlotRequestRequestTypeDef
 ):
     pass
 
-UpdateSlotResponseTypeDef = TypedDict(
-    "UpdateSlotResponseTypeDef",
+_RequiredUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSlotRequestRequestTypeDef",
     {
         "slotId": str,
         "slotName": str,
-        "description": str,
-        "slotTypeId": str,
         "valueElicitationSetting": SlotValueElicitationSettingTypeDef,
-        "obfuscationSetting": ObfuscationSettingTypeDef,
         "botId": str,
         "botVersion": str,
         "localeId": str,
         "intentId": str,
-        "creationDateTime": datetime,
-        "lastUpdatedDateTime": datetime,
+    },
+)
+_OptionalUpdateSlotRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSlotRequestRequestTypeDef",
+    {
+        "description": str,
+        "slotTypeId": str,
+        "obfuscationSetting": ObfuscationSettingTypeDef,
         "multipleValuesSetting": MultipleValuesSettingTypeDef,
         "subSlotSetting": SubSlotSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
+
+class UpdateSlotRequestRequestTypeDef(
+    _RequiredUpdateSlotRequestRequestTypeDef, _OptionalUpdateSlotRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/waiter.py` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models/waiter.pyi` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.0/mypy_boto3_lexv2_models.egg-info/SOURCES.txt` & `mypy-boto3-lexv2-models-1.28.5/mypy_boto3_lexv2_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-models-1.28.0/setup.py` & `mypy-boto3-lexv2-models-1.28.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lexv2-models",
-    version="1.28.0",
+    version="1.28.5",
     packages=["mypy_boto3_lexv2_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexModelsV2 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.LexModelsV2 1.28.5 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

