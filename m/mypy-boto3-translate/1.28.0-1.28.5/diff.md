# Comparing `tmp/mypy-boto3-translate-1.28.0.tar.gz` & `tmp/mypy-boto3-translate-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-translate-1.28.0.tar", last modified: Thu Jul  6 21:00:49 2023, max compression
+gzip compressed data, was "mypy-boto3-translate-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-translate-1.28.0.tar` & `mypy-boto3-translate-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.038454 mypy-boto3-translate-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-07-06 21:00:49.038454 mypy-boto3-translate-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.038454 mypy-boto3-translate-1.28.0/mypy_boto3_translate/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20156 2023-07-06 20:57:29.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20137 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:28.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.038454 mypy-boto3-translate-1.28.0/mypy_boto3_translate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-07-06 21:00:48.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:00:48.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:48.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:48.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:48.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 21:00:48.000000 mypy-boto3-translate-1.28.0/mypy_boto3_translate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:49.038454 mypy-boto3-translate-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:57:27.000000 mypy-boto3-translate-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.766719 mypy-boto3-translate-1.28.5/mypy_boto3_translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-07-18 19:32:30.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21207 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 19:32:41.000000 mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.774719 mypy-boto3-translate-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-18 19:32:29.000000 mypy-boto3-translate-1.28.5/setup.py
```

### Comparing `mypy-boto3-translate-1.28.0/LICENSE` & `mypy-boto3-translate-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.0/PKG-INFO` & `mypy-boto3-translate-1.28.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-translate
-Version: 1.28.0
-Summary: Type annotations for boto3.Translate 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.5
+Summary: Type annotations for boto3.Translate 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,48 +341,54 @@
     CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
     DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionKeyOutputTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
     PaginatorConfigTypeDef,
+    ParallelDataConfigOutputTypeDef,
     ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
     StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
     StopTextTranslationJobResponseTypeDef,
+    TranslationSettingsOutputTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
-    TerminologyPropertiesTypeDef,
-    ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    OutputDataConfigOutputTypeDef,
+    TerminologyPropertiesTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
+    ParallelDataPropertiesTypeDef,
     TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.0/README.md` & `mypy-boto3-translate-1.28.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,48 +309,54 @@
     CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
     DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionKeyOutputTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
     PaginatorConfigTypeDef,
+    ParallelDataConfigOutputTypeDef,
     ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
     StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
     StopTextTranslationJobResponseTypeDef,
+    TranslationSettingsOutputTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
-    TerminologyPropertiesTypeDef,
-    ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    OutputDataConfigOutputTypeDef,
+    TerminologyPropertiesTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
+    ParallelDataPropertiesTypeDef,
     TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/__init__.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/__init__.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/__main__.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Translate 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Translate 1.28.5\nVersion:         1.28.5\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate\nOther"
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

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/client.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/client.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/literals.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/literals.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/paginator.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/paginator.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/type_defs.py` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -32,61 +32,66 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TermTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
     "CreateParallelDataResponseTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
     "DeleteParallelDataResponseTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
     "DocumentTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionKeyOutputTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
     "TerminologyDataTypeDef",
+    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
     "LanguageTypeDef",
     "ListLanguagesRequestRequestTypeDef",
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTerminologiesRequestRequestTypeDef",
     "TextTranslationJobFilterTypeDef",
     "PaginatorConfigTypeDef",
+    "ParallelDataConfigOutputTypeDef",
     "ResponseMetadataTypeDef",
     "TranslationSettingsTypeDef",
     "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
     "StopTextTranslationJobResponseTypeDef",
+    "TranslationSettingsOutputTypeDef",
     "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateParallelDataResponseTypeDef",
     "AppliedTerminologyTypeDef",
     "OutputDataConfigTypeDef",
-    "TerminologyPropertiesTypeDef",
-    "ParallelDataPropertiesTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "OutputDataConfigOutputTypeDef",
+    "TerminologyPropertiesTypeDef",
     "ImportTerminologyRequestRequestTypeDef",
     "ListLanguagesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTextTranslationJobsRequestRequestTypeDef",
+    "ParallelDataPropertiesTypeDef",
     "TranslateDocumentRequestRequestTypeDef",
     "TranslateTextRequestRequestTypeDef",
     "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
     "TextTranslationJobPropertiesTypeDef",
     "GetTerminologyResponseTypeDef",
@@ -100,15 +105,14 @@
 
 TermTypeDef = TypedDict(
     "TermTypeDef",
     {
         "SourceText": str,
         "TargetText": str,
     },
-    total=False,
 )
 
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "Type": Literal["KMS"],
         "Id": str,
@@ -181,14 +185,22 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionKeyOutputTypeDef = TypedDict(
+    "EncryptionKeyOutputTypeDef",
+    {
+        "Type": Literal["KMS"],
+        "Id": str,
+    },
+)
+
 GetParallelDataRequestRequestTypeDef = TypedDict(
     "GetParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -210,21 +222,19 @@
     "_OptionalGetTerminologyRequestRequestTypeDef",
     {
         "TerminologyDataFormat": TerminologyDataFormatType,
     },
     total=False,
 )
 
-
 class GetTerminologyRequestRequestTypeDef(
     _RequiredGetTerminologyRequestRequestTypeDef, _OptionalGetTerminologyRequestRequestTypeDef
 ):
     pass
 
-
 TerminologyDataLocationTypeDef = TypedDict(
     "TerminologyDataLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
     },
 )
@@ -240,18 +250,24 @@
     "_OptionalTerminologyDataTypeDef",
     {
         "Directionality": DirectionalityType,
     },
     total=False,
 )
 
-
 class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
     pass
 
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "ContentType": str,
+    },
+)
 
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
         "ContentType": str,
     },
@@ -260,15 +276,14 @@
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "TranslatedDocumentsCount": int,
         "DocumentsWithErrorsCount": int,
         "InputDocumentsCount": int,
     },
-    total=False,
 )
 
 LanguageTypeDef = TypedDict(
     "LanguageTypeDef",
     {
         "LanguageName": str,
         "LanguageCode": str,
@@ -297,14 +312,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
     "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -335,14 +358,22 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ParallelDataConfigOutputTypeDef = TypedDict(
+    "ParallelDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "Format": ParallelDataFormatType,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -380,14 +411,22 @@
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TranslationSettingsOutputTypeDef = TypedDict(
+    "TranslationSettingsOutputTypeDef",
+    {
+        "Formality": FormalityType,
+        "Profanity": Literal["MASK"],
+    },
+)
+
 TranslatedDocumentTypeDef = TypedDict(
     "TranslatedDocumentTypeDef",
     {
         "Content": bytes,
     },
 )
 
@@ -412,15 +451,14 @@
 
 AppliedTerminologyTypeDef = TypedDict(
     "AppliedTerminologyTypeDef",
     {
         "Name": str,
         "Terms": List[TermTypeDef],
     },
-    total=False,
 )
 
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
@@ -429,64 +467,17 @@
     "_OptionalOutputDataConfigTypeDef",
     {
         "EncryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
-
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
-
-TerminologyPropertiesTypeDef = TypedDict(
-    "TerminologyPropertiesTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Arn": str,
-        "SourceLanguageCode": str,
-        "TargetLanguageCodes": List[str],
-        "EncryptionKey": EncryptionKeyTypeDef,
-        "SizeBytes": int,
-        "TermCount": int,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Directionality": DirectionalityType,
-        "Message": str,
-        "SkippedTermCount": int,
-        "Format": TerminologyDataFormatType,
-    },
-    total=False,
-)
-
-ParallelDataPropertiesTypeDef = TypedDict(
-    "ParallelDataPropertiesTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Description": str,
-        "Status": ParallelDataStatusType,
-        "SourceLanguageCode": str,
-        "TargetLanguageCodes": List[str],
-        "ParallelDataConfig": ParallelDataConfigTypeDef,
-        "Message": str,
-        "ImportedDataSize": int,
-        "ImportedRecordCount": int,
-        "FailedRecordCount": int,
-        "SkippedRecordCount": int,
-        "EncryptionKey": EncryptionKeyTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -495,22 +486,20 @@
     "_OptionalUpdateParallelDataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateParallelDataRequestRequestTypeDef(
     _RequiredUpdateParallelDataRequestRequestTypeDef,
     _OptionalUpdateParallelDataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -521,35 +510,53 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
 ):
     pass
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+OutputDataConfigOutputTypeDef = TypedDict(
+    "OutputDataConfigOutputTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "S3Uri": str,
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+TerminologyPropertiesTypeDef = TypedDict(
+    "TerminologyPropertiesTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "Name": str,
+        "Description": str,
+        "Arn": str,
+        "SourceLanguageCode": str,
+        "TargetLanguageCodes": List[str],
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
+        "SizeBytes": int,
+        "TermCount": int,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Directionality": DirectionalityType,
+        "Message": str,
+        "SkippedTermCount": int,
+        "Format": TerminologyDataFormatType,
     },
 )
 
 _RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
     "_RequiredImportTerminologyRequestRequestTypeDef",
     {
         "Name": str,
@@ -563,41 +570,70 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ImportTerminologyRequestRequestTypeDef(
     _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
 ):
     pass
 
-
 ListLanguagesResponseTypeDef = TypedDict(
     "ListLanguagesResponseTypeDef",
     {
         "Languages": List[LanguageTypeDef],
         "DisplayLanguageCode": DisplayLanguageCodeType,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
     "ListTextTranslationJobsRequestRequestTypeDef",
     {
         "Filter": TextTranslationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ParallelDataPropertiesTypeDef = TypedDict(
+    "ParallelDataPropertiesTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Description": str,
+        "Status": ParallelDataStatusType,
+        "SourceLanguageCode": str,
+        "TargetLanguageCodes": List[str],
+        "ParallelDataConfig": ParallelDataConfigOutputTypeDef,
+        "Message": str,
+        "ImportedDataSize": int,
+        "ImportedRecordCount": int,
+        "FailedRecordCount": int,
+        "SkippedRecordCount": int,
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+    },
+)
+
 _RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateDocumentRequestRequestTypeDef",
     {
         "Document": DocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -607,21 +643,19 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class TranslateDocumentRequestRequestTypeDef(
     _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -631,41 +665,39 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
-
 TranslateDocumentResponseTypeDef = TypedDict(
     "TranslateDocumentResponseTypeDef",
     {
         "TranslatedDocument": TranslatedDocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
-        "AppliedSettings": TranslationSettingsTypeDef,
+        "AppliedSettings": TranslationSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
-        "AppliedSettings": TranslationSettingsTypeDef,
+        "AppliedSettings": TranslationSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTextTranslationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextTranslationJobRequestRequestTypeDef",
     {
@@ -684,42 +716,39 @@
         "TerminologyNames": Sequence[str],
         "ParallelDataNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class StartTextTranslationJobRequestRequestTypeDef(
     _RequiredStartTextTranslationJobRequestRequestTypeDef,
     _OptionalStartTextTranslationJobRequestRequestTypeDef,
 ):
     pass
 
-
 TextTranslationJobPropertiesTypeDef = TypedDict(
     "TextTranslationJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "JobDetails": JobDetailsTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCodes": List[str],
         "TerminologyNames": List[str],
         "ParallelDataNames": List[str],
         "Message": str,
         "SubmittedTime": datetime,
         "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
         "DataAccessRoleArn": str,
-        "Settings": TranslationSettingsTypeDef,
+        "Settings": TranslationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 GetTerminologyResponseTypeDef = TypedDict(
     "GetTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "TerminologyDataLocation": TerminologyDataLocationTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate/type_defs.pyi` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,60 +32,67 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TermTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
     "CreateParallelDataResponseTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
     "DeleteParallelDataResponseTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
     "DocumentTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionKeyOutputTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
     "TerminologyDataTypeDef",
+    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
     "LanguageTypeDef",
     "ListLanguagesRequestRequestTypeDef",
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTerminologiesRequestRequestTypeDef",
     "TextTranslationJobFilterTypeDef",
     "PaginatorConfigTypeDef",
+    "ParallelDataConfigOutputTypeDef",
     "ResponseMetadataTypeDef",
     "TranslationSettingsTypeDef",
     "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
     "StopTextTranslationJobResponseTypeDef",
+    "TranslationSettingsOutputTypeDef",
     "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateParallelDataResponseTypeDef",
     "AppliedTerminologyTypeDef",
     "OutputDataConfigTypeDef",
-    "TerminologyPropertiesTypeDef",
-    "ParallelDataPropertiesTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "OutputDataConfigOutputTypeDef",
+    "TerminologyPropertiesTypeDef",
     "ImportTerminologyRequestRequestTypeDef",
     "ListLanguagesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTextTranslationJobsRequestRequestTypeDef",
+    "ParallelDataPropertiesTypeDef",
     "TranslateDocumentRequestRequestTypeDef",
     "TranslateTextRequestRequestTypeDef",
     "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
     "TextTranslationJobPropertiesTypeDef",
     "GetTerminologyResponseTypeDef",
@@ -99,15 +106,14 @@
 
 TermTypeDef = TypedDict(
     "TermTypeDef",
     {
         "SourceText": str,
         "TargetText": str,
     },
-    total=False,
 )
 
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "Type": Literal["KMS"],
         "Id": str,
@@ -180,14 +186,22 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionKeyOutputTypeDef = TypedDict(
+    "EncryptionKeyOutputTypeDef",
+    {
+        "Type": Literal["KMS"],
+        "Id": str,
+    },
+)
+
 GetParallelDataRequestRequestTypeDef = TypedDict(
     "GetParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -209,19 +223,21 @@
     "_OptionalGetTerminologyRequestRequestTypeDef",
     {
         "TerminologyDataFormat": TerminologyDataFormatType,
     },
     total=False,
 )
 
+
 class GetTerminologyRequestRequestTypeDef(
     _RequiredGetTerminologyRequestRequestTypeDef, _OptionalGetTerminologyRequestRequestTypeDef
 ):
     pass
 
+
 TerminologyDataLocationTypeDef = TypedDict(
     "TerminologyDataLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
     },
 )
@@ -237,17 +253,27 @@
     "_OptionalTerminologyDataTypeDef",
     {
         "Directionality": DirectionalityType,
     },
     total=False,
 )
 
+
 class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
     pass
 
+
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "ContentType": str,
+    },
+)
+
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
         "ContentType": str,
     },
 )
@@ -255,15 +281,14 @@
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "TranslatedDocumentsCount": int,
         "DocumentsWithErrorsCount": int,
         "InputDocumentsCount": int,
     },
-    total=False,
 )
 
 LanguageTypeDef = TypedDict(
     "LanguageTypeDef",
     {
         "LanguageName": str,
         "LanguageCode": str,
@@ -292,14 +317,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ListTerminologiesRequestListTerminologiesPaginateTypeDef = TypedDict(
     "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -330,14 +363,22 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ParallelDataConfigOutputTypeDef = TypedDict(
+    "ParallelDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "Format": ParallelDataFormatType,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -375,14 +416,22 @@
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+TranslationSettingsOutputTypeDef = TypedDict(
+    "TranslationSettingsOutputTypeDef",
+    {
+        "Formality": FormalityType,
+        "Profanity": Literal["MASK"],
+    },
+)
+
 TranslatedDocumentTypeDef = TypedDict(
     "TranslatedDocumentTypeDef",
     {
         "Content": bytes,
     },
 )
 
@@ -407,15 +456,14 @@
 
 AppliedTerminologyTypeDef = TypedDict(
     "AppliedTerminologyTypeDef",
     {
         "Name": str,
         "Terms": List[TermTypeDef],
     },
-    total=False,
 )
 
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
@@ -424,61 +472,18 @@
     "_OptionalOutputDataConfigTypeDef",
     {
         "EncryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
+
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
-TerminologyPropertiesTypeDef = TypedDict(
-    "TerminologyPropertiesTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Arn": str,
-        "SourceLanguageCode": str,
-        "TargetLanguageCodes": List[str],
-        "EncryptionKey": EncryptionKeyTypeDef,
-        "SizeBytes": int,
-        "TermCount": int,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Directionality": DirectionalityType,
-        "Message": str,
-        "SkippedTermCount": int,
-        "Format": TerminologyDataFormatType,
-    },
-    total=False,
-)
-
-ParallelDataPropertiesTypeDef = TypedDict(
-    "ParallelDataPropertiesTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Description": str,
-        "Status": ParallelDataStatusType,
-        "SourceLanguageCode": str,
-        "TargetLanguageCodes": List[str],
-        "ParallelDataConfig": ParallelDataConfigTypeDef,
-        "Message": str,
-        "ImportedDataSize": int,
-        "ImportedRecordCount": int,
-        "FailedRecordCount": int,
-        "SkippedRecordCount": int,
-        "EncryptionKey": EncryptionKeyTypeDef,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "LatestUpdateAttemptStatus": ParallelDataStatusType,
-        "LatestUpdateAttemptAt": datetime,
-    },
-    total=False,
-)
 
 _RequiredUpdateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
@@ -488,20 +493,22 @@
     "_OptionalUpdateParallelDataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateParallelDataRequestRequestTypeDef(
     _RequiredUpdateParallelDataRequestRequestTypeDef,
     _OptionalUpdateParallelDataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -512,36 +519,58 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+OutputDataConfigOutputTypeDef = TypedDict(
+    "OutputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
+    },
+)
+
+TerminologyPropertiesTypeDef = TypedDict(
+    "TerminologyPropertiesTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Arn": str,
+        "SourceLanguageCode": str,
+        "TargetLanguageCodes": List[str],
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
+        "SizeBytes": int,
+        "TermCount": int,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Directionality": DirectionalityType,
+        "Message": str,
+        "SkippedTermCount": int,
+        "Format": TerminologyDataFormatType,
+    },
+)
+
 _RequiredImportTerminologyRequestRequestTypeDef = TypedDict(
     "_RequiredImportTerminologyRequestRequestTypeDef",
     {
         "Name": str,
         "MergeStrategy": Literal["OVERWRITE"],
         "TerminologyData": TerminologyDataTypeDef,
     },
@@ -552,39 +581,72 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ImportTerminologyRequestRequestTypeDef(
     _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
 ):
     pass
 
+
 ListLanguagesResponseTypeDef = TypedDict(
     "ListLanguagesResponseTypeDef",
     {
         "Languages": List[LanguageTypeDef],
         "DisplayLanguageCode": DisplayLanguageCodeType,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTextTranslationJobsRequestRequestTypeDef = TypedDict(
     "ListTextTranslationJobsRequestRequestTypeDef",
     {
         "Filter": TextTranslationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ParallelDataPropertiesTypeDef = TypedDict(
+    "ParallelDataPropertiesTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Description": str,
+        "Status": ParallelDataStatusType,
+        "SourceLanguageCode": str,
+        "TargetLanguageCodes": List[str],
+        "ParallelDataConfig": ParallelDataConfigOutputTypeDef,
+        "Message": str,
+        "ImportedDataSize": int,
+        "ImportedRecordCount": int,
+        "FailedRecordCount": int,
+        "SkippedRecordCount": int,
+        "EncryptionKey": EncryptionKeyOutputTypeDef,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "LatestUpdateAttemptStatus": ParallelDataStatusType,
+        "LatestUpdateAttemptAt": datetime,
+    },
+)
+
 _RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateDocumentRequestRequestTypeDef",
     {
         "Document": DocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -594,19 +656,21 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class TranslateDocumentRequestRequestTypeDef(
     _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -616,39 +680,41 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
+
 TranslateDocumentResponseTypeDef = TypedDict(
     "TranslateDocumentResponseTypeDef",
     {
         "TranslatedDocument": TranslatedDocumentTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
-        "AppliedSettings": TranslationSettingsTypeDef,
+        "AppliedSettings": TranslationSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
-        "AppliedSettings": TranslationSettingsTypeDef,
+        "AppliedSettings": TranslationSettingsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartTextTranslationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextTranslationJobRequestRequestTypeDef",
     {
@@ -667,40 +733,41 @@
         "TerminologyNames": Sequence[str],
         "ParallelDataNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class StartTextTranslationJobRequestRequestTypeDef(
     _RequiredStartTextTranslationJobRequestRequestTypeDef,
     _OptionalStartTextTranslationJobRequestRequestTypeDef,
 ):
     pass
 
+
 TextTranslationJobPropertiesTypeDef = TypedDict(
     "TextTranslationJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "JobDetails": JobDetailsTypeDef,
         "SourceLanguageCode": str,
         "TargetLanguageCodes": List[str],
         "TerminologyNames": List[str],
         "ParallelDataNames": List[str],
         "Message": str,
         "SubmittedTime": datetime,
         "EndTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
         "DataAccessRoleArn": str,
-        "Settings": TranslationSettingsTypeDef,
+        "Settings": TranslationSettingsOutputTypeDef,
     },
-    total=False,
 )
 
 GetTerminologyResponseTypeDef = TypedDict(
     "GetTerminologyResponseTypeDef",
     {
         "TerminologyProperties": TerminologyPropertiesTypeDef,
         "TerminologyDataLocation": TerminologyDataLocationTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate.egg-info/PKG-INFO` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-translate
-Version: 1.28.0
-Summary: Type annotations for boto3.Translate 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.5
+Summary: Type annotations for boto3.Translate 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,48 +341,54 @@
     CreateParallelDataResponseTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
     DeleteParallelDataResponseTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionKeyOutputTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
     LanguageTypeDef,
     ListLanguagesRequestRequestTypeDef,
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
     PaginatorConfigTypeDef,
+    ParallelDataConfigOutputTypeDef,
     ResponseMetadataTypeDef,
     TranslationSettingsTypeDef,
     StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
     StopTextTranslationJobResponseTypeDef,
+    TranslationSettingsOutputTypeDef,
     TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateParallelDataResponseTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
-    TerminologyPropertiesTypeDef,
-    ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    OutputDataConfigOutputTypeDef,
+    TerminologyPropertiesTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
+    ParallelDataPropertiesTypeDef,
     TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
     TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
```

### Comparing `mypy-boto3-translate-1.28.0/mypy_boto3_translate.egg-info/SOURCES.txt` & `mypy-boto3-translate-1.28.5/mypy_boto3_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.28.0/setup.py` & `mypy-boto3-translate-1.28.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-translate",
-    version="1.28.0",
+    version="1.28.5",
     packages=["mypy_boto3_translate"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Translate 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Translate 1.28.5 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

