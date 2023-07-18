# Comparing `tmp/circuitree-0.3.1.tar.gz` & `tmp/circuitree-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitree-0.3.1.tar", max compression
+gzip compressed data, was "circuitree-0.4.0.tar", max compression
```

## Comparing `circuitree-0.3.1.tar` & `circuitree-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.3.1/LICENSE
--rw-r--r--   0        0        0     1011 2023-06-09 16:36:39.964761 circuitree-0.3.1/README.md
--rwxr-xr-x   0        0        0      117 2023-06-23 05:39:39.142840 circuitree-0.3.1/circuitree/__init__.py
--rwxr-xr-x   0        0        0    15966 2023-07-13 21:38:18.014416 circuitree-0.3.1/circuitree/circuitree.py
--rwxr-xr-x   0        0        0    17012 2023-07-13 01:44:13.327169 circuitree-0.3.1/circuitree/models.py
--rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.3.1/circuitree/modularity.py
--rw-r--r--   0        0        0     9766 2023-07-14 02:05:56.385892 circuitree-0.3.1/circuitree/parallel.py
--rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.3.1/circuitree/regret.py
--rw-r--r--   0        0        0      750 2023-05-13 02:24:31.319175 circuitree-0.3.1/circuitree/rewards.py
--rw-r--r--   0        0        0     1442 2023-06-23 05:30:14.382829 circuitree-0.3.1/circuitree/utils.py
--rw-r--r--   0        0        0    10391 2023-06-28 20:54:12.669759 circuitree-0.3.1/circuitree/viz.py
--rw-r--r--   0        0        0     1813 2023-07-14 19:52:18.408930 circuitree-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 circuitree-0.3.1/setup.py
--rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 circuitree-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1011 2023-06-09 16:36:39.964761 circuitree-0.4.0/README.md
+-rwxr-xr-x   0        0        0      117 2023-06-23 05:39:39.142840 circuitree-0.4.0/circuitree/__init__.py
+-rwxr-xr-x   0        0        0    17548 2023-07-18 19:19:54.411916 circuitree-0.4.0/circuitree/circuitree.py
+-rwxr-xr-x   0        0        0    17012 2023-07-13 01:44:13.327169 circuitree-0.4.0/circuitree/models.py
+-rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.4.0/circuitree/modularity.py
+-rw-r--r--   0        0        0     9766 2023-07-14 23:28:38.055080 circuitree-0.4.0/circuitree/parallel.py
+-rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.4.0/circuitree/regret.py
+-rw-r--r--   0        0        0      750 2023-05-13 02:24:31.319175 circuitree-0.4.0/circuitree/rewards.py
+-rw-r--r--   0        0        0     1442 2023-06-23 05:30:14.382829 circuitree-0.4.0/circuitree/utils.py
+-rw-r--r--   0        0        0    10391 2023-06-28 20:54:12.669759 circuitree-0.4.0/circuitree/viz.py
+-rw-r--r--   0        0        0     1813 2023-07-18 19:21:46.231887 circuitree-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 circuitree-0.4.0/setup.py
+-rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 circuitree-0.4.0/PKG-INFO
```

### Comparing `circuitree-0.3.1/LICENSE` & `circuitree-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.1/README.md` & `circuitree-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.1/circuitree/circuitree.py` & `circuitree-0.4.0/circuitree/circuitree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from abc import ABC, abstractmethod
 from itertools import cycle, chain, repeat
+import json
+from pathlib import Path
 from typing import Callable, Literal, Optional, Iterable, Any
 import numpy as np
 import networkx as nx
 
 from .modularity import tree_modularity, tree_modularity_estimate
 
 
@@ -61,21 +63,24 @@
                 raise ValueError("Must specify seed if rg is not specified")
             else:
                 rg = np.random.default_rng(seed)
 
         self.rg = rg
         self.seed = self.rg.bit_generator._seed_seq.entropy
 
+        self.root = root
         if graph is None:
             self.graph = nx.DiGraph()
+            self.graph.add_node(self.root, visits=0, reward=0)
         else:
             self.graph = graph
-
-        self.root = root
-        self.graph.add_node(self.root, visits=0, reward=0)
+            if self.root not in self.graph:
+                raise ValueError(
+                    f"Supplied graph does not contain the root node: {root}"
+                )
 
         if tree_shape not in ("tree", "dag"):
             raise ValueError("Argument `tree_shape` must be `tree` or `dag`.")
         self.tree_shape = tree_shape
 
         if score_func is None:
             self._score_func = ucb_score
@@ -455,14 +460,58 @@
         graph.remove_nodes_from(nodes_to_remove)
 
         for n1, n2 in graph.edges:
             graph.edges[n1, n2].update(graph.nodes[n2])
 
         return graph, node, reward
 
+    def to_file(
+        self,
+        gml_file: str | Path,
+        json_file: Optional[str | Path] = None,
+        save_attrs: Optional[Iterable[str]] = None,
+        **kwargs,
+    ):
+        gml_target = Path(gml_file).with_suffix(".gml")
+        nx.write_gml(self.graph, gml_target, **kwargs)
+
+        if json_file is not None:
+            if save_attrs is None:
+                keys = set(self.__dict__.keys()) - set(["graph", "rg"])
+            else:
+                keys = set(save_attrs)
+
+            if "graph" in keys:
+                raise ValueError("Cannot serialize networkx DiGraph objects")
+            if "rg" in keys:
+                raise ValueError("Cannot serialize NumPy BitGenerator objects")
+
+            attrs = {k: v for k, v in self.__dict__.items() if k in keys}
+
+            json_target = Path(json_file).with_suffix(".json")
+            with json_target.open("w") as f:
+                json.dump(attrs, f, indent=4)
+
+            return gml_target, json_target
+
+        else:
+            return gml_target
+
+    @classmethod
+    def from_gml(
+        cls, graph_gml: str | Path, opts_json: Optional[str | Path] = None, **kwargs
+    ):
+        if opts_json is not None:
+            with open(opts_json, "r") as f:
+                kwargs.update(json.load(f))
+
+        graph = nx.read_gml(graph_gml)
+
+        return cls(graph=graph, **kwargs)
+
 
 def accumulate_visits_and_rewards(
     graph: nx.DiGraph, visits_attr: Any = "visits", reward_attr: Any = "reward"
 ):
     """Accumulate results on nodes post-hoc"""
     for n in graph.nodes:
         total_visits = sum([v for _, _, v in graph.in_edges(n, data=visits_attr)])
```

### Comparing `circuitree-0.3.1/circuitree/models.py` & `circuitree-0.4.0/circuitree/models.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.1/circuitree/modularity.py` & `circuitree-0.4.0/circuitree/modularity.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.1/circuitree/parallel.py` & `circuitree-0.4.0/circuitree/parallel.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.1/circuitree/rewards.py` & `circuitree-0.4.0/circuitree/rewards.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.1/circuitree/utils.py` & `circuitree-0.4.0/circuitree/utils.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.1/circuitree/viz.py` & `circuitree-0.4.0/circuitree/viz.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.1/pyproject.toml` & `circuitree-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circuitree"
-version = "0.3.1"
+version = "0.4.0"
 description = "Genetic circuit design using Monte Carlo tree search"
 authors = ["pranav-bhamidipati <pbhamidi@usc.edu>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `circuitree-0.3.1/setup.py` & `circuitree-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
               'pandas>=2.0.0,<3.0.0',
               'tables>=3.8.0,<4.0.0',
               'pyarrow>=12.0.0,<13.0.0',
               'h5py>=3.8.0,<4.0.0']}
 
 setup_kwargs = {
     'name': 'circuitree',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': 'Genetic circuit design using Monte Carlo tree search',
     'long_description': '# CircuiTree\nGenetic circuit design using Monte Carlo tree search\n\n## Installation\n\n### From a package repository\nTo install using `pip`:\n\n```pip install circuitree```\n\n### From the GitHub repository\n\nTo install and use `circuitree` from the GitHub source code, first clone the repo into a directory.\n\n```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```\n\nThen, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). \n\nFrom the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. \n\n## Usage\n\nSee the [quick-start demo](examples/quick_start.ipynb).\n',
     'author': 'pranav-bhamidipati',
     'author_email': 'pbhamidi@usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `circuitree-0.3.1/PKG-INFO` & `circuitree-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitree
-Version: 0.3.1
+Version: 0.4.0
 Summary: Genetic circuit design using Monte Carlo tree search
 License: GPLv3
 Author: pranav-bhamidipati
 Author-email: pbhamidi@usc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

