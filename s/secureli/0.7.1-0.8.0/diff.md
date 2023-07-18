# Comparing `tmp/secureli-0.7.1.tar.gz` & `tmp/secureli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.7.1.tar", max compression
+gzip compressed data, was "secureli-0.8.0.tar", max compression
```

## Comparing `secureli-0.7.1.tar` & `secureli-0.8.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11343 2023-07-13 21:57:57.989070 secureli-0.7.1/LICENSE
--rw-r--r--   0        0        0    11614 2023-07-13 21:57:57.989070 secureli-0.7.1/README.md
--rw-r--r--   0        0        0     2043 2023-07-13 21:57:57.993070 secureli-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0     6906 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/actions/__init__.py
--rw-r--r--   0        0        0    11784 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10628 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/actions/update.py
--rw-r--r--   0        0        0     6450 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/main.py
--rw-r--r--   0        0        0        0 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     3632 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/__init__.py
--rw-r--r--   0        0        0      791 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/base-pre-commit.yaml
--rw-r--r--   0        0        0     4883 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/build.txt
--rw-r--r--   0        0        0       93 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/configs/javascript.config.yaml
--rw-r--r--   0        0        0      161 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/configs/typescript.config.yaml
--rw-r--r--   0        0        0      659 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      115 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/go-pre-commit.yaml
--rw-r--r--   0        0        0      130 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0      618 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/javascript-pre-commit.yaml
--rw-r--r--   0        0        0      367 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      232 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      228 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0      714 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0    12318 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/services/language_config.py
--rw-r--r--   0        0        0    18724 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/services/language_support.py
--rw-r--r--   0        0        0     4470 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3048 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0      254 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/utilities/hash.py
--rw-r--r--   0        0        0     1372 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0     1028 2023-07-13 21:57:57.993070 secureli-0.7.1/secureli/utilities/usage_stats.py
--rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-07-18 20:02:34.146263 secureli-0.8.0/LICENSE
+-rw-r--r--   0        0        0    11614 2023-07-18 20:02:34.146263 secureli-0.8.0/README.md
+-rw-r--r--   0        0        0     2070 2023-07-18 20:02:34.150263 secureli-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0     6906 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    11784 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10628 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/update.py
+-rw-r--r--   0        0        0     6450 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     3632 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/__init__.py
+-rw-r--r--   0        0        0      791 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/base-pre-commit.yaml
+-rw-r--r--   0        0        0     4883 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0       93 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/configs/javascript.config.yaml
+-rw-r--r--   0        0        0      161 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/configs/typescript.config.yaml
+-rw-r--r--   0        0        0      659 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      115 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/go-pre-commit.yaml
+-rw-r--r--   0        0        0      130 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0      618 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/javascript-pre-commit.yaml
+-rw-r--r--   0        0        0      367 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      232 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      228 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0      714 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0    12318 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/language_config.py
+-rw-r--r--   0        0        0    18724 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4470 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3048 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0      254 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/hash.py
+-rw-r--r--   0        0        0     1372 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0     1028 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    12526 1970-01-01 00:00:00.000000 secureli-0.8.0/PKG-INFO
```

### Comparing `secureli-0.7.1/LICENSE` & `secureli-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/README.md` & `secureli-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/pyproject.toml` & `secureli-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.7.1"
+version = "0.8.0"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
@@ -32,26 +32,27 @@
 dependency-injector = {version = "^4.40.0", extras = ["yaml"]}
 pydantic = "^1.10.2"
 jinja2 = "^3.1.2"
 pathspec = ">=0.10.1,<0.12.0"
 cfgv = "^3.3.1"
 pre-commit = ">=2.20,<4.0"
 requests = "^2.31.0"
+pyyaml = ">=6.0.1"
 
 [tool.pytest.ini_options]
 addopts = "-p no:cacheprovider"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-mock = "^3.10.0"
 coverage = ">=6.5,<8.0"
 black = ">=22.10,<24.0"
 identify = "^2.5.7"
 poethepoet = ">=0.16.4,<0.22.0"
-python-semantic-release = "^7.33.1"
+python-semantic-release = ">=7.33.1,<9.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_toml = [
```

### Comparing `secureli-0.7.1/secureli/abstractions/echo.py` & `secureli-0.8.0/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/abstractions/lexer_guesser.py` & `secureli-0.8.0/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/abstractions/pre_commit.py` & `secureli-0.8.0/secureli/abstractions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/actions/action.py` & `secureli-0.8.0/secureli/actions/action.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/actions/build.py` & `secureli-0.8.0/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/actions/initializer.py` & `secureli-0.8.0/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/actions/scan.py` & `secureli-0.8.0/secureli/actions/scan.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/actions/setup.py` & `secureli-0.8.0/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/actions/update.py` & `secureli-0.8.0/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/container.py` & `secureli-0.8.0/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/main.py` & `secureli-0.8.0/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/repositories/repo_files.py` & `secureli-0.8.0/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/repositories/secureli_config.py` & `secureli-0.8.0/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/repositories/settings.py` & `secureli-0.8.0/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/resources/files/base-pre-commit.yaml` & `secureli-0.8.0/secureli/resources/files/base-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/resources/files/build.txt` & `secureli-0.8.0/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.8.0/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/resources/files/javascript-pre-commit.yaml` & `secureli-0.8.0/secureli/resources/files/javascript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.8.0/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/resources/read_resource.py` & `secureli-0.8.0/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/resources/slugify.py` & `secureli-0.8.0/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/services/git_ignore.py` & `secureli-0.8.0/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/services/language_analyzer.py` & `secureli-0.8.0/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/services/language_config.py` & `secureli-0.8.0/secureli/services/language_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/services/language_support.py` & `secureli-0.8.0/secureli/services/language_support.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/services/logging.py` & `secureli-0.8.0/secureli/services/logging.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/services/scanner.py` & `secureli-0.8.0/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/services/secureli_ignore.py` & `secureli-0.8.0/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/services/updater.py` & `secureli-0.8.0/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/settings.py` & `secureli-0.8.0/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/utilities/git_meta.py` & `secureli-0.8.0/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/utilities/patterns.py` & `secureli-0.8.0/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/secureli/utilities/usage_stats.py` & `secureli-0.8.0/secureli/utilities/usage_stats.py`

 * *Files identical despite different names*

### Comparing `secureli-0.7.1/PKG-INFO` & `secureli-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.7.1
+Version: 0.8.0
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Requires-Dist: cfgv (>=3.3.1,<4.0.0)
 Requires-Dist: dependency-injector[yaml] (>=4.40.0,<5.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pathspec (>=0.10.1,<0.12.0)
 Requires-Dist: pre-commit (>=2.20,<4.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.6.1,<0.10.0)
 Description-Content-Type: text/markdown
 
 [![SeCureLI Logo](https://repository-images.githubusercontent.com/606206029/aa43fa10-689b-4f8a-a6dc-2e9ed06d9e2d)](https://github.com/slalombuild/secureli)
 
 <h1 align="center">SeCureLI</h1>
```

