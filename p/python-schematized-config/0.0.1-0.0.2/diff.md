# Comparing `tmp/python-schematized-config-0.0.1.tar.gz` & `tmp/python-schematized-config-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-schematized-config-0.0.1.tar", last modified: Mon Jul 17 08:24:36 2023, max compression
+gzip compressed data, was "python-schematized-config-0.0.2.tar", last modified: Tue Jul 18 09:02:07 2023, max compression
```

## Comparing `python-schematized-config-0.0.1.tar` & `python-schematized-config-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-17 08:24:36.631070 python-schematized-config-0.0.1/
--rw-rw-r--   0 alexhuang   (501) wheel        (0)    11337 2023-04-27 10:12:58.000000 python-schematized-config-0.0.1/LICENSE
--rw-rw-r--   0 alexhuang   (501) wheel        (0)      111 2023-04-27 10:12:58.000000 python-schematized-config-0.0.1/MANIFEST.in
--rw-r--r--   0 alexhuang   (501) wheel        (0)     1287 2023-07-17 08:24:36.630928 python-schematized-config-0.0.1/PKG-INFO
--rw-r--r--   0 alexhuang   (501) wheel        (0)      452 2023-07-17 08:24:33.000000 python-schematized-config-0.0.1/README.md
-drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-17 08:24:36.630222 python-schematized-config-0.0.1/python_schematized_config.egg-info/
--rw-r--r--   0 alexhuang   (501) wheel        (0)     1287 2023-07-17 08:24:36.000000 python-schematized-config-0.0.1/python_schematized_config.egg-info/PKG-INFO
--rw-r--r--   0 alexhuang   (501) wheel        (0)      509 2023-07-17 08:24:36.000000 python-schematized-config-0.0.1/python_schematized_config.egg-info/SOURCES.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-07-17 08:24:36.000000 python-schematized-config-0.0.1/python_schematized_config.egg-info/dependency_links.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)       58 2023-07-17 08:24:36.000000 python-schematized-config-0.0.1/python_schematized_config.egg-info/entry_points.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-06-17 02:13:48.000000 python-schematized-config-0.0.1/python_schematized_config.egg-info/not-zip-safe
--rw-r--r--   0 alexhuang   (501) wheel        (0)       47 2023-07-17 08:24:36.000000 python-schematized-config-0.0.1/python_schematized_config.egg-info/requires.txt
--rw-r--r--   0 alexhuang   (501) wheel        (0)       19 2023-07-17 08:24:36.000000 python-schematized-config-0.0.1/python_schematized_config.egg-info/top_level.txt
-drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-17 08:24:36.630754 python-schematized-config-0.0.1/schematized_config/
--rw-r--r--   0 alexhuang   (501) wheel        (0)       22 2023-07-17 08:24:32.000000 python-schematized-config-0.0.1/schematized_config/__init__.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)     3959 2023-07-17 08:24:32.000000 python-schematized-config-0.0.1/schematized_config/_modidx.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)     2139 2023-07-17 08:24:32.000000 python-schematized-config-0.0.1/schematized_config/cli.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)     6087 2023-07-17 08:24:32.000000 python-schematized-config-0.0.1/schematized_config/core.py
--rw-r--r--   0 alexhuang   (501) wheel        (0)     1031 2023-07-17 08:20:59.000000 python-schematized-config-0.0.1/settings.ini
--rw-r--r--   0 alexhuang   (501) wheel        (0)       38 2023-07-17 08:24:36.631111 python-schematized-config-0.0.1/setup.cfg
--rw-rw-r--   0 alexhuang   (501) wheel        (0)     2596 2023-04-27 10:12:58.000000 python-schematized-config-0.0.1/setup.py
+drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-18 09:02:07.444052 python-schematized-config-0.0.2/
+-rw-rw-r--   0 alexhuang   (501) wheel        (0)    11337 2023-04-27 10:12:58.000000 python-schematized-config-0.0.2/LICENSE
+-rw-rw-r--   0 alexhuang   (501) wheel        (0)      111 2023-04-27 10:12:58.000000 python-schematized-config-0.0.2/MANIFEST.in
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     1285 2023-07-18 09:02:07.443913 python-schematized-config-0.0.2/PKG-INFO
+-rw-r--r--   0 alexhuang   (501) wheel        (0)      452 2023-07-17 08:24:33.000000 python-schematized-config-0.0.2/README.md
+drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-18 09:02:07.443184 python-schematized-config-0.0.2/python_schematized_config.egg-info/
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     1285 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/PKG-INFO
+-rw-r--r--   0 alexhuang   (501) wheel        (0)      509 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/SOURCES.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/dependency_links.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       58 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/entry_points.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)        1 2023-06-17 02:13:48.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/not-zip-safe
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       72 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/requires.txt
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       19 2023-07-18 09:02:07.000000 python-schematized-config-0.0.2/python_schematized_config.egg-info/top_level.txt
+drwxr-xr-x   0 alexhuang   (501) wheel        (0)        0 2023-07-18 09:02:07.443732 python-schematized-config-0.0.2/schematized_config/
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       22 2023-07-18 09:00:39.000000 python-schematized-config-0.0.2/schematized_config/__init__.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     4084 2023-07-18 09:00:39.000000 python-schematized-config-0.0.2/schematized_config/_modidx.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     2140 2023-07-18 09:00:39.000000 python-schematized-config-0.0.2/schematized_config/cli.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)     6365 2023-07-18 09:00:39.000000 python-schematized-config-0.0.2/schematized_config/core.py
+-rw-r--r--   0 alexhuang   (501) wheel        (0)      993 2023-07-18 08:59:24.000000 python-schematized-config-0.0.2/settings.ini
+-rw-r--r--   0 alexhuang   (501) wheel        (0)       38 2023-07-18 09:02:07.444095 python-schematized-config-0.0.2/setup.cfg
+-rw-rw-r--   0 alexhuang   (501) wheel        (0)     2596 2023-04-27 10:12:58.000000 python-schematized-config-0.0.2/setup.py
```

### Comparing `python-schematized-config-0.0.1/LICENSE` & `python-schematized-config-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-schematized-config-0.0.1/PKG-INFO` & `python-schematized-config-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: python-schematized-config
-Version: 0.0.1
+Version: 0.0.2
 Summary: validate configs using json schema
-Home-page: https://github.com/aistriketeam/python-schematized-config
+Home-page: https://github.com/tutankalex/python-schematized-config
 Author: tutankalex
 Author-email: 109660532+tutankalex@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `python-schematized-config-0.0.1/python_schematized_config.egg-info/PKG-INFO` & `python-schematized-config-0.0.2/python_schematized_config.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: python-schematized-config
-Version: 0.0.1
+Version: 0.0.2
 Summary: validate configs using json schema
-Home-page: https://github.com/aistriketeam/python-schematized-config
+Home-page: https://github.com/tutankalex/python-schematized-config
 Author: tutankalex
 Author-email: 109660532+tutankalex@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `python-schematized-config-0.0.1/schematized_config/_modidx.py` & `python-schematized-config-0.0.2/schematized_config/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/python-schematized-config',
-                'doc_host': 'https://aistriketeam.github.io',
-                'git_url': 'https://github.com/aistriketeam/python-schematized-config',
+                'doc_host': 'https://tutankalex.github.io',
+                'git_url': 'https://github.com/tutankalex/python-schematized-config',
                 'lib_path': 'schematized_config'},
   'syms': { 'schematized_config.cli': { 'schematized_config.cli.generate_sample_dotenv': ( 'cli.html#generate_sample_dotenv',
                                                                                            'schematized_config/cli.py'),
                                         'schematized_config.cli.main': ('cli.html#main', 'schematized_config/cli.py'),
                                         'schematized_config.cli.validate_env': ('cli.html#validate_env', 'schematized_config/cli.py')},
             'schematized_config.core': { 'schematized_config.core.ConfigValidator': ( 'core.html#configvalidator',
                                                                                       'schematized_config/core.py'),
@@ -15,20 +15,21 @@
                                                                                                'schematized_config/core.py'),
                                          'schematized_config.core.ConfigValidator.get_default_json_schema': ( 'core.html#configvalidator.get_default_json_schema',
                                                                                                               'schematized_config/core.py'),
                                          'schematized_config.core.ConfigValidator.load_config': ( 'core.html#configvalidator.load_config',
                                                                                                   'schematized_config/core.py'),
                                          'schematized_config.core.ConfigValidator.load_dotenv': ( 'core.html#configvalidator.load_dotenv',
                                                                                                   'schematized_config/core.py'),
+                                         'schematized_config.core.ConfigValidator.load_json': ( 'core.html#configvalidator.load_json',
+                                                                                                'schematized_config/core.py'),
                                          'schematized_config.core.ConfigValidator.load_validated_config': ( 'core.html#configvalidator.load_validated_config',
                                                                                                             'schematized_config/core.py'),
                                          'schematized_config.core.ConfigValidator.load_validated_environment': ( 'core.html#configvalidator.load_validated_environment',
                                                                                                                  'schematized_config/core.py'),
                                          'schematized_config.core.ConfigValidatorException': ( 'core.html#configvalidatorexception',
                                                                                                'schematized_config/core.py'),
                                          'schematized_config.core.ConfigValidatorException.__init__': ( 'core.html#configvalidatorexception.__init__',
                                                                                                         'schematized_config/core.py'),
                                          'schematized_config.core.coerce_primitive_values': ( 'core.html#coerce_primitive_values',
                                                                                               'schematized_config/core.py'),
                                          'schematized_config.core.extract_declared_items': ( 'core.html#extract_declared_items',
-                                                                                             'schematized_config/core.py'),
-                                         'schematized_config.core.load_json': ('core.html#load_json', 'schematized_config/core.py')}}}
+                                                                                             'schematized_config/core.py')}}}
```

### Comparing `python-schematized-config-0.0.1/schematized_config/cli.py` & `python-schematized-config-0.0.2/schematized_config/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # %% auto 0
 __all__ = ['validate_env', 'generate_sample_dotenv', 'main']
 
 # %% ../nbs/01_cli.ipynb 2
 from schematized_config.core import (
     ConfigValidator,
     ConfigValidatorException,
-    load_json,
     extract_declared_items,
 )
 
 import os
 import sys
 import argparse
 import dotenv
@@ -28,15 +27,15 @@
         sys.stderr.write(f'{str(ex)}\n')
         for error in ex.errors:
             sys.stderr.write(f'{error.json_path}:\t{error.message}\n')
         return False
 
 # %% ../nbs/01_cli.ipynb 4
 def generate_sample_dotenv(json_schema: Union[str, dict], seed_config: dict=None):
-    schema_dict = load_json(json_schema)
+    schema_dict = ConfigValidator.load_json(json_schema)
     merged_config = dict(os.environ)
     default_dotenv = dotenv.dotenv_values()
     merged_config.update(default_dotenv)
     merged_config.update(seed_config or {})
     extracted_config = extract_declared_items(schema_dict, merged_config)
     out = [
         f'{key}={value}'
```

### Comparing `python-schematized-config-0.0.1/schematized_config/core.py` & `python-schematized-config-0.0.2/schematized_config/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,30 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['logger', 'load_json', 'coerce_primitive_values', 'extract_declared_items', 'ConfigValidatorException',
-           'ConfigValidator']
+__all__ = ['logger', 'coerce_primitive_values', 'extract_declared_items', 'ConfigValidatorException', 'ConfigValidator']
 
 # %% ../nbs/00_core.ipynb 2
 from nbdev.showdoc import *
 from fastcore.test import *
 
 import dotenv
 import json
 import os
 import jsonschema
 import logging
 from jsonschema import validate, ValidationError
 from typing import Union
+from fs.base import FS
+from fs.osfs import OSFS
 
 
 logger = logging.getLogger(__name__)
 
 # %% ../nbs/00_core.ipynb 3
-def load_json(json_source: Union[str, dict]=None) -> dict:
-    '''
-    convenience method to return a dict from either
-    a file path or an already-loaded dict
-    '''
-    if isinstance(json_source, str):
-        with open(json_source) as ifile:
-            return json.load(ifile)
-    elif isinstance(json_source, dict):
-        return json_source
-
-# %% ../nbs/00_core.ipynb 4
 def coerce_primitive_values(json_schema: dict, data: dict) -> dict:
     '''
     given a JSON schema dict, return a dict where the values that have
     primitive types (`string`, `integer`, `number`, `boolean`) as described
     in the schema are converted to the corresponding types from `str`
     
     :param json_schema: expected (but not validated) to be a json schema
@@ -69,15 +58,15 @@
                     parsed_boolean = False
                 out[property_name] = parsed_boolean
         except:
             # leave any validation error descriptions to json schema
             continue
     return out
 
-# %% ../nbs/00_core.ipynb 7
+# %% ../nbs/00_core.ipynb 6
 def extract_declared_items(json_schema: dict, data: dict) -> dict:
     '''
     given a JSON schema dict, return a dict where
     - all keys that are not declared in the schema are removed
     - all keys that are declared in the schem are present;
       if a key is declared in the schema with a default,
       BUT NOT present in the original data, it will be added
@@ -90,46 +79,61 @@
     properties = json_schema['properties']
     out = {key: value for (key, value) in data.items() if key in properties}
     for required_property, property_schema in properties.items():
         if required_property not in out and 'default' in property_schema:
             out[required_property] = property_schema['default']
     return out
 
-# %% ../nbs/00_core.ipynb 9
+# %% ../nbs/00_core.ipynb 8
 class ConfigValidatorException(Exception):
     
     def __init__(self, errors):
         super().__init__('config failed to validate against JSON schema')
         self.errors = errors
 
 
 class ConfigValidator(object):
+
+    DEFAULT_STORAGE_DRIVER: FS = OSFS('.')
     
     CONFIG_VALIDATOR_JSON_SCHEMA_ENVVAR_NAME = 'CONFIG_VALIDATOR_JSON_SCHEMA'
-    
+
+    @classmethod
+    def load_json(cls, json_source: Union[str, dict]=None) -> dict:
+        '''
+        convenience method to return a dict from either
+        a file path or an already-loaded dict
+        '''
+        if isinstance(json_source, str):
+            with cls.DEFAULT_STORAGE_DRIVER.open(json_source) as ifile:
+                return json.load(ifile)
+        elif isinstance(json_source, dict):
+            return json_source
+
     @classmethod
     def get_default_json_schema(cls):
         if cls.CONFIG_VALIDATOR_JSON_SCHEMA_ENVVAR_NAME in os.environ:
             expected_json_schema_path = \
                 os.environ[cls.CONFIG_VALIDATOR_JSON_SCHEMA_ENVVAR_NAME]
-            with open(expected_json_schema_path) as ifile:
+            with cls.DEFAULT_STORAGE_DRIVER.open(expected_json_schema_path) as ifile:
                 return json.load(ifile)
         return None
 
-    def __init__(self, json_schema: Union[str, dict]=None):
+    def __init__(self, json_schema: Union[str, dict]=None, storage_driver: FS=None):
         '''
         :param json_schema: a str path to a json schema file, or a schema in dict form
         
         if no value is provided, it will fall back to looking for
         an environment variable corresponding to the class variable
         `CONFIG_VALIDATOR_JSON_SCHEMA_ENVVAR_NAME`
         to find a JSON schema file
         '''
+        self.storage_driver = storage_driver or self.__class__.DEFAULT_STORAGE_DRIVER
         if isinstance(json_schema, (str, dict)):
-            self._json_schema = load_json(json_schema)
+            self._json_schema = self.__class__.load_json(json_schema)
         elif (default_schema := self.__class__.get_default_json_schema()):
             self._json_schema = default_schema
         else:
             raise Exception('did not receive or find a JSON schema')
 
     def load_config(self, config: dict):
         extracted_config = extract_declared_items(self._json_schema, config)
```

### Comparing `python-schematized-config-0.0.1/setup.py` & `python-schematized-config-0.0.2/setup.py`

 * *Files identical despite different names*

