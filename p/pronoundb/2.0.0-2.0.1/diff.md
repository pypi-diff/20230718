# Comparing `tmp/pronoundb-2.0.0.tar.gz` & `tmp/pronoundb-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pronoundb-2.0.0.tar", max compression
+gzip compressed data, was "pronoundb-2.0.1.tar", max compression
```

## Comparing `pronoundb-2.0.0.tar` & `pronoundb-2.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2022-11-18 17:05:56.697373 pronoundb-2.0.0/LICENSE
--rw-r--r--   0        0        0       93 2022-11-18 16:02:01.482088 pronoundb-2.0.0/pronoundb/__init__.py
--rw-r--r--   0        0        0     3026 2023-05-27 21:33:50.816512 pronoundb-2.0.0/pronoundb/api.py
--rw-r--r--   0        0        0      175 2023-05-27 21:01:46.113572 pronoundb-2.0.0/pronoundb/platform.py
--rw-r--r--   0        0        0      664 2023-05-27 21:40:24.484655 pronoundb-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1889 2023-05-27 21:42:02.059224 pronoundb-2.0.0/README.md
--rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 pronoundb-2.0.0/setup.py
--rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 pronoundb-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-07-18 10:23:53.257491 pronoundb-2.0.1/LICENSE
+-rw-r--r--   0        0        0       93 2023-07-18 10:23:53.258486 pronoundb-2.0.1/pronoundb/__init__.py
+-rw-r--r--   0        0        0     3026 2023-07-18 10:23:53.258486 pronoundb-2.0.1/pronoundb/api.py
+-rw-r--r--   0        0        0      175 2023-07-18 10:23:53.258486 pronoundb-2.0.1/pronoundb/platform.py
+-rw-r--r--   0        0        0      677 2023-07-18 10:33:59.458889 pronoundb-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1889 2023-07-18 10:23:53.257491 pronoundb-2.0.1/README.md
+-rw-r--r--   0        0        0     2609 1970-01-01 00:00:00.000000 pronoundb-2.0.1/setup.py
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 pronoundb-2.0.1/PKG-INFO
```

### Comparing `pronoundb-2.0.0/LICENSE` & `pronoundb-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pronoundb-2.0.0/pronoundb/api.py` & `pronoundb-2.0.1/pronoundb/api.py`

 * *Files identical despite different names*

### Comparing `pronoundb-2.0.0/pyproject.toml` & `pronoundb-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "pronoundb"
-version = "2.0.0"
+version = "2.0.1"
 description = "API wrapper for the pronoundb.org API."
 license = "MIT"
 authors = ["SteffoSpieler <steffo@steffospieler.de>"]
 maintainers = ["SteffoSpieler <steffo@steffospieler.de>"]
 readme = "README.md"
-repository = "https://gitlab.com/SteffoSpieler/pronoundb-library"
+repository = "https://git.steffospieler.de/SteffoSpieler/python-pronoundb-lib"
 keywords = ["pronouns", "pronoundb", "api"]
 packages = [{include = "pronoundb"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = "^3.8"
```

### Comparing `pronoundb-2.0.0/README.md` & `pronoundb-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pronoundb-2.0.0/setup.py` & `pronoundb-2.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8,<4.0']
 
 setup_kwargs = {
     'name': 'pronoundb',
-    'version': '2.0.0',
+    'version': '2.0.1',
     'description': 'API wrapper for the pronoundb.org API.',
     'long_description': '# PronounDB Python API\n\n![PyPI](https://img.shields.io/pypi/v/pronoundb?style=flat-square)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pronoundb?style=flat-square)\n![PyPI - License](https://img.shields.io/pypi/l/pronoundb?style=flat-square)\n\nAPI wrapper for the pronoundb.org API.\n\n## Installation\n\n```bash\npip install pronoundb\n```\n\n## Examples\n\nlookup someone\'s pronouns by their discord id:\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.DISCORD, 123456789012345678)\n# -> {123456789012345678: ["he", "him"]}\n```\n\nlookup someone\'s pronouns by their minecraft (java) uuid:\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.MINECRAFT, "12345678-1234-1234-1234-123456789012")\n# -> {"12345678-1234-1234-1234-123456789012": ["they", "them"]}\n```\n\nlookup multiple users pronouns by their discord id:\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.DISCORD, [123456789012345678, 987654321098765432])\n# -> {123456789012345678: ["he", "him"], 987654321098765432: ["she", "her"]}\n```\n\n## Supported Platforms\n\n- Discord\n- GitHub\n- Minecraft (Java)\n- Twitch\n- Twitter\n\n## Custom Pronouns (Version 2.0.0)\n\nBeginning with version 2.0.0 you can give the lookup function a list of pronouns to translate them for example.\n\n```py\nfrom pronoundb import lookup, Platform\n\nlookup(Platform.DISCORD, 123456789012345678, {\n    "unspecified": [],\n    "he": ["Er", "Ihn"],\n    "she": ["Sie", "Ihr"],\n    "they": ["They", "Them"],\n    "any": ["Jede"],\n    "other": ["Anderes"],\n    "ask": ["Frag"],\n    "avoid": ["Nutz Name"],\n})\n# -> {123456789012345678: ["Er", "Ihn"]}\n```\n\n## Contributing\n\nContributions to this library are always welcome and highly encouraged.\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.\n',
     'author': 'SteffoSpieler',
     'author_email': 'steffo@steffospieler.de',
     'maintainer': 'SteffoSpieler',
     'maintainer_email': 'steffo@steffospieler.de',
-    'url': 'https://gitlab.com/SteffoSpieler/pronoundb-library',
+    'url': 'https://git.steffospieler.de/SteffoSpieler/python-pronoundb-lib',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `pronoundb-2.0.0/PKG-INFO` & `pronoundb-2.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pronoundb
-Version: 2.0.0
+Version: 2.0.1
 Summary: API wrapper for the pronoundb.org API.
-Home-page: https://gitlab.com/SteffoSpieler/pronoundb-library
+Home-page: https://git.steffospieler.de/SteffoSpieler/python-pronoundb-lib
 License: MIT
 Keywords: pronouns,pronoundb,api
 Author: SteffoSpieler
 Author-email: steffo@steffospieler.de
 Maintainer: SteffoSpieler
 Maintainer-email: steffo@steffospieler.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8,<4.0)
-Project-URL: Repository, https://gitlab.com/SteffoSpieler/pronoundb-library
+Project-URL: Repository, https://git.steffospieler.de/SteffoSpieler/python-pronoundb-lib
 Description-Content-Type: text/markdown
 
 # PronounDB Python API
 
 ![PyPI](https://img.shields.io/pypi/v/pronoundb?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pronoundb?style=flat-square)
 ![PyPI - License](https://img.shields.io/pypi/l/pronoundb?style=flat-square)
```

