# Comparing `tmp/pospell-1.1.tar.gz` & `tmp/pospell-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pospell-1.1.tar", last modified: Fri Nov 26 09:41:18 2021, max compression
+gzip compressed data, was "pospell-1.2.tar", last modified: Tue Jul 18 13:06:34 2023, max compression
```

## Comparing `pospell-1.1.tar` & `pospell-1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2021-11-26 09:41:18.849828 pospell-1.1/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2725 2021-11-26 09:41:18.849828 pospell-1.1/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2081 2021-10-27 17:10:33.000000 pospell-1.1/README.md
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2021-11-26 09:41:18.849828 pospell-1.1/pospell.egg-info/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2725 2021-11-26 09:41:18.000000 pospell-1.1/pospell.egg-info/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)      242 2021-11-26 09:41:18.000000 pospell-1.1/pospell.egg-info/SOURCES.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2021-11-26 09:41:18.000000 pospell-1.1/pospell.egg-info/dependency_links.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       42 2021-11-26 09:41:18.000000 pospell-1.1/pospell.egg-info/entry_points.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       33 2021-11-26 09:41:18.000000 pospell-1.1/pospell.egg-info/requires.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        8 2021-11-26 09:41:18.000000 pospell-1.1/pospell.egg-info/top_level.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)    15796 2021-11-26 09:36:05.000000 pospell-1.1/pospell.py
--rw-r--r--   0 mdk       (1000) mdk       (1000)       90 2021-04-09 22:07:43.000000 pospell-1.1/pyproject.toml
--rw-r--r--   0 mdk       (1000) mdk       (1000)      839 2021-11-26 09:41:18.849828 pospell-1.1/setup.cfg
--rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2020-11-23 11:50:50.000000 pospell-1.1/setup.py
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-18 13:06:34.722670 pospell-1.2/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2714 2023-07-18 13:06:34.722670 pospell-1.2/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2082 2023-04-10 13:30:19.000000 pospell-1.2/README.md
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-18 13:06:34.722670 pospell-1.2/pospell.egg-info/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2714 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      245 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/SOURCES.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/dependency_links.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       41 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/entry_points.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       27 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/requires.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        8 2023-07-18 13:06:34.000000 pospell-1.2/pospell.egg-info/top_level.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    15975 2023-07-18 13:04:11.000000 pospell-1.2/pospell.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1111 2023-07-18 12:38:53.000000 pospell-1.2/pyproject.toml
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-07-18 13:06:34.722670 pospell-1.2/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-18 13:06:34.722670 pospell-1.2/tests/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2617 2021-04-09 22:07:43.000000 pospell-1.2/tests/test_pospell.py
```

### Comparing `pospell-1.1/PKG-INFO` & `pospell-1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pospell
-Version: 1.1
+Version: 1.2
 Summary: Spellcheck .po files containing reStructuredText translations
-Home-page: https://github.com/AFPy/pospell
-Author: Julien Palard
-Author-email: julien@palard.fr
+Author-email: Julien Palard <julien@palard.fr>
 License: MIT license
+Project-URL: Homepage, https://git.afpy.org/AFPy/pospell
 Keywords: po,spell,gettext,reStructuredText,check,sphinx,translation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 
 # pospell
 
-`pospell` is a spellcheckers for po files containing reStructuedText.
+`pospell` is a spellcheckers for po files containing reStructuredText.
 
 
 ## Pospell is part of poutils!
 
 [Poutils](https://pypi.org/project/poutils) (`.po` utils) is a metapackage to easily install useful Python tools to use with po files
 and `pospell` is a part of it! Go check out [Poutils](https://pypi.org/project/poutils) to discover the other tools!
 
@@ -97,9 +95,7 @@
 
 And to test it locally:
 
 ```bash
 python -m pip install tox
 tox -p all
 ```
-
-
```

### Comparing `pospell-1.1/README.md` & `pospell-1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pospell
 
-`pospell` is a spellcheckers for po files containing reStructuedText.
+`pospell` is a spellcheckers for po files containing reStructuredText.
 
 
 ## Pospell is part of poutils!
 
 [Poutils](https://pypi.org/project/poutils) (`.po` utils) is a metapackage to easily install useful Python tools to use with po files
 and `pospell` is a part of it! Go check out [Poutils](https://pypi.org/project/poutils) to discover the other tools!
```

### Comparing `pospell-1.1/pospell.egg-info/PKG-INFO` & `pospell-1.2/pospell.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: pospell
-Version: 1.1
+Version: 1.2
 Summary: Spellcheck .po files containing reStructuredText translations
-Home-page: https://github.com/AFPy/pospell
-Author: Julien Palard
-Author-email: julien@palard.fr
+Author-email: Julien Palard <julien@palard.fr>
 License: MIT license
+Project-URL: Homepage, https://git.afpy.org/AFPy/pospell
 Keywords: po,spell,gettext,reStructuredText,check,sphinx,translation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 
 # pospell
 
-`pospell` is a spellcheckers for po files containing reStructuedText.
+`pospell` is a spellcheckers for po files containing reStructuredText.
 
 
 ## Pospell is part of poutils!
 
 [Poutils](https://pypi.org/project/poutils) (`.po` utils) is a metapackage to easily install useful Python tools to use with po files
 and `pospell` is a part of it! Go check out [Poutils](https://pypi.org/project/poutils) to discover the other tools!
 
@@ -97,9 +95,7 @@
 
 And to test it locally:
 
 ```bash
 python -m pip install tox
 tox -p all
 ```
-
-
```

### Comparing `pospell-1.1/pospell.py` & `pospell-1.2/pospell.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import docutils.parsers.rst
 import polib
 from docutils.parsers.rst import roles
 from docutils.utils import new_document
 
 import regex
 
-__version__ = "1.1"
+__version__ = "1.2"
 
 DEFAULT_DROP_CAPITALIZED = {"fr": True, "fr_FR": True}
 
 
 input_line = collections.namedtuple("input_line", "filename line text")
 
 
@@ -86,19 +86,22 @@
     to dictionaires).
     """
 
     IGNORE_LIST = (
         "emphasis",
         "superscript",
         "title_reference",
+        "substitution_reference",
+        "citation_reference",
         "strong",
         "DummyNodeClass",
         "reference",
         "literal",
         "Text",
+        "system_message",
     )
 
     def __init__(self, document):
         """Initialize visitor for the given node/document."""
         self.output = []
         super().__init__(document)
 
@@ -119,15 +122,15 @@
         """Skip childrens from the IGNORE_LIST."""
         if name.startswith("visit_") and name[6:] in self.IGNORE_LIST:
             return self.ignore
         raise AttributeError(name)
 
     def visit_Text(self, node):
         """Keep this node text, this is typically what we want to spell check."""
-        self.output.append(node.rawsource)
+        self.output.append(docutils.nodes.unescape(node, restore_backslashes=True))
 
     def __str__(self):
         """Give the accumulated strings."""
         return " ".join(self.output)
 
 
 def strip_rst(line):
@@ -225,14 +228,16 @@
     try:
         entries = polib.pofile(Path(po_path).read_text(encoding="UTF-8"))
     except Exception as err:
         raise POSpellException(str(err)) from err
     for entry in entries:
         if entry.msgid == entry.msgstr:
             continue
+        if entry.obsolete:
+            continue
         while lines < entry.linenum:
             lines += 1
             input_lines.append(input_line(po_path, lines, ""))
         lines += 1
         input_lines.append(
             input_line(
                 po_path,
```

