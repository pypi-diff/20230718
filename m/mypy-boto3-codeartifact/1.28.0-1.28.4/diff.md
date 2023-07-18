# Comparing `tmp/mypy-boto3-codeartifact-1.28.0.tar.gz` & `tmp/mypy-boto3-codeartifact-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeartifact-1.28.0.tar", last modified: Thu Jul  6 20:59:12 2023, max compression
+gzip compressed data, was "mypy-boto3-codeartifact-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-codeartifact-1.28.0.tar` & `mypy-boto3-codeartifact-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.598251 mypy-boto3-codeartifact-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-07-06 20:59:12.598251 mypy-boto3-codeartifact-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.598251 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34383 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34332 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-06 20:35:41.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-06 20:35:41.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46932 2023-07-06 20:35:43.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46853 2023-07-06 20:35:41.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.598251 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-07-06 20:59:12.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:59:12.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:12.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:12.000000 mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:12.598251 mypy-boto3-codeartifact-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:35:40.000000 mypy-boto3-codeartifact-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34383 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34332 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46438 2023-07-18 01:00:27.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46363 2023-07-18 01:00:26.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/setup.py
```

### Comparing `mypy-boto3-codeartifact-1.28.0/LICENSE` & `mypy-boto3-codeartifact-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.0/PKG-INFO` & `mypy-boto3-codeartifact-1.28.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeartifact
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeArtifact 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.4
+Summary: Type annotations for boto3.CodeArtifact 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
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
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,14 +354,15 @@
 `mypy_boto3_codeartifact.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -376,75 +377,76 @@
     DescribePackageVersionRequestRequestTypeDef,
     DescribeRepositoryRequestRequestTypeDef,
     DisassociateExternalConnectionRequestRequestTypeDef,
     DisposePackageVersionsRequestRequestTypeDef,
     DomainEntryPointTypeDef,
     DomainSummaryTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
-    GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyRequestRequestTypeDef,
     GetPackageVersionAssetRequestRequestTypeDef,
-    GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeRequestRequestTypeDef,
-    GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointRequestRequestTypeDef,
-    GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyRequestRequestTypeDef,
     LicenseInfoTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
     ListPackageVersionAssetsRequestRequestTypeDef,
     ListPackageVersionDependenciesRequestRequestTypeDef,
     PackageDependencyTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
-    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
-    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    PackageOriginRestrictionsOutputTypeDef,
     PackageOriginRestrictionsTypeDef,
-    PaginatorConfigTypeDef,
     PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
+    GetAuthorizationTokenResultTypeDef,
+    GetPackageVersionAssetResultTypeDef,
+    GetPackageVersionReadmeResultTypeDef,
+    GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainResultTypeDef,
     DeleteDomainResultTypeDef,
     DescribeDomainResultTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     UpdateRepositoryRequestRequestTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     PackageVersionOriginTypeDef,
     ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
     PackageVersionSummaryTypeDef,
     PackageDescriptionTypeDef,
     PackageSummaryTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.28.0/README.md` & `mypy-boto3-codeartifact-1.28.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
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
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,14 +322,15 @@
 `mypy_boto3_codeartifact.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -344,75 +345,76 @@
     DescribePackageVersionRequestRequestTypeDef,
     DescribeRepositoryRequestRequestTypeDef,
     DisassociateExternalConnectionRequestRequestTypeDef,
     DisposePackageVersionsRequestRequestTypeDef,
     DomainEntryPointTypeDef,
     DomainSummaryTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
-    GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyRequestRequestTypeDef,
     GetPackageVersionAssetRequestRequestTypeDef,
-    GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeRequestRequestTypeDef,
-    GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointRequestRequestTypeDef,
-    GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyRequestRequestTypeDef,
     LicenseInfoTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
     ListPackageVersionAssetsRequestRequestTypeDef,
     ListPackageVersionDependenciesRequestRequestTypeDef,
     PackageDependencyTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
-    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
-    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    PackageOriginRestrictionsOutputTypeDef,
     PackageOriginRestrictionsTypeDef,
-    PaginatorConfigTypeDef,
     PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
+    GetAuthorizationTokenResultTypeDef,
+    GetPackageVersionAssetResultTypeDef,
+    GetPackageVersionReadmeResultTypeDef,
+    GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainResultTypeDef,
     DeleteDomainResultTypeDef,
     DescribeDomainResultTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     UpdateRepositoryRequestRequestTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     PackageVersionOriginTypeDef,
     ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
     PackageVersionSummaryTypeDef,
     PackageDescriptionTypeDef,
     PackageSummaryTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/__init__.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/__init__.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/__main__.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeArtifact 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CodeArtifact 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact\nOther"
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

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/client.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/client.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/literals.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/literals.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/paginator.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
         """
 
 
@@ -104,15 +104,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackageVersionAssetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionassetspaginator)
         """
 
 
@@ -130,15 +130,15 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         originType: PackageVersionOriginTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackageVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionspaginator)
         """
 
 
@@ -155,30 +155,30 @@
         repository: str,
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         publish: AllowPublishType = ...,
         upstream: AllowUpstreamType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagespaginator)
         """
 
 
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
-        self, *, repositoryPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, repositoryPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRepositoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriespaginator)
         """
 
 
@@ -191,13 +191,13 @@
     def paginate(
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRepositoriesInDomainResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriesindomainpaginator)
         """
```

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/paginator.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listdomainspaginator)
         """
 
 class ListPackageVersionAssetsPaginator(Paginator):
@@ -99,15 +99,15 @@
         domain: str,
         repository: str,
         format: PackageFormatType,
         package: str,
         packageVersion: str,
         domainOwner: str = ...,
         namespace: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackageVersionAssetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionassetspaginator)
         """
 
 class ListPackageVersionsPaginator(Paginator):
@@ -124,15 +124,15 @@
         format: PackageFormatType,
         package: str,
         domainOwner: str = ...,
         namespace: str = ...,
         status: PackageVersionStatusType = ...,
         sortBy: Literal["PUBLISHED_TIME"] = ...,
         originType: PackageVersionOriginTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackageVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackageversionspaginator)
         """
 
 class ListPackagesPaginator(Paginator):
@@ -148,29 +148,29 @@
         repository: str,
         domainOwner: str = ...,
         format: PackageFormatType = ...,
         namespace: str = ...,
         packagePrefix: str = ...,
         publish: AllowPublishType = ...,
         upstream: AllowUpstreamType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listpackagespaginator)
         """
 
 class ListRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriespaginator)
     """
 
     def paginate(
-        self, *, repositoryPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, repositoryPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRepositoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriespaginator)
         """
 
 class ListRepositoriesInDomainPaginator(Paginator):
@@ -182,13 +182,13 @@
     def paginate(
         self,
         *,
         domain: str,
         domainOwner: str = ...,
         administratorAccount: str = ...,
         repositoryPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRepositoriesInDomainResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/paginators/#listrepositoriesindomainpaginator)
         """
```

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/type_defs.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
     "SuccessfulPackageVersionInfoTypeDef",
     "TagTypeDef",
     "DomainDescriptionTypeDef",
     "UpstreamRepositoryTypeDef",
     "DeleteDomainPermissionsPolicyRequestRequestTypeDef",
@@ -59,75 +60,76 @@
     "DescribePackageVersionRequestRequestTypeDef",
     "DescribeRepositoryRequestRequestTypeDef",
     "DisassociateExternalConnectionRequestRequestTypeDef",
     "DisposePackageVersionsRequestRequestTypeDef",
     "DomainEntryPointTypeDef",
     "DomainSummaryTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
-    "GetAuthorizationTokenResultTypeDef",
     "GetDomainPermissionsPolicyRequestRequestTypeDef",
     "GetPackageVersionAssetRequestRequestTypeDef",
-    "GetPackageVersionAssetResultTypeDef",
     "GetPackageVersionReadmeRequestRequestTypeDef",
-    "GetPackageVersionReadmeResultTypeDef",
     "GetRepositoryEndpointRequestRequestTypeDef",
-    "GetRepositoryEndpointResultTypeDef",
     "GetRepositoryPermissionsPolicyRequestRequestTypeDef",
     "LicenseInfoTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
     "ListPackageVersionAssetsRequestRequestTypeDef",
     "ListPackageVersionDependenciesRequestRequestTypeDef",
     "PackageDependencyTypeDef",
-    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
-    "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListPackagesRequestRequestTypeDef",
-    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "PackageOriginRestrictionsOutputTypeDef",
     "PackageOriginRestrictionsTypeDef",
-    "PaginatorConfigTypeDef",
     "PublishPackageVersionRequestRequestTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
+    "GetAuthorizationTokenResultTypeDef",
+    "GetPackageVersionAssetResultTypeDef",
+    "GetPackageVersionReadmeResultTypeDef",
+    "GetRepositoryEndpointResultTypeDef",
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainResultTypeDef",
     "DeleteDomainResultTypeDef",
     "DescribeDomainResultTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "UpdateRepositoryRequestRequestTypeDef",
     "DeleteDomainPermissionsPolicyResultTypeDef",
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     "GetDomainPermissionsPolicyResultTypeDef",
     "GetRepositoryPermissionsPolicyResultTypeDef",
     "PutDomainPermissionsPolicyResultTypeDef",
     "PutRepositoryPermissionsPolicyResultTypeDef",
     "PackageVersionOriginTypeDef",
     "ListDomainsResultTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
     "PackageVersionSummaryTypeDef",
     "PackageDescriptionTypeDef",
     "PackageSummaryTypeDef",
@@ -141,34 +143,23 @@
     "DescribePackageVersionResultTypeDef",
     "ListPackageVersionsResultTypeDef",
     "DescribePackageResultTypeDef",
     "DeletePackageResultTypeDef",
     "ListPackagesResultTypeDef",
 )
 
-_RequiredAssetSummaryTypeDef = TypedDict(
-    "_RequiredAssetSummaryTypeDef",
+AssetSummaryTypeDef = TypedDict(
+    "AssetSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalAssetSummaryTypeDef = TypedDict(
-    "_OptionalAssetSummaryTypeDef",
-    {
         "size": int,
         "hashes": Dict[HashAlgorithmType, str],
     },
-    total=False,
 )
 
-
-class AssetSummaryTypeDef(_RequiredAssetSummaryTypeDef, _OptionalAssetSummaryTypeDef):
-    pass
-
-
 _RequiredAssociateExternalConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateExternalConnectionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "externalConnection": str,
     },
@@ -185,14 +176,25 @@
 class AssociateExternalConnectionRequestRequestTypeDef(
     _RequiredAssociateExternalConnectionRequestRequestTypeDef,
     _OptionalAssociateExternalConnectionRequestRequestTypeDef,
 ):
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
 _RequiredCopyPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredCopyPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "sourceRepository": str,
         "destinationRepository": str,
         "format": PackageFormatType,
@@ -222,24 +224,22 @@
 
 PackageVersionErrorTypeDef = TypedDict(
     "PackageVersionErrorTypeDef",
     {
         "errorCode": PackageVersionErrorCodeType,
         "errorMessage": str,
     },
-    total=False,
 )
 
 SuccessfulPackageVersionInfoTypeDef = TypedDict(
     "SuccessfulPackageVersionInfoTypeDef",
     {
         "revision": str,
         "status": PackageVersionStatusType,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
@@ -255,15 +255,14 @@
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
         "repositoryCount": int,
         "assetSizeBytes": int,
         "s3BucketArn": str,
     },
-    total=False,
 )
 
 UpstreamRepositoryTypeDef = TypedDict(
     "UpstreamRepositoryTypeDef",
     {
         "repositoryName": str,
     },
@@ -295,15 +294,14 @@
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "resourceArn": str,
         "revision": str,
         "document": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDomainRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -573,28 +571,26 @@
 
 DomainEntryPointTypeDef = TypedDict(
     "DomainEntryPointTypeDef",
     {
         "repositoryName": str,
         "externalConnectionName": str,
     },
-    total=False,
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "name": str,
         "owner": str,
         "arn": str,
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
     },
-    total=False,
 )
 
 _RequiredGetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizationTokenRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -612,23 +608,14 @@
 class GetAuthorizationTokenRequestRequestTypeDef(
     _RequiredGetAuthorizationTokenRequestRequestTypeDef,
     _OptionalGetAuthorizationTokenRequestRequestTypeDef,
 ):
     pass
 
 
-GetAuthorizationTokenResultTypeDef = TypedDict(
-    "GetAuthorizationTokenResultTypeDef",
-    {
-        "authorizationToken": str,
-        "expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
@@ -672,25 +659,14 @@
 class GetPackageVersionAssetRequestRequestTypeDef(
     _RequiredGetPackageVersionAssetRequestRequestTypeDef,
     _OptionalGetPackageVersionAssetRequestRequestTypeDef,
 ):
     pass
 
 
-GetPackageVersionAssetResultTypeDef = TypedDict(
-    "GetPackageVersionAssetResultTypeDef",
-    {
-        "asset": StreamingBody,
-        "assetName": str,
-        "packageVersion": str,
-        "packageVersionRevision": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPackageVersionReadmeRequestRequestTypeDef = TypedDict(
     "_RequiredGetPackageVersionReadmeRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -710,27 +686,14 @@
 class GetPackageVersionReadmeRequestRequestTypeDef(
     _RequiredGetPackageVersionReadmeRequestRequestTypeDef,
     _OptionalGetPackageVersionReadmeRequestRequestTypeDef,
 ):
     pass
 
 
-GetPackageVersionReadmeResultTypeDef = TypedDict(
-    "GetPackageVersionReadmeResultTypeDef",
-    {
-        "format": PackageFormatType,
-        "namespace": str,
-        "package": str,
-        "version": str,
-        "versionRevision": str,
-        "readme": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRepositoryEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryEndpointRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
     },
@@ -747,22 +710,14 @@
 class GetRepositoryEndpointRequestRequestTypeDef(
     _RequiredGetRepositoryEndpointRequestRequestTypeDef,
     _OptionalGetRepositoryEndpointRequestRequestTypeDef,
 ):
     pass
 
 
-GetRepositoryEndpointResultTypeDef = TypedDict(
-    "GetRepositoryEndpointResultTypeDef",
-    {
-        "repositoryEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -784,62 +739,35 @@
 
 LicenseInfoTypeDef = TypedDict(
     "LicenseInfoTypeDef",
     {
         "name": str,
         "url": str,
     },
-    total=False,
 )
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
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
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-        "packageVersion": str,
-    },
-)
-_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
-    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPackageVersionAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionAssetsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -897,47 +825,16 @@
     "PackageDependencyTypeDef",
     {
         "namespace": str,
         "package": str,
         "dependencyType": str,
         "versionRequirement": str,
     },
-    total=False,
 )
 
-_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-    },
-)
-_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "status": PackageVersionStatusType,
-        "sortBy": Literal["PUBLISHED_TIME"],
-        "originType": PackageVersionOriginTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
-    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -961,43 +858,14 @@
 class ListPackageVersionsRequestRequestTypeDef(
     _RequiredListPackageVersionsRequestRequestTypeDef,
     _OptionalListPackageVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-    },
-)
-_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "format": PackageFormatType,
-        "namespace": str,
-        "packagePrefix": str,
-        "publish": AllowPublishType,
-        "upstream": AllowUpstreamType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPackagesRequestListPackagesPaginateTypeDef(
-    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
-    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPackagesRequestRequestTypeDef = TypedDict(
     "_RequiredListPackagesRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -1019,39 +887,14 @@
 
 class ListPackagesRequestRequestTypeDef(
     _RequiredListPackagesRequestRequestTypeDef, _OptionalListPackagesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "administratorAccount": str,
-        "repositoryPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
-    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesInDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
@@ -1081,24 +924,14 @@
         "administratorAccount": str,
         "domainName": str,
         "domainOwner": str,
         "arn": str,
         "description": str,
         "createdTime": datetime,
     },
-    total=False,
-)
-
-ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
-    {
-        "repositoryPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListRepositoriesRequestRequestTypeDef = TypedDict(
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": str,
         "maxResults": int,
@@ -1110,30 +943,36 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-PackageOriginRestrictionsTypeDef = TypedDict(
-    "PackageOriginRestrictionsTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+PackageOriginRestrictionsOutputTypeDef = TypedDict(
+    "PackageOriginRestrictionsOutputTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PackageOriginRestrictionsTypeDef = TypedDict(
+    "PackageOriginRestrictionsTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
     },
-    total=False,
 )
 
 _RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredPublishPackageVersionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -1215,34 +1054,21 @@
 RepositoryExternalConnectionInfoTypeDef = TypedDict(
     "RepositoryExternalConnectionInfoTypeDef",
     {
         "externalConnectionName": str,
         "packageFormat": PackageFormatType,
         "status": Literal["Available"],
     },
-    total=False,
 )
 
 UpstreamRepositoryInfoTypeDef = TypedDict(
     "UpstreamRepositoryInfoTypeDef",
     {
         "repositoryName": str,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
@@ -1275,75 +1101,116 @@
 class UpdatePackageVersionsStatusRequestRequestTypeDef(
     _RequiredUpdatePackageVersionsStatusRequestRequestTypeDef,
     _OptionalUpdatePackageVersionsStatusRequestRequestTypeDef,
 ):
     pass
 
 
+GetAuthorizationTokenResultTypeDef = TypedDict(
+    "GetAuthorizationTokenResultTypeDef",
+    {
+        "authorizationToken": str,
+        "expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionAssetResultTypeDef = TypedDict(
+    "GetPackageVersionAssetResultTypeDef",
+    {
+        "asset": StreamingBody,
+        "assetName": str,
+        "packageVersion": str,
+        "packageVersionRevision": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionReadmeResultTypeDef = TypedDict(
+    "GetPackageVersionReadmeResultTypeDef",
+    {
+        "format": PackageFormatType,
+        "namespace": str,
+        "package": str,
+        "version": str,
+        "versionRevision": str,
+        "readme": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRepositoryEndpointResultTypeDef = TypedDict(
+    "GetRepositoryEndpointResultTypeDef",
+    {
+        "repositoryEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPackageVersionAssetsResultTypeDef = TypedDict(
     "ListPackageVersionAssetsResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "assets": List[AssetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublishPackageVersionResultTypeDef = TypedDict(
     "PublishPackageVersionResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "status": PackageVersionStatusType,
         "asset": AssetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyPackageVersionsResultTypeDef = TypedDict(
     "CopyPackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageVersionsResultTypeDef = TypedDict(
     "DeletePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisposePackageVersionsResultTypeDef = TypedDict(
     "DisposePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePackageVersionsStatusResultTypeDef = TypedDict(
     "UpdatePackageVersionsStatusResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "domain": str,
@@ -1361,51 +1228,43 @@
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
 CreateDomainResultTypeDef = TypedDict(
     "CreateDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResultTypeDef = TypedDict(
     "DeleteDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResultTypeDef = TypedDict(
     "DescribeDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "domain": str,
@@ -1454,114 +1313,249 @@
     pass
 
 
 DeleteDomainPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainPermissionsPolicyResultTypeDef = TypedDict(
     "GetDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "GetRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDomainPermissionsPolicyResultTypeDef = TypedDict(
     "PutDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "PutRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackageVersionOriginTypeDef = TypedDict(
     "PackageVersionOriginTypeDef",
     {
         "domainEntryPoint": DomainEntryPointTypeDef,
         "originType": PackageVersionOriginTypeType,
     },
-    total=False,
 )
 
 ListDomainsResultTypeDef = TypedDict(
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+        "packageVersion": str,
+    },
+)
+_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
+    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+    },
+)
+_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "status": PackageVersionStatusType,
+        "sortBy": Literal["PUBLISHED_TIME"],
+        "originType": PackageVersionOriginTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+
+class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
+    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+    },
+)
+_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "format": PackageFormatType,
+        "namespace": str,
+        "packagePrefix": str,
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPackagesRequestListPackagesPaginateTypeDef(
+    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
+    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "administratorAccount": str,
+        "repositoryPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
+    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+):
+    pass
+
+
+ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
+    {
+        "repositoryPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListPackageVersionDependenciesResultTypeDef = TypedDict(
     "ListPackageVersionDependenciesResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "dependencies": List[PackageDependencyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRepositoriesInDomainResultTypeDef = TypedDict(
     "ListRepositoriesInDomainResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRepositoriesResultTypeDef = TypedDict(
     "ListRepositoriesResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
-        "restrictions": PackageOriginRestrictionsTypeDef,
+        "restrictions": PackageOriginRestrictionsOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredPutPackageOriginConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutPackageOriginConfigurationRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -1596,15 +1590,14 @@
         "domainOwner": str,
         "arn": str,
         "description": str,
         "upstreams": List[UpstreamRepositoryInfoTypeDef],
         "externalConnections": List[RepositoryExternalConnectionInfoTypeDef],
         "createdTime": datetime,
     },
-    total=False,
 )
 
 PackageVersionDescriptionTypeDef = TypedDict(
     "PackageVersionDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
@@ -1616,156 +1609,140 @@
         "sourceCodeRepository": str,
         "publishedTime": datetime,
         "licenses": List[LicenseInfoTypeDef],
         "revision": str,
         "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-_RequiredPackageVersionSummaryTypeDef = TypedDict(
-    "_RequiredPackageVersionSummaryTypeDef",
+PackageVersionSummaryTypeDef = TypedDict(
+    "PackageVersionSummaryTypeDef",
     {
         "version": str,
-        "status": PackageVersionStatusType,
-    },
-)
-_OptionalPackageVersionSummaryTypeDef = TypedDict(
-    "_OptionalPackageVersionSummaryTypeDef",
-    {
         "revision": str,
+        "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-
-class PackageVersionSummaryTypeDef(
-    _RequiredPackageVersionSummaryTypeDef, _OptionalPackageVersionSummaryTypeDef
-):
-    pass
-
-
 PackageDescriptionTypeDef = TypedDict(
     "PackageDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "name": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PackageSummaryTypeDef = TypedDict(
     "PackageSummaryTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PutPackageOriginConfigurationResultTypeDef = TypedDict(
     "PutPackageOriginConfigurationResultTypeDef",
     {
         "originConfiguration": PackageOriginConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateExternalConnectionResultTypeDef = TypedDict(
     "AssociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResultTypeDef = TypedDict(
     "CreateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResultTypeDef = TypedDict(
     "DeleteRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoryResultTypeDef = TypedDict(
     "DescribeRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateExternalConnectionResultTypeDef = TypedDict(
     "DisassociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRepositoryResultTypeDef = TypedDict(
     "UpdateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageVersionResultTypeDef = TypedDict(
     "DescribePackageVersionResultTypeDef",
     {
         "packageVersion": PackageVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageVersionsResultTypeDef = TypedDict(
     "ListPackageVersionsResultTypeDef",
     {
         "defaultDisplayVersion": str,
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "versions": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageResultTypeDef = TypedDict(
     "DescribePackageResultTypeDef",
     {
         "package": PackageDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageResultTypeDef = TypedDict(
     "DeletePackageResultTypeDef",
     {
         "deletedPackage": PackageSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResultTypeDef = TypedDict(
     "ListPackagesResultTypeDef",
     {
         "packages": List[PackageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact/type_defs.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssetSummaryTypeDef",
     "AssociateExternalConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CopyPackageVersionsRequestRequestTypeDef",
     "PackageVersionErrorTypeDef",
     "SuccessfulPackageVersionInfoTypeDef",
     "TagTypeDef",
     "DomainDescriptionTypeDef",
     "UpstreamRepositoryTypeDef",
     "DeleteDomainPermissionsPolicyRequestRequestTypeDef",
@@ -58,75 +59,76 @@
     "DescribePackageVersionRequestRequestTypeDef",
     "DescribeRepositoryRequestRequestTypeDef",
     "DisassociateExternalConnectionRequestRequestTypeDef",
     "DisposePackageVersionsRequestRequestTypeDef",
     "DomainEntryPointTypeDef",
     "DomainSummaryTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
-    "GetAuthorizationTokenResultTypeDef",
     "GetDomainPermissionsPolicyRequestRequestTypeDef",
     "GetPackageVersionAssetRequestRequestTypeDef",
-    "GetPackageVersionAssetResultTypeDef",
     "GetPackageVersionReadmeRequestRequestTypeDef",
-    "GetPackageVersionReadmeResultTypeDef",
     "GetRepositoryEndpointRequestRequestTypeDef",
-    "GetRepositoryEndpointResultTypeDef",
     "GetRepositoryPermissionsPolicyRequestRequestTypeDef",
     "LicenseInfoTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
     "ListPackageVersionAssetsRequestRequestTypeDef",
     "ListPackageVersionDependenciesRequestRequestTypeDef",
     "PackageDependencyTypeDef",
-    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
-    "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListPackagesRequestRequestTypeDef",
-    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "PackageOriginRestrictionsOutputTypeDef",
     "PackageOriginRestrictionsTypeDef",
-    "PaginatorConfigTypeDef",
     "PublishPackageVersionRequestRequestTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePackageVersionsStatusRequestRequestTypeDef",
+    "GetAuthorizationTokenResultTypeDef",
+    "GetPackageVersionAssetResultTypeDef",
+    "GetPackageVersionReadmeResultTypeDef",
+    "GetRepositoryEndpointResultTypeDef",
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainResultTypeDef",
     "DeleteDomainResultTypeDef",
     "DescribeDomainResultTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "UpdateRepositoryRequestRequestTypeDef",
     "DeleteDomainPermissionsPolicyResultTypeDef",
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     "GetDomainPermissionsPolicyResultTypeDef",
     "GetRepositoryPermissionsPolicyResultTypeDef",
     "PutDomainPermissionsPolicyResultTypeDef",
     "PutRepositoryPermissionsPolicyResultTypeDef",
     "PackageVersionOriginTypeDef",
     "ListDomainsResultTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
     "PackageVersionSummaryTypeDef",
     "PackageDescriptionTypeDef",
     "PackageSummaryTypeDef",
@@ -140,32 +142,23 @@
     "DescribePackageVersionResultTypeDef",
     "ListPackageVersionsResultTypeDef",
     "DescribePackageResultTypeDef",
     "DeletePackageResultTypeDef",
     "ListPackagesResultTypeDef",
 )
 
-_RequiredAssetSummaryTypeDef = TypedDict(
-    "_RequiredAssetSummaryTypeDef",
+AssetSummaryTypeDef = TypedDict(
+    "AssetSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalAssetSummaryTypeDef = TypedDict(
-    "_OptionalAssetSummaryTypeDef",
-    {
         "size": int,
         "hashes": Dict[HashAlgorithmType, str],
     },
-    total=False,
 )
 
-class AssetSummaryTypeDef(_RequiredAssetSummaryTypeDef, _OptionalAssetSummaryTypeDef):
-    pass
-
 _RequiredAssociateExternalConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateExternalConnectionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "externalConnection": str,
     },
@@ -180,14 +173,25 @@
 
 class AssociateExternalConnectionRequestRequestTypeDef(
     _RequiredAssociateExternalConnectionRequestRequestTypeDef,
     _OptionalAssociateExternalConnectionRequestRequestTypeDef,
 ):
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
 _RequiredCopyPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredCopyPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "sourceRepository": str,
         "destinationRepository": str,
         "format": PackageFormatType,
@@ -215,24 +219,22 @@
 
 PackageVersionErrorTypeDef = TypedDict(
     "PackageVersionErrorTypeDef",
     {
         "errorCode": PackageVersionErrorCodeType,
         "errorMessage": str,
     },
-    total=False,
 )
 
 SuccessfulPackageVersionInfoTypeDef = TypedDict(
     "SuccessfulPackageVersionInfoTypeDef",
     {
         "revision": str,
         "status": PackageVersionStatusType,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
@@ -248,15 +250,14 @@
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
         "repositoryCount": int,
         "assetSizeBytes": int,
         "s3BucketArn": str,
     },
-    total=False,
 )
 
 UpstreamRepositoryTypeDef = TypedDict(
     "UpstreamRepositoryTypeDef",
     {
         "repositoryName": str,
     },
@@ -286,15 +287,14 @@
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "resourceArn": str,
         "revision": str,
         "document": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDomainRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -542,28 +542,26 @@
 
 DomainEntryPointTypeDef = TypedDict(
     "DomainEntryPointTypeDef",
     {
         "repositoryName": str,
         "externalConnectionName": str,
     },
-    total=False,
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "name": str,
         "owner": str,
         "arn": str,
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
     },
-    total=False,
 )
 
 _RequiredGetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizationTokenRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -579,23 +577,14 @@
 
 class GetAuthorizationTokenRequestRequestTypeDef(
     _RequiredGetAuthorizationTokenRequestRequestTypeDef,
     _OptionalGetAuthorizationTokenRequestRequestTypeDef,
 ):
     pass
 
-GetAuthorizationTokenResultTypeDef = TypedDict(
-    "GetAuthorizationTokenResultTypeDef",
-    {
-        "authorizationToken": str,
-        "expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetDomainPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalGetDomainPermissionsPolicyRequestRequestTypeDef = TypedDict(
@@ -635,25 +624,14 @@
 
 class GetPackageVersionAssetRequestRequestTypeDef(
     _RequiredGetPackageVersionAssetRequestRequestTypeDef,
     _OptionalGetPackageVersionAssetRequestRequestTypeDef,
 ):
     pass
 
-GetPackageVersionAssetResultTypeDef = TypedDict(
-    "GetPackageVersionAssetResultTypeDef",
-    {
-        "asset": StreamingBody,
-        "assetName": str,
-        "packageVersion": str,
-        "packageVersionRevision": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPackageVersionReadmeRequestRequestTypeDef = TypedDict(
     "_RequiredGetPackageVersionReadmeRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -671,27 +649,14 @@
 
 class GetPackageVersionReadmeRequestRequestTypeDef(
     _RequiredGetPackageVersionReadmeRequestRequestTypeDef,
     _OptionalGetPackageVersionReadmeRequestRequestTypeDef,
 ):
     pass
 
-GetPackageVersionReadmeResultTypeDef = TypedDict(
-    "GetPackageVersionReadmeResultTypeDef",
-    {
-        "format": PackageFormatType,
-        "namespace": str,
-        "package": str,
-        "version": str,
-        "versionRevision": str,
-        "readme": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRepositoryEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryEndpointRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
     },
@@ -706,22 +671,14 @@
 
 class GetRepositoryEndpointRequestRequestTypeDef(
     _RequiredGetRepositoryEndpointRequestRequestTypeDef,
     _OptionalGetRepositoryEndpointRequestRequestTypeDef,
 ):
     pass
 
-GetRepositoryEndpointResultTypeDef = TypedDict(
-    "GetRepositoryEndpointResultTypeDef",
-    {
-        "repositoryEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPermissionsPolicyRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -741,60 +698,35 @@
 
 LicenseInfoTypeDef = TypedDict(
     "LicenseInfoTypeDef",
     {
         "name": str,
         "url": str,
     },
-    total=False,
 )
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
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
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-        "packageVersion": str,
-    },
-)
-_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
-    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPackageVersionAssetsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionAssetsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
         "package": str,
@@ -848,44 +780,15 @@
     "PackageDependencyTypeDef",
     {
         "namespace": str,
         "package": str,
         "dependencyType": str,
         "versionRequirement": str,
     },
-    total=False,
-)
-
-_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-        "format": PackageFormatType,
-        "package": str,
-    },
 )
-_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "namespace": str,
-        "status": PackageVersionStatusType,
-        "sortBy": Literal["PUBLISHED_TIME"],
-        "originType": PackageVersionOriginTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
-    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "format": PackageFormatType,
@@ -908,41 +811,14 @@
 
 class ListPackageVersionsRequestRequestTypeDef(
     _RequiredListPackageVersionsRequestRequestTypeDef,
     _OptionalListPackageVersionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domain": str,
-        "repository": str,
-    },
-)
-_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "format": PackageFormatType,
-        "namespace": str,
-        "packagePrefix": str,
-        "publish": AllowPublishType,
-        "upstream": AllowUpstreamType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPackagesRequestListPackagesPaginateTypeDef(
-    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
-    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
-):
-    pass
-
 _RequiredListPackagesRequestRequestTypeDef = TypedDict(
     "_RequiredListPackagesRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
     },
 )
@@ -962,37 +838,14 @@
 )
 
 class ListPackagesRequestRequestTypeDef(
     _RequiredListPackagesRequestRequestTypeDef, _OptionalListPackagesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
-    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
-    {
-        "domainOwner": str,
-        "administratorAccount": str,
-        "repositoryPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
-    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
-):
-    pass
-
 _RequiredListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesInDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
 )
 _OptionalListRepositoriesInDomainRequestRequestTypeDef = TypedDict(
@@ -1020,24 +873,14 @@
         "administratorAccount": str,
         "domainName": str,
         "domainOwner": str,
         "arn": str,
         "description": str,
         "createdTime": datetime,
     },
-    total=False,
-)
-
-ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
-    {
-        "repositoryPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 ListRepositoriesRequestRequestTypeDef = TypedDict(
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": str,
         "maxResults": int,
@@ -1049,30 +892,36 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-PackageOriginRestrictionsTypeDef = TypedDict(
-    "PackageOriginRestrictionsTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+PackageOriginRestrictionsOutputTypeDef = TypedDict(
+    "PackageOriginRestrictionsOutputTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PackageOriginRestrictionsTypeDef = TypedDict(
+    "PackageOriginRestrictionsTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
     },
-    total=False,
 )
 
 _RequiredPublishPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredPublishPackageVersionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -1148,34 +997,21 @@
 RepositoryExternalConnectionInfoTypeDef = TypedDict(
     "RepositoryExternalConnectionInfoTypeDef",
     {
         "externalConnectionName": str,
         "packageFormat": PackageFormatType,
         "status": Literal["Available"],
     },
-    total=False,
 )
 
 UpstreamRepositoryInfoTypeDef = TypedDict(
     "UpstreamRepositoryInfoTypeDef",
     {
         "repositoryName": str,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
@@ -1206,75 +1042,116 @@
 
 class UpdatePackageVersionsStatusRequestRequestTypeDef(
     _RequiredUpdatePackageVersionsStatusRequestRequestTypeDef,
     _OptionalUpdatePackageVersionsStatusRequestRequestTypeDef,
 ):
     pass
 
+GetAuthorizationTokenResultTypeDef = TypedDict(
+    "GetAuthorizationTokenResultTypeDef",
+    {
+        "authorizationToken": str,
+        "expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionAssetResultTypeDef = TypedDict(
+    "GetPackageVersionAssetResultTypeDef",
+    {
+        "asset": StreamingBody,
+        "assetName": str,
+        "packageVersion": str,
+        "packageVersionRevision": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionReadmeResultTypeDef = TypedDict(
+    "GetPackageVersionReadmeResultTypeDef",
+    {
+        "format": PackageFormatType,
+        "namespace": str,
+        "package": str,
+        "version": str,
+        "versionRevision": str,
+        "readme": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRepositoryEndpointResultTypeDef = TypedDict(
+    "GetRepositoryEndpointResultTypeDef",
+    {
+        "repositoryEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPackageVersionAssetsResultTypeDef = TypedDict(
     "ListPackageVersionAssetsResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "assets": List[AssetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublishPackageVersionResultTypeDef = TypedDict(
     "PublishPackageVersionResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "status": PackageVersionStatusType,
         "asset": AssetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyPackageVersionsResultTypeDef = TypedDict(
     "CopyPackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageVersionsResultTypeDef = TypedDict(
     "DeletePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisposePackageVersionsResultTypeDef = TypedDict(
     "DisposePackageVersionsResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePackageVersionsStatusResultTypeDef = TypedDict(
     "UpdatePackageVersionsStatusResultTypeDef",
     {
         "successfulVersions": Dict[str, SuccessfulPackageVersionInfoTypeDef],
         "failedVersions": Dict[str, PackageVersionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "domain": str,
@@ -1290,51 +1167,43 @@
 )
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
 CreateDomainResultTypeDef = TypedDict(
     "CreateDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResultTypeDef = TypedDict(
     "DeleteDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResultTypeDef = TypedDict(
     "DescribeDomainResultTypeDef",
     {
         "domain": DomainDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "domain": str,
@@ -1379,114 +1248,241 @@
 ):
     pass
 
 DeleteDomainPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "DeleteRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainPermissionsPolicyResultTypeDef = TypedDict(
     "GetDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "GetRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDomainPermissionsPolicyResultTypeDef = TypedDict(
     "PutDomainPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRepositoryPermissionsPolicyResultTypeDef = TypedDict(
     "PutRepositoryPermissionsPolicyResultTypeDef",
     {
         "policy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackageVersionOriginTypeDef = TypedDict(
     "PackageVersionOriginTypeDef",
     {
         "domainEntryPoint": DomainEntryPointTypeDef,
         "originType": PackageVersionOriginTypeType,
     },
-    total=False,
 )
 
 ListDomainsResultTypeDef = TypedDict(
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+        "packageVersion": str,
+    },
+)
+_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(
+    _RequiredListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    _OptionalListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+        "format": PackageFormatType,
+        "package": str,
+    },
+)
+_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "namespace": str,
+        "status": PackageVersionStatusType,
+        "sortBy": Literal["PUBLISHED_TIME"],
+        "originType": PackageVersionOriginTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
+    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_RequiredListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domain": str,
+        "repository": str,
+    },
+)
+_OptionalListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "_OptionalListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "format": PackageFormatType,
+        "namespace": str,
+        "packagePrefix": str,
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPackagesRequestListPackagesPaginateTypeDef(
+    _RequiredListPackagesRequestListPackagesPaginateTypeDef,
+    _OptionalListPackagesRequestListPackagesPaginateTypeDef,
+):
+    pass
+
+_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = TypedDict(
+    "_OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
+    {
+        "domainOwner": str,
+        "administratorAccount": str,
+        "repositoryPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(
+    _RequiredListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    _OptionalListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+):
+    pass
+
+ListRepositoriesRequestListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
+    {
+        "repositoryPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListPackageVersionDependenciesResultTypeDef = TypedDict(
     "ListPackageVersionDependenciesResultTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "version": str,
         "versionRevision": str,
         "nextToken": str,
         "dependencies": List[PackageDependencyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRepositoriesInDomainResultTypeDef = TypedDict(
     "ListRepositoriesInDomainResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRepositoriesResultTypeDef = TypedDict(
     "ListRepositoriesResultTypeDef",
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
-        "restrictions": PackageOriginRestrictionsTypeDef,
+        "restrictions": PackageOriginRestrictionsOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredPutPackageOriginConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutPackageOriginConfigurationRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -1519,15 +1515,14 @@
         "domainOwner": str,
         "arn": str,
         "description": str,
         "upstreams": List[UpstreamRepositoryInfoTypeDef],
         "externalConnections": List[RepositoryExternalConnectionInfoTypeDef],
         "createdTime": datetime,
     },
-    total=False,
 )
 
 PackageVersionDescriptionTypeDef = TypedDict(
     "PackageVersionDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
@@ -1539,154 +1534,140 @@
         "sourceCodeRepository": str,
         "publishedTime": datetime,
         "licenses": List[LicenseInfoTypeDef],
         "revision": str,
         "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-_RequiredPackageVersionSummaryTypeDef = TypedDict(
-    "_RequiredPackageVersionSummaryTypeDef",
+PackageVersionSummaryTypeDef = TypedDict(
+    "PackageVersionSummaryTypeDef",
     {
         "version": str,
-        "status": PackageVersionStatusType,
-    },
-)
-_OptionalPackageVersionSummaryTypeDef = TypedDict(
-    "_OptionalPackageVersionSummaryTypeDef",
-    {
         "revision": str,
+        "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-class PackageVersionSummaryTypeDef(
-    _RequiredPackageVersionSummaryTypeDef, _OptionalPackageVersionSummaryTypeDef
-):
-    pass
-
 PackageDescriptionTypeDef = TypedDict(
     "PackageDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "name": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PackageSummaryTypeDef = TypedDict(
     "PackageSummaryTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PutPackageOriginConfigurationResultTypeDef = TypedDict(
     "PutPackageOriginConfigurationResultTypeDef",
     {
         "originConfiguration": PackageOriginConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateExternalConnectionResultTypeDef = TypedDict(
     "AssociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResultTypeDef = TypedDict(
     "CreateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResultTypeDef = TypedDict(
     "DeleteRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoryResultTypeDef = TypedDict(
     "DescribeRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateExternalConnectionResultTypeDef = TypedDict(
     "DisassociateExternalConnectionResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRepositoryResultTypeDef = TypedDict(
     "UpdateRepositoryResultTypeDef",
     {
         "repository": RepositoryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageVersionResultTypeDef = TypedDict(
     "DescribePackageVersionResultTypeDef",
     {
         "packageVersion": PackageVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageVersionsResultTypeDef = TypedDict(
     "ListPackageVersionsResultTypeDef",
     {
         "defaultDisplayVersion": str,
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "versions": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageResultTypeDef = TypedDict(
     "DescribePackageResultTypeDef",
     {
         "package": PackageDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageResultTypeDef = TypedDict(
     "DeletePackageResultTypeDef",
     {
         "deletedPackage": PackageSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResultTypeDef = TypedDict(
     "ListPackagesResultTypeDef",
     {
         "packages": List[PackageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact.egg-info/PKG-INFO` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeartifact
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeArtifact 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.4
+Summary: Type annotations for boto3.CodeArtifact 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
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
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,14 +354,15 @@
 `mypy_boto3_codeartifact.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeartifact.type_defs import (
     AssetSummaryTypeDef,
     AssociateExternalConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CopyPackageVersionsRequestRequestTypeDef,
     PackageVersionErrorTypeDef,
     SuccessfulPackageVersionInfoTypeDef,
     TagTypeDef,
     DomainDescriptionTypeDef,
     UpstreamRepositoryTypeDef,
     DeleteDomainPermissionsPolicyRequestRequestTypeDef,
@@ -376,75 +377,76 @@
     DescribePackageVersionRequestRequestTypeDef,
     DescribeRepositoryRequestRequestTypeDef,
     DisassociateExternalConnectionRequestRequestTypeDef,
     DisposePackageVersionsRequestRequestTypeDef,
     DomainEntryPointTypeDef,
     DomainSummaryTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
-    GetAuthorizationTokenResultTypeDef,
     GetDomainPermissionsPolicyRequestRequestTypeDef,
     GetPackageVersionAssetRequestRequestTypeDef,
-    GetPackageVersionAssetResultTypeDef,
     GetPackageVersionReadmeRequestRequestTypeDef,
-    GetPackageVersionReadmeResultTypeDef,
     GetRepositoryEndpointRequestRequestTypeDef,
-    GetRepositoryEndpointResultTypeDef,
     GetRepositoryPermissionsPolicyRequestRequestTypeDef,
     LicenseInfoTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
     ListPackageVersionAssetsRequestRequestTypeDef,
     ListPackageVersionDependenciesRequestRequestTypeDef,
     PackageDependencyTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
-    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
-    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    PackageOriginRestrictionsOutputTypeDef,
     PackageOriginRestrictionsTypeDef,
-    PaginatorConfigTypeDef,
     PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePackageVersionsStatusRequestRequestTypeDef,
+    GetAuthorizationTokenResultTypeDef,
+    GetPackageVersionAssetResultTypeDef,
+    GetPackageVersionReadmeResultTypeDef,
+    GetRepositoryEndpointResultTypeDef,
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainResultTypeDef,
     DeleteDomainResultTypeDef,
     DescribeDomainResultTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     UpdateRepositoryRequestRequestTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
     DeleteRepositoryPermissionsPolicyResultTypeDef,
     GetDomainPermissionsPolicyResultTypeDef,
     GetRepositoryPermissionsPolicyResultTypeDef,
     PutDomainPermissionsPolicyResultTypeDef,
     PutRepositoryPermissionsPolicyResultTypeDef,
     PackageVersionOriginTypeDef,
     ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
+    ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
     PackageVersionSummaryTypeDef,
     PackageDescriptionTypeDef,
     PackageSummaryTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.28.0/mypy_boto3_codeartifact.egg-info/SOURCES.txt` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.0/setup.py` & `mypy-boto3-codeartifact-1.28.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeartifact",
-    version="1.28.0",
+    version="1.28.4",
     packages=["mypy_boto3_codeartifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeArtifact 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CodeArtifact 1.28.4 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

