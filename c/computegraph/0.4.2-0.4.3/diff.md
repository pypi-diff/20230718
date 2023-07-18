# Comparing `tmp/computegraph-0.4.2.tar.gz` & `tmp/computegraph-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computegraph-0.4.2.tar", max compression
+gzip compressed data, was "computegraph-0.4.3.tar", max compression
```

## Comparing `computegraph-0.4.2.tar` & `computegraph-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0      120 2023-02-10 03:25:56.177925 computegraph-0.4.2/computegraph/__init__.py
--rw-r--r--   0        0        0       37 2022-07-27 01:31:10.208964 computegraph-0.4.2/computegraph/draw/__init__.py
--rw-r--r--   0        0        0     6357 2022-07-27 01:31:10.209474 computegraph-0.4.2/computegraph/draw/add_edge.py
--rw-r--r--   0        0        0     4461 2023-02-10 03:25:56.178945 computegraph-0.4.2/computegraph/draw/draw.py
--rw-r--r--   0        0        0     1199 2022-07-27 01:31:10.209964 computegraph-0.4.2/computegraph/draw/ngraph.py
--rw-r--r--   0        0        0     1283 2022-07-27 01:31:10.208464 computegraph-0.4.2/computegraph/draw/README.md
--rw-r--r--   0        0        0     3108 2023-02-10 03:25:56.179927 computegraph-0.4.2/computegraph/dynamic.py
--rw-r--r--   0        0        0     6211 2023-04-04 19:58:26.736956 computegraph-0.4.2/computegraph/graph.py
--rw-r--r--   0        0        0     1989 2023-02-10 03:25:56.181926 computegraph-0.4.2/computegraph/jaxify.py
--rw-r--r--   0        0        0      490 2022-07-27 01:31:10.210965 computegraph-0.4.2/computegraph/options.py
--rw-r--r--   0        0        0     7400 2023-02-10 03:25:56.183431 computegraph-0.4.2/computegraph/types.py
--rw-r--r--   0        0        0    11697 2023-02-10 03:25:56.184364 computegraph-0.4.2/computegraph/utils.py
--rw-r--r--   0        0        0     1296 2022-07-27 01:31:10.207464 computegraph-0.4.2/LICENSE
--rw-r--r--   0        0        0     1272 2023-04-04 23:38:26.431064 computegraph-0.4.2/pyproject.toml
--rw-r--r--   0        0        0       88 2022-07-27 01:31:10.207965 computegraph-0.4.2/README.md
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 computegraph-0.4.2/setup.py
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 computegraph-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      120 2023-02-10 03:25:56.177925 computegraph-0.4.3/computegraph/__init__.py
+-rw-r--r--   0        0        0       37 2022-07-27 01:31:10.208964 computegraph-0.4.3/computegraph/draw/__init__.py
+-rw-r--r--   0        0        0     6357 2022-07-27 01:31:10.209474 computegraph-0.4.3/computegraph/draw/add_edge.py
+-rw-r--r--   0        0        0     4492 2023-04-26 00:33:51.036337 computegraph-0.4.3/computegraph/draw/draw.py
+-rw-r--r--   0        0        0     1199 2022-07-27 01:31:10.209964 computegraph-0.4.3/computegraph/draw/ngraph.py
+-rw-r--r--   0        0        0     1283 2022-07-27 01:31:10.208464 computegraph-0.4.3/computegraph/draw/README.md
+-rw-r--r--   0        0        0     3108 2023-02-10 03:25:56.179927 computegraph-0.4.3/computegraph/dynamic.py
+-rw-r--r--   0        0        0     6335 2023-04-26 01:01:04.663285 computegraph-0.4.3/computegraph/graph.py
+-rw-r--r--   0        0        0     1989 2023-02-10 03:25:56.181926 computegraph-0.4.3/computegraph/jaxify.py
+-rw-r--r--   0        0        0      490 2022-07-27 01:31:10.210965 computegraph-0.4.3/computegraph/options.py
+-rw-r--r--   0        0        0     7649 2023-07-17 22:22:34.936466 computegraph-0.4.3/computegraph/types.py
+-rw-r--r--   0        0        0    11697 2023-05-09 19:48:50.064014 computegraph-0.4.3/computegraph/utils.py
+-rw-r--r--   0        0        0     1296 2022-07-27 01:31:10.207464 computegraph-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1272 2023-07-18 01:40:26.110519 computegraph-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0       88 2022-07-27 01:31:10.207965 computegraph-0.4.3/README.md
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 computegraph-0.4.3/PKG-INFO
```

### Comparing `computegraph-0.4.2/computegraph/draw/add_edge.py` & `computegraph-0.4.3/computegraph/draw/add_edge.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.2/computegraph/draw/draw.py` & `computegraph-0.4.3/computegraph/draw/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         dag, pos=pos, labels=labels, node_color=node_colors, width=0.4, node_size=500, **kwargs
     )
 
 
 def draw_computegraph_plotly(
     dag: nx.DiGraph, targets: Optional[List[str]] = None, title: str = None, **kwargs
 ):
-
     if options.drawing["use_graphviz"]:
         pos = nx.nx_agraph.graphviz_layout(dag, prog="dot")
     else:
         pos = nx.spring_layout(dag)
 
     node_specs = nx.get_node_attributes(dag, "node_spec")
 
@@ -66,19 +65,20 @@
     tab_str = "&nbsp;" * 4
 
     def get_label_and_desc(name, node_spec):
         out_text = [name]
         if isinstance(node_spec, Function):
             if node_spec.func is assign:
                 label = name
-            else:
+            elif name.startswith("_"):
                 label = str(node_spec.func.__name__)
+            else:
+                label = name
+            out_text += ["function:"]
             out_text += [str(node_spec.func.__name__)]
-            out_text += ["node name:"]
-            out_text = [str(name)]
             out_text += ["args:"]
             out_text += [f"{tab_str}{arg}" for arg in node_spec.args]
             out_text += ["kwargs:"]
             out_text += [f"{tab_str}{k}: {v}" for k, v in node_spec.kwargs.items()]
         else:
             out_text += [str(node_spec)]
             label = name
```

### Comparing `computegraph-0.4.2/computegraph/draw/ngraph.py` & `computegraph-0.4.3/computegraph/draw/ngraph.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.2/computegraph/draw/README.md` & `computegraph-0.4.3/computegraph/draw/README.md`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.2/computegraph/dynamic.py` & `computegraph-0.4.3/computegraph/dynamic.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.2/computegraph/graph.py` & `computegraph-0.4.3/computegraph/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,7 +201,11 @@
             if targets is None:
                 targets = self._targets
 
         return build_callable(self.dag, targets, include_inputs, self.local_source_name)
 
     def __getitem__(self, key):
         return self.dag.nodes[key]["node_spec"]
+
+    def items(self):
+        for key, node_spec in self.dag.nodes.items():
+            yield (key, node_spec["node_spec"])
```

### Comparing `computegraph-0.4.2/computegraph/jaxify.py` & `computegraph-0.4.3/computegraph/jaxify.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.2/computegraph/types.py` & `computegraph-0.4.3/computegraph/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 import numpy as np
 
 from computegraph.jaxify import get_modules
 
 fnp = get_modules()["numpy"]
 
 
+# Helper for indexing function
+def getitem(obj, index):
+    return obj[index]
+
+
 class AbstractGraphObject(ABC):
     node_name = None
 
     @abstractmethod
     def evaluate(self, **sources):
         pass
 
@@ -67,21 +72,26 @@
 
     def __array_function__(self, func, types, args, kwargs):
         fnp = get_modules()["numpy"]
         fnp_attr = getattr(fnp, func.__name__)
         return Function(fnp_attr, args, kwargs)
 
     def __getitem__(self, idx):
-        return Function(lambda x, idx: x[idx], [self, idx])
+        return Function(getitem, [self, idx])
 
     def __iter__(self):
         # Without this we get stuck in infinite __getitem__ loops when containers
         # attempt to iterate on GraphObjects
         raise TypeError(f"{type(self)} object is not iterable")
 
+    def get_graph(self):
+        from .graph import ComputeGraph
+
+        return ComputeGraph(self)
+
     # def __getattr__(self, attr):
     #     try:
     #         np_attr = getattr(np, attr)
     #     except AttributeError:
     #         np_attr = None
 
     #     if isinstance(np_attr, np.ufunc):
@@ -120,16 +130,17 @@
             return False
 
     def evaluate(self, **sources):
         return sources[self.source][self.key]
 
 
 class Data(GraphObject):
-    def __init__(self, data):
+    def __init__(self, data, name=None):
         self.data = data
+        self.node_name = name
 
     def __repr__(self):
         return f"Data: {rrepr(self.data)}"
 
     def evaluate(self, **sources):
         return self.data
 
@@ -173,25 +184,26 @@
 
 class Function(GraphObject):
     """Universal wrapper for callable functions, whose args and kwargs
     may be either GraphObject (resolved at run-time), or any other Python value
     (regarded as constant)
     """
 
-    def __init__(self, func: callable, args: tuple = None, kwargs: dict = None):
+    def __init__(self, func: callable, args: tuple = None, kwargs: dict = None, name=None):
         self.func = func
         if args is None:
             args = ()
         if kwargs is None:
             kwargs = {}
         if not (isinstance(args, tuple) or isinstance(args, list)):
             raise TypeError("Args must be list or tuple", args)
         self.args = tuple(args)
         self.kwargs = kwargs
         self._validate_args()
+        self.node_name = name
 
     def _validate_args(self):
         _data_wrap = lambda x: x if isinstance(x, Hashable) else Data(x)
         self.args = tuple([_data_wrap(a) for a in self.args])
         self.kwargs = {k: _data_wrap(v) for k, v in self.kwargs.items()}
 
     def __hash__(self):
```

### Comparing `computegraph-0.4.2/computegraph/utils.py` & `computegraph-0.4.3/computegraph/utils.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.2/LICENSE` & `computegraph-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.2/pyproject.toml` & `computegraph-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "computegraph"
-version = "0.4.2"
+version = "0.4.3"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "https://github.com/monash-emu/computegraph"
 repository = "https://github.com/monash-emu/computegraph"
 documentation = "https://github.com/monash-emu/computegraph"
 keywords = [
     "graph",
```

### Comparing `computegraph-0.4.2/PKG-INFO` & `computegraph-0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: computegraph
-Version: 0.4.2
+Version: 0.4.3
 Summary: computegraph is a tool for managing computational graphs using networkx
 Home-page: https://github.com/monash-emu/computegraph
 License: BSD-2-Clause
 Keywords: graph,networkx,plotting,jax,summerepi2
 Author: David Shipman
 Author-email: dshipman@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: plotting
-Requires-Dist: jax[cpu] (>=0.4); sys_platform == "darwin"
-Requires-Dist: jax[cpu] (>=0.4); sys_platform == "linux"
-Requires-Dist: matplotlib (>=3.5.1); extra == "plotting"
+Requires-Dist: jax[cpu] (>=0.4) ; sys_platform == "darwin"
+Requires-Dist: jax[cpu] (>=0.4) ; sys_platform == "linux"
+Requires-Dist: matplotlib (>=3.5.1) ; extra == "plotting"
 Requires-Dist: networkx (>=2.6.2)
 Requires-Dist: numpy (>=1.20.3)
-Requires-Dist: plotly (>=5.6.0); extra == "plotting"
-Requires-Dist: pygraphviz (>=1.8); (sys_platform == "linux") and (extra == "plotting")
+Requires-Dist: plotly (>=5.6.0) ; extra == "plotting"
+Requires-Dist: pygraphviz (>=1.8) ; (sys_platform == "linux") and (extra == "plotting")
 Requires-Dist: scipy (>=1.7.3)
 Project-URL: Documentation, https://github.com/monash-emu/computegraph
 Project-URL: Repository, https://github.com/monash-emu/computegraph
 Description-Content-Type: text/markdown
 
 # computegraph
 Tools for managing computation graphs based on dictionaries and networkx
```

