# Comparing `tmp/onto_tool-1.7.3.tar.gz` & `tmp/onto_tool-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onto_tool-1.7.3.tar", last modified: Wed Jun 14 01:37:12 2023, max compression
+gzip compressed data, was "onto_tool-1.7.4.tar", last modified: Tue Jul 18 20:26:42 2023, max compression
```

## Comparing `onto_tool-1.7.3.tar` & `onto_tool-1.7.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.727115 onto_tool-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-14 01:36:59.000000 onto_tool-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-06-14 01:37:12.727115 onto_tool-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27123 2023-06-14 01:36:59.000000 onto_tool-1.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.723115 onto_tool-1.7.3/onto_tool/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/bundle_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/mdutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    53313 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/onto_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    40027 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/ontograph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/sparql_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.727115 onto_tool-1.7.3/onto_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:37:12.727115 onto_tool-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-14 01:36:59.000000 onto_tool-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.727115 onto_tool-1.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.727115 onto_tool-1.7.3/tests/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_file_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_sparql.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_syntax_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.727115 onto_tool-1.7.3/tests/graphic/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/graphic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/graphic/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/graphic/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/test_issue-36.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:26:42.408925 onto_tool-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-18 20:26:29.000000 onto_tool-1.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-07-18 20:26:42.408925 onto_tool-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27123 2023-07-18 20:26:29.000000 onto_tool-1.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:26:42.404925 onto_tool-1.7.4/onto_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 20:26:29.000000 onto_tool-1.7.4/onto_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 20:26:29.000000 onto_tool-1.7.4/onto_tool/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-07-18 20:26:29.000000 onto_tool-1.7.4/onto_tool/bundle_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-07-18 20:26:29.000000 onto_tool-1.7.4/onto_tool/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-18 20:26:29.000000 onto_tool-1.7.4/onto_tool/mdutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53313 2023-07-18 20:26:29.000000 onto_tool-1.7.4/onto_tool/onto_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40027 2023-07-18 20:26:29.000000 onto_tool-1.7.4/onto_tool/ontograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-18 20:26:29.000000 onto_tool-1.7.4/onto_tool/sparql_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:26:42.408925 onto_tool-1.7.4/onto_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-07-18 20:26:42.000000 onto_tool-1.7.4/onto_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-18 20:26:42.000000 onto_tool-1.7.4/onto_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:26:42.000000 onto_tool-1.7.4/onto_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 20:26:42.000000 onto_tool-1.7.4/onto_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 20:26:42.000000 onto_tool-1.7.4/onto_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 20:26:42.000000 onto_tool-1.7.4/onto_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 20:26:42.408925 onto_tool-1.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-18 20:26:29.000000 onto_tool-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:26:42.408925 onto_tool-1.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:26:42.408925 onto_tool-1.7.4/tests/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/bundle/test_file_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/bundle/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/bundle/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/bundle/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/bundle/test_sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/bundle/test_syntax_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/bundle/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/bundle/test_verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:26:42.408925 onto_tool-1.7.4/tests/graphic/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/graphic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/graphic/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-18 20:26:29.000000 onto_tool-1.7.4/tests/graphic/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-18 20:26:30.000000 onto_tool-1.7.4/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-18 20:26:30.000000 onto_tool-1.7.4/tests/test_issue-36.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-18 20:26:30.000000 onto_tool-1.7.4/tests/test_update.py
```

### Comparing `onto_tool-1.7.3/LICENSE` & `onto_tool-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/PKG-INFO` & `onto_tool-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onto_tool
-Version: 1.7.3
+Version: 1.7.4
 Summary: Ontology Maintenance and Release Tool
 Home-page: https://github.com/semanticarts/ontology-toolkit
 Author: Boris Pelakh
 Author-email: boris.pelakh@semanticarts.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onto_tool-1.7.3/README.md` & `onto_tool-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/onto_tool/bundle_schema.yaml` & `onto_tool-1.7.4/onto_tool/bundle_schema.yaml`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/onto_tool/command_line.py` & `onto_tool-1.7.4/onto_tool/command_line.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/onto_tool/onto_tool.py` & `onto_tool-1.7.4/onto_tool/onto_tool.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/onto_tool/ontograph.py` & `onto_tool-1.7.4/onto_tool/ontograph.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/onto_tool/sparql_utils.py` & `onto_tool-1.7.4/onto_tool/sparql_utils.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/onto_tool.egg-info/PKG-INFO` & `onto_tool-1.7.4/onto_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onto-tool
-Version: 1.7.3
+Version: 1.7.4
 Summary: Ontology Maintenance and Release Tool
 Home-page: https://github.com/semanticarts/ontology-toolkit
 Author: Boris Pelakh
 Author-email: boris.pelakh@semanticarts.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onto_tool-1.7.3/onto_tool.egg-info/SOURCES.txt` & `onto_tool-1.7.4/onto_tool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 tests/__init__.py
 tests/test_export.py
 tests/test_issue-36.py
 tests/test_update.py
 tests/bundle/__init__.py
 tests/bundle/test_file_ref.py
 tests/bundle/test_logging.py
+tests/bundle/test_markdown.py
 tests/bundle/test_message.py
 tests/bundle/test_sparql.py
 tests/bundle/test_syntax_error.py
 tests/bundle/test_transform.py
 tests/bundle/test_verify.py
 tests/graphic/__init__.py
 tests/graphic/test_instance.py
```

### Comparing `onto_tool-1.7.3/setup.py` & `onto_tool-1.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     url="https://github.com/semanticarts/ontology-toolkit",
     packages=setuptools.find_packages(),
     install_requires=[
         'pyparsing==2.4.7',
         'rdflib~=6.1.1',
         'pydot',
         'jinja2',
-        'markdown',
+        'markdown2',
         'pyyaml',
         'jsonschema>=3.2.0',
         'SPARQLWrapper>=1.8.5',
         'pyshacl~=0.17.0'
     ],
     tests_require=[
         'pytest'
```

### Comparing `onto_tool-1.7.3/tests/bundle/test_logging.py` & `onto_tool-1.7.4/tests/bundle/test_logging.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/tests/bundle/test_sparql.py` & `onto_tool-1.7.4/tests/bundle/test_sparql.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/tests/bundle/test_transform.py` & `onto_tool-1.7.4/tests/bundle/test_transform.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/tests/bundle/test_verify.py` & `onto_tool-1.7.4/tests/bundle/test_verify.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/tests/graphic/test_instance.py` & `onto_tool-1.7.4/tests/graphic/test_instance.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/tests/graphic/test_schema.py` & `onto_tool-1.7.4/tests/graphic/test_schema.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/tests/test_export.py` & `onto_tool-1.7.4/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/tests/test_issue-36.py` & `onto_tool-1.7.4/tests/test_issue-36.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.3/tests/test_update.py` & `onto_tool-1.7.4/tests/test_update.py`

 * *Files identical despite different names*

