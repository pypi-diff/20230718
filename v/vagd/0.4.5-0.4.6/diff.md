# Comparing `tmp/vagd-0.4.5.tar.gz` & `tmp/vagd-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagd-0.4.5.tar", last modified: Sat Jul 15 07:45:53 2023, max compression
+gzip compressed data, was "vagd-0.4.6.tar", last modified: Tue Jul 18 13:01:54 2023, max compression
```

## Comparing `vagd-0.4.5.tar` & `vagd-0.4.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-15 07:45:53.357860 vagd-0.4.5/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.4.5/LICENSE
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4389 2023-07-15 07:45:53.357860 vagd-0.4.5/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3805 2023-06-17 16:19:04.000000 vagd-0.4.5/README.md
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-07-15 07:45:31.000000 vagd-0.4.5/pyproject.toml
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-07-15 07:45:53.357860 vagd-0.4.5/setup.cfg
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-15 07:45:53.351193 vagd-0.4.5/src/
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-15 07:45:53.354527 vagd-0.4.5/src/vagd/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.4.5/src/vagd/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.4.5/src/vagd/__main__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      939 2023-06-17 11:38:21.000000 vagd-0.4.5/src/vagd/box.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-15 07:45:53.357860 vagd-0.4.5/src/vagd/gdb/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.4.5/src/vagd/gdb/__init__.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.4.5/src/vagd/gdb/events.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.4.5/src/vagd/gdb/printing.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.4.5/src/vagd/gdb/prompt.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.4.5/src/vagd/gdb/types.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.4.5/src/vagd/gdb/unwinder.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.4.5/src/vagd/gdb/xmethod.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.4.5/src/vagd/gdb.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.4.5/src/vagd/helper.py
--rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      839 2023-06-17 11:43:56.000000 vagd-0.4.5/src/vagd/template.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1307 2023-07-15 07:29:51.000000 vagd-0.4.5/src/vagd/templates.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-15 07:45:53.357860 vagd-0.4.5/src/vagd/virts/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.4.5/src/vagd/virts/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5773 2023-07-15 07:37:43.000000 vagd-0.4.5/src/vagd/virts/dogd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10666 2023-06-17 15:51:31.000000 vagd-0.4.5/src/vagd/virts/pwngd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10849 2023-06-17 15:49:55.000000 vagd-0.4.5/src/vagd/virts/qegd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.4.5/src/vagd/virts/shgd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.4.5/src/vagd/virts/vagd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.4.5/src/vagd/wrapper.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-15 07:45:53.354527 vagd-0.4.5/src/vagd.egg-info/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4389 2023-07-15 07:45:53.000000 vagd-0.4.5/src/vagd.egg-info/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-07-15 07:45:53.000000 vagd-0.4.5/src/vagd.egg-info/SOURCES.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-07-15 07:45:53.000000 vagd-0.4.5/src/vagd.egg-info/dependency_links.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-07-15 07:45:53.000000 vagd-0.4.5/src/vagd.egg-info/requires.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-07-15 07:45:53.000000 vagd-0.4.5/src/vagd.egg-info/top_level.txt
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-15 07:45:53.357860 vagd-0.4.5/test/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1206 2023-06-17 15:43:05.000000 vagd-0.4.5/test/test.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-18 13:01:54.072378 vagd-0.4.6/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.4.6/LICENSE
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4389 2023-07-18 13:01:54.072378 vagd-0.4.6/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3805 2023-06-17 16:19:04.000000 vagd-0.4.6/README.md
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-07-18 13:01:09.000000 vagd-0.4.6/pyproject.toml
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-07-18 13:01:54.072378 vagd-0.4.6/setup.cfg
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-18 13:01:54.065711 vagd-0.4.6/src/
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-18 13:01:54.065711 vagd-0.4.6/src/vagd/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.4.6/src/vagd/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.4.6/src/vagd/__main__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      939 2023-06-17 11:38:21.000000 vagd-0.4.6/src/vagd/box.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-18 13:01:54.069044 vagd-0.4.6/src/vagd/gdb/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.4.6/src/vagd/gdb/__init__.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.4.6/src/vagd/gdb/events.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.4.6/src/vagd/gdb/printing.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.4.6/src/vagd/gdb/prompt.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.4.6/src/vagd/gdb/types.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.4.6/src/vagd/gdb/unwinder.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.4.6/src/vagd/gdb/xmethod.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.4.6/src/vagd/gdb.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.4.6/src/vagd/helper.py
+-rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)     1299 2023-07-18 13:00:12.000000 vagd-0.4.6/src/vagd/template.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1307 2023-07-15 07:29:51.000000 vagd-0.4.6/src/vagd/templates.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-18 13:01:54.072378 vagd-0.4.6/src/vagd/virts/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.4.6/src/vagd/virts/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5773 2023-07-15 07:37:43.000000 vagd-0.4.6/src/vagd/virts/dogd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10666 2023-06-17 15:51:31.000000 vagd-0.4.6/src/vagd/virts/pwngd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10849 2023-06-17 15:49:55.000000 vagd-0.4.6/src/vagd/virts/qegd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.4.6/src/vagd/virts/shgd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.4.6/src/vagd/virts/vagd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.4.6/src/vagd/wrapper.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-18 13:01:54.069044 vagd-0.4.6/src/vagd.egg-info/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4389 2023-07-18 13:01:54.000000 vagd-0.4.6/src/vagd.egg-info/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-07-18 13:01:54.000000 vagd-0.4.6/src/vagd.egg-info/SOURCES.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-07-18 13:01:54.000000 vagd-0.4.6/src/vagd.egg-info/dependency_links.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-07-18 13:01:54.000000 vagd-0.4.6/src/vagd.egg-info/requires.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-07-18 13:01:54.000000 vagd-0.4.6/src/vagd.egg-info/top_level.txt
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-07-18 13:01:54.072378 vagd-0.4.6/test/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1206 2023-06-17 15:43:05.000000 vagd-0.4.6/test/test.py
```

### Comparing `vagd-0.4.5/LICENSE` & `vagd-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/PKG-INFO` & `vagd-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 0.4.5
+Version: 0.4.6
 Summary: VirtuAlization GDb integrations in pwntools
 Author-email: 0x6fe1be2 <author@example.com>
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vagd-0.4.5/README.md` & `vagd-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/pyproject.toml` & `vagd-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vagd"
-version = "0.4.5"
+version = "0.4.6"
 authors = [
   { name="0x6fe1be2", email="author@example.com" },
 ]
 description = "VirtuAlization GDb integrations in pwntools"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ['pwntools', 'python-vagrant', 'docker']
```

### Comparing `vagd-0.4.5/src/vagd/box.py` & `vagd-0.4.6/src/vagd/box.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/gdb/__init__.pyi` & `vagd-0.4.6/src/vagd/gdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/gdb/events.pyi` & `vagd-0.4.6/src/vagd/gdb/events.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/gdb/printing.pyi` & `vagd-0.4.6/src/vagd/gdb/printing.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/gdb/types.pyi` & `vagd-0.4.6/src/vagd/gdb/types.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/gdb/xmethod.pyi` & `vagd-0.4.6/src/vagd/gdb/xmethod.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/helper.py` & `vagd-0.4.6/src/vagd/helper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/templates.py` & `vagd-0.4.6/src/vagd/templates.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/virts/dogd.py` & `vagd-0.4.6/src/vagd/virts/dogd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/virts/pwngd.py` & `vagd-0.4.6/src/vagd/virts/pwngd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/virts/qegd.py` & `vagd-0.4.6/src/vagd/virts/qegd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/virts/shgd.py` & `vagd-0.4.6/src/vagd/virts/shgd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/virts/vagd.py` & `vagd-0.4.6/src/vagd/virts/vagd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd/wrapper.py` & `vagd-0.4.6/src/vagd/wrapper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/src/vagd.egg-info/PKG-INFO` & `vagd-0.4.6/src/vagd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 0.4.5
+Version: 0.4.6
 Summary: VirtuAlization GDb integrations in pwntools
 Author-email: 0x6fe1be2 <author@example.com>
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vagd-0.4.5/src/vagd.egg-info/SOURCES.txt` & `vagd-0.4.6/src/vagd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vagd-0.4.5/test/test.py` & `vagd-0.4.6/test/test.py`

 * *Files identical despite different names*

