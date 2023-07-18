# Comparing `tmp/craft_documents-0.1.2.tar.gz` & `tmp/craft_documents-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft_documents-0.1.2.tar", max compression
+gzip compressed data, was "craft_documents-0.1.3.tar", max compression
```

## Comparing `craft_documents-0.1.2.tar` & `craft_documents-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0        0 2023-07-18 08:48:00.447292 craft_documents-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-18 16:13:47.390728 craft_documents-0.1.2/craft_documents/__init__.py
--rw-r--r--   0        0        0      810 2023-07-18 16:13:47.369726 craft_documents-0.1.2/craft_documents/common/DiskRepresentable.py
--rw-r--r--   0        0        0     4629 2023-07-18 16:18:09.637059 craft_documents-0.1.2/craft_documents/common/Exercise.py
--rw-r--r--   0        0        0     3571 2023-07-18 16:18:15.603824 craft_documents-0.1.2/craft_documents/common/File.py
--rw-r--r--   0        0        0     1348 2023-07-18 16:18:15.603766 craft_documents-0.1.2/craft_documents/common/Folder.py
--rw-r--r--   0        0        0     1291 2023-07-18 16:18:11.002009 craft_documents-0.1.2/craft_documents/common/Header.py
--rw-r--r--   0        0        0      725 2023-07-18 16:18:15.597922 craft_documents-0.1.2/craft_documents/common/Preamble.py
--rw-r--r--   0        0        0    12389 2023-07-18 16:13:47.371992 craft_documents-0.1.2/craft_documents/common/Prompt.py
--rw-r--r--   0        0        0     1381 2023-07-18 16:18:15.133887 craft_documents-0.1.2/craft_documents/common/Prompter.py
--rw-r--r--   0        0        0     7409 2023-07-18 16:18:10.850944 craft_documents-0.1.2/craft_documents/common/Template.py
--rw-r--r--   0        0        0     1942 2023-07-18 16:18:15.097438 craft_documents-0.1.2/craft_documents/common/TexTemplate.py
--rw-r--r--   0        0        0     2338 2023-07-18 16:13:47.373445 craft_documents-0.1.2/craft_documents/common/helpers.py
--rw-r--r--   0        0        0      512 2023-07-18 16:18:14.300283 craft_documents-0.1.2/craft_documents/configuration/AllowEvalValidator.py
--rw-r--r--   0        0        0     6925 2023-07-18 16:18:10.691785 craft_documents-0.1.2/craft_documents/configuration/Configuration.py
--rw-r--r--   0        0        0      967 2023-07-18 16:18:14.213506 craft_documents-0.1.2/craft_documents/configuration/DocumentNameValidator.py
--rw-r--r--   0        0        0     5962 2023-07-18 16:26:54.411808 craft_documents-0.1.2/craft_documents/configuration/DraftExercisesValidator.py
--rw-r--r--   0        0        0     1161 2023-07-18 16:18:13.694218 craft_documents-0.1.2/craft_documents/configuration/HeaderValidator.py
--rw-r--r--   0        0        0      526 2023-07-18 16:18:13.686001 craft_documents-0.1.2/craft_documents/configuration/MultipleExercisesValidator.py
--rw-r--r--   0        0        0     1819 2023-07-18 16:18:13.638487 craft_documents-0.1.2/craft_documents/configuration/PreambleValidator.py
--rw-r--r--   0        0        0      522 2023-07-18 16:18:13.628748 craft_documents-0.1.2/craft_documents/configuration/RemoveCommentsValidator.py
--rw-r--r--   0        0        0      179 2023-07-18 16:13:47.378656 craft_documents-0.1.2/craft_documents/configuration/Semantic.py
--rw-r--r--   0        0        0     1685 2023-07-18 16:18:13.628722 craft_documents-0.1.2/craft_documents/configuration/TokensValidator.py
--rw-r--r--   0        0        0      689 2023-07-18 16:18:13.628685 craft_documents-0.1.2/craft_documents/configuration/UniqueExercisePlaceholdersValidator.py
--rw-r--r--   0        0        0     2391 2023-07-18 16:18:13.628655 craft_documents-0.1.2/craft_documents/configuration/Validator.py
--rw-r--r--   0        0        0      507 2023-07-18 16:18:13.561298 craft_documents-0.1.2/craft_documents/configuration/VerboseValidator.py
--rw-r--r--   0        0        0      608 2023-07-18 16:18:13.506353 craft_documents-0.1.2/craft_documents/debug/Debugger.py
--rw-r--r--   0        0        0      295 2023-07-18 16:44:14.258869 craft_documents-0.1.2/craft_documents/debug/main.py
--rw-r--r--   0        0        0      479 2023-07-18 16:44:14.258195 craft_documents-0.1.2/craft_documents/main.py
--rw-r--r--   0        0        0    10275 2023-07-18 16:18:10.555669 craft_documents-0.1.2/craft_documents/new/Compiler.py
--rw-r--r--   0        0        0     1966 2023-07-18 16:44:14.264788 craft_documents-0.1.2/craft_documents/new/Subcommands.py
--rw-r--r--   0        0        0     1391 2023-07-18 16:13:47.385313 craft_documents-0.1.2/craft_documents/new/Validators.py
--rw-r--r--   0        0        0      975 2023-07-18 16:44:14.256569 craft_documents-0.1.2/craft_documents/new/main.py
--rw-r--r--   0        0        0     2683 2023-07-18 16:18:13.506519 craft_documents-0.1.2/craft_documents/templates/TemplateManager.py
--rw-r--r--   0        0        0     2875 2023-07-18 16:18:12.483042 craft_documents-0.1.2/craft_documents/templates/fetch.py
--rw-r--r--   0        0        0      708 2023-07-18 16:18:12.150008 craft_documents-0.1.2/craft_documents/templates/list.py
--rw-r--r--   0        0        0     1233 2023-07-18 16:44:14.257598 craft_documents-0.1.2/craft_documents/templates/main.py
--rw-r--r--   0        0        0     3506 2023-07-18 16:44:14.257149 craft_documents-0.1.2/craft_documents/templates/new/main.py
--rw-r--r--   0        0        0      628 2023-07-18 16:44:10.872148 craft_documents-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 craft_documents-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-18 17:57:13.684174 craft_documents-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 17:57:13.685125 craft_documents-0.1.3/craft_documents/__init__.py
+-rw-r--r--   0        0        0      810 2023-07-18 17:57:13.685347 craft_documents-0.1.3/craft_documents/common/DiskRepresentable.py
+-rw-r--r--   0        0        0     4629 2023-07-18 19:51:06.929419 craft_documents-0.1.3/craft_documents/common/Exercise.py
+-rw-r--r--   0        0        0     3571 2023-07-18 17:57:13.685549 craft_documents-0.1.3/craft_documents/common/File.py
+-rw-r--r--   0        0        0     1348 2023-07-18 17:57:13.685651 craft_documents-0.1.3/craft_documents/common/Folder.py
+-rw-r--r--   0        0        0     1291 2023-07-18 19:51:06.929694 craft_documents-0.1.3/craft_documents/common/Header.py
+-rw-r--r--   0        0        0      725 2023-07-18 17:57:13.685816 craft_documents-0.1.3/craft_documents/common/Preamble.py
+-rw-r--r--   0        0        0    12389 2023-07-18 17:57:13.685918 craft_documents-0.1.3/craft_documents/common/Prompt.py
+-rw-r--r--   0        0        0     1381 2023-07-18 17:57:13.685993 craft_documents-0.1.3/craft_documents/common/Prompter.py
+-rw-r--r--   0        0        0     7409 2023-07-18 19:51:06.929987 craft_documents-0.1.3/craft_documents/common/Template.py
+-rw-r--r--   0        0        0     1942 2023-07-18 17:57:13.686189 craft_documents-0.1.3/craft_documents/common/TexTemplate.py
+-rw-r--r--   0        0        0     2338 2023-07-18 17:57:13.686265 craft_documents-0.1.3/craft_documents/common/helpers.py
+-rw-r--r--   0        0        0      512 2023-07-18 17:57:13.686392 craft_documents-0.1.3/craft_documents/configuration/AllowEvalValidator.py
+-rw-r--r--   0        0        0     6925 2023-07-18 19:51:06.930263 craft_documents-0.1.3/craft_documents/configuration/Configuration.py
+-rw-r--r--   0        0        0     5890 2023-07-18 19:51:06.930441 craft_documents-0.1.3/craft_documents/configuration/CraftExercisesValidator.py
+-rw-r--r--   0        0        0      967 2023-07-18 17:57:13.686615 craft_documents-0.1.3/craft_documents/configuration/DocumentNameValidator.py
+-rw-r--r--   0        0        0     1161 2023-07-18 19:51:06.930697 craft_documents-0.1.3/craft_documents/configuration/HeaderValidator.py
+-rw-r--r--   0        0        0      526 2023-07-18 17:57:13.686861 craft_documents-0.1.3/craft_documents/configuration/MultipleExercisesValidator.py
+-rw-r--r--   0        0        0     1819 2023-07-18 19:51:06.930945 craft_documents-0.1.3/craft_documents/configuration/PreambleValidator.py
+-rw-r--r--   0        0        0      522 2023-07-18 17:57:13.687025 craft_documents-0.1.3/craft_documents/configuration/RemoveCommentsValidator.py
+-rw-r--r--   0        0        0      179 2023-07-18 17:57:13.687143 craft_documents-0.1.3/craft_documents/configuration/Semantic.py
+-rw-r--r--   0        0        0     1685 2023-07-18 17:57:13.687217 craft_documents-0.1.3/craft_documents/configuration/TokensValidator.py
+-rw-r--r--   0        0        0      689 2023-07-18 17:57:13.687305 craft_documents-0.1.3/craft_documents/configuration/UniqueExercisePlaceholdersValidator.py
+-rw-r--r--   0        0        0     2391 2023-07-18 17:57:13.687407 craft_documents-0.1.3/craft_documents/configuration/Validator.py
+-rw-r--r--   0        0        0      507 2023-07-18 17:57:13.687497 craft_documents-0.1.3/craft_documents/configuration/VerboseValidator.py
+-rw-r--r--   0        0        0      608 2023-07-18 17:57:13.687617 craft_documents-0.1.3/craft_documents/debug/Debugger.py
+-rw-r--r--   0        0        0      295 2023-07-18 19:55:09.286270 craft_documents-0.1.3/craft_documents/debug/main.py
+-rw-r--r--   0        0        0      479 2023-07-18 19:55:09.286051 craft_documents-0.1.3/craft_documents/main.py
+-rw-r--r--   0        0        0    10275 2023-07-18 19:51:06.931203 craft_documents-0.1.3/craft_documents/new/Compiler.py
+-rw-r--r--   0        0        0     1966 2023-07-18 19:55:09.288355 craft_documents-0.1.3/craft_documents/new/Subcommands.py
+-rw-r--r--   0        0        0     1391 2023-07-18 17:57:13.688072 craft_documents-0.1.3/craft_documents/new/Validators.py
+-rw-r--r--   0        0        0      975 2023-07-18 19:55:09.285156 craft_documents-0.1.3/craft_documents/new/main.py
+-rw-r--r--   0        0        0     2683 2023-07-18 19:51:06.931657 craft_documents-0.1.3/craft_documents/templates/TemplateManager.py
+-rw-r--r--   0        0        0     2875 2023-07-18 19:51:06.931855 craft_documents-0.1.3/craft_documents/templates/fetch.py
+-rw-r--r--   0        0        0      708 2023-07-18 17:57:13.688406 craft_documents-0.1.3/craft_documents/templates/list.py
+-rw-r--r--   0        0        0     1233 2023-07-18 19:55:09.285826 craft_documents-0.1.3/craft_documents/templates/main.py
+-rw-r--r--   0        0        0     3506 2023-07-18 19:55:09.285538 craft_documents-0.1.3/craft_documents/templates/new/main.py
+-rw-r--r--   0        0        0      628 2023-07-18 19:51:20.178392 craft_documents-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 craft_documents-0.1.3/PKG-INFO
```

### Comparing `craft_documents-0.1.2/craft_documents/common/DiskRepresentable.py` & `craft_documents-0.1.3/craft_documents/common/DiskRepresentable.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/common/Exercise.py` & `craft_documents-0.1.3/craft_documents/common/Exercise.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from rich import print
 
 from craft_documents.common.helpers import create_list
 from craft_documents.common.Prompter import Prompter
 from craft_documents.common.Template import Template
 from craft_documents.common.TexTemplate import TexTemplate
 from craft_documents.configuration.Configuration import Configuration
-from craft_documents.configuration.DraftExercisesValidator import (
-    DraftExercisesValidator,
+from craft_documents.configuration.CraftExercisesValidator import (
+    CraftExercisesValidator,
 )
 
 
 class Exercise(TexTemplate):
     """
     A class representing an exercise template.
 
-    Exercise templates are stored in `.config/draft/exercises/`.
+    Exercise templates are stored in `.config/craft/exercises/`.
     They are always latex documents.
     """
 
     @property
     def contents(self) -> str:
         """
         Returns the entire contents.
```

### Comparing `craft_documents-0.1.2/craft_documents/common/File.py` & `craft_documents-0.1.3/craft_documents/common/File.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/common/Folder.py` & `craft_documents-0.1.3/craft_documents/common/Folder.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/common/Header.py` & `craft_documents-0.1.3/craft_documents/common/Header.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import re
 from pathlib import Path
 
 from craft_documents.common.TexTemplate import TexTemplate
 from craft_documents.configuration.Configuration import Configuration
-from craft_documents.configuration.DraftExercisesValidator import (
-    DraftExercisesValidator,
+from craft_documents.configuration.CraftExercisesValidator import (
+    CraftExercisesValidator,
 )
 
 
 class Header(TexTemplate):
     """
     A class representing a header template.
 
-    Header templates are stored in `.config/draft/headers/`.
+    Header templates are stored in `.config/craft/headers/`.
     They are always latex documents.
     """
 
     def __init__(self, path: Path, configuration: Configuration):
         super().__init__(path, configuration)
 
         self.remove_documentclass()
@@ -26,20 +26,20 @@
         """
         Remove the input statement of the preamble from the contents.
         """
         with self.path.open("r") as file:
             self._contents = file.read()
             self._disk_contents = self.contents
 
-    def set_draft_exercises(self, value: str):
+    def set_craft_exercises(self, value: str):
         pattern = re.compile(
             r"%s%s%s"
             % (
                 self.placeholder_prefix,
-                DraftExercisesValidator().key,
+                CraftExercisesValidator().key,
                 self.placeholder_suffix,
             )
         )
 
         # escape `\`
         value = re.sub("\\\\", "\\\\\\\\", value)
         self._contents = re.sub(pattern, value, self.contents)
```

### Comparing `craft_documents-0.1.2/craft_documents/common/Preamble.py` & `craft_documents-0.1.3/craft_documents/common/Preamble.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/common/Prompt.py` & `craft_documents-0.1.3/craft_documents/common/Prompt.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/common/Prompter.py` & `craft_documents-0.1.3/craft_documents/common/Prompter.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/common/Template.py` & `craft_documents-0.1.3/craft_documents/common/Template.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import yaml
 
 from craft_documents.common.File import File
 from craft_documents.common.helpers import combine_dictionaries
 from craft_documents.common.Prompt import Prompt
 from craft_documents.common.Prompter import Prompter
 from craft_documents.configuration.Configuration import Configuration
-from craft_documents.configuration.DraftExercisesValidator import (
-    DraftExercisesValidator,
+from craft_documents.configuration.CraftExercisesValidator import (
+    CraftExercisesValidator,
 )
 from craft_documents.configuration.RemoveCommentsValidator import (
     RemoveCommentsValidator,
 )
 from craft_documents.configuration.TokensValidator import TokensValidator
 
 
@@ -156,16 +156,16 @@
 
         They can be customized in any YAML-block.
         """
         prompts: List[Prompt] = []
 
         # TODO: Rewrite to use 'typed' prompts
         for placeholder in self.placeholders:
-            # ignore `<<draft-exercises>>`
-            if placeholder == "draft-exercises" or placeholder.startswith(
+            # ignore `<<craft-exercises>>`
+            if placeholder == "craft-exercises" or placeholder.startswith(
                 "supplements/"
             ):
                 continue
 
             question: Prompt = Prompt(
                 name=placeholder,
                 type=Prompt.Type.input,
```

### Comparing `craft_documents-0.1.2/craft_documents/common/TexTemplate.py` & `craft_documents-0.1.3/craft_documents/common/TexTemplate.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/common/helpers.py` & `craft_documents-0.1.3/craft_documents/common/helpers.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/configuration/AllowEvalValidator.py` & `craft_documents-0.1.3/craft_documents/configuration/AllowEvalValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/configuration/Configuration.py` & `craft_documents-0.1.3/craft_documents/configuration/Configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import Any, List
 
 import yaml
 from rich import print
 
 from craft_documents.configuration.AllowEvalValidator import AllowEvalValidator
 from craft_documents.configuration.DocumentNameValidator import DocumentNameValidator
-from craft_documents.configuration.DraftExercisesValidator import (
-    DraftExercisesValidator,
+from craft_documents.configuration.CraftExercisesValidator import (
+    CraftExercisesValidator,
 )
 from craft_documents.configuration.HeaderValidator import HeaderValidator
 from craft_documents.configuration.MultipleExercisesValidator import (
     MultipleExercisesValidator,
 )
 from craft_documents.configuration.PreambleValidator import PreambleValidator
 from craft_documents.configuration.RemoveCommentsValidator import (
@@ -33,15 +33,15 @@
     of the user.
 
     ### Settings
 
     - `preamble`: required, defaults to `default.tex`
     - `allow_eval`: required, defaults to `False`
     - `remove_comments`: required, defaults to `False`
-    - `draft-exercises`: optional
+    - `craft-exercises`: optional
     - `multiple-exercises`: required, defaults to `True`
     - `tokens`: required, loads defaults for `.tex` and `.ly`
     """
 
     @property
     def validators(self) -> list[Validator]:
         return self._validators
@@ -93,16 +93,16 @@
         return self[VerboseValidator().key]
 
     @property
     def remove_comments(self) -> bool:
         return self[RemoveCommentsValidator().key]
 
     @property
-    def draft_exercises(self) -> dict[str, dict[str, Any]] | None:
-        return self.get(DraftExercisesValidator().key, None)
+    def craft_exercises(self) -> dict[str, dict[str, Any]] | None:
+        return self.get(CraftExercisesValidator().key, None)
 
     @property
     def multiple_exercises(self) -> bool:
         return self[AllowEvalValidator().key]
 
     @property
     def unique_exercise_placeholders(self) -> bool:
@@ -110,15 +110,15 @@
 
     @property
     def document_name(self) -> str:
         return self.get(DocumentNameValidator().key, None)
 
     def __init__(
         self,
-        main: Path = Path.home() / ".config/draft/draftrc",
+        main: Path = Path.home() / ".config/craft/craftrc",
         root: Path = Path.home(),
         cwd: Path = Path.cwd(),
         *args,
         **kwargs,
     ):
         self._main = main
         self._root = root
@@ -128,31 +128,31 @@
         self.load()
         self.validate()
 
     def load(self):
         """
         Load the configuration from the disk.
 
-        The user can configure draft in yaml-formatted
-        configuration files: `draftrc`, `.draftrc`.
+        The user can configure craft in yaml-formatted
+        configuration files: `craftrc`, `.craftrc`.
 
         Draft will read all configuration files from
         the current working directory to home and
         accumulate their values. Files closer to
         the current working directory take
         precedence.
 
         Additionally there is one configuration file
-        at `~/.config/draft/draftrc` which stores
+        at `~/.config/craft/craftrc` which stores
         gets read last. It stores global configuration
         such as prefixes for single-line-comments for
         a specific file extension. Make sure to escape
         them correctly.
         """
-        files: List[str] = ["draftrc", ".draftrc"]
+        files: List[str] = ["craftrc", ".craftrc"]
         directory: Path = self.cwd
 
         while True:
             for file in files:
                 file_path: Path = directory / file
                 if not file_path.is_file():
                     continue
@@ -167,15 +167,15 @@
             # Exit if the root directory has been reached
             if directory == self.root:
                 break
 
             # Move up to the parent directory
             directory = directory.parent
 
-        # read file at `~/.config/draft/draftrc`
+        # read file at `~/.config/craft/craftrc`
         try:
             data = yaml.safe_load(self.main.open())
             for key, value in data.items():
                 if key not in self:
                     self[key] = value
         except:
             pass
@@ -203,15 +203,15 @@
             )
 
         self._validators = [
             PreambleValidator(),
             AllowEvalValidator(),
             RemoveCommentsValidator(),
             AllowEvalValidator(),
-            DraftExercisesValidator(),
+            CraftExercisesValidator(),
             MultipleExercisesValidator(),
             TokensValidator(),
             HeaderValidator(),
             UniqueExercisePlaceholdersValidator(),
             DocumentNameValidator(),
             VerboseValidator(),
         ]
```

### Comparing `craft_documents-0.1.2/craft_documents/configuration/DocumentNameValidator.py` & `craft_documents-0.1.3/craft_documents/configuration/DocumentNameValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/configuration/DraftExercisesValidator.py` & `craft_documents-0.1.3/craft_documents/configuration/CraftExercisesValidator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pathlib import Path
 
-# from craft_documents.configuration.Configuration import Configuration
 from craft_documents.configuration.Semantic import Semantic
 from craft_documents.configuration.Validator import Validator
 
 
 class ExerciseConfiguration(dict):
     """
     Wrapper around a dictionary that defines a minimal interface of
@@ -54,30 +53,30 @@
                     else:
                         self["path"] = configuration.main.parent / "exercises" / path
 
         # Absolute path
         self["path"] = self["path"].resolve()
 
 
-class DraftExercisesValidator(Validator):
+class CraftExercisesValidator(Validator):
     """
     Optional, that defaults to a dictionary:
 
     ```
     {
         "intervals": {
             "count": 1,
             "path": Path(...),
         }
     }
     ```
     """
 
     def __init__(self):
-        self._key = "draft-exercises"
+        self._key = "craft-exercises"
         self._semantic = Semantic.OPTIONAL
 
     def remove_tex(self, value: str) -> str:
         return value.removesuffix(".tex")
 
     def exercise_path_appending(self, component: str | Path) -> Path:
         match component:
@@ -97,21 +96,21 @@
         def dict_types(dictionary: dict, key, value) -> bool:
             return all(
                 isinstance(k, key) and isinstance(v, value)
                 for k, v in dictionary.items()
             )
 
         match value:
-            # draft-exercises: intervals
+            # craft-exercises: intervals
             case str(exercise_name):
                 result[exercise_name] = ExerciseConfiguration(
                     self.configuration, exercise_name
                 )
 
-            # draft-exercises:
+            # craft-exercises:
             case list(items):
                 for item in items:
                     match item:
                         # - intervals
                         case str(exercise_name):
                             result[exercise_name] = ExerciseConfiguration(
                                 self.configuration, exercise_name
@@ -126,15 +125,15 @@
                         # - intervals:
                         case dict(item) if dict_types(item, str, dict):
                             for exercise_name, kwargs in item.items():
                                 result[exercise_name] = ExerciseConfiguration(
                                     self.configuration, exercise_name, **kwargs
                                 )
 
-            # draft-exercises:
+            # craft-exercises:
             case dict(items):
                 for exercise_name, v in items.items():
                     match v:
                         # 2
                         case int(count):
                             result[exercise_name] = ExerciseConfiguration(
                                 self.configuration, exercise_name, count=count
```

### Comparing `craft_documents-0.1.2/craft_documents/configuration/HeaderValidator.py` & `craft_documents-0.1.3/craft_documents/configuration/HeaderValidator.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from craft_documents.configuration.Validator import Validator
 
 
 class HeaderValidator(Validator):
     """
     Accepts an absolute or relative path to a tex-file.
     Relative paths will be interpreted as being inside
-    `~/.config/draft/headers/`.
+    `~/.config/craft/headers/`.
 
     Optional
     """
 
     def __init__(self):
         self._key = "header"
         self._semantic = Semantic.OPTIONAL
```

### Comparing `craft_documents-0.1.2/craft_documents/configuration/MultipleExercisesValidator.py` & `craft_documents-0.1.3/craft_documents/configuration/MultipleExercisesValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/configuration/PreambleValidator.py` & `craft_documents-0.1.3/craft_documents/configuration/PreambleValidator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from craft_documents.configuration.Validator import Validator
 
 
 class PreambleValidator(Validator):
     """
     Accepts an absolute or relative path to a tex-file.
     Relative paths will be interpreted as being inside
-    `~/.config/draft/preambles/`.
+    `~/.config/craft/preambles/`.
 
     Defaults to an absolute path to a tex-file.
     """
 
     def __init__(self):
         self._key = "preamble"
         self._semantic = Semantic.REQUIRED
@@ -52,10 +52,10 @@
                 "[blue]==>[/blue] Created the default preamble at '%s' :sparkles:\n"
                 % path
             )
             path.parent.mkdir(parents=True, exist_ok=True)
             path.touch(exist_ok=True)
             path.write_text(r"\documentclass{scrreport}")
             print(
-                "Run 'draft templates fetch --verbose' to fetch more templates from GitHub.\n"
+                "Run 'craft templates fetch --verbose' to fetch more templates from GitHub.\n"
             )
             return path
```

### Comparing `craft_documents-0.1.2/craft_documents/configuration/RemoveCommentsValidator.py` & `craft_documents-0.1.3/craft_documents/configuration/RemoveCommentsValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/configuration/TokensValidator.py` & `craft_documents-0.1.3/craft_documents/configuration/TokensValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/configuration/UniqueExercisePlaceholdersValidator.py` & `craft_documents-0.1.3/craft_documents/configuration/UniqueExercisePlaceholdersValidator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/configuration/Validator.py` & `craft_documents-0.1.3/craft_documents/configuration/Validator.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/debug/Debugger.py` & `craft_documents-0.1.3/craft_documents/debug/Debugger.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/new/Compiler.py` & `craft_documents-0.1.3/craft_documents/new/Compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 from craft_documents.common.Exercise import Exercise
 from craft_documents.common.Folder import Folder
 from craft_documents.common.Header import Header
 from craft_documents.common.Preamble import Preamble
 from craft_documents.common.Prompt import Checkbox, Input
 from craft_documents.configuration.Configuration import Configuration
-from craft_documents.configuration.DraftExercisesValidator import (
-    DraftExercisesValidator,
+from craft_documents.configuration.CraftExercisesValidator import (
+    CraftExercisesValidator,
     ExerciseConfiguration,
 )
 from craft_documents.configuration.MultipleExercisesValidator import (
     MultipleExercisesValidator,
 )
 from craft_documents.new.Validators import (
     DocumentNamePromptValidator,
@@ -97,21 +97,21 @@
         if configuration.header is not None:
             self._header = Header(configuration.header, configuration)
         else:
             raise Exception("Unexpectedly found `None` at `configuration.header`.")
             # TODO: Handle Exception
 
         # Prompt for exercises if they are not defined in a configuration file
-        if DraftExercisesValidator().key not in self.configuration:
+        if CraftExercisesValidator().key not in self.configuration:
             self.configuration[
-                DraftExercisesValidator().key
+                CraftExercisesValidator().key
             ] = self.prompt_for_exercises()
 
         self._exercises: list[Exercise] = []
-        for config in self.configuration[DraftExercisesValidator().key].values():
+        for config in self.configuration[CraftExercisesValidator().key].values():
             self._exercises += [
                 Exercise(config["path"], self.configuration)
                 for _ in range(config["count"])
             ]
         self.disambiguate_exercises()
 
         if DocumentNameValidator().key not in self.configuration:
@@ -214,15 +214,15 @@
                     + "-" * (79 - 5 - len(exercise.disambiguated_name))
                     + " %\n"
                 )
                 body_exercises += exercise.body
                 if not exercise.body.endswith("\n\n"):
                     body_exercises += "\n"
 
-        self.header.set_draft_exercises(body_exercises)
+        self.header.set_craft_exercises(body_exercises)
         self.document += "\\begin{document}\n"
         self.document += self.header.body
         self.document += "\\end{document}\n"
 
         self.work_jobs()
 
     def work_jobs(self):
@@ -249,17 +249,17 @@
         answer = prompt(question)
         return answer[key]
 
     def prompt_for_exercises(self) -> dict:
         """
         Prompt the user which exercises should be included.
         """
-        key = DraftExercisesValidator().key
+        key = CraftExercisesValidator().key
         question = Checkbox(
-            DraftExercisesValidator().key,
+            CraftExercisesValidator().key,
             [
                 Checkbox.Choice(name=exercise.name)
                 for exercise in self.template_manager.exercises
             ],
             "Which exercises should be included?",
             when=lambda _: key not in self.configuration,
         )
@@ -285,11 +285,11 @@
                 config["count"] = int(count)
 
         return answer
 
     def disambiguate_exercises(self):
         count = {}
         for exercise in self.exercises:
-            if self.configuration["draft-exercises"][exercise.name]["count"] > 1:
+            if self.configuration["craft-exercises"][exercise.name]["count"] > 1:
                 add = count.get(exercise.name, 1)
                 exercise.disambiguation_suffix = add
                 count[exercise.name] = count.get(exercise.name, 1) + 1
```

### Comparing `craft_documents-0.1.2/craft_documents/new/Subcommands.py` & `craft_documents-0.1.3/craft_documents/new/Subcommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from craft_documents.new.Compiler import Compiler
 
 
 class Subcommands:
     """
     Initialize the subcommands; one for each header declared in the
     templates:
-    - draft new exam
-    - draft new worksheet
+    - craft new exam
+    - craft new worksheet
 
     Hand off the neccessary files to the compiler.
     """
 
     @property
     def template_manager(self) -> TemplateManager:
         return self._template_manager
```

### Comparing `craft_documents-0.1.2/craft_documents/new/Validators.py` & `craft_documents-0.1.3/craft_documents/new/Validators.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/new/main.py` & `craft_documents-0.1.3/craft_documents/new/main.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/templates/TemplateManager.py` & `craft_documents-0.1.3/craft_documents/templates/TemplateManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class TemplateManager:
     """
     A class that manages the templates installed on the system.
     """
 
     @property
     def folder(self) -> Folder:
-        """The folder of the templates: `~/.config/draft/`."""
+        """The folder of the templates: `~/.config/craft/`."""
         return self._folder
 
     @property
     def headers(self) -> list[Header]:
         """List of all Headers."""
         return self._headers
```

### Comparing `craft_documents-0.1.2/craft_documents/templates/fetch.py` & `craft_documents-0.1.3/craft_documents/templates/fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     verbose: bool, templates_manager: TemplateManager, app: typer.Typer
 ):
     print("Fetching templates from GitHub...")
 
     templates_are_uptodate = True
 
     owner = "tobiashauser"
-    repo = "42.43-draft"
-    path = "config.draft/"
+    repo = "42.43-craft"
+    path = "config.craft/"
 
     preambles = fetch_github_directory(owner, repo, path + "preambles/")
     headers = fetch_github_directory(owner, repo, path + "headers/")
     exercises = fetch_github_directory(owner, repo, path + "exercises")
 
     def resolve_templates(dict, type, creator, path: Path):
         for name, contents in dict.items():
```

### Comparing `craft_documents-0.1.2/craft_documents/templates/list.py` & `craft_documents-0.1.3/craft_documents/templates/list.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/templates/main.py` & `craft_documents-0.1.3/craft_documents/templates/main.py`

 * *Files identical despite different names*

### Comparing `craft_documents-0.1.2/craft_documents/templates/new/main.py` & `craft_documents-0.1.3/craft_documents/templates/new/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import typer
 from rich import print
 from typing_extensions import Annotated
 
-from craft_documents.configuration.Configuration import Configuration
 from craft_documents.templates.TemplateManager import TemplateManager
+from craft_documents.configuration.Configuration import Configuration
 
 app = typer.Typer(no_args_is_help=True)
 
 configuration = Configuration()
 template_manager = TemplateManager(configuration)
 
 import os
@@ -73,15 +73,15 @@
 
 % Add your declarations
 
 % Add content to the document-body
 \begin{document}
 
 % This placeholder will be replaced with exercises
-<<draft-exercises>> 
+<<craft-exercises>> 
 
 \end{document}
 """
     path.write_text(contents)
 
     editor = os.environ.get("EDITOR", DEFAULT_EDITOR)
     subprocess.call([editor, path])
```

### Comparing `craft_documents-0.1.2/pyproject.toml` & `craft_documents-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "craft_documents"
-version = "0.1.2"
+version = "0.1.3"
 description = "A template based command line utility to create exams or worksheets with LaTeX."
 authors = ["Tobias Hauser <apps.hausertobias@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 craft = "craft_documents.main:app"
```

### Comparing `craft_documents-0.1.2/PKG-INFO` & `craft_documents-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-documents
-Version: 0.1.2
+Version: 0.1.3
 Summary: A template based command line utility to create exams or worksheets with LaTeX.
 License: MIT
 Author: Tobias Hauser
 Author-email: apps.hausertobias@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

