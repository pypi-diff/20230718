# Comparing `tmp/TravSHACL-1.4.0.tar.gz` & `tmp/TravSHACL-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TravSHACL-1.4.0.tar", last modified: Thu Jul 13 12:18:34 2023, max compression
+gzip compressed data, was "TravSHACL-1.4.1.tar", last modified: Tue Jul 18 12:29:38 2023, max compression
```

## Comparing `TravSHACL-1.4.0.tar` & `TravSHACL-1.4.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.216628 TravSHACL-1.4.0/TravSHACL/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/TravSHACL.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.216628 TravSHACL-1.4.0/TravSHACL/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/MaxOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/MinMaxConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/MinOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/SPARQLConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/TravSHACL/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/GraphTraversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/RulePattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/Shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    29359 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/ShapeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/ShapeSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/TravSHACL/rule_based_validation/
--rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/rule_based_validation/InstancesRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/rule_based_validation/Validation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/rule_based_validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/TravSHACL/sparql/
--rw-r--r--   0 runner    (1001) docker     (123)    27726 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/sparql/QueryGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/sparql/SPARQLEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/sparql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/TravSHACL/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/utils/ValidationStats.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/utils/VariableGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/TravSHACL/utils/fileManagement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.216628 TravSHACL-1.4.0/TravSHACL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-13 12:18:34.000000 TravSHACL-1.4.0/TravSHACL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 12:18:34.000000 TravSHACL-1.4.0/TravSHACL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:18:34.000000 TravSHACL-1.4.0/TravSHACL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 12:18:34.000000 TravSHACL-1.4.0/TravSHACL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 12:18:34.000000 TravSHACL-1.4.0/TravSHACL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:18:34.220629 TravSHACL-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-13 12:18:23.000000 TravSHACL-1.4.0/tests/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.109178 TravSHACL-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-18 12:29:38.109178 TravSHACL-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.093178 TravSHACL-1.4.1/TravSHACL/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/TravSHACL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.101178 TravSHACL-1.4.1/TravSHACL/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/MaxOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/MinMaxConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/MinOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/SPARQLConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.105178 TravSHACL-1.4.1/TravSHACL/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/GraphTraversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/RulePattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24062 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/ShapeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/ShapeSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.105178 TravSHACL-1.4.1/TravSHACL/rule_based_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/rule_based_validation/InstancesRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/rule_based_validation/Validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/rule_based_validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.109178 TravSHACL-1.4.1/TravSHACL/sparql/
+-rw-r--r--   0 runner    (1001) docker     (123)    27726 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/sparql/QueryGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/sparql/SPARQLEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/sparql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.109178 TravSHACL-1.4.1/TravSHACL/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/utils/ValidationStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/utils/VariableGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/utils/fileManagement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.097178 TravSHACL-1.4.1/TravSHACL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-18 12:29:38.000000 TravSHACL-1.4.1/TravSHACL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 12:29:38.000000 TravSHACL-1.4.1/TravSHACL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:29:38.000000 TravSHACL-1.4.1/TravSHACL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-18 12:29:38.000000 TravSHACL-1.4.1/TravSHACL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 12:29:38.000000 TravSHACL-1.4.1/TravSHACL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-18 12:29:38.113178 TravSHACL-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.109178 TravSHACL-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/tests/test_cases.py
```

### Comparing `TravSHACL-1.4.0/LICENSE` & `TravSHACL-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/PKG-INFO` & `TravSHACL-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TravSHACL
-Version: 1.4.0
+Version: 1.4.1
 Summary: A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.
 Home-page: https://github.com/SDM-TIB/Trav-SHACL
-Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.4.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.4.1.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `TravSHACL-1.4.0/README.md` & `TravSHACL-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/TravSHACL.py` & `TravSHACL-1.4.1/TravSHACL/TravSHACL.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/constraints/Constraint.py` & `TravSHACL-1.4.1/TravSHACL/constraints/Constraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/constraints/MaxOnlyConstraint.py` & `TravSHACL-1.4.1/TravSHACL/constraints/MaxOnlyConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/constraints/MinMaxConstraint.py` & `TravSHACL-1.4.1/TravSHACL/constraints/MinMaxConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/constraints/MinOnlyConstraint.py` & `TravSHACL-1.4.1/TravSHACL/constraints/MinOnlyConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/constraints/SPARQLConstraint.py` & `TravSHACL-1.4.1/TravSHACL/constraints/SPARQLConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/core/GraphTraversal.py` & `TravSHACL-1.4.1/TravSHACL/core/GraphTraversal.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/core/RulePattern.py` & `TravSHACL-1.4.1/TravSHACL/core/RulePattern.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/core/Shape.py` & `TravSHACL-1.4.1/TravSHACL/core/Shape.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/core/ShapeParser.py` & `TravSHACL-1.4.1/TravSHACL/core/ShapeParser.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from rdflib import Graph
 from itertools import islice
 
 from TravSHACL.constraints.SPARQLConstraint import SPARQLConstraint
 from TravSHACL.core.Shape import Shape
 from TravSHACL.utils.VariableGenerator import VariableGenerator
 from TravSHACL.constraints.MaxOnlyConstraint import MaxOnlyConstraint
-from TravSHACL.constraints.MinMaxConstraint import MinMaxConstraint
 from TravSHACL.constraints.MinOnlyConstraint import MinOnlyConstraint
 
 QUERY_TARGET_QUERY = '''SELECT ?query WHERE {{
   <{shape}> a <http://www.w3.org/ns/shacl#NodeShape> ;
       <http://www.w3.org/ns/shacl#targetQuery> ?query .
 }}'''
 
@@ -174,24 +173,15 @@
 
             #valid_flag = [entry['flag'] for entry in const_array if entry['flag']]
             valid_flag = []
             for entry in const_array:
                 if 'flag' in entry.keys():
                     valid_flag.append(entry['flag'])
 
-            if True in valid_flag:
-                var_generator = VariableGenerator()
-                valid_options = self.parse_or_constraint(var_generator, const_array, id_ + "_c",
-                                                         target_def)  # remember you removed +str(i + 1) in id_ used
-                valid_raw = self.extract_only_or(const_array)
-            else:
-                valid_options = None
-                valid_raw = None
-
-            constraints = self.parse_constraints_ttl(const_array, target_def, id_, valid_options, valid_raw)
+            constraints = self.parse_constraints_ttl(const_array, target_def, id_)
             include_sparql_prefixes = self.abbreviated_syntax_used(constraints)
             prefixes = None
             referenced_shapes = self.shape_references(const_array)
 
             # helps to navigate the shape.__compute_target_queries function
             referenced_shape = {'<' + key + '>': '<' + referenced_shapes[key] + '>'
                                 for key in referenced_shapes.keys()
@@ -303,25 +293,14 @@
                                   <{shape}> a <http://www.w3.org/ns/shacl#NodeShape> .
                                   <{shape}> <http://www.w3.org/ns/shacl#or> ?constraint .
                                 }}
                                 '''
         return QUERY_SHAPES, QUERY_TARGET_1, QUERY_TARGET_2, QUERY_CONSTRAINTS, QUERY_CONSTRAINT_DETAILS, \
                QUERY_QVS_REF_1, QUERY_QVS_REF_2, QUERY_SPARQL_CONSTRAINTS, QUERY_OR
 
-    @staticmethod
-    def extract_only_or(or_constraint):
-        or_raw = []
-        for option in or_constraint:
-            keys = list(option['or'].keys())
-            grouping = []
-            for key in keys:
-                grouping.append(option['or'][key])
-            or_raw.append(grouping)
-        return or_raw
-
     def get_res(self, filename, name, query):
         """
 
         :param query: List of queries
         :param name: name of the Shape
         :param filename: shape file in ttl format
         :return: valid response from query execution
@@ -452,35 +431,38 @@
         var_generator = VariableGenerator()
         constraints = []
         options = None
         [constraints.extend(self.parse_constraint(var_generator, array[0][i], constraints_id + '_c' + str(i + 1),
                                                   target_def, options)) for i in range(len(array[0]))]
         return constraints
 
-    def parse_constraints_ttl(self, array, target_def, constraints_id, options, raw_or):
+    def parse_constraints_ttl(self, array, target_def, constraints_id):
         """
         Parses all constraints of a shape.
 
         :param array: list of constraints belonging to the shape
         :param target_def: the target definition of the shape
         :param constraints_id: suffix for the constraint IDs
-        :param options: option to be used in or_operations
-        :param raw_or: raw form for 'or' query response
         :return: list of constraints in internal constraint representation
         """
         var_generator = VariableGenerator()
         constraints = []
-        if not options:
-            [constraints.extend(
-                self.parse_constraint(var_generator, array[i], constraints_id + '_c' + str(i + 1), target_def
-                                      )) for i in range(len(array))]
-        else:
-            [constraints.extend(
-                self.parse_constraint(var_generator, array[i], constraints_id + '_c' + str(i + 1), target_def,
-                                      options[i], raw_or[i])) for i in range(len(array))]
+
+        for i, constraint in enumerate(array):
+            if constraint.get('flag'):
+                or_constraints = []
+                raw_or = []
+                for key in constraint['or'].keys():
+                    sub_constraint = constraint['or'][key]
+                    raw_or.append(sub_constraint)
+                    or_constraints.extend(self.parse_constraint(var_generator, sub_constraint, constraints_id + '_c' + str(i + 1), target_def, None, []))
+                constraints.extend(self.parse_constraint(var_generator, constraint, constraints_id + '_c' + str(i + 1), target_def, or_constraints, raw_or))
+            else:
+                constraints.extend(self.parse_constraint(var_generator, constraint, constraints_id + '_c' + str(i + 1), target_def, None, []))
+
         return constraints
 
     @staticmethod
     def parse_constraint(var_generator, obj, id_, target_def, options=None, raw_or=None):
         """
         Parses one constraint to the internal representation.
 
@@ -530,109 +512,16 @@
 
         if urlparse(datatype).netloc != '' and datatype is not None:  # if the data type is a url, add '<>' to it
             o_datatype = '<' + datatype + '>'
 
         if o_path is not None:
             if o_min is not None:
                 if o_max is not None:
-                    # return MinMaxConstraint(var_generator, id_, o_path, o_min, o_max, o_neg, o_datatype, o_value, o_shape_ref, target_def)
-                    return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype,
-                                              o_value, o_shape_ref, target_def),
-                            MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, raw_or, o_datatype,
-                                              o_value, o_shape_ref, target_def)]
-                return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype,
-                                          o_value, o_shape_ref, target_def)]
+                    return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype, o_value, o_shape_ref, target_def),
+                            MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, raw_or, o_datatype, o_value, o_shape_ref, target_def)]
+                return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype, o_value, o_shape_ref, target_def)]
             if o_max is not None:
-                return [MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, raw_or, o_datatype,
-                                          o_value, o_shape_ref, target_def)]
+                return [MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, raw_or, o_datatype, o_value, o_shape_ref, target_def)]
         elif o_query is not None:
             return [SPARQLConstraint(id_, o_neg, o_query)]
         elif o_path is None:
-            return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype, o_value,
-                                      o_shape_ref, target_def)]
-
-    @staticmethod
-    def parse_or_constraint(var_generator, objs, id_, target_def):
-        """
-        Parses one constraint to the internal representation.
-
-        :param var_generator: reference to the VariableGenerator instance for variable generation for SPARQL queries
-        :param objs: the constraint in its original representation
-        :param id_: suffix for the constraint ID
-        :param target_def: the target definition of the associated shape
-        :return: constraint in internal representation
-        """
-        constraint_list = []
-        options = None
-        raw_or = None
-        for obj in objs:
-            shape_ref = obj.get("shape")
-            datatype = obj.get("datatype")
-            value = obj.get("value")
-            negated = obj.get("negated")
-            query = obj.get('sparql')
-
-            keys = list(obj['or'].keys())
-            or_constraints = []
-            for key in keys:
-                min_ = None
-                max_ = None
-                path = None
-                for key_, value_ in obj['or'][key].items():
-                    if key_ == 'path':
-                        path = value_
-                    if key_ == 'max':
-                        max_ = value_
-                    if key_ == 'min':
-                        min_ = value_
-
-                o_min = None if (min_ is None) else int(min_)
-                o_max = None if (max_ is None) else int(max_)
-                o_shape_ref = None if (shape_ref is None) else str(shape_ref)
-                o_datatype = None if (datatype is None) else str(datatype)
-                o_value = None if (value is None) else str(value)
-                o_path = None if (path is None) else str(path)
-                o_neg = True if (negated is None) else not negated
-                o_query = None if (query is None) else str(query)           # not used in this implementation
-
-                if path is not None and str(path).startswith('^'):
-                    is_inverse_path = True
-                    path = str(path)[1:]
-                else:
-                    is_inverse_path = False
-
-                if urlparse(path).netloc != '':  # if the predicate is a url, add '<>' to it
-                    o_path = '<' + path + '>'
-                if is_inverse_path:
-                    o_path = '^' + o_path
-
-                if urlparse(
-                        shape_ref).netloc != '' and shape_ref is not None:  # if shape reference is a url, add '<>' to it
-                    o_shape_ref = '<' + shape_ref + '>'
-
-                if urlparse(
-                        value).netloc != '' and value is not None:  # if the value reference is a url, add '<>' to it
-                    o_value = '<' + value + '>'
-
-                if urlparse(
-                        datatype).netloc != '' and datatype is not None:  # if the data type is a url, add '<>' to it
-                    o_datatype = '<' + datatype + '>'
-
-                if o_path is not None:
-                    if o_min is not None:
-                        if o_max is not None:
-                            constraint = [
-                                MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype,
-                                                  o_value, o_shape_ref, target_def),
-                                MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, raw_or, o_datatype,
-                                                  o_value, o_shape_ref, target_def)]
-                        else:
-                            constraint = MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or,
-                                                           o_datatype, o_value, o_shape_ref, target_def)
-                    else:
-                        if o_max is not None:
-                            constraint = MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options,  raw_or,
-                                                           o_datatype, o_value, o_shape_ref, target_def)
-
-                    or_constraints.append(constraint)
-            constraint_list.append(or_constraints.copy() if or_constraints else None)
-        return constraint_list
+            return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype, o_value, o_shape_ref, target_def)]
```

### Comparing `TravSHACL-1.4.0/TravSHACL/core/ShapeSchema.py` & `TravSHACL-1.4.1/TravSHACL/core/ShapeSchema.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/rule_based_validation/InstancesRetrieval.py` & `TravSHACL-1.4.1/TravSHACL/rule_based_validation/InstancesRetrieval.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/rule_based_validation/Validation.py` & `TravSHACL-1.4.1/TravSHACL/rule_based_validation/Validation.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/sparql/QueryGenerator.py` & `TravSHACL-1.4.1/TravSHACL/sparql/QueryGenerator.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/sparql/SPARQLEndpoint.py` & `TravSHACL-1.4.1/TravSHACL/sparql/SPARQLEndpoint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/utils/ValidationStats.py` & `TravSHACL-1.4.1/TravSHACL/utils/ValidationStats.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/utils/VariableGenerator.py` & `TravSHACL-1.4.1/TravSHACL/utils/VariableGenerator.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL/utils/fileManagement.py` & `TravSHACL-1.4.1/TravSHACL/utils/fileManagement.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/TravSHACL.egg-info/PKG-INFO` & `TravSHACL-1.4.1/TravSHACL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TravSHACL
-Version: 1.4.0
+Version: 1.4.1
 Summary: A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.
 Home-page: https://github.com/SDM-TIB/Trav-SHACL
-Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.4.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.4.1.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `TravSHACL-1.4.0/TravSHACL.egg-info/SOURCES.txt` & `TravSHACL-1.4.1/TravSHACL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/setup.py` & `TravSHACL-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.0/tests/test_cases.py` & `TravSHACL-1.4.1/tests/test_cases.py`

 * *Files identical despite different names*

