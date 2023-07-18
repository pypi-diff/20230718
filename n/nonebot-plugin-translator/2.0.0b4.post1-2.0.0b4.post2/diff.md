# Comparing `tmp/nonebot_plugin_translator-2.0.0b4.post1.tar.gz` & `tmp/nonebot_plugin_translator-2.0.0b4.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_translator-2.0.0b4.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_translator-2.0.0b4.post2.tar", max compression
```

## Comparing `nonebot_plugin_translator-2.0.0b4.post1.tar` & `nonebot_plugin_translator-2.0.0b4.post2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35823 2022-12-25 18:39:12.996734 nonebot_plugin_translator-2.0.0b4.post1/LICENSE
--rw-r--r--   0        0        0       26 2023-07-17 12:59:32.105124 nonebot_plugin_translator-2.0.0b4.post1/nonebot_plugin_translator/__init__.py
--rw-r--r--   0        0        0    17871 2023-07-17 12:59:31.916261 nonebot_plugin_translator-2.0.0b4.post1/nonebot_plugin_translator/translator.py
--rw-r--r--   0        0        0      667 2023-07-17 12:59:38.355808 nonebot_plugin_translator-2.0.0b4.post1/pyproject.toml
--rw-r--r--   0        0        0     3795 2023-01-23 04:52:26.786650 nonebot_plugin_translator-2.0.0b4.post1/README.rst
--rw-r--r--   0        0        0     4614 1970-01-01 00:00:00.000000 nonebot_plugin_translator-2.0.0b4.post1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-12-25 18:39:12.996734 nonebot_plugin_translator-2.0.0b4.post2/LICENSE
+-rw-r--r--   0        0        0       67 2023-07-18 01:27:21.913442 nonebot_plugin_translator-2.0.0b4.post2/nonebot_plugin_translator/__init__.py
+-rw-r--r--   0        0        0    17871 2023-07-17 12:59:31.916261 nonebot_plugin_translator-2.0.0b4.post2/nonebot_plugin_translator/translator.py
+-rw-r--r--   0        0        0      667 2023-07-18 01:27:30.739020 nonebot_plugin_translator-2.0.0b4.post2/pyproject.toml
+-rw-r--r--   0        0        0     3795 2023-01-23 04:52:26.786650 nonebot_plugin_translator-2.0.0b4.post2/README.rst
+-rw-r--r--   0        0        0     4614 1970-01-01 00:00:00.000000 nonebot_plugin_translator-2.0.0b4.post2/PKG-INFO
```

### Comparing `nonebot_plugin_translator-2.0.0b4.post1/LICENSE` & `nonebot_plugin_translator-2.0.0b4.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_translator-2.0.0b4.post1/nonebot_plugin_translator/translator.py` & `nonebot_plugin_translator-2.0.0b4.post2/nonebot_plugin_translator/translator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_translator-2.0.0b4.post1/pyproject.toml` & `nonebot_plugin_translator-2.0.0b4.post2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_translator"
-version = "2.0.0b4.post1"
+version = "2.0.0b4.post2"
 description = "Multi language tanslator worked with nonebot2"
 authors = ["Lancercmd <lancercmd@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 repository = "https://github.com/Lancercmd/nonebot_plugin_translator"
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_translator-2.0.0b4.post1/README.rst` & `nonebot_plugin_translator-2.0.0b4.post2/README.rst`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_translator-2.0.0b4.post1/PKG-INFO` & `nonebot_plugin_translator-2.0.0b4.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-translator
-Version: 2.0.0b4.post1
+Version: 2.0.0b4.post2
 Summary: Multi language tanslator worked with nonebot2
 Home-page: https://github.com/Lancercmd/nonebot_plugin_translator
 License: GPL-3.0-or-later
 Author: Lancercmd
 Author-email: lancercmd@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

