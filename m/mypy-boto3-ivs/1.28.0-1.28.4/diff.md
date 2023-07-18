# Comparing `tmp/mypy-boto3-ivs-1.28.0.tar.gz` & `tmp/mypy-boto3-ivs-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-1.28.0.tar", last modified: Thu Jul  6 20:59:51 2023, max compression
+gzip compressed data, was "mypy-boto3-ivs-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-ivs-1.28.0.tar` & `mypy-boto3-ivs-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:51.074336 mypy-boto3-ivs-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:16.000000 mypy-boto3-ivs-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-06 20:59:51.074336 mypy-boto3-ivs-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-07-06 20:44:16.000000 mypy-boto3-ivs-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:51.066336 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-06 20:44:16.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-06 20:44:16.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:44:16.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-07-06 20:44:19.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-07-06 20:44:18.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-07-06 20:44:19.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-07-06 20:44:19.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-06 20:44:19.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-06 20:44:19.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:16.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26328 2023-07-06 20:44:20.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26301 2023-07-06 20:44:19.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:16.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:51.074336 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-06 20:59:50.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:50.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:50.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:50.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:50.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:50.000000 mypy-boto3-ivs-1.28.0/mypy_boto3_ivs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:51.074336 mypy-boto3-ivs-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:44:16.000000 mypy-boto3-ivs-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16775 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.965310 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22888 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26821 2023-07-18 01:01:28.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16775 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 01:01:41.000000 mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.973310 mypy-boto3-ivs-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-18 01:01:27.000000 mypy-boto3-ivs-1.28.4/setup.py
```

### Comparing `mypy-boto3-ivs-1.28.0/LICENSE` & `mypy-boto3-ivs-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.0/PKG-INFO` & `mypy-boto3-ivs-1.28.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.28.0
-Summary: Type annotations for boto3.IVS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.4
+Summary: Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,16 +318,20 @@
     ListChannelsPaginatorName,
     ListPlaybackKeyPairsPaginatorName,
     ListRecordingConfigurationsPaginatorName,
     ListStreamKeysPaginatorName,
     ListStreamsPaginatorName,
     RecordingConfigurationStateType,
     RecordingModeType,
+    RenditionConfigurationRenditionSelectionType,
+    RenditionConfigurationRenditionType,
     StreamHealthType,
     StreamStateType,
+    ThumbnailConfigurationResolutionType,
+    ThumbnailConfigurationStorageType,
     TranscodePresetType,
     IVSServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -346,87 +350,92 @@
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetStreamKeyRequestRequestTypeDef,
     StreamKeyTypeDef,
     BatchStartViewerSessionRevocationErrorTypeDef,
     BatchStartViewerSessionRevocationViewerSessionTypeDef,
     ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
+    RenditionConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
     StreamTypeDef,
     GetStreamSessionRequestRequestTypeDef,
     ImportPlaybackKeyPairRequestRequestTypeDef,
     VideoConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
     ListPlaybackKeyPairsRequestRequestTypeDef,
     PlaybackKeyPairSummaryTypeDef,
-    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
     ListRecordingConfigurationsRequestRequestTypeDef,
-    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListStreamKeysRequestRequestTypeDef,
     StreamKeySummaryTypeDef,
     ListStreamSessionsRequestRequestTypeDef,
     StreamSessionSummaryTypeDef,
     StreamFiltersTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutMetadataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    RenditionConfigurationOutputTypeDef,
+    ThumbnailConfigurationOutputTypeDef,
     StartViewerSessionRevocationRequestRequestTypeDef,
     StopStreamRequestRequestTypeDef,
     StreamEventTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchGetChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdateChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
+    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
+    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
-    CreateRecordingConfigurationRequestRequestTypeDef,
     RecordingConfigurationSummaryTypeDef,
     RecordingConfigurationTypeDef,
+    CreateRecordingConfigurationRequestRequestTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     GetRecordingConfigurationResponseTypeDef,
     StreamSessionTypeDef,
     GetStreamSessionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ivs-1.28.0/README.md` & `mypy-boto3-ivs-1.28.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,16 +286,20 @@
     ListChannelsPaginatorName,
     ListPlaybackKeyPairsPaginatorName,
     ListRecordingConfigurationsPaginatorName,
     ListStreamKeysPaginatorName,
     ListStreamsPaginatorName,
     RecordingConfigurationStateType,
     RecordingModeType,
+    RenditionConfigurationRenditionSelectionType,
+    RenditionConfigurationRenditionType,
     StreamHealthType,
     StreamStateType,
+    ThumbnailConfigurationResolutionType,
+    ThumbnailConfigurationStorageType,
     TranscodePresetType,
     IVSServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -314,87 +318,92 @@
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetStreamKeyRequestRequestTypeDef,
     StreamKeyTypeDef,
     BatchStartViewerSessionRevocationErrorTypeDef,
     BatchStartViewerSessionRevocationViewerSessionTypeDef,
     ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
+    RenditionConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
     StreamTypeDef,
     GetStreamSessionRequestRequestTypeDef,
     ImportPlaybackKeyPairRequestRequestTypeDef,
     VideoConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
     ListPlaybackKeyPairsRequestRequestTypeDef,
     PlaybackKeyPairSummaryTypeDef,
-    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
     ListRecordingConfigurationsRequestRequestTypeDef,
-    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListStreamKeysRequestRequestTypeDef,
     StreamKeySummaryTypeDef,
     ListStreamSessionsRequestRequestTypeDef,
     StreamSessionSummaryTypeDef,
     StreamFiltersTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutMetadataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    RenditionConfigurationOutputTypeDef,
+    ThumbnailConfigurationOutputTypeDef,
     StartViewerSessionRevocationRequestRequestTypeDef,
     StopStreamRequestRequestTypeDef,
     StreamEventTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchGetChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdateChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
+    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
+    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
-    CreateRecordingConfigurationRequestRequestTypeDef,
     RecordingConfigurationSummaryTypeDef,
     RecordingConfigurationTypeDef,
+    CreateRecordingConfigurationRequestRequestTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     GetRecordingConfigurationResponseTypeDef,
     StreamSessionTypeDef,
     GetStreamSessionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/__init__.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/__init__.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/__main__.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IVS 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IVS 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS\nOther"
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

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/client.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     ListChannelsResponseTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    RenditionConfigurationTypeDef,
     StreamFiltersTypeDef,
     ThumbnailConfigurationTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -167,14 +168,15 @@
 
     def create_recording_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
+        renditionConfiguration: RenditionConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
         thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
```

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/client.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     ListChannelsResponseTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    RenditionConfigurationTypeDef,
     StreamFiltersTypeDef,
     ThumbnailConfigurationTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -156,14 +157,15 @@
         """
     def create_recording_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
         recordingReconnectWindowSeconds: int = ...,
+        renditionConfiguration: RenditionConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
         thumbnailConfiguration: ThumbnailConfigurationTypeDef = ...
     ) -> CreateRecordingConfigurationResponseTypeDef:
         """
         Creates a new recording configuration, used to enable recording to Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client.create_recording_configuration)
```

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/literals.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     "ListChannelsPaginatorName",
     "ListPlaybackKeyPairsPaginatorName",
     "ListRecordingConfigurationsPaginatorName",
     "ListStreamKeysPaginatorName",
     "ListStreamsPaginatorName",
     "RecordingConfigurationStateType",
     "RecordingModeType",
+    "RenditionConfigurationRenditionSelectionType",
+    "RenditionConfigurationRenditionType",
     "StreamHealthType",
     "StreamStateType",
+    "ThumbnailConfigurationResolutionType",
+    "ThumbnailConfigurationStorageType",
     "TranscodePresetType",
     "IVSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -45,16 +49,20 @@
 ListChannelsPaginatorName = Literal["list_channels"]
 ListPlaybackKeyPairsPaginatorName = Literal["list_playback_key_pairs"]
 ListRecordingConfigurationsPaginatorName = Literal["list_recording_configurations"]
 ListStreamKeysPaginatorName = Literal["list_stream_keys"]
 ListStreamsPaginatorName = Literal["list_streams"]
 RecordingConfigurationStateType = Literal["ACTIVE", "CREATE_FAILED", "CREATING"]
 RecordingModeType = Literal["DISABLED", "INTERVAL"]
+RenditionConfigurationRenditionSelectionType = Literal["ALL", "CUSTOM", "NONE"]
+RenditionConfigurationRenditionType = Literal["FULL_HD", "HD", "LOWEST_RESOLUTION", "SD"]
 StreamHealthType = Literal["HEALTHY", "STARVING", "UNKNOWN"]
 StreamStateType = Literal["LIVE", "OFFLINE"]
+ThumbnailConfigurationResolutionType = Literal["FULL_HD", "HD", "LOWEST_RESOLUTION", "SD"]
+ThumbnailConfigurationStorageType = Literal["LATEST", "SEQUENTIAL"]
 TranscodePresetType = Literal["CONSTRAINED_BANDWIDTH_DELIVERY", "HIGHER_BANDWIDTH_DELIVERY"]
 IVSServiceName = Literal["ivs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
```

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/literals.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,20 @@
     "ListChannelsPaginatorName",
     "ListPlaybackKeyPairsPaginatorName",
     "ListRecordingConfigurationsPaginatorName",
     "ListStreamKeysPaginatorName",
     "ListStreamsPaginatorName",
     "RecordingConfigurationStateType",
     "RecordingModeType",
+    "RenditionConfigurationRenditionSelectionType",
+    "RenditionConfigurationRenditionType",
     "StreamHealthType",
     "StreamStateType",
+    "ThumbnailConfigurationResolutionType",
+    "ThumbnailConfigurationStorageType",
     "TranscodePresetType",
     "IVSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -43,16 +47,20 @@
 ListChannelsPaginatorName = Literal["list_channels"]
 ListPlaybackKeyPairsPaginatorName = Literal["list_playback_key_pairs"]
 ListRecordingConfigurationsPaginatorName = Literal["list_recording_configurations"]
 ListStreamKeysPaginatorName = Literal["list_stream_keys"]
 ListStreamsPaginatorName = Literal["list_streams"]
 RecordingConfigurationStateType = Literal["ACTIVE", "CREATE_FAILED", "CREATING"]
 RecordingModeType = Literal["DISABLED", "INTERVAL"]
+RenditionConfigurationRenditionSelectionType = Literal["ALL", "CUSTOM", "NONE"]
+RenditionConfigurationRenditionType = Literal["FULL_HD", "HD", "LOWEST_RESOLUTION", "SD"]
 StreamHealthType = Literal["HEALTHY", "STARVING", "UNKNOWN"]
 StreamStateType = Literal["LIVE", "OFFLINE"]
+ThumbnailConfigurationResolutionType = Literal["FULL_HD", "HD", "LOWEST_RESOLUTION", "SD"]
+ThumbnailConfigurationStorageType = Literal["LATEST", "SEQUENTIAL"]
 TranscodePresetType = Literal["CONSTRAINED_BANDWIDTH_DELIVERY", "HIGHER_BANDWIDTH_DELIVERY"]
 IVSServiceName = Literal["ivs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
```

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/paginator.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,98 +45,91 @@
     "ListChannelsPaginator",
     "ListPlaybackKeyPairsPaginator",
     "ListRecordingConfigurationsPaginator",
     "ListStreamKeysPaginator",
     "ListStreamsPaginator",
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
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         filterByName: str = ...,
         filterByRecordingConfigurationArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
         """
 
-
 class ListPlaybackKeyPairsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlaybackKeyPairsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
         """
 
-
 class ListRecordingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecordingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
         """
 
-
 class ListStreamKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
     """
 
     def paginate(
-        self, *, channelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, channelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
         """
 
-
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         filterBy: StreamFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/paginator.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,91 +45,98 @@
     "ListChannelsPaginator",
     "ListPlaybackKeyPairsPaginator",
     "ListRecordingConfigurationsPaginator",
     "ListStreamKeysPaginator",
     "ListStreamsPaginator",
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
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         filterByName: str = ...,
         filterByRecordingConfigurationArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listchannelspaginator)
         """
 
+
 class ListPlaybackKeyPairsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlaybackKeyPairsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListPlaybackKeyPairs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listplaybackkeypairspaginator)
         """
 
+
 class ListRecordingConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecordingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListRecordingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#listrecordingconfigurationspaginator)
         """
 
+
 class ListStreamKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
     """
 
     def paginate(
-        self, *, channelArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, channelArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreamKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamkeyspaginator)
         """
 
+
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         filterBy: StreamFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/paginators/#liststreamspaginator)
         """
```

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/type_defs.py` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,103 +16,112 @@
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ChannelLatencyModeType,
     ChannelTypeType,
     RecordingConfigurationStateType,
     RecordingModeType,
+    RenditionConfigurationRenditionSelectionType,
+    RenditionConfigurationRenditionType,
     StreamHealthType,
     StreamStateType,
+    ThumbnailConfigurationResolutionType,
+    ThumbnailConfigurationStorageType,
     TranscodePresetType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
     "ChannelTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
     "StreamKeyTypeDef",
     "BatchStartViewerSessionRevocationErrorTypeDef",
     "BatchStartViewerSessionRevocationViewerSessionTypeDef",
     "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
+    "RenditionConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetPlaybackKeyPairRequestRequestTypeDef",
     "PlaybackKeyPairTypeDef",
     "GetRecordingConfigurationRequestRequestTypeDef",
     "GetStreamKeyRequestRequestTypeDef",
     "GetStreamRequestRequestTypeDef",
     "StreamTypeDef",
     "GetStreamSessionRequestRequestTypeDef",
     "ImportPlaybackKeyPairRequestRequestTypeDef",
     "VideoConfigurationTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     "PlaybackKeyPairSummaryTypeDef",
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
     "ListRecordingConfigurationsRequestRequestTypeDef",
-    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListStreamKeysRequestRequestTypeDef",
     "StreamKeySummaryTypeDef",
     "ListStreamSessionsRequestRequestTypeDef",
     "StreamSessionSummaryTypeDef",
     "StreamFiltersTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutMetadataRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "RenditionConfigurationOutputTypeDef",
+    "ThumbnailConfigurationOutputTypeDef",
     "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "BatchGetChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChannelResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
     "BatchStartViewerSessionRevocationResponseTypeDef",
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
+    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
-    "CreateRecordingConfigurationRequestRequestTypeDef",
     "RecordingConfigurationSummaryTypeDef",
     "RecordingConfigurationTypeDef",
+    "CreateRecordingConfigurationRequestRequestTypeDef",
     "ListRecordingConfigurationsResponseTypeDef",
     "CreateRecordingConfigurationResponseTypeDef",
     "GetRecordingConfigurationResponseTypeDef",
     "StreamSessionTypeDef",
     "GetStreamSessionResponseTypeDef",
 )
 
@@ -120,25 +129,23 @@
     "AudioConfigurationTypeDef",
     {
         "channels": int,
         "codec": str,
         "sampleRate": int,
         "targetBitrate": int,
     },
-    total=False,
 )
 
 BatchErrorTypeDef = TypedDict(
     "BatchErrorTypeDef",
     {
         "arn": str,
         "code": str,
         "message": str,
     },
-    total=False,
 )
 
 BatchGetChannelRequestRequestTypeDef = TypedDict(
     "BatchGetChannelRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -155,15 +162,25 @@
         "name": str,
         "playbackUrl": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
 )
 
 BatchGetStreamKeyRequestRequestTypeDef = TypedDict(
     "BatchGetStreamKeyRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -173,41 +190,26 @@
     "StreamKeyTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
-    total=False,
 )
 
-_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+BatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationErrorTypeDef",
     {
         "channelArn": str,
-        "viewerId": str,
-    },
-)
-_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
-    {
         "code": str,
         "message": str,
+        "viewerId": str,
     },
-    total=False,
 )
 
-
-class BatchStartViewerSessionRevocationErrorTypeDef(
-    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
-    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
-):
-    pass
-
-
 _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
     "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
     },
 )
@@ -236,15 +238,14 @@
         "latencyMode": ChannelLatencyModeType,
         "name": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
         "insecureIngest": bool,
@@ -254,18 +255,29 @@
         "recordingConfigurationArn": str,
         "tags": Mapping[str, str],
         "type": ChannelTypeType,
     },
     total=False,
 )
 
+RenditionConfigurationTypeDef = TypedDict(
+    "RenditionConfigurationTypeDef",
+    {
+        "renditionSelection": RenditionConfigurationRenditionSelectionType,
+        "renditions": Sequence[RenditionConfigurationRenditionType],
+    },
+    total=False,
+)
+
 ThumbnailConfigurationTypeDef = TypedDict(
     "ThumbnailConfigurationTypeDef",
     {
         "recordingMode": RecordingModeType,
+        "resolution": ThumbnailConfigurationResolutionType,
+        "storage": Sequence[ThumbnailConfigurationStorageType],
         "targetIntervalSeconds": int,
     },
     total=False,
 )
 
 _RequiredCreateStreamKeyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamKeyRequestRequestTypeDef",
@@ -312,25 +324,25 @@
 DeleteStreamKeyRequestRequestTypeDef = TypedDict(
     "DeleteStreamKeyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-S3DestinationConfigurationTypeDef = TypedDict(
-    "S3DestinationConfigurationTypeDef",
+S3DestinationConfigurationOutputTypeDef = TypedDict(
+    "S3DestinationConfigurationOutputTypeDef",
     {
         "bucketName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+S3DestinationConfigurationTypeDef = TypedDict(
+    "S3DestinationConfigurationTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "bucketName": str,
     },
 )
 
 GetChannelRequestRequestTypeDef = TypedDict(
     "GetChannelRequestRequestTypeDef",
     {
         "arn": str,
@@ -348,15 +360,14 @@
     "PlaybackKeyPairTypeDef",
     {
         "arn": str,
         "fingerprint": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 GetRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecordingConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
@@ -383,15 +394,14 @@
         "health": StreamHealthType,
         "playbackUrl": str,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 _RequiredGetStreamSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetStreamSessionRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -442,23 +452,22 @@
         "codec": str,
         "encoder": str,
         "targetBitrate": int,
         "targetFramerate": int,
         "videoHeight": int,
         "videoWidth": int,
     },
-    total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "filterByName": str,
-        "filterByRecordingConfigurationArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
@@ -466,22 +475,14 @@
         "filterByRecordingConfigurationArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPlaybackKeyPairsRequestRequestTypeDef = TypedDict(
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -490,56 +491,25 @@
 PlaybackKeyPairSummaryTypeDef = TypedDict(
     "PlaybackKeyPairSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
-)
-
-ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListRecordingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListRecordingConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "channelArn": str,
-    },
-)
-_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
-    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
-    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStreamKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamKeysRequestRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 _OptionalListStreamKeysRequestRequestTypeDef = TypedDict(
@@ -561,15 +531,14 @@
 StreamKeySummaryTypeDef = TypedDict(
     "StreamKeySummaryTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredListStreamSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamSessionsRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -595,15 +564,14 @@
     "StreamSessionSummaryTypeDef",
     {
         "endTime": datetime,
         "hasErrorEvent": bool,
         "startTime": datetime,
         "streamId": str,
     },
-    total=False,
 )
 
 StreamFiltersTypeDef = TypedDict(
     "StreamFiltersTypeDef",
     {
         "health": StreamHealthType,
     },
@@ -616,58 +584,46 @@
         "channelArn": str,
         "health": StreamHealthType,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 PutMetadataRequestRequestTypeDef = TypedDict(
     "PutMetadataRequestRequestTypeDef",
     {
         "channelArn": str,
         "metadata": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+RenditionConfigurationOutputTypeDef = TypedDict(
+    "RenditionConfigurationOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "renditionSelection": RenditionConfigurationRenditionSelectionType,
+        "renditions": List[RenditionConfigurationRenditionType],
+    },
+)
+
+ThumbnailConfigurationOutputTypeDef = TypedDict(
+    "ThumbnailConfigurationOutputTypeDef",
+    {
+        "recordingMode": RecordingModeType,
+        "resolution": ThumbnailConfigurationResolutionType,
+        "storage": List[ThumbnailConfigurationStorageType],
+        "targetIntervalSeconds": int,
     },
 )
 
 _RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "channelArn": str,
@@ -700,15 +656,14 @@
 StreamEventTypeDef = TypedDict(
     "StreamEventTypeDef",
     {
         "eventTime": datetime,
         "name": str,
         "type": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -751,73 +706,88 @@
 
 
 BatchGetChannelResponseTypeDef = TypedDict(
     "BatchGetChannelResponseTypeDef",
     {
         "channels": List[ChannelTypeDef],
         "errors": List[BatchErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetStreamKeyResponseTypeDef = TypedDict(
     "BatchGetStreamKeyResponseTypeDef",
     {
         "errors": List[BatchErrorTypeDef],
         "streamKeys": List[StreamKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamKeyResponseTypeDef = TypedDict(
     "CreateStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamKeyResponseTypeDef = TypedDict(
     "GetStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStartViewerSessionRevocationResponseTypeDef = TypedDict(
     "BatchStartViewerSessionRevocationResponseTypeDef",
     {
         "errors": List[BatchStartViewerSessionRevocationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "viewerSessions": Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],
@@ -825,15 +795,22 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "s3": S3DestinationConfigurationOutputTypeDef,
     },
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "s3": S3DestinationConfigurationTypeDef,
@@ -841,75 +818,122 @@
     total=False,
 )
 
 GetPlaybackKeyPairResponseTypeDef = TypedDict(
     "GetPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportPlaybackKeyPairResponseTypeDef = TypedDict(
     "ImportPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamResponseTypeDef = TypedDict(
     "GetStreamResponseTypeDef",
     {
         "stream": StreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IngestConfigurationTypeDef = TypedDict(
     "IngestConfigurationTypeDef",
     {
         "audio": AudioConfigurationTypeDef,
         "video": VideoConfigurationTypeDef,
     },
+)
+
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "filterByName": str,
+        "filterByRecordingConfigurationArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
+ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "channelArn": str,
+    },
+)
+_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
+    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
+    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
+):
+    pass
+
+
 ListPlaybackKeyPairsResponseTypeDef = TypedDict(
     "ListPlaybackKeyPairsResponseTypeDef",
     {
         "keyPairs": List[PlaybackKeyPairSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamKeysResponseTypeDef = TypedDict(
     "ListStreamKeysResponseTypeDef",
     {
         "nextToken": str,
         "streamKeys": List[StreamKeySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamSessionsResponseTypeDef = TypedDict(
     "ListStreamSessionsResponseTypeDef",
     {
         "nextToken": str,
         "streamSessions": List[StreamSessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsRequestListStreamsPaginateTypeDef",
     {
         "filterBy": StreamFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListStreamsRequestRequestTypeDef = TypedDict(
     "ListStreamsRequestRequestTypeDef",
     {
@@ -921,132 +945,107 @@
 )
 
 ListStreamsResponseTypeDef = TypedDict(
     "ListStreamsResponseTypeDef",
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
-    {
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
+RecordingConfigurationSummaryTypeDef = TypedDict(
+    "RecordingConfigurationSummaryTypeDef",
     {
+        "arn": str,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
-        "recordingReconnectWindowSeconds": int,
-        "tags": Mapping[str, str],
-        "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
+        "state": RecordingConfigurationStateType,
+        "tags": Dict[str, str],
     },
-    total=False,
 )
 
-
-class CreateRecordingConfigurationRequestRequestTypeDef(
-    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
-    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationSummaryTypeDef",
+RecordingConfigurationTypeDef = TypedDict(
+    "RecordingConfigurationTypeDef",
     {
         "arn": str,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
-    },
-)
-_OptionalRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationSummaryTypeDef",
-    {
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
+        "recordingReconnectWindowSeconds": int,
+        "renditionConfiguration": RenditionConfigurationOutputTypeDef,
+        "state": RecordingConfigurationStateType,
         "tags": Dict[str, str],
+        "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
-
-class RecordingConfigurationSummaryTypeDef(
-    _RequiredRecordingConfigurationSummaryTypeDef, _OptionalRecordingConfigurationSummaryTypeDef
-):
-    pass
-
-
-_RequiredRecordingConfigurationTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationTypeDef",
+_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
         "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
     },
 )
-_OptionalRecordingConfigurationTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationTypeDef",
+_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "recordingReconnectWindowSeconds": int,
-        "tags": Dict[str, str],
+        "renditionConfiguration": RenditionConfigurationTypeDef,
+        "tags": Mapping[str, str],
         "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class RecordingConfigurationTypeDef(
-    _RequiredRecordingConfigurationTypeDef, _OptionalRecordingConfigurationTypeDef
+class CreateRecordingConfigurationRequestRequestTypeDef(
+    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
+    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "recordingConfigurations": List[RecordingConfigurationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRecordingConfigurationResponseTypeDef = TypedDict(
     "CreateRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecordingConfigurationResponseTypeDef = TypedDict(
     "GetRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamSessionTypeDef = TypedDict(
     "StreamSessionTypeDef",
     {
         "channel": ChannelTypeDef,
         "endTime": datetime,
         "ingestConfiguration": IngestConfigurationTypeDef,
         "recordingConfiguration": RecordingConfigurationTypeDef,
         "startTime": datetime,
         "streamId": str,
         "truncatedEvents": List[StreamEventTypeDef],
     },
-    total=False,
 )
 
 GetStreamSessionResponseTypeDef = TypedDict(
     "GetStreamSessionResponseTypeDef",
     {
         "streamSession": StreamSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs/type_defs.pyi` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -16,102 +16,111 @@
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ChannelLatencyModeType,
     ChannelTypeType,
     RecordingConfigurationStateType,
     RecordingModeType,
+    RenditionConfigurationRenditionSelectionType,
+    RenditionConfigurationRenditionType,
     StreamHealthType,
     StreamStateType,
+    ThumbnailConfigurationResolutionType,
+    ThumbnailConfigurationStorageType,
     TranscodePresetType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
     "ChannelTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
     "StreamKeyTypeDef",
     "BatchStartViewerSessionRevocationErrorTypeDef",
     "BatchStartViewerSessionRevocationViewerSessionTypeDef",
     "ChannelSummaryTypeDef",
     "CreateChannelRequestRequestTypeDef",
+    "RenditionConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeletePlaybackKeyPairRequestRequestTypeDef",
     "DeleteRecordingConfigurationRequestRequestTypeDef",
     "DeleteStreamKeyRequestRequestTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "S3DestinationConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetChannelRequestRequestTypeDef",
     "GetPlaybackKeyPairRequestRequestTypeDef",
     "PlaybackKeyPairTypeDef",
     "GetRecordingConfigurationRequestRequestTypeDef",
     "GetStreamKeyRequestRequestTypeDef",
     "GetStreamRequestRequestTypeDef",
     "StreamTypeDef",
     "GetStreamSessionRequestRequestTypeDef",
     "ImportPlaybackKeyPairRequestRequestTypeDef",
     "VideoConfigurationTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     "PlaybackKeyPairSummaryTypeDef",
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
     "ListRecordingConfigurationsRequestRequestTypeDef",
-    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListStreamKeysRequestRequestTypeDef",
     "StreamKeySummaryTypeDef",
     "ListStreamSessionsRequestRequestTypeDef",
     "StreamSessionSummaryTypeDef",
     "StreamFiltersTypeDef",
     "StreamSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutMetadataRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "RenditionConfigurationOutputTypeDef",
+    "ThumbnailConfigurationOutputTypeDef",
     "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "BatchGetChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChannelResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "BatchGetStreamKeyResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
     "BatchStartViewerSessionRevocationResponseTypeDef",
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
     "IngestConfigurationTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
+    "ListStreamKeysRequestListStreamKeysPaginateTypeDef",
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
-    "CreateRecordingConfigurationRequestRequestTypeDef",
     "RecordingConfigurationSummaryTypeDef",
     "RecordingConfigurationTypeDef",
+    "CreateRecordingConfigurationRequestRequestTypeDef",
     "ListRecordingConfigurationsResponseTypeDef",
     "CreateRecordingConfigurationResponseTypeDef",
     "GetRecordingConfigurationResponseTypeDef",
     "StreamSessionTypeDef",
     "GetStreamSessionResponseTypeDef",
 )
 
@@ -119,25 +128,23 @@
     "AudioConfigurationTypeDef",
     {
         "channels": int,
         "codec": str,
         "sampleRate": int,
         "targetBitrate": int,
     },
-    total=False,
 )
 
 BatchErrorTypeDef = TypedDict(
     "BatchErrorTypeDef",
     {
         "arn": str,
         "code": str,
         "message": str,
     },
-    total=False,
 )
 
 BatchGetChannelRequestRequestTypeDef = TypedDict(
     "BatchGetChannelRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -154,15 +161,25 @@
         "name": str,
         "playbackUrl": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
 )
 
 BatchGetStreamKeyRequestRequestTypeDef = TypedDict(
     "BatchGetStreamKeyRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -172,39 +189,26 @@
     "StreamKeyTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
         "value": str,
     },
-    total=False,
 )
 
-_RequiredBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_RequiredBatchStartViewerSessionRevocationErrorTypeDef",
+BatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
+    "BatchStartViewerSessionRevocationErrorTypeDef",
     {
         "channelArn": str,
-        "viewerId": str,
-    },
-)
-_OptionalBatchStartViewerSessionRevocationErrorTypeDef = TypedDict(
-    "_OptionalBatchStartViewerSessionRevocationErrorTypeDef",
-    {
         "code": str,
         "message": str,
+        "viewerId": str,
     },
-    total=False,
 )
 
-class BatchStartViewerSessionRevocationErrorTypeDef(
-    _RequiredBatchStartViewerSessionRevocationErrorTypeDef,
-    _OptionalBatchStartViewerSessionRevocationErrorTypeDef,
-):
-    pass
-
 _RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef = TypedDict(
     "_RequiredBatchStartViewerSessionRevocationViewerSessionTypeDef",
     {
         "channelArn": str,
         "viewerId": str,
     },
 )
@@ -231,15 +235,14 @@
         "latencyMode": ChannelLatencyModeType,
         "name": str,
         "preset": TranscodePresetType,
         "recordingConfigurationArn": str,
         "tags": Dict[str, str],
         "type": ChannelTypeType,
     },
-    total=False,
 )
 
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": bool,
         "insecureIngest": bool,
@@ -249,18 +252,29 @@
         "recordingConfigurationArn": str,
         "tags": Mapping[str, str],
         "type": ChannelTypeType,
     },
     total=False,
 )
 
+RenditionConfigurationTypeDef = TypedDict(
+    "RenditionConfigurationTypeDef",
+    {
+        "renditionSelection": RenditionConfigurationRenditionSelectionType,
+        "renditions": Sequence[RenditionConfigurationRenditionType],
+    },
+    total=False,
+)
+
 ThumbnailConfigurationTypeDef = TypedDict(
     "ThumbnailConfigurationTypeDef",
     {
         "recordingMode": RecordingModeType,
+        "resolution": ThumbnailConfigurationResolutionType,
+        "storage": Sequence[ThumbnailConfigurationStorageType],
         "targetIntervalSeconds": int,
     },
     total=False,
 )
 
 _RequiredCreateStreamKeyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamKeyRequestRequestTypeDef",
@@ -305,25 +319,25 @@
 DeleteStreamKeyRequestRequestTypeDef = TypedDict(
     "DeleteStreamKeyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-S3DestinationConfigurationTypeDef = TypedDict(
-    "S3DestinationConfigurationTypeDef",
+S3DestinationConfigurationOutputTypeDef = TypedDict(
+    "S3DestinationConfigurationOutputTypeDef",
     {
         "bucketName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+S3DestinationConfigurationTypeDef = TypedDict(
+    "S3DestinationConfigurationTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "bucketName": str,
     },
 )
 
 GetChannelRequestRequestTypeDef = TypedDict(
     "GetChannelRequestRequestTypeDef",
     {
         "arn": str,
@@ -341,15 +355,14 @@
     "PlaybackKeyPairTypeDef",
     {
         "arn": str,
         "fingerprint": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 GetRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "GetRecordingConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
@@ -376,15 +389,14 @@
         "health": StreamHealthType,
         "playbackUrl": str,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 _RequiredGetStreamSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetStreamSessionRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -431,23 +443,22 @@
         "codec": str,
         "encoder": str,
         "targetBitrate": int,
         "targetFramerate": int,
         "videoHeight": int,
         "videoWidth": int,
     },
-    total=False,
 )
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "filterByName": str,
-        "filterByRecordingConfigurationArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
@@ -455,22 +466,14 @@
         "filterByRecordingConfigurationArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
-    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPlaybackKeyPairsRequestRequestTypeDef = TypedDict(
     "ListPlaybackKeyPairsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -479,54 +482,25 @@
 PlaybackKeyPairSummaryTypeDef = TypedDict(
     "PlaybackKeyPairSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "tags": Dict[str, str],
     },
-    total=False,
-)
-
-ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
-    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListRecordingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListRecordingConfigurationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "channelArn": str,
-    },
-)
-_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
-    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
-    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
-    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
-):
-    pass
-
 _RequiredListStreamKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamKeysRequestRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 _OptionalListStreamKeysRequestRequestTypeDef = TypedDict(
@@ -546,15 +520,14 @@
 StreamKeySummaryTypeDef = TypedDict(
     "StreamKeySummaryTypeDef",
     {
         "arn": str,
         "channelArn": str,
         "tags": Dict[str, str],
     },
-    total=False,
 )
 
 _RequiredListStreamSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamSessionsRequestRequestTypeDef",
     {
         "channelArn": str,
     },
@@ -578,15 +551,14 @@
     "StreamSessionSummaryTypeDef",
     {
         "endTime": datetime,
         "hasErrorEvent": bool,
         "startTime": datetime,
         "streamId": str,
     },
-    total=False,
 )
 
 StreamFiltersTypeDef = TypedDict(
     "StreamFiltersTypeDef",
     {
         "health": StreamHealthType,
     },
@@ -599,58 +571,46 @@
         "channelArn": str,
         "health": StreamHealthType,
         "startTime": datetime,
         "state": StreamStateType,
         "streamId": str,
         "viewerCount": int,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 PutMetadataRequestRequestTypeDef = TypedDict(
     "PutMetadataRequestRequestTypeDef",
     {
         "channelArn": str,
         "metadata": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+RenditionConfigurationOutputTypeDef = TypedDict(
+    "RenditionConfigurationOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "renditionSelection": RenditionConfigurationRenditionSelectionType,
+        "renditions": List[RenditionConfigurationRenditionType],
+    },
+)
+
+ThumbnailConfigurationOutputTypeDef = TypedDict(
+    "ThumbnailConfigurationOutputTypeDef",
+    {
+        "recordingMode": RecordingModeType,
+        "resolution": ThumbnailConfigurationResolutionType,
+        "storage": List[ThumbnailConfigurationStorageType],
+        "targetIntervalSeconds": int,
     },
 )
 
 _RequiredStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "_RequiredStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "channelArn": str,
@@ -681,15 +641,14 @@
 StreamEventTypeDef = TypedDict(
     "StreamEventTypeDef",
     {
         "eventTime": datetime,
         "name": str,
         "type": str,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -730,73 +689,88 @@
     pass
 
 BatchGetChannelResponseTypeDef = TypedDict(
     "BatchGetChannelResponseTypeDef",
     {
         "channels": List[ChannelTypeDef],
         "errors": List[BatchErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetStreamKeyResponseTypeDef = TypedDict(
     "BatchGetStreamKeyResponseTypeDef",
     {
         "errors": List[BatchErrorTypeDef],
         "streamKeys": List[StreamKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channel": ChannelTypeDef,
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamKeyResponseTypeDef = TypedDict(
     "CreateStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamKeyResponseTypeDef = TypedDict(
     "GetStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStartViewerSessionRevocationResponseTypeDef = TypedDict(
     "BatchStartViewerSessionRevocationResponseTypeDef",
     {
         "errors": List[BatchStartViewerSessionRevocationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchStartViewerSessionRevocationRequestRequestTypeDef = TypedDict(
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     {
         "viewerSessions": Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],
@@ -804,15 +778,22 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "s3": S3DestinationConfigurationOutputTypeDef,
     },
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "s3": S3DestinationConfigurationTypeDef,
@@ -820,75 +801,120 @@
     total=False,
 )
 
 GetPlaybackKeyPairResponseTypeDef = TypedDict(
     "GetPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportPlaybackKeyPairResponseTypeDef = TypedDict(
     "ImportPlaybackKeyPairResponseTypeDef",
     {
         "keyPair": PlaybackKeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamResponseTypeDef = TypedDict(
     "GetStreamResponseTypeDef",
     {
         "stream": StreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IngestConfigurationTypeDef = TypedDict(
     "IngestConfigurationTypeDef",
     {
         "audio": AudioConfigurationTypeDef,
         "video": VideoConfigurationTypeDef,
     },
+)
+
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "filterByName": str,
+        "filterByRecordingConfigurationArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef = TypedDict(
+    "ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef = TypedDict(
+    "ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "channelArn": str,
+    },
+)
+_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef = TypedDict(
+    "_OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
+class ListStreamKeysRequestListStreamKeysPaginateTypeDef(
+    _RequiredListStreamKeysRequestListStreamKeysPaginateTypeDef,
+    _OptionalListStreamKeysRequestListStreamKeysPaginateTypeDef,
+):
+    pass
+
 ListPlaybackKeyPairsResponseTypeDef = TypedDict(
     "ListPlaybackKeyPairsResponseTypeDef",
     {
         "keyPairs": List[PlaybackKeyPairSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamKeysResponseTypeDef = TypedDict(
     "ListStreamKeysResponseTypeDef",
     {
         "nextToken": str,
         "streamKeys": List[StreamKeySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamSessionsResponseTypeDef = TypedDict(
     "ListStreamSessionsResponseTypeDef",
     {
         "nextToken": str,
         "streamSessions": List[StreamSessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsRequestListStreamsPaginateTypeDef",
     {
         "filterBy": StreamFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListStreamsRequestRequestTypeDef = TypedDict(
     "ListStreamsRequestRequestTypeDef",
     {
@@ -900,126 +926,105 @@
 )
 
 ListStreamsResponseTypeDef = TypedDict(
     "ListStreamsResponseTypeDef",
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
-    {
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
+RecordingConfigurationSummaryTypeDef = TypedDict(
+    "RecordingConfigurationSummaryTypeDef",
     {
+        "arn": str,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
-        "recordingReconnectWindowSeconds": int,
-        "tags": Mapping[str, str],
-        "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
+        "state": RecordingConfigurationStateType,
+        "tags": Dict[str, str],
     },
-    total=False,
 )
 
-class CreateRecordingConfigurationRequestRequestTypeDef(
-    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
-    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationSummaryTypeDef",
+RecordingConfigurationTypeDef = TypedDict(
+    "RecordingConfigurationTypeDef",
     {
         "arn": str,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
-    },
-)
-_OptionalRecordingConfigurationSummaryTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationSummaryTypeDef",
-    {
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "name": str,
+        "recordingReconnectWindowSeconds": int,
+        "renditionConfiguration": RenditionConfigurationOutputTypeDef,
+        "state": RecordingConfigurationStateType,
         "tags": Dict[str, str],
+        "thumbnailConfiguration": ThumbnailConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
-class RecordingConfigurationSummaryTypeDef(
-    _RequiredRecordingConfigurationSummaryTypeDef, _OptionalRecordingConfigurationSummaryTypeDef
-):
-    pass
-
-_RequiredRecordingConfigurationTypeDef = TypedDict(
-    "_RequiredRecordingConfigurationTypeDef",
+_RequiredCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecordingConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
         "destinationConfiguration": DestinationConfigurationTypeDef,
-        "state": RecordingConfigurationStateType,
     },
 )
-_OptionalRecordingConfigurationTypeDef = TypedDict(
-    "_OptionalRecordingConfigurationTypeDef",
+_OptionalCreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecordingConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "recordingReconnectWindowSeconds": int,
-        "tags": Dict[str, str],
+        "renditionConfiguration": RenditionConfigurationTypeDef,
+        "tags": Mapping[str, str],
         "thumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
-class RecordingConfigurationTypeDef(
-    _RequiredRecordingConfigurationTypeDef, _OptionalRecordingConfigurationTypeDef
+class CreateRecordingConfigurationRequestRequestTypeDef(
+    _RequiredCreateRecordingConfigurationRequestRequestTypeDef,
+    _OptionalCreateRecordingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 ListRecordingConfigurationsResponseTypeDef = TypedDict(
     "ListRecordingConfigurationsResponseTypeDef",
     {
         "nextToken": str,
         "recordingConfigurations": List[RecordingConfigurationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRecordingConfigurationResponseTypeDef = TypedDict(
     "CreateRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecordingConfigurationResponseTypeDef = TypedDict(
     "GetRecordingConfigurationResponseTypeDef",
     {
         "recordingConfiguration": RecordingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamSessionTypeDef = TypedDict(
     "StreamSessionTypeDef",
     {
         "channel": ChannelTypeDef,
         "endTime": datetime,
         "ingestConfiguration": IngestConfigurationTypeDef,
         "recordingConfiguration": RecordingConfigurationTypeDef,
         "startTime": datetime,
         "streamId": str,
         "truncatedEvents": List[StreamEventTypeDef],
     },
-    total=False,
 )
 
 GetStreamSessionResponseTypeDef = TypedDict(
     "GetStreamSessionResponseTypeDef",
     {
         "streamSession": StreamSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs.egg-info/PKG-INFO` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.28.0
-Summary: Type annotations for boto3.IVS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.4
+Summary: Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivs?color=blue)](https://pypistats.org/packages/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
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
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,16 +318,20 @@
     ListChannelsPaginatorName,
     ListPlaybackKeyPairsPaginatorName,
     ListRecordingConfigurationsPaginatorName,
     ListStreamKeysPaginatorName,
     ListStreamsPaginatorName,
     RecordingConfigurationStateType,
     RecordingModeType,
+    RenditionConfigurationRenditionSelectionType,
+    RenditionConfigurationRenditionType,
     StreamHealthType,
     StreamStateType,
+    ThumbnailConfigurationResolutionType,
+    ThumbnailConfigurationStorageType,
     TranscodePresetType,
     IVSServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -346,87 +350,92 @@
 
 ```python
 from mypy_boto3_ivs.type_defs import (
     AudioConfigurationTypeDef,
     BatchErrorTypeDef,
     BatchGetChannelRequestRequestTypeDef,
     ChannelTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetStreamKeyRequestRequestTypeDef,
     StreamKeyTypeDef,
     BatchStartViewerSessionRevocationErrorTypeDef,
     BatchStartViewerSessionRevocationViewerSessionTypeDef,
     ChannelSummaryTypeDef,
     CreateChannelRequestRequestTypeDef,
+    RenditionConfigurationTypeDef,
     ThumbnailConfigurationTypeDef,
     CreateStreamKeyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeletePlaybackKeyPairRequestRequestTypeDef,
     DeleteRecordingConfigurationRequestRequestTypeDef,
     DeleteStreamKeyRequestRequestTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     S3DestinationConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelRequestRequestTypeDef,
     GetPlaybackKeyPairRequestRequestTypeDef,
     PlaybackKeyPairTypeDef,
     GetRecordingConfigurationRequestRequestTypeDef,
     GetStreamKeyRequestRequestTypeDef,
     GetStreamRequestRequestTypeDef,
     StreamTypeDef,
     GetStreamSessionRequestRequestTypeDef,
     ImportPlaybackKeyPairRequestRequestTypeDef,
     VideoConfigurationTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
     ListPlaybackKeyPairsRequestRequestTypeDef,
     PlaybackKeyPairSummaryTypeDef,
-    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
     ListRecordingConfigurationsRequestRequestTypeDef,
-    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListStreamKeysRequestRequestTypeDef,
     StreamKeySummaryTypeDef,
     ListStreamSessionsRequestRequestTypeDef,
     StreamSessionSummaryTypeDef,
     StreamFiltersTypeDef,
     StreamSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutMetadataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    RenditionConfigurationOutputTypeDef,
+    ThumbnailConfigurationOutputTypeDef,
     StartViewerSessionRevocationRequestRequestTypeDef,
     StopStreamRequestRequestTypeDef,
     StreamEventTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     BatchGetChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChannelResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UpdateChannelResponseTypeDef,
     BatchGetStreamKeyResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateStreamKeyResponseTypeDef,
     GetStreamKeyResponseTypeDef,
     BatchStartViewerSessionRevocationResponseTypeDef,
     BatchStartViewerSessionRevocationRequestRequestTypeDef,
     ListChannelsResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     GetPlaybackKeyPairResponseTypeDef,
     ImportPlaybackKeyPairResponseTypeDef,
     GetStreamResponseTypeDef,
     IngestConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListPlaybackKeyPairsRequestListPlaybackKeyPairsPaginateTypeDef,
+    ListRecordingConfigurationsRequestListRecordingConfigurationsPaginateTypeDef,
+    ListStreamKeysRequestListStreamKeysPaginateTypeDef,
     ListPlaybackKeyPairsResponseTypeDef,
     ListStreamKeysResponseTypeDef,
     ListStreamSessionsResponseTypeDef,
     ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     ListStreamsResponseTypeDef,
-    CreateRecordingConfigurationRequestRequestTypeDef,
     RecordingConfigurationSummaryTypeDef,
     RecordingConfigurationTypeDef,
+    CreateRecordingConfigurationRequestRequestTypeDef,
     ListRecordingConfigurationsResponseTypeDef,
     CreateRecordingConfigurationResponseTypeDef,
     GetRecordingConfigurationResponseTypeDef,
     StreamSessionTypeDef,
     GetStreamSessionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-ivs-1.28.0/mypy_boto3_ivs.egg-info/SOURCES.txt` & `mypy-boto3-ivs-1.28.4/mypy_boto3_ivs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.28.0/setup.py` & `mypy-boto3-ivs-1.28.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivs",
-    version="1.28.0",
+    version="1.28.4",
     packages=["mypy_boto3_ivs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IVS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IVS 1.28.4 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

