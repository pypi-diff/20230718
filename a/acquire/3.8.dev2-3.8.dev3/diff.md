# Comparing `tmp/acquire-3.8.dev2.tar.gz` & `tmp/acquire-3.8.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.8.dev2.tar", last modified: Tue Jul 11 09:12:26 2023, max compression
+gzip compressed data, was "acquire-3.8.dev3.tar", last modified: Tue Jul 18 08:15:16 2023, max compression
```

## Comparing `acquire-3.8.dev2.tar` & `acquire-3.8.dev3.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.480426 acquire-3.8.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 09:12:04.000000 acquire-3.8.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-11 09:12:04.000000 acquire-3.8.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 09:12:04.000000 acquire-3.8.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-11 09:12:26.480426 acquire-3.8.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-11 09:12:04.000000 acquire-3.8.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.456426 acquire-3.8.dev2/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77540 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.460426 acquire-3.8.dev2/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.464426 acquire-3.8.dev2/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.468426 acquire-3.8.dev2/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.468426 acquire-3.8.dev2/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.472426 acquire-3.8.dev2/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-11 09:12:04.000000 acquire-3.8.dev2/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.460426 acquire-3.8.dev2/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 09:12:26.000000 acquire-3.8.dev2/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-11 09:12:13.000000 acquire-3.8.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:12:26.480426 acquire-3.8.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.476426 acquire-3.8.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:12:26.480426 acquire-3.8.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_decryptor_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-11 09:12:04.000000 acquire-3.8.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.754882 acquire-3.8.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-18 08:15:00.000000 acquire-3.8.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-18 08:15:00.000000 acquire-3.8.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 08:15:00.000000 acquire-3.8.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-18 08:15:16.754882 acquire-3.8.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-18 08:15:00.000000 acquire-3.8.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.734882 acquire-3.8.dev3/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77538 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.734882 acquire-3.8.dev3/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.742882 acquire-3.8.dev3/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.742882 acquire-3.8.dev3/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.742882 acquire-3.8.dev3/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.746882 acquire-3.8.dev3/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-18 08:15:00.000000 acquire-3.8.dev3/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.734882 acquire-3.8.dev3/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 08:15:16.000000 acquire-3.8.dev3/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-18 08:15:05.000000 acquire-3.8.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:15:16.754882 acquire-3.8.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.754882 acquire-3.8.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:15:16.754882 acquire-3.8.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_acquire_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_decryptor_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-18 08:15:00.000000 acquire-3.8.dev3/tox.ini
```

### Comparing `acquire-3.8.dev2/LICENSE` & `acquire-3.8.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/PKG-INFO` & `acquire-3.8.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.8.dev2
+Version: 3.8.dev3
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.8.dev2/README.md` & `acquire-3.8.dev3/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/acquire.py` & `acquire-3.8.dev3/acquire/acquire.py`

 * *Files 0% similar despite different names*

```diff
@@ -864,38 +864,38 @@
         # ESET
         ("dir", "sysvol/Documents and Settings/All Users/Application Data/ESET/ESET NOD32 Antivirus/Logs"),
         ("dir", "sysvol/ProgramData/ESET/ESET NOD32 Antivirus/Logs"),
         # Emsisoft
         ("glob", "sysvol/ProgramData/Emsisoft/Reports/scan*.txt"),
         # F-Secure
         ("dir", "sysvol/ProgramData/F-Secure/Log"),
-        ("dir", "sysvol/Users*/AppData/Local/F-Secure/Log"),
+        ("dir", "AppData/Local/F-Secure/Log", from_user_home),
         ("dir", "sysvol/ProgramData/F-Secure/Antivirus/ScheduledScanReports"),
         # HitmanPro
         ("dir", "sysvol/ProgramData/HitmanPro/Logs"),
         ("dir", "sysvol/ProgramData/HitmanPro.Alert/Logs"),
         ("file", "sysvol/ProgramData/HitmanPro.Alert/excalibur.db"),
-        ("glob", "sysvol/ProgramData/HitmanPro/Quarantine"),
+        ("dir", "sysvol/ProgramData/HitmanPro/Quarantine"),
         # Malwarebytes
         ("glob", "sysvol/ProgramData/Malwarebytes/Malwarebytes Anti-Malware/Logs/mbam-log-*.xml"),
         ("glob", "sysvol/ProgramData/Malwarebytes/MBAMService/logs/mbamservice.log*"),
-        ("dir", "sysvol/Users*/AppData/Roaming/Malwarebytes/Malwarebytes Anti-Malware/Logs"),
+        ("dir", "AppData/Roaming/Malwarebytes/Malwarebytes Anti-Malware/Logs", from_user_home),
         ("dir", "sysvol/ProgramData/Malwarebytes/MBAMService/ScanResults"),
         # McAfee
-        ("dir", "sysvol/Users/All Users/Application Data/McAfee/DesktopProtection"),
+        ("dir", "Application Data/McAfee/DesktopProtection", from_user_home),
         ("dir", "sysvol/ProgramData/McAfee/DesktopProtection"),
         ("dir", "sysvol/ProgramData/McAfee/Endpoint Security/Logs"),
         ("dir", "sysvol/ProgramData/McAfee/Endpoint Security/Logs_Old"),
         ("dir", "sysvol/ProgramData/Mcafee/VirusScan"),
         ("dir", "sysvol/ProgramData/McAfee/Endpoint Security/Logs"),
         ("dir", "sysvol/ProgramData/McAfee/MSC/Logs"),
         # RogueKiller
         ("glob", "sysvol/ProgramData/RogueKiller/logs/AdliceReport_*.json"),
         # SUPERAntiSpyware
-        ("dir", "sysvol/Users*/AppData/Roaming/SUPERAntiSpyware/Logs"),
+        ("dir", "AppData/Roaming/SUPERAntiSpyware/Logs", from_user_home),
         # SecureAge
         ("dir", "sysvol/ProgramData/SecureAge Technology/SecureAge/log"),
         # SentinelOne
         ("dir", "sysvol/programdata/sentinel/logs"),
         # Sophos
         ("glob", "sysvol/Documents and Settings/All Users/Application Data/Sophos/Sophos */Logs"),
         ("glob", "sysvol/ProgramData/Sophos/Sophos */Logs"),
@@ -968,25 +968,25 @@
         ("file", "Local Settings/History/History.IE5/index.dat", from_user_home),
         ("glob", "Local Settings/History/History.IE5/MSHist*/index.dat", from_user_home),
         ("file", "Local Settings/Temporary Internet Files/Content.IE5/index.dat", from_user_home),
         ("file", "Local Settings/Application Data/Microsoft/Feeds Cache/index.dat", from_user_home),
         ("dir", "AppData/Local/Microsoft/Internet Explorer/Recovery", from_user_home),
         ("file", "AppData/Local/Microsoft/Windows/History/History.IE5/index.dat", from_user_home),
         (
-            "file",
+            "glob",
             "AppData/Local/Microsoft/Windows/History/History.IE5/MSHist*/index.dat",
             from_user_home,
         ),
         (
             "file",
             "AppData/Local/Microsoft/Windows/History/Low/History.IE5/index.dat",
             from_user_home,
         ),
         (
-            "file",
+            "glob",
             "AppData/Local/Microsoft/Windows/History/Low/History.IE5/MSHist*/index.dat",
             from_user_home,
         ),
         ("dir", "AppData/Local/Microsoft/Windows/INetCookies", from_user_home),
         (
             "file",
             "AppData/Local/Microsoft/Windows/Temporary Internet Files/Content.IE5/index.dat",
```

### Comparing `acquire-3.8.dev2/acquire/collector.py` & `acquire-3.8.dev3/acquire/collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,14 @@
     def add_file_failed(self, module: str, failed_path: Path) -> None:
         exc = get_formatted_exception()
         self._register(module, Outcome.FAILURE, ArtifactType.FILE, failed_path, exc)
 
     def add_file_missing(self, module: str, missing_path: Path) -> None:
         self._register(module, Outcome.MISSING, ArtifactType.FILE, missing_path)
 
-    def add_glob_collected(self, module: str, pattern: str) -> None:
-        self._register(module, Outcome.SUCCESS, ArtifactType.GLOB, pattern)
-
     def add_glob_failed(self, module: str, failed_pattern: str) -> None:
         exc = get_formatted_exception()
         self._register(module, Outcome.FAILURE, ArtifactType.GLOB, failed_pattern, exc)
 
     def add_glob_empty(self, module: str, pattern: str) -> None:
         self._register(module, Outcome.EMPTY, ArtifactType.GLOB, pattern)
 
@@ -363,15 +360,15 @@
         except Exception:
             log.error("- Failed to collect glob %s", pattern, exc_info=True)
             self.report.add_glob_failed(module_name, pattern)
         else:
             if glob_is_empty:
                 self.report.add_glob_empty(module_name, pattern)
             else:
-                self.report.add_glob_collected(module_name, pattern)
+                log.info("- Collecting glob %s succeeded", pattern)
 
     def collect_path(
         self,
         path: Union[str, fsutil.TargetPath],
         seen_paths: Optional[set] = None,
         module_name: Optional[str] = None,
         follow: bool = True,
```

### Comparing `acquire-3.8.dev2/acquire/crypt.py` & `acquire-3.8.dev3/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/dynamic/windows/collect.py` & `acquire-3.8.dev3/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/dynamic/windows/handles.py` & `acquire-3.8.dev3/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/dynamic/windows/named_objects.py` & `acquire-3.8.dev3/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/dynamic/windows/ntdll.py` & `acquire-3.8.dev3/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/dynamic/windows/types.py` & `acquire-3.8.dev3/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/esxi.py` & `acquire-3.8.dev3/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/hashes.py` & `acquire-3.8.dev3/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/log.py` & `acquire-3.8.dev3/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/outputs/base.py` & `acquire-3.8.dev3/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/outputs/dir.py` & `acquire-3.8.dev3/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/outputs/tar.py` & `acquire-3.8.dev3/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/tools/decrypter.py` & `acquire-3.8.dev3/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/uploaders/minio.py` & `acquire-3.8.dev3/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/uploaders/plugin.py` & `acquire-3.8.dev3/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/uploaders/plugin_registry.py` & `acquire-3.8.dev3/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire/utils.py` & `acquire-3.8.dev3/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/acquire.egg-info/PKG-INFO` & `acquire-3.8.dev3/acquire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.8.dev2
+Version: 3.8.dev3
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.8.dev2/acquire.egg-info/SOURCES.txt` & `acquire-3.8.dev3/acquire.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 acquire/uploaders/__init__.py
 acquire/uploaders/minio.py
 acquire/uploaders/plugin.py
 acquire/uploaders/plugin_registry.py
 tests/__init__.py
 tests/conftest.py
 tests/test_acquire_command.py
+tests/test_acquire_modules.py
 tests/test_collector.py
 tests/test_decryptor_funcs.py
 tests/test_esxi_memory.py
 tests/test_file_sorting.py
 tests/test_minio_uploader.py
 tests/test_plugin.py
 tests/test_utils.py
```

### Comparing `acquire-3.8.dev2/pyproject.toml` & `acquire-3.8.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tests/conftest.py` & `acquire-3.8.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tests/docs/Makefile` & `acquire-3.8.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tests/docs/conf.py` & `acquire-3.8.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tests/test_acquire_command.py` & `acquire-3.8.dev3/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tests/test_collector.py` & `acquire-3.8.dev3/tests/test_collector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import errno
-from unittest.mock import Mock, patch
+from pathlib import Path
+from unittest.mock import MagicMock, Mock, patch
 
 import pytest
 from dissect.target import Target
 from dissect.target.exceptions import (
     FileNotFoundError,
     NotADirectoryError,
     NotASymlinkError,
     SymlinkRecursionError,
 )
 from dissect.target.filesystem import VirtualFilesystem
 
-from acquire.collector import Collector
+from acquire.collector import CollectionReport, Collector, Outcome
 
 
 def test_collector() -> None:
     target = Target("local")
 
     with patch("acquire.collector.log", autospec=True) as mock_log:
         fs_1 = VirtualFilesystem()
@@ -42,74 +43,76 @@
     return collector
 
 
 MOCK_SEEN_PATHS = set()
 MOCK_MODULE_NAME = "DUMMY"
 
 
-def test_collector_collect_path_no_module_name(mock_collector) -> None:
+def test_collector_collect_path_no_module_name(mock_collector: Collector) -> None:
     with pytest.raises(ValueError):
         mock_collector.collect_path("/some/path")
 
 
-def test_collector_collect_path_dir_as_target_path(mock_target, mock_collector) -> None:
+def test_collector_collect_path_dir_as_target_path(mock_target: Target, mock_collector: Collector) -> None:
     with patch.object(mock_collector, "collect_dir", autospec=True):
         path = mock_target.fs.path("/foo/bar")
         mock_collector.collect_path(
             path,
             seen_paths=MOCK_SEEN_PATHS,
             module_name=MOCK_MODULE_NAME,
         )
         mock_collector.collect_dir.assert_called()
 
 
-def test_collector_collect_path_dir(mock_collector) -> None:
+def test_collector_collect_path_dir(mock_collector: Collector) -> None:
     with patch.object(mock_collector, "collect_dir", autospec=True):
         mock_collector.collect_path(
             "/foo/bar",
             seen_paths=MOCK_SEEN_PATHS,
             module_name=MOCK_MODULE_NAME,
         )
         mock_collector.collect_dir.assert_called()
 
 
-def test_collector_collect_path_file(mock_collector) -> None:
+def test_collector_collect_path_file(mock_collector: Collector) -> None:
     with patch.object(mock_collector, "collect_file", autospec=True):
         mock_collector.collect_path(
             "/foo/bar/some-file",
             seen_paths=MOCK_SEEN_PATHS,
             module_name=MOCK_MODULE_NAME,
         )
         mock_collector.collect_file.assert_called()
 
 
-def test_collector_collect_path_symlink(mock_collector) -> None:
-    with patch.object(mock_collector, "collect_symlink", autospec=True):
-        with patch.object(mock_collector, "collect_file", autospec=True):
-            mock_collector.collect_path(
-                "/foo/bar/some-symlink",
-                follow=False,
-                seen_paths=MOCK_SEEN_PATHS,
-                module_name=MOCK_MODULE_NAME,
-            )
-            mock_collector.collect_symlink.assert_called()
-            mock_collector.collect_file.assert_not_called()
+def test_collector_collect_path_symlink(mock_collector: Collector) -> None:
+    with patch.object(mock_collector, "collect_symlink", autospec=True), patch.object(
+        mock_collector, "collect_file", autospec=True
+    ):
+        mock_collector.collect_path(
+            "/foo/bar/some-symlink",
+            follow=False,
+            seen_paths=MOCK_SEEN_PATHS,
+            module_name=MOCK_MODULE_NAME,
+        )
+        mock_collector.collect_symlink.assert_called()
+        mock_collector.collect_file.assert_not_called()
 
 
-def test_collector_collect_path_symlink_follow(mock_collector) -> None:
-    with patch.object(mock_collector, "collect_symlink", autospec=True):
-        with patch.object(mock_collector, "collect_file", autospec=True):
-            mock_collector.collect_path(
-                "/foo/bar/some-symlink",
-                follow=True,
-                seen_paths=MOCK_SEEN_PATHS,
-                module_name=MOCK_MODULE_NAME,
-            )
-            mock_collector.collect_symlink.assert_called()
-            mock_collector.collect_file.assert_called()
+def test_collector_collect_path_symlink_follow(mock_collector: Collector) -> None:
+    with patch.object(mock_collector, "collect_symlink", autospec=True), patch.object(
+        mock_collector, "collect_file", autospec=True
+    ):
+        mock_collector.collect_path(
+            "/foo/bar/some-symlink",
+            follow=True,
+            seen_paths=MOCK_SEEN_PATHS,
+            module_name=MOCK_MODULE_NAME,
+        )
+        mock_collector.collect_symlink.assert_called()
+        mock_collector.collect_file.assert_called()
 
 
 @pytest.mark.parametrize(
     "path, symlink_called, file_called",
     [
         (
             "/foo/bar/own-file",
@@ -129,74 +132,87 @@
         (
             "/foo/bar/some-symlink",
             True,
             True,
         ),
     ],
 )
-def test_collector_collect_path_skip_list(mock_collector, path, symlink_called, file_called) -> None:
-    with patch.object(mock_collector, "skip_list", new={"/foo/bar/own-file"}):
-        with patch.object(mock_collector, "collect_symlink", autospec=True):
-            with patch.object(mock_collector, "collect_file", autospec=True):
-                mock_collector.collect_path(
-                    path,
-                    follow=True,
-                    seen_paths=MOCK_SEEN_PATHS,
-                    module_name=MOCK_MODULE_NAME,
-                )
-                if symlink_called:
-                    mock_collector.collect_symlink.assert_called()
-                else:
-                    mock_collector.collect_symlink.assert_not_called()
-
-                if file_called:
-                    mock_collector.collect_file.assert_called()
-                else:
-                    mock_collector.collect_file.assert_not_called()
+def test_collector_collect_path_skip_list(
+    mock_collector: Collector, path: str, symlink_called: bool, file_called: bool
+) -> None:
+    with (
+        patch.object(mock_collector, "skip_list", new={"/foo/bar/own-file"}),
+        patch.object(mock_collector, "collect_symlink", autospec=True),
+        patch.object(mock_collector, "collect_file", autospec=True),
+    ):
+        mock_collector.collect_path(
+            path,
+            follow=True,
+            seen_paths=MOCK_SEEN_PATHS,
+            module_name=MOCK_MODULE_NAME,
+        )
+        if symlink_called:
+            mock_collector.collect_symlink.assert_called()
+        else:
+            mock_collector.collect_symlink.assert_not_called()
 
+        if file_called:
+            mock_collector.collect_file.assert_called()
+        else:
+            mock_collector.collect_file.assert_not_called()
 
-def test_collector_collect_glob(mock_collector) -> None:
-    with patch.object(mock_collector, "collect_file", autospec=True):
+
+def test_collector_collect_glob(mock_collector: Collector) -> None:
+    with patch.object(mock_collector, "collect_file", autospec=True), patch.object(
+        mock_collector, "report", autospec=True
+    ):
         mock_collector.collect_glob(
             "/foo/bar/*",
             module_name=MOCK_MODULE_NAME,
         )
         assert len(mock_collector.collect_file.mock_calls) == 3
         assert mock_collector.collect_file.call_args.kwargs.get("module_name", None) == MOCK_MODULE_NAME
 
 
-def test_collector_collect_path_non_existing_file(mock_collector) -> None:
-    with patch("acquire.collector.log", autospec=True) as mock_log:
-        with patch.object(mock_collector, "report", autospec=True) as mock_report:
-            mock_collector.collect_path(
-                "/foo/bar/non-existing-file",
-                seen_paths=MOCK_SEEN_PATHS,
-                module_name=MOCK_MODULE_NAME,
-            )
-            mock_report.add_path_missing.assert_called()
-            mock_log.error.assert_called()
-            assert mock_log.error.call_args.args[0] == "- Path %s is not found"
+def test_collector_collect_path_non_existing_file(mock_collector: Collector) -> None:
+    with (
+        patch("acquire.collector.log", autospec=True) as mock_log,
+        patch.object(mock_collector, "report", autospec=True) as mock_report,
+    ):
+        mock_collector.collect_path(
+            "/foo/bar/non-existing-file",
+            seen_paths=MOCK_SEEN_PATHS,
+            module_name=MOCK_MODULE_NAME,
+        )
+        mock_report.add_path_missing.assert_called()
+        mock_log.error.assert_called()
+        assert mock_log.error.call_args.args[0] == "- Path %s is not found"
 
 
-def test_collector_collect_path_no_file_type(mock_target, mock_collector) -> None:
+def test_collector_collect_path_no_file_type(mock_target: Target, mock_collector: Collector) -> None:
     path = mock_target.fs.path("/foo/bar/non-existing-file")
-    with patch("acquire.collector.log", autospec=True) as mock_log:
-        with patch.object(mock_collector, "report", autospec=True) as mock_report:
-            with patch.object(path, "get", return_value=True, autospec=True):
-                with patch.object(path, "is_dir", return_value=False, autospec=True):
-                    with patch.object(path, "is_file", return_value=False, autospec=True):
-                        with patch.object(path, "is_symlink", return_value=False, autospec=True):
-                            mock_collector.collect_path(
-                                path,
-                                seen_paths=MOCK_SEEN_PATHS,
-                                module_name=MOCK_MODULE_NAME,
-                            )
-                            mock_report.add_path_failed.assert_called()
-                            mock_log.error.assert_called()
-                            assert mock_log.error.call_args.args[0] == "- Don't know how to collect %s in module %s"
+    with (
+        patch("acquire.collector.log", autospec=True) as mock_log,
+        patch.object(mock_collector, "report", autospec=True) as mock_report,
+        patch.multiple(
+            path,
+            get=MagicMock(return_value=True),
+            is_dir=MagicMock(return_value=False),
+            is_file=MagicMock(return_value=False),
+            is_symlink=MagicMock(return_value=False),
+        ),
+    ):
+        mock_collector.collect_path(
+            path,
+            seen_paths=MOCK_SEEN_PATHS,
+            module_name=MOCK_MODULE_NAME,
+        )
+        mock_report.add_path_failed.assert_called()
+        mock_log.error.assert_called()
+        assert mock_log.error.call_args.args[0] == "- Don't know how to collect %s in module %s"
 
 
 @pytest.mark.parametrize(
     "report_func, exception, log_msg",
     [
         (
             "add_path_missing",
@@ -243,19 +259,87 @@
             Exception,
             "- Failed to collect path %s",
         ),
     ],
 )
 def test_collector_collect_path_with_exception(mock_target, mock_collector, report_func, exception, log_msg) -> None:
     path = mock_target.fs.path("/foo/bar/non-existing-file")
-    with patch("acquire.collector.log", autospec=True) as mock_log:
-        with patch.object(mock_collector, "report", autospec=True) as mock_report:
-            with patch.object(path, "get", side_effect=exception, autospec=True):
-                mock_collector.collect_path(
-                    path,
-                    seen_paths=MOCK_SEEN_PATHS,
-                    module_name=MOCK_MODULE_NAME,
-                )
-                report_func = getattr(mock_report, report_func)
-                report_func.assert_called()
-                mock_log.error.assert_called()
-                assert mock_log.error.call_args.args[0] == log_msg
+    with (
+        patch("acquire.collector.log", autospec=True) as mock_log,
+        patch.object(mock_collector, "report", autospec=True) as mock_report,
+        patch.object(path, "get", side_effect=exception, autospec=True),
+    ):
+        mock_collector.collect_path(
+            path,
+            seen_paths=MOCK_SEEN_PATHS,
+            module_name=MOCK_MODULE_NAME,
+        )
+        report_func = getattr(mock_report, report_func)
+        report_func.assert_called()
+        mock_log.error.assert_called()
+        assert mock_log.error.call_args.args[0] == log_msg
+
+
+def create_temp_files(tmp_path: Path, paths: list[str]) -> None:
+    for path in paths:
+        creation_path = tmp_path.joinpath(path)
+        creation_path.parent.mkdir(parents=True, exist_ok=True)
+        creation_path.touch()
+
+
+def collect_report(
+    collector: Collector,
+    function_name: str,
+    collect_point: Path,
+) -> CollectionReport:
+    func = getattr(collector, f"collect_{function_name}")
+    func(collect_point, module_name=MOCK_MODULE_NAME)
+
+    return collector.report
+
+
+@pytest.mark.parametrize(
+    "function_name, collection_point, expected_results, create_paths",
+    [
+        (
+            "dir",
+            "collect",
+            2,
+            ["collect/this/file", "collect/this/test"],
+        ),
+        (
+            "glob",
+            "/collect/*/file",
+            1,
+            ["collect/this/file"],
+        ),
+        (
+            "glob",
+            "/collect/*/file",
+            0,
+            [],
+        ),
+        (
+            "file",
+            "collect/this/file",
+            1,
+            ["collect/this/file"],
+        ),
+    ],
+)
+def test_collector_report_succeeded(
+    tmp_path: Path,
+    mock_target: Target,
+    mock_collector: Collector,
+    function_name: str,
+    collection_point: str,
+    expected_results: int,
+    create_paths: list[str],
+):
+    create_temp_files(tmp_path, create_paths)
+    fs = mock_target.filesystems[0]
+    fs.map_dir("/", tmp_path)
+    mock_target.fs.mount("/", fs)
+
+    report = collect_report(mock_collector, function_name, collection_point)
+    successful_outputs = list(value for value in report.registry if value.outcome == Outcome.SUCCESS)
+    assert len(successful_outputs) == expected_results
```

### Comparing `acquire-3.8.dev2/tests/test_decryptor_funcs.py` & `acquire-3.8.dev3/tests/test_decryptor_funcs.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tests/test_esxi_memory.py` & `acquire-3.8.dev3/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tests/test_file_sorting.py` & `acquire-3.8.dev3/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tests/test_minio_uploader.py` & `acquire-3.8.dev3/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tests/test_plugin.py` & `acquire-3.8.dev3/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tests/test_utils.py` & `acquire-3.8.dev3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev2/tox.ini` & `acquire-3.8.dev3/tox.ini`

 * *Files identical despite different names*

