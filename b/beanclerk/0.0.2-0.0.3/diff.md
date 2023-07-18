# Comparing `tmp/beanclerk-0.0.2.tar.gz` & `tmp/beanclerk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanclerk-0.0.2.tar", last modified: Thu Jul 13 15:01:01 2023, max compression
+gzip compressed data, was "beanclerk-0.0.3.tar", last modified: Tue Jul 18 15:21:23 2023, max compression
```

## Comparing `beanclerk-0.0.2.tar` & `beanclerk-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:01:01.580780 beanclerk-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-07-13 15:00:47.000000 beanclerk-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-07-13 15:01:01.580780 beanclerk-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 15:00:47.000000 beanclerk-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:01:01.576780 beanclerk-0.0.2/beanclerk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/bean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/clerk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:01:01.580780 beanclerk-0.0.2/beanclerk/importers/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/importers/banka_creditas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-13 15:00:47.000000 beanclerk-0.0.2/beanclerk/importers/fio_banka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:01:01.580780 beanclerk-0.0.2/beanclerk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 15:01:01.000000 beanclerk-0.0.2/beanclerk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-13 15:00:47.000000 beanclerk-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:01:01.580780 beanclerk-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:23.964979 beanclerk-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-07-18 15:21:10.000000 beanclerk-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-07-18 15:21:23.964979 beanclerk-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-18 15:21:10.000000 beanclerk-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:23.960979 beanclerk-0.0.3/beanclerk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/bean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/clerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:23.964979 beanclerk-0.0.3/beanclerk/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/importers/banka_creditas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-18 15:21:10.000000 beanclerk-0.0.3/beanclerk/importers/fio_banka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:23.960979 beanclerk-0.0.3/beanclerk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:21:23.000000 beanclerk-0.0.3/beanclerk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-18 15:21:10.000000 beanclerk-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:21:23.964979 beanclerk-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:21:23.964979 beanclerk-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-18 15:21:10.000000 beanclerk-0.0.3/tests/test_clerk.py
```

### Comparing `beanclerk-0.0.2/LICENSE` & `beanclerk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.2/PKG-INFO` & `beanclerk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: beanclerk
-Version: 0.0.2
-Summary: Additional automation for Beancount
+Version: 0.0.3
+Summary: Automation for Beancount
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
          Everyone is permitted to copy and distribute verbatim copies
@@ -348,15 +348,15 @@
         
         Note:
         This is a GNU GPL "v2 only" license.
         This is not a GNU GPL "v2 or any later version" license.
                                           ---Martin Blais (the author of Beancount)
         
 Keywords: accounting,finance,beancount,automation,API
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `beanclerk-0.0.2/README.md` & `beanclerk-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.2/beanclerk/bean_helpers.py` & `beanclerk-0.0.3/beanclerk/bean_helpers.py`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.2/beanclerk/cli.py` & `beanclerk-0.0.3/beanclerk/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 def cli(ctx: click.Context, config_file: Path) -> None:
     """Additional automation for Beancount."""
     # https://click.palletsprojects.com/en/8.1.x/commands/#nested-handling-and-contexts
     ctx.ensure_object(dict)
     ctx.obj["config_file"] = config_file
 
 
+# TODO: simplify by subclassing click.DateTime?
 class Date(click.ParamType):
-    """A custom date type for click.
+    """A convenience date type for Click.
 
-    click.DateTime is not convenient because it converts a date into a datetime.
+    Converts dates to a date instead of datetime.
     """
 
     name = "date"
 
     def convert(self, value, param, ctx):
         if isinstance(value, date):
             return value
@@ -49,19 +50,19 @@
 
 @cli.command("import")
 @click.option("--from-date", type=Date(), help="The first date to import (YYYY-MM-DD).")
 @click.option("--to-date", type=Date(), help="The last date to import (YYYY-MM-DD).")
 @click.pass_context
 def import_(
     ctx: click.Context,
-    from_date: click.DateTime,
-    to_date: click.DateTime,
+    from_date: click.DateTime,  # FIXME: use Date() instead
+    to_date: click.DateTime,  # FIXME: use Date() instead
 ) -> None:
     """Import transactions from configured importers."""
     try:
         import_transactions(
-            configfile=ctx.obj["config_file"],
+            config_file=ctx.obj["config_file"],
             from_date=from_date,
             to_date=to_date,
         )
     except BeanclerkError as exc:
         raise click.ClickException(str(exc)) from exc
```

### Comparing `beanclerk-0.0.2/beanclerk/importers/__init__.py` & `beanclerk-0.0.3/beanclerk/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.2/beanclerk/importers/banka_creditas.py` & `beanclerk-0.0.3/beanclerk/importers/banka_creditas.py`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.2/beanclerk/importers/fio_banka.py` & `beanclerk-0.0.3/beanclerk/importers/fio_banka.py`

 * *Files identical despite different names*

### Comparing `beanclerk-0.0.2/beanclerk.egg-info/PKG-INFO` & `beanclerk-0.0.3/beanclerk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: beanclerk
-Version: 0.0.2
-Summary: Additional automation for Beancount
+Version: 0.0.3
+Summary: Automation for Beancount
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
          Everyone is permitted to copy and distribute verbatim copies
@@ -348,15 +348,15 @@
         
         Note:
         This is a GNU GPL "v2 only" license.
         This is not a GNU GPL "v2 or any later version" license.
                                           ---Martin Blais (the author of Beancount)
         
 Keywords: accounting,finance,beancount,automation,API
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Accounting
```

### Comparing `beanclerk-0.0.2/pyproject.toml` & `beanclerk-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "beanclerk"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name = "Petr Beranek", email = "petrberanek.mail@gmail.com" },
 ]
 license = {file = "LICENSE"}
-description = "Additional automation for Beancount"
+description = "Automation for Beancount"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["accounting", "finance", "beancount", "automation", "API"]
 classifiers = [
-  "Development Status :: 2 - Pre-Alpha",
+  "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Intended Audience :: End Users/Desktop",
   "Intended Audience :: Information Technology",
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Operating System :: POSIX :: Linux",
   "Programming Language :: Python :: 3.11",
   "Topic :: Office/Business :: Financial :: Accounting",
 ]
 # Always sync with additional dependencies for Mypy in pyproject.toml
+# TODO: simplify dep definitions via '~=' syntax; sort
 dependencies = [
   "PyYAML>=6.0,<7",
   "beancount>=2.3.5,<3",
   "fio-banka>=1.0.3,<2",
   "creditas==1.0.0.*",
   "lxml>=4.9.2,<5",
   "click>=8.1.4,<9",
+  "pydantic>=2.0.3,<3",
+  "pydantic-settings>=2.0.2,<3",
+  "rich>=13.4.2,<14",
 ]
 
 [project.optional-dependencies]
 devel = [
   "pre-commit>=3.3.3,<4",
   "pytest>=7.4.0,<8",
 ]
 
 [project.scripts]
 bean-clerk = "beanclerk.cli:cli"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
+# TODO: Use https://docs.pydantic.dev/dev-v2/integrations/mypy/
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.ruff]
 # https://beta.ruff.rs/docs/rules/
 select = [
   "F",    # pyflakes
@@ -80,14 +85,15 @@
   "PTH",  # flake8-use-pathlib
   "PGH",  # pygrep-hooks
   "PL",   # pylint
   "TRY",  # tryceptors
   "FLY",  # flynt
   "RUF",  # Ruff-specific rules
 ]
+ignore = ["TRY003"]
 unfixable = [
   # These may break temporarily commented-out code
   "F401",
   "F841",
 ]
 
 [tool.ruff.per-file-ignores]
```

