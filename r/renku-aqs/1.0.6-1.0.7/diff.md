# Comparing `tmp/renku-aqs-1.0.6.tar.gz` & `tmp/renku-aqs-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renku-aqs-1.0.6.tar", last modified: Tue Jul 11 12:12:07 2023, max compression
+gzip compressed data, was "renku-aqs-1.0.7.tar", last modified: Tue Jul 18 09:04:24 2023, max compression
```

## Comparing `renku-aqs-1.0.6.tar` & `renku-aqs-1.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      187 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/.gitignore
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    11358 2021-06-14 15:54:58.000000 renku-aqs-1.0.6/LICENSE
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      114 2021-06-14 15:54:58.000000 renku-aqs-1.0.6/MANIFEST.in
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      937 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/PKG-INFO
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     6340 2023-02-22 13:05:10.000000 renku-aqs-1.0.6/README.md
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        5 2023-07-11 12:11:05.000000 renku-aqs-1.0.6/VERSION
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      345 2021-06-14 15:54:58.000000 renku-aqs-1.0.6/concepts.md
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1659 2021-06-28 10:31:11.000000 renku-aqs-1.0.6/example.md
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/readme_imgs/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)  1891362 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/animation_expansion_retraction.gif
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    22497 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/enable_disable_configuration-graph.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   302729 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/example_display_graph_complete.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   150316 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/example_display_graph_final-an.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    36993 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/example_display_graph_final-an_no-oda-info.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   146690 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/example_show-graph.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    61174 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/expanded_plan.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    71535 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/hierarchical_view.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    52046 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/reduced_plan.png
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    52899 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/readme_imgs/subgraph.png
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/renku_aqs.egg-info/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      937 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/PKG-INFO
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1066 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/SOURCES.txt
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/dependency_links.txt
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      171 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/entry_points.txt
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2021-12-08 07:18:18.000000 renku-aqs-1.0.6/renku_aqs.egg-info/not-zip-safe
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      120 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/requires.txt
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        9 2023-07-11 12:12:07.000000 renku-aqs-1.0.6/renku_aqs.egg-info/top_level.txt
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/renkuaqs/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     5975 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/renkuaqs/__init__.py
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      606 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/renkuaqs/config.py
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     2092 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/renkuaqs/graph_config.yaml
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     7384 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/renkuaqs/graph_graphical_config.json
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     8836 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/renkuaqs/graph_nodes_subset_config.json
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      421 2023-02-10 17:08:04.000000 renku-aqs-1.0.6/renkuaqs/graph_reduction_config.json
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    50791 2023-06-05 17:42:34.000000 renku-aqs-1.0.6/renkuaqs/graph_utils.py
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/renkuaqs/icons/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3416 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/renkuaqs/icons/graph_icon.svg
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    11874 2023-03-14 09:55:25.000000 renku-aqs-1.0.6/renkuaqs/javascript_graph_utils.py
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    42892 2023-05-26 14:38:27.000000 renku-aqs-1.0.6/renkuaqs/ontology.ttl
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    18752 2023-07-11 12:03:33.000000 renku-aqs-1.0.6/renkuaqs/plugin.py
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        0 2023-01-23 09:07:17.000000 renku-aqs-1.0.6/requirements.txt
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)       38 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/setup.cfg
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     2399 2023-07-11 12:10:22.000000 renku-aqs-1.0.6/setup.py
-drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-11 12:12:07.064849 renku-aqs-1.0.6/tests/
--rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3093 2023-02-08 14:37:58.000000 renku-aqs-1.0.6/tests/test_example.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-18 09:04:24.192872 renku-aqs-1.0.7/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      187 2023-06-05 17:42:34.000000 renku-aqs-1.0.7/.gitignore
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    11358 2021-06-14 15:54:58.000000 renku-aqs-1.0.7/LICENSE
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      114 2021-06-14 15:54:58.000000 renku-aqs-1.0.7/MANIFEST.in
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      937 2023-07-18 09:04:24.192872 renku-aqs-1.0.7/PKG-INFO
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     6340 2023-02-22 13:05:10.000000 renku-aqs-1.0.7/README.md
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        5 2023-07-12 14:26:23.000000 renku-aqs-1.0.7/VERSION
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      345 2021-06-14 15:54:58.000000 renku-aqs-1.0.7/concepts.md
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1659 2021-06-28 10:31:11.000000 renku-aqs-1.0.7/example.md
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-18 09:04:24.188871 renku-aqs-1.0.7/readme_imgs/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)  1891362 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/readme_imgs/animation_expansion_retraction.gif
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    22497 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/readme_imgs/enable_disable_configuration-graph.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   302729 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/readme_imgs/example_display_graph_complete.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   150316 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/readme_imgs/example_display_graph_final-an.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    36993 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/readme_imgs/example_display_graph_final-an_no-oda-info.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)   146690 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/readme_imgs/example_show-graph.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    61174 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/readme_imgs/expanded_plan.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    71535 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/readme_imgs/hierarchical_view.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    52046 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/readme_imgs/reduced_plan.png
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    52899 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/readme_imgs/subgraph.png
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-18 09:04:24.192872 renku-aqs-1.0.7/renku_aqs.egg-info/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      937 2023-07-18 09:04:24.000000 renku-aqs-1.0.7/renku_aqs.egg-info/PKG-INFO
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     1066 2023-07-18 09:04:24.000000 renku-aqs-1.0.7/renku_aqs.egg-info/SOURCES.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2023-07-18 09:04:24.000000 renku-aqs-1.0.7/renku_aqs.egg-info/dependency_links.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      171 2023-07-18 09:04:24.000000 renku-aqs-1.0.7/renku_aqs.egg-info/entry_points.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        1 2021-12-08 07:18:18.000000 renku-aqs-1.0.7/renku_aqs.egg-info/not-zip-safe
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      120 2023-07-18 09:04:24.000000 renku-aqs-1.0.7/renku_aqs.egg-info/requires.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        9 2023-07-18 09:04:24.000000 renku-aqs-1.0.7/renku_aqs.egg-info/top_level.txt
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-18 09:04:24.192872 renku-aqs-1.0.7/renkuaqs/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     5975 2023-06-05 17:42:34.000000 renku-aqs-1.0.7/renkuaqs/__init__.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      606 2023-06-05 17:42:34.000000 renku-aqs-1.0.7/renkuaqs/config.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     2092 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/renkuaqs/graph_config.yaml
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     7384 2023-06-05 17:42:34.000000 renku-aqs-1.0.7/renkuaqs/graph_graphical_config.json
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     9253 2023-07-17 14:33:11.000000 renku-aqs-1.0.7/renkuaqs/graph_nodes_subset_config.json
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)      421 2023-02-10 17:08:04.000000 renku-aqs-1.0.7/renkuaqs/graph_reduction_config.json
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    51108 2023-07-17 13:01:05.000000 renku-aqs-1.0.7/renkuaqs/graph_utils.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-18 09:04:24.192872 renku-aqs-1.0.7/renkuaqs/icons/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3416 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/renkuaqs/icons/graph_icon.svg
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    11874 2023-03-14 09:55:25.000000 renku-aqs-1.0.7/renkuaqs/javascript_graph_utils.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    42892 2023-05-26 14:38:27.000000 renku-aqs-1.0.7/renkuaqs/ontology.ttl
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)    18752 2023-07-11 12:13:06.000000 renku-aqs-1.0.7/renkuaqs/plugin.py
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)        0 2023-01-23 09:07:17.000000 renku-aqs-1.0.7/requirements.txt
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)       38 2023-07-18 09:04:24.192872 renku-aqs-1.0.7/setup.cfg
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     2399 2023-07-18 09:04:17.000000 renku-aqs-1.0.7/setup.py
+drwxrwxr-x   0 gabriele  (1001) gabriele  (1001)        0 2023-07-18 09:04:24.192872 renku-aqs-1.0.7/tests/
+-rw-rw-r--   0 gabriele  (1001) gabriele  (1001)     3093 2023-02-08 14:37:58.000000 renku-aqs-1.0.7/tests/test_example.py
```

### Comparing `renku-aqs-1.0.6/LICENSE` & `renku-aqs-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/PKG-INFO` & `renku-aqs-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renku-aqs
-Version: 1.0.6
+Version: 1.0.7
 Summary: Renku AQS plugin
 Author: Gabriele Barni, Volodymyr Savchenko
 Author-email: 
 License: Apache License 2.0
 Keywords: Renku AQS
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `renku-aqs-1.0.6/README.md` & `renku-aqs-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/example.md` & `renku-aqs-1.0.7/example.md`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/readme_imgs/animation_expansion_retraction.gif` & `renku-aqs-1.0.7/readme_imgs/animation_expansion_retraction.gif`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/readme_imgs/enable_disable_configuration-graph.png` & `renku-aqs-1.0.7/readme_imgs/enable_disable_configuration-graph.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/readme_imgs/example_display_graph_complete.png` & `renku-aqs-1.0.7/readme_imgs/example_display_graph_complete.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/readme_imgs/example_display_graph_final-an.png` & `renku-aqs-1.0.7/readme_imgs/example_display_graph_final-an.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/readme_imgs/example_display_graph_final-an_no-oda-info.png` & `renku-aqs-1.0.7/readme_imgs/example_display_graph_final-an_no-oda-info.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/readme_imgs/example_show-graph.png` & `renku-aqs-1.0.7/readme_imgs/example_show-graph.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/readme_imgs/expanded_plan.png` & `renku-aqs-1.0.7/readme_imgs/expanded_plan.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/readme_imgs/hierarchical_view.png` & `renku-aqs-1.0.7/readme_imgs/hierarchical_view.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/readme_imgs/reduced_plan.png` & `renku-aqs-1.0.7/readme_imgs/reduced_plan.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/readme_imgs/subgraph.png` & `renku-aqs-1.0.7/readme_imgs/subgraph.png`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/renku_aqs.egg-info/PKG-INFO` & `renku-aqs-1.0.7/renku_aqs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renku-aqs
-Version: 1.0.6
+Version: 1.0.7
 Summary: Renku AQS plugin
 Author: Gabriele Barni, Volodymyr Savchenko
 Author-email: 
 License: Apache License 2.0
 Keywords: Renku AQS
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `renku-aqs-1.0.6/renku_aqs.egg-info/SOURCES.txt` & `renku-aqs-1.0.7/renku_aqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/renkuaqs/__init__.py` & `renku-aqs-1.0.7/renkuaqs/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/renkuaqs/config.py` & `renku-aqs-1.0.7/renkuaqs/config.py`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/renkuaqs/graph_config.yaml` & `renku-aqs-1.0.7/renkuaqs/graph_config.yaml`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/renkuaqs/graph_graphical_config.json` & `renku-aqs-1.0.7/renkuaqs/graph_graphical_config.json`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/renkuaqs/graph_nodes_subset_config.json` & `renku-aqs-1.0.7/renkuaqs/graph_nodes_subset_config.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'oda'": "{'query_construct': '?parameter_binding_ontology_class a "*

 * *          '<http://www.w3.org/2002/07/owl#Class> '*

 * *          ';\\n\\t<http://www.w3.org/2000/01/rdf-schema#subClassOf> '*

 * *          '?parameter_binding_ontology_parent_class '*

 * *          ';\\n\\t<http://www.w3.org/2000/01/rdf-schema#label> '*

 * *          '?parameter_binding_ontology_class_extracted_label .\\n\\n?entityOutput '*

 * *          '<http://odahub.io/ontology#hasParameter> ?parameter_binding_output ;\\n\\t '*

 * *          '<http://odahub.io/o […]*

```diff
@@ -1,9 +1,9 @@
 {
     "oda": {
         "description": "oda astroquery-related nodes",
         "ontology_url": "http://odahub.io/ontology/ontology.ttl",
         "prefixes": "oda, odas",
-        "query_construct": "?parameter_binding_ontology_class a <http://www.w3.org/2002/07/owl#Class> ;\n\t<http://www.w3.org/2000/01/rdf-schema#subClassOf> ?parameter_binding_ontology_parent_class ;\n\t<http://www.w3.org/2000/01/rdf-schema#label> ?parameter_binding_ontology_class_extracted_label .\n\n?entityOutput <http://odahub.io/ontology#hasParameter> ?parameter_binding_output ;\n\t <http://odahub.io/ontology#hasOutput> ?output_binding_output .\n\n?parameter_binding_output <http://odahub.io/ontology#parameter_name> ?parameter_binding_output_name ;\n\ta ?parameter_binding_output_type ;\n\t<http://odahub.io/ontology#value> ?parameter_binding_output_value ;\n\t<http://odahub.io/ontology#isAlso> ?parameter_binding_output_type .\n\t\n?output_binding_output <http://odahub.io/ontology#output_name> ?output_binding_output_name ;\n\ta ?output_binding_output_type ;\n\t<http://odahub.io/ontology#isAlso> ?output_binding_output_type .\n\n?entityInput <http://odahub.io/ontology#hasParameter> ?parameter_binding_input .\n\n?parameter_binding_input <http://odahub.io/ontology#parameter_name> ?parameter_binding_input_name ;\n\ta ?parameter_binding_input_type ;\n\t<http://odahub.io/ontology#value> ?parameter_binding_input_value ;\n\t<http://odahub.io/ontology#isAlso> ?parameter_binding_input_type .\n\n?activity <http://www.w3.org/ns/oa#calls> ?run .\n\n?run <http://odahub.io/ontology#isRequestingAstroObject> ?a_object ;\n        <http://odahub.io/ontology#isRequestingAstroRegion> ?a_region ;\n        <http://odahub.io/ontology#isRequestingAstroImage> ?a_image ;\n        <http://purl.org/dc/terms/title> ?run_title ;\n        <http://odahub.io/ontology#isUsing> ?aq_module ;\n        a ?run_rdf_type .\n    \n?aq_module <https://odahub.io/ontology#AQModule> ?aq_module_name ;\n\ta ?aq_mod_rdf_type ;\n\t<http://odahub.io/ontology#isAlso> ?aq_mod_rdf_type .\n\n?a_object <https://odahub.io/ontology#AstroObject> ?a_object_name ;\n\ta ?a_obj_rdf_type ;\n\t<http://odahub.io/ontology#isAlso> ?a_obj_rdf_type .\n\n?a_region a ?a_region_type ; \n\t<http://purl.org/dc/terms/title> ?a_region_name ;\n\t<http://odahub.io/ontology#isUsingSkyCoordinates> ?a_sky_coordinates ;\n\t<http://odahub.io/ontology#isUsingRadius> ?a_radius .\n\n?a_image a ?a_image_type ;\n\t<http://purl.org/dc/terms/title> ?a_image_name ;\n\t<http://odahub.io/ontology#isUsingCoordinates> ?a_coordinates ;\n\t<http://odahub.io/ontology#isUsingPosition> ?a_position ;\n\t<http://odahub.io/ontology#isUsingRadius> ?a_radius ;\n\t<http://odahub.io/ontology#isUsingPixels> ?a_pixels ;\n\t<http://odahub.io/ontology#isUsingImageBand> ?a_image_band .\n\n?a_pixels a ?a_pixels_type ;\n\t<http://purl.org/dc/terms/title> ?a_pixels_name .\n\n?a_image_band a ?a_image_band_type ;\n\t<http://purl.org/dc/terms/title> ?a_image_band_name .\n\n?a_coordinates a ?a_coordinates_type ;\n\t<http://purl.org/dc/terms/title> ?a_coordinates_name .\n\n?a_sky_coordinates a ?a_sky_coordinates_type ;\n\t<http://purl.org/dc/terms/title> ?a_sky_coordinates_name .\n\n?a_position a ?a_position_type ;\n\t<http://purl.org/dc/terms/title> ?a_position_name .\n\n?a_radius a ?a_radius_type ;\n\t<http://purl.org/dc/terms/title> ?a_radius_name .",
-        "query_where": "{\n\tOPTIONAL { ?parameter_binding_ontology_class a <http://www.w3.org/2002/07/owl#Class> . }\n\tOPTIONAL { ?parameter_binding_ontology_class <http://www.w3.org/2000/01/rdf-schema#subClassOf> ?parameter_binding_ontology_parent_class . }\n\tOPTIONAL { ?parameter_binding_ontology_class <http://www.w3.org/2000/01/rdf-schema#label> ?parameter_binding_ontology_class_label . }\n\t\n\tBIND(STRAFTER(STR(?parameter_binding_ontology_class), \"#\") AS ?parameter_binding_ontology_class_extracted_label) .\n}\nUNION\n{\t\n\t?workflow_input <http://odahub.io/ontology#expects> ?parameter_binding_input ;\n\t\t<http://odahub.io/ontology#entity_checksum> ?entityInputChecksum ;\n\t\ta <http://odahub.io/ontology#workflow> .\n\n\t?parameter_binding_input a ?parameter_binding_input_type .\n\t\n\tBIND(STRAFTER(STR(?parameter_binding_input), \"#\") AS ?parameter_binding_input_name) .\n\t\n\tOPTIONAL { ?parameter_binding_input_type a <http://www.w3.org/2002/07/owl#Class> . }\n\tOPTIONAL { ?parameter_binding_input <http://odahub.io/ontology#value> ?parameter_binding_input_value . }\n}\nUNION\n{\t\n\t?workflow_output <http://odahub.io/ontology#expects> ?parameter_binding_output ;\n\t\t<http://odahub.io/ontology#outputs> ?output_binding_output ;\n\t\t<http://odahub.io/ontology#entity_checksum> ?entityOutputChecksum ;\n\t\ta <http://odahub.io/ontology#workflow> .\n\n\t?parameter_binding_output a ?parameter_binding_output_type .\n\t?output_binding_output a ?output_binding_output_type .\n\t\n\tBIND(STRAFTER(STR(?parameter_binding_output), \"#\") AS ?parameter_binding_output_name) .\n\tBIND(STRAFTER(STR(?output_binding_output), \"#\") AS ?output_binding_output_name) .\n\t\n\tOPTIONAL { ?parameter_binding_output_type a <http://www.w3.org/2002/07/owl#Class> . }\n\tOPTIONAL { ?parameter_binding_equivalent_output_type <http://www.w3.org/2000/01/rdf-schema#equivalentClass> ?parameter_binding_output_type . }\n\tOPTIONAL { ?parameter_binding_output <http://odahub.io/ontology#value> ?parameter_binding_output_value . }\n}\nUNION\n{\t\n\t?run <http://odahub.io/ontology#isUsing> ?aq_module ;\n\t    <http://odahub.io/ontology#isRequestingAstroObject> ?a_object ;\n\t    a ?run_rdf_type ;\n\t    ^<http://www.w3.org/ns/oa#hasBody>/<http://www.w3.org/ns/oa#hasTarget> ?activity .\n\n        ?aq_module <http://purl.org/dc/terms/title> ?aq_module_name ;\n\t    a ?aq_mod_rdf_type .\n\n\t?a_object <http://purl.org/dc/terms/title> ?a_object_name ;\n           a ?a_obj_rdf_type .\n\n\tOPTIONAL { ?run <http://purl.org/dc/terms/title> ?run_title . } .\n\n\t?run ?p ?o .\n\n\tFILTER(!REGEX(STR(?a_object), \"\\\\s\")) .\n\t\n\tOPTIONAL {\n\t  ?aq_type a <http://www.w3.org/2002/07/owl#Class> .\n\t  FILTER (?aq_type IN (?aq_mod_rdf_type, ?a_obj_rdf_type))\n\t}\n}\nUNION\n{\n\t?run <http://odahub.io/ontology#isUsing> ?aq_module ;\n\t    <http://odahub.io/ontology#isRequestingAstroRegion> ?a_region ;\n\t    a ?run_rdf_type ;\n\t    ^<http://www.w3.org/ns/oa#hasBody>/<http://www.w3.org/ns/oa#hasTarget> ?activity .\n\n\t?aq_module a ?aq_mod_rdf_type ;\n\t    <http://purl.org/dc/terms/title> ?aq_module_name .\n\n\t?a_region a ?a_region_type ; \n\t    <http://purl.org/dc/terms/title> ?a_region_name ;\n\t    <http://odahub.io/ontology#isUsingSkyCoordinates> ?a_sky_coordinates ;\n\t    <http://odahub.io/ontology#isUsingRadius> ?a_radius .\n\n\t?a_sky_coordinates a ?a_sky_coordinates_type ;\n\t    <http://purl.org/dc/terms/title> ?a_sky_coordinates_name .\n\n\t?a_radius a ?a_radius_type ;\n\t    <http://purl.org/dc/terms/title> ?a_radius_name .\n\n\tOPTIONAL { ?run <http://purl.org/dc/terms/title> ?run_title . } .\n\n\t?run ?p ?o .\n\t\n\tOPTIONAL {\n\t  ?aq_type a <http://www.w3.org/2002/07/owl#Class> .\n\t  FILTER (?aq_type IN (?aq_mod_rdf_type, ?a_region_type, ?a_sky_coordinates_type, ?a_radius_type))\n\t}\n\t\t\n}\nUNION\n{\n\t?run <http://odahub.io/ontology#isUsing> ?aq_module ;\n\t    <http://odahub.io/ontology#isRequestingAstroImage> ?a_image ;\n\t    a ?run_rdf_type ;\n\t    ^<http://www.w3.org/ns/oa#hasBody>/<http://www.w3.org/ns/oa#hasTarget> ?activity .\n\n\t?aq_module a ?aq_mod_rdf_type ;\n\t    <http://purl.org/dc/terms/title> ?aq_module_name .\n\n\t?a_image a ?a_image_type ;\n\t    <http://purl.org/dc/terms/title> ?a_image_name ;\n\n\tOPTIONAL { ?a_image <http://odahub.io/ontology#isUsingCoordinates> ?a_coordinates .\n\t    ?a_coordinates a ?a_coordinates_type ;\n\t\t<http://purl.org/dc/terms/title> ?a_coordinates_name .\n\t}\n\tOPTIONAL { ?a_image <http://odahub.io/ontology#isUsingPosition> ?a_position .\n\t    ?a_position a ?a_position_type ;\n\t\t<http://purl.org/dc/terms/title> ?a_position_name .\n\t}\n\tOPTIONAL { ?a_image <http://odahub.io/ontology#isUsingRadius> ?a_radius .\n\t    ?a_radius a ?a_radius_type ;\n\t\t<http://purl.org/dc/terms/title> ?a_radius_name .\n\t}\n\tOPTIONAL { ?a_image <http://odahub.io/ontology#isUsingPixels> ?a_pixels .\n\t    ?a_pixels a ?a_pixels_type ;\n\t\t<http://purl.org/dc/terms/title> ?a_pixels_name .\n\t}\n\tOPTIONAL { ?a_image <http://odahub.io/ontology#isUsingImageBand> ?a_image_band .\n\t    ?a_image_band a ?a_image_band_type ;\n\t\t<http://purl.org/dc/terms/title> ?a_image_band_name .\n\t}\n\n\tOPTIONAL { ?run <http://purl.org/dc/terms/title> ?run_title . } .\n\n\t?run ?p ?o .\n\t\n\tOPTIONAL {\n\t  ?aq_type a <http://www.w3.org/2002/07/owl#Class> .\n\t  FILTER (?aq_type IN (?a_coordinates_type, ?a_position_type, ?a_radius_type, ?a_pixels_type, ?a_image_band_type))\n\t}\n\t\n}"
+        "query_construct": "?parameter_binding_ontology_class a <http://www.w3.org/2002/07/owl#Class> ;\n\t<http://www.w3.org/2000/01/rdf-schema#subClassOf> ?parameter_binding_ontology_parent_class ;\n\t<http://www.w3.org/2000/01/rdf-schema#label> ?parameter_binding_ontology_class_extracted_label .\n\n?entityOutput <http://odahub.io/ontology#hasParameter> ?parameter_binding_output ;\n\t <http://odahub.io/ontology#hasOutput> ?output_binding_output .\n\n?parameter_binding_output <http://odahub.io/ontology#parameter_name> ?parameter_binding_output_name ;\n\ta ?parameter_binding_output_type ;\n\t<http://odahub.io/ontology#value> ?parameter_binding_output_value ;\n\t<http://odahub.io/ontology#isAlso> ?parameter_binding_ontology_output_type .\n\t\n?output_binding_output <http://odahub.io/ontology#output_name> ?output_binding_output_name ;\n\ta ?output_binding_output_type ;\n\t<http://odahub.io/ontology#isAlso> ?output_binding_ontology_output_type .\n\n?entityInput <http://odahub.io/ontology#hasParameter> ?parameter_binding_input .\n\n?parameter_binding_input <http://odahub.io/ontology#parameter_name> ?parameter_binding_input_name ;\n\ta ?parameter_binding_input_type ;\n\t<http://odahub.io/ontology#value> ?parameter_binding_input_value ;\n\t<http://odahub.io/ontology#isAlso> ?parameter_binding_ontology_input_type .\n\n?activity <http://www.w3.org/ns/oa#calls> ?run .\n\n?run <http://odahub.io/ontology#isRequestingAstroObject> ?a_object ;\n        <http://odahub.io/ontology#isRequestingAstroRegion> ?a_region ;\n        <http://odahub.io/ontology#isRequestingAstroImage> ?a_image ;\n        <http://purl.org/dc/terms/title> ?run_title ;\n        <http://odahub.io/ontology#isUsing> ?aq_module ;\n        a ?run_rdf_type .\n    \n?aq_module <https://odahub.io/ontology#AQModule> ?aq_module_name ;\n\ta ?aq_mod_rdf_type ;\n\t<http://odahub.io/ontology#isAlso> ?aq_mod_rdf_type .\n\n?a_object <https://odahub.io/ontology#AstroObject> ?a_object_name ;\n\ta ?a_obj_rdf_type ;\n\t<http://odahub.io/ontology#isAlso> ?a_obj_rdf_type .\n\n?a_region a ?a_region_type ; \n\t<http://purl.org/dc/terms/title> ?a_region_name ;\n\t<http://odahub.io/ontology#isUsingSkyCoordinates> ?a_sky_coordinates ;\n\t<http://odahub.io/ontology#isUsingRadius> ?a_radius .\n\n?a_image a ?a_image_type ;\n\t<http://purl.org/dc/terms/title> ?a_image_name ;\n\t<http://odahub.io/ontology#isUsingCoordinates> ?a_coordinates ;\n\t<http://odahub.io/ontology#isUsingPosition> ?a_position ;\n\t<http://odahub.io/ontology#isUsingRadius> ?a_radius ;\n\t<http://odahub.io/ontology#isUsingPixels> ?a_pixels ;\n\t<http://odahub.io/ontology#isUsingImageBand> ?a_image_band .\n\n?a_pixels a ?a_pixels_type ;\n\t<http://purl.org/dc/terms/title> ?a_pixels_name .\n\n?a_image_band a ?a_image_band_type ;\n\t<http://purl.org/dc/terms/title> ?a_image_band_name .\n\n?a_coordinates a ?a_coordinates_type ;\n\t<http://purl.org/dc/terms/title> ?a_coordinates_name .\n\n?a_sky_coordinates a ?a_sky_coordinates_type ;\n\t<http://purl.org/dc/terms/title> ?a_sky_coordinates_name .\n\n?a_position a ?a_position_type ;\n\t<http://purl.org/dc/terms/title> ?a_position_name .\n\n?a_radius a ?a_radius_type ;\n\t<http://purl.org/dc/terms/title> ?a_radius_name .",
+        "query_where": "{\n\tOPTIONAL { ?parameter_binding_ontology_class a <http://www.w3.org/2002/07/owl#Class> . }\n\tOPTIONAL { ?parameter_binding_ontology_class <http://www.w3.org/2000/01/rdf-schema#subClassOf> ?parameter_binding_ontology_parent_class . }\n\tOPTIONAL { ?parameter_binding_ontology_class <http://www.w3.org/2000/01/rdf-schema#label> ?parameter_binding_ontology_class_label . }\n\t\n\tBIND(STRAFTER(STR(?parameter_binding_ontology_class), \"#\") AS ?parameter_binding_ontology_class_extracted_label) .\n}\nUNION\n{\t\n\t?workflow_input <http://odahub.io/ontology#expects> ?parameter_binding_input ;\n\t\t<http://odahub.io/ontology#entity_checksum> ?entityInputChecksum ;\n\t\ta <http://odahub.io/ontology#workflow> .\n\n\t?parameter_binding_input a ?parameter_binding_input_type .\n\t\n\tOPTIONAL\n\t{ \n\t\t?parameter_binding_input a ?parameter_binding_ontology_input_type . \n\t\t?parameter_binding_ontology_input_type a <http://www.w3.org/2002/07/owl#Class> .\n\t}\n\t\n\tBIND(STRAFTER(STR(?parameter_binding_input), \"#\") AS ?parameter_binding_input_name) .\n\t\n\t\n\tOPTIONAL { ?parameter_binding_input <http://odahub.io/ontology#value> ?parameter_binding_input_value . }\n}\nUNION\n{\t\n\t?workflow_output <http://odahub.io/ontology#expects> ?parameter_binding_output ;\n\t\t<http://odahub.io/ontology#outputs> ?output_binding_output ;\n\t\t<http://odahub.io/ontology#entity_checksum> ?entityOutputChecksum ;\n\t\ta <http://odahub.io/ontology#workflow> .\n\n\t?parameter_binding_output a ?parameter_binding_output_type .\n\t\n\tOPTIONAL\n\t{\n\t\t?parameter_binding_output a ?parameter_binding_ontology_output_type . \n\t\t?parameter_binding_ontology_output_type a <http://www.w3.org/2002/07/owl#Class> .\n\t}\n\t\n\t\n\t?output_binding_output a ?output_binding_output_type .\n\t\n\tOPTIONAL\n\t{\n\t\t?output_binding_output a ?output_binding_ontology_output_type .\n\t\t?output_binding_ontology_output_type a <http://www.w3.org/2002/07/owl#Class> .\n\t}\n\t\n\tBIND(STRAFTER(STR(?parameter_binding_output), \"#\") AS ?parameter_binding_output_name) .\n\tBIND(STRAFTER(STR(?output_binding_output), \"#\") AS ?output_binding_output_name) .\n\t\n\tOPTIONAL { ?parameter_binding_equivalent_output_type <http://www.w3.org/2000/01/rdf-schema#equivalentClass> ?parameter_binding_output_type . }\n\tOPTIONAL { ?parameter_binding_output <http://odahub.io/ontology#value> ?parameter_binding_output_value . }\n}\nUNION\n{\t\n\t?run <http://odahub.io/ontology#isUsing> ?aq_module ;\n\t    <http://odahub.io/ontology#isRequestingAstroObject> ?a_object ;\n\t    a ?run_rdf_type ;\n\t    ^<http://www.w3.org/ns/oa#hasBody>/<http://www.w3.org/ns/oa#hasTarget> ?activity .\n\n        ?aq_module <http://purl.org/dc/terms/title> ?aq_module_name ;\n\t    a ?aq_mod_rdf_type .\n\n\t?a_object <http://purl.org/dc/terms/title> ?a_object_name ;\n           a ?a_obj_rdf_type .\n\n\tOPTIONAL { ?run <http://purl.org/dc/terms/title> ?run_title . } .\n\n\t?run ?p ?o .\n\n\tFILTER(!REGEX(STR(?a_object), \"\\\\s\")) .\n\t\n\tOPTIONAL {\n\t  ?aq_type a <http://www.w3.org/2002/07/owl#Class> .\n\t  FILTER (?aq_type IN (?aq_mod_rdf_type, ?a_obj_rdf_type))\n\t}\n}\nUNION\n{\n\t?run <http://odahub.io/ontology#isUsing> ?aq_module ;\n\t    <http://odahub.io/ontology#isRequestingAstroRegion> ?a_region ;\n\t    a ?run_rdf_type ;\n\t    ^<http://www.w3.org/ns/oa#hasBody>/<http://www.w3.org/ns/oa#hasTarget> ?activity .\n\n\t?aq_module a ?aq_mod_rdf_type ;\n\t    <http://purl.org/dc/terms/title> ?aq_module_name .\n\n\t?a_region a ?a_region_type ; \n\t    <http://purl.org/dc/terms/title> ?a_region_name ;\n\t    <http://odahub.io/ontology#isUsingSkyCoordinates> ?a_sky_coordinates ;\n\t    <http://odahub.io/ontology#isUsingRadius> ?a_radius .\n\n\t?a_sky_coordinates a ?a_sky_coordinates_type ;\n\t    <http://purl.org/dc/terms/title> ?a_sky_coordinates_name .\n\n\t?a_radius a ?a_radius_type ;\n\t    <http://purl.org/dc/terms/title> ?a_radius_name .\n\n\tOPTIONAL { ?run <http://purl.org/dc/terms/title> ?run_title . } .\n\n\t?run ?p ?o .\n\t\n\tOPTIONAL {\n\t  ?aq_type a <http://www.w3.org/2002/07/owl#Class> .\n\t  FILTER (?aq_type IN (?aq_mod_rdf_type, ?a_region_type, ?a_sky_coordinates_type, ?a_radius_type))\n\t}\n\t\t\n}\nUNION\n{\n\t?run <http://odahub.io/ontology#isUsing> ?aq_module ;\n\t    <http://odahub.io/ontology#isRequestingAstroImage> ?a_image ;\n\t    a ?run_rdf_type ;\n\t    ^<http://www.w3.org/ns/oa#hasBody>/<http://www.w3.org/ns/oa#hasTarget> ?activity .\n\n\t?aq_module a ?aq_mod_rdf_type ;\n\t    <http://purl.org/dc/terms/title> ?aq_module_name .\n\n\t?a_image a ?a_image_type ;\n\t    <http://purl.org/dc/terms/title> ?a_image_name ;\n\n\tOPTIONAL { ?a_image <http://odahub.io/ontology#isUsingCoordinates> ?a_coordinates .\n\t    ?a_coordinates a ?a_coordinates_type ;\n\t\t<http://purl.org/dc/terms/title> ?a_coordinates_name .\n\t}\n\tOPTIONAL { ?a_image <http://odahub.io/ontology#isUsingPosition> ?a_position .\n\t    ?a_position a ?a_position_type ;\n\t\t<http://purl.org/dc/terms/title> ?a_position_name .\n\t}\n\tOPTIONAL { ?a_image <http://odahub.io/ontology#isUsingRadius> ?a_radius .\n\t    ?a_radius a ?a_radius_type ;\n\t\t<http://purl.org/dc/terms/title> ?a_radius_name .\n\t}\n\tOPTIONAL { ?a_image <http://odahub.io/ontology#isUsingPixels> ?a_pixels .\n\t    ?a_pixels a ?a_pixels_type ;\n\t\t<http://purl.org/dc/terms/title> ?a_pixels_name .\n\t}\n\tOPTIONAL { ?a_image <http://odahub.io/ontology#isUsingImageBand> ?a_image_band .\n\t    ?a_image_band a ?a_image_band_type ;\n\t\t<http://purl.org/dc/terms/title> ?a_image_band_name .\n\t}\n\n\tOPTIONAL { ?run <http://purl.org/dc/terms/title> ?run_title . } .\n\n\t?run ?p ?o .\n\t\n\tOPTIONAL {\n\t  ?aq_type a <http://www.w3.org/2002/07/owl#Class> .\n\t  FILTER (?aq_type IN (?a_coordinates_type, ?a_position_type, ?a_radius_type, ?a_pixels_type, ?a_image_band_type))\n\t}\n\t\n}"
     }
 }
```

### Comparing `renku-aqs-1.0.6/renkuaqs/graph_utils.py` & `renku-aqs-1.0.7/renkuaqs/graph_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,14 +303,22 @@
 
 def build_graph_image(revision, paths, filename, no_oda_info, input_notebook):
 
     if paths is None:
         paths = project_context.path
 
     graph = _renku_graph(revision, paths)
+
+    graph.bind("aqs", "http://www.w3.org/ns/aqs#")
+    graph.bind("oa", "http://www.w3.org/ns/oa#")
+    graph.bind("xsd", "http://www.w3.org/2001/XAQSchema#")
+    graph.bind("oda", "http://odahub.io/ontology#")
+    graph.bind("odas", "https://odahub.io/ontology#")
+    graph.bind("local-renku", f"file://{paths}/")
+
     renku_path = paths
 
     query_where = build_query_where(input_notebook=input_notebook, no_oda_info=no_oda_info)
     query_construct = build_query_construct(no_oda_info=no_oda_info)
 
     query = f"""{query_construct}
                {query_where}
```

### Comparing `renku-aqs-1.0.6/renkuaqs/icons/graph_icon.svg` & `renku-aqs-1.0.7/renkuaqs/icons/graph_icon.svg`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/renkuaqs/javascript_graph_utils.py` & `renku-aqs-1.0.7/renkuaqs/javascript_graph_utils.py`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/renkuaqs/ontology.ttl` & `renku-aqs-1.0.7/renkuaqs/ontology.ttl`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/renkuaqs/plugin.py` & `renku-aqs-1.0.7/renkuaqs/plugin.py`

 * *Files identical despite different names*

### Comparing `renku-aqs-1.0.6/setup.py` & `renku-aqs-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import find_packages, setup
 
 install_requires = [
     'deepdiff',
     'pydotplus',
     'rdflib',
     'bs4',
-    'renku==2.2.0',
+    'renku==2.6.0',
     'astroquery',
     'aqsconverters',
     'nb2workflow>=1.3.41',
     'pyvis==0.3.0',
     'pydotplus',
     'lockfile'
 ]
```

### Comparing `renku-aqs-1.0.6/tests/test_example.py` & `renku-aqs-1.0.7/tests/test_example.py`

 * *Files identical despite different names*

