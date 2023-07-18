# Comparing `tmp/rispy-0.8.0.tar.gz` & `tmp/rispy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rispy-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rispy-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rispy-0.8.0.tar` & `rispy-0.8.1.tar`

### file list

```diff
@@ -1,31 +1,29 @@
--rw-r--r--   0        0        0       95 2023-06-07 11:31:31.290631 rispy-0.8.0/.flake8
--rw-r--r--   0        0        0      573 2023-07-13 19:04:25.612108 rispy-0.8.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      245 2023-06-07 11:31:31.290980 rispy-0.8.0/.gitignore
--rw-r--r--   0        0        0     3183 2023-07-13 19:04:35.135681 rispy-0.8.0/HISTORY.rst
--rw-r--r--   0        0        0     1070 2023-07-13 19:04:25.612752 rispy-0.8.0/LICENSE
--rw-r--r--   0        0        0     1328 2023-07-13 19:04:25.613134 rispy-0.8.0/Makefile
--rw-r--r--   0        0        0    10490 2023-07-13 19:04:25.613611 rispy-0.8.0/README.rst
--rw-r--r--   0        0        0     1291 2023-07-13 19:04:25.614044 rispy-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-07 11:31:31.291777 rispy-0.8.0/pytest.ini
--rw-r--r--   0        0        0      525 2023-07-13 19:04:35.135988 rispy-0.8.0/rispy/__init__.py
--rw-r--r--   0        0        0     5780 2023-07-13 16:16:46.968010 rispy-0.8.0/rispy/config.py
--rw-r--r--   0        0        0    13412 2023-07-13 19:04:25.614790 rispy-0.8.0/rispy/parser.py
--rw-r--r--   0        0        0     1640 2023-07-13 19:04:25.615134 rispy-0.8.0/rispy/utils.py
--rw-r--r--   0        0        0     7552 2023-07-13 19:04:25.615512 rispy-0.8.0/rispy/writer.py
--rw-r--r--   0        0        0      168 2023-06-07 11:31:31.292903 rispy-0.8.0/tests/data/example_basic.ris
--rw-r--r--   0        0        0       54 2023-06-07 11:31:31.293000 rispy-0.8.0/tests/data/example_bom.ris
--rw-r--r--   0        0        0       98 2023-06-07 11:31:31.293092 rispy-0.8.0/tests/data/example_custom_list_tags.ris
--rw-r--r--   0        0        0     1901 2023-06-07 11:31:31.293273 rispy-0.8.0/tests/data/example_extraneous_data.ris
--rw-r--r--   0        0        0     1759 2023-06-07 11:31:31.293426 rispy-0.8.0/tests/data/example_full.ris
--rw-r--r--   0        0        0     1757 2023-06-07 11:31:31.293549 rispy-0.8.0/tests/data/example_full_without_whitespace.ris
--rw-r--r--   0        0        0     1617 2023-07-13 19:04:52.587777 rispy-0.8.0/tests/data/example_full_write.ris
--rw-r--r--   0        0        0      192 2023-06-07 11:31:31.293736 rispy-0.8.0/tests/data/example_multi_unknown_tags.ris
--rw-r--r--   0        0        0      202 2023-06-07 11:31:31.293831 rispy-0.8.0/tests/data/example_single_unknown_tag.ris
--rw-r--r--   0        0        0      170 2023-06-07 11:31:31.293924 rispy-0.8.0/tests/data/example_starting_newlines.ris
--rw-r--r--   0        0        0      847 2023-07-11 15:17:37.154523 rispy-0.8.0/tests/data/example_urls.ris
--rw-r--r--   0        0        0      910 2023-06-07 11:31:31.294031 rispy-0.8.0/tests/data/example_utf_chars.ris
--rw-r--r--   0        0        0    16195 2023-06-07 11:31:31.294243 rispy-0.8.0/tests/data/example_wos.ris
--rw-r--r--   0        0        0      302 2023-06-07 11:31:31.294342 rispy-0.8.0/tests/data/multiline.ris
--rw-r--r--   0        0        0    15625 2023-07-13 19:04:25.615918 rispy-0.8.0/tests/test_parser.py
--rw-r--r--   0        0        0     5270 2023-07-13 19:04:25.616266 rispy-0.8.0/tests/test_writer.py
--rw-r--r--   0        0        0    11449 1970-01-01 00:00:00.000000 rispy-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-07-18 01:34:06.811306 rispy-0.8.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      271 2023-07-14 01:54:30.633436 rispy-0.8.1/.gitignore
+-rw-r--r--   0        0        0     3317 2023-07-18 01:34:06.811572 rispy-0.8.1/HISTORY.rst
+-rw-r--r--   0        0        0     1070 2023-07-13 19:04:25.612752 rispy-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1345 2023-07-18 01:34:06.811776 rispy-0.8.1/Makefile
+-rw-r--r--   0        0        0    10490 2023-07-13 19:04:25.613611 rispy-0.8.1/README.rst
+-rw-r--r--   0        0        0     1353 2023-07-14 01:53:37.354446 rispy-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      525 2023-07-18 01:34:06.811968 rispy-0.8.1/rispy/__init__.py
+-rw-r--r--   0        0        0     5780 2023-07-13 16:16:46.968010 rispy-0.8.1/rispy/config.py
+-rw-r--r--   0        0        0    13496 2023-07-17 22:50:31.442772 rispy-0.8.1/rispy/parser.py
+-rw-r--r--   0        0        0     1640 2023-07-13 19:04:25.615134 rispy-0.8.1/rispy/utils.py
+-rw-r--r--   0        0        0     8299 2023-07-17 22:50:31.443080 rispy-0.8.1/rispy/writer.py
+-rw-r--r--   0        0        0      168 2023-06-07 11:31:31.292903 rispy-0.8.1/tests/data/example_basic.ris
+-rw-r--r--   0        0        0       54 2023-06-07 11:31:31.293000 rispy-0.8.1/tests/data/example_bom.ris
+-rw-r--r--   0        0        0       98 2023-06-07 11:31:31.293092 rispy-0.8.1/tests/data/example_custom_list_tags.ris
+-rw-r--r--   0        0        0     1901 2023-06-07 11:31:31.293273 rispy-0.8.1/tests/data/example_extraneous_data.ris
+-rw-r--r--   0        0        0     1759 2023-06-07 11:31:31.293426 rispy-0.8.1/tests/data/example_full.ris
+-rw-r--r--   0        0        0     1757 2023-06-07 11:31:31.293549 rispy-0.8.1/tests/data/example_full_without_whitespace.ris
+-rw-r--r--   0        0        0     1617 2023-07-14 01:53:26.486049 rispy-0.8.1/tests/data/example_full_write.ris
+-rw-r--r--   0        0        0      192 2023-06-07 11:31:31.293736 rispy-0.8.1/tests/data/example_multi_unknown_tags.ris
+-rw-r--r--   0        0        0      202 2023-06-07 11:31:31.293831 rispy-0.8.1/tests/data/example_single_unknown_tag.ris
+-rw-r--r--   0        0        0      170 2023-06-07 11:31:31.293924 rispy-0.8.1/tests/data/example_starting_newlines.ris
+-rw-r--r--   0        0        0      847 2023-07-11 15:17:37.154523 rispy-0.8.1/tests/data/example_urls.ris
+-rw-r--r--   0        0        0      910 2023-06-07 11:31:31.294031 rispy-0.8.1/tests/data/example_utf_chars.ris
+-rw-r--r--   0        0        0    16195 2023-06-07 11:31:31.294243 rispy-0.8.1/tests/data/example_wos.ris
+-rw-r--r--   0        0        0      302 2023-06-07 11:31:31.294342 rispy-0.8.1/tests/data/multiline.ris
+-rw-r--r--   0        0        0    15625 2023-07-13 19:04:25.615918 rispy-0.8.1/tests/test_parser.py
+-rw-r--r--   0        0        0     6727 2023-07-17 22:50:31.443317 rispy-0.8.1/tests/test_writer.py
+-rw-r--r--   0        0        0    11449 1970-01-01 00:00:00.000000 rispy-0.8.1/PKG-INFO
```

### Comparing `rispy-0.8.0/.github/workflows/main.yml` & `rispy-0.8.1/.github/workflows/main.yml`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   backend:
     name: lint + test
     runs-on: ubuntu-22.04
 
     strategy:
       max-parallel: 4
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12-dev"]
 
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: install
```

### Comparing `rispy-0.8.0/HISTORY.rst` & `rispy-0.8.1/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 History
 =======
 
+v0.8.1 (2023-07-17)
+-------------------
+
+* Update RIS exporter to optionally write list tags or delimited single tags (@scott-8 #55)
+
 v0.8.0 (2023-07-13)
 -------------------
 
 Breaking changes:
 
 * Update minimum python version from 3.6 to 3.8
 * Improve URL parsing to be more robust and consistent with the spec; saved as a plural "urls" dictionary key instead of the singular "url" (@scott-8/shapiromatron #52)
```

### Comparing `rispy-0.8.0/LICENSE` & `rispy-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/Makefile` & `rispy-0.8.1/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 	match = re.match(r'^([a-zA-Z_-]+):.*?## (.*)$$', line)
 	if match:
 		target, help = match.groups()
 		print("%-20s %s" % (target, help))
 endef
 export PRINT_HELP_PYSCRIPT
 
+VERSION := $(shell python -c "import rispy; print(rispy.__version__)")
 
 help:
 	@python -c "$$PRINT_HELP_PYSCRIPT" < $(MAKEFILE_LIST)
 
 clean:  ## Remove all build, test and Python artifacts
 	# build artifacts
 	rm -fr build/
@@ -47,9 +48,9 @@
 
 build: clean ## builds source and wheel package
 	flit build
 	ls -l dist
 
 publish: ## package and upload a release
 	flit publish
-	git tag -a "$(python -c 'import rispy; print(rispy.__version__)')" -m ""
+	git tag $(VERSION)
 	git push --tags
```

### Comparing `rispy-0.8.0/README.rst` & `rispy-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/pyproject.toml` & `rispy-0.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -38,19 +38,22 @@
 build-backend = "flit_core.buildapi"
 
 [tool.black]
 line-length = 98
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
+[tool.coverage.run]
+omit = [
+    "tests/*",
+]
+
 [tool.ruff]
 line-length = 100
 target-version = "py38"
 select = ["F", "E", "W", "I", "UP", "S", "B", "T20", "RUF"]
 
 [tool.ruff.per-file-ignores]
 "test_*.py" = ["S101"]
 
-[tool.coverage.run]
-omit = [
-    "tests/*",
-]
+[tool.pytest.ini_options]
+addopts = "--doctest-glob='*.rst'"
```

### Comparing `rispy-0.8.0/rispy/__init__.py` & `rispy-0.8.1/rispy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A Python reader/writer of RIS reference files"""
 
 from .config import LIST_TYPE_TAGS, TAG_KEY_MAPPING, TYPE_OF_REFERENCE_MAPPING
 from .parser import BaseParser, RisParser, WokParser, load, loads
 from .writer import BaseWriter, RisWriter, dump, dumps
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 __all__ = [
     "__version__",
     "LIST_TYPE_TAGS",
     "TAG_KEY_MAPPING",
     "TYPE_OF_REFERENCE_MAPPING",
     "load",
```

### Comparing `rispy-0.8.0/rispy/config.py` & `rispy-0.8.1/rispy/config.py`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/rispy/parser.py` & `rispy-0.8.1/rispy/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,37 +55,38 @@
         clean_text: Clean the text body before parsing begins. By default,
                     it removes UTF-BOM characters.
 
     """
 
     START_TAG: str
     END_TAG: str = "ER"
+    UNKNOWN_TAG: str = "UK"
     PATTERN: str
     DEFAULT_IGNORE: ClassVar[List[str]] = []
     DEFAULT_MAPPING: Dict
     DEFAULT_LIST_TAGS: List[str]
     DEFAULT_DELIMITER_MAPPING: Dict
 
     def __init__(
         self,
         *,
         mapping: Optional[Dict] = None,
         list_tags: Optional[List[str]] = None,
-        delimiter_mapping: Optional[Dict] = None,
+        delimiter_tags_mapping: Optional[Dict] = None,
         ignore: Optional[List[str]] = None,
         skip_missing_tags: bool = False,
         skip_unknown_tags: bool = False,
         enforce_list_tags: bool = True,
     ):
         """Initialize the parser function.
 
         Args:
             mapping (dict, optional): Map tags to tag names.
             list_tags (list, optional): List of list-type tags.
-            delimiter_mapping (dict, optional): Map of delimiters to tags.
+            delimiter_tags_mapping (dict, optional): Map of delimiters to tags.
             ignore (list, optional): List of tags to ignore.
             skip_missing_tags (bool, optional): Bool to skip lines that don't have
                                                 valid tags, regardless of whether
                                                 of where they are in a reference.
                                                 This is the inverse of the former
                                                 `strict` parameter. If the goal is
                                                 to skip reference headers, see the
@@ -106,15 +107,17 @@
                                                 list tags. Defaults to `True`.
 
         """
         self.pattern = re.compile(self.PATTERN)
         self.mapping = mapping if mapping is not None else self.DEFAULT_MAPPING
         self.list_tags = list_tags if list_tags is not None else self.DEFAULT_LIST_TAGS
         self.delimiter_map = (
-            delimiter_mapping if delimiter_mapping is not None else self.DEFAULT_DELIMITER_MAPPING
+            delimiter_tags_mapping
+            if delimiter_tags_mapping is not None
+            else self.DEFAULT_DELIMITER_MAPPING
         )
         self.ignore = ignore if ignore is not None else self.DEFAULT_IGNORE
         self.skip_missing_tags = skip_missing_tags
         self.skip_unknown_tags = skip_unknown_tags
         self.enforce_list_tags = enforce_list_tags
 
     def parse(self, text: str) -> List[Dict]:
@@ -236,15 +239,15 @@
 
         if tag in self.list_tags:
             self._add_list_value(name, new_value)
         else:
             self._add_single_value(name, new_value, is_multi=all_line)
 
     def _add_unknown_tag(self, tag, line):
-        name = self.mapping["UK"]
+        name = self.mapping[self.UNKNOWN_TAG]
         value = self.get_content(line)
         # check if unknown_tag dict exists
         if name not in self.current:
             self.current[name] = defaultdict(list)
 
         self.current[name][tag].append(value)
```

### Comparing `rispy-0.8.0/rispy/utils.py` & `rispy-0.8.1/rispy/utils.py`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/rispy/writer.py` & `rispy-0.8.1/rispy/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """RIS Writer."""
 
 import warnings
 from abc import ABC
 from typing import ClassVar, Dict, List, Optional, TextIO, Type
 
-from .config import LIST_TYPE_TAGS, TAG_KEY_MAPPING
+from .config import DELIMITED_TAG_MAPPING, LIST_TYPE_TAGS, TAG_KEY_MAPPING
 from .utils import invert_dictionary
 
 __all__ = ["dump", "dumps", "BaseWriter", "RisWriter"]
 
 
 class BaseWriter(ABC):
     """Base writer class. Create a subclass to use.
@@ -35,55 +35,65 @@
         set_header: Create a header for each reference. Has the reference
                     number as a parameter.
 
     """
 
     START_TAG: str
     END_TAG: str = "ER"
+    UNKNOWN_TAG: str = "UK"
     PATTERN: str
     DEFAULT_IGNORE: ClassVar[List[str]] = []
     DEFAULT_MAPPING: Dict
     DEFAULT_LIST_TAGS: List[str]
+    DEFAULT_DELIMITER_MAPPING: Dict
     DEFAULT_REFERENCE_TYPE: str = "JOUR"
+    REFERENCE_TYPE_KEY: str = "type_of_reference"
     SEPARATOR: Optional[str] = "\n"
 
     def __init__(
         self,
         *,
         mapping: Optional[Dict] = None,
         list_tags: Optional[List[str]] = None,
+        delimiter_tags_mapping: Optional[Dict] = None,
         ignore: Optional[List[str]] = None,
         skip_unknown_tags: bool = False,
         enforce_list_tags: bool = True,
     ):
         """Override default tag map and list tags in instance.
 
         Args:
             mapping (dict, optional): Map tags to tag names.
             list_tags (list, optional): List of list-type tags.
+            delimiter_tags_mapping (dict, optional): Map of delimiters to tags.
             ignore (list, optional): List of tags to ignore.
             skip_unknown_tags (bool, optional): Bool for whether to write unknown
                                                 tags to the file. Defaults to
                                                 `False`.
             enforce_list_tags (bool, optional): If `True` tags that are not set as
                                                 list tags will be written into one
                                                 line. Defaults to `True`.
 
         """
         self.mapping = mapping if mapping is not None else self.DEFAULT_MAPPING
         self.list_tags = list_tags if list_tags is not None else self.DEFAULT_LIST_TAGS
+        self.delimiter_map = (
+            delimiter_tags_mapping
+            if delimiter_tags_mapping is not None
+            else self.DEFAULT_DELIMITER_MAPPING
+        )
         self.ignore = ignore if ignore is not None else self.DEFAULT_IGNORE
         self._rev_mapping = invert_dictionary(self.mapping)
         self.skip_unknown_tags = skip_unknown_tags
         self.enforce_list_tags = enforce_list_tags
 
     def _get_reference_type(self, ref):
-        if "type_of_reference" in ref.keys():
+        if self.REFERENCE_TYPE_KEY in ref:
             # TODO add check
-            return ref["type_of_reference"]
+            return ref[self.REFERENCE_TYPE_KEY]
 
         if self.DEFAULT_REFERENCE_TYPE is not None:
             return self.DEFAULT_REFERENCE_TYPE
         else:
             raise ValueError("Unknown type of reference")
 
     def _format_line(self, tag, value=""):
@@ -96,15 +106,15 @@
         header = self.set_header(count)
         if header is not None:
             lines.append(header)
         lines.append(self._format_line(self.START_TAG, self._get_reference_type(ref)))
 
         tags_to_skip = [self.START_TAG, *self.ignore]
         if self.skip_unknown_tags:
-            tags_to_skip.append("UK")
+            tags_to_skip.append(self.UNKNOWN_TAG)
 
         for label, value in ref.items():
             # not available
             try:
                 tag = self._rev_mapping[label.lower()]
             except KeyError:
                 warnings.warn(UserWarning(f"label `{label}` not exported"), stacklevel=2)
@@ -116,24 +126,29 @@
 
             # list tag
             if tag in self.list_tags or (not self.enforce_list_tags and isinstance(value, list)):
                 for val_i in value:
                     lines.append(self._format_line(tag, val_i))
 
             # unknown tag(s), which are lists held in a defaultdict
-            elif tag == "UK":
+            elif tag == self.UNKNOWN_TAG:
                 for unknown_tag in value.keys():
                     for val_i in value[unknown_tag]:
                         lines.append(self._format_line(unknown_tag, val_i))
 
+            # write delimited tags
+            elif tag in self.delimiter_map:
+                combined_val = self.delimiter_map[tag].join(value)
+                lines.append(self._format_line(tag, combined_val))
+
             # all non-list tags
             else:
                 lines.append(self._format_line(tag, value))
 
-        lines.append(self._format_line("ER"))
+        lines.append(self._format_line(self.END_TAG))
 
         if self.SEPARATOR is not None:
             lines.append(self.SEPARATOR.replace("\n", "", 1))
 
         return lines
 
     def _format_all_references(self, references):
@@ -155,14 +170,15 @@
 class RisWriter(BaseWriter):
     """Subclass of BaseWriter for writing RIS files."""
 
     START_TAG = "TY"
     PATTERN = "{tag}  - {value}"
     DEFAULT_MAPPING = TAG_KEY_MAPPING
     DEFAULT_LIST_TAGS = LIST_TYPE_TAGS
+    DEFAULT_DELIMITER_MAPPING = DELIMITED_TAG_MAPPING
 
     def set_header(self, count):
         return f"{count}."
 
 
 def dump(
     references: List[Dict],
```

### Comparing `rispy-0.8.0/tests/data/example_extraneous_data.ris` & `rispy-0.8.1/tests/data/example_extraneous_data.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/tests/data/example_full.ris` & `rispy-0.8.1/tests/data/example_full.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/tests/data/example_full_without_whitespace.ris` & `rispy-0.8.1/tests/data/example_full_without_whitespace.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/tests/data/example_full_write.ris` & `rispy-0.8.1/tests/data/example_full_write.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/tests/data/example_urls.ris` & `rispy-0.8.1/tests/data/example_urls.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/tests/data/example_utf_chars.ris` & `rispy-0.8.1/tests/data/example_utf_chars.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/tests/data/example_wos.ris` & `rispy-0.8.1/tests/data/example_wos.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/tests/test_parser.py` & `rispy-0.8.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `rispy-0.8.0/tests/test_writer.py` & `rispy-0.8.1/tests/test_writer.py`

 * *Files 15% similar despite different names*

```diff
@@ -187,7 +187,51 @@
     text_output = rispy.dumps(entries)
 
     # check output is as expected
     lines = text_output.splitlines()
     assert lines[6] == "JP  - CRISPR"
     assert lines[7] == "ED  - Swinburne, Ricardo"
     assert len(lines) == 9
+
+
+def test_default_dump():
+    entries = [
+        {
+            "type_of_reference": "JOUR",
+            "authors": ["Shannon, Claude E.", "Doe, John"],
+            "year": "1948/07//",
+            "title": "A Mathematical Theory of Communication",
+            "start_page": "379",
+            "urls": ["https://example.com", "https://example2.com"],
+        }
+    ]
+
+    text_output = rispy.dumps(entries)
+    lines = text_output.splitlines()
+    assert lines[2] == "AU  - Shannon, Claude E."
+    assert lines[3] == "AU  - Doe, John"
+    assert lines[7] == "UR  - https://example.com"
+    assert lines[8] == "UR  - https://example2.com"
+    assert len(lines) == 10
+
+
+def test_delimited_dump():
+    entries = [
+        {
+            "type_of_reference": "JOUR",
+            "authors": ["Shannon, Claude E.", "Doe, John"],
+            "year": "1948/07//",
+            "title": "A Mathematical Theory of Communication",
+            "start_page": "379",
+            "urls": ["https://example.com", "https://example2.com"],
+        }
+    ]
+
+    # remove URLs from list_tags and give it a custom delimiter
+    text_output = rispy.dumps(entries, list_tags=["AU"], delimiter_tags_mapping={"UR": ","})
+
+    # check output is as expected
+    lines = text_output.splitlines()
+    assert lines[2] == "AU  - Shannon, Claude E."
+    assert lines[3] == "AU  - Doe, John"
+    assert lines[7] == "UR  - https://example.com,https://example2.com"
+    assert len(lines) == 9
```

### Comparing `rispy-0.8.0/PKG-INFO` & `rispy-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rispy
-Version: 0.8.0
+Version: 0.8.1
 Summary: A Python reader/writer of RIS reference files
 Keywords: RIS,parser,bibliograph
 Author-email: Maik Derstappen <md@derico.de>
 Maintainer-email: Andy Shapiro <shapiromatron@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
```

