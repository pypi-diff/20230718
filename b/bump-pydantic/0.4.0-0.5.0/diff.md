# Comparing `tmp/bump_pydantic-0.4.0.tar.gz` & `tmp/bump_pydantic-0.5.0.tar.gz`

## Comparing `bump_pydantic-0.4.0.tar` & `bump_pydantic-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/__main__.py
--rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/py.typed
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/__init__.py
--rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/add_default_none.py
--rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/con_func.py
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/field.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/mypy_visitor.py
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/replace_config.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/replace_generic_model.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/replace_imports.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/root_model.py
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/bump_pydantic/codemods/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/case.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/file.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/folder.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/test_cli.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/add_none.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/base_settings.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/con_func.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/config_to_model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/field.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/folder_inside_folder.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/is_base_model.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/replace_validator.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/root_model.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/integration/cases/unicode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_add_default_none.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_class_def_visitor.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_con_func.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_field.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_generic_model.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_replace_config.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_replace_imports.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_root_model.py
--rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/tests/unit/test_validator.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/README.md
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 bump_pydantic-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/__main__.py
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/py.typed
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/codemods/__init__.py
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/codemods/add_default_none.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/codemods/class_def_visitor.py
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/codemods/con_func.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/codemods/field.py
+-rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/codemods/replace_config.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/codemods/replace_generic_model.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/codemods/replace_imports.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/codemods/root_model.py
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/bump_pydantic/codemods/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/case.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/file.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/folder.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/add_none.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/base_settings.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/con_func.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/config_to_model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/field.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/folder_inside_folder.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/is_base_model.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/replace_validator.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/root_model.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/integration/cases/unicode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/unit/test_add_default_none.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/unit/test_class_def_visitor.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/unit/test_con_func.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/unit/test_field.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/unit/test_generic_model.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/unit/test_replace_config.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/unit/test_replace_imports.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/unit/test_root_model.py
+-rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/tests/unit/test_validator.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/README.md
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8876 2020-02-02 00:00:00.000000 bump_pydantic-0.5.0/PKG-INFO
```

### Comparing `bump_pydantic-0.4.0/.github/workflows/main.yml` & `bump_pydantic-0.5.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/bump_pydantic/main.py` & `bump_pydantic-0.5.0/bump_pydantic/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 import difflib
 import functools
 import multiprocessing
 import os
 import time
 import traceback
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, Iterable, List, Set, Tuple, Type, TypeVar, Union
 
 import libcst as cst
 from libcst.codemod import CodemodContext, ContextAwareTransformer
 from libcst.helpers import calculate_module_and_package
 from libcst.metadata import FullRepoManager, FullyQualifiedNameProvider, ScopeProvider
 from rich.console import Console
 from rich.progress import Progress
 from typer import Argument, Exit, Option, Typer, echo
 from typing_extensions import ParamSpec
 
 from bump_pydantic import __version__
 from bump_pydantic.codemods import Rule, gather_codemods
-from bump_pydantic.codemods.mypy_visitor import CONTEXT_KEY, run_mypy_visitor
+from bump_pydantic.codemods.class_def_visitor import ClassDefVisitor
 
-app = Typer(
-    help="Convert Pydantic from V1 to V2 ♻️",
-    invoke_without_command=True,
-    add_completion=False,
-)
+app = Typer(invoke_without_command=True, add_completion=False)
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def version_callback(value: bool):
     if value:
@@ -46,14 +42,18 @@
         None,
         "--version",
         callback=version_callback,
         is_eager=True,
         help="Show the version and exit.",
     ),
 ):
+    """Convert Pydantic from V1 to V2 ♻️
+
+    Check the README for more information: https://github.com/pydantic/bump-pydantic.
+    """
     console = Console(log_time=True)
     console.log("Start bump-pydantic.")
     # NOTE: LIBCST_PARSER_TYPE=native is required according to https://github.com/Instagram/LibCST/issues/487.
     os.environ["LIBCST_PARSER_TYPE"] = "native"
 
     if os.path.isfile(path):
         package = path.parent
@@ -65,24 +65,55 @@
 
     console.log(f"Found {len(files)} files to process")
 
     providers = {FullyQualifiedNameProvider, ScopeProvider}
     metadata_manager = FullRepoManager(".", files, providers=providers)  # type: ignore[arg-type]
     metadata_manager.resolve_cache()
 
-    console.log("Running mypy to get type information. This may take a while...")
-    classes = run_mypy_visitor(files)
-    scratch: dict[str, Any] = {CONTEXT_KEY: classes}
-    console.log("Finished mypy.")
+    scratch: dict[str, Any] = {}
+    with Progress(*Progress.get_default_columns(), transient=True) as progress:
+        task = progress.add_task(description="Looking for Pydantic Models...", total=len(files))
+        queue: List[str] = [files[0]]
+        visited: Set[str] = set()
+
+        while queue:
+            # Queue logic
+            filename = queue.pop()
+            visited.add(filename)
+            progress.advance(task)
+
+            # Visitor logic
+            code = Path(filename).read_text(encoding="utf8")
+            module = cst.parse_module(code)
+            module_and_package = calculate_module_and_package(str(package), filename)
+
+            context = CodemodContext(
+                metadata_manager=metadata_manager,
+                filename=filename,
+                full_module_name=module_and_package.name,
+                full_package_name=module_and_package.package,
+                scratch=scratch,
+            )
+            visitor = ClassDefVisitor(context=context)
+            visitor.transform_module(module)
+
+            # Queue logic
+            next_file = visitor.next_file(visited)
+            if next_file is not None:
+                queue.append(next_file)
+
+            missing_files = set(files) - visited
+            if not queue and missing_files:
+                queue.append(next(iter(missing_files)))
 
     start_time = time.time()
 
     codemods = gather_codemods(disabled=disable)
 
-    log_fp = log_file.open("a+")
+    log_fp = log_file.open("a+", encoding="utf8")
     partial_run_codemods = functools.partial(run_codemods, codemods, metadata_manager, scratch, package, diff)
     with Progress(*Progress.get_default_columns(), transient=True) as progress:
         task = progress.add_task(description="Executing codemods...", total=len(files))
         count_errors = 0
         difflines: List[List[str]] = []
         with multiprocessing.Pool() as pool:
             for error, _difflines in pool.imap_unordered(partial_run_codemods, files):
```

### Comparing `bump_pydantic-0.4.0/bump_pydantic/.github/workflows/ci.yml` & `bump_pydantic-0.5.0/bump_pydantic/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/bump_pydantic/codemods/__init__.py` & `bump_pydantic-0.5.0/bump_pydantic/codemods/__init__.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/bump_pydantic/codemods/add_default_none.py` & `bump_pydantic-0.5.0/bump_pydantic/codemods/add_default_none.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.codemod import CodemodContext, VisitorBasedCodemodCommand
 from libcst.metadata import FullyQualifiedNameProvider, QualifiedName
 
-from bump_pydantic.codemods.mypy_visitor import CONTEXT_KEY
+from bump_pydantic.codemods.class_def_visitor import ClassDefVisitor
 
 
 class AddDefaultNoneCommand(VisitorBasedCodemodCommand):
     """This codemod adds the default value `None` to all fields of a pydantic model that
     are either type `Optional[T]`, `Union[T, None]` or `Any`.
 
     Example::
@@ -45,15 +45,15 @@
     def visit_ClassDef(self, node: cst.ClassDef) -> None:
         fqn_set = self.get_metadata(FullyQualifiedNameProvider, node)
 
         if not fqn_set:
             return None
 
         fqn: QualifiedName = next(iter(fqn_set))  # type: ignore
-        if self.context.scratch[CONTEXT_KEY].get(fqn.name, False):
+        if fqn.name in self.context.scratch[ClassDefVisitor.BASE_MODEL_CONTEXT_KEY]:
             self.inside_base_model = True
 
     def leave_ClassDef(self, original_node: cst.ClassDef, updated_node: cst.ClassDef) -> cst.ClassDef:
         self.inside_base_model = False
         return updated_node
 
     def visit_AnnAssign(self, node: cst.AnnAssign) -> None:
@@ -134,13 +134,10 @@
             )
             f.write(content)
         module = str(Path(module_path).relative_to(tmpdir))
         mrg = FullRepoManager(tmpdir, {module}, providers={FullyQualifiedNameProvider})
         wrapper = mrg.get_metadata_wrapper_for_path(module)
         context = CodemodContext(wrapper=wrapper)
 
-        # classes = run_mypy_visitor(context=context)
-        # mod = wrapper.visit(command)
-
         command = AddDefaultNoneCommand(context=context)  # type: ignore[assignment]
         mod = wrapper.visit(command)
         print(mod.code)
```

### Comparing `bump_pydantic-0.4.0/bump_pydantic/codemods/con_func.py` & `bump_pydantic-0.5.0/bump_pydantic/codemods/con_func.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/bump_pydantic/codemods/field.py` & `bump_pydantic-0.5.0/bump_pydantic/codemods/field.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/bump_pydantic/codemods/replace_config.py` & `bump_pydantic-0.5.0/bump_pydantic/codemods/replace_config.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/bump_pydantic/codemods/replace_generic_model.py` & `bump_pydantic-0.5.0/bump_pydantic/codemods/replace_generic_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/bump_pydantic/codemods/replace_imports.py` & `bump_pydantic-0.5.0/bump_pydantic/codemods/replace_imports.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/bump_pydantic/codemods/root_model.py` & `bump_pydantic-0.5.0/bump_pydantic/codemods/root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/bump_pydantic/codemods/validator.py` & `bump_pydantic-0.5.0/bump_pydantic/codemods/validator.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/folder.py` & `bump_pydantic-0.5.0/tests/integration/folder.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/test_cli.py` & `bump_pydantic-0.5.0/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/__init__.py` & `bump_pydantic-0.5.0/tests/integration/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/add_none.py` & `bump_pydantic-0.5.0/tests/integration/cases/add_none.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/base_settings.py` & `bump_pydantic-0.5.0/tests/integration/cases/base_settings.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/con_func.py` & `bump_pydantic-0.5.0/tests/integration/cases/con_func.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/config_to_model.py` & `bump_pydantic-0.5.0/tests/integration/cases/config_to_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/field.py` & `bump_pydantic-0.5.0/tests/integration/cases/field.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/folder_inside_folder.py` & `bump_pydantic-0.5.0/tests/integration/cases/folder_inside_folder.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/is_base_model.py` & `bump_pydantic-0.5.0/tests/integration/cases/is_base_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/replace_validator.py` & `bump_pydantic-0.5.0/tests/integration/cases/replace_validator.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/root_model.py` & `bump_pydantic-0.5.0/tests/integration/cases/root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/integration/cases/unicode.py` & `bump_pydantic-0.5.0/tests/integration/cases/unicode.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/unit/test_add_default_none.py` & `bump_pydantic-0.5.0/tests/unit/test_add_default_none.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import pytest
 from libcst import MetadataWrapper, parse_module
 from libcst.codemod import CodemodContext, CodemodTest
 from libcst.metadata import FullyQualifiedNameProvider
 from libcst.testing.utils import UnitTest
 
 from bump_pydantic.codemods.add_default_none import AddDefaultNoneCommand
-from bump_pydantic.codemods.mypy_visitor import CONTEXT_KEY, run_mypy_visitor
+from bump_pydantic.codemods.class_def_visitor import ClassDefVisitor
 
 
-@pytest.mark.skip(reason="The file needs to exists for the test to pass.")
 class TestClassDefVisitor(UnitTest):
     def add_default_none(self, file_path: str, code: str) -> cst.Module:
         mod = MetadataWrapper(
             parse_module(CodemodTest.make_fixture_data(code)),
             cache={
                 FullyQualifiedNameProvider: FullyQualifiedNameProvider.gen_cache(Path(""), [file_path], None).get(
                     file_path, ""
                 )
             },
         )
         mod.resolve_many(AddDefaultNoneCommand.METADATA_DEPENDENCIES)
         context = CodemodContext(wrapper=mod)
-        classes = run_mypy_visitor(arg_files=[file_path])
-        context.scratch.update({CONTEXT_KEY: classes})
+        instance = ClassDefVisitor(context=context)
+        mod.visit(instance)
 
         instance = AddDefaultNoneCommand(context=context)  # type: ignore[assignment]
         return mod.visit(instance)
 
     def test_no_annotations(self) -> None:
         source = textwrap.dedent(
             """class Potato:
```

### Comparing `bump_pydantic-0.4.0/tests/unit/test_class_def_visitor.py` & `bump_pydantic-0.5.0/tests/unit/test_class_def_visitor.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/unit/test_con_func.py` & `bump_pydantic-0.5.0/tests/unit/test_con_func.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/unit/test_field.py` & `bump_pydantic-0.5.0/tests/unit/test_field.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/unit/test_generic_model.py` & `bump_pydantic-0.5.0/tests/unit/test_generic_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/unit/test_replace_config.py` & `bump_pydantic-0.5.0/tests/unit/test_replace_config.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/unit/test_replace_imports.py` & `bump_pydantic-0.5.0/tests/unit/test_replace_imports.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/unit/test_root_model.py` & `bump_pydantic-0.5.0/tests/unit/test_root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/tests/unit/test_validator.py` & `bump_pydantic-0.5.0/tests/unit/test_validator.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/.gitignore` & `bump_pydantic-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/LICENSE.txt` & `bump_pydantic-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.4.0/README.md` & `bump_pydantic-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,27 @@
 
 ---
 
 ## Usage
 
 `bump-pydantic` is a CLI tool, hence you can use it from your terminal.
 
-To see the available options, you can run:
+It's easy to use. If your project structure is:
 
 ```bash
-bump-pydantic --help
+repository/
+└── my_package/
+    └── <python source files>
+```
+
+Then you'll want to do:
+
+```bash
+cd /path/to/repository
+bump-pydantic my_package
 ```
 
 ### Check diff before applying changes
 
 To check the diff before applying the changes, you can run:
 
 ```bash
```

### Comparing `bump_pydantic-0.4.0/pyproject.toml` & `bump_pydantic-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Framework :: Pydantic",
 ]
-dependencies = ["typer>=0.7.0", "libcst", "rich", "typing_extensions", "mypy"]
+dependencies = ["typer>=0.7.0", "libcst", "rich", "typing_extensions"]
 
 [project.urls]
 Documentation = "https://github.com/pydantic/bump-pydantic#readme"
 Issues = "https://github.com/pydantic/bump-pydantic/issues"
 Source = "https://github.com/pydantic/bump-pydantic"
 
 [project.scripts]
@@ -74,14 +74,19 @@
 isort = { known-first-party = ['bump_pydantic', 'tests'] }
 line-length = 120
 mccabe = { max-complexity = 14 }
 target-version = 'py38'
 
 [tool.pytest.ini_options]
 xfail_strict = true
+filterwarnings = [
+    # Turn warnings that aren't filtered into exceptions
+    "error",
+    "ignore::pytest.PytestUnraisableExceptionWarning"
+]
 
 [tool.coverage.run]
 branch = true
 source_pkgs = ["bump_pydantic"]
 
 [tool.coverage.report]
 exclude_lines = [
```

### Comparing `bump_pydantic-0.4.0/PKG-INFO` & `bump_pydantic-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-pydantic
-Version: 0.4.0
+Version: 0.5.0
 Summary: Convert Pydantic from V1 to V2 ♻
 Project-URL: Documentation, https://github.com/pydantic/bump-pydantic#readme
 Project-URL: Issues, https://github.com/pydantic/bump-pydantic/issues
 Project-URL: Source, https://github.com/pydantic/bump-pydantic
 Author-email: Marcelo Trylesinski <marcelotryle@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: libcst
-Requires-Dist: mypy
 Requires-Dist: rich
 Requires-Dist: typer>=0.7.0
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # Bump Pydantic ♻️
 
@@ -68,18 +67,27 @@
 
 ---
 
 ## Usage
 
 `bump-pydantic` is a CLI tool, hence you can use it from your terminal.
 
-To see the available options, you can run:
+It's easy to use. If your project structure is:
 
 ```bash
-bump-pydantic --help
+repository/
+└── my_package/
+    └── <python source files>
+```
+
+Then you'll want to do:
+
+```bash
+cd /path/to/repository
+bump-pydantic my_package
 ```
 
 ### Check diff before applying changes
 
 To check the diff before applying the changes, you can run:
 
 ```bash
```

