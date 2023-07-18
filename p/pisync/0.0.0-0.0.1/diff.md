# Comparing `tmp/pisync-0.0.0.tar.gz` & `tmp/pisync-0.0.1.tar.gz`

## Comparing `pisync-0.0.0.tar` & `pisync-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 pisync-0.0.0/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pisync-0.0.0/dev-requirements.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pisync-0.0.0/requirements.txt
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pisync-0.0.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pisync-0.0.0/examples/run_backups.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pisync-0.0.0/src/pisync/__about__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pisync-0.0.0/src/pisync/__init__.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 pisync-0.0.0/src/pisync/backup.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pisync-0.0.0/src/pisync/util.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pisync-0.0.0/src/pisync/config/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pisync-0.0.0/src/pisync/config/base_config.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pisync-0.0.0/src/pisync/config/local_config.py
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 pisync-0.0.0/src/pisync/config/remote_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pisync-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pisync-0.0.0/tests/conftest.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 pisync-0.0.0/tests/test_backup.py
--rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 pisync-0.0.0/tests/test_local_config.py
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 pisync-0.0.0/tests/test_remote_config.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pisync-0.0.0/LICENSE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pisync-0.0.0/README.md
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 pisync-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 pisync-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pisync-0.0.1/Makefile
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pisync-0.0.1/dev-requirements.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pisync-0.0.1/requirements.txt
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pisync-0.0.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pisync-0.0.1/examples/run_backups.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pisync-0.0.1/src/pisync/__about__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pisync-0.0.1/src/pisync/__init__.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 pisync-0.0.1/src/pisync/backup.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pisync-0.0.1/src/pisync/util.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pisync-0.0.1/src/pisync/config/__init__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pisync-0.0.1/src/pisync/config/base_config.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pisync-0.0.1/src/pisync/config/local_config.py
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 pisync-0.0.1/src/pisync/config/remote_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pisync-0.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pisync-0.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 pisync-0.0.1/tests/test_backup.py
+-rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 pisync-0.0.1/tests/test_local_config.py
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 pisync-0.0.1/tests/test_remote_config.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pisync-0.0.1/LICENSE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pisync-0.0.1/README.md
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 pisync-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 pisync-0.0.1/PKG-INFO
```

### Comparing `pisync-0.0.0/.github/workflows/main.yaml` & `pisync-0.0.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/examples/run_backups.py` & `pisync-0.0.1/examples/run_backups.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/src/pisync/backup.py` & `pisync-0.0.1/src/pisync/backup.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/src/pisync/config/base_config.py` & `pisync-0.0.1/src/pisync/config/base_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/src/pisync/config/local_config.py` & `pisync-0.0.1/src/pisync/config/local_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/src/pisync/config/remote_config.py` & `pisync-0.0.1/src/pisync/config/remote_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/tests/conftest.py` & `pisync-0.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/tests/test_backup.py` & `pisync-0.0.1/tests/test_backup.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/tests/test_local_config.py` & `pisync-0.0.1/tests/test_local_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/tests/test_remote_config.py` & `pisync-0.0.1/tests/test_remote_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/LICENSE` & `pisync-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/README.md` & `pisync-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/pyproject.toml` & `pisync-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pisync-0.0.0/PKG-INFO` & `pisync-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisync
-Version: 0.0.0
+Version: 0.0.1
 Summary: Minimal incremental backup script using rsync 
 Project-URL: Documentation, https://github.com/erietz/pisync#readme
 Project-URL: Issues, https://github.com/erietz/pisync/issues
 Project-URL: Source, https://github.com/erietz/pisync
 Author-email: erietz <ewrietz@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

