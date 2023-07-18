# Comparing `tmp/firebirdsql_run-1.0.5.tar.gz` & `tmp/firebirdsql_run-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebirdsql_run-1.0.5.tar", max compression
+gzip compressed data, was "firebirdsql_run-1.0.6.tar", max compression
```

## Comparing `firebirdsql_run-1.0.5.tar` & `firebirdsql_run-1.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/LICENSE
--rw-r--r--   0        0        0     2152 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/README.md
--rw-r--r--   0        0        0     2295 2023-07-08 11:19:00.471922 firebirdsql_run-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      241 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/src/firebirdsql_run/__init__.py
--rw-r--r--   0        0        0     2807 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/src/firebirdsql_run/main.py
--rw-r--r--   0        0        0      521 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/src/firebirdsql_run/type.py
--rw-r--r--   0        0        0      357 2023-07-08 11:18:43.999279 firebirdsql_run-1.0.5/src/firebirdsql_run/util.py
--rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-18 19:22:29.750702 firebirdsql_run-1.0.6/LICENSE
+-rw-r--r--   0        0        0     2152 2023-07-18 19:22:29.750702 firebirdsql_run-1.0.6/README.md
+-rw-r--r--   0        0        0     2362 2023-07-18 19:22:45.546707 firebirdsql_run-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      241 2023-07-18 19:22:29.754701 firebirdsql_run-1.0.6/src/firebirdsql_run/__init__.py
+-rw-r--r--   0        0        0     2807 2023-07-18 19:22:29.754701 firebirdsql_run-1.0.6/src/firebirdsql_run/main.py
+-rw-r--r--   0        0        0      521 2023-07-18 19:22:29.754701 firebirdsql_run-1.0.6/src/firebirdsql_run/type.py
+-rw-r--r--   0        0        0      357 2023-07-18 19:22:29.754701 firebirdsql_run-1.0.6/src/firebirdsql_run/util.py
+-rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 firebirdsql_run-1.0.6/PKG-INFO
```

### Comparing `firebirdsql_run-1.0.5/LICENSE` & `firebirdsql_run-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `firebirdsql_run-1.0.5/README.md` & `firebirdsql_run-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `firebirdsql_run-1.0.5/pyproject.toml` & `firebirdsql_run-1.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,62 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "firebirdsql-run"
-version = "1.0.5"
+version = "1.0.6"
 description = "Firebirdsql wrapper inspired by subprocess.run"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/firebirdsql-run"
 repository = "https://github.com/DeadNews/firebirdsql-run"
 keywords = ["firebird", "sql", "api"]
 classifiers = ["Operating System :: OS Independent", "Topic :: Database"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 firebirdsql = "^1.2.2"
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.3.0"
+black = "^23.7.0"
 mypy = "^1.4.1"
-poethepoet = "^0.20.0"
-ruff = "^0.0.275"
+poethepoet = "^0.21.1"
+ruff = "^0.0.278"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+
 [tool.poe.tasks]
 ruff = "ruff check ."
 black = "black --check ."
 mypy = "mypy ."
 lint.sequence = ["ruff", "black", "mypy"]
 
-[tool.poetry-dynamic-versioning]
-enable = false
-vcs = "git"
-style = "semver"
+[tool.poe.tasks.test]
+cmd = "pytest --cov-report=xml"
+
+[tool.pytest.ini_options]
+addopts = "--verbose --cov=./src --cov-report=term"
+testpaths = ["tests"]
+markers = ["docker", "online"]
+
+[tool.coverage.report]
+exclude_lines = [
+  "# pragma: no cover",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
 
 [tool.black]
 line-length = 99
 
 [tool.mypy]
 disallow_untyped_defs = true
 follow_imports = "silent"
@@ -50,26 +65,14 @@
 show_error_codes = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 allow_untyped_defs = true
 
-[tool.pytest.ini_options]
-addopts = "--verbose --cov=./src"
-testpaths = ["tests"]
-markers = ["docker", "key_required"]
-
-[tool.coverage.report]
-exclude_lines = [
-  "# pragma: no cover",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
-
 [tool.ruff]
 line-length = 99
 select = ["ALL"]
 ignore = [
   "COM812",  # Trailing comma missing
   "D203",    # 1 blank line required before class docstring
   "D212",    # Multi-line docstring summary should start at the first line
```

### Comparing `firebirdsql_run-1.0.5/src/firebirdsql_run/main.py` & `firebirdsql_run-1.0.6/src/firebirdsql_run/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from firebirdsql_run.type import CompletedTransaction
 from firebirdsql_run.util import get_env
 
 
 def connection(
     db: Path | str,
-    host: str = "localhost",
+    host: str = "127.0.0.1",
     port: int = 3050,
     user: str = "TWUSER",
     passwd: str | None = None,
 ) -> Connection:
     """Create a connection to the database."""
     return connect(
         host=getfqdn(host),
@@ -26,15 +26,15 @@
     )
 
 
 def execute(
     query: str,
     params: tuple = (),
     db: Path | str = "",
-    host: str = "localhost",
+    host: str = "127.0.0.1",
     port: int = 3050,
     user: str = "TWUSER",
     passwd: str | None = None,
     use_conn: Connection | None = None,
 ) -> CompletedTransaction:
     """
     Execute transaction.
@@ -84,15 +84,15 @@
     )
 
 
 def callproc(
     procname: str,
     params: tuple = (),
     db: Path | str = "",
-    host: str = "localhost",
+    host: str = "127.0.0.1",
     port: int = 3050,
     user: str = "TWUSER",
     passwd: str | None = None,
     use_conn: Connection | None = None,
 ) -> CompletedTransaction:
     """Execute procedure with params."""
     query = f"EXECUTE PROCEDURE {procname} " + ",".join("?" * len(params))
```

### Comparing `firebirdsql_run-1.0.5/src/firebirdsql_run/type.py` & `firebirdsql_run-1.0.6/src/firebirdsql_run/type.py`

 * *Files identical despite different names*

### Comparing `firebirdsql_run-1.0.5/PKG-INFO` & `firebirdsql_run-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebirdsql-run
-Version: 1.0.5
+Version: 1.0.6
 Summary: Firebirdsql wrapper inspired by subprocess.run
 Home-page: https://github.com/DeadNews/firebirdsql-run
 License: MIT
 Keywords: firebird,sql,api
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
```

