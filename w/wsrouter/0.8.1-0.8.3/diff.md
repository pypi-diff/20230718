# Comparing `tmp/wsrouter-0.8.1.tar.gz` & `tmp/wsrouter-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsrouter-0.8.1.tar", max compression
+gzip compressed data, was "wsrouter-0.8.3.tar", max compression
```

## Comparing `wsrouter-0.8.1.tar` & `wsrouter-0.8.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2022-07-29 23:12:24.958584 wsrouter-0.8.1/LICENSE.txt
--rw-r--r--   0        0        0      355 2022-07-29 23:12:24.958584 wsrouter-0.8.1/README.md
--rw-r--r--   0        0        0     1219 2022-07-29 23:12:24.959584 wsrouter-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      392 2022-07-29 23:12:24.959584 wsrouter-0.8.1/wsrouter/__init__.py
--rw-r--r--   0        0        0     5519 2022-07-29 23:12:24.959584 wsrouter-0.8.1/wsrouter/cmd.py
--rw-r--r--   0        0        0     1366 2022-07-29 23:12:24.959584 wsrouter-0.8.1/wsrouter/message.py
--rw-r--r--   0        0        0     6260 2022-07-29 23:12:24.959584 wsrouter-0.8.1/wsrouter/router.py
--rw-r--r--   0        0        0     3670 2022-07-29 23:12:24.959584 wsrouter-0.8.1/wsrouter/static/websocket.js
--rw-r--r--   0        0        0     1259 2022-07-29 23:12:43.401433 wsrouter-0.8.1/setup.py
--rw-r--r--   0        0        0     1506 2022-07-29 23:12:43.401768 wsrouter-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-06-04 18:10:06.358926 wsrouter-0.8.3/LICENSE.txt
+-rw-r--r--   0        0        0      355 2022-07-29 22:54:32.147383 wsrouter-0.8.3/README.md
+-rw-r--r--   0        0        0     1225 2023-07-18 05:30:23.215361 wsrouter-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      392 2022-06-27 13:04:23.013489 wsrouter-0.8.3/wsrouter/__init__.py
+-rw-r--r--   0        0        0     5519 2022-06-27 09:47:27.663349 wsrouter-0.8.3/wsrouter/cmd.py
+-rw-r--r--   0        0        0     1366 2022-06-26 19:40:18.290599 wsrouter-0.8.3/wsrouter/message.py
+-rw-r--r--   0        0        0     6260 2022-06-26 18:50:19.290413 wsrouter-0.8.3/wsrouter/router.py
+-rw-r--r--   0        0        0     3670 2022-06-17 21:09:58.015655 wsrouter-0.8.3/wsrouter/static/websocket.js
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 wsrouter-0.8.3/setup.py
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 wsrouter-0.8.3/PKG-INFO
```

### Comparing `wsrouter-0.8.1/LICENSE.txt` & `wsrouter-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wsrouter-0.8.1/pyproject.toml` & `wsrouter-0.8.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wsrouter"
-version = "0.8.1"
+version = "0.8.3"
 description = "Starlette Shared WebSocket Endpoint"
 documentation = "https://selcouth.gitlab.io/wsrouter/"
 authors = ["David Morris <gypsysoftware@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/selcouth/wsrouter"
 readme = "README.md"
 classifiers = [
@@ -16,29 +16,31 @@
     "Environment :: Web Environment",
     "Operating System :: OS Independent",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-starlette = "^0.20.1"
-shortuuid = "^1.0.9"
-orjson = "^3.7.1"
-boltons = "^21.0.0"
+starlette = ">=0.20.1"
+shortuuid = ">=1.0.9"
+orjson = ">=3.7.1"
+boltons = ">=21.0.0"
 
-# Optional dependencies for documentation
-Sphinx = {version = "^5.1.1", optional = true}
-sphinx-immaterial = {version = "^0.8.1", optional = true}
+[tool.poetry.group.dev.dependencies]
+pytest = ">=7.1.2"
+pytest-asyncio = ">=0.18.3"
+pytest-cov = ">=3.0.0"
+requests = ">=2.27.1"
+coveralls = ">=3.3.1"
+httpx = ">=0.24.1"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-pytest-asyncio = "^0.18.3"
-pytest-cov = "^3.0.0"
-requests = "^2.27.1"
-coveralls = "^3.3.1"
+[tool.poetry.group.docs]
+# Optional dependencies for building documentation
+optional = true
 
-[tool.poetry.extras]
-docs = ["Sphinx", "sphinx-immaterial"]
+[tool.poetry.group.docs.dependencies]
+Sphinx = ">=5.1.1"
+sphinx-immaterial = ">=0.8.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wsrouter-0.8.1/wsrouter/cmd.py` & `wsrouter-0.8.3/wsrouter/cmd.py`

 * *Files identical despite different names*

### Comparing `wsrouter-0.8.1/wsrouter/message.py` & `wsrouter-0.8.3/wsrouter/message.py`

 * *Files identical despite different names*

### Comparing `wsrouter-0.8.1/wsrouter/router.py` & `wsrouter-0.8.3/wsrouter/router.py`

 * *Files identical despite different names*

### Comparing `wsrouter-0.8.1/wsrouter/static/websocket.js` & `wsrouter-0.8.3/wsrouter/static/websocket.js`

 * *Files identical despite different names*

### Comparing `wsrouter-0.8.1/setup.py` & `wsrouter-0.8.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['wsrouter']
 
 package_data = \
-{'': ['*'], 'wsrouter': ['static/*']}
+{'': ['*'], 'wsrouter': ['static/websocket.js']}
 
 install_requires = \
-['boltons>=21.0.0,<22.0.0',
- 'orjson>=3.7.1,<4.0.0',
- 'shortuuid>=1.0.9,<2.0.0',
- 'starlette>=0.20.1,<0.21.0']
-
-extras_require = \
-{'docs': ['Sphinx>=5.1.1,<6.0.0', 'sphinx-immaterial>=0.8.1,<0.9.0']}
+['boltons>=21.0.0', 'orjson>=3.7.1', 'shortuuid>=1.0.9', 'starlette>=0.20.1']
 
 setup_kwargs = {
     'name': 'wsrouter',
-    'version': '0.8.1',
+    'version': '0.8.3',
     'description': 'Starlette Shared WebSocket Endpoint',
     'long_description': '# WebSocket Router for Starlette\n\nThis package acts as a websocket message router for [Starlette](https://github.com/encode/starlette)\n[WebSocket](https://www.starlette.io/websockets/) connections, permitting socket sharing for\nmultiple client-server connections.\n\nFor installation and usage, [see the documentation](https://selcouth.gitlab.io/wsrouter).\n',
     'author': 'David Morris',
     'author_email': 'gypsysoftware@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://gitlab.com/selcouth/wsrouter',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'extras_require': extras_require,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `wsrouter-0.8.1/PKG-INFO` & `wsrouter-0.8.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: wsrouter
-Version: 0.8.1
+Version: 0.8.3
 Summary: Starlette Shared WebSocket Endpoint
 Home-page: https://gitlab.com/selcouth/wsrouter
 License: MIT
 Author: David Morris
 Author-email: gypsysoftware@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
-Provides-Extra: docs
-Requires-Dist: Sphinx (>=5.1.1,<6.0.0); extra == "docs"
-Requires-Dist: boltons (>=21.0.0,<22.0.0)
-Requires-Dist: orjson (>=3.7.1,<4.0.0)
-Requires-Dist: shortuuid (>=1.0.9,<2.0.0)
-Requires-Dist: sphinx-immaterial (>=0.8.1,<0.9.0); extra == "docs"
-Requires-Dist: starlette (>=0.20.1,<0.21.0)
+Requires-Dist: boltons (>=21.0.0)
+Requires-Dist: orjson (>=3.7.1)
+Requires-Dist: shortuuid (>=1.0.9)
+Requires-Dist: starlette (>=0.20.1)
 Project-URL: Documentation, https://selcouth.gitlab.io/wsrouter/
 Project-URL: Repository, https://gitlab.com/selcouth/wsrouter
 Description-Content-Type: text/markdown
 
 # WebSocket Router for Starlette
 
 This package acts as a websocket message router for [Starlette](https://github.com/encode/starlette)
```

