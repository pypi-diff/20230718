# Comparing `tmp/acquire-3.8.dev3.tar.gz` & `tmp/acquire-3.8.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.8.dev3.tar", last modified: Tue Jul 18 08:15:16 2023, max compression
+gzip compressed data, was "acquire-3.8.dev4.tar", last modified: Tue Jul 18 11:34:38 2023, max compression
```

## Comparing `acquire-3.8.dev3.tar` & `acquire-3.8.dev4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.754882 acquire-3.8.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-18 08:15:00.000000 acquire-3.8.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-18 08:15:00.000000 acquire-3.8.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 08:15:00.000000 acquire-3.8.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-18 08:15:16.754882 acquire-3.8.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-18 08:15:00.000000 acquire-3.8.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.734882 acquire-3.8.dev3/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77538 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.734882 acquire-3.8.dev3/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.742882 acquire-3.8.dev3/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.742882 acquire-3.8.dev3/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.742882 acquire-3.8.dev3/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.746882 acquire-3.8.dev3/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.734882 acquire-3.8.dev3/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-18 08:15:05.000000 acquire-3.8.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:15:16.754882 acquire-3.8.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.754882 acquire-3.8.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.754882 acquire-3.8.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_acquire_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_decryptor_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:38.131793 acquire-3.8.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-18 11:34:23.000000 acquire-3.8.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-18 11:34:23.000000 acquire-3.8.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 11:34:23.000000 acquire-3.8.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-18 11:34:38.131793 acquire-3.8.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-18 11:34:23.000000 acquire-3.8.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:38.123793 acquire-3.8.dev4/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78826 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:38.127793 acquire-3.8.dev4/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:38.127793 acquire-3.8.dev4/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:38.127793 acquire-3.8.dev4/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:38.127793 acquire-3.8.dev4/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:38.131793 acquire-3.8.dev4/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-18 11:34:23.000000 acquire-3.8.dev4/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-18 11:34:38.000000 acquire-3.8.dev4/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:38.127793 acquire-3.8.dev4/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-18 11:34:38.000000 acquire-3.8.dev4/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-18 11:34:38.000000 acquire-3.8.dev4/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:34:38.000000 acquire-3.8.dev4/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 11:34:38.000000 acquire-3.8.dev4/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-18 11:34:38.000000 acquire-3.8.dev4/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 11:34:38.000000 acquire-3.8.dev4/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-18 11:34:28.000000 acquire-3.8.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:34:38.131793 acquire-3.8.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:38.131793 acquire-3.8.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:38.131793 acquire-3.8.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/test_acquire_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/test_decryptor_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-18 11:34:23.000000 acquire-3.8.dev4/tox.ini
```

### Comparing `acquire-3.8.dev3/LICENSE` & `acquire-3.8.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/PKG-INFO` & `acquire-3.8.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.8.dev3
+Version: 3.8.dev4
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.8.dev3/README.md` & `acquire-3.8.dev4/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/acquire.py` & `acquire-3.8.dev4/acquire/acquire.py`

 * *Files 1% similar despite different names*

```diff
@@ -1326,30 +1326,62 @@
         ("glob", "/boot/init*"),
     ]
 
 
 @register_module("--home")
 class Home(Module):
     SPEC = [
+        # TODO: Use from_user_home if supported for osx
         ("glob", "/root/.*[akz]sh*"),
         ("dir", "/root/.config"),
         ("glob", "/home/*/.*[akz]sh*"),
         ("glob", "/home/*/.config"),
         ("glob", "/home/*/*/.*[akz]sh*"),
         ("glob", "/home/*/*/.config"),
         # OS-X home (aka /Users)
         ("glob", "/Users/*/.*[akz]sh*"),
+        ("glob", "/Users/*/.config"),
         ("glob", "/Users/*/.bash_sessions/*"),
         ("glob", "/Users/*/Library/LaunchAgents/*"),
         ("glob", "/Users/*/Library/Logs/*"),
         ("glob", "/Users/*/Preferences/*"),
         ("glob", "/Users/*/Library/Preferences/*"),
     ]
 
 
+@register_module("--ssh")
+class SSH(Module):
+    @classmethod
+    def _run(cls, target: Target, collector):
+        user_pattern = ".ssh/*"
+
+        # Gather user paths
+        # TODO: Use from_user_home if supported for osx
+        if target._os.os == "osx":
+            iterator = [f"/Users/*/{user_pattern}"]
+        else:
+            iterator = list(from_user_home(target, user_pattern))
+
+        # Acquire SSH configuration in sshd directories
+        iterator += ["/etc/ssh/*", "sysvol/ProgramData/ssh/*"]
+
+        globbed_path = (path for pattern in iterator for path in target.fs.glob(pattern))
+        for path in globbed_path:
+            if target.fs.path(path).is_dir():
+                collector.collect_dir(path)
+                continue
+
+            with target.fs.path(path).open("rt") as file:
+                if "PRIVATE KEY" in file.readline():
+                    # Detected a private key, skipping.
+                    continue
+
+            collector.collect_file(path, outpath=path)
+
+
 @register_module("--var")
 class Var(Module):
     SPEC = [
         # In OS-X /var is a symlink to /private/var. To prevent collecting
         # duplicates, we only use the /var directory here.
         ("dir", "/var/log"),
         ("dir", "/var/spool/at"),
@@ -1915,40 +1947,45 @@
             DNS,
             History,
             Misc,
             NTDS,
             QuarantinedFiles,
             RemoteAccess,
             WindowsNotifications,
+            SSH,
         ],
         "linux": [
             Etc,
             Boot,
             Home,
             History,
+            SSH,
             Var,
         ],
         "bsd": [
             Etc,
             Boot,
+            SSH,
             Home,
             Var,
             BSD,
         ],
         "esxi": [
             Bootbanks,
             ESXi,
             VMFS,
+            SSH,
         ],
         "osx": [
             Etc,
             Home,
             Var,
             OSX,
             History,
+            SSH,
         ],
     },
     "default": {
         "windows": [
             NTFS,
             EventLogs,
             Registry,
@@ -1971,27 +2008,30 @@
             RemoteAccess,
             ActivitiesCache,
         ],
         "linux": [
             Etc,
             Boot,
             Home,
+            SSH,
             Var,
         ],
         "bsd": [
             Etc,
             Boot,
             Home,
+            SSH,
             Var,
             BSD,
         ],
         "esxi": [
             Bootbanks,
             ESXi,
             VMFS,
+            SSH,
         ],
         "osx": [
             Etc,
             Home,
             Var,
             OSX,
         ],
@@ -2008,26 +2048,29 @@
             PCA,
             Misc,
         ],
         "linux": [
             Etc,
             Boot,
             Home,
+            SSH,
             Var,
         ],
         "bsd": [
             Etc,
             Boot,
             Home,
+            SSH,
             Var,
             BSD,
         ],
         "esxi": [
             Bootbanks,
             ESXi,
+            SSH,
         ],
         "osx": [
             Etc,
             Home,
             Var,
             OSX,
         ],
```

### Comparing `acquire-3.8.dev3/acquire/collector.py` & `acquire-3.8.dev4/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/crypt.py` & `acquire-3.8.dev4/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/dynamic/windows/collect.py` & `acquire-3.8.dev4/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/dynamic/windows/handles.py` & `acquire-3.8.dev4/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/dynamic/windows/named_objects.py` & `acquire-3.8.dev4/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/dynamic/windows/ntdll.py` & `acquire-3.8.dev4/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/dynamic/windows/types.py` & `acquire-3.8.dev4/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/esxi.py` & `acquire-3.8.dev4/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/hashes.py` & `acquire-3.8.dev4/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/log.py` & `acquire-3.8.dev4/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/outputs/base.py` & `acquire-3.8.dev4/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/outputs/dir.py` & `acquire-3.8.dev4/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/outputs/tar.py` & `acquire-3.8.dev4/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/tools/decrypter.py` & `acquire-3.8.dev4/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/uploaders/minio.py` & `acquire-3.8.dev4/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/uploaders/plugin.py` & `acquire-3.8.dev4/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/uploaders/plugin_registry.py` & `acquire-3.8.dev4/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire/utils.py` & `acquire-3.8.dev4/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/acquire.egg-info/PKG-INFO` & `acquire-3.8.dev4/acquire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.8.dev3
+Version: 3.8.dev4
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.8.dev3/acquire.egg-info/SOURCES.txt` & `acquire-3.8.dev4/acquire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/pyproject.toml` & `acquire-3.8.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/conftest.py` & `acquire-3.8.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/docs/Makefile` & `acquire-3.8.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/docs/conf.py` & `acquire-3.8.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/test_acquire_command.py` & `acquire-3.8.dev4/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/test_acquire_modules.py` & `acquire-3.8.dev4/tests/test_acquire_modules.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/test_collector.py` & `acquire-3.8.dev4/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/test_decryptor_funcs.py` & `acquire-3.8.dev4/tests/test_decryptor_funcs.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/test_esxi_memory.py` & `acquire-3.8.dev4/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/test_file_sorting.py` & `acquire-3.8.dev4/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/test_minio_uploader.py` & `acquire-3.8.dev4/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/test_plugin.py` & `acquire-3.8.dev4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tests/test_utils.py` & `acquire-3.8.dev4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev3/tox.ini` & `acquire-3.8.dev4/tox.ini`

 * *Files identical despite different names*

