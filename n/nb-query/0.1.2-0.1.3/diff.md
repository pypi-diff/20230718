# Comparing `tmp/nb_query-0.1.2.tar.gz` & `tmp/nb_query-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_query-0.1.2.tar", max compression
+gzip compressed data, was "nb_query-0.1.3.tar", max compression
```

## Comparing `nb_query-0.1.2.tar` & `nb_query-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2022-12-18 11:13:36.050143 nb_query-0.1.2/LICENSE
--rw-r--r--   0        0        0      950 2022-12-18 11:13:36.050143 nb_query-0.1.2/README.md
--rw-r--r--   0        0        0      183 2022-12-18 11:13:36.050143 nb_query-0.1.2/nb_query/__init__.py
--rw-r--r--   0        0        0     2581 2022-12-18 11:13:36.050143 nb_query-0.1.2/nb_query/main.py
--rw-r--r--   0        0        0     1259 2022-12-18 11:13:36.050143 nb_query-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 nb_query-0.1.2/setup.py
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 nb_query-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-18 14:58:24.061355 nb_query-0.1.3/LICENSE
+-rw-r--r--   0        0        0      950 2023-07-18 14:58:24.061355 nb_query-0.1.3/README.md
+-rw-r--r--   0        0        0      183 2023-07-18 14:58:24.061355 nb_query-0.1.3/nb_query/__init__.py
+-rw-r--r--   0        0        0     2581 2023-07-18 14:58:24.061355 nb_query-0.1.3/nb_query/main.py
+-rw-r--r--   0        0        0     1260 2023-07-18 14:58:24.061355 nb_query-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 nb_query-0.1.3/setup.py
+-rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 nb_query-0.1.3/PKG-INFO
```

### Comparing `nb_query-0.1.2/LICENSE` & `nb_query-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_query-0.1.2/README.md` & `nb_query-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nb_query-0.1.2/nb_query/main.py` & `nb_query-0.1.3/nb_query/main.py`

 * *Files identical despite different names*

### Comparing `nb_query-0.1.2/pyproject.toml` & `nb_query-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = 'nb-query'
-version = "0.1.2"
+version = "0.1.3"
 description = 'Python package to search in jupyter notebooks'
 authors = ['Laszlo Sragner <sragner@gmail.com>']
 license = 'MIT'
 homepage = 'https://github.com/xLaszlo/nb-query'
 repository = 'https://github.com/xLaszlo/nb-query'
 readme = 'README.md'
 packages = [{include = 'nb_query'}]
 documentation = "https://nb-query.readthedocs.io"
 
 [tool.poetry.scripts]
 nb-query = 'nb_query.main:app'
 
 [tool.poetry.dependencies]
-python = '^3.8.1'
+python = '~3.11'
 typer = {extras = ['all'], version = '^0.7.0'}
-pandas = '^1.5.2'
+pandas = "^2.0.3"
+pre-commit = "^3.3.3"
 
 [tool.black]
 skip-string-normalization = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = '^7.2.0'
 coverage = {version = '^6.5.0', extras = ['toml']}
@@ -32,15 +33,14 @@
 flake8-import-order = '^0.18.2'
 mypy = "^0.991"
 flake8-annotations = "^2.9.1"
 flake8-docstrings = "^1.6.0"
 darglint = "^1.8.1"
 sphinx = "^5.3.0"
 sphinx-autodoc-typehints = "^1.19.5"
-codecov = "^2.1.12"
 
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.coverage.paths]
 source = ['nb_query', 'tests']
```

### Comparing `nb_query-0.1.2/setup.py` & `nb_query-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['nb_query']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pandas>=1.5.2,<2.0.0', 'typer[all]>=0.7.0,<0.8.0']
+['pandas>=2.0.3,<3.0.0', 'pre-commit>=3.3.3,<4.0.0', 'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['nb-query = nb_query.main:app']}
 
 setup_kwargs = {
     'name': 'nb-query',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Python package to search in jupyter notebooks',
     'long_description': '# nb_query\n\nPython package to search in Jupyter notebooks.\n\n[![Tests](https://github.com/xLaszlo/nb-query/workflows/Tests/badge.svg)](https://github.com/xLaszlo/nb-query/actions?workflow=Tests)\n[![Codecov](https://codecov.io/gh/xLaszlo/nb-query/branch/master/graph/badge.svg)](https://codecov.io/gh/xLaszlo/nb-query)\n[![PyPI](https://img.shields.io/pypi/v/nb-query.svg)](https://pypi.org/project/nb-query/)\n[![Read the Docs](https://readthedocs.org/projects/nb-query/badge/)](https://nb-query.readthedocs.io/)\n\nInstallation:\n\n```\n    $ pip install nb-query\n```\n\nUsage\n\n```\n    >>  from nb_query import nb_query\n    >>  nb_query(\'Hello\')\n    >>  nb_query(\'Hello\', [\'data/notebooks\',])\n    >>  nb_query(\'He(ll|r)o\')\n    >>  nb_query(lambda line: len(line) == 2)\n```\n\nCreated with the help of the "Hypermodern python" article series.\n\nJoin the [Code Quality for Data Science (CQ4ds) Discord channel](https://discord.com/invite/8uUZNMCad2) for feedback.\n',
     'author': 'Laszlo Sragner',
     'author_email': 'sragner@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/xLaszlo/nb-query',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<4.0.0',
+    'python_requires': '>=3.11,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `nb_query-0.1.2/PKG-INFO` & `nb_query-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: nb-query
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package to search in jupyter notebooks
 Home-page: https://github.com/xLaszlo/nb-query
 License: MIT
 Author: Laszlo Sragner
 Author-email: sragner@gmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://nb-query.readthedocs.io
 Project-URL: Repository, https://github.com/xLaszlo/nb-query
 Description-Content-Type: text/markdown
 
 # nb_query
```

