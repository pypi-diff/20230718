# Comparing `tmp/fuisce-1.0.0.tar.gz` & `tmp/fuisce-1.0.1.tar.gz`

## Comparing `fuisce-1.0.0.tar` & `fuisce-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fuisce-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 fuisce-1.0.0/Makefile
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fuisce-1.0.0/README.md -> docs/source/README.md
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fuisce-1.0.0/_vimrc_local.vim
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fuisce-1.0.0/config.mk
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fuisce-1.0.0/requirements.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fuisce-1.0.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fuisce-1.0.0/docs/make.bat
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 fuisce-1.0.0/docs/source/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 fuisce-1.0.0/docs/source/conf.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fuisce-1.0.0/docs/source/index.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/_version.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/database/__init__.py
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/database/interface.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/testing/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/testing/config.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 fuisce-1.0.0/src/fuisce/testing/manager.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fuisce-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fuisce-1.0.0/tests/database/test_interface.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 fuisce-1.0.0/tests/helpers/testing_helpers.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fuisce-1.0.0/tests/testing/test_manager.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 fuisce-1.0.0/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 fuisce-1.0.0/COPYING
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fuisce-1.0.0/LICENSE
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 fuisce-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 fuisce-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 fuisce-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 fuisce-1.0.1/Makefile
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fuisce-1.0.1/README.md -> docs/source/README.md
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fuisce-1.0.1/_vimrc_local.vim
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fuisce-1.0.1/config.mk
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fuisce-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fuisce-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fuisce-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 fuisce-1.0.1/docs/source/README.md
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 fuisce-1.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fuisce-1.0.1/docs/source/index.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/_version.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/database/__init__.py
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/database/interface.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/testing/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/testing/config.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 fuisce-1.0.1/src/fuisce/testing/manager.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 fuisce-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fuisce-1.0.1/tests/database/test_interface.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 fuisce-1.0.1/tests/helpers/testing_helpers.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fuisce-1.0.1/tests/testing/test_manager.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 fuisce-1.0.1/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 fuisce-1.0.1/COPYING
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fuisce-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 fuisce-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 fuisce-1.0.1/PKG-INFO
```

### Comparing `fuisce-1.0.0/Makefile` & `fuisce-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/config.mk` & `fuisce-1.0.1/config.mk`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/docs/Makefile` & `fuisce-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/docs/make.bat` & `fuisce-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/docs/source/README.md` & `fuisce-1.0.1/docs/source/README.md`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/docs/source/conf.py` & `fuisce-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/src/fuisce/database/interface.py` & `fuisce-1.0.1/src/fuisce/database/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 """
 An interface for connecting to and working with the SQLite database.
 """
 import functools
 
 from flask import current_app
-from sqlalchemy import MetaData, create_engine, event
+from sqlalchemy import MetaData, URL, create_engine, event
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import DeclarativeBase, scoped_session, sessionmaker
 
 DIALECT = "sqlite"
 DBAPI = "pysqlite"
 
 
 class SQLAlchemy:
-    """Store an interface to SQLAlchemy database objects."""
+    """
+    Store an interface to SQLAlchemy database objects.
+
+    This creates, stores, and manages an interface to work with
+    SQLAlchemy objects. At the class level, it stores a reference to
+    the current database metadata and a reference to the currently
+    active interface instance. That instance can be used to set up
+    the database engine and tables with consistent parameters, open
+    and close sessions, as well as select an interface instance to use.
+    Most often, this interface instance will be the default interface
+    defined by an application; however, when testing, this may be a
+    new interface used for only a subset of tests.
+
+    Parameters
+    ----------
+    echo_engine : bool
+        A flag passed to the interface's engine indicating if output
+        should be echoed. The default is `False`.
+    """
 
     metadata = MetaData()
     default_interface = None
 
     def __init__(self, echo_engine=False):
         self.engine = None
         self.scoped_session = None
@@ -38,16 +56,17 @@
 
         Parameters
         ----------
         db_path : os.PathLike
             The path to the local database.
         """
         echo_engine = self.echo_engine if echo_engine is None else echo_engine
-        # Create the engine using the custom database URL
-        db_url = f"{DIALECT}+{DBAPI}:///{db_path}"
+        # Create the engine using the customodatabase URL
+        db_url = URL.create(drivername=f"{DIALECT}+{DBAPI}", database=db_path)
+        #db_url = f"{DIALECT}+{DBAPI}:///{db_path}"
         self.engine = create_engine(db_url, echo=echo_engine)
         # Use a session factory to generate sessions
         session_factory = sessionmaker(
             bind=self.engine,
             autoflush=False,
             future=True,
         )
@@ -119,16 +138,16 @@
                         "A default database interface has not yet been defined. "
                         "Define a default interface for all apps running in "
                         "production or development mode."
                     )
                 app.db = cls.default_interface
             else:
                 app.db = cls(
-                    *app.config["DATABASE_INTERFACE_ARGS"],
-                    **app.config["DATABASE_INTERFACE_KWARGS"],
+                    *app.config.get("DATABASE_INTERFACE_ARGS", []),
+                    **app.config.get("DATABASE_INTERFACE_KWARGS", {}),
                 )
             app.db.setup_engine(db_path=app.config["DATABASE"])
             init_app_func(app)
             # Establish behavior for closing the database
             app.teardown_appcontext(app.db.close)
             # If testing, the database still needs to be initialized/prepopulated
             # (otherwise, database initialization is typically executed via the CLI)
```

### Comparing `fuisce-1.0.0/src/fuisce/testing/manager.py` & `fuisce-1.0.1/src/fuisce/testing/manager.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/tests/conftest.py` & `fuisce-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/tests/database/test_interface.py` & `fuisce-1.0.1/tests/database/test_interface.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/tests/helpers/testing_helpers.py` & `fuisce-1.0.1/tests/helpers/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/tests/testing/test_manager.py` & `fuisce-1.0.1/tests/testing/test_manager.py`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/.gitignore` & `fuisce-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/COPYING` & `fuisce-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/pyproject.toml` & `fuisce-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fuisce-1.0.0/PKG-INFO` & `fuisce-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuisce
-Version: 1.0.0
+Version: 1.0.1
 Summary: Database management and testing for SQLAlchemy-based Flask apps.
 Project-URL: Download, https://pypi.org/project/fuisce
 Project-URL: Homepage, https://github.com/mitchnegus/fuisce
 Project-URL: Repository, https://github.com/mitchnegus/fuisce
 Project-URL: Changelog, https://github.com/mitchnegus/fuisce/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
```

