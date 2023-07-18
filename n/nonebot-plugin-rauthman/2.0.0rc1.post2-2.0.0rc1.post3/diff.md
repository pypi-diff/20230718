# Comparing `tmp/nonebot_plugin_rauthman-2.0.0rc1.post2.tar.gz` & `tmp/nonebot_plugin_rauthman-2.0.0rc1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rauthman-2.0.0rc1.post2.tar", max compression
+gzip compressed data, was "nonebot_plugin_rauthman-2.0.0rc1.post3.tar", max compression
```

## Comparing `nonebot_plugin_rauthman-2.0.0rc1.post2.tar` & `nonebot_plugin_rauthman-2.0.0rc1.post3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35823 2022-07-25 20:59:00.187265 nonebot_plugin_rauthman-2.0.0rc1.post2/LICENSE
--rw-r--r--   0        0        0       49 2023-07-17 12:50:48.313328 nonebot_plugin_rauthman-2.0.0rc1.post2/nonebot_plugin_rauthman/__init__.py
--rw-r--r--   0        0        0    33786 2023-07-17 12:50:48.129589 nonebot_plugin_rauthman-2.0.0rc1.post2/nonebot_plugin_rauthman/_FileStation.py
--rw-r--r--   0        0        0    21239 2023-07-17 12:50:47.898088 nonebot_plugin_rauthman-2.0.0rc1.post2/nonebot_plugin_rauthman/RAM.py
--rw-r--r--   0        0        0      694 2023-07-17 12:52:32.208830 nonebot_plugin_rauthman-2.0.0rc1.post2/pyproject.toml
--rw-r--r--   0        0        0     8032 2022-10-04 17:31:09.512480 nonebot_plugin_rauthman-2.0.0rc1.post2/README.rst
--rw-r--r--   0        0        0     8743 1970-01-01 00:00:00.000000 nonebot_plugin_rauthman-2.0.0rc1.post2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-07-25 20:59:00.187265 nonebot_plugin_rauthman-2.0.0rc1.post3/LICENSE
+-rw-r--r--   0        0        0       66 2023-07-18 01:25:14.411070 nonebot_plugin_rauthman-2.0.0rc1.post3/nonebot_plugin_rauthman/__init__.py
+-rw-r--r--   0        0        0    33786 2023-07-17 12:50:48.129589 nonebot_plugin_rauthman-2.0.0rc1.post3/nonebot_plugin_rauthman/_FileStation.py
+-rw-r--r--   0        0        0    21239 2023-07-18 01:24:53.251809 nonebot_plugin_rauthman-2.0.0rc1.post3/nonebot_plugin_rauthman/RAM.py
+-rw-r--r--   0        0        0      694 2023-07-18 01:25:26.180152 nonebot_plugin_rauthman-2.0.0rc1.post3/pyproject.toml
+-rw-r--r--   0        0        0     8032 2022-10-04 17:31:09.512480 nonebot_plugin_rauthman-2.0.0rc1.post3/README.rst
+-rw-r--r--   0        0        0     8743 1970-01-01 00:00:00.000000 nonebot_plugin_rauthman-2.0.0rc1.post3/PKG-INFO
```

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post2/LICENSE` & `nonebot_plugin_rauthman-2.0.0rc1.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post2/nonebot_plugin_rauthman/_FileStation.py` & `nonebot_plugin_rauthman-2.0.0rc1.post3/nonebot_plugin_rauthman/_FileStation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post2/nonebot_plugin_rauthman/RAM.py` & `nonebot_plugin_rauthman-2.0.0rc1.post3/nonebot_plugin_rauthman/RAM.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post2/pyproject.toml` & `nonebot_plugin_rauthman-2.0.0rc1.post3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_rauthman"
-version = "2.0.0rc1.post2"
+version = "2.0.0rc1.post3"
 description = "Rule-based authorization manager worked with nonebot2"
 authors = ["Lancercmd <lancercmd@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 repository = "https://github.com/Lancercmd/nonebot_plugin_rauthman"
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post2/README.rst` & `nonebot_plugin_rauthman-2.0.0rc1.post3/README.rst`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rauthman-2.0.0rc1.post2/PKG-INFO` & `nonebot_plugin_rauthman-2.0.0rc1.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rauthman
-Version: 2.0.0rc1.post2
+Version: 2.0.0rc1.post3
 Summary: Rule-based authorization manager worked with nonebot2
 Home-page: https://github.com/Lancercmd/nonebot_plugin_rauthman
 License: GPL-3.0-or-later
 Author: Lancercmd
 Author-email: lancercmd@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

