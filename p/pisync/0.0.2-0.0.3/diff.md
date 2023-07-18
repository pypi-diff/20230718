# Comparing `tmp/pisync-0.0.2.tar.gz` & `tmp/pisync-0.0.3.tar.gz`

## Comparing `pisync-0.0.2.tar` & `pisync-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pisync-0.0.2/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pisync-0.0.2/dev-requirements.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pisync-0.0.2/requirements.txt
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pisync-0.0.2/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pisync-0.0.2/examples/run_backups.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pisync-0.0.2/src/pisync/__about__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pisync-0.0.2/src/pisync/__init__.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 pisync-0.0.2/src/pisync/backup.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pisync-0.0.2/src/pisync/util.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pisync-0.0.2/src/pisync/config/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pisync-0.0.2/src/pisync/config/base_config.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pisync-0.0.2/src/pisync/config/local_config.py
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 pisync-0.0.2/src/pisync/config/remote_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pisync-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pisync-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 pisync-0.0.2/tests/test_backup.py
--rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 pisync-0.0.2/tests/test_local_config.py
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 pisync-0.0.2/tests/test_remote_config.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pisync-0.0.2/LICENSE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pisync-0.0.2/README.md
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 pisync-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 pisync-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pisync-0.0.3/Makefile
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pisync-0.0.3/dev-requirements.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pisync-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pisync-0.0.3/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pisync-0.0.3/examples/run_backups.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/__about__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/__init__.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/backup.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/util.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/config/__init__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/config/base_config.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/config/local_config.py
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 pisync-0.0.3/src/pisync/config/remote_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pisync-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pisync-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 pisync-0.0.3/tests/test_backup.py
+-rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 pisync-0.0.3/tests/test_local_config.py
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 pisync-0.0.3/tests/test_remote_config.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pisync-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pisync-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pisync-0.0.3/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 pisync-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 pisync-0.0.3/PKG-INFO
```

### Comparing `pisync-0.0.2/Makefile` & `pisync-0.0.3/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 	pytest -s -vv
 
 .PHONY: freeze
 freeze:
 	pip list --format=freeze > requirements.txt
 
 
+.PHONY: dist
 dist:
 	python3 -m pip install --upgrade build
 	python3 -m build
 	python3 -m pip install --upgrade twine
 	echo "CHECK THIS VERSION NUMBER AND CHANGE IF NECESSARY!"
 	cat ./src/pisync/__about__.py
 	python3 -m twine upload dist/*
```

### Comparing `pisync-0.0.2/.github/workflows/main.yaml` & `pisync-0.0.3/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/examples/run_backups.py` & `pisync-0.0.3/examples/run_backups.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/src/pisync/backup.py` & `pisync-0.0.3/src/pisync/backup.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/src/pisync/config/base_config.py` & `pisync-0.0.3/src/pisync/config/base_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/src/pisync/config/local_config.py` & `pisync-0.0.3/src/pisync/config/local_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/src/pisync/config/remote_config.py` & `pisync-0.0.3/src/pisync/config/remote_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/tests/conftest.py` & `pisync-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/tests/test_backup.py` & `pisync-0.0.3/tests/test_backup.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/tests/test_local_config.py` & `pisync-0.0.3/tests/test_local_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/tests/test_remote_config.py` & `pisync-0.0.3/tests/test_remote_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/LICENSE` & `pisync-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/README.md` & `pisync-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pisync-0.0.2/pyproject.toml` & `pisync-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = []
+dependencies = [ "fabric" ]
 
 [project.urls]
 Documentation = "https://github.com/erietz/pisync#readme"
 Issues = "https://github.com/erietz/pisync/issues"
 Source = "https://github.com/erietz/pisync"
 
 [tool.hatch.version]
```

### Comparing `pisync-0.0.2/PKG-INFO` & `pisync-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisync
-Version: 0.0.2
+Version: 0.0.3
 Summary: Minimal incremental backup script using rsync 
 Project-URL: Documentation, https://github.com/erietz/pisync#readme
 Project-URL: Issues, https://github.com/erietz/pisync/issues
 Project-URL: Source, https://github.com/erietz/pisync
 Author-email: erietz <ewrietz@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: fabric
 Description-Content-Type: text/markdown
 
 `pisync` is a simple library to aid in writing incremental backup scripts to
 local or remote machines. The only dependencies are [rsync][rsync],
 [python][python] >= v3.6, [fabric][fabric], and ssh keys copied over to a unix
 machine if doing a remote backup. *Note:* no dependencies are required on the
 remote machine.
```

