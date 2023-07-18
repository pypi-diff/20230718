# Comparing `tmp/craft_documents-0.1.1.tar.gz` & `tmp/craft_documents-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft_documents-0.1.1.tar", max compression
+gzip compressed data, was "craft_documents-0.1.2.tar", max compression
```

## Comparing `craft_documents-0.1.1.tar` & `craft_documents-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0        0 2023-07-18 08:48:00.447292 craft_documents-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-18 16:13:47.390728 craft_documents-0.1.1/craft_documents/__init__.py
--rw-r--r--   0        0        0      810 2023-07-18 16:13:47.369726 craft_documents-0.1.1/craft_documents/common/DiskRepresentable.py
--rw-r--r--   0        0        0     4629 2023-07-18 16:18:09.637059 craft_documents-0.1.1/craft_documents/common/Exercise.py
--rw-r--r--   0        0        0     3571 2023-07-18 16:18:15.603824 craft_documents-0.1.1/craft_documents/common/File.py
--rw-r--r--   0        0        0     1348 2023-07-18 16:18:15.603766 craft_documents-0.1.1/craft_documents/common/Folder.py
--rw-r--r--   0        0        0     1291 2023-07-18 16:18:11.002009 craft_documents-0.1.1/craft_documents/common/Header.py
--rw-r--r--   0        0        0      725 2023-07-18 16:18:15.597922 craft_documents-0.1.1/craft_documents/common/Preamble.py
--rw-r--r--   0        0        0    12389 2023-07-18 16:13:47.371992 craft_documents-0.1.1/craft_documents/common/Prompt.py
--rw-r--r--   0        0        0     1381 2023-07-18 16:18:15.133887 craft_documents-0.1.1/craft_documents/common/Prompter.py
--rw-r--r--   0        0        0     7409 2023-07-18 16:18:10.850944 craft_documents-0.1.1/craft_documents/common/Template.py
--rw-r--r--   0        0        0     1942 2023-07-18 16:18:15.097438 craft_documents-0.1.1/craft_documents/common/TexTemplate.py
--rw-r--r--   0        0        0     2338 2023-07-18 16:13:47.373445 craft_documents-0.1.1/craft_documents/common/helpers.py
--rw-r--r--   0        0        0      512 2023-07-18 16:18:14.300283 craft_documents-0.1.1/craft_documents/configuration/AllowEvalValidator.py
--rw-r--r--   0        0        0     6925 2023-07-18 16:18:10.691785 craft_documents-0.1.1/craft_documents/configuration/Configuration.py
--rw-r--r--   0        0        0      967 2023-07-18 16:18:14.213506 craft_documents-0.1.1/craft_documents/configuration/DocumentNameValidator.py
--rw-r--r--   0        0        0     5962 2023-07-18 16:26:54.411808 craft_documents-0.1.1/craft_documents/configuration/DraftExercisesValidator.py
--rw-r--r--   0        0        0     1161 2023-07-18 16:18:13.694218 craft_documents-0.1.1/craft_documents/configuration/HeaderValidator.py
--rw-r--r--   0        0        0      526 2023-07-18 16:18:13.686001 craft_documents-0.1.1/craft_documents/configuration/MultipleExercisesValidator.py
--rw-r--r--   0        0        0     1819 2023-07-18 16:18:13.638487 craft_documents-0.1.1/craft_documents/configuration/PreambleValidator.py
--rw-r--r--   0        0        0      522 2023-07-18 16:18:13.628748 craft_documents-0.1.1/craft_documents/configuration/RemoveCommentsValidator.py
--rw-r--r--   0        0        0      179 2023-07-18 16:13:47.378656 craft_documents-0.1.1/craft_documents/configuration/Semantic.py
--rw-r--r--   0        0        0     1685 2023-07-18 16:18:13.628722 craft_documents-0.1.1/craft_documents/configuration/TokensValidator.py
--rw-r--r--   0        0        0      689 2023-07-18 16:18:13.628685 craft_documents-0.1.1/craft_documents/configuration/UniqueExercisePlaceholdersValidator.py
--rw-r--r--   0        0        0     2391 2023-07-18 16:18:13.628655 craft_documents-0.1.1/craft_documents/configuration/Validator.py
--rw-r--r--   0        0        0      507 2023-07-18 16:18:13.561298 craft_documents-0.1.1/craft_documents/configuration/VerboseValidator.py
--rw-r--r--   0        0        0      608 2023-07-18 16:18:13.506353 craft_documents-0.1.1/craft_documents/debug/Debugger.py
--rw-r--r--   0        0        0      295 2023-07-18 16:33:13.377131 craft_documents-0.1.1/craft_documents/debug/main.py
--rw-r--r--   0        0        0      479 2023-07-18 16:33:13.376572 craft_documents-0.1.1/craft_documents/main.py
--rw-r--r--   0        0        0    10275 2023-07-18 16:18:10.555669 craft_documents-0.1.1/craft_documents/new/Compiler.py
--rw-r--r--   0        0        0     1966 2023-07-18 16:33:13.383652 craft_documents-0.1.1/craft_documents/new/Subcommands.py
--rw-r--r--   0        0        0     1391 2023-07-18 16:13:47.385313 craft_documents-0.1.1/craft_documents/new/Validators.py
--rw-r--r--   0        0        0      975 2023-07-18 16:33:13.374889 craft_documents-0.1.1/craft_documents/new/main.py
--rw-r--r--   0        0        0     2683 2023-07-18 16:18:13.506519 craft_documents-0.1.1/craft_documents/templates/TemplateManager.py
--rw-r--r--   0        0        0     2875 2023-07-18 16:18:12.483042 craft_documents-0.1.1/craft_documents/templates/fetch.py
--rw-r--r--   0        0        0      708 2023-07-18 16:18:12.150008 craft_documents-0.1.1/craft_documents/templates/list.py
--rw-r--r--   0        0        0     1233 2023-07-18 16:33:13.375888 craft_documents-0.1.1/craft_documents/templates/main.py
--rw-r--r--   0        0        0     3506 2023-07-18 16:33:13.375432 craft_documents-0.1.1/craft_documents/templates/new/main.py
--rw-r--r--   0        0        0      628 2023-07-18 16:33:05.807866 craft_documents-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 craft_documents-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-18 08:48:00.447292 craft_documents-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 16:13:47.390728 craft_documents-0.1.2/craft_documents/__init__.py
+-rw-r--r--   0        0        0      810 2023-07-18 16:13:47.369726 craft_documents-0.1.2/craft_documents/common/DiskRepresentable.py
+-rw-r--r--   0        0        0     4629 2023-07-18 16:18:09.637059 craft_documents-0.1.2/craft_documents/common/Exercise.py
+-rw-r--r--   0        0        0     3571 2023-07-18 16:18:15.603824 craft_documents-0.1.2/craft_documents/common/File.py
+-rw-r--r--   0        0        0     1348 2023-07-18 16:18:15.603766 craft_documents-0.1.2/craft_documents/common/Folder.py
+-rw-r--r--   0        0        0     1291 2023-07-18 16:18:11.002009 craft_documents-0.1.2/craft_documents/common/Header.py
+-rw-r--r--   0        0        0      725 2023-07-18 16:18:15.597922 craft_documents-0.1.2/craft_documents/common/Preamble.py
+-rw-r--r--   0        0        0    12389 2023-07-18 16:13:47.371992 craft_documents-0.1.2/craft_documents/common/Prompt.py
+-rw-r--r--   0        0        0     1381 2023-07-18 16:18:15.133887 craft_documents-0.1.2/craft_documents/common/Prompter.py
+-rw-r--r--   0        0        0     7409 2023-07-18 16:18:10.850944 craft_documents-0.1.2/craft_documents/common/Template.py
+-rw-r--r--   0        0        0     1942 2023-07-18 16:18:15.097438 craft_documents-0.1.2/craft_documents/common/TexTemplate.py
+-rw-r--r--   0        0        0     2338 2023-07-18 16:13:47.373445 craft_documents-0.1.2/craft_documents/common/helpers.py
+-rw-r--r--   0        0        0      512 2023-07-18 16:18:14.300283 craft_documents-0.1.2/craft_documents/configuration/AllowEvalValidator.py
+-rw-r--r--   0        0        0     6925 2023-07-18 16:18:10.691785 craft_documents-0.1.2/craft_documents/configuration/Configuration.py
+-rw-r--r--   0        0        0      967 2023-07-18 16:18:14.213506 craft_documents-0.1.2/craft_documents/configuration/DocumentNameValidator.py
+-rw-r--r--   0        0        0     5962 2023-07-18 16:26:54.411808 craft_documents-0.1.2/craft_documents/configuration/DraftExercisesValidator.py
+-rw-r--r--   0        0        0     1161 2023-07-18 16:18:13.694218 craft_documents-0.1.2/craft_documents/configuration/HeaderValidator.py
+-rw-r--r--   0        0        0      526 2023-07-18 16:18:13.686001 craft_documents-0.1.2/craft_documents/configuration/MultipleExercisesValidator.py
+-rw-r--r--   0        0        0     1819 2023-07-18 16:18:13.638487 craft_documents-0.1.2/craft_documents/configuration/PreambleValidator.py
+-rw-r--r--   0        0        0      522 2023-07-18 16:18:13.628748 craft_documents-0.1.2/craft_documents/configuration/RemoveCommentsValidator.py
+-rw-r--r--   0        0        0      179 2023-07-18 16:13:47.378656 craft_documents-0.1.2/craft_documents/configuration/Semantic.py
+-rw-r--r--   0        0        0     1685 2023-07-18 16:18:13.628722 craft_documents-0.1.2/craft_documents/configuration/TokensValidator.py
+-rw-r--r--   0        0        0      689 2023-07-18 16:18:13.628685 craft_documents-0.1.2/craft_documents/configuration/UniqueExercisePlaceholdersValidator.py
+-rw-r--r--   0        0        0     2391 2023-07-18 16:18:13.628655 craft_documents-0.1.2/craft_documents/configuration/Validator.py
+-rw-r--r--   0        0        0      507 2023-07-18 16:18:13.561298 craft_documents-0.1.2/craft_documents/configuration/VerboseValidator.py
+-rw-r--r--   0        0        0      608 2023-07-18 16:18:13.506353 craft_documents-0.1.2/craft_documents/debug/Debugger.py
+-rw-r--r--   0        0        0      295 2023-07-18 16:44:14.258869 craft_documents-0.1.2/craft_documents/debug/main.py
+-rw-r--r--   0        0        0      479 2023-07-18 16:44:14.258195 craft_documents-0.1.2/craft_documents/main.py
+-rw-r--r--   0        0        0    10275 2023-07-18 16:18:10.555669 craft_documents-0.1.2/craft_documents/new/Compiler.py
+-rw-r--r--   0        0        0     1966 2023-07-18 16:44:14.264788 craft_documents-0.1.2/craft_documents/new/Subcommands.py
+-rw-r--r--   0        0        0     1391 2023-07-18 16:13:47.385313 craft_documents-0.1.2/craft_documents/new/Validators.py
+-rw-r--r--   0        0        0      975 2023-07-18 16:44:14.256569 craft_documents-0.1.2/craft_documents/new/main.py
+-rw-r--r--   0        0        0     2683 2023-07-18 16:18:13.506519 craft_documents-0.1.2/craft_documents/templates/TemplateManager.py
+-rw-r--r--   0        0        0     2875 2023-07-18 16:18:12.483042 craft_documents-0.1.2/craft_documents/templates/fetch.py
+-rw-r--r--   0        0        0      708 2023-07-18 16:18:12.150008 craft_documents-0.1.2/craft_documents/templates/list.py
+-rw-r--r--   0        0        0     1233 2023-07-18 16:44:14.257598 craft_documents-0.1.2/craft_documents/templates/main.py
+-rw-r--r--   0        0        0     3506 2023-07-18 16:44:14.257149 craft_documents-0.1.2/craft_documents/templates/new/main.py
+-rw-r--r--   0        0        0      628 2023-07-18 16:44:10.872148 craft_documents-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 craft_documents-0.1.2/PKG-INFO
```

### Comparing `craft_documents-0.1.1/craft_documents/common/DiskRepresentable.py` & `craft_documents-0.1.2/craft_documents/common/DiskRepresentable.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/common/Exercise.py` & `craft_documents-0.1.2/craft_documents/common/Exercise.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/common/File.py` & `craft_documents-0.1.2/craft_documents/common/File.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/common/Folder.py` & `craft_documents-0.1.2/craft_documents/common/Folder.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/common/Header.py` & `craft_documents-0.1.2/craft_documents/common/Header.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/common/Preamble.py` & `craft_documents-0.1.2/craft_documents/common/Preamble.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/common/Prompt.py` & `craft_documents-0.1.2/craft_documents/common/Prompt.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/common/Prompter.py` & `craft_documents-0.1.2/craft_documents/common/Prompter.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/common/Template.py` & `craft_documents-0.1.2/craft_documents/common/Template.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/common/TexTemplate.py` & `craft_documents-0.1.2/craft_documents/common/TexTemplate.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/common/helpers.py` & `craft_documents-0.1.2/craft_documents/common/helpers.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/AllowEvalValidator.py` & `craft_documents-0.1.2/craft_documents/configuration/AllowEvalValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/Configuration.py` & `craft_documents-0.1.2/craft_documents/configuration/Configuration.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/DocumentNameValidator.py` & `craft_documents-0.1.2/craft_documents/configuration/DocumentNameValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/DraftExercisesValidator.py` & `craft_documents-0.1.2/craft_documents/configuration/DraftExercisesValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/HeaderValidator.py` & `craft_documents-0.1.2/craft_documents/configuration/HeaderValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/MultipleExercisesValidator.py` & `craft_documents-0.1.2/craft_documents/configuration/MultipleExercisesValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/PreambleValidator.py` & `craft_documents-0.1.2/craft_documents/configuration/PreambleValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/RemoveCommentsValidator.py` & `craft_documents-0.1.2/craft_documents/configuration/RemoveCommentsValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/TokensValidator.py` & `craft_documents-0.1.2/craft_documents/configuration/TokensValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/UniqueExercisePlaceholdersValidator.py` & `craft_documents-0.1.2/craft_documents/configuration/UniqueExercisePlaceholdersValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/configuration/Validator.py` & `craft_documents-0.1.2/craft_documents/configuration/Validator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/debug/Debugger.py` & `craft_documents-0.1.2/craft_documents/debug/Debugger.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/new/Compiler.py` & `craft_documents-0.1.2/craft_documents/new/Compiler.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/new/Subcommands.py` & `craft_documents-0.1.2/craft_documents/new/Subcommands.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/new/Validators.py` & `craft_documents-0.1.2/craft_documents/new/Validators.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/new/main.py` & `craft_documents-0.1.2/craft_documents/new/main.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/templates/TemplateManager.py` & `craft_documents-0.1.2/craft_documents/templates/TemplateManager.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/templates/fetch.py` & `craft_documents-0.1.2/craft_documents/templates/fetch.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/templates/list.py` & `craft_documents-0.1.2/craft_documents/templates/list.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/templates/main.py` & `craft_documents-0.1.2/craft_documents/templates/main.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/craft_documents/templates/new/main.py` & `craft_documents-0.1.2/craft_documents/templates/new/main.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.1/pyproject.toml` & `craft_documents-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "craft_documents"
-version = "0.1.1"
+version = "0.1.2"
 description = "A template based command line utility to create exams or worksheets with LaTeX."
 authors = ["Tobias Hauser <apps.hausertobias@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 craft = "craft_documents.main:app"
```

### Comparing `craft_documents-0.1.1/PKG-INFO` & `craft_documents-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-documents
-Version: 0.1.1
+Version: 0.1.2
 Summary: A template based command line utility to create exams or worksheets with LaTeX.
 License: MIT
 Author: Tobias Hauser
 Author-email: apps.hausertobias@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

