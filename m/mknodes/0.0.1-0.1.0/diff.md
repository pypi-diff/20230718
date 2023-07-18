# Comparing `tmp/mknodes-0.0.1.tar.gz` & `tmp/mknodes-0.1.0.tar.gz`

## Comparing `mknodes-0.0.1.tar` & `mknodes-0.1.0.tar`

### file list

```diff
@@ -1,54 +1,58 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mknodes-0.0.1/.editorconfig
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 mknodes-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 mknodes-0.0.1/Makefile
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 mknodes-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mknodes-0.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 mknodes-0.0.1/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 mknodes-0.0.1/docs/gen_pages.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 mknodes-0.0.1/docs/gen_qt.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/__init__.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/admonition.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/baseclasstable.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/binaryimage.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/classdiagram.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/classhelpers.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/classpage.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/classtable.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/code.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/connectionbuilder.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/diagram.py
--rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/docstrings.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/image.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/link.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/list.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/markdownnode.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/mermaid.py
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/mkpage.py
--rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/moduledocumentation.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/modulepage.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/moduletable.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/nav.py
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/node.py
--rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/noderesolver.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/snippet.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/sourceandresult.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/table.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/tabs.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/__linkreplacer/__init__.py
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 mknodes-0.0.1/mknodes/__linkreplacer/linkreplacer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 mknodes-0.0.1/tests/test_add.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mknodes-0.0.1/tests/test_docstrings.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 mknodes-0.0.1/tests/test_image.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 mknodes-0.0.1/tests/test_list.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mknodes-0.0.1/tests/test_markdownnode.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 mknodes-0.0.1/tests/test_mkpage.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 mknodes-0.0.1/tests/test_tabblock.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mknodes-0.0.1/tests/test_text.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 mknodes-0.0.1/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mknodes-0.0.1/LICENSE
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mknodes-0.0.1/README.md
--rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 mknodes-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 mknodes-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mknodes-0.1.0/.editorconfig
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 mknodes-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 mknodes-0.1.0/Makefile
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 mknodes-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mknodes-0.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 mknodes-0.1.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 mknodes-0.1.0/docs/gen_pages.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 mknodes-0.1.0/docs/gen_qt.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/__init__.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/admonition.py
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/baseclasstable.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/binaryimage.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/classdiagram.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/classhelpers.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/classpage.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/classtable.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/code.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/connectionbuilder.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/diagram.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/docstrings.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/image.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/link.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/list.py
+-rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/markdownnode.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/mermaid.py
+-rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/mkpage.py
+-rw-r--r--   0        0        0     9380 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/moduledocumentation.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/modulepage.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/moduletable.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/nav.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/node.py
+-rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/noderesolver.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/snippet.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/sourceandresult.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/table.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/tabs.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/__linkreplacer/__init__.py
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/__linkreplacer/linkreplacer.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/manual/__init__.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/manual/page_1.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/manual/page_2.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 mknodes-0.1.0/mknodes/manual/page_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_add.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_docstrings.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_image.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_list.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_markdownnode.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_mkpage.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_tabblock.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mknodes-0.1.0/tests/test_text.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 mknodes-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mknodes-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mknodes-0.1.0/README.md
+-rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 mknodes-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 mknodes-0.1.0/PKG-INFO
```

### Comparing `mknodes-0.0.1/.pre-commit-config.yaml` & `mknodes-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/Makefile` & `mknodes-0.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mkdocs.yml` & `mknodes-0.1.0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 - glightbox  # better image support
 - macros
 - include-markdown  # include content of other markdown files
 - literate-nav:  # move nav out of mkdocs.yml
     nav_file: SUMMARY.md
     # implicit_index: true
 # - autorefs  # allows linking to any header
-- linkreplacer  # allows linking to any markdown page (alternative: https://github.com/Jackiexiao/mkdocs-roamlinks-plugin)
+- linkreplacer  # allows linking to any markdown page
 - gen-files: # https://github.com/oprypin/mkdocs-gen-files
     scripts:
       - docs/gen_pages.py  # or any other name or path
 - mkdocstrings:
     default_handler: python
     handlers:
       python:
```

### Comparing `mknodes-0.0.1/.github/workflows/build.yml` & `mknodes-0.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/.github/workflows/documentation.yml` & `mknodes-0.1.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/docs/gen_qt.py` & `mknodes-0.1.0/docs/gen_qt.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/__init__.py` & `mknodes-0.1.0/mknodes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,8 @@
     "ModuleDocumentation",
     "TabBlock",
     "Tabbed",
     "SourceAndResult",
     "Snippet",
 ]
 
-__version__ = "0.0.1"
+__version__ = "0.1.0"
```

### Comparing `mknodes-0.0.1/mknodes/admonition.py` & `mknodes-0.1.0/mknodes/admonition.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/baseclasstable.py` & `mknodes-0.1.0/mknodes/baseclasstable.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class BaseClassTable(table.Table):
     """Table showing info for a list of classes."""
 
     def __init__(
         self,
         klasses: list[type],
         *,
-        layout: Literal["default", "extended"] = "default",
+        layout: Literal["default", "extended"] = "extended",
         filter_fn: Callable | None = None,
         **kwargs,
     ):
         self.klasses = klasses
         if filter_fn is None:
 
             def always_true(_):
```

### Comparing `mknodes-0.0.1/mknodes/binaryimage.py` & `mknodes-0.1.0/mknodes/binaryimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/classdiagram.py` & `mknodes-0.1.0/mknodes/classdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/classhelpers.py` & `mknodes-0.1.0/mknodes/classhelpers.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/classpage.py` & `mknodes-0.1.0/mknodes/classpage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import logging
 import os
 import pathlib
 
+from typing import Any
+
 from mknodes import (
     classdiagram,
     classhelpers,
     classtable,
     docstrings,
     mkpage,
     utils,
@@ -31,15 +33,15 @@
 
     def __init__(
         self,
         klass: type,
         *,
         module_path: tuple[str, ...] | str | None = None,
         path: str | os.PathLike = "",
-        **kwargs,
+        **kwargs: Any,
     ):
         path = pathlib.Path(f"{klass.__name__}.md")
         super().__init__(path=path, **kwargs)
         self.klass = klass
         match module_path:
             case None:
                 self.parts = klass.__module__.split(".")
```

### Comparing `mknodes-0.0.1/mknodes/classtable.py` & `mknodes-0.1.0/mknodes/classtable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/code.py` & `mknodes-0.1.0/mknodes/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         "pymdownx.inlinehilite",
         "pymdownx.snippets",
         "pymdownx.superfences",
     ]
 
     def __init__(
         self,
-        language: str,
         code: str | markdownnode.MkNode = "",
+        language: str = "py",
         *,
         title: str = "",
         header: str = "",
         linenums: int | None = None,
         highlight_lines: list[int] | None = None,
         parent=None,
     ):
@@ -69,13 +69,13 @@
         if extract_body and isinstance(obj, type | types.FunctionType | types.MethodType):
             code = utils.get_function_body(obj)
         elif extract_body:
             raise TypeError("Can only extract body from Functions, Methods and classes")
         else:
             code = inspect.getsource(obj)
         code = textwrap.dedent(code) if dedent else code
-        return cls(language="py", code=code, header=header)
+        return cls(code=code, header=header)
 
 
 if __name__ == "__main__":
     code = Code.for_object(Code, extract_body=True)
     print(code)
```

### Comparing `mknodes-0.0.1/mknodes/connectionbuilder.py` & `mknodes-0.1.0/mknodes/connectionbuilder.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/diagram.py` & `mknodes-0.1.0/mknodes/diagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/docstrings.py` & `mknodes-0.1.0/mknodes/docstrings.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         show_root_toc_entry: bool | None = None,
         show_root_full_path: bool | None = None,
         show_root_members_full_path: bool | None = None,
         show_object_full_path: bool | None = None,
         show_category_heading: bool | None = None,
         show_symbol_type_heading: bool | None = None,
         show_symbol_type_toc: bool | None = None,
+        inherited_members: bool | None = None,
         members: list[str] | None = None,
         members_order: Literal["alphabetical", "source"] | None = None,
         filters: list[str] | None = None,
         group_by_category: bool | None = None,
         show_submodules: bool | None = None,
         docstring_section_style: Literal["table", "list", "spacy"] | None = None,
         merge_init_into_class: bool | None = None,
@@ -79,14 +80,15 @@
             show_object_full_path: Show the full Python path of every object.
             show_category_heading: When grouped by categories, show a heading
                                    for each category.
             show_symbol_type_heading: Show the symbol type in headings (e.g. mod,
                                       class, func and attr).
             show_symbol_type_toc: Show the symbol type in the Table of
                                   Contents (e.g. mod, class, func and attr).
+            inherited_members: Also show inherited members.
             members: An explicit list of members to render.
             members_order: The members ordering to use.
             filters: A list of filters applied to filter objects based on their name.
                      A filter starting with ! will exclude matching objects instead of
                      including them. The members option takes precedence over filters
                      (filters will still be applied recursively to lower members in the
                      hierarchy).
@@ -140,14 +142,15 @@
         self.options["show_root_toc_entry"] = show_root_toc_entry
         self.options["show_root_full_path"] = show_root_full_path
         self.options["show_root_members_full_path"] = show_root_members_full_path
         self.options["show_object_full_path"] = show_object_full_path
         self.options["show_category_heading"] = show_category_heading
         self.options["show_symbol_type_heading"] = show_symbol_type_heading
         self.options["show_symbol_type_toc"] = show_symbol_type_toc
+        self.options["inherited_members"] = inherited_members
         self.options["members"] = members
         self.options["members_order"] = members_order
         self.options["filters"] = filters
         self.options["group_by_category"] = group_by_category
         self.options["show_submodules"] = show_submodules
         self.options["docstring_section_style"] = docstring_section_style
         self.options["merge_init_into_class"] = merge_init_into_class
```

### Comparing `mknodes-0.0.1/mknodes/image.py` & `mknodes-0.1.0/mknodes/image.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/link.py` & `mknodes-0.1.0/mknodes/link.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/list.py` & `mknodes-0.1.0/mknodes/list.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/markdownnode.py` & `mknodes-0.1.0/mknodes/markdownnode.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,31 +57,36 @@
         text = self._to_markdown()
         if self.indent:
             text = textwrap.indent(text, self.indent)
         return f"## {self.header}\n\n{text}" if self.header else text
 
     @property
     def resolved_parts(self) -> tuple[str, ...]:
+        """Returns a tuple containing all section names."""
         from mknodes import nav
 
         parent = self
         parts = [self.section] if isinstance(self, nav.Nav) and self.section else []
         while parent := parent.parent_item:
             if isinstance(parent, nav.Nav) and parent.section:
                 parts.append(parent.section)
         return tuple(reversed(parts))
 
     @property
     def resolved_file_path(self) -> str:
+        """Returns the resulting section/subsection/../filename.xyz path."""
         filename = str(self.path) if hasattr(self, "path") else ""
         path = "/".join(self.resolved_parts) + "/" + filename
         return path
 
     def virtual_files(self):
-        """Virtual, this can be overridden by nodes if they want files to be included."""
+        """Returns a dict containing the virtual files attached to this tree element.
+
+        This can be overridden by nodes if they want files to be included in the build.
+        """
         return {}
 
     def all_virtual_files(self) -> dict[str, str | bytes]:
         """Return a dictionary containing all virtual files of itself and all children.
 
         Dict key contains the filename, dict value contains the file content.
 
@@ -145,15 +150,15 @@
     def __repr__(self):
         return utils.get_repr(self, items=self.items)
 
     @staticmethod
     def examples():
         from mknodes import code
 
-        yield dict(items=[code.Code(language="py", code="a = 1 + 2"), Text("abc")])
+        yield dict(items=[code.Code(code="a = 1 + 2"), Text("abc")])
 
     def _to_markdown(self) -> str:
         return "\n\n".join(i.to_markdown() for i in self.items)
 
     def append(self, other: str | MkNode):
         other = Text(other, parent=self) if isinstance(other, str) else other
         self.items.append(other)
```

### Comparing `mknodes-0.0.1/mknodes/mermaid.py` & `mknodes-0.1.0/mknodes/mermaid.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/mkpage.py` & `mknodes-0.1.0/mknodes/mkpage.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from typing import Any, Literal
 
 from mknodes import (
     admonition,
     code as codeblock,
     docstrings,
+    link,
     markdownnode,
     nav,
     tabs,
     utils,
 )
 
 
@@ -79,14 +80,29 @@
         """Add line separators to the page.
 
         Arguments:
             num: Amount of newlines to add.
         """
         self.append("<br>" * num)
 
+    def add_link(
+        self,
+        url: str,
+        title: str = "",
+    ) -> link.Link:
+        """Add a Link to the page.
+
+        Arguments:
+            url: URL to link to.
+            title: Text to display for the link
+        """
+        item = link.Link(url)
+        self.append(item)
+        return item
+
     def add_header(self, text: str, level: int = 2):
         """Add line separators to the page.
 
         Arguments:
             text: header text
             level: header level
         """
@@ -241,15 +257,15 @@
         )
         self.append(item)
         return item
 
     def add_code(
         self,
         code: str | markdownnode.MkNode,
-        language: str = "",
+        language: str = "py",
         *,
         title: str = "",
         header: str = "",
         linenums: int | None = None,
         highlight_lines: list[int] | None = None,
     ):
         """Add code block to the page.
@@ -273,16 +289,16 @@
         )
         self.append(item)
         return item
 
     def add_tabs(
         self,
         data: Mapping[str, str | markdownnode.MkNode],
-        style="tabbed",
-        **kwargs,
+        style: Literal["tabbed", "tabblock"] = "tabbed",
+        **kwargs: Any,
     ):
         """Add tabs to the page.
 
         Arguments:
             data: tab data
             style: Whether to use new-style (tabblock) or old-style (tabbed) tabs.
             kwargs: Keyword arguments passed to Tabs
@@ -293,10 +309,11 @@
             tabblock = tabs.TabBlock(data, parent=self, **kwargs)
         self.append(tabblock)
         return tabblock
 
 
 if __name__ == "__main__":
     doc = MkPage()
+    doc.add_link("test")
     doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
     print(doc)
     # print(doc.children)
```

### Comparing `mknodes-0.0.1/mknodes/moduledocumentation.py` & `mknodes-0.1.0/mknodes/moduledocumentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 # import contextlib
 # import importlib
 import inspect
 import logging
 import pathlib
 import types
 
+from typing import Any
+
 from mknodes import classhelpers, classpage, modulepage, nav, utils
 
 
 logger = logging.getLogger(__name__)
 
 
 class ModuleDocumentation(nav.Nav):
@@ -143,15 +145,20 @@
                     submodule=submod,
                     recursive=True,
                     predicate=predicate,
                     _seen=seen,
                 )
 
     def add_class_page(
-        self, klass: type, *, find_topmost: bool = True, flatten: bool = False, **kwargs
+        self,
+        klass: type,
+        *,
+        find_topmost: bool = True,
+        flatten: bool = False,
+        **kwargs: Any,
     ) -> classpage.ClassPage:
         """Add a page showing information about a class.
 
         Arguments:
             klass: klass to build a page for
             find_topmost: Whether to use a module path from a parent package if available
             flatten: Put page into top level nav if nested.
@@ -180,15 +187,17 @@
     #         path=pathlib.Path("index.md"),
     #         # parent=self,
     #     )
     #     page += mknodes.ModuleTable(self.module_name, predicate=predicate)
     #     return page
 
     def add_module_overview(
-        self, title: str | None = None, **kwargs
+        self,
+        title: str | None = None,
+        **kwargs: Any,
     ) -> modulepage.ModulePage:
         """Add a page showing all submodules.
 
         Arguments:
             title: Override title for the section.
             kwargs: kwargs passed to ModulePage.
         """
```

### Comparing `mknodes-0.0.1/mknodes/modulepage.py` & `mknodes-0.1.0/mknodes/modulepage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/moduletable.py` & `mknodes-0.1.0/mknodes/moduletable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/nav.py` & `mknodes-0.1.0/mknodes/nav.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,23 +53,21 @@
     def __repr__(self):
         return utils.get_repr(
             self,
             section=self.section or "<root>",
             filename=self.filename,
         )
 
-    def __setitem__(self, item: tuple | str, value: mkpage.MkPage | Nav):
+    def __setitem__(self, item: tuple | str, node: mkpage.MkPage | Nav):
         if isinstance(item, str):
             item = tuple(item.split("."))
-        self.nav[item] = value
+        self.nav[item] = node
 
-    #     self._mapping[item] = value
-
-    # def __getitem__(self, item):
-    #     return self._mapping[item]
+    def __getitem__(self, index: tuple) -> mkpage.MkPage | Nav:
+        return self.nav[index]
 
     @property
     def navs(self):
         return [node for node in self.nav.values() if isinstance(node, Nav)]
 
     @property
     def pages(self):
@@ -89,14 +87,18 @@
         Arguments:
             section: Name of the new nav.
         """
         navi = nav.Nav(section=section, parent=self)
         self.nav[(section,)] = navi
         return navi
 
+    def add_index_page(self) -> mkpage.MkPage:
+        page = mkpage.MkPage(path="index.md", hide_toc=True, hide_nav=True, parent=self)
+        return page
+
     def write_navs(self):
         for navi in self.navs:
             navi.write()
 
     def virtual_files(self) -> dict[str, str]:
         return {str(self.path): self.to_markdown()}
 
@@ -116,17 +118,17 @@
         self,
         title: str,
         *,
         hide_toc: bool = False,
         hide_nav: bool = False,
         hide_path: bool = False,
         filename: str | None = None,
-    ):
+    ) -> mkpage.MkPage:
         """Add a page to the Nav."""
-        filename = filename or f"{title}.md"
+        filename = filename or utils.slugify(f"{title}.md")
         page = mkpage.MkPage(
             path=filename,
             parent=self,
             hide_toc=hide_toc,
             hide_nav=hide_nav,
             hide_path=hide_path,
         )
```

### Comparing `mknodes-0.0.1/mknodes/node.py` & `mknodes-0.1.0/mknodes/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 
     def __repr__(self):
         return utils.get_repr(self)
 
     def __iter__(self) -> Iterator[Self]:
         yield from self.children
 
-    def __getitem__(self, index: int) -> Self:
-        return self.children[index]
-
     def __rshift__(self, other: Self):
         """Set children using >> bitshift operator for self >> other.
 
         Args:
             other (Self): other node, children
         """
         other.parent_item = self
@@ -154,24 +151,24 @@
     def row(self) -> int:
         if self.parent_item:
             return self.parent_item.children.index(self)  # type: ignore
         else:
             return 0
 
     def pprint(self, indent: int = 0, max_depth: int | None = None):
-        for _indent, child_item in self.yield_nodes(indent, max_depth):
+        for _indent, child_item in self.iter_nodes(indent, max_depth):
             text = _indent * "    " + repr(child_item)
             logger.warning(text)
 
-    def yield_nodes(self, indent: int = 0, max_depth: int | None = None):
+    def iter_nodes(self, indent: int = 0, max_depth: int | None = None):
         if max_depth is not None and indent > max_depth:
             return
         yield indent, self
         for child_item in self.children:
-            yield from child_item.yield_nodes(indent + 1)
+            yield from child_item.iter_nodes(indent + 1)
 
 
 def preorder_iter(
     tree: BaseNode,
     filter_condition: Callable[[BaseNode], bool] | None = None,
     stop_condition: Callable[[BaseNode], bool] | None = None,
     max_depth: int = 0,
```

### Comparing `mknodes-0.0.1/mknodes/noderesolver.py` & `mknodes-0.1.0/mknodes/noderesolver.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/snippet.py` & `mknodes-0.1.0/mknodes/snippet.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/sourceandresult.py` & `mknodes-0.1.0/mknodes/sourceandresult.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, fn: Callable, header: str = ""):
         super().__init__(header)
         self.fn = fn
 
     @staticmethod
     def examples():
         def test():
-            return code.Code(language="py", code="a = 2 + 4")
+            return code.Code(code="a = 2 + 4")
 
         yield dict(fn=test)
 
     def __str__(self):
         return self.to_markdown()
 
     def __repr__(self):
```

### Comparing `mknodes-0.0.1/mknodes/table.py` & `mknodes-0.1.0/mknodes/table.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/tabs.py` & `mknodes-0.1.0/mknodes/tabs.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/mknodes/utils.py` & `mknodes-0.1.0/mknodes/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,21 @@
         escape_chars = r"\)"
     else:
         escape_chars = r"_*[]()~`>#+-=|{}.!"
 
     return re.sub(f"([{re.escape(escape_chars)}])", r"\\\1", text)
 
 
+def slugify(text: str) -> str:
+    text = text.lower()
+    text = re.sub("[^0-9a-zA-Z_.]", "_", text)
+    text = re.sub("^[^a-zA-Z_#]+", "", text)
+    return text
+
+
 def groupby(data, keyfunc: Callable | None = None):
     data = sorted(data, key=keyfunc or (lambda x: x))
     return {k: list(g) for k, g in itertools.groupby(data, keyfunc)}
 
 
 def groupby_first_letter(data, keyfunc: Callable | None = None):
     data = sorted(data, key=keyfunc or (lambda x: x))
@@ -90,15 +97,20 @@
 # with path.open("rb") as file:
 #     inv = inventory.Inventory.parse_sphinx(file)
 
 #     logger.warning(inv.values())
 
 
 def linked(identifier: str, title: str | None = None) -> str:
-    suffix = "" if identifier.startswith(("http:", "https:", "www.")) else ".md"
+    suffix = (
+        ""
+        if identifier.startswith(("http:", "https:", "www."))
+        or identifier.endswith(".md")
+        else ".md"
+    )
     return f"[{identifier if title is None else title}]({identifier}{suffix})"
 
 
 def styled(
     text: str,
     size: int | None = None,
     bold: bool = False,
```

### Comparing `mknodes-0.0.1/mknodes/__linkreplacer/linkreplacer.py` & `mknodes-0.1.0/mknodes/__linkreplacer/linkreplacer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/tests/test_add.py` & `mknodes-0.1.0/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/.gitignore` & `mknodes-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/LICENSE` & `mknodes-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/README.md` & `mknodes-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.0.1/pyproject.toml` & `mknodes-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,14 @@
     "SLF001",# Private member accessed
     "RUF012", # Mutable class attributes should be annotated
     "RUF013", # PEP 484 prohibits implicit `Optional`
 ]
 extend-exclude = [
     'docs',
     '__init__.py',
-    "prettyqt/qt/",
 ]
 target-version = "py310"
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.ruff.isort]
```

### Comparing `mknodes-0.0.1/PKG-INFO` & `mknodes-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknodes
-Version: 0.0.1
+Version: 0.1.0
 Summary: Generate docs with ease.
 Project-URL: Documentation, https://phil65.github.io/mknodes/
 Project-URL: Source, https://github.com/phil65/mknodes
 Author-email: mknodes <philipptemminghoff@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mknodes Version: 0.0.1 Summary: Generate docs with
+Metadata-Version: 2.1 Name: mknodes Version: 0.1.0 Summary: Generate docs with
 ease. Project-URL: Documentation, https://phil65.github.io/mknodes/ Project-
 URL: Source, https://github.com/phil65/mknodes Author-email: mknodes
 gmail.com> License-File: LICENSE Classifier: Programming Language :: Python ::
 3 :: Only Requires-Python: >=3.10 Requires-Dist: mkdocs Requires-Dist: mkdocs-
 gen-files Requires-Dist: typing-extensions Description-Content-Type: text/
 markdown # MkNodes
                            Generate docs with ease.
```

