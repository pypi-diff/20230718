# Comparing `tmp/fuisce-1.0.1.tar.gz` & `tmp/fuisce-1.0.2.tar.gz`

## Comparing `fuisce-1.0.1.tar` & `fuisce-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 fuisce-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 fuisce-1.0.1/Makefile
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fuisce-1.0.1/README.md -> docs/source/README.md
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fuisce-1.0.1/_vimrc_local.vim
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fuisce-1.0.1/config.mk
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fuisce-1.0.1/requirements.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fuisce-1.0.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fuisce-1.0.1/docs/make.bat
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 fuisce-1.0.1/docs/source/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 fuisce-1.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fuisce-1.0.1/docs/source/index.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/_version.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/database/__init__.py
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/database/interface.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/testing/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/testing/config.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/testing/manager.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fuisce-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fuisce-1.0.1/tests/database/test_interface.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 fuisce-1.0.1/tests/helpers/testing_helpers.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fuisce-1.0.1/tests/testing/test_manager.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 fuisce-1.0.1/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 fuisce-1.0.1/COPYING
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fuisce-1.0.1/LICENSE
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 fuisce-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 fuisce-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 fuisce-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 fuisce-1.0.2/Makefile
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fuisce-1.0.2/README.md -> docs/source/README.md
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fuisce-1.0.2/_vimrc_local.vim
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fuisce-1.0.2/config.mk
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fuisce-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fuisce-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fuisce-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 fuisce-1.0.2/docs/source/README.md
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 fuisce-1.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fuisce-1.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fuisce-1.0.2/src/fuisce/_version.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fuisce-1.0.2/src/fuisce/database/__init__.py
+-rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 fuisce-1.0.2/src/fuisce/database/interface.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fuisce-1.0.2/src/fuisce/testing/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 fuisce-1.0.2/src/fuisce/testing/config.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 fuisce-1.0.2/src/fuisce/testing/manager.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fuisce-1.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fuisce-1.0.2/tests/database/test_interface.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 fuisce-1.0.2/tests/helpers/testing_helpers.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fuisce-1.0.2/tests/testing/test_manager.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 fuisce-1.0.2/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 fuisce-1.0.2/COPYING
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fuisce-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 fuisce-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 fuisce-1.0.2/PKG-INFO
```

### Comparing `fuisce-1.0.1/Makefile` & `fuisce-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/config.mk` & `fuisce-1.0.2/config.mk`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/docs/Makefile` & `fuisce-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/docs/make.bat` & `fuisce-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/docs/source/README.md` & `fuisce-1.0.2/docs/source/README.md`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/docs/source/conf.py` & `fuisce-1.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/docs/source/index.rst` & `fuisce-1.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/src/fuisce/database/interface.py` & `fuisce-1.0.2/src/fuisce/database/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         Parameters
         ----------
         db_path : os.PathLike
             The path to the local database.
         """
         echo_engine = self.echo_engine if echo_engine is None else echo_engine
         # Create the engine using the customodatabase URL
-        db_url = URL.create(drivername=f"{DIALECT}+{DBAPI}", database=db_path)
+        db_url = URL.create(drivername=f"{DIALECT}+{DBAPI}", database=str(db_path))
         #db_url = f"{DIALECT}+{DBAPI}:///{db_path}"
         self.engine = create_engine(db_url, echo=echo_engine)
         # Use a session factory to generate sessions
         session_factory = sessionmaker(
             bind=self.engine,
             autoflush=False,
             future=True,
```

### Comparing `fuisce-1.0.1/src/fuisce/testing/manager.py` & `fuisce-1.0.2/src/fuisce/testing/manager.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/tests/conftest.py` & `fuisce-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/tests/database/test_interface.py` & `fuisce-1.0.2/tests/database/test_interface.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/tests/helpers/testing_helpers.py` & `fuisce-1.0.2/tests/helpers/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/tests/testing/test_manager.py` & `fuisce-1.0.2/tests/testing/test_manager.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/.gitignore` & `fuisce-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/COPYING` & `fuisce-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/pyproject.toml` & `fuisce-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.1/PKG-INFO` & `fuisce-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuisce
-Version: 1.0.1
+Version: 1.0.2
 Summary: Database management and testing for SQLAlchemy-based Flask apps.
 Project-URL: Download, https://pypi.org/project/fuisce
 Project-URL: Homepage, https://github.com/mitchnegus/fuisce
 Project-URL: Repository, https://github.com/mitchnegus/fuisce
 Project-URL: Changelog, https://github.com/mitchnegus/fuisce/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
```

