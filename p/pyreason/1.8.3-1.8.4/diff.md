# Comparing `tmp/pyreason-1.8.3.tar.gz` & `tmp/pyreason-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.8.3.tar", last modified: Fri Jul 14 17:05:45 2023, max compression
+gzip compressed data, was "pyreason-1.8.4.tar", last modified: Tue Jul 18 13:35:14 2023, max compression
```

## Comparing `pyreason-1.8.3.tar` & `pyreason-1.8.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.992014 pyreason-1.8.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-14 17:05:29.000000 pyreason-1.8.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 17:05:29.000000 pyreason-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-14 17:05:45.992014 pyreason-1.8.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-07-14 17:05:29.000000 pyreason-1.8.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.976014 pyreason-1.8.3/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.980014 pyreason-1.8.3/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.980014 pyreason-1.8.3/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    30332 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.980014 pyreason-1.8.3/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/facts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/facts/fact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    76573 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.988014 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.988014 pyreason-1.8.3/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.988014 pyreason-1.8.3/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.992014 pyreason-1.8.3/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/rule_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.980014 pyreason-1.8.3/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-14 17:05:45.000000 pyreason-1.8.3/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-14 17:05:45.000000 pyreason-1.8.3/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:05:45.000000 pyreason-1.8.3/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 17:05:45.000000 pyreason-1.8.3/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 17:05:45.000000 pyreason-1.8.3/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:05:45.992014 pyreason-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-14 17:05:29.000000 pyreason-1.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.992014 pyreason-1.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-14 17:05:29.000000 pyreason-1.8.3/tests/test_hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-18 13:35:03.000000 pyreason-1.8.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 13:35:03.000000 pyreason-1.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-18 13:35:14.621158 pyreason-1.8.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-07-18 13:35:03.000000 pyreason-1.8.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31359 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/facts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/facts/fact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77308 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5238 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2404 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4552 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/rule_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-18 13:35:14.000000 pyreason-1.8.4/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-18 13:35:14.000000 pyreason-1.8.4/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:35:14.000000 pyreason-1.8.4/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-18 13:35:14.000000 pyreason-1.8.4/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 13:35:14.000000 pyreason-1.8.4/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:35:14.621158 pyreason-1.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-18 13:35:03.000000 pyreason-1.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-18 13:35:03.000000 pyreason-1.8.4/tests/test_hello_world.py
```

### Comparing `pyreason-1.8.3/LICENSE.md` & `pyreason-1.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/PKG-INFO` & `pyreason-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.3
+Version: 1.8.4
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.3/README.md` & `pyreason-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/__init__.py` & `pyreason-1.8.4/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.8.4/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.8.4/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.8.4/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/pyreason.py` & `pyreason-1.8.4/pyreason/pyreason.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self.__reverse_digraph = False
         self.__atom_trace = False
         self.__save_graph_attributes_to_trace = False
         self.__canonical = False
         self.__inconsistency_check = True
         self.__static_graph_facts = True
         self.__store_interpretation_changes = True
+        self.__parallel_computing = False
 
     @property
     def verbose(self) -> bool:
         """Returns whether verbose mode is on or not. Default is True
 
         :return: bool
         """
@@ -142,14 +143,23 @@
         """Returns whether to keep track of changes that occur in the interpretation. You will not be able to view
         interpretation results after reasoning. Default is True
 
         :return: bool
         """
         return self.__store_interpretation_changes
 
+    @property
+    def parallel_computing(self) -> bool:
+        """Returns whether to use multiple CPU cores for inference. This will disable cacheing and pyreason will have
+        to be re-compiled at each run - but after compilation it will be faster. Default is False
+
+        :return: bool
+        """
+        return self.__parallel_computing
+
     @verbose.setter
     def verbose(self, value: bool) -> None:
         """Set verbose mode. Default is True
 
         :param value: verbose or not
         :raises TypeError: If not boolean, raise error
         """
@@ -303,14 +313,27 @@
         :raises TypeError: If not bool raise error
         """
         if not isinstance(value, bool):
             raise TypeError('value has to be a bool')
         else:
             self.__store_interpretation_changes = value
 
+    @parallel_computing.setter
+    def parallel_computing(self, value: bool) -> None:
+        """Whether to use multiple CPU cores for inference. This will disable cacheing and pyreason will have
+        to be re-compiled at each run - but after compilation it will be faster. Default is False
+
+        :param value: Whether to make inference run on parallel hardware (multiple CPU cores)
+        :raises TypeError: If not bool raise error
+        """
+        if not isinstance(value, bool):
+            raise TypeError('value has to be a bool')
+        else:
+            self.__parallel_computing = value
+
 
 # VARIABLES
 __graph = None
 __rules = None
 __node_facts = None
 __edge_facts = None
 __ipl = None
@@ -614,15 +637,15 @@
     if not settings.store_interpretation_changes:
         settings.atom_trace = False
 
     # Convert list of annotation functions into tuple to be numba compatible
     annotation_functions = tuple(__annotation_functions)
 
     # Setup logical program
-    __program = Program(__graph, all_node_facts, all_edge_facts, __rules, __ipl, annotation_functions, settings.reverse_digraph, settings.atom_trace, settings.save_graph_attributes_to_trace, settings.canonical, settings.inconsistency_check, settings.store_interpretation_changes)
+    __program = Program(__graph, all_node_facts, all_edge_facts, __rules, __ipl, annotation_functions, settings.reverse_digraph, settings.atom_trace, settings.save_graph_attributes_to_trace, settings.canonical, settings.inconsistency_check, settings.store_interpretation_changes, settings.parallel_computing)
     __program.available_labels_node = __node_labels
     __program.available_labels_edge = __edge_labels
     __program.specific_node_labels = __specific_node_labels
     __program.specific_edge_labels = __specific_edge_labels
 
     # Run Program and get final interpretation
     interpretation = __program.reason(timesteps, convergence_threshold, convergence_bound_threshold, settings.verbose)
```

### Comparing `pyreason-1.8.3/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.8.4/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/args.py` & `pyreason-1.8.4/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/components/world.py` & `pyreason-1.8.4/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/diffuse.py` & `pyreason-1.8.4/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/facts/fact.py` & `pyreason-1.8.4/pyreason/scripts/facts/fact.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.8.4/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/facts/fact_node.py` & `pyreason-1.8.4/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.8.4/pyreason/scripts/interpretation/interpretation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import pyreason.scripts.numba_wrapper.numba_types.world_type as world
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
 import pyreason.scripts.annotation_functions.annotation_functions as ann_fns
 
 import numba
-from numba import objmode
+from numba import objmode, prange
 
 
+# Parallel computing settings
+PARALLEL_COMPUTING = False
+CACHEING = True
+
 # Types for the dictionaries
 node_type = numba.types.string
 edge_type = numba.types.UniTuple(numba.types.string, 2)
 
 # Type for storing list of qualified nodes/edges
 list_of_nodes = numba.types.ListType(node_type)
 list_of_edges = numba.types.ListType(edge_type)
@@ -35,14 +39,16 @@
 	numba.types.ListType(numba.types.ListType(node_type)),
 	numba.types.ListType(numba.types.ListType(edge_type)),
 	numba.types.Tuple((numba.types.ListType(node_type), numba.types.ListType(node_type), label.label_type))
 ))
 
 
 class Interpretation:
+	parallel_computing = False
+	cacheing = True
 	available_labels_node = []
 	available_labels_edge = []
 	specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(node_type))
 	specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(edge_type))
 
 	def __init__(self, graph, ipl, annotation_functions, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes):
 		self.graph = graph
@@ -51,14 +57,19 @@
 		self.reverse_graph = reverse_graph
 		self.atom_trace = atom_trace
 		self.save_graph_attributes_to_rule_trace = save_graph_attributes_to_rule_trace
 		self.canonical = canonical
 		self.inconsistency_check = inconsistency_check
 		self.store_interpretation_changes = store_interpretation_changes
 
+		# Parallel computing settings
+		global PARALLEL_COMPUTING, CACHEING
+		PARALLEL_COMPUTING = self.parallel_computing
+		CACHEING = self.cacheing
+
 		# For reasoning and reasoning again (contains previous time and previous fp operation cnt)
 		self.time = 0
 		self.prev_reasoning_data = numba.typed.List([0, 0])
 
 		# Initialize list of tuples for rules/facts to be applied, along with all the ground atoms that fired the rule. One to One correspondence between rules_to_be_applied_node and rules_to_be_applied_node_trace if atom_trace is true
 		self.rules_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.rules_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
@@ -100,15 +111,15 @@
 			l = numba.typed.List.empty_list(node_type)
 			[l.append(neigh) for neigh in self.graph.neighbors(n)]
 			self.neighbors[n] = l
 
 		self.reverse_neighbors = self._init_reverse_neighbors(self.neighbors)
 
 	@staticmethod
-	@numba.njit(cache=True)
+	@numba.njit(cache=CACHEING)
 	def _init_reverse_neighbors(neighbors):
 		reverse_neighbors = numba.typed.Dict.empty(key_type=node_type, value_type=list_of_nodes)
 		for n, neighbor_nodes in neighbors.items():
 			for neighbor_node in neighbor_nodes:
 				if neighbor_node in reverse_neighbors and n not in reverse_neighbors[neighbor_node]:
 					reverse_neighbors[neighbor_node].append(n)
 				else:
@@ -116,43 +127,43 @@
 			# This makes sure each node has a value
 			if n not in reverse_neighbors:
 				reverse_neighbors[n] = numba.typed.List.empty_list(node_type)
 
 		return reverse_neighbors
 
 	@staticmethod
-	@numba.njit(cache=True)
+	@numba.njit(cache=CACHEING)
 	def _init_interpretations_node(nodes, available_labels, specific_labels):
 		interpretations = numba.typed.Dict.empty(key_type=node_type, value_type=world.world_type)
 		# General labels
 		for n in nodes:
 			interpretations[n] = world.World(available_labels)
 		# Specific labels
 		for l, ns in specific_labels.items():
 			for n in ns:
 				interpretations[n].world[l] = interval.closed(0.0, 1.0)
 
 		return interpretations
 	
 	@staticmethod
-	@numba.njit(cache=True)
+	@numba.njit(cache=CACHEING)
 	def _init_interpretations_edge(edges, available_labels, specific_labels):
 		interpretations = numba.typed.Dict.empty(key_type=edge_type, value_type=world.world_type)
 		# General labels
 		for e in edges:
 			interpretations[e] = world.World(available_labels)
 		# Specific labels
 		for l, es in specific_labels.items():
 			for e in es:
 				interpretations[e].world[l] = interval.closed(0.0, 1.0)
 
 		return interpretations
 	
 	@staticmethod
-	@numba.njit(cache=True)
+	@numba.njit(cache=CACHEING)
 	def _init_convergence(convergence_bound_threshold, convergence_threshold):
 		if convergence_bound_threshold==-1 and convergence_threshold==-1:
 			convergence_mode = 'perfect_convergence'
 			convergence_delta = 0
 		elif convergence_bound_threshold==-1:
 			convergence_mode = 'delta_interpretation'
 			convergence_delta = convergence_threshold
@@ -164,15 +175,15 @@
 	def start_fp(self, tmax, facts_node, facts_edge, rules, verbose, convergence_threshold, convergence_bound_threshold):
 		self.tmax = tmax
 		self._convergence_mode, self._convergence_delta = self._init_convergence(convergence_bound_threshold, convergence_threshold)
 		max_facts_time = self._init_facts(facts_node, facts_edge, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.atom_trace)
 		self._start_fp(rules, max_facts_time, verbose)
 
 	@staticmethod
-	@numba.njit(cache=True)
+	@numba.njit(cache=CACHEING)
 	def _init_facts(facts_node, facts_edge, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, atom_trace):
 		max_time = 0
 		for fact in facts_node:
 			for t in range(fact.get_time_lower(), fact.get_time_upper() + 1):
 				max_time = max(max_time, t)
 				name = fact.get_name()
 				graph_attribute = True if name=='graph-attribute-fact' else False
@@ -195,15 +206,15 @@
 		# If we need to reason again, store the next timestep to start from
 		self.prev_reasoning_data[0] = t
 		self.prev_reasoning_data[1] = fp_cnt
 		if verbose:
 			print('Fixed Point iterations:', fp_cnt)
 
 	@staticmethod
-	@numba.njit(cache=True)
+	@numba.njit(cache=CACHEING)
 	def reason(interpretations_node, interpretations_edge, tmax, prev_reasoning_data, rules, nodes, edges, neighbors, reverse_neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes, max_facts_time, annotation_functions, convergence_mode, convergence_delta, verbose):
 		t = prev_reasoning_data[0]
 		fp_cnt = prev_reasoning_data[1]
 		max_rules_time = 0
 		timestep_loop = True
 		facts_to_be_applied_node_new = numba.typed.List.empty_list(facts_to_be_applied_node_type)
 		facts_to_be_applied_edge_new = numba.typed.List.empty_list(facts_to_be_applied_edge_type)
@@ -677,15 +688,15 @@
 		_add_edge(edge[0], edge[1], self.neighbors, self.reverse_neighbors, self.nodes, self.edges, l, self.interpretations_node, self.interpretations_edge)
 
 	def delete_edge(self, edge):
 		# This function is useful for pyreason gym, called externally
 		_delete_edge(edge, self.neighbors, self.reverse_neighbors, self.edges, self.interpretations_edge)
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING, parallel=PARALLEL_COMPUTING)
 def _ground_node_rule(rule, interpretations_node, interpretations_edge, nodes, neighbors, reverse_neighbors, atom_trace, reverse_graph, nodes_to_skip):
 	# Extract rule params
 	rule_type = rule.get_type()
 	clauses = rule.get_clauses()
 	thresholds = rule.get_thresholds()
 	ann_fn = rule.get_annotation_function()
 	rule_edges = rule.get_edges()
@@ -700,15 +711,16 @@
 	# Steps
 	# 1. Loop through all nodes and evaluate each clause with that node and check the truth with the thresholds
 	# 2. Inside the clause loop it may be necessary to loop through all nodes/edges while grounding the variables
 	# 3. If the clause is true add the qualified nodes and qualified edges to the atom trace, if on. Break otherwise
 	# 4. After going through all clauses, add to the annotations list all the annotations of the specified subset. These will be passed to the annotation function
 	# 5. Finally, if there are any edges to be added, place them in the list
 
-	for target_node in nodes:
+	for piter in prange(len(nodes)):
+		target_node = nodes[piter]
 		if target_node in nodes_to_skip:
 			continue
 		# Initialize dictionary where keys are strings (x1, x2 etc.) and values are lists of qualified neighbors
 		# Keep track of qualified nodes and qualified edges
 		# If it's a node clause update (x1 or x2 etc.) qualified neighbors, if it's an edge clause update the qualified neighbors for the source and target (x1, x2)
 		subsets = numba.typed.Dict.empty(key_type=numba.types.string, value_type=list_of_nodes)
 		qualified_nodes = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
@@ -862,15 +874,15 @@
 
 			# node/edge, annotations, qualified nodes, qualified edges, edges to be added
 			applicable_rules.append((target_node, annotations, qualified_nodes, qualified_edges, edges_to_be_added))
 
 	return applicable_rules
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING, parallel=PARALLEL_COMPUTING)
 def _ground_edge_rule(rule, interpretations_node, interpretations_edge, nodes, edges, neighbors, reverse_neighbors, atom_trace, reverse_graph, edges_to_skip):
 	# Extract rule params
 	rule_type = rule.get_type()
 	clauses = rule.get_clauses()
 	thresholds = rule.get_thresholds()
 	ann_fn = rule.get_annotation_function()
 	rule_edges = rule.get_edges()
@@ -885,15 +897,16 @@
 	# Steps
 	# 1. Loop through all nodes and evaluate each clause with that node and check the truth with the thresholds
 	# 2. Inside the clause loop it may be necessary to loop through all nodes/edges while grounding the variables
 	# 3. If the clause is true add the qualified nodes and qualified edges to the atom trace, if on. Break otherwise
 	# 4. After going through all clauses, add to the annotations list all the annotations of the specified subset. These will be passed to the annotation function
 	# 5. Finally, if there are any edges to be added, place them in the list
 
-	for target_edge in edges:
+	for piter in prange(len(edges)):
+		target_edge = edges[piter]
 		if target_edge in edges_to_skip:
 			continue
 		# Initialize dictionary where keys are strings (x1, x2 etc.) and values are lists of qualified neighbors
 		# Keep track of qualified nodes and qualified edges
 		# If it's a node clause update (x1 or x2 etc.) qualified neighbors, if it's an edge clause update the qualified neighbors for the source and target (x1, x2)
 		subsets = numba.typed.Dict.empty(key_type=numba.types.string, value_type=list_of_nodes)
 		qualified_nodes = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
@@ -1075,41 +1088,41 @@
 
 			# node/edge, annotations, qualified nodes, qualified edges, edges to be added
 			applicable_rules.append((target_edge, annotations, qualified_nodes, qualified_edges, edges_to_be_added))
 
 	return applicable_rules
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def get_qualified_components_node_clause(interpretations_node, candidates, l, bnd):
 	# Get all the qualified neighbors for a particular clause
 	qualified_nodes = numba.typed.List.empty_list(node_type)
 	for n in candidates:
 		if is_satisfied_node(interpretations_node, n, (l, bnd)):
 			qualified_nodes.append(n)
 
 	return qualified_nodes
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def get_qualified_components_edge_clause(interpretations_edge, candidates_source, candidates_target, l, bnd, reverse_graph):
 	# Get all the qualified sources and targets for a particular clause
 	qualified_nodes_source = numba.typed.List.empty_list(node_type)
 	qualified_nodes_target = numba.typed.List.empty_list(node_type)
 	for i, source in enumerate(candidates_source):
 		for target in candidates_target[i]:
 			edge = (source, target) if not reverse_graph else (target, source)
 			if is_satisfied_edge(interpretations_edge, edge, (l, bnd)):
 				qualified_nodes_source.append(source)
 				qualified_nodes_target.append(target)
 
 	return (qualified_nodes_source, qualified_nodes_target)
 	
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def _satisfies_threshold(num_neigh, num_qualified_component, threshold):
 	# Checks if qualified neighbors satisfy threshold. This is for one clause
 	if threshold[1][0]=='number':
 		if threshold[0]=='greater_equal':
 			result = True if num_qualified_component >= threshold[2] else False
 		elif threshold[0]=='greater':
 			result = True if num_qualified_component > threshold[2] else False
@@ -1133,15 +1146,15 @@
 			result = True if num_qualified_component/num_neigh < threshold[2]*0.01 else False
 		elif threshold[0]=='equal':
 			result = True if num_qualified_component/num_neigh == threshold[2]*0.01 else False
 
 	return result
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def _update_node(interpretations, comp, na, ipl, rule_trace, fp_cnt, t_cnt, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_trace, idx, facts_to_be_applied_trace, rule_trace_atoms, store_interpretation_changes, mode, override=False):
 	updated = False
 	# This is to prevent a key error in case the label is a specific label
 	try:
 		world = interpretations[comp]
 		l, bnd = na
 		updated_bnds = numba.typed.List.empty_list(interval.interval_type)
@@ -1149,19 +1162,23 @@
 		# Add label to world if it is not there
 		if l not in world.world:
 			world.world[l] = interval.closed(0, 1)
 
 		# Check if update is necessary with previous bnd
 		prev_bnd = world.world[l].copy()
 
-		# override will not check for inconsistencies
-		if override:
-			world.world[l].set_lower_upper(bnd.lower, bnd.upper)
+		if l.value == 'normal' or l.value == 'abnormal':
+			world.update_average(l, bnd)
 		else:
-			world.update(l, bnd)
+			# override will not check for inconsistencies
+			if override:
+				world.world[l].set_lower_upper(bnd.lower, bnd.upper)
+			else:
+				world.update_intersection(l, bnd)
+
 		world.world[l].set_static(static)
 		if world.world[l]!=prev_bnd:
 			updated = True
 			updated_bnds.append(world.world[l])
 
 			# Add to rule trace if update happened and add to atom trace if necessary
 			if (save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact') and store_interpretation_changes:
@@ -1222,15 +1239,15 @@
 
 		return (updated, change)
 
 	except:
 		return (False, 0)
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def _update_edge(interpretations, comp, na, ipl, rule_trace, fp_cnt, t_cnt, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_trace, idx, facts_to_be_applied_trace, rule_trace_atoms, store_interpretation_changes, mode, override=False):
 	updated = False
 	# This is to prevent a key error in case the label is a specific label
 	try:
 		world = interpretations[comp]
 		l, bnd = na
 		updated_bnds = numba.typed.List.empty_list(interval.interval_type)
@@ -1238,19 +1255,23 @@
 		# Add label to world if it is not there
 		if l not in world.world:
 			world.world[l] = interval.closed(0, 1)
 
 		# Check if update is necessary with previous bnd
 		prev_bnd = world.world[l].copy()
 
-		# override will not check for inconsistencies
-		if override:
-			world.world[l].set_lower_upper(bnd.lower, bnd.upper)
+		if l.value == 'normal' or l.value == 'abnormal':
+			world.update_average(l, bnd)
 		else:
-			world.update(l, bnd)
+			# override will not check for inconsistencies
+			if override:
+				world.world[l].set_lower_upper(bnd.lower, bnd.upper)
+			else:
+				world.update_intersection(l, bnd)
+
 		world.world[l].set_static(static)
 		if world.world[l]!=prev_bnd:
 			updated = True
 			updated_bnds.append(world.world[l])
 
 			# Add to rule trace if update happened and add to atom trace if necessary
 			if (save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact') and store_interpretation_changes:
@@ -1310,105 +1331,105 @@
 					change = 1 + ip_update_cnt
 		
 		return (updated, change)
 	except:
 		return (False, 0)
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def _update_rule_trace(rule_trace, qn, qe, prev_bnd, name):
 	rule_trace.append((qn, qe, prev_bnd.copy(), name))
 	
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def are_satisfied_node(interpretations, comp, nas):
 	result = True
 	for (label, interval) in nas:
 		result = result and is_satisfied_node(interpretations, comp, (label, interval))
 	return result
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def is_satisfied_node(interpretations, comp, na):
 	result = False
 	if (not (na[0] is None or na[1] is None)):
 		# This is to prevent a key error in case the label is a specific label
 		try:
 			world = interpretations[comp]
 			result = world.is_satisfied(na[0], na[1])
 		except:
 			result = False
 	else:
 		result = True
 	return result
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def are_satisfied_edge(interpretations, comp, nas):
 	result = True
 	for (label, interval) in nas:
 		result = result and is_satisfied_edge(interpretations, comp, (label, interval))
 	return result
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def is_satisfied_edge(interpretations, comp, na):
 	result = False
 	if (not (na[0] is None or na[1] is None)):
 		# This is to prevent a key error in case the label is a specific label
 		try:
 			world = interpretations[comp]
 			result = world.is_satisfied(na[0], na[1])
 		except:
 			result = False
 	else:
 		result = True
 	return result
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def annotate(annotation_functions, rule, annotations, weights):
 	func_name = rule.get_annotation_function()
 	if func_name == '':
 		return rule.get_bnd().lower, rule.get_bnd().upper
 	else:
 		with numba.objmode(annotation='Tuple((float64, float64))'):
 			for func in annotation_functions:
 				if func.__name__ == func_name:
 					annotation = func(annotations, weights)
 		return annotation
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def check_consistent_node(interpretations, comp, na):
 	world = interpretations[comp]
 	if na[0] in world.world:
 		bnd = world.world[na[0]]
 	else:
 		bnd = interval.closed(0, 1)
 	if (na[1].lower > bnd.upper) or (bnd.lower > na[1].upper):
 		return False
 	else:
 		return True
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def check_consistent_edge(interpretations, comp, na):
 	world = interpretations[comp]
 	if na[0] in world.world:
 		bnd = world.world[na[0]]
 	else:
 		bnd = interval.closed(0, 1)
 	if (na[1].lower > bnd.upper) or (bnd.lower > na[1].upper):
 		return False
 	else:
 		return True
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def resolve_inconsistency_node(interpretations, comp, na, ipl, t_cnt, fp_cnt, atom_trace, rule_trace, rule_trace_atoms, store_interpretation_changes):
 	world = interpretations[comp]
 	if store_interpretation_changes:
 		rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, na[0], interval.closed(0,1)))
 		if atom_trace:
 			_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[na[0]], 'Inconsistency')
 	# Resolve inconsistency and set static
@@ -1429,15 +1450,15 @@
 			world.world[p1].set_lower_upper(0, 1)
 			world.world[p1].set_static(True)
 			if store_interpretation_changes:
 				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
 	# Add inconsistent predicates to a list 
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def resolve_inconsistency_edge(interpretations, comp, na, ipl, t_cnt, fp_cnt, atom_trace, rule_trace, rule_trace_atoms, store_interpretation_changes):
 	w = interpretations[comp]
 	if store_interpretation_changes:
 		rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, na[0], interval.closed(0,1)))
 		if atom_trace:
 			_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), w.world[na[0]], 'Inconsistency')
 	# Resolve inconsistency and set static
@@ -1457,23 +1478,23 @@
 				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), w.world[p1], 'Inconsistency')
 			w.world[p1].set_lower_upper(0, 1)
 			w.world[p1].set_static(True)
 			if store_interpretation_changes:
 				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def _add_node(node, neighbors, reverse_neighbors, nodes, interpretations_node):
 	nodes.append(node)
 	neighbors[node] = numba.typed.List.empty_list(node_type)
 	reverse_neighbors[node] = numba.typed.List.empty_list(node_type)
 	interpretations_node[node] = world.World(numba.typed.List.empty_list(label.label_type))
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def _add_edge(source, target, neighbors, reverse_neighbors, nodes, edges, l, interpretations_node, interpretations_edge):
 	# If not a node, add to list of nodes and initialize neighbors
 	if source not in nodes:
 		_add_node(source, neighbors, reverse_neighbors, nodes, interpretations_node)
 
 	if target not in nodes:
 		_add_node(target, neighbors, reverse_neighbors, nodes, interpretations_node)
@@ -1496,33 +1517,34 @@
 		if l not in interpretations_edge[edge].world and l.value!='':
 			new_edge = True
 			interpretations_edge[edge].world[l] = interval.closed(0, 1)
 
 	return (edge, new_edge)
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def _add_edges(sources, targets, neighbors, reverse_neighbors, nodes, edges, l, interpretations_node, interpretations_edge):
 	changes = 0
 	edges_added = numba.typed.List.empty_list(edge_type)
 	for source in sources:
 		for target in targets:
 			edge, new_edge = _add_edge(source, target, neighbors, reverse_neighbors, nodes, edges, l, interpretations_node, interpretations_edge)
 			edges_added.append(edge)
 			changes = changes+1 if new_edge else changes
 	return (edges_added, changes)
 
-@numba.njit(cache=True)
+
+@numba.njit(cache=CACHEING)
 def _delete_edge(edge, neighbors, reverse_neighbors, edges, interpretations_edge):
 	source, target = edge
 	edges.remove(edge)
 	del interpretations_edge[edge]
 	neighbors[source].remove(target)
 	reverse_neighbors[target].remove(source)
 
 
-@numba.njit(cache=True)
+@numba.njit(cache=CACHEING)
 def float_to_str(value):
 	number = int(value)
 	decimal = int(value % 1 * 1000)
 	float_str = f'{number}.{decimal}'
 	return float_str
```

### Comparing `pyreason-1.8.3/pyreason/scripts/interval/interval.py` & `pyreason-1.8.4/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,19 +96,30 @@
         result = False
         bnd = world.world[label]
         result = bnd in interval
 
         return result
     return impl
 
-@overload_method(WorldType, 'update')
-def update(w, label, interval):
-    def impl(w, label, interval):       
+@overload_method(WorldType, 'update_intersection')
+def update_intersection(w, label, bnd):
+    def impl(w, label, bnd):       
         current_bnd = w.world[label]
-        new_bnd = current_bnd.intersection(interval)
+        new_bnd = current_bnd.intersection(bnd)
+        w.world[label] = new_bnd
+    return impl
+
+@overload_method(WorldType, 'update_average')
+def update_average(w, label, bnd):
+    def impl(w, label, bnd):       
+        current_bnd = w.world[label]
+        if current_bnd.lower == 0 and current_bnd.upper == 1:
+            new_bnd = interval.closed(bnd.lower, bnd.upper)
+        else:
+            new_bnd = interval.closed((bnd.lower + current_bnd.lower)/2, (bnd.upper + current_bnd.upper)/2)
         w.world[label] = new_bnd
     return impl
 
 @overload_method(WorldType, 'get_bound')
 def get_bound(world, label):
     def impl(world, label):
         result = None
```

### Comparing `pyreason-1.8.3/pyreason/scripts/program/program.py` & `pyreason-1.8.4/pyreason/scripts/program/program.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,37 +3,43 @@
 
 class Program:
 	available_labels_node = []
 	available_labels_edge = []
 	specific_node_labels = []
 	specific_edge_labels = []
 
-	def __init__(self, graph, facts_node, facts_edge, rules, ipl, annotation_functions, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes):
+	def __init__(self, graph, facts_node, facts_edge, rules, ipl, annotation_functions, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes, parallel_computing):
 		self._graph = graph
 		self._facts_node = facts_node
 		self._facts_edge = facts_edge
 		self._rules = rules
 		self._ipl = ipl
 		self._annotation_functions = annotation_functions
 		self._reverse_graph = reverse_graph
 		self._atom_trace = atom_trace
 		self._save_graph_attributes_to_rule_trace = save_graph_attributes_to_rule_trace
 		self._canonical = canonical
 		self._inconsistency_check = inconsistency_check
 		self._store_interpretation_changes = store_interpretation_changes
+		self._parallel_computing = parallel_computing
 		self.interp = None
 
 	def reason(self, tmax, convergence_threshold, convergence_bound_threshold, verbose=True):
 		self._tmax = tmax
 		# Set up available labels
 		Interpretation.available_labels_node = self.available_labels_node
 		Interpretation.available_labels_edge = self.available_labels_edge
 		Interpretation.specific_node_labels = self.specific_node_labels
 		Interpretation.specific_edge_labels = self.specific_edge_labels
 
+		# Set up parallel computing settings (we cannot cache with parallel=True)
+		Interpretation.parallel_computing = self._parallel_computing
+		if self._parallel_computing:
+			Interpretation.cacheing = False
+
 		self.interp = Interpretation(self._graph, self._ipl, self._annotation_functions, self._reverse_graph, self._atom_trace, self._save_graph_attributes_to_rule_trace, self._canonical, self._inconsistency_check, self._store_interpretation_changes)
 		self.interp.start_fp(self._tmax, self._facts_node, self._facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold)
 
 		return self.interp
 	
 	def reason_again(self, tmax, convergence_threshold, convergence_bound_threshold, facts_node, facts_edge, verbose=True):
 		assert self.interp is not None, 'Call reason before calling reason again'
```

### Comparing `pyreason-1.8.3/pyreason/scripts/rules/rule.py` & `pyreason-1.8.4/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/utils/filter.py` & `pyreason-1.8.4/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.8.4/pyreason/scripts/utils/graphml_parser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 
                 if label.Label(l) not in specific_edge_labels.keys():
                     specific_edge_labels[label.Label(l)] = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.string)))
                 specific_edge_labels[label.Label(l)].append((e[0], e[1]))
                 f = fact_edge.Fact('graph-attribute-fact', (e[0], e[1]), label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0, static=static_facts)
                 facts_edge.append(f)
 
-        return facts_node, facts_edge, specific_node_labels, specific_edge_labels
+        return facts_node, facts_edge, specific_node_labels, specific_edge_labels
```

### Comparing `pyreason-1.8.3/pyreason/scripts/utils/output.py` & `pyreason-1.8.4/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/utils/plotter.py` & `pyreason-1.8.4/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/utils/rule_parser.py` & `pyreason-1.8.4/pyreason/scripts/utils/rule_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/utils/visuals.py` & `pyreason-1.8.4/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.8.4/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/pyreason.egg-info/PKG-INFO` & `pyreason-1.8.4/pyreason.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.3
+Version: 1.8.4
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.3/pyreason.egg-info/SOURCES.txt` & `pyreason-1.8.4/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.3/setup.py` & `pyreason-1.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyreason',
-    version='1.8.3',
+    version='1.8.4',
     author='Dyuman Aditya',
     author_email='dyuman.aditya@gmail.com',
     description='An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lab-v2/pyreason',
     license='BSD 3-clause',
```

### Comparing `pyreason-1.8.3/tests/test_hello_world.py` & `pyreason-1.8.4/tests/test_hello_world.py`

 * *Files identical despite different names*

