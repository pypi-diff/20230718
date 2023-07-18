# Comparing `tmp/phlorest-0.2.0.tar.gz` & `tmp/phlorest-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phlorest-0.2.0.tar", last modified: Tue Dec 20 09:13:32 2022, max compression
+gzip compressed data, was "phlorest-1.0.0.tar", last modified: Tue Jul 18 13:00:07 2023, max compression
```

## Comparing `phlorest-0.2.0.tar` & `phlorest-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-20 09:13:32.735090 phlorest-0.2.0/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11357 2021-11-25 10:44:17.000000 phlorest-0.2.0/LICENSE
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       50 2021-11-25 10:44:17.000000 phlorest-0.2.0/MANIFEST.in
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3295 2022-12-20 09:13:32.735090 phlorest-0.2.0/PKG-INFO
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1705 2022-12-20 08:36:22.000000 phlorest-0.2.0/README.md
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       81 2022-12-08 07:57:43.000000 phlorest-0.2.0/pyproject.toml
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2277 2022-12-20 09:13:32.739090 phlorest-0.2.0/setup.cfg
--rwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)       39 2022-12-08 07:57:43.000000 phlorest-0.2.0/setup.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-20 09:13:32.735090 phlorest-0.2.0/src/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-20 09:13:32.735090 phlorest-0.2.0/src/phlorest/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      293 2022-12-20 09:12:40.000000 phlorest-0.2.0/src/phlorest/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3945 2022-12-08 07:57:43.000000 phlorest-0.2.0/src/phlorest/__main__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2777 2021-12-01 12:55:24.000000 phlorest-0.2.0/src/phlorest/beast.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     9100 2022-12-14 10:07:07.000000 phlorest-0.2.0/src/phlorest/cldfwriter.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-20 09:13:32.735090 phlorest-0.2.0/src/phlorest/commands/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-11-23 10:18:21.000000 phlorest-0.2.0/src/phlorest/commands/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2429 2022-12-14 08:12:27.000000 phlorest-0.2.0/src/phlorest/commands/check.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1734 2021-11-24 15:07:25.000000 phlorest-0.2.0/src/phlorest/commands/merge_characters.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     9652 2022-12-14 08:50:37.000000 phlorest-0.2.0/src/phlorest/dataset.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2192 2022-12-14 09:47:03.000000 phlorest-0.2.0/src/phlorest/metadata.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3324 2022-12-08 07:57:43.000000 phlorest-0.2.0/src/phlorest/nexuslib.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-20 09:13:32.735090 phlorest-0.2.0/src/phlorest/phlorest_template/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-20 09:13:32.735090 phlorest-0.2.0/src/phlorest/phlorest_template/.github/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-20 09:13:32.735090 phlorest-0.2.0/src/phlorest/phlorest_template/.github/workflows/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      629 2021-11-23 10:18:21.000000 phlorest-0.2.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      796 2022-11-24 06:45:17.000000 phlorest-0.2.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-20 09:13:32.735090 phlorest-0.2.0/src/phlorest/phlorest_template/etc/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       10 2021-11-23 10:18:21.000000 phlorest-0.2.0/src/phlorest/phlorest_template/etc/characters.csv
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       16 2021-11-23 10:18:21.000000 phlorest-0.2.0/src/phlorest/phlorest_template/etc/taxa.csv
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       89 2021-11-23 10:18:21.000000 phlorest-0.2.0/src/phlorest/phlorest_template/setup.cfg
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      605 2021-11-23 10:18:21.000000 phlorest-0.2.0/src/phlorest/phlorest_template/setup.py_tmpl
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      258 2021-11-23 10:18:21.000000 phlorest-0.2.0/src/phlorest/scaffold.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-20 09:13:32.735090 phlorest-0.2.0/src/phlorest.egg-info/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3295 2022-12-20 09:13:32.000000 phlorest-0.2.0/src/phlorest.egg-info/PKG-INFO
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      924 2022-12-20 09:13:32.000000 phlorest-0.2.0/src/phlorest.egg-info/SOURCES.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2022-12-20 09:13:32.000000 phlorest-0.2.0/src/phlorest.egg-info/dependency_links.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      172 2022-12-20 09:13:32.000000 phlorest-0.2.0/src/phlorest.egg-info/entry_points.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-11-23 10:18:32.000000 phlorest-0.2.0/src/phlorest.egg-info/not-zip-safe
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      236 2022-12-20 09:13:32.000000 phlorest-0.2.0/src/phlorest.egg-info/requires.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        9 2022-12-20 09:13:32.000000 phlorest-0.2.0/src/phlorest.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-23 10:52:09.000000 phlorest-1.0.0/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)       50 2022-12-23 10:52:09.000000 phlorest-1.0.0/MANIFEST.in
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2907 2023-07-18 13:00:07.177544 phlorest-1.0.0/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1934 2023-07-17 08:36:51.000000 phlorest-1.0.0/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)       81 2022-12-23 10:52:09.000000 phlorest-1.0.0/pyproject.toml
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2242 2023-07-18 13:00:07.177544 phlorest-1.0.0/setup.cfg
+-rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2022-12-23 10:52:08.000000 phlorest-1.0.0/setup.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      293 2023-07-18 12:59:16.000000 phlorest-1.0.0/src/phlorest/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3945 2022-12-23 10:52:07.000000 phlorest-1.0.0/src/phlorest/__main__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3307 2023-07-12 10:55:15.000000 phlorest-1.0.0/src/phlorest/beast.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    10020 2023-07-17 10:08:16.000000 phlorest-1.0.0/src/phlorest/cldfwriter.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/commands/
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/commands/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2429 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/commands/check.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1734 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/commands/merge_characters.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     8676 2023-07-18 11:31:01.000000 phlorest-1.0.0/src/phlorest/dataset.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2192 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/metadata.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3700 2023-07-17 11:04:32.000000 phlorest-1.0.0/src/phlorest/nexuslib.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/phlorest_template/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/phlorest_template/.github/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/phlorest_template/.github/workflows/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      629 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml
+-rw-rw-r--   0 robert    (1000) robert    (1000)      796 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest/phlorest_template/etc/
+-rw-rw-r--   0 robert    (1000) robert    (1000)       10 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/etc/characters.csv
+-rw-rw-r--   0 robert    (1000) robert    (1000)       16 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/etc/taxa.csv
+-rw-rw-r--   0 robert    (1000) robert    (1000)       89 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/setup.cfg
+-rw-rw-r--   0 robert    (1000) robert    (1000)      605 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/phlorest_template/setup.py_tmpl
+-rw-rw-r--   0 robert    (1000) robert    (1000)      258 2022-12-23 10:52:08.000000 phlorest-1.0.0/src/phlorest/scaffold.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/src/phlorest.egg-info/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2907 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1078 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)      171 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/entry_points.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-12-23 10:52:07.000000 phlorest-1.0.0/src/phlorest.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)      245 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        9 2023-07-18 13:00:07.000000 phlorest-1.0.0/src/phlorest.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 13:00:07.177544 phlorest-1.0.0/tests/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      663 2023-07-12 10:55:15.000000 phlorest-1.0.0/tests/test_beast.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2232 2023-07-12 10:55:15.000000 phlorest-1.0.0/tests/test_cldfwriter.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      681 2022-12-23 10:52:07.000000 phlorest-1.0.0/tests/test_cli.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3484 2023-07-12 10:55:15.000000 phlorest-1.0.0/tests/test_dataset.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      409 2022-12-23 10:52:07.000000 phlorest-1.0.0/tests/test_metadata.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      814 2023-07-12 10:55:15.000000 phlorest-1.0.0/tests/test_nexuslib.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      261 2022-12-23 10:52:07.000000 phlorest-1.0.0/tests/test_scaffold.py
```

### Comparing `phlorest-0.2.0/LICENSE` & `phlorest-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phlorest-0.2.0/PKG-INFO` & `phlorest-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,105 @@
 Metadata-Version: 2.1
 Name: phlorest
-Version: 0.2.0
+Version: 1.0.0
 Summary: A cldfbench plugin to curate language phylogenies
 Home-page: https://github.com/phlorest/phlorest
 Author: Simon Greenhill and Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/phlorest/phlorest/issues
-Description: # phlorest
-        
-        A [cldfbench](https://github.com/cldf/cldfbench) plugin to curate language phylogenies.
-        
-        
-        ## Install
-        
-        ```shell
-        pip install phlorest
-        ```
-        
-        
-        ## Usage
-        
-        ### Bootstrapping a `phlorest`-curated dataset
-        
-        `phlorest` provides a `cldfbench` dataset template to create the skeleton of files and directories for a
-        `phlorest`-curated dataset, to be run with [cldfbench new](https://github.com/cldf/cldfbench/#creating-a-skeleton-for-a-new-dataset-directory).
-        
-        Running
-        
-        ```shell
-        cldfbench new --template phlorest 
-        ```
-        
-        will create a dataset skeleton looking as follows
-        ```shell
-        $ tree testtree/
-        testtree/
-        ├── cldf
-        │   └── README.md
-        ├── cldfbench_testtree.py
-        ├── etc
-        │   ├── characters.csv
-        │   └── taxa.csv
-        ├── metadata.json
-        ├── raw
-        │   └── README.md
-        ├── setup.cfg
-        ├── setup.py
-        └── test.py
-        ```
-        
-        
-        ### Implementng CLDF creation
-        
-        Implementing CLDF creation means - as for any other `cldfbench`-curated dataset - filling in the
-        `cmd_makecldf` method of the `Dataset` subclass in `cldfbench_<id>.py`.
-        
-        The CLDF writer which can be accessed as `args.writer` within `cmd_makecldf` is an instance of
-        `phlorest.CLDFWriter`, which has convenience methods to add summary- or posterior trees to the CLDF
-        dataset. At least a summary is needed to make a dataset valid. Adding one looks as follows
-        
-        ```python
-            args.writer.add_summary(
-                self.raw_dir.read_tree(...),
-                self.metadata,
-                args.log)
-        ```
-        
-        
-        ### Running CLDF creation
-        
-        With `cmd_makecldf` implemented, CLDF creation can be triggered running
-        ```shell
-        cldfbench makecldf cldfbench_<id>.py
-        ```
-        
-        The resulting CLDF dataset can be validated running
-        ```shell
-        pytest
-        ```
-        
 Keywords: cldf
 Platform: any
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# phlorest
+
+A [cldfbench](https://github.com/cldf/cldfbench) plugin to curate language phylogenies.
+
+
+## Install
+
+```shell
+pip install phlorest
+```
+
+
+## Usage
+
+### Bootstrapping a `phlorest`-curated dataset
+
+`phlorest` provides a `cldfbench` dataset template to create the skeleton of files and directories for a
+`phlorest`-curated dataset, to be run with [cldfbench new](https://github.com/cldf/cldfbench/#creating-a-skeleton-for-a-new-dataset-directory).
+
+Running
+
+```shell
+cldfbench new --template phlorest 
+```
+
+will create a dataset skeleton looking as follows
+```shell
+$ tree testtree/
+testtree/
+├── cldf
+│   └── README.md
+├── cldfbench_testtree.py
+├── etc
+│   ├── characters.csv
+│   └── taxa.csv
+├── metadata.json
+├── raw
+│   └── README.md
+├── setup.cfg
+├── setup.py
+└── test.py
+```
+
+
+### Implementing CLDF creation
+
+Implementing CLDF creation means - as for any other `cldfbench`-curated dataset - filling in the
+`cmd_makecldf` method of the `Dataset` subclass in `cldfbench_<id>.py`.
+
+The CLDF writer which can be accessed as `args.writer` within `cmd_makecldf` is an instance of
+`phlorest.CLDFWriter`, which has convenience methods to add summary- or posterior trees to the CLDF
+dataset. At least a summary is needed to make a dataset valid. Adding one looks as follows
+
+```python
+    args.writer.add_summary(
+        self.raw_dir.read_tree(...),
+        self.metadata,
+        args.log)
+```
+
+
+### Running CLDF creation
+
+With `cmd_makecldf` implemented, CLDF creation can be triggered running
+```shell
+cldfbench makecldf cldfbench_<id>.py
+```
+
+The resulting CLDF dataset can be validated running
+```shell
+pytest
+```
+
+
+## Dependencies
+
+The `run_treeannotator` method of `Dataset` requires the `treeannotator` command from BEAST to be
+installed. For details on how to install `treeannotator` (and `BEAST`), see https://beast.community/index.html
```

### Comparing `phlorest-0.2.0/README.md` & `phlorest-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 │   └── README.md
 ├── setup.cfg
 ├── setup.py
 └── test.py
 ```
 
 
-### Implementng CLDF creation
+### Implementing CLDF creation
 
 Implementing CLDF creation means - as for any other `cldfbench`-curated dataset - filling in the
 `cmd_makecldf` method of the `Dataset` subclass in `cldfbench_<id>.py`.
 
 The CLDF writer which can be accessed as `args.writer` within `cmd_makecldf` is an instance of
 `phlorest.CLDFWriter`, which has convenience methods to add summary- or posterior trees to the CLDF
 dataset. At least a summary is needed to make a dataset valid. Adding one looks as follows
@@ -66,7 +66,13 @@
 cldfbench makecldf cldfbench_<id>.py
 ```
 
 The resulting CLDF dataset can be validated running
 ```shell
 pytest
 ```
+
+
+## Dependencies
+
+The `run_treeannotator` method of `Dataset` requires the `treeannotator` command from BEAST to be
+installed. For details on how to install `treeannotator` (and `BEAST`), see https://beast.community/index.html
```

### Comparing `phlorest-0.2.0/setup.cfg` & `phlorest-1.0.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phlorest
-version = 0.2.0
+version = 1.0.0
 author = Simon Greenhill and Robert Forkel
 author_email = dlce.rdm@eva.mpg.de
 description = A cldfbench plugin to curate language phylogenies
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = cldf
 license = Apache 2.0
@@ -15,35 +15,35 @@
 platforms = any
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Developers
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: Apache Software License
 
 [options]
 zip_safe = False
 packages = find:
 package_dir = 
 	= src
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
+	newick>=1.9
+	commonnexus>=1.4
 	cldfviz>=0.10
 	pycldf>=1.33.0
 	clldutils
 	cldfbench>=1.10.0
 	cldfcatalog
 	attrs
-	python-nexus>=2.8.0
 	pyglottolog>=3.9.0
 	termcolor
 include_package_data = True
 
 [options.packages.find]
 where = src
 
@@ -101,15 +101,15 @@
 	tests
 
 [coverage:report]
 show_missing = true
 skip_covered = true
 
 [tox:tox]
-envlist = py37, py38, py39, py310, py311
+envlist = py38, py39, py310, py311
 isolated_build = true
 skip_missing_interpreter = true
 
 [testenv]
 deps = .[test]
 commands = pytest {posargs}
```

### Comparing `phlorest-0.2.0/src/phlorest/__main__.py` & `phlorest-1.0.0/src/phlorest/__main__.py`

 * *Files identical despite different names*

### Comparing `phlorest-0.2.0/src/phlorest/beast.py` & `phlorest-1.0.0/src/phlorest/beast.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,82 @@
+import typing
+import pathlib
+import collections
 import xml.etree.cElementTree as ElementTree
 
-import nexus
+from commonnexus import Nexus
+from commonnexus.blocks import Characters
 
 __all__ = ['BeastFile']
 
 
 class BeastFile:
-    def __init__(self, path, text=None):
+    def __init__(self, path: typing.Union[str, pathlib.Path], text: typing.Optional[str] = None):
         self.path = path
         self.text = text
+        if self.text:
+            self.xml = ElementTree.fromstring(self.text)
+        else:
+            self.xml = ElementTree.parse(str(self.path))
 
-    def nexus_and_characters(self):
-        return beast_to_nexus(self.path or self.text)
-
-
-def beast_to_nexus(filename, valid_states="01?"):
-    nex = nexus.NexusWriter()
-    if isinstance(filename, str):
-        xml = ElementTree.fromstring(filename)
-    else:
-        xml = ElementTree.parse(str(filename))
-    #
-    # <sequence>
-    # <taxon idref=""/>
-    # 1111111
-    # </sequence>
-    #
-    seq_found = False
-    for seq in xml.findall('./data/sequence'):
-        seq_found = True
-        for i, state in enumerate([s for s in seq.get('value') if s != ' '], start=1):
-            assert state in valid_states, 'Invalid State %s' % state
-            nex.add(seq.get('taxon'), i, state)
-
-    if not seq_found:
-        for seq in xml.findall('.//sequence[taxon]'):
-            data = (seq.text.strip() if seq.text else None) or seq.find('taxon').tail.strip()
-            assert data, ElementTree.tostring(seq).decode('utf8').replace('\n', '')
-            for i, state in enumerate(list(data), start=1):
+    def nexus(self, valid_states: str = '01?') -> Nexus:
+        """
+        Read the character data used in a BEAST file and format it as NEXUS file.
+
+        :param valid_states: String listing one-character state labels.
+        :return: A Nexus instance with a CHARACTERS block encoding the data from the BEAST file as \
+        MATRIX.
+        """
+        try:  # Read the character labels.
+            chars = dict(self.iter_characters())
+        except (ValueError, KeyError):  # pragma: no cover
+            chars = {}  # No character labels.
+
+        matrix = collections.OrderedDict()
+
+        def add_row(taxon, seq):
+            matrix[taxon] = collections.OrderedDict()
+            for i, state in enumerate([s for s in seq if s != ' '], start=1):
                 assert state in valid_states, 'Invalid State %s' % state
-                nex.add(seq.find('taxon').get('idref'), i, state)
+                matrix[taxon][chars.get(i, str(i))] = None if state == '?' else state
 
-    try:
-        chars = sorted(list(beast2chars(xml)))
-    except (ValueError, KeyError):  # pragma: no cover
-        chars = None
-    return nexus.NexusReader.from_string(nex.write()), chars
-
-
-def beast2chars(xml):
-    def get_partition(p):
-        x, y = [int(_) for _ in p.get('filter').split("-")]
-        return (p.get('id'), x, y)
-
-    def printchar(p, x, y, ascertained=False):
-        n = 1
-        for i in range(x, y + 1):
-            label = "%s-%s" % (p, 'ascertained' if n == 1 and ascertained else str(n))
-            yield i, label
-            n += 1
-
-    def get_by_id(data_id):
-        if data_id.startswith("@"):
-            data_id = data_id.lstrip("@")
-        res = xml.find(".//alignment[@id='%s']" % data_id)
-        if res is None:  # pragma: no cover
-            raise ValueError(data_id)
-        return res
-
-    for treelh in xml.findall(".//distribution[@spec='TreeLikelihood']"):
-        if treelh.get('data'):
-            data = get_by_id(treelh.get('data'))
-            ascertained = data.get('ascertained') == 'true'
-            yield from printchar(*get_partition(data.find('./data')), ascertained=ascertained)
-        else:
-            data = treelh.find('./data')
-            ascertained = data.get('ascertained') == 'true'
-            dd = get_by_id(data.get('data')) if data.get('data') else treelh.find('./data/data')
-            yield from printchar(*get_partition(dd), ascertained=ascertained)
+        for seq in self.xml.findall('./data/sequence'):
+            add_row(seq.get('taxon'), seq.get('value'))
+
+        if not matrix:
+            for seq in self.xml.findall('.//sequence[taxon]'):
+                data = (seq.text.strip() if seq.text else None) or seq.find('taxon').tail.strip()
+                assert data, ElementTree.tostring(seq).decode('utf8').replace('\n', '')
+                add_row(seq.find('taxon').attrib['idref'], data)
+
+        return Nexus.from_blocks(Characters.from_data(matrix))
+
+    def iter_characters(self):
+        def get_partition(p):
+            x, y = [int(_) for _ in p.get('filter').split("-")]
+            return (p.get('id'), x, y)
+
+        def printchar(p, x, y, ascertained=False):
+            n = 1
+            for i in range(x, y + 1):
+                label = "%s-%s" % (p, 'ascertained' if n == 1 and ascertained else str(n))
+                yield i, label
+                n += 1
+
+        def get_by_id(data_id):
+            if data_id.startswith("@"):
+                data_id = data_id.lstrip("@")
+            res = self.xml.find(".//alignment[@id='%s']" % data_id)
+            if res is None:  # pragma: no cover
+                raise ValueError(data_id)
+            return res
+
+        for treelh in self.xml.findall(".//distribution[@spec='TreeLikelihood']"):
+            if treelh.get('data'):
+                data = get_by_id(treelh.get('data'))
+                ascertained = data.get('ascertained') == 'true'
+                yield from printchar(*get_partition(data.find('./data')), ascertained=ascertained)
+            else:
+                data = treelh.find('./data')
+                ascertained = data.get('ascertained') == 'true'
+                dd = get_by_id(data.get('data')) if data.get('data') else treelh.find('./data/data')
+                yield from printchar(*get_partition(dd), ascertained=ascertained)
```

### Comparing `phlorest-0.2.0/src/phlorest/cldfwriter.py` & `phlorest-1.0.0/src/phlorest/cldfwriter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import typing
+import pathlib
 
 import cldfbench
-
+import newick
 import tqdm
-import nexus
-from nexus.handlers.tree import Tree as NexusTree
 from pycldf.terms import TERMS
+from commonnexus import Nexus
+from commonnexus.tools.normalise import normalise
+from commonnexus.tools.matrix import CharacterMatrix
+from commonnexus.blocks.characters import Characters
 
+from .beast import BeastFile
 from .metadata import Metadata
 from .nexuslib import NexusFile
-from .beast import BeastFile
 
 
 class CLDFWriter(cldfbench.CLDFWriter):
     """
     A CLDF writer that knows how to add phylogentic data.
     """
     def __enter__(self):
@@ -70,22 +73,23 @@
             k = rename.get(k, k)
             if k in TERMS:
                 k = TERMS[k].to_column().name
             d[k] = v
         self.objects[table].append(d)
 
     def add_tree(self,
-                 tree: NexusTree,
+                 tree: typing.Union[str, newick.Node],
                  nex: NexusFile,
                  tid: str,
                  metadata: Metadata,
                  log,
                  type_,
-                 source=None):
-        nex.append(tree, tid, self._lids, metadata.scaling, log)
+                 source=None,
+                 rooted: typing.Optional[bool] = None):
+        nex.append(tree, tid, self._lids, metadata.scaling, log, rooted=rooted)
         if source is None:
             bibkeys = list(self.cldf.sources.keys())
             if len(bibkeys) == 1:
                 source = bibkeys[0]
 
         # Add media file only if necessary!
         mids = [m['ID'] for m in self.objects['MediaTable']]
@@ -98,68 +102,83 @@
                 Path_In_Zip=None if nex.path.stem == 'summary' else 'posterior.trees',
             ))
 
         self.objects['TreeTable'].append(dict(
             ID=tid,
             Name=tid,
             Media_ID=nex.path.stem,
-            Tree_Is_Rooted=tree.rooted,
+            Tree_Is_Rooted=rooted,
             Tree_Type=type_,
             Description=metadata.analysis,
             Tree_Branch_Length_Unit=None if nex.scaling == 'none' else nex.scaling,
             Source=[source] if isinstance(source, str) else source,
         ))
 
     def add_summary(self,
-                    tree: NexusTree,
+                    tree: typing.Union[str, newick.Node],
                     metadata: Metadata,
                     log,
-                    source=None):
-        self.add_tree(tree, self.summary, 'summary', metadata, log, 'summary', source=source)
+                    source=None,
+                    rooted=None):
+        """
+        Add `tree` as summary tree to the dataset.
+        """
+        self.add_tree(
+            tree, self.summary, 'summary', metadata, log, 'summary', source=source, rooted=rooted)
         log.info("added summary tree")
 
     def add_posterior(self,
-                      trees: typing.List[NexusTree],
+                      trees: typing.List[typing.Union[str, newick.Node]],
                       metadata: Metadata,
                       log,
                       source=None,
-                      verbose=False):
+                      verbose=False,
+                      rooted=None):
+        """
+        Add `trees` as posterior sample of trees to the dataset.
+        """
         i = 0
         for i, tree in (
                 tqdm.tqdm(enumerate(trees, start=1), total=len(trees))
                 if verbose else enumerate(trees, start=1)):
             self.add_tree(
                 tree,
                 self.posterior,
                 'posterior-{}'.format(i),
                 metadata,
                 log,
                 'sample',
-                source=source)
+                source=source,
+                rooted=rooted)
         log.info("added posterior trees (n=%d)" % i)
 
-    def add_data(self, input, characters, log):
+    def add_data(self,
+                 input: typing.Union[BeastFile, pathlib.Path, str, Nexus],
+                 characters: typing.Iterable[typing.Dict[str, str]],
+                 log,
+                 binarise: bool = False):
+        """
+        Add character data from which the tree(s) in the dataset were computed.
+
+        :param input: Character data can be read from BEAST files and NEXUS files.
+        :param characters: Character metadata, per site.
+        :param log:
+        """
         if isinstance(input, BeastFile):
-            nex, chars = input.nexus_and_characters()
+            nex = input.nexus()
+        elif isinstance(input, pathlib.Path):
+            nex = Nexus.from_file(input)
+        elif isinstance(input, str):
+            nex = Nexus(input)
         else:
-            nex = input if isinstance(input, (nexus.NexusReader, nexus.NexusWriter)) \
-                else nexus.NexusReader(input)
-            chars = sorted(nex.data.charlabels.items())
-
-        if not chars:
-            chars = [
-                (i + 1, 'Site {}'.format(i + 1))
-                for i, _ in enumerate(list(nex.data.matrix.values())[0])]
-
-        if chars[0][0] == 0:
-            # A zero-based index. Switch to 1-based:
-            chars = [(k + 1, v) for k, v in chars]
+            nex = input
+        assert isinstance(nex, Nexus)
+        charlabels, _ = nex.characters.get_charstatelabels()
 
         md = {int(row.pop('Site')): row for row in characters}
-        assert all(len(chars) == len(d) for d in nex.data.matrix.values()), str(len(chars))
         t = self.cldf.add_component(
             'ParameterTable',
             {
                 'name': 'Nexus_File',
                 'dc:description':
                     'The data for this parameter is stored at 1-based index {ID} '
                     'of the sequences in the DATA block of the Nexus file specified here. '
@@ -171,39 +190,44 @@
             "The ParameterTable lists characters (a.k.a. sites), i.e. the (often binary) " \
             "variables used as data basis to compute the phylogeny from."
         if md:
             self.add_columns(
                 'ParameterTable', list(md.values())[0], log, exclude=['Label'])
         self.cldf['ParameterTable', 'ID'].common_props['dc:description'] = \
             "Sequence index of the site in the corresponding Nexus file."
-        for site, label in chars:
+        for site, label in charlabels.items():
             d = dict(ID=site, Name=label, Nexus_File='data')
             self.add_obj('ParameterTable', d, md.get(site, {}), rename=dict(Label='Name'))
         self.add_obj(
             'MediaTable',
             dict(ID='data', Media_Type='text/plain', Download_URL='file:///data.nex'))
 
-        missing = [t for t in nex.data.taxa if t not in self._lids]
-        assert not len(missing), "Taxa in nexus not in taxa.csv: %r" % missing
+        assert all(t in self._lids for t in nex.taxa), "Taxa in nexus not in taxa.csv: {}".format(
+            [t for t in nex.taxa if t not in self._lids])
 
-        missing = [t for t in nex.data.matrix if t not in self._lids]
-        assert not len(missing), "Taxa in nexus not in taxa.csv: %r" % missing
+        if binarise:
+            _, statelabels = nex.characters.get_charstatelabels()
+            new = CharacterMatrix.binarised(nex.characters.get_matrix(), statelabels=statelabels)
+            nex.replace_block(nex.characters, Characters.from_data(new))
 
-        nex.write_to_file(self.cldf_spec.dir / 'data.nex')
+        normalise(nex).to_file(self.cldf_spec.dir / 'data.nex')
         self.cldf.add_provenance(
             wasDerivedFrom={
                 "rdf:about": "data.nex",
                 "rdf:type": "prov:Entity",
                 'dc:description': 'The data underlying the analysis which created the phylogeny',
                 'dc:format': 'https://en.wikipedia.org/wiki/Nexus_file',
             }
         )
-        log.info("added data nexus (characters=%d)" % len(chars))
+        log.info("added data nexus (characters=%d)" % len(charlabels))
 
-    def add_taxa(self, taxa, glottolog, log):
+    def add_taxa(self,
+                 taxa: typing.List[typing.Dict[str, str]],
+                 glottolog,
+                 log):
         glangs = {lg.id: lg for lg in glottolog.languoids()}
         #
         # FIXME: add metadata from Glottolog, put in dplace-tree-specific Dataset base class.
         # FIXME: log warnings if taxa are mapped to bookkeeping languoids!
         #
         for i, row in enumerate(taxa):
             if i == 0:
```

### Comparing `phlorest-0.2.0/src/phlorest/commands/check.py` & `phlorest-1.0.0/src/phlorest/commands/check.py`

 * *Files identical despite different names*

### Comparing `phlorest-0.2.0/src/phlorest/commands/merge_characters.py` & `phlorest-1.0.0/src/phlorest/commands/merge_characters.py`

 * *Files identical despite different names*

### Comparing `phlorest-0.2.0/src/phlorest/dataset.py` & `phlorest-1.0.0/src/phlorest/dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,61 @@
-import re
+import gzip
 import shlex
-import random
 import shutil
+import random
 import typing
 import pathlib
 import subprocess
 
 import cldfbench
 from cldfbench.datadir import DataDir
-import nexus
-from nexus.handlers.tree import Tree
-from nexus.tools import delete_trees, sample_trees, strip_comments_in_trees
 from pyglottolog.languoids import Glottocode
 from clldutils.path import TemporaryDirectory, ensure_cmd
 from pycldf.trees import TreeTable
 from cldfviz.tree import render
+from commonnexus import Nexus
+from commonnexus.tools.normalise import normalise as nexus_norm
 
+from .nexuslib import Tree
 from .metadata import Metadata
 from .cldfwriter import CLDFWriter
 
 
 class PhlorestDir(DataDir):
     """
     Enhanced `DataDir`, adding methods to access phylogenetic data.
     """
     def read_nexus(self,
                    path: typing.Optional[typing.Union[str, pathlib.Path]] = None,
                    text: typing.Optional[str] = None,
-                   remove_rate: bool = False,
                    encoding: str = 'utf-8-sig',
-                   preprocessor: typing.Callable[[str], str] = lambda s: s) -> nexus.NexusReader:
+                   normalise: bool = False,
+                   preprocessor: typing.Callable[[str], str] = lambda s: s) -> Nexus:
         """
         :param path: path to nexus file (or `None`).
         :param text: text content of a nexus file.
-        :param remove_rate: Some trees have annotations before *and* after the colon, separating \
-        the branch length. The newick package can't handle these. So we can remove the simpler \
-        annotation after the ":".
-        :return: Initialized `NexusReader` object.
+        :return: Initialized `Nexus` object.
         """
         assert (path or text) and not (path and text), 'Must pass either path or text'
-        if not text:
-            text = self.read(path, encoding=encoding)
-        if remove_rate:
-            text = self.remove_rate(text)
-        return nexus.NexusReader.from_string(preprocessor(text))
+        if path:
+            path = self._path(path)
+            if path.suffix == '.gz':
+                with gzip.open(path, 'rt', encoding='utf8') as fp:
+                    text = fp.read()
+        res = Nexus(preprocessor(text or self.read(path, encoding=encoding)))
+        return nexus_norm(res) if normalise else res
 
     def read_trees(self,
                    path: typing.Union[str, pathlib.Path] = None,
                    text: str = None,
                    detranslate: bool = False,
                    burnin: int = 0,
                    sample: int = 0,
-                   remove_rate: bool = False,
                    strip_annotation: bool = False,
+                   seed=12345,
                    preprocessor: typing.Callable[[str], str] = lambda s: s) -> typing.List[Tree]:
         """
         Reads trees from `path` and transforms them as required.
 
         Processing order:
             burnin -> sample -> strip_annotation -> remove_rate -> detranslate
 
@@ -67,62 +66,59 @@
         :param sample: number of trees to sample (default=all).
         :param remove_rate: remove extra rate information.
         :param strip_annotation: remove comments and annotations in trees (default=False).
         :param preprocessor: function to preprocess nexus text.
         :return:
         """
         nex = self.read_nexus(path=path, text=text, preprocessor=preprocessor)
+        trees = nex.TREES.trees
         # remove burn-in first
         if burnin:
-            nex = delete_trees(nex, list(range(burnin + 1)))
+            trees = trees[burnin:]
         # ..then sample if needed
-        if sample and len(nex.trees.trees) > sample:
-            nex = sample_trees(nex, sample)
-        # remove comments if asked
-        if strip_annotation:
-            nex = strip_comments_in_trees(nex)
-        # remove rates if asked
-        if remove_rate:
-            nex.trees.trees = [self.remove_rate(t) for t in nex.trees.trees]
+        if sample and len(trees) > sample:
+            random.seed(seed)
+            trees = random.sample(trees, sample)
+
+        trees = [Tree(tree.name, tree.newick, tree.rooted) for tree in trees]
         # ...then detranslate.
         if detranslate:
-            nex.trees.detranslate()
-        return nex.trees.trees
+            # We must use a reference to the same block in order to make the translation-mapping
+            # caching work.
+            cmd = nex.TREES.translate
+            for tree in trees:
+                tree.newick = cmd(tree.newick)
+
+        # remove comments if asked
+        if strip_annotation:
+            for tree in trees:
+                tree.newick.strip_comments()
+
+        return trees
 
     def read_tree(self,
                   path: typing.Union[str, pathlib.Path] = None,
                   text: str = None,
                   detranslate: bool = False,
                   burnin: int = 0,
                   sample: int = 0,
                   remove_rate: bool = False,
                   strip_annotation: bool = False,
+                  seed=12345,
                   preprocessor=lambda s: s) -> Tree:
         return self.read_trees(
             path=path,
             text=text,
             detranslate=detranslate,
             burnin=burnin,
             sample=sample,
-            remove_rate=remove_rate,
             strip_annotation=strip_annotation,
+            seed=seed,
             preprocessor=preprocessor)[0]
 
-    def remove_rate(self, text: str) -> Tree:
-        """
-        Some trees have annotations before *and* after the colon (i.e. on the
-        node), separating the branch length. The newick package can't handle
-        these. This method removes the simpler annotation after the ":", keeping
-        the branch annotations.
-
-        :param text: nexus content in text.
-        :return: str
-        """
-        return Tree(re.sub(r':\[&rate=[0-9]*\.?[0-9]*]', ':', text))
-
 
 class Dataset(cldfbench.Dataset):
     """
     An augmented `cldfbench.Dataset`
 
     - swapping in `PhlorestDir` as `DataDir` implementation for `raw`
     - swapping in a custom CLDFWriter implementation `phorest.cldfwriter.CLDFWriter`
@@ -199,45 +195,28 @@
     def taxa(self) -> typing.List[dict]:
         return self._read_from_etc('taxa.csv')
 
     @property
     def characters(self) -> typing.List[dict]:
         return self._read_from_etc('characters.csv')
 
-    def run_treeannotator(self, cmd, input):
+    @staticmethod
+    def run_treeannotator(cmd, input: typing.Union[str, pathlib.Path]) -> Nexus:
         with TemporaryDirectory() as d:
             in_ = d / 'in.nex'
             if isinstance(input, str):
                 in_.write_text(input, encoding='utf8')
             else:
                 shutil.copy(input, in_)
             out = d / 'out.nex'
             subprocess.check_call(
                 [ensure_cmd('treeannotator')] + shlex.split(cmd) + [str(in_), str(out)],
                 stderr=subprocess.DEVNULL,
             )
-            return nexus.NexusReader.from_string(out.read_text(encoding='utf8'))
+            return Nexus(out.read_text(encoding='utf8'))
 
-    def run_rscript(self, script, output_fname):
+    @staticmethod
+    def run_rscript(script, output_fname):
         with TemporaryDirectory() as d:
             d.joinpath('script.r').write_text(script, encoding='utf8')
             subprocess.check_call([ensure_cmd('Rscript'), str(d / 'script.r')], cwd=d)
             return d.joinpath(output_fname).read_text(encoding='utf8')
-
-    def remove_burnin(self, input, amount, as_nexus=False):
-        res = delete_trees(input, list(range(amount + 1)))
-        return res if as_nexus else res.write()
-
-    def sample(self,
-               input,
-               seed=12345,
-               detranslate=False,
-               as_nexus=False,
-               n=1000,
-               strip_annotation=False):
-        random.seed(seed)
-        res = sample_trees(input, n)
-        if strip_annotation:
-            res = strip_comments_in_trees(res)
-        if detranslate:
-            res.trees.detranslate()
-        return res if as_nexus else res.write()
```

### Comparing `phlorest-0.2.0/src/phlorest/metadata.py` & `phlorest-1.0.0/src/phlorest/metadata.py`

 * *Files identical despite different names*

### Comparing `phlorest-0.2.0/src/phlorest/nexuslib.py` & `phlorest-1.0.0/src/phlorest/nexuslib.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,83 @@
 import copy
 import typing
 import zipfile
 import functools
+import dataclasses
 
 import newick
-import nexus
-from nexus.handlers.tree import Tree as NexusTree
-from nexus.tools import visit_tree_nodes
+from commonnexus import Nexus
+from commonnexus.blocks import Trees
 
 from .metadata import RESCALE_TO_YEARS
 
-__all__ = ['newick2nexus', 'NexusFile']
+__all__ = ['NexusFile', 'Tree', 'rescale_to_years']
 
 
-def newick2nexus(tree: typing.Union[str, newick.Node], name='tree') -> NexusTree:
-    tree = getattr(tree, 'newick', tree)
-    if not tree.endswith(';'):
-        tree += ';'
-    return NexusTree('tree {} = {}'.format(name, tree))
-
-
-def rescale_to_years(nex, orig_scaling, log=None):
+def rescale_to_years(nex: Nexus, orig_scaling, log=None) -> Nexus:
     """
-    Rescales trees in a nexus file to years (if possible) in the fashion of other `nexus.tools`
-    tree manipulation functions.
+    Rescales trees in a nexus file to years (if possible).
 
     :param nex:
     :param orig_scaling:
     :param log:
-    :return: The mutated `NexusReader` object.
+    :return: The mutated `Nexus` object.
     """
     def _rescaler(factor, n):
-        n._length_formatter = lambda l: '{:.0f}'.format(l) if l else None
+        n._length_formatter = lambda lg: '{:.0f}'.format(lg) if lg else None
         if n._length:
             n.length = n.length * factor
 
     if orig_scaling in RESCALE_TO_YEARS:
-        return visit_tree_nodes(nex, functools.partial(_rescaler, RESCALE_TO_YEARS[orig_scaling]))
+        trees = []
+        for tree in nex.TREES.trees:
+            nwk = tree.newick
+            nwk.visit(functools.partial(_rescaler, RESCALE_TO_YEARS[orig_scaling]))
+            trees.append((tree.name, nwk, tree.rooted))
+        nex.replace_block(
+            nex.TREES,
+            Trees.from_data(*trees, **nex.TREES.TRANSLATE.mappings if nex.TREES.TRANSLATE else {}))
+        return nex
     raise ValueError('Cannot rescale {} to years.'.format(orig_scaling))
 
 
+@dataclasses.dataclass
+class Tree:
+    name: str
+    newick: typing.Union[str, newick.Node]
+    rooted: typing.Optional[bool] = None
+
+    def __str__(self):
+        return self.newick if isinstance(self.newick, str) else '{};'.format(self.newick.newick)
+
+
 class NexusFile:
     def __init__(self, path, zipped=False):
         self.path = path
         self._trees = []
         self.scaling = None
         self.zipped = zipped
 
-    def append(self, tree: NexusTree, tid, lids, scaling, log):
+    def append(self,
+               tree: typing.Union[Tree, str, newick.Node],
+               tid: str,
+               lids: typing.List[str],
+               scaling,
+               log,
+               rooted: typing.Optional[bool] = None):
+        if isinstance(tree, Tree):
+            tid = tid or tree.name
+            rooted = rooted or tree.rooted
+            tree = tree.newick
+        if isinstance(tree, str):
+            tree = newick.loads(tree)[0]
         with_lids = bool(lids)
         if with_lids:
             lids = copy.copy(lids)
-        ntree = tree.newick_tree
-        for node in ntree.walk():
+        for node in tree.walk():
             if node.name == 'root':
                 continue
             if node.is_leaf:
                 assert node.name
             if node.name:
                 try:
                     if with_lids:
@@ -72,26 +93,23 @@
             log.warning('extra taxa specified in LanguageTable: {}'.format(lids))
 
         if self.scaling:
             if scaling != self.scaling:
                 raise ValueError('All trees in a NexusFile must have the same scaling!')
         else:
             self.scaling = scaling
-        self._trees.append(NexusTree.from_newick(ntree, name=tid or tree.name, rooted=tree.rooted))
+        self._trees.append((tid, tree, rooted))
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self._trees:
-            nex = nexus.NexusWriter()
-            for i, tree in enumerate(self._trees, start=1):
-                nex.trees.append(NexusTree.from_newick(
-                    tree.newick_string, name=tree.name or 'tree{}'.format(i), rooted=tree.rooted))
-            nex.write_to_file(self.path)
+            nex = Nexus.from_blocks(Trees.from_data(*self._trees))
+            nex.to_file(self.path)
             if self.zipped:
                 with zipfile.ZipFile(
                     self.path.parent / (self.path.name + '.zip'),
                     'w',
                     compression=zipfile.ZIP_DEFLATED
                 ) as zf:
                     zf.write(self.path, self.path.name)
```

### Comparing `phlorest-0.2.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml` & `phlorest-1.0.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml`

 * *Files identical despite different names*

### Comparing `phlorest-0.2.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl` & `phlorest-1.0.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl`

 * *Files identical despite different names*

### Comparing `phlorest-0.2.0/src/phlorest/phlorest_template/setup.py_tmpl` & `phlorest-1.0.0/src/phlorest/phlorest_template/setup.py_tmpl`

 * *Files identical despite different names*

### Comparing `phlorest-0.2.0/src/phlorest.egg-info/PKG-INFO` & `phlorest-1.0.0/src/phlorest.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,105 @@
 Metadata-Version: 2.1
 Name: phlorest
-Version: 0.2.0
+Version: 1.0.0
 Summary: A cldfbench plugin to curate language phylogenies
 Home-page: https://github.com/phlorest/phlorest
 Author: Simon Greenhill and Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/phlorest/phlorest/issues
-Description: # phlorest
-        
-        A [cldfbench](https://github.com/cldf/cldfbench) plugin to curate language phylogenies.
-        
-        
-        ## Install
-        
-        ```shell
-        pip install phlorest
-        ```
-        
-        
-        ## Usage
-        
-        ### Bootstrapping a `phlorest`-curated dataset
-        
-        `phlorest` provides a `cldfbench` dataset template to create the skeleton of files and directories for a
-        `phlorest`-curated dataset, to be run with [cldfbench new](https://github.com/cldf/cldfbench/#creating-a-skeleton-for-a-new-dataset-directory).
-        
-        Running
-        
-        ```shell
-        cldfbench new --template phlorest 
-        ```
-        
-        will create a dataset skeleton looking as follows
-        ```shell
-        $ tree testtree/
-        testtree/
-        ├── cldf
-        │   └── README.md
-        ├── cldfbench_testtree.py
-        ├── etc
-        │   ├── characters.csv
-        │   └── taxa.csv
-        ├── metadata.json
-        ├── raw
-        │   └── README.md
-        ├── setup.cfg
-        ├── setup.py
-        └── test.py
-        ```
-        
-        
-        ### Implementng CLDF creation
-        
-        Implementing CLDF creation means - as for any other `cldfbench`-curated dataset - filling in the
-        `cmd_makecldf` method of the `Dataset` subclass in `cldfbench_<id>.py`.
-        
-        The CLDF writer which can be accessed as `args.writer` within `cmd_makecldf` is an instance of
-        `phlorest.CLDFWriter`, which has convenience methods to add summary- or posterior trees to the CLDF
-        dataset. At least a summary is needed to make a dataset valid. Adding one looks as follows
-        
-        ```python
-            args.writer.add_summary(
-                self.raw_dir.read_tree(...),
-                self.metadata,
-                args.log)
-        ```
-        
-        
-        ### Running CLDF creation
-        
-        With `cmd_makecldf` implemented, CLDF creation can be triggered running
-        ```shell
-        cldfbench makecldf cldfbench_<id>.py
-        ```
-        
-        The resulting CLDF dataset can be validated running
-        ```shell
-        pytest
-        ```
-        
 Keywords: cldf
 Platform: any
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# phlorest
+
+A [cldfbench](https://github.com/cldf/cldfbench) plugin to curate language phylogenies.
+
+
+## Install
+
+```shell
+pip install phlorest
+```
+
+
+## Usage
+
+### Bootstrapping a `phlorest`-curated dataset
+
+`phlorest` provides a `cldfbench` dataset template to create the skeleton of files and directories for a
+`phlorest`-curated dataset, to be run with [cldfbench new](https://github.com/cldf/cldfbench/#creating-a-skeleton-for-a-new-dataset-directory).
+
+Running
+
+```shell
+cldfbench new --template phlorest 
+```
+
+will create a dataset skeleton looking as follows
+```shell
+$ tree testtree/
+testtree/
+├── cldf
+│   └── README.md
+├── cldfbench_testtree.py
+├── etc
+│   ├── characters.csv
+│   └── taxa.csv
+├── metadata.json
+├── raw
+│   └── README.md
+├── setup.cfg
+├── setup.py
+└── test.py
+```
+
+
+### Implementing CLDF creation
+
+Implementing CLDF creation means - as for any other `cldfbench`-curated dataset - filling in the
+`cmd_makecldf` method of the `Dataset` subclass in `cldfbench_<id>.py`.
+
+The CLDF writer which can be accessed as `args.writer` within `cmd_makecldf` is an instance of
+`phlorest.CLDFWriter`, which has convenience methods to add summary- or posterior trees to the CLDF
+dataset. At least a summary is needed to make a dataset valid. Adding one looks as follows
+
+```python
+    args.writer.add_summary(
+        self.raw_dir.read_tree(...),
+        self.metadata,
+        args.log)
+```
+
+
+### Running CLDF creation
+
+With `cmd_makecldf` implemented, CLDF creation can be triggered running
+```shell
+cldfbench makecldf cldfbench_<id>.py
+```
+
+The resulting CLDF dataset can be validated running
+```shell
+pytest
+```
+
+
+## Dependencies
+
+The `run_treeannotator` method of `Dataset` requires the `treeannotator` command from BEAST to be
+installed. For details on how to install `treeannotator` (and `BEAST`), see https://beast.community/index.html
```

### Comparing `phlorest-0.2.0/src/phlorest.egg-info/SOURCES.txt` & `phlorest-1.0.0/src/phlorest.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,15 @@
 src/phlorest/commands/check.py
 src/phlorest/commands/merge_characters.py
 src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl
 src/phlorest/phlorest_template/setup.cfg
 src/phlorest/phlorest_template/setup.py_tmpl
 src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml
 src/phlorest/phlorest_template/etc/characters.csv
-src/phlorest/phlorest_template/etc/taxa.csv
+src/phlorest/phlorest_template/etc/taxa.csv
+tests/test_beast.py
+tests/test_cldfwriter.py
+tests/test_cli.py
+tests/test_dataset.py
+tests/test_metadata.py
+tests/test_nexuslib.py
+tests/test_scaffold.py
```

