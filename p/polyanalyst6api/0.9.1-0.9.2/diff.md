# Comparing `tmp/polyanalyst6api-0.9.1.tar.gz` & `tmp/polyanalyst6api-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyanalyst6api-0.9.1.tar", last modified: Fri Oct 25 15:23:49 2019, max compression
+gzip compressed data, was "polyanalyst6api-0.9.2.tar", last modified: Tue Oct 29 12:51:22 2019, max compression
```

## Comparing `polyanalyst6api-0.9.1.tar` & `polyanalyst6api-0.9.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1057 2019-10-24 14:00:58.345844 polyanalyst6api-0.9.1/LICENSE
--rw-r--r--   0        0        0       42 2019-10-25 15:21:05.640023 polyanalyst6api-0.9.1/polyanalyst6api/__init__.py
--rw-r--r--   0        0        0    19320 2019-10-25 15:11:05.605839 polyanalyst6api-0.9.1/polyanalyst6api/api.py
--rw-r--r--   0        0        0      876 2019-10-24 14:00:58.353838 polyanalyst6api-0.9.1/polyanalyst6api/exceptions.py
--rw-r--r--   0        0        0      900 2019-10-25 15:21:48.091565 polyanalyst6api-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1993 2019-10-24 14:00:58.346844 polyanalyst6api-0.9.1/README.md
--rw-r--r--   0        0        0     2753 1970-01-01 00:00:00.000000 polyanalyst6api-0.9.1/setup.py
--rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 polyanalyst6api-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2019-10-24 14:00:58.345844 polyanalyst6api-0.9.2/LICENSE
+-rw-r--r--   0        0        0       42 2019-10-29 12:49:03.429934 polyanalyst6api-0.9.2/polyanalyst6api/__init__.py
+-rw-r--r--   0        0        0    19324 2019-10-29 12:36:43.124673 polyanalyst6api-0.9.2/polyanalyst6api/api.py
+-rw-r--r--   0        0        0      876 2019-10-24 14:00:58.353838 polyanalyst6api-0.9.2/polyanalyst6api/exceptions.py
+-rw-r--r--   0        0        0      900 2019-10-29 12:49:30.877092 polyanalyst6api-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1993 2019-10-24 14:00:58.346844 polyanalyst6api-0.9.2/README.md
+-rw-r--r--   0        0        0     2753 1970-01-01 00:00:00.000000 polyanalyst6api-0.9.2/setup.py
+-rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 polyanalyst6api-0.9.2/PKG-INFO
```

### Comparing `polyanalyst6api-0.9.1/LICENSE` & `polyanalyst6api-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polyanalyst6api-0.9.1/polyanalyst6api/api.py` & `polyanalyst6api-0.9.2/polyanalyst6api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,42 +284,42 @@
     def create_folder(self, name: str, path: str = '') -> None:
         """
         Create a new folder inside the PolyAnalyst's user directory.
 
         :param name: the folder name
         :param path: a relative path of the folder's parent directory
         """
-        self.api.get('folder/create', json={'path': path, 'name': name})
+        self.api.post('folder/create', json={'path': path, 'name': name})
 
     def delete_folder(self, name: str, path: str = '') -> None:
         """
         Delete the folder in the PolyAnalyst's user directory.
 
         :param name: the folder name
         :param path: a relative path of the folder's parent directory
         """
-        self.api.get('folder/delete', json={'path': path, 'name': name})
+        self.api.post('folder/delete', json={'path': path, 'name': name})
 
     def delete_file(self, name: str, path: str = '') -> None:
         """
         Delete the file in the PolyAnalyst's user directory.
 
         :param name: the filename
         :param path: a relative path of the file's parent directory
         """
-        self.api.get('file/delete', json={'path': path, 'name': name})
+        self.api.post('file/delete', json={'path': path, 'name': name})
 
     def download_file(self, name: str, path: str = '') -> bytes:
         """
         Download the binary content of the file.
 
         :param name: the filename
         :param path: a relative path of the file's parent directory
         """
-        data = self.api.get('file/download', json={'path': path, 'name': name})
+        data = self.api.post('file/download', json={'path': path, 'name': name})
         resp, _ = self.api.request(
             urljoin(self.api.url, '/polyanalyst/download'),
             method='get',
             params={'uid': data['uid']}
         )
         return resp.content
```

### Comparing `polyanalyst6api-0.9.1/polyanalyst6api/exceptions.py` & `polyanalyst6api-0.9.2/polyanalyst6api/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyanalyst6api-0.9.1/pyproject.toml` & `polyanalyst6api-0.9.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyanalyst6api"
-version = "0.9.1"
+version = "0.9.2"
 description = "polyanalyst6api is a PolyAnalyst API client for Python."
 authors = ["yatmanov <yatmanov@megaputer.ru>"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/Megaputer/polyanalyst6api-python/"
 documentation = "https://megaputer.github.io/polyanalyst6api-python/"
```

### Comparing `polyanalyst6api-0.9.1/README.md` & `polyanalyst6api-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `polyanalyst6api-0.9.1/setup.py` & `polyanalyst6api-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pytus>=0.2.1,<0.3.0', 'requests>=2.19,<3.0']
 
 setup_kwargs = {
     'name': 'polyanalyst6api',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'polyanalyst6api is a PolyAnalyst API client for Python.',
     'long_description': "# polyanalyst6api\n\n`polyanalyst6api` is a python package for accessing PolyAnalyst's APIs.\n\n## Installation\n\nThe easiest way to install `polyanalyst6api-python` is from [PyPI](https://pypi.org/project/polyanalyst6api/):\n\n```\n$ pip install polyanalyst6api\n```\n\nYou may also use Git to clone the repository from GitHub and install it manually:\n\n```\ngit clone https://github.com/Megaputer/polyanalyst6api-python.git\ncd polyanalyst6api-python\npip install poetry\npoetry install\n```\n\n## Usage\n\nSee [API Reference](https://megaputer.github.io/polyanalyst6api-python/) for more detailed information.\n\n### Authentication\n\nImport client, initialize it and log in to PolyAnalyst's server:\n\n```python\nimport polyanalyst6api as polyanalyst\n\napi = polyanalyst.API(POLYANALIST_URL, USERNAME, PASSWORD)\napi.login()\n```\n\n`API` supports Context Manager protocol, so you could use it with `with` statement. In this case `API` will automatically log in with provided credentials.\n\n```python\nwith polyanalyst.API(POLYANALIST_URL, USERNAME, PASSWORD) as api:\n    pass\n```\n\n### Working with project\n\nSee [polyanalyst6api-python/examples](https://github.com/Megaputer/polyanalyst6api-python/tree/master/examples) for a more complex examples.\n\nAt first you need to connect to existing project:\n```python\nprj = api.project(PROJECT_UUID)\n```\n\nPrint node names within project:\n```python\nfor node_name in prj.get_nodes():\n    print(node_name)\n```\n\nInitiate node execution:\n```python\nprj.execute(NODE_NAME)\n```\n\nDisplay the preview of node results:\n```python\nresult = prj.preview(NODE_NAME)\nprint(result)\n```\n\nSave project:\n```python\nprj.save()\n```\n\n## PolyAnalyst API\nFull API specification is stored in the **PolyAnalyst User Manual** under the url below:\n\n```\n/polyanalyst/help/eng/24_Application_Programming_Interfaces/toc.html\n```\n\n## Supported Python version\n\n`polyanalyst6api-python` works only with `python3` (3.4+).\n\n## License\n\nThis project is licensed under the MIT License - see the LICENSE.md file for details\n",
     'author': 'yatmanov',
     'author_email': 'yatmanov@megaputer.ru',
     'url': 'https://github.com/Megaputer/polyanalyst6api-python/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `polyanalyst6api-0.9.1/PKG-INFO` & `polyanalyst6api-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyanalyst6api
-Version: 0.9.1
+Version: 0.9.2
 Summary: polyanalyst6api is a PolyAnalyst API client for Python.
 Home-page: https://github.com/Megaputer/polyanalyst6api-python/
 License: MIT
 Keywords: megaputer,polyanalyst,polyanalyst6api,api
 Author: yatmanov
 Author-email: yatmanov@megaputer.ru
 Requires-Python: >=3.6,<4.0
```

