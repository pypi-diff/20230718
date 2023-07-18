# Comparing `tmp/pyqrlew-0.2.0.tar.gz` & `tmp/pyqrlew-0.2.1.tar.gz`

## Comparing `pyqrlew-0.2.0.tar` & `pyqrlew-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 pyqrlew-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123     4542 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3539 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/.gitignore
--rw-r--r--   0     1001      123      818 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/.readthedocs.yaml
--rw-r--r--   0     1001      123      655 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/CHANGELOG.md
--rw-r--r--   0     1001      123    11357 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/LICENSE
--rw-r--r--   0     1001      123     1466 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/README.md
--rw-r--r--   0     1001      123      634 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/Makefile
--rw-r--r--   0     1001      123     1212 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/conf.py
--rw-r--r--   0     1001      123      224 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/contributing.md
--rw-r--r--   0     1001      123     1786 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/index.md
--rw-r--r--   0     1001      123      800 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/make.bat
--rw-r--r--   0     1001      123       61 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/requirements.txt
--rw-r--r--   0     1001      123    49678 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/PyQrlew.ipynb
--rw-r--r--   0     1001      123   146621 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/demo.ipynb
--rw-r--r--   0     1001      123      431 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/retail_data/dataset.json
--rw-r--r--   0     1001      123     1032 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/retail_data/install_db.sql
--rw-r--r--   0     1001      123      234 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/retail_data/install_db_on_docker.sh
--rw-r--r--   0     1001      123    84990 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/retail_data/schema.json
--rw-r--r--   0     1001      123    11484 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/retail_data/size.json
--rw-r--r--   0     1001      123      133 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/requirements.txt
--rw-r--r--   0     1001      123      317 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/simple.py
--rw-r--r--   0     1001      123     1139 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123      112 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/python/pyqrlew/__init__.py
--rw-r--r--   0     1001      123       45 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/python/pyqrlew/io/__init__.py
--rw-r--r--   0     1001      123    10178 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/python/pyqrlew/io/database.py
--rw-r--r--   0     1001      123     2612 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/python/pyqrlew/io/postgresql.py
--rw-r--r--   0     1001      123    13493 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123      136 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/tests/conftest.py
--rw-r--r--   0     1001      123     2481 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/tests/queries/sql_unlimited_queries.sql
--rw-r--r--   0     1001      123     7054 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/tests/queries/valid_queries.sql
--rw-r--r--   0     1001      123      178 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/tests/requirements.txt
--rw-r--r--   0     1001      123     1399 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/tests/test_financial_dataset.py
--rw-r--r--   0     1001      123    45460 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pyqrlew-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 pyqrlew-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123     4542 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3539 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/.gitignore
+-rw-r--r--   0     1001      123      818 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/.readthedocs.yaml
+-rw-r--r--   0     1001      123      719 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/CHANGELOG.md
+-rw-r--r--   0     1001      123    11357 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/LICENSE
+-rw-r--r--   0     1001      123     1466 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/README.md
+-rw-r--r--   0     1001      123      634 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/Makefile
+-rw-r--r--   0     1001      123     1212 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/conf.py
+-rw-r--r--   0     1001      123      224 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/contributing.md
+-rw-r--r--   0     1001      123     1786 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/index.md
+-rw-r--r--   0     1001      123      800 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/make.bat
+-rw-r--r--   0     1001      123       61 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/docs/requirements.txt
+-rw-r--r--   0     1001      123    49678 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/PyQrlew.ipynb
+-rw-r--r--   0     1001      123   146621 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/demo.ipynb
+-rw-r--r--   0     1001      123      431 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/retail_data/dataset.json
+-rw-r--r--   0     1001      123     1032 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/retail_data/install_db.sql
+-rw-r--r--   0     1001      123      234 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/retail_data/install_db_on_docker.sh
+-rw-r--r--   0     1001      123    84990 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/retail_data/schema.json
+-rw-r--r--   0     1001      123    11484 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/demo/retail_data/size.json
+-rw-r--r--   0     1001      123      133 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/requirements.txt
+-rw-r--r--   0     1001      123      317 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/examples/simple.py
+-rw-r--r--   0     1001      123     1139 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123      112 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/python/pyqrlew/__init__.py
+-rw-r--r--   0     1001      123       45 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/python/pyqrlew/io/__init__.py
+-rw-r--r--   0     1001      123    10178 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/python/pyqrlew/io/database.py
+-rw-r--r--   0     1001      123     2612 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/python/pyqrlew/io/postgresql.py
+-rw-r--r--   0     1001      123    13493 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123      136 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/tests/conftest.py
+-rw-r--r--   0     1001      123     2481 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/tests/queries/sql_unlimited_queries.sql
+-rw-r--r--   0     1001      123     7054 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/tests/queries/valid_queries.sql
+-rw-r--r--   0     1001      123      178 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/tests/requirements.txt
+-rw-r--r--   0     1001      123     1399 2023-07-18 15:28:19.000000 pyqrlew-0.2.1/tests/test_financial_dataset.py
+-rw-r--r--   0     1001      123    45460 2023-07-18 15:28:28.000000 pyqrlew-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pyqrlew-0.2.1/PKG-INFO
```

### Comparing `pyqrlew-0.2.0/.github/workflows/CI.yml` & `pyqrlew-0.2.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/.gitignore` & `pyqrlew-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/.readthedocs.yaml` & `pyqrlew-0.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/CHANGELOG.md` & `pyqrlew-0.2.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.1] - 2023-07-18
+### Changed
+- Updated `qrlew-datasets`
+
 ## [0.2.0] - 2023-07-18
 ### Changed
 - Remove data and db from pyqrlew. They are now in the qrlew-dataset package.
 - The example notebook has been updated.
 
 ## [0.1.0] - 2023-07-11
```

### Comparing `pyqrlew-0.2.0/LICENSE` & `pyqrlew-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/README.md` & `pyqrlew-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/docs/Makefile` & `pyqrlew-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/docs/conf.py` & `pyqrlew-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/docs/index.md` & `pyqrlew-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/docs/make.bat` & `pyqrlew-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/examples/PyQrlew.ipynb` & `pyqrlew-0.2.1/examples/PyQrlew.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/examples/demo/demo.ipynb` & `pyqrlew-0.2.1/examples/demo/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/examples/demo/retail_data/install_db.sql` & `pyqrlew-0.2.1/examples/demo/retail_data/install_db.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/examples/demo/retail_data/schema.json` & `pyqrlew-0.2.1/examples/demo/retail_data/schema.json`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/examples/demo/retail_data/size.json` & `pyqrlew-0.2.1/examples/demo/retail_data/size.json`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/pyproject.toml` & `pyqrlew-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = [
   "SQLAlchemy ~= 2.0",
   "psycopg[binary, pool] ~= 3.0",
   "pymysql ~= 1.0",
-  "qrlew-datasets ~= 0.2.5",
+  "qrlew-datasets ~= 0.2.6",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest ~= 7.0",
   "mypy ~= 1.0",
 ]
```

### Comparing `pyqrlew-0.2.0/python/pyqrlew/io/database.py` & `pyqrlew-0.2.1/python/pyqrlew/io/database.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/python/pyqrlew/io/postgresql.py` & `pyqrlew-0.2.1/python/pyqrlew/io/postgresql.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/src/lib.rs` & `pyqrlew-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/tests/queries/sql_unlimited_queries.sql` & `pyqrlew-0.2.1/tests/queries/sql_unlimited_queries.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/tests/queries/valid_queries.sql` & `pyqrlew-0.2.1/tests/queries/valid_queries.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/tests/test_financial_dataset.py` & `pyqrlew-0.2.1/tests/test_financial_dataset.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.2.0/Cargo.lock` & `pyqrlew-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyqrlew"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "pyo3",
  "qrlew",
  "qrlew-sarus",
  "serde_json",
 ]
```

### Comparing `pyqrlew-0.2.0/PKG-INFO` & `pyqrlew-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyqrlew
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: SQLAlchemy ~= 2.0
 Requires-Dist: psycopg[binary, pool] ~= 3.0
 Requires-Dist: pymysql ~= 1.0
-Requires-Dist: qrlew-datasets ~= 0.2.5
+Requires-Dist: qrlew-datasets ~= 0.2.6
 Requires-Dist: pytest ~= 7.0; extra == 'test'
 Requires-Dist: mypy ~= 1.0; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: A library to manipulate SQL queries, designed with privacy application in mind.
 Keywords: SQL,Privecy,Differential Privacy,AST,Intermediate Representation,Rust
 Author-email: Nicolas Grislain <ng@sarus.tech>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/Qrlew/pyqrlew
-Project-URL: homepage, https://qrlew.github.io
 Project-URL: changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
+Project-URL: homepage, https://qrlew.github.io
 Project-URL: documentation, https://pyqrlew.readthedocs.io
 
 # [Qrlew](https://qrlew.github.io/) framework (by [Sarus](https://www.sarus.tech/))
 Open source SQL manipulation framework written in Rust
 
 ## What is [Qrlew](https://qrlew.github.io/)?
 [Qrlew](https://qrlew.github.io/) is an open source library that aims to parse and compile SQL queries into an Intermediate Representation (IR) that is well-suited for various rewriting tasks. Although it was originally designed for privacy-focused applications, it can be utilized for a wide range of purposes.
```

