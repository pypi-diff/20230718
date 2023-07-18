# Comparing `tmp/mypy-boto3-snowball-1.28.0.tar.gz` & `tmp/mypy-boto3-snowball-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-snowball-1.28.0.tar", last modified: Thu Jul  6 21:00:40 2023, max compression
+gzip compressed data, was "mypy-boto3-snowball-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-snowball-1.28.0.tar` & `mypy-boto3-snowball-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.806438 mypy-boto3-snowball-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-07-06 21:00:40.806438 mypy-boto3-snowball-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15299 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.806438 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23506 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-07-06 20:56:08.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-06 20:56:08.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-06 20:56:08.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-07-06 20:56:09.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27587 2023-07-06 20:56:08.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.806438 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-07-06 21:00:40.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:00:40.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:40.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:40.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:40.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:40.000000 mypy-boto3-snowball-1.28.0/mypy_boto3_snowball.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:40.806438 mypy-boto3-snowball-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:56:07.000000 mypy-boto3-snowball-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.758719 mypy-boto3-snowball-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-07-18 19:32:41.754719 mypy-boto3-snowball-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34275 2023-07-18 19:32:29.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34254 2023-07-18 19:32:28.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 19:32:41.000000 mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.758719 mypy-boto3-snowball-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-18 19:32:27.000000 mypy-boto3-snowball-1.28.5/setup.py
```

### Comparing `mypy-boto3-snowball-1.28.0/LICENSE` & `mypy-boto3-snowball-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.0/PKG-INFO` & `mypy-boto3-snowball-1.28.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snowball
-Version: 1.28.0
-Summary: Type annotations for boto3.Snowball 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.5
+Summary: Type annotations for boto3.Snowball 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,17 +314,19 @@
 ### Literals
 
 `mypy_boto3_snowball.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_snowball.literals import (
+    AddressTypeType,
     ClusterStateType,
     DescribeAddressesPaginatorName,
     DeviceServiceNameType,
+    ImpactLevelType,
     JobStateType,
     JobTypeType,
     ListClusterJobsPaginatorName,
     ListClustersPaginatorName,
     ListCompatibleImagesPaginatorName,
     ListJobsPaginatorName,
     ListLongTermPricingPaginatorName,
@@ -342,115 +344,140 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ClusterStateType) -> bool:
+def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_snowball.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snowball.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
-    NotificationTypeDef,
+    NotificationOutputTypeDef,
     CompatibleImageTypeDef,
     CreateAddressResultTypeDef,
+    NotificationTypeDef,
     JobListEntryTypeDef,
+    PickupDetailsTypeDef,
     CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
     CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
     CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
+    ServiceVersionOutputTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
     DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
+    EKSOnDeviceServiceConfigurationOutputTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
+    Ec2AmiResourceOutputTypeDef,
     Ec2AmiResourceTypeDef,
+    EventTriggerDefinitionOutputTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
     GetSoftwareUpdatesResultTypeDef,
+    INDTaxDocumentsOutputTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
+    PickupDetailsOutputTypeDef,
+    KeyRangeOutputTypeDef,
     KeyRangeTypeDef,
     ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
     ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
     ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
+    ListPickupLocationsRequestRequestTypeDef,
+    NFSOnDeviceServiceConfigurationOutputTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
+    S3OnDeviceServiceConfigurationOutputTypeDef,
+    TGWOnDeviceServiceConfigurationOutputTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
+    TargetOnDeviceServiceOutputTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
+    WirelessConnectionOutputTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
-    CreateAddressRequestRequestTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
+    ListPickupLocationsResultTypeDef,
+    CreateAddressRequestRequestTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
+    DependentServiceOutputTypeDef,
     DependentServiceTypeDef,
+    LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
+    TaxDocumentsOutputTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
+    OnDeviceServiceConfigurationOutputTypeDef,
     OnDeviceServiceConfigurationTypeDef,
+    S3ResourceOutputTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
+    SnowconeDeviceConfigurationOutputTypeDef,
     SnowconeDeviceConfigurationTypeDef,
-    ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
+    ListServiceVersionsRequestRequestTypeDef,
+    JobResourceOutputTypeDef,
     JobResourceTypeDef,
+    DeviceConfigurationOutputTypeDef,
     DeviceConfigurationTypeDef,
     ClusterMetadataTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobMetadataTypeDef,
+    CreateJobRequestRequestTypeDef,
     DescribeClusterResultTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-snowball-1.28.0/README.md` & `mypy-boto3-snowball-1.28.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,17 +282,19 @@
 ### Literals
 
 `mypy_boto3_snowball.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_snowball.literals import (
+    AddressTypeType,
     ClusterStateType,
     DescribeAddressesPaginatorName,
     DeviceServiceNameType,
+    ImpactLevelType,
     JobStateType,
     JobTypeType,
     ListClusterJobsPaginatorName,
     ListClustersPaginatorName,
     ListCompatibleImagesPaginatorName,
     ListJobsPaginatorName,
     ListLongTermPricingPaginatorName,
@@ -310,115 +312,140 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ClusterStateType) -> bool:
+def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_snowball.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snowball.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
-    NotificationTypeDef,
+    NotificationOutputTypeDef,
     CompatibleImageTypeDef,
     CreateAddressResultTypeDef,
+    NotificationTypeDef,
     JobListEntryTypeDef,
+    PickupDetailsTypeDef,
     CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
     CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
     CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
+    ServiceVersionOutputTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
     DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
+    EKSOnDeviceServiceConfigurationOutputTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
+    Ec2AmiResourceOutputTypeDef,
     Ec2AmiResourceTypeDef,
+    EventTriggerDefinitionOutputTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
     GetSoftwareUpdatesResultTypeDef,
+    INDTaxDocumentsOutputTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
+    PickupDetailsOutputTypeDef,
+    KeyRangeOutputTypeDef,
     KeyRangeTypeDef,
     ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
     ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
     ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
+    ListPickupLocationsRequestRequestTypeDef,
+    NFSOnDeviceServiceConfigurationOutputTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
+    S3OnDeviceServiceConfigurationOutputTypeDef,
+    TGWOnDeviceServiceConfigurationOutputTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
+    TargetOnDeviceServiceOutputTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
+    WirelessConnectionOutputTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
-    CreateAddressRequestRequestTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
+    ListPickupLocationsResultTypeDef,
+    CreateAddressRequestRequestTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
+    DependentServiceOutputTypeDef,
     DependentServiceTypeDef,
+    LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
+    TaxDocumentsOutputTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
+    OnDeviceServiceConfigurationOutputTypeDef,
     OnDeviceServiceConfigurationTypeDef,
+    S3ResourceOutputTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
+    SnowconeDeviceConfigurationOutputTypeDef,
     SnowconeDeviceConfigurationTypeDef,
-    ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
+    ListServiceVersionsRequestRequestTypeDef,
+    JobResourceOutputTypeDef,
     JobResourceTypeDef,
+    DeviceConfigurationOutputTypeDef,
     DeviceConfigurationTypeDef,
     ClusterMetadataTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobMetadataTypeDef,
+    CreateJobRequestRequestTypeDef,
     DescribeClusterResultTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/__init__.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/__init__.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/__main__.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Snowball 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Snowball 1.28.5\nVersion:         1.28.5\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball\nOther"
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

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/client.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    ImpactLevelType,
     JobTypeType,
     LongTermPricingTypeType,
     RemoteManagementType,
     ServiceNameType,
     ShipmentStateType,
     ShippingOptionType,
     SnowballCapacityType,
@@ -56,17 +57,19 @@
     GetSoftwareUpdatesResultTypeDef,
     JobResourceTypeDef,
     ListClusterJobsResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
+    ListPickupLocationsResultTypeDef,
     ListServiceVersionsResultTypeDef,
     NotificationTypeDef,
     OnDeviceServiceConfigurationTypeDef,
+    PickupDetailsTypeDef,
     TaxDocumentsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -198,30 +201,32 @@
         Notification: NotificationTypeDef = ...,
         ClusterId: str = ...,
         SnowballType: SnowballTypeType = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
-        LongTermPricingId: str = ...
+        LongTermPricingId: str = ...,
+        ImpactLevel: ImpactLevelType = ...,
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> CreateJobResultTypeDef:
         """
         Creates a job to import or export data between Amazon S3 and your on-premises
         data center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_job)
         """
 
     def create_long_term_pricing(
         self,
         *,
         LongTermPricingType: LongTermPricingTypeType,
-        IsLongTermPricingAutoRenew: bool = ...,
-        SnowballType: SnowballTypeType = ...
+        SnowballType: SnowballTypeType,
+        IsLongTermPricingAutoRenew: bool = ...
     ) -> CreateLongTermPricingResultTypeDef:
         """
         Creates a job with the long-term usage option for a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_long_term_pricing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_long_term_pricing)
         """
@@ -354,17 +359,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#list_clusters)
         """
 
     def list_compatible_images(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListCompatibleImagesResultTypeDef:
         """
-        This action returns a list of the different Amazon EC2 Amazon Machine Images
-        (AMIs) that are owned by your Amazon Web Services accountthat would be supported
-        for use on a Snow device.
+        This action returns a list of the different Amazon EC2-compatible Amazon Machine
+        Images (AMIs) that are owned by your Amazon Web Services accountthat would be
+        supported for use on a Snow device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_compatible_images)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#list_compatible_images)
         """
 
     def list_jobs(self, *, MaxResults: int = ..., NextToken: str = ...) -> ListJobsResultTypeDef:
         """
@@ -380,14 +385,24 @@
         """
         Lists all long-term pricing types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_long_term_pricing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#list_long_term_pricing)
         """
 
+    def list_pickup_locations(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListPickupLocationsResultTypeDef:
+        """
+        A list of locations from which the customer can choose to pickup a device.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_pickup_locations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#list_pickup_locations)
+        """
+
     def list_service_versions(
         self,
         *,
         ServiceName: ServiceNameType,
         DependentServices: Sequence[DependentServiceTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -428,15 +443,16 @@
         Notification: NotificationTypeDef = ...,
         Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
-        ForwardingAddressId: str = ...
+        ForwardingAddressId: str = ...,
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         While a job's `JobState` value is `New`, you can update some of the information
         associated with a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#update_job)
```

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/client.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    ImpactLevelType,
     JobTypeType,
     LongTermPricingTypeType,
     RemoteManagementType,
     ServiceNameType,
     ShipmentStateType,
     ShippingOptionType,
     SnowballCapacityType,
@@ -56,17 +57,19 @@
     GetSoftwareUpdatesResultTypeDef,
     JobResourceTypeDef,
     ListClusterJobsResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
+    ListPickupLocationsResultTypeDef,
     ListServiceVersionsResultTypeDef,
     NotificationTypeDef,
     OnDeviceServiceConfigurationTypeDef,
+    PickupDetailsTypeDef,
     TaxDocumentsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -187,29 +190,31 @@
         Notification: NotificationTypeDef = ...,
         ClusterId: str = ...,
         SnowballType: SnowballTypeType = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
-        LongTermPricingId: str = ...
+        LongTermPricingId: str = ...,
+        ImpactLevel: ImpactLevelType = ...,
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> CreateJobResultTypeDef:
         """
         Creates a job to import or export data between Amazon S3 and your on-premises
         data center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_job)
         """
     def create_long_term_pricing(
         self,
         *,
         LongTermPricingType: LongTermPricingTypeType,
-        IsLongTermPricingAutoRenew: bool = ...,
-        SnowballType: SnowballTypeType = ...
+        SnowballType: SnowballTypeType,
+        IsLongTermPricingAutoRenew: bool = ...
     ) -> CreateLongTermPricingResultTypeDef:
         """
         Creates a job with the long-term usage option for a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_long_term_pricing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_long_term_pricing)
         """
@@ -328,17 +333,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#list_clusters)
         """
     def list_compatible_images(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListCompatibleImagesResultTypeDef:
         """
-        This action returns a list of the different Amazon EC2 Amazon Machine Images
-        (AMIs) that are owned by your Amazon Web Services accountthat would be supported
-        for use on a Snow device.
+        This action returns a list of the different Amazon EC2-compatible Amazon Machine
+        Images (AMIs) that are owned by your Amazon Web Services accountthat would be
+        supported for use on a Snow device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_compatible_images)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#list_compatible_images)
         """
     def list_jobs(self, *, MaxResults: int = ..., NextToken: str = ...) -> ListJobsResultTypeDef:
         """
         Returns an array of `JobListEntry` objects of the specified length.
@@ -351,14 +356,23 @@
     ) -> ListLongTermPricingResultTypeDef:
         """
         Lists all long-term pricing types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_long_term_pricing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#list_long_term_pricing)
         """
+    def list_pickup_locations(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListPickupLocationsResultTypeDef:
+        """
+        A list of locations from which the customer can choose to pickup a device.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_pickup_locations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#list_pickup_locations)
+        """
     def list_service_versions(
         self,
         *,
         ServiceName: ServiceNameType,
         DependentServices: Sequence[DependentServiceTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -397,15 +411,16 @@
         Notification: NotificationTypeDef = ...,
         Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
-        ForwardingAddressId: str = ...
+        ForwardingAddressId: str = ...,
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         While a job's `JobState` value is `New`, you can update some of the information
         associated with a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#update_job)
```

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/literals.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 Type annotations for snowball service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_snowball.literals import ClusterStateType
+    from mypy_boto3_snowball.literals import AddressTypeType
 
-    data: ClusterStateType = "AwaitingQuorum"
+    data: AddressTypeType = "AWS_SHIP"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "AddressTypeType",
     "ClusterStateType",
     "DescribeAddressesPaginatorName",
     "DeviceServiceNameType",
+    "ImpactLevelType",
     "JobStateType",
     "JobTypeType",
     "ListClusterJobsPaginatorName",
     "ListClustersPaginatorName",
     "ListCompatibleImagesPaginatorName",
     "ListJobsPaginatorName",
     "ListLongTermPricingPaginatorName",
@@ -43,18 +44,19 @@
     "SnowballServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
+AddressTypeType = Literal["AWS_SHIP", "CUST_PICKUP"]
 ClusterStateType = Literal["AwaitingQuorum", "Cancelled", "Complete", "InUse", "Pending"]
 DescribeAddressesPaginatorName = Literal["describe_addresses"]
 DeviceServiceNameType = Literal["NFS_ON_DEVICE_SERVICE", "S3_ON_DEVICE_SERVICE"]
+ImpactLevelType = Literal["IL2", "IL4", "IL5", "IL6", "IL99"]
 JobStateType = Literal[
     "Cancelled",
     "Complete",
     "InProgress",
     "InTransitToAWS",
     "InTransitToCustomer",
     "Listing",
@@ -69,24 +71,33 @@
 JobTypeType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 ListClusterJobsPaginatorName = Literal["list_cluster_jobs"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListCompatibleImagesPaginatorName = Literal["list_compatible_images"]
 ListJobsPaginatorName = Literal["list_jobs"]
 ListLongTermPricingPaginatorName = Literal["list_long_term_pricing"]
 LongTermPricingTypeType = Literal["OneMonth", "OneYear", "ThreeYear"]
-RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY"]
+RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY", "NOT_INSTALLED"]
 ServiceNameType = Literal["EKS_ANYWHERE", "KUBERNETES"]
 ShipmentStateType = Literal["RECEIVED", "RETURNED"]
 ShippingLabelStatusType = Literal["Failed", "InProgress", "Succeeded", "TimedOut"]
 ShippingOptionType = Literal["EXPRESS", "NEXT_DAY", "SECOND_DAY", "STANDARD"]
 SnowballCapacityType = Literal[
-    "NoPreference", "T100", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
+    "NoPreference", "T100", "T13", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
 ]
 SnowballTypeType = Literal[
-    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C", "V3_5S"
+    "EDGE",
+    "EDGE_C",
+    "EDGE_CG",
+    "EDGE_S",
+    "RACK_5U_C",
+    "SNC1_HDD",
+    "SNC1_SSD",
+    "STANDARD",
+    "V3_5C",
+    "V3_5S",
 ]
 StorageUnitType = Literal["TB"]
 TransferOptionType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 SnowballServiceName = Literal["snowball"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
```

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/literals.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 Type annotations for snowball service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_snowball.literals import ClusterStateType
+    from mypy_boto3_snowball.literals import AddressTypeType
 
-    data: ClusterStateType = "AwaitingQuorum"
+    data: AddressTypeType = "AWS_SHIP"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
+    "AddressTypeType",
     "ClusterStateType",
     "DescribeAddressesPaginatorName",
     "DeviceServiceNameType",
+    "ImpactLevelType",
     "JobStateType",
     "JobTypeType",
     "ListClusterJobsPaginatorName",
     "ListClustersPaginatorName",
     "ListCompatibleImagesPaginatorName",
     "ListJobsPaginatorName",
     "ListLongTermPricingPaginatorName",
@@ -42,17 +45,20 @@
     "SnowballServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
+AddressTypeType = Literal["AWS_SHIP", "CUST_PICKUP"]
 ClusterStateType = Literal["AwaitingQuorum", "Cancelled", "Complete", "InUse", "Pending"]
 DescribeAddressesPaginatorName = Literal["describe_addresses"]
 DeviceServiceNameType = Literal["NFS_ON_DEVICE_SERVICE", "S3_ON_DEVICE_SERVICE"]
+ImpactLevelType = Literal["IL2", "IL4", "IL5", "IL6", "IL99"]
 JobStateType = Literal[
     "Cancelled",
     "Complete",
     "InProgress",
     "InTransitToAWS",
     "InTransitToCustomer",
     "Listing",
@@ -67,24 +73,33 @@
 JobTypeType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 ListClusterJobsPaginatorName = Literal["list_cluster_jobs"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListCompatibleImagesPaginatorName = Literal["list_compatible_images"]
 ListJobsPaginatorName = Literal["list_jobs"]
 ListLongTermPricingPaginatorName = Literal["list_long_term_pricing"]
 LongTermPricingTypeType = Literal["OneMonth", "OneYear", "ThreeYear"]
-RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY"]
+RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY", "NOT_INSTALLED"]
 ServiceNameType = Literal["EKS_ANYWHERE", "KUBERNETES"]
 ShipmentStateType = Literal["RECEIVED", "RETURNED"]
 ShippingLabelStatusType = Literal["Failed", "InProgress", "Succeeded", "TimedOut"]
 ShippingOptionType = Literal["EXPRESS", "NEXT_DAY", "SECOND_DAY", "STANDARD"]
 SnowballCapacityType = Literal[
-    "NoPreference", "T100", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
+    "NoPreference", "T100", "T13", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
 ]
 SnowballTypeType = Literal[
-    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C", "V3_5S"
+    "EDGE",
+    "EDGE_C",
+    "EDGE_CG",
+    "EDGE_S",
+    "RACK_5U_C",
+    "SNC1_HDD",
+    "SNC1_SSD",
+    "STANDARD",
+    "V3_5C",
+    "V3_5S",
 ]
 StorageUnitType = Literal["TB"]
 TransferOptionType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 SnowballServiceName = Literal["snowball"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
```

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/paginator.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/paginator.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/type_defs.py` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 Type annotations for snowball service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_snowball.type_defs import AddressTypeDef
+    from mypy_boto3_snowball.type_defs import AddressOutputTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
+    AddressTypeType,
     ClusterStateType,
     DeviceServiceNameType,
+    ImpactLevelType,
     JobStateType,
     JobTypeType,
     LongTermPricingTypeType,
     RemoteManagementType,
     ServiceNameType,
     ShipmentStateType,
     ShippingLabelStatusType,
@@ -38,100 +40,146 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
-    "NotificationTypeDef",
+    "NotificationOutputTypeDef",
     "CompatibleImageTypeDef",
     "CreateAddressResultTypeDef",
+    "NotificationTypeDef",
     "JobListEntryTypeDef",
+    "PickupDetailsTypeDef",
     "CreateJobResultTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
     "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
     "CreateReturnShippingLabelResultTypeDef",
     "DataTransferTypeDef",
+    "ServiceVersionOutputTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
     "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeReturnShippingLabelRequestRequestTypeDef",
     "DescribeReturnShippingLabelResultTypeDef",
+    "EKSOnDeviceServiceConfigurationOutputTypeDef",
     "EKSOnDeviceServiceConfigurationTypeDef",
+    "Ec2AmiResourceOutputTypeDef",
     "Ec2AmiResourceTypeDef",
+    "EventTriggerDefinitionOutputTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
     "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
     "GetJobUnlockCodeResultTypeDef",
     "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
     "GetSoftwareUpdatesResultTypeDef",
+    "INDTaxDocumentsOutputTypeDef",
     "INDTaxDocumentsTypeDef",
     "JobLogsTypeDef",
+    "PickupDetailsOutputTypeDef",
+    "KeyRangeOutputTypeDef",
     "KeyRangeTypeDef",
     "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
+    "ListPickupLocationsRequestRequestTypeDef",
+    "NFSOnDeviceServiceConfigurationOutputTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
+    "S3OnDeviceServiceConfigurationOutputTypeDef",
+    "TGWOnDeviceServiceConfigurationOutputTypeDef",
     "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
+    "TargetOnDeviceServiceOutputTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
+    "WirelessConnectionOutputTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
-    "CreateAddressRequestRequestTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
+    "ListPickupLocationsResultTypeDef",
+    "CreateAddressRequestRequestTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
     "CreateClusterResultTypeDef",
     "ListClusterJobsResultTypeDef",
     "ListJobsResultTypeDef",
+    "DependentServiceOutputTypeDef",
     "DependentServiceTypeDef",
+    "LambdaResourceOutputTypeDef",
     "LambdaResourceTypeDef",
+    "TaxDocumentsOutputTypeDef",
     "TaxDocumentsTypeDef",
     "ListLongTermPricingResultTypeDef",
+    "OnDeviceServiceConfigurationOutputTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
+    "S3ResourceOutputTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
+    "SnowconeDeviceConfigurationOutputTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
-    "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
+    "ListServiceVersionsRequestRequestTypeDef",
+    "JobResourceOutputTypeDef",
     "JobResourceTypeDef",
+    "DeviceConfigurationOutputTypeDef",
     "DeviceConfigurationTypeDef",
     "ClusterMetadataTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobMetadataTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "DescribeClusterResultTypeDef",
     "DescribeJobResultTypeDef",
 )
 
+AddressOutputTypeDef = TypedDict(
+    "AddressOutputTypeDef",
+    {
+        "AddressId": str,
+        "Name": str,
+        "Company": str,
+        "Street1": str,
+        "Street2": str,
+        "Street3": str,
+        "City": str,
+        "StateOrProvince": str,
+        "PrefectureOrDistrict": str,
+        "Landmark": str,
+        "Country": str,
+        "PostalCode": str,
+        "PhoneNumber": str,
+        "IsRestricted": bool,
+        "Type": AddressTypeType,
+    },
+)
+
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressId": str,
         "Name": str,
         "Company": str,
         "Street1": str,
@@ -141,14 +189,15 @@
         "StateOrProvince": str,
         "PrefectureOrDistrict": str,
         "Landmark": str,
         "Country": str,
         "PostalCode": str,
         "PhoneNumber": str,
         "IsRestricted": bool,
+        "Type": AddressTypeType,
     },
     total=False,
 )
 
 CancelClusterRequestRequestTypeDef = TypedDict(
     "CancelClusterRequestRequestTypeDef",
     {
@@ -167,55 +216,77 @@
     "ClusterListEntryTypeDef",
     {
         "ClusterId": str,
         "ClusterState": ClusterStateType,
         "CreationDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
-NotificationTypeDef = TypedDict(
-    "NotificationTypeDef",
+NotificationOutputTypeDef = TypedDict(
+    "NotificationOutputTypeDef",
     {
         "SnsTopicARN": str,
-        "JobStatesToNotify": Sequence[JobStateType],
+        "JobStatesToNotify": List[JobStateType],
         "NotifyAll": bool,
+        "DevicePickupSnsTopicARN": str,
     },
-    total=False,
 )
 
 CompatibleImageTypeDef = TypedDict(
     "CompatibleImageTypeDef",
     {
         "AmiId": str,
         "Name": str,
     },
-    total=False,
 )
 
 CreateAddressResultTypeDef = TypedDict(
     "CreateAddressResultTypeDef",
     {
         "AddressId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+NotificationTypeDef = TypedDict(
+    "NotificationTypeDef",
+    {
+        "SnsTopicARN": str,
+        "JobStatesToNotify": Sequence[JobStateType],
+        "NotifyAll": bool,
+        "DevicePickupSnsTopicARN": str,
+    },
+    total=False,
+)
+
 JobListEntryTypeDef = TypedDict(
     "JobListEntryTypeDef",
     {
         "JobId": str,
         "JobState": JobStateType,
         "IsMaster": bool,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
         "Description": str,
     },
+)
+
+PickupDetailsTypeDef = TypedDict(
+    "PickupDetailsTypeDef",
+    {
+        "Name": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "IdentificationNumber": str,
+        "IdentificationExpirationDate": Union[datetime, str],
+        "IdentificationIssuingOrg": str,
+        "DevicePickupId": str,
+    },
     total=False,
 )
 
 CreateJobResultTypeDef = TypedDict(
     "CreateJobResultTypeDef",
     {
         "JobId": str,
@@ -223,21 +294,21 @@
     },
 )
 
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
+        "SnowballType": SnowballTypeType,
     },
 )
 _OptionalCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLongTermPricingRequestRequestTypeDef",
     {
         "IsLongTermPricingAutoRenew": bool,
-        "SnowballType": SnowballTypeType,
     },
     total=False,
 )
 
 
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
@@ -288,15 +359,21 @@
     "DataTransferTypeDef",
     {
         "BytesTransferred": int,
         "ObjectsTransferred": int,
         "TotalBytes": int,
         "TotalObjects": int,
     },
-    total=False,
+)
+
+ServiceVersionOutputTypeDef = TypedDict(
+    "ServiceVersionOutputTypeDef",
+    {
+        "Version": str,
+    },
 )
 
 ServiceVersionTypeDef = TypedDict(
     "ServiceVersionTypeDef",
     {
         "Version": str,
     },
@@ -354,23 +431,39 @@
         "Status": ShippingLabelStatusType,
         "ExpirationDate": datetime,
         "ReturnShippingLabelURI": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EKSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "EKSOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "KubernetesVersion": str,
+        "EKSAnywhereVersion": str,
+    },
+)
+
 EKSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
     total=False,
 )
 
+Ec2AmiResourceOutputTypeDef = TypedDict(
+    "Ec2AmiResourceOutputTypeDef",
+    {
+        "AmiId": str,
+        "SnowballAmiId": str,
+    },
+)
+
 _RequiredEc2AmiResourceTypeDef = TypedDict(
     "_RequiredEc2AmiResourceTypeDef",
     {
         "AmiId": str,
     },
 )
 _OptionalEc2AmiResourceTypeDef = TypedDict(
@@ -382,14 +475,21 @@
 )
 
 
 class Ec2AmiResourceTypeDef(_RequiredEc2AmiResourceTypeDef, _OptionalEc2AmiResourceTypeDef):
     pass
 
 
+EventTriggerDefinitionOutputTypeDef = TypedDict(
+    "EventTriggerDefinitionOutputTypeDef",
+    {
+        "EventResourceARN": str,
+    },
+)
+
 EventTriggerDefinitionTypeDef = TypedDict(
     "EventTriggerDefinitionTypeDef",
     {
         "EventResourceARN": str,
     },
     total=False,
 )
@@ -444,14 +544,21 @@
     "GetSoftwareUpdatesResultTypeDef",
     {
         "UpdatesURI": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+INDTaxDocumentsOutputTypeDef = TypedDict(
+    "INDTaxDocumentsOutputTypeDef",
+    {
+        "GSTIN": str,
+    },
+)
+
 INDTaxDocumentsTypeDef = TypedDict(
     "INDTaxDocumentsTypeDef",
     {
         "GSTIN": str,
     },
     total=False,
 )
@@ -459,15 +566,35 @@
 JobLogsTypeDef = TypedDict(
     "JobLogsTypeDef",
     {
         "JobCompletionReportURI": str,
         "JobSuccessLogURI": str,
         "JobFailureLogURI": str,
     },
-    total=False,
+)
+
+PickupDetailsOutputTypeDef = TypedDict(
+    "PickupDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "IdentificationNumber": str,
+        "IdentificationExpirationDate": datetime,
+        "IdentificationIssuingOrg": str,
+        "DevicePickupId": str,
+    },
+)
+
+KeyRangeOutputTypeDef = TypedDict(
+    "KeyRangeOutputTypeDef",
+    {
+        "BeginMarker": str,
+        "EndMarker": str,
+    },
 )
 
 KeyRangeTypeDef = TypedDict(
     "KeyRangeTypeDef",
     {
         "BeginMarker": str,
         "EndMarker": str,
@@ -597,26 +724,60 @@
         "CurrentActiveJob": str,
         "ReplacementJob": str,
         "IsLongTermPricingAutoRenew": bool,
         "LongTermPricingStatus": str,
         "SnowballType": SnowballTypeType,
         "JobIds": List[str],
     },
+)
+
+ListPickupLocationsRequestRequestTypeDef = TypedDict(
+    "ListPickupLocationsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
     total=False,
 )
 
+NFSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "NFSOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": int,
+        "StorageUnit": Literal["TB"],
+    },
+)
+
 NFSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "NFSOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
+S3OnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "S3OnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": float,
+        "StorageUnit": Literal["TB"],
+        "ServiceSize": int,
+        "FaultTolerance": int,
+    },
+)
+
+TGWOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "TGWOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": int,
+        "StorageUnit": Literal["TB"],
+    },
+)
+
 S3OnDeviceServiceConfigurationTypeDef = TypedDict(
     "S3OnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": float,
         "StorageUnit": Literal["TB"],
         "ServiceSize": int,
         "FaultTolerance": int,
@@ -650,14 +811,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+TargetOnDeviceServiceOutputTypeDef = TypedDict(
+    "TargetOnDeviceServiceOutputTypeDef",
+    {
+        "ServiceName": DeviceServiceNameType,
+        "TransferOption": TransferOptionType,
+    },
+)
+
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
     total=False,
@@ -665,15 +834,21 @@
 
 ShipmentTypeDef = TypedDict(
     "ShipmentTypeDef",
     {
         "Status": str,
         "TrackingNumber": str,
     },
-    total=False,
+)
+
+WirelessConnectionOutputTypeDef = TypedDict(
+    "WirelessConnectionOutputTypeDef",
+    {
+        "IsWifiEnabled": bool,
+    },
 )
 
 WirelessConnectionTypeDef = TypedDict(
     "WirelessConnectionTypeDef",
     {
         "IsWifiEnabled": bool,
     },
@@ -707,38 +882,47 @@
 class UpdateLongTermPricingRequestRequestTypeDef(
     _RequiredUpdateLongTermPricingRequestRequestTypeDef,
     _OptionalUpdateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
 
-CreateAddressRequestRequestTypeDef = TypedDict(
-    "CreateAddressRequestRequestTypeDef",
-    {
-        "Address": AddressTypeDef,
-    },
-)
-
 DescribeAddressResultTypeDef = TypedDict(
     "DescribeAddressResultTypeDef",
     {
-        "Address": AddressTypeDef,
+        "Address": AddressOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddressesResultTypeDef = TypedDict(
     "DescribeAddressesResultTypeDef",
     {
-        "Addresses": List[AddressTypeDef],
+        "Addresses": List[AddressOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPickupLocationsResultTypeDef = TypedDict(
+    "ListPickupLocationsResultTypeDef",
+    {
+        "Addresses": List[AddressOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateAddressRequestRequestTypeDef = TypedDict(
+    "CreateAddressRequestRequestTypeDef",
+    {
+        "Address": AddressTypeDef,
+    },
+)
+
 ListClustersResultTypeDef = TypedDict(
     "ListClustersResultTypeDef",
     {
         "ClusterListEntries": List[ClusterListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -776,32 +960,55 @@
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DependentServiceOutputTypeDef = TypedDict(
+    "DependentServiceOutputTypeDef",
+    {
+        "ServiceName": ServiceNameType,
+        "ServiceVersion": ServiceVersionOutputTypeDef,
+    },
+)
+
 DependentServiceTypeDef = TypedDict(
     "DependentServiceTypeDef",
     {
         "ServiceName": ServiceNameType,
         "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
 )
 
+LambdaResourceOutputTypeDef = TypedDict(
+    "LambdaResourceOutputTypeDef",
+    {
+        "LambdaArn": str,
+        "EventTriggers": List[EventTriggerDefinitionOutputTypeDef],
+    },
+)
+
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": Sequence[EventTriggerDefinitionTypeDef],
     },
     total=False,
 )
 
+TaxDocumentsOutputTypeDef = TypedDict(
+    "TaxDocumentsOutputTypeDef",
+    {
+        "IND": INDTaxDocumentsOutputTypeDef,
+    },
+)
+
 TaxDocumentsTypeDef = TypedDict(
     "TaxDocumentsTypeDef",
     {
         "IND": INDTaxDocumentsTypeDef,
     },
     total=False,
 )
@@ -811,25 +1018,44 @@
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "OnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "NFSOnDeviceService": NFSOnDeviceServiceConfigurationOutputTypeDef,
+        "TGWOnDeviceService": TGWOnDeviceServiceConfigurationOutputTypeDef,
+        "EKSOnDeviceService": EKSOnDeviceServiceConfigurationOutputTypeDef,
+        "S3OnDeviceService": S3OnDeviceServiceConfigurationOutputTypeDef,
+    },
+)
+
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
         "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
+S3ResourceOutputTypeDef = TypedDict(
+    "S3ResourceOutputTypeDef",
+    {
+        "BucketArn": str,
+        "KeyRange": KeyRangeOutputTypeDef,
+        "TargetOnDeviceServices": List[TargetOnDeviceServiceOutputTypeDef],
+    },
+)
+
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
         "BucketArn": str,
         "KeyRange": KeyRangeTypeDef,
         "TargetOnDeviceServices": Sequence[TargetOnDeviceServiceTypeDef],
     },
@@ -839,25 +1065,42 @@
 ShippingDetailsTypeDef = TypedDict(
     "ShippingDetailsTypeDef",
     {
         "ShippingOption": ShippingOptionType,
         "InboundShipment": ShipmentTypeDef,
         "OutboundShipment": ShipmentTypeDef,
     },
-    total=False,
+)
+
+SnowconeDeviceConfigurationOutputTypeDef = TypedDict(
+    "SnowconeDeviceConfigurationOutputTypeDef",
+    {
+        "WirelessConnection": WirelessConnectionOutputTypeDef,
+    },
 )
 
 SnowconeDeviceConfigurationTypeDef = TypedDict(
     "SnowconeDeviceConfigurationTypeDef",
     {
         "WirelessConnection": WirelessConnectionTypeDef,
     },
     total=False,
 )
 
+ListServiceVersionsResultTypeDef = TypedDict(
+    "ListServiceVersionsResultTypeDef",
+    {
+        "ServiceVersions": List[ServiceVersionOutputTypeDef],
+        "ServiceName": ServiceNameType,
+        "DependentServices": List[DependentServiceOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListServiceVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceVersionsRequestRequestTypeDef",
     {
         "ServiceName": ServiceNameType,
     },
 )
 _OptionalListServiceVersionsRequestRequestTypeDef = TypedDict(
@@ -874,35 +1117,40 @@
 class ListServiceVersionsRequestRequestTypeDef(
     _RequiredListServiceVersionsRequestRequestTypeDef,
     _OptionalListServiceVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListServiceVersionsResultTypeDef = TypedDict(
-    "ListServiceVersionsResultTypeDef",
+JobResourceOutputTypeDef = TypedDict(
+    "JobResourceOutputTypeDef",
     {
-        "ServiceVersions": List[ServiceVersionTypeDef],
-        "ServiceName": ServiceNameType,
-        "DependentServices": List[DependentServiceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "S3Resources": List[S3ResourceOutputTypeDef],
+        "LambdaResources": List[LambdaResourceOutputTypeDef],
+        "Ec2AmiResources": List[Ec2AmiResourceOutputTypeDef],
     },
 )
 
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
         "LambdaResources": Sequence[LambdaResourceTypeDef],
         "Ec2AmiResources": Sequence[Ec2AmiResourceTypeDef],
     },
     total=False,
 )
 
+DeviceConfigurationOutputTypeDef = TypedDict(
+    "DeviceConfigurationOutputTypeDef",
+    {
+        "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationOutputTypeDef,
+    },
+)
+
 DeviceConfigurationTypeDef = TypedDict(
     "DeviceConfigurationTypeDef",
     {
         "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationTypeDef,
     },
     total=False,
 )
@@ -914,23 +1162,22 @@
         "Description": str,
         "KmsKeyARN": str,
         "RoleARN": str,
         "ClusterState": ClusterStateType,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
-        "Resources": JobResourceTypeDef,
+        "Resources": JobResourceOutputTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
-        "Notification": NotificationTypeDef,
+        "Notification": NotificationOutputTypeDef,
         "ForwardingAddressId": str,
-        "TaxDocuments": TaxDocumentsTypeDef,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "TaxDocuments": TaxDocumentsOutputTypeDef,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
         "AddressId": str,
@@ -1007,74 +1254,79 @@
         "Resources": JobResourceTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
         "Description": str,
         "SnowballCapacityPreference": SnowballCapacityType,
         "ForwardingAddressId": str,
+        "PickupDetails": PickupDetailsTypeDef,
     },
     total=False,
 )
 
 
 class UpdateJobRequestRequestTypeDef(
     _RequiredUpdateJobRequestRequestTypeDef, _OptionalUpdateJobRequestRequestTypeDef
 ):
     pass
 
 
-CreateJobRequestRequestTypeDef = TypedDict(
-    "CreateJobRequestRequestTypeDef",
+JobMetadataTypeDef = TypedDict(
+    "JobMetadataTypeDef",
     {
+        "JobId": str,
+        "JobState": JobStateType,
         "JobType": JobTypeType,
-        "Resources": JobResourceTypeDef,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "SnowballType": SnowballTypeType,
+        "CreationDate": datetime,
+        "Resources": JobResourceOutputTypeDef,
         "Description": str,
-        "AddressId": str,
         "KmsKeyARN": str,
         "RoleARN": str,
+        "AddressId": str,
+        "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
-        "ShippingOption": ShippingOptionType,
-        "Notification": NotificationTypeDef,
+        "Notification": NotificationOutputTypeDef,
+        "DataTransferProgress": DataTransferTypeDef,
+        "JobLogInfo": JobLogsTypeDef,
         "ClusterId": str,
-        "SnowballType": SnowballTypeType,
         "ForwardingAddressId": str,
-        "TaxDocuments": TaxDocumentsTypeDef,
-        "DeviceConfiguration": DeviceConfigurationTypeDef,
+        "TaxDocuments": TaxDocumentsOutputTypeDef,
+        "DeviceConfiguration": DeviceConfigurationOutputTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
+        "ImpactLevel": ImpactLevelType,
+        "PickupDetails": PickupDetailsOutputTypeDef,
+        "SnowballId": str,
     },
-    total=False,
 )
 
-JobMetadataTypeDef = TypedDict(
-    "JobMetadataTypeDef",
+CreateJobRequestRequestTypeDef = TypedDict(
+    "CreateJobRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobState": JobStateType,
         "JobType": JobTypeType,
-        "SnowballType": SnowballTypeType,
-        "CreationDate": datetime,
         "Resources": JobResourceTypeDef,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "Description": str,
+        "AddressId": str,
         "KmsKeyARN": str,
         "RoleARN": str,
-        "AddressId": str,
-        "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
+        "ShippingOption": ShippingOptionType,
         "Notification": NotificationTypeDef,
-        "DataTransferProgress": DataTransferTypeDef,
-        "JobLogInfo": JobLogsTypeDef,
         "ClusterId": str,
+        "SnowballType": SnowballTypeType,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "DeviceConfiguration": DeviceConfigurationTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "ImpactLevel": ImpactLevelType,
+        "PickupDetails": PickupDetailsTypeDef,
     },
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
```

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball/type_defs.pyi` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball/type_defs.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 Type annotations for snowball service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_snowball.type_defs import AddressTypeDef
+    from mypy_boto3_snowball.type_defs import AddressOutputTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
+    AddressTypeType,
     ClusterStateType,
     DeviceServiceNameType,
+    ImpactLevelType,
     JobStateType,
     JobTypeType,
     LongTermPricingTypeType,
     RemoteManagementType,
     ServiceNameType,
     ShipmentStateType,
     ShippingLabelStatusType,
@@ -37,100 +39,146 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
-    "NotificationTypeDef",
+    "NotificationOutputTypeDef",
     "CompatibleImageTypeDef",
     "CreateAddressResultTypeDef",
+    "NotificationTypeDef",
     "JobListEntryTypeDef",
+    "PickupDetailsTypeDef",
     "CreateJobResultTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
     "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
     "CreateReturnShippingLabelResultTypeDef",
     "DataTransferTypeDef",
+    "ServiceVersionOutputTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
     "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeReturnShippingLabelRequestRequestTypeDef",
     "DescribeReturnShippingLabelResultTypeDef",
+    "EKSOnDeviceServiceConfigurationOutputTypeDef",
     "EKSOnDeviceServiceConfigurationTypeDef",
+    "Ec2AmiResourceOutputTypeDef",
     "Ec2AmiResourceTypeDef",
+    "EventTriggerDefinitionOutputTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
     "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
     "GetJobUnlockCodeResultTypeDef",
     "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
     "GetSoftwareUpdatesResultTypeDef",
+    "INDTaxDocumentsOutputTypeDef",
     "INDTaxDocumentsTypeDef",
     "JobLogsTypeDef",
+    "PickupDetailsOutputTypeDef",
+    "KeyRangeOutputTypeDef",
     "KeyRangeTypeDef",
     "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
+    "ListPickupLocationsRequestRequestTypeDef",
+    "NFSOnDeviceServiceConfigurationOutputTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
+    "S3OnDeviceServiceConfigurationOutputTypeDef",
+    "TGWOnDeviceServiceConfigurationOutputTypeDef",
     "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
+    "TargetOnDeviceServiceOutputTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
+    "WirelessConnectionOutputTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
-    "CreateAddressRequestRequestTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
+    "ListPickupLocationsResultTypeDef",
+    "CreateAddressRequestRequestTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
     "CreateClusterResultTypeDef",
     "ListClusterJobsResultTypeDef",
     "ListJobsResultTypeDef",
+    "DependentServiceOutputTypeDef",
     "DependentServiceTypeDef",
+    "LambdaResourceOutputTypeDef",
     "LambdaResourceTypeDef",
+    "TaxDocumentsOutputTypeDef",
     "TaxDocumentsTypeDef",
     "ListLongTermPricingResultTypeDef",
+    "OnDeviceServiceConfigurationOutputTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
+    "S3ResourceOutputTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
+    "SnowconeDeviceConfigurationOutputTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
-    "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
+    "ListServiceVersionsRequestRequestTypeDef",
+    "JobResourceOutputTypeDef",
     "JobResourceTypeDef",
+    "DeviceConfigurationOutputTypeDef",
     "DeviceConfigurationTypeDef",
     "ClusterMetadataTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobMetadataTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "DescribeClusterResultTypeDef",
     "DescribeJobResultTypeDef",
 )
 
+AddressOutputTypeDef = TypedDict(
+    "AddressOutputTypeDef",
+    {
+        "AddressId": str,
+        "Name": str,
+        "Company": str,
+        "Street1": str,
+        "Street2": str,
+        "Street3": str,
+        "City": str,
+        "StateOrProvince": str,
+        "PrefectureOrDistrict": str,
+        "Landmark": str,
+        "Country": str,
+        "PostalCode": str,
+        "PhoneNumber": str,
+        "IsRestricted": bool,
+        "Type": AddressTypeType,
+    },
+)
+
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "AddressId": str,
         "Name": str,
         "Company": str,
         "Street1": str,
@@ -140,14 +188,15 @@
         "StateOrProvince": str,
         "PrefectureOrDistrict": str,
         "Landmark": str,
         "Country": str,
         "PostalCode": str,
         "PhoneNumber": str,
         "IsRestricted": bool,
+        "Type": AddressTypeType,
     },
     total=False,
 )
 
 CancelClusterRequestRequestTypeDef = TypedDict(
     "CancelClusterRequestRequestTypeDef",
     {
@@ -166,55 +215,77 @@
     "ClusterListEntryTypeDef",
     {
         "ClusterId": str,
         "ClusterState": ClusterStateType,
         "CreationDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
-NotificationTypeDef = TypedDict(
-    "NotificationTypeDef",
+NotificationOutputTypeDef = TypedDict(
+    "NotificationOutputTypeDef",
     {
         "SnsTopicARN": str,
-        "JobStatesToNotify": Sequence[JobStateType],
+        "JobStatesToNotify": List[JobStateType],
         "NotifyAll": bool,
+        "DevicePickupSnsTopicARN": str,
     },
-    total=False,
 )
 
 CompatibleImageTypeDef = TypedDict(
     "CompatibleImageTypeDef",
     {
         "AmiId": str,
         "Name": str,
     },
-    total=False,
 )
 
 CreateAddressResultTypeDef = TypedDict(
     "CreateAddressResultTypeDef",
     {
         "AddressId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+NotificationTypeDef = TypedDict(
+    "NotificationTypeDef",
+    {
+        "SnsTopicARN": str,
+        "JobStatesToNotify": Sequence[JobStateType],
+        "NotifyAll": bool,
+        "DevicePickupSnsTopicARN": str,
+    },
+    total=False,
+)
+
 JobListEntryTypeDef = TypedDict(
     "JobListEntryTypeDef",
     {
         "JobId": str,
         "JobState": JobStateType,
         "IsMaster": bool,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
         "Description": str,
     },
+)
+
+PickupDetailsTypeDef = TypedDict(
+    "PickupDetailsTypeDef",
+    {
+        "Name": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "IdentificationNumber": str,
+        "IdentificationExpirationDate": Union[datetime, str],
+        "IdentificationIssuingOrg": str,
+        "DevicePickupId": str,
+    },
     total=False,
 )
 
 CreateJobResultTypeDef = TypedDict(
     "CreateJobResultTypeDef",
     {
         "JobId": str,
@@ -222,21 +293,21 @@
     },
 )
 
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
+        "SnowballType": SnowballTypeType,
     },
 )
 _OptionalCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLongTermPricingRequestRequestTypeDef",
     {
         "IsLongTermPricingAutoRenew": bool,
-        "SnowballType": SnowballTypeType,
     },
     total=False,
 )
 
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
     _OptionalCreateLongTermPricingRequestRequestTypeDef,
@@ -283,15 +354,21 @@
     "DataTransferTypeDef",
     {
         "BytesTransferred": int,
         "ObjectsTransferred": int,
         "TotalBytes": int,
         "TotalObjects": int,
     },
-    total=False,
+)
+
+ServiceVersionOutputTypeDef = TypedDict(
+    "ServiceVersionOutputTypeDef",
+    {
+        "Version": str,
+    },
 )
 
 ServiceVersionTypeDef = TypedDict(
     "ServiceVersionTypeDef",
     {
         "Version": str,
     },
@@ -349,23 +426,39 @@
         "Status": ShippingLabelStatusType,
         "ExpirationDate": datetime,
         "ReturnShippingLabelURI": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EKSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "EKSOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "KubernetesVersion": str,
+        "EKSAnywhereVersion": str,
+    },
+)
+
 EKSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
     total=False,
 )
 
+Ec2AmiResourceOutputTypeDef = TypedDict(
+    "Ec2AmiResourceOutputTypeDef",
+    {
+        "AmiId": str,
+        "SnowballAmiId": str,
+    },
+)
+
 _RequiredEc2AmiResourceTypeDef = TypedDict(
     "_RequiredEc2AmiResourceTypeDef",
     {
         "AmiId": str,
     },
 )
 _OptionalEc2AmiResourceTypeDef = TypedDict(
@@ -375,14 +468,21 @@
     },
     total=False,
 )
 
 class Ec2AmiResourceTypeDef(_RequiredEc2AmiResourceTypeDef, _OptionalEc2AmiResourceTypeDef):
     pass
 
+EventTriggerDefinitionOutputTypeDef = TypedDict(
+    "EventTriggerDefinitionOutputTypeDef",
+    {
+        "EventResourceARN": str,
+    },
+)
+
 EventTriggerDefinitionTypeDef = TypedDict(
     "EventTriggerDefinitionTypeDef",
     {
         "EventResourceARN": str,
     },
     total=False,
 )
@@ -437,14 +537,21 @@
     "GetSoftwareUpdatesResultTypeDef",
     {
         "UpdatesURI": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+INDTaxDocumentsOutputTypeDef = TypedDict(
+    "INDTaxDocumentsOutputTypeDef",
+    {
+        "GSTIN": str,
+    },
+)
+
 INDTaxDocumentsTypeDef = TypedDict(
     "INDTaxDocumentsTypeDef",
     {
         "GSTIN": str,
     },
     total=False,
 )
@@ -452,15 +559,35 @@
 JobLogsTypeDef = TypedDict(
     "JobLogsTypeDef",
     {
         "JobCompletionReportURI": str,
         "JobSuccessLogURI": str,
         "JobFailureLogURI": str,
     },
-    total=False,
+)
+
+PickupDetailsOutputTypeDef = TypedDict(
+    "PickupDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "IdentificationNumber": str,
+        "IdentificationExpirationDate": datetime,
+        "IdentificationIssuingOrg": str,
+        "DevicePickupId": str,
+    },
+)
+
+KeyRangeOutputTypeDef = TypedDict(
+    "KeyRangeOutputTypeDef",
+    {
+        "BeginMarker": str,
+        "EndMarker": str,
+    },
 )
 
 KeyRangeTypeDef = TypedDict(
     "KeyRangeTypeDef",
     {
         "BeginMarker": str,
         "EndMarker": str,
@@ -586,26 +713,60 @@
         "CurrentActiveJob": str,
         "ReplacementJob": str,
         "IsLongTermPricingAutoRenew": bool,
         "LongTermPricingStatus": str,
         "SnowballType": SnowballTypeType,
         "JobIds": List[str],
     },
+)
+
+ListPickupLocationsRequestRequestTypeDef = TypedDict(
+    "ListPickupLocationsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
     total=False,
 )
 
+NFSOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "NFSOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": int,
+        "StorageUnit": Literal["TB"],
+    },
+)
+
 NFSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "NFSOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
+S3OnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "S3OnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": float,
+        "StorageUnit": Literal["TB"],
+        "ServiceSize": int,
+        "FaultTolerance": int,
+    },
+)
+
+TGWOnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "TGWOnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "StorageLimit": int,
+        "StorageUnit": Literal["TB"],
+    },
+)
+
 S3OnDeviceServiceConfigurationTypeDef = TypedDict(
     "S3OnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": float,
         "StorageUnit": Literal["TB"],
         "ServiceSize": int,
         "FaultTolerance": int,
@@ -639,14 +800,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+TargetOnDeviceServiceOutputTypeDef = TypedDict(
+    "TargetOnDeviceServiceOutputTypeDef",
+    {
+        "ServiceName": DeviceServiceNameType,
+        "TransferOption": TransferOptionType,
+    },
+)
+
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
     total=False,
@@ -654,15 +823,21 @@
 
 ShipmentTypeDef = TypedDict(
     "ShipmentTypeDef",
     {
         "Status": str,
         "TrackingNumber": str,
     },
-    total=False,
+)
+
+WirelessConnectionOutputTypeDef = TypedDict(
+    "WirelessConnectionOutputTypeDef",
+    {
+        "IsWifiEnabled": bool,
+    },
 )
 
 WirelessConnectionTypeDef = TypedDict(
     "WirelessConnectionTypeDef",
     {
         "IsWifiEnabled": bool,
     },
@@ -694,38 +869,47 @@
 
 class UpdateLongTermPricingRequestRequestTypeDef(
     _RequiredUpdateLongTermPricingRequestRequestTypeDef,
     _OptionalUpdateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
-CreateAddressRequestRequestTypeDef = TypedDict(
-    "CreateAddressRequestRequestTypeDef",
-    {
-        "Address": AddressTypeDef,
-    },
-)
-
 DescribeAddressResultTypeDef = TypedDict(
     "DescribeAddressResultTypeDef",
     {
-        "Address": AddressTypeDef,
+        "Address": AddressOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddressesResultTypeDef = TypedDict(
     "DescribeAddressesResultTypeDef",
     {
-        "Addresses": List[AddressTypeDef],
+        "Addresses": List[AddressOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListPickupLocationsResultTypeDef = TypedDict(
+    "ListPickupLocationsResultTypeDef",
+    {
+        "Addresses": List[AddressOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateAddressRequestRequestTypeDef = TypedDict(
+    "CreateAddressRequestRequestTypeDef",
+    {
+        "Address": AddressTypeDef,
+    },
+)
+
 ListClustersResultTypeDef = TypedDict(
     "ListClustersResultTypeDef",
     {
         "ClusterListEntries": List[ClusterListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -763,32 +947,55 @@
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DependentServiceOutputTypeDef = TypedDict(
+    "DependentServiceOutputTypeDef",
+    {
+        "ServiceName": ServiceNameType,
+        "ServiceVersion": ServiceVersionOutputTypeDef,
+    },
+)
+
 DependentServiceTypeDef = TypedDict(
     "DependentServiceTypeDef",
     {
         "ServiceName": ServiceNameType,
         "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
 )
 
+LambdaResourceOutputTypeDef = TypedDict(
+    "LambdaResourceOutputTypeDef",
+    {
+        "LambdaArn": str,
+        "EventTriggers": List[EventTriggerDefinitionOutputTypeDef],
+    },
+)
+
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": Sequence[EventTriggerDefinitionTypeDef],
     },
     total=False,
 )
 
+TaxDocumentsOutputTypeDef = TypedDict(
+    "TaxDocumentsOutputTypeDef",
+    {
+        "IND": INDTaxDocumentsOutputTypeDef,
+    },
+)
+
 TaxDocumentsTypeDef = TypedDict(
     "TaxDocumentsTypeDef",
     {
         "IND": INDTaxDocumentsTypeDef,
     },
     total=False,
 )
@@ -798,25 +1005,44 @@
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OnDeviceServiceConfigurationOutputTypeDef = TypedDict(
+    "OnDeviceServiceConfigurationOutputTypeDef",
+    {
+        "NFSOnDeviceService": NFSOnDeviceServiceConfigurationOutputTypeDef,
+        "TGWOnDeviceService": TGWOnDeviceServiceConfigurationOutputTypeDef,
+        "EKSOnDeviceService": EKSOnDeviceServiceConfigurationOutputTypeDef,
+        "S3OnDeviceService": S3OnDeviceServiceConfigurationOutputTypeDef,
+    },
+)
+
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
         "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
+S3ResourceOutputTypeDef = TypedDict(
+    "S3ResourceOutputTypeDef",
+    {
+        "BucketArn": str,
+        "KeyRange": KeyRangeOutputTypeDef,
+        "TargetOnDeviceServices": List[TargetOnDeviceServiceOutputTypeDef],
+    },
+)
+
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
         "BucketArn": str,
         "KeyRange": KeyRangeTypeDef,
         "TargetOnDeviceServices": Sequence[TargetOnDeviceServiceTypeDef],
     },
@@ -826,25 +1052,42 @@
 ShippingDetailsTypeDef = TypedDict(
     "ShippingDetailsTypeDef",
     {
         "ShippingOption": ShippingOptionType,
         "InboundShipment": ShipmentTypeDef,
         "OutboundShipment": ShipmentTypeDef,
     },
-    total=False,
+)
+
+SnowconeDeviceConfigurationOutputTypeDef = TypedDict(
+    "SnowconeDeviceConfigurationOutputTypeDef",
+    {
+        "WirelessConnection": WirelessConnectionOutputTypeDef,
+    },
 )
 
 SnowconeDeviceConfigurationTypeDef = TypedDict(
     "SnowconeDeviceConfigurationTypeDef",
     {
         "WirelessConnection": WirelessConnectionTypeDef,
     },
     total=False,
 )
 
+ListServiceVersionsResultTypeDef = TypedDict(
+    "ListServiceVersionsResultTypeDef",
+    {
+        "ServiceVersions": List[ServiceVersionOutputTypeDef],
+        "ServiceName": ServiceNameType,
+        "DependentServices": List[DependentServiceOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListServiceVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceVersionsRequestRequestTypeDef",
     {
         "ServiceName": ServiceNameType,
     },
 )
 _OptionalListServiceVersionsRequestRequestTypeDef = TypedDict(
@@ -859,35 +1102,40 @@
 
 class ListServiceVersionsRequestRequestTypeDef(
     _RequiredListServiceVersionsRequestRequestTypeDef,
     _OptionalListServiceVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListServiceVersionsResultTypeDef = TypedDict(
-    "ListServiceVersionsResultTypeDef",
+JobResourceOutputTypeDef = TypedDict(
+    "JobResourceOutputTypeDef",
     {
-        "ServiceVersions": List[ServiceVersionTypeDef],
-        "ServiceName": ServiceNameType,
-        "DependentServices": List[DependentServiceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "S3Resources": List[S3ResourceOutputTypeDef],
+        "LambdaResources": List[LambdaResourceOutputTypeDef],
+        "Ec2AmiResources": List[Ec2AmiResourceOutputTypeDef],
     },
 )
 
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
         "LambdaResources": Sequence[LambdaResourceTypeDef],
         "Ec2AmiResources": Sequence[Ec2AmiResourceTypeDef],
     },
     total=False,
 )
 
+DeviceConfigurationOutputTypeDef = TypedDict(
+    "DeviceConfigurationOutputTypeDef",
+    {
+        "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationOutputTypeDef,
+    },
+)
+
 DeviceConfigurationTypeDef = TypedDict(
     "DeviceConfigurationTypeDef",
     {
         "SnowconeDeviceConfiguration": SnowconeDeviceConfigurationTypeDef,
     },
     total=False,
 )
@@ -899,23 +1147,22 @@
         "Description": str,
         "KmsKeyARN": str,
         "RoleARN": str,
         "ClusterState": ClusterStateType,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
-        "Resources": JobResourceTypeDef,
+        "Resources": JobResourceOutputTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
-        "Notification": NotificationTypeDef,
+        "Notification": NotificationOutputTypeDef,
         "ForwardingAddressId": str,
-        "TaxDocuments": TaxDocumentsTypeDef,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "TaxDocuments": TaxDocumentsOutputTypeDef,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
         "AddressId": str,
@@ -988,72 +1235,77 @@
         "Resources": JobResourceTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
         "Description": str,
         "SnowballCapacityPreference": SnowballCapacityType,
         "ForwardingAddressId": str,
+        "PickupDetails": PickupDetailsTypeDef,
     },
     total=False,
 )
 
 class UpdateJobRequestRequestTypeDef(
     _RequiredUpdateJobRequestRequestTypeDef, _OptionalUpdateJobRequestRequestTypeDef
 ):
     pass
 
-CreateJobRequestRequestTypeDef = TypedDict(
-    "CreateJobRequestRequestTypeDef",
+JobMetadataTypeDef = TypedDict(
+    "JobMetadataTypeDef",
     {
+        "JobId": str,
+        "JobState": JobStateType,
         "JobType": JobTypeType,
-        "Resources": JobResourceTypeDef,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "SnowballType": SnowballTypeType,
+        "CreationDate": datetime,
+        "Resources": JobResourceOutputTypeDef,
         "Description": str,
-        "AddressId": str,
         "KmsKeyARN": str,
         "RoleARN": str,
+        "AddressId": str,
+        "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
-        "ShippingOption": ShippingOptionType,
-        "Notification": NotificationTypeDef,
+        "Notification": NotificationOutputTypeDef,
+        "DataTransferProgress": DataTransferTypeDef,
+        "JobLogInfo": JobLogsTypeDef,
         "ClusterId": str,
-        "SnowballType": SnowballTypeType,
         "ForwardingAddressId": str,
-        "TaxDocuments": TaxDocumentsTypeDef,
-        "DeviceConfiguration": DeviceConfigurationTypeDef,
+        "TaxDocuments": TaxDocumentsOutputTypeDef,
+        "DeviceConfiguration": DeviceConfigurationOutputTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationOutputTypeDef,
+        "ImpactLevel": ImpactLevelType,
+        "PickupDetails": PickupDetailsOutputTypeDef,
+        "SnowballId": str,
     },
-    total=False,
 )
 
-JobMetadataTypeDef = TypedDict(
-    "JobMetadataTypeDef",
+CreateJobRequestRequestTypeDef = TypedDict(
+    "CreateJobRequestRequestTypeDef",
     {
-        "JobId": str,
-        "JobState": JobStateType,
         "JobType": JobTypeType,
-        "SnowballType": SnowballTypeType,
-        "CreationDate": datetime,
         "Resources": JobResourceTypeDef,
+        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "Description": str,
+        "AddressId": str,
         "KmsKeyARN": str,
         "RoleARN": str,
-        "AddressId": str,
-        "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
+        "ShippingOption": ShippingOptionType,
         "Notification": NotificationTypeDef,
-        "DataTransferProgress": DataTransferTypeDef,
-        "JobLogInfo": JobLogsTypeDef,
         "ClusterId": str,
+        "SnowballType": SnowballTypeType,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "DeviceConfiguration": DeviceConfigurationTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
-        "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "ImpactLevel": ImpactLevelType,
+        "PickupDetails": PickupDetailsTypeDef,
     },
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
```

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball.egg-info/PKG-INFO` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snowball
-Version: 1.28.0
-Summary: Type annotations for boto3.Snowball 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.5
+Summary: Type annotations for boto3.Snowball 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,17 +314,19 @@
 ### Literals
 
 `mypy_boto3_snowball.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_snowball.literals import (
+    AddressTypeType,
     ClusterStateType,
     DescribeAddressesPaginatorName,
     DeviceServiceNameType,
+    ImpactLevelType,
     JobStateType,
     JobTypeType,
     ListClusterJobsPaginatorName,
     ListClustersPaginatorName,
     ListCompatibleImagesPaginatorName,
     ListJobsPaginatorName,
     ListLongTermPricingPaginatorName,
@@ -342,115 +344,140 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ClusterStateType) -> bool:
+def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_snowball.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snowball.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
-    NotificationTypeDef,
+    NotificationOutputTypeDef,
     CompatibleImageTypeDef,
     CreateAddressResultTypeDef,
+    NotificationTypeDef,
     JobListEntryTypeDef,
+    PickupDetailsTypeDef,
     CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
     CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
     CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
+    ServiceVersionOutputTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
     DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
+    EKSOnDeviceServiceConfigurationOutputTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
+    Ec2AmiResourceOutputTypeDef,
     Ec2AmiResourceTypeDef,
+    EventTriggerDefinitionOutputTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
     GetSoftwareUpdatesResultTypeDef,
+    INDTaxDocumentsOutputTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
+    PickupDetailsOutputTypeDef,
+    KeyRangeOutputTypeDef,
     KeyRangeTypeDef,
     ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
     ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
     ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
     ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
+    ListPickupLocationsRequestRequestTypeDef,
+    NFSOnDeviceServiceConfigurationOutputTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
+    S3OnDeviceServiceConfigurationOutputTypeDef,
+    TGWOnDeviceServiceConfigurationOutputTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
+    TargetOnDeviceServiceOutputTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
+    WirelessConnectionOutputTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
-    CreateAddressRequestRequestTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
+    ListPickupLocationsResultTypeDef,
+    CreateAddressRequestRequestTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
+    DependentServiceOutputTypeDef,
     DependentServiceTypeDef,
+    LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
+    TaxDocumentsOutputTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
+    OnDeviceServiceConfigurationOutputTypeDef,
     OnDeviceServiceConfigurationTypeDef,
+    S3ResourceOutputTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
+    SnowconeDeviceConfigurationOutputTypeDef,
     SnowconeDeviceConfigurationTypeDef,
-    ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
+    ListServiceVersionsRequestRequestTypeDef,
+    JobResourceOutputTypeDef,
     JobResourceTypeDef,
+    DeviceConfigurationOutputTypeDef,
     DeviceConfigurationTypeDef,
     ClusterMetadataTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobMetadataTypeDef,
+    CreateJobRequestRequestTypeDef,
     DescribeClusterResultTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-snowball-1.28.0/mypy_boto3_snowball.egg-info/SOURCES.txt` & `mypy-boto3-snowball-1.28.5/mypy_boto3_snowball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.28.0/setup.py` & `mypy-boto3-snowball-1.28.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-snowball",
-    version="1.28.0",
+    version="1.28.5",
     packages=["mypy_boto3_snowball"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Snowball 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Snowball 1.28.5 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

