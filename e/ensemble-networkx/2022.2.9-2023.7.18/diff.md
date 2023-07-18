# Comparing `tmp/ensemble_networkx-2022.2.9.tar.gz` & `tmp/ensemble_networkx-2023.7.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensemble_networkx-2022.2.9.tar", last modified: Wed Feb  9 21:06:59 2022, max compression
+gzip compressed data, was "ensemble_networkx-2023.7.18.tar", last modified: Tue Jul 18 19:15:29 2023, max compression
```

## Comparing `ensemble_networkx-2022.2.9.tar` & `ensemble_networkx-2023.7.18.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 jespinoz  (3456) tigr        (63)        0 2022-02-09 21:06:59.421461 ensemble_networkx-2022.2.9/
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)     2026 2020-07-03 01:51:37.000000 ensemble_networkx-2022.2.9/LICENSE.txt
--rw-r--r--   0 jespinoz  (3456) tigr        (63)      284 2022-02-09 21:06:59.421157 ensemble_networkx-2022.2.9/PKG-INFO
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)    12918 2021-10-26 19:27:19.000000 ensemble_networkx-2022.2.9/README.md
-drwxr-xr-x   0 jespinoz  (3456) tigr        (63)        0 2022-02-09 21:06:59.411455 ensemble_networkx-2022.2.9/ensemble_networkx/
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)     3015 2022-02-09 21:02:12.000000 ensemble_networkx-2022.2.9/ensemble_networkx/__init__.py
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)   114002 2022-02-09 21:01:04.000000 ensemble_networkx-2022.2.9/ensemble_networkx/ensemble_networkx.py
-drwxr-xr-x   0 jespinoz  (3456) tigr        (63)        0 2022-02-09 21:06:59.419929 ensemble_networkx-2022.2.9/ensemble_networkx.egg-info/
--rw-------   0 jespinoz  (3456) tigr        (63)        0 2022-02-09 20:00:58.000000 ensemble_networkx-2022.2.9/ensemble_networkx.egg-info/Icon
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)      284 2022-02-09 21:06:59.000000 ensemble_networkx-2022.2.9/ensemble_networkx.egg-info/PKG-INFO
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)      336 2022-02-09 21:06:59.000000 ensemble_networkx-2022.2.9/ensemble_networkx.egg-info/SOURCES.txt
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)        1 2022-02-09 21:06:59.000000 ensemble_networkx-2022.2.9/ensemble_networkx.egg-info/dependency_links.txt
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)      116 2022-02-09 21:06:59.000000 ensemble_networkx-2022.2.9/ensemble_networkx.egg-info/requires.txt
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)       18 2022-02-09 21:06:59.000000 ensemble_networkx-2022.2.9/ensemble_networkx.egg-info/top_level.txt
--rw-r--r--   0 jespinoz  (3456) tigr        (63)       38 2022-02-09 21:06:59.421558 ensemble_networkx-2022.2.9/setup.cfg
--rwxrwxr-x   0 jespinoz  (3456) tigr        (63)      886 2022-02-09 21:02:44.000000 ensemble_networkx-2022.2.9/setup.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-18 19:15:29.468668 ensemble_networkx-2023.7.18/
+-rw-------   0 jespinoz  (3456) staff       (20)     1563 2023-07-18 19:13:30.000000 ensemble_networkx-2023.7.18/LICENSE
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      281 2023-07-18 19:15:29.468349 ensemble_networkx-2023.7.18/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)    12928 2023-07-18 19:15:16.000000 ensemble_networkx-2023.7.18/README.md
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-18 19:15:29.465787 ensemble_networkx-2023.7.18/ensemble_networkx/
+-rw-------   0 jespinoz  (3456) staff       (20)     2986 2023-07-18 18:45:57.000000 ensemble_networkx-2023.7.18/ensemble_networkx/__init__.py
+-rw-------   0 jespinoz  (3456) staff       (20)   117136 2023-07-18 19:11:44.000000 ensemble_networkx-2023.7.18/ensemble_networkx/ensemble_networkx.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-18 19:15:29.467862 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/
+-rw-------   0 jespinoz  (3456) staff       (20)      281 2023-07-18 19:15:29.000000 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)      299 2023-07-18 19:15:29.000000 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/SOURCES.txt
+-rw-------   0 jespinoz  (3456) staff       (20)        1 2023-07-18 19:15:29.000000 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/dependency_links.txt
+-rw-------   0 jespinoz  (3456) staff       (20)      116 2023-07-18 19:15:29.000000 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/requires.txt
+-rw-------   0 jespinoz  (3456) staff       (20)       18 2023-07-18 19:15:29.000000 ensemble_networkx-2023.7.18/ensemble_networkx.egg-info/top_level.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-07-18 19:15:29.468798 ensemble_networkx-2023.7.18/setup.cfg
+-rw-------   0 jespinoz  (3456) staff       (20)      886 2022-02-09 21:02:44.000000 ensemble_networkx-2023.7.18/setup.py
```

### Comparing `ensemble_networkx-2022.2.9/LICENSE.txt` & `ensemble_networkx-2023.7.18/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# ==============
-# Ensemble NetworkX
-# ==============
-# Ensemble network methods in Python
-# ------------------------------------
-# GitHub: https://github.com/jolespin/ensemble_networkx
-# PyPI: https://pypi.org/project/ensemble_networkx
-# ------------------------------------
-# =======
-# Contact
-# =======
-# Producer: Josh L. Espinoza
-# Contact: jespinoz@jcvi.org, jol.espinoz@gmail.com
-# Google Scholar: https://scholar.google.com/citations?user=r9y1tTQAAAAJ&hl
 # =======
 # License BSD-3
 # =======
 # https://opensource.org/licenses/BSD-3-Clause
 #
 # Copyright 2018 Josh L. Espinoza
 #
```

### Comparing `ensemble_networkx-2022.2.9/README.md` & `ensemble_networkx-2023.7.18/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 
 
    * Nabwera HM+, Espinoza JL+, Worwui A, Betts M, Okoi C, Sesay AK, Bancroft R, Agbla SC, Jarju S, Bradbury RS, Colley M, Jallow AT, Liu J, Houpt ER, Prentice AM, Antonio M, Bernstein RM, Dupont CL+, Kwambana-Adams BA+. *Interactions between fecal gut microbiome, enteric pathogens, and energy regulating hormones among acutely malnourished rural Gambian children*. EBioMedicine. 2021 Oct 22;73:103644. [doi: 10.1016/j.ebiom.2021.103644](https://doi.org/10.1016/j.ebiom.2021.103644). PMID: 34695658.
 
 
 #### Install:
 ```
-# "Stable" release (still developmental)
+# Stable release (Preferred)
 pip install ensemble_networkx
-# Current release
+
+# Current developmental release
 pip install git+https://github.com/jolespin/ensemble_networkx
 ```
 
 #### Source:
 * Migrated from [`soothsayer`](https://github.com/jolespin/soothsayer)
 
 #### Case studies, tutorials and usage:
@@ -41,15 +42,15 @@
 ```
 
 ##### Simple case of an [iris dataset](https://en.wikipedia.org/wiki/Iris_flower_data_set) ensemble network
 
 ```python
 # Load in data
 import soothsayer_utils as syu
-X = syu.get_iris_data(["X"])
+X,y = syu.get_iris_data(["X", "y"])
 
 # Create ensemble network
 ens = enx.EnsembleAssociationNetwork(name="Iris", node_type="leaf measurement", edge_type="association", observation_type="specimen")
 ens.fit(X=X, metric="spearman",  n_iter=100, stats_summary=[np.mean,np.var, stats.kurtosis, stats.skew], stats_tests=[stats.normaltest], copy_ensemble=True)
 print(ens)
 # =======================================================
 # EnsembleAssociationNetwork(Name:Iris, Metric: spearman)
```

### Comparing `ensemble_networkx-2022.2.9/ensemble_networkx/__init__.py` & `ensemble_networkx-2023.7.18/ensemble_networkx/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,30 +29,29 @@
 #
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 #
 # =======
 # Version
 # =======
-__version__= "2022.2.9"
+__version__= "2023.7.18"
 __author__ = "Josh L. Espinoza"
 __email__ = "jespinoz@jcvi.org, jol.espinoz@gmail.com"
 __url__ = "https://github.com/jolespin/ensemble_networkx"
 __license__ = "BSD-3"
 __developmental__ = True
 
 # =======
 # Direct Exports
 # =======
 __functions__ = [
     "pairwise_biweight_midcorrelation",
     "umap_fuzzy_simplical_set_graph",
 ] + [
     "signed",
-    "get_weights_from_graph",
     "get_symmetric_category",
     "dense_to_condensed",
     "condensed_to_dense",
     "convert_network",
 ] + [
     "connectivity",
     "density",
```

### Comparing `ensemble_networkx-2022.2.9/ensemble_networkx/ensemble_networkx.py` & `ensemble_networkx-2023.7.18/ensemble_networkx/ensemble_networkx.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 # Built-ins
 import os, sys, time, datetime, copy, warnings
 from typing import Dict, Union, Any
 from collections import defaultdict, OrderedDict
 from collections.abc import Mapping, Hashable
 from itertools import combinations, product
 
-# PyData
+# Packages
 import pandas as pd
 import numpy as np
 import networkx as nx
+import igraph as ig
 import xarray as xr
 from scipy import stats
 from scipy.special import comb
 from scipy.spatial.distance import squareform, pdist
 
 # Compositional
 from compositional import pairwise_rho, pairwise_phi
@@ -27,64 +28,35 @@
 from soothsayer_utils import pv, flatten, assert_acceptable_arguments, is_symmetrical, is_graph, write_object, format_memory, format_header, format_path, is_nonstring_iterable, Suppress, dict_build, dict_filter, is_dict, is_dict_like, is_color, is_number, check_packages, is_query_class
 
 try:
     from . import __version__
 except ImportError:
     __version__ = "ImportError: attempted relative import with no known parent package"
 
-# ===================s
-# Transformations
-# ===================
-# Unsigned network to signed network
-def signed(X):
-    """
-    unsigned -> signed correlation
-    """
-    return (X + 1)/2
-
-# ===================s
-# Transformations
-# ===================
-
-
-
 
 # ===================
 # Converting Networks
-# ===================
-#Get weights from graph
-def get_weights_from_graph(graph, into=np.asarray, weight="weight",  generator=False):
-    weights = map(lambda edge_data: edge_data[-1][weight], graph.edges(data=True))
-    if generator:
-        return weights
-    else:
-        weights = list(weights)
-        return into(weights)
-        
+# ===================  
+# Remove self-loops
+def remove_self_edges(graph):
+    self_edges = list(nx.selfloop_edges(graph))
+    return graph.remove_edges_from(self_edges)
+
 # pd.DataFrame 2D to pd.Series
 def dense_to_condensed(X, name=None, assert_symmetry=True, tol=None, nans_ok=True):
     if assert_symmetry:
         assert is_symmetrical(X, tol=tol, nans_ok=nans_ok), "`X` is not symmetric with tol=`{}` or try with `nans_ok=True`".format(tol)
     labels = X.index
-    index=pd.Index(list(map(frozenset, combinations(labels, 2))), name=name)
+    index = pd.Index(list(map(frozenset, combinations(labels, 2))), name=name)
     data = squareform(X, checks=False)
     return pd.Series(data, index=index, name=name)
 
 # pd.Series to pd.DataFrame 2D
-def condensed_to_dense(y:pd.Series, fill_diagonal="infer", index=None):
-    # Check if there are self-interactions
-    number_of_unique_nodes_in_edges = y.index.map(len).unique()
-    assert set(number_of_unique_nodes_in_edges) <= {1,2}, "Number of unique nodes in edge must be either 1 or 2"
-    if isinstance(fill_diagonal, str):
-        if fill_diagonal == "infer":
-            if number_of_unique_nodes_in_edges.min() == 1:
-                fill_diagonal = None
-            else:
-                fill_diagonal = np.nan
- 
+def condensed_to_dense(y:pd.Series, fill_diagonal=None, index=None):
+
     # Need to optimize this
     data = defaultdict(dict)
     for edge, w in y.iteritems():
         number_of_unique_nodes = len(edge)
         if len(edge) == 2:
             node_a, node_b = tuple(edge)
         else:
@@ -98,147 +70,263 @@
                 data[node][node] = fill_diagonal[node]
         else:
             for node in data:
                 data[node][node] = fill_diagonal
             
     df_dense = pd.DataFrame(data)
     if index is None:
-        index = df_dense.index
+        index = sorted(df_dense.index)
     return df_dense.loc[index,index]
 
 # Get symmetric category
 def get_symmetric_category(obj):
-        if type(obj) is type:
-            string_representation = str(obj)
-        else:
-            string_representation = str(type(obj))
-        class_type = string_representation.split("'")[1]
-        fields = class_type.split(".")
-        module = fields[0]
-        category = None
-        if fields[-1] == "Symmetric":
-            category = "Symmetric"
-        if module == "pandas":
-            if fields[-1] == "Series":
-                category = ("pandas", "Series")
-            if fields[-1] == "DataFrame":
-                category = ("pandas", "DataFrame")
-        if module in  {"networkx", "igraph"}:
-            category = module
-        assert category is not None, "`data` must be either a pandas[Series, DataFrame], ensemble_networkx[Symmetric], networkx[Graph, DiGraph, OrdereredGraph, DiOrderedGraph], igraph[Graph]"
-        return category
+    """
+    Future: Add support for Hive objects
+    """
+    if type(obj) is type:
+        string_representation = str(obj)
+    else:
+        string_representation = str(type(obj))
+    class_type = string_representation.split("'")[1]
+    fields = class_type.split(".")
+    module = fields[0]
+    category = None
+    if fields[-1] == "Symmetric":
+        category = "Symmetric"
+    if module == "pandas":
+        if fields[-1] == "Series":
+            category = ("pandas", "Series")
+        if fields[-1] == "DataFrame":
+            category = ("pandas", "DataFrame")
+    if module in  {"networkx", "igraph"}:
+        category = module
+    assert category is not None, "`data` must be either a pandas[Series, DataFrame], ensemble_networkx[Symmetric], networkx[Graph, DiGraph, OrdereredGraph, DiOrderedGraph], igraph[Graph]"
+    return category
     
-def convert_network(data, into, index=None, assert_symmetry=True, tol=1e-10, **attrs):
+# Convert Networks
+def convert_network(
+    # I/O
+    data, 
+    into, 
+    
+    # Subgraphs
+    node_subgraph:list=None, 
+    edge_subgraph:list=None, 
+        
+    # Symmetry
+    remove_self_interactions:bool=True,
+    assert_symmetry=True, 
+    tol=None, 
+
+    # Missing values
+    remove_missing_values:bool=True,
+    fill_missing_values_with=np.nan,
+    fill_diagonal=np.nan, 
+    
+    # Attributes
+    # propogate_input_attributes=False,
+    **attrs,
+    ):
     """
     Convert to and from the following network structures:
         * pd.DataFrame (must be symmetrical)
         * pd.Series (index must be frozenset of {node_a, node_b})
         * Symmetric
         * nx.[Di|Ordered]Graph
         * ig.Graph
-
-    NOTE: This needs to be cleaned up
+    
+    Future: 
+    Add support for existing attributes to propogate to next level. Currently, Symmetric isn't supported so I removed it entirely.
+    Add support for Hive objects
     """
     input_category = get_symmetric_category(data)
     output_category = get_symmetric_category(into)
 
     assert output_category in {("pandas", "Series"), ("pandas", "DataFrame"), "Symmetric", "networkx", "igraph"}, "`data` must be either a pandas[Series, DataFrame], ensemble_networkx[Symmetric], networkx[Graph, DiGraph, OrdereredGraph, DiOrderedGraph], igraph[Graph]"
     assert isinstance(into, type), "`into` must be an instantiated object: a pandas[Series, DataFrame], ensemble_networkx[Symmetric], networkx[Graph, DiGraph, OrdereredGraph, DiOrderedGraph], igraph[Graph]"
     assert into not in {nx.MultiGraph, nx.MultiDiGraph},  "`into` cannot be a `Multi[Di]Graph`"
     
-    # self -> self
-    if isinstance(data, into):
+    
+    assert not (node_subgraph is not None) & (edge_subgraph is not None), "Cannot create subgraph from `node_subgraph` and `edge_subgraph`"
+    
+    if all([
+        input_category == output_category,
+        node_subgraph is None, 
+        edge_subgraph is None, 
+        remove_self_interactions == False,
+        ]):
         return data.copy()
     
-    # HACK and I'm not proud of it...
-    @check_packages(["igraph"])
-    def _to_igraph(data): 
-        return Symmetric(data).to_igraph(**attrs)
-    if output_category == "igraph":
-        return _to_igraph(convert_network(data, into=pd.Series))
-                        
-    # pd.Series --> Symmetric
-    if isinstance(data, pd.Series):
-        data =  Symmetric(data, **attrs)
-        if into == Symmetric:
-            return data
+    _attrs = dict()
     
-    # pd.DataFrame -> Symmetric or NetworkX
-    if isinstance(data, pd.DataFrame) and (into in {Symmetric, nx.Graph, nx.OrderedGraph, nx.DiGraph, nx.OrderedDiGraph}):
-        weights = dense_to_condensed(data, assert_symmetry=assert_symmetry, tol=tol)
-        if into == Symmetric:
-            return Symmetric(weights, **attrs)
+    # Convert to pd.Series
+    if input_category == "igraph":
+        # iGraph -> NetworkX
+        if all([
+            output_category == "network",
+            node_subgraph is None, 
+            edge_subgraph is None, 
+            remove_self_interactions == False,
+            ]):
+            return data.to_networkx(into)
         else:
-            return Symmetric(weights).to_networkx(into=into, **attrs)
-        
-    # pd.DataFrame -> pd.Series
-    if isinstance(data, pd.DataFrame) and (into in {pd.Series}):
-        return dense_to_condensed(data, assert_symmetry=assert_symmetry, tol=tol)
-
-        
-    # Symmetric -> pd.DataFrame, pd.Series, or NetworkX
-    if isinstance(data, Symmetric):
-        # pd.DataFrame
-        if into == pd.DataFrame:
-            df = data.to_dense()
-            if index is None:
-                return df
-            else:
-                assert set(index) <= set(df.index), "Not all `index` values are in `data`"
-                return df.loc[index,index]
-        elif into == pd.Series:
-            return data.weights.copy()
-        # Graph
+            if data.is_directed():
+                warnings.warn("Currently conversions cannot handle directed graphs and will force into undirected configuration")
+            weights = data.es["weight"]
+            nodes = np.asarray(data.vs["name"])
+            edges = list(map(lambda edge_indicies: frozenset(nodes[list(edge_indicies)]), data.get_edgelist()))
+            data = pd.Series(weights, index=edges)
+            input_category == ("pandas", "Series")
+        
+    if input_category == "networkx":
+        # Update attrs
+        # _attrs.update(graph.data)
+        # NetworkX -> iGraph
+        if all([
+            output_category == "igraph",
+            node_subgraph is None, 
+            edge_subgraph is None, 
+            remove_self_interactions == False,
+            ]):
+            return ig.Graph.from_networkx(data)
         else:
-            return data.to_networkx(into=into, **attrs)
-        
-    # NetworkX -> Symmetric
-    if isinstance(data, (nx.Graph, nx.OrderedGraph, nx.DiGraph, nx.OrderedDiGraph)):
-        if into == Symmetric:
-            return Symmetric(data=data, **attrs)
-        if into == pd.DataFrame:
-            return Symmetric(data=data, **attrs).to_dense()
-        if into in {nx.Graph, nx.OrderedGraph, nx.DiGraph, nx.OrderedDiGraph}:
-            return Symmetric(data=data).to_networkx(into=into, **attrs)
-        if into == pd.Series:
-            return convert_network(data=data, into=Symmetric, index=index, assert_symmetry=assert_symmetry, tol=tol).weights
-
+            # Weights
+            edge_weights = dict()
+            for edge_data in data.edges(data=True):
+                edge = frozenset(edge_data[:-1])
+                weight = edge_data[-1]["weight"]
+                edge_weights[edge] = weight
+            data = pd.Series(edge_weights)
+            input_category == ("pandas", "Series")
+            
+    if input_category == ("pandas", "DataFrame"):
+        assert len(data.shape) == 2, "`data.shape` must be square (2 dimensions)"
+        assert np.all(data.index == data.columns), "`data.index` must equal `data.columns`"
+        # if assert_symmetry:
+        #     assert is_symmetrical(data, tol=tol, nans_ok=True), "`data` is not symmetric with tol=`{}` or try with `nans_ok=True`".format(tol)
+        # data = data.stack()
+        # data.index = data.index.map(frozenset)
+        
+        data = dense_to_condensed(data, assert_symmetry=assert_symmetry, tol=tol, nans_ok=True)
+        input_category == ("pandas", "Series")
+
+    if input_category == "Symmetric":
+        data = data.weights
+        input_category == ("pandas", "Series")
+        
+    
+    if input_category == ("pandas", "Series"):
+        if data.name is not None:
+            if "name" in _attrs:
+                if _attrs["name"] is None:
+                    _attrs["name"] = data.name
+            else:
+                _attrs["name"] = data.name
 
+    # Overwrite existing attrs with provided attrs
+    for k, v in attrs.items():
+        if v is not None:
+            _attrs[k] = v
+    
+    # Remove duplicates
+    data = data[~data.index.duplicated()]
+    
+    # Subgraphs
+    if node_subgraph is not None:
+        nodes = frozenset.union(*data.index)
+        node_subgraph = frozenset(node_subgraph)
+        assert node_subgraph <= nodes, "`node_subgraph` must be a subset of the nodes in `data`"
+        edge_subgraph = sorted(set(data.index[data.index.map(lambda edge: edge <= node_subgraph)]))
+        
+    if edge_subgraph is not None:
+        assert set(edge_subgraph) <= set(data.index), "`edge_subgraph` must be a subset of the edge set in `data`"
+        data = data[edge_subgraph]
+        
+    if remove_self_interactions:
+        data = data[data.index.map(lambda edge: len(edge) > 1)]
+        
+    # Missing values
+    if remove_missing_values:
+        data = data.dropna()
+    else:
+        if data.isnull().sum() > 0:
+            data = data.fillna(fill_missing_values_with)
+            
+    # Output
+    if output_category == ("pandas", "Series"):
+        data.name = _attrs.get("name", None)
+        return data
+    
+    if output_category == ("pandas", "DataFrame"):
+        return condensed_to_dense(data, fill_diagonal=fill_diagonal)
+    
+    if output_category == "networkx":
+        graph = into(**_attrs)
+        for edge, w in data.items():
+            if len(edge) == 1:
+                node_a = node_b = list(edge)[0]
+            else:
+                node_a, node_b = list(edge)
+            graph.add_edge(node_a, node_b, weight=w)
+        return graph
+    
+    if output_category == "igraph":
+        graph = into() 
+        # nodes = sorted(flatten(data.index.map(list), unique=True))
+        nodes = sorted(frozenset.union(*data.index))
+        graph.add_vertices(nodes)
+        for edge, w in data.items():
+            if len(edge) == 1:
+                node_a = node_b = list(edge)[0]
+            else:
+                node_a, node_b = list(edge)
+            graph.add_edge(node_a, node_b, weight=w)
+        for k, v in _attrs.items():
+            graph[k] = v
+        return graph
+    
+    if output_category == "Symmetric":
+        return Symmetric(data=data, **_attrs)
+    
 # ===================
 # Network Statistics
 # ===================
 # Connectivity
-def connectivity(data, groups:pd.Series=None, include_self_loops=False, tol=1e-10):
+def connectivity(data, groups:pd.Series=None, remove_self_interactions=True, tol=1e-10):
     """
     Calculate connectivity from pd.DataFrame (must be symmetric), Symmetric, Hive, or NetworkX graph
     
     groups must be dict-like: {node:group}
     """
     # This is a hack to allow Hives from hive_networkx
     if is_query_class(data, "Hive"):
-        data = condensed_to_dense(data.weights)
-    assert isinstance(data, (pd.DataFrame, Symmetric, nx.Graph, nx.DiGraph, nx.OrderedGraph, nx.OrderedDiGraph)), "Must be either a symmetric pd.DataFrame, Symmetric, nx.Graph, or hx.Hive object"
-    if is_graph(data):
-        weights = dict()
-        for edge_data in data.edges(data=True):
-            edge = frozenset(edge_data[:-1])
-            weight = edge_data[-1]["weight"]
-            weights[edge] = weight
-        weights = pd.Series(weights, name="Weights")#.sort_index()
-        data = Symmetric(weights)
-    if isinstance(data, Symmetric):
-        df_dense = condensed_to_dense(data.weights)
-
-    if isinstance(data, pd.DataFrame):
-        assert is_symmetrical(data, tol=tol)
-        df_dense = data
-        
+        data = data.weights
+    # assert isinstance(data, (pd.DataFrame, Symmetric, nx.Graph, nx.DiGraph, nx.OrderedGraph, nx.OrderedDiGraph)), "Must be either a symmetric pd.DataFrame, Symmetric, nx.Graph, or hx.Hive object"
+#     if is_graph(data):
+#         weights = dict()
+#         for edge_data in data.edges(data=True):
+#             edge = frozenset(edge_data[:-1])
+#             weight = edge_data[-1]["weight"]
+#             weights[edge] = weight
+#         weights = pd.Series(weights, name="Weights")#.sort_index()
+#         data = Symmetric(weights)
+#     if isinstance(data, Symmetric):
+#         df_dense = condensed_to_dense(data.weights)
+
+#     if isinstance(data, pd.DataFrame):
+#         assert is_symmetrical(data, tol=tol)
+#         df_dense = data
 
-    df_dense = df_dense.copy()
-    if not include_self_loops:
+    if not isinstance(data, pd.DataFrame):
+        df_dense = convert_network(data=data, into=pd.DataFrame, remove_missing_values=False, remove_self_interactions=False, tol=tol)
+    else:
+        assert is_symmetrical(X=data, tol=tol, nans_ok=True)
+        df_dense = data.copy()
+        
+    if remove_self_interactions:
         np.fill_diagonal(df_dense.values, 0)
 
     #kTotal
     k_total = df_dense.sum(axis=1)
     
     if groups is None:
         return k_total
@@ -247,16 +335,16 @@
         data_connectivity = OrderedDict()
         
         data_connectivity["kTotal"] = k_total
         
         #kWithin
         k_within = list()
         for group in groups.unique():
-            idx_nodes = pd.Index(sorted(set(groups[lambda x: x == group].index) & set(df_dense.index)))
-            k_group = df_dense.loc[idx_nodes,idx_nodes].sum(axis=1)
+            index_nodes = pd.Index(sorted(set(groups[lambda x: x == group].index) & set(df_dense.index)))
+            k_group = df_dense.loc[index_nodes,index_nodes].sum(axis=1)
             k_within.append(k_group)
         data_connectivity["kWithin"] = pd.concat(k_within)
         
         #kOut
         data_connectivity["kOut"] = data_connectivity["kTotal"] - data_connectivity["kWithin"]
 
         #kDiff
@@ -288,15 +376,24 @@
     Heterogeneity = sqrt(nGenes * sum(khelp^2)/sum(khelp)^2 - 1)
     https://github.com/cran/WGCNA/blob/15de0a1fe2b214f7047b887e6f8ccbb1c681e39e/R/Functions.R#L1967
     """
     number_of_nodes = k.size
     return np.sqrt(number_of_nodes * np.sum(k**2)/np.sum(k)**2 - 1)
 
 # Topological overlap
-def topological_overlap_measure(data, into=None, node_type=None, edge_type="topological_overlap_measure", association="network", assert_symmetry=True, tol=1e-10):
+def topological_overlap_measure(
+    data, 
+    into=None, 
+    node_type=None, 
+    edge_type="topological_overlap_measure", 
+    association_type="network", 
+    assert_symmetry=True, 
+    tol=1e-10,
+    fill_diagonal=np.nan,
+    ):
     """
     Compute the topological overlap for a weighted adjacency matrix
     
     `data` and `into` can be the following network structures/objects:
         * pd.DataFrame (must be symmetrical)
         * Symmetric
         * nx.[Di|Ordered]Graph
@@ -361,15 +458,15 @@
     if node_labels is None:
         return A_tom
 
     # Labeled adjacency
     else:
         df_tom = pd.DataFrame(A_tom, index=node_labels, columns=node_labels)
         df_tom.index.name = df_tom.columns.name = node_type
-        return convert_network(df_tom, into=into, assert_symmetry=assert_symmetry, tol=tol, adjacency="network", node_type=node_type, edge_type=edge_type, association=association)
+        return convert_network(df_tom, into=into, fill_diagonal=fill_diagonal, assert_symmetry=assert_symmetry, tol=tol, association_type="network", node_type=node_type, edge_type=edge_type)
 
 
 
 
 # =======================================================
 # Community Detection
 # =======================================================
@@ -387,31 +484,30 @@
         except ModuleNotFoundError:
             Exception("Please install `python-louvain` to use {} algorithm".format(algorithm))
     
         # Keywords
         _algo_kws = {}
         _algo_kws.update(algo_kws)
         
+        graph = convert_network(graph, nx.Graph) 
+        
         def partition_function(graph, weight, random_state, algo_kws):
             return best_partition(graph, weight=weight, random_state=random_state, **algo_kws)
         
     # Leiden
     if algorithm == "leiden":
         try:
-            import igraph as ig
-        except ModuleNotFoundError:
-            Exception("Please install `igraph` to use {} algorithm".format(algorithm))
-        try:
             from leidenalg import find_partition, ModularityVertexPartition
         except ModuleNotFoundError:
             Exception("Please install `leidenalg` to use {} algorithm".format(algorithm))
 
         # Convert NetworkX to iGraph
-        graph = ig.Graph.from_networkx(graph)
-        nodes_list = np.asarray(graph.vs["_nx_name"])
+        # graph = ig.Graph.from_networkx(graph)
+        graph = convert_network(graph, ig.Graph) 
+        nodes_list = np.asarray(graph.vs["name"])
         
         # Keywords
         _algo_kws = {"partition_type":ModularityVertexPartition, "n_iterations":-1}
         _algo_kws.update(algo_kws)
         
         def partition_function(graph, weight, random_state, algo_kws, nodes_list=nodes_list):
             node_to_partition = dict()
@@ -573,15 +669,23 @@
             name=name,
     )
 
     if into == pd.Series:
         return data
     else:
         # Get symmetric object
-        network = Symmetric(data=data, association="network", assert_symmetry=False, remove_missing_values=True, name=name, node_type=node_type, edge_type=edge_type)
+        network = Symmetric(
+            data=data, 
+            association_type="network", 
+            assert_symmetry=False, 
+            remove_missing_values=True, 
+            name=name, 
+            node_type=node_type, 
+            edge_type=edge_type,
+            )
         
         if into == Symmetric:
             return network
         else:
             return convert_network(network, into)
         
 # Biweight midcorrelation
@@ -692,15 +796,15 @@
 
     # Make half of the edges negative to showcase edge coloring (not statistically meaningful at all)
     for a, b in zip(np.random.RandomState(0).randint(low=0, high=149, size=number_of_edges_negative), np.random.RandomState(1).randint(low=0, high=149, size=number_of_edges_negative)):
         if a != b:
             df_sim.values[a,b] = df_sim.values[b,a] = df_sim.values[a,b]*-1
 
     # Create a Symmetric object from the association matrix
-    sym_iris = enx.Symmetric(data=df_sim, node_type="iris sample", edge_type=method, name="iris", association="network")
+    sym_iris = enx.Symmetric(data=df_sim, node_type="iris sample", edge_type=method, name="iris", association_type="network")
     # ====================================
     # Symmetric(Name:iris, dtype: float64)
     # ====================================
     #     * Number of nodes (iris sample): 150
     #     * Number of edges (correlation): 11175
     #     * Association: network
     #     * Memory: 174.609 KB
@@ -717,14 +821,17 @@
     #     (iris_149, iris_146)    0.986481
     #     (iris_147, iris_148)    0.995708
     #     (iris_149, iris_147)    0.994460
     #     (iris_149, iris_148)    0.999916
     =====
     devel
     =====
+    2022-Feb-12
+    * Completely rewrote Symmetric to clean it up. A little slower but much easier to prototype
+    
     2022-Feb-08
     * Added support for iGraph
     * Added support for non-fully-connected graphs
     
     2020-June-23
     * Replace self._dense_to_condensed to dense_to_condensed
     * Dropped math operations
@@ -746,204 +853,86 @@
     def __init__(
         self, 
         data, 
         name=None, 
         node_type=None, 
         edge_type=None, 
         func_metric=None,  
-        association="infer", 
-        acceptable_associations={"similarity", "dissimilarity", "statistical_test", "network", "infer", None}, 
+        association_type=None, 
         
         # Symmetry
         assert_symmetry=True, 
         tol=None, 
+        diagonal=None,
 
         # Missing values
         remove_missing_values=True,
         fill_missing_values_with=np.nan,
         nans_ok=True, 
         
+        # Attributes
         **attrs,
         ):
         
-        self._acceptable_associations = acceptable_associations
-        
-        self.name = name
-        self.node_type = node_type
-        self.edge_type = edge_type
-        self.func_metric = func_metric
-        self.association = association
-        self.diagonal = None
+        # Metadata
         self.metadata = dict()
         
-        # Missing values
-        self.remove_missing_values=remove_missing_values
-        self.fill_missing_values_with=fill_missing_values_with
-        self.nans_ok=nans_ok
+        # Association type
+        assert_acceptable_arguments(association_type, {"similarity", "dissimilarity", "statistical_test", "network", None})
+
         
-        # Get input type
-        input_category = get_symmetric_category(data)
+        # Keywords
         
+        kwargs = {"name":name, "node_type":node_type, "edge_type":edge_type, "func_metric":func_metric, "association_type":association_type}
+
         # From Symmetric object
-        if input_category == "Symmetric":
+        # if input_category == "Symmetric":
+        if isinstance(data, type(self)):
             if not nans_ok:
                 assert not np.any(data.weights.isnull()), "Cannot move forward with missing values"
-            self._from_symmetric(data=data, name=name, node_type=node_type, edge_type=edge_type, func_metric=func_metric, association=association)
-                
-        # From networkx
-        if input_category == "networkx":
-            self._from_networkx(data=data, association=association)
-            
-        # From igraph
-        if input_category == "igraph":
-            self._from_igraph(data=data, association=association)
-        
-        # From pandas
-        if input_category in [("pandas", "Series"), ("pandas", "DataFrame")]:
-            if not nans_ok:
-                assert not np.any(data.isnull()), "Cannot move forward with missing values"
-            # From pd.DataFrame object
-            if isinstance(data, pd.DataFrame):
-                self._from_pandas_dataframe(data=data, association=association, assert_symmetry=assert_symmetry, nans_ok=nans_ok, tol=tol)
-
-            # From pd.Series object
-            if isinstance(data, pd.Series):
-                self._from_pandas_series(data=data, association=association)
-                
-        # Universal
+            self.__dict__.update(data.__dict__)
+            
+            # Set keywords
+            for k, v in kwargs.items():
+                if v is not None:
+                    setattr(self, k, v)
+            
+        # Convert network type
+        else:
+            self.weights = convert_network(
+                data=data, 
+                into=pd.Series, 
+                remove_self_interactions=True, 
+                assert_symmetry=assert_symmetry, 
+                tol=tol, 
+                remove_missing_values=remove_missing_values, 
+                fill_missing_values_with=fill_missing_values_with,
+                name="Weights",
+            )
+            self.edges = pd.Index(self.weights.index, name="Edges")
+            self.nodes = pd.Index(sorted(frozenset.union(*self.weights.index)), name="Nodes")
+            
+            # Set keywords
+            for k, v in kwargs.items():
+                setattr(self, k, v)
+
         # If there's still no `edge_type` and `func_metric` is not empty, then use this the name of `func_metric`
         if (self.edge_type is None) and (self.func_metric is not None):
             self.edge_type = self.func_metric.__name__
-            
+        
+        self.set_diagonal(diagonal)
         self.values = self.weights.values
         self.number_of_nodes = self.nodes.size
         self.number_of_edges = self.edges.size
-#         self.graph = self.to_networkx(into=graph) # Not storing graph because it will double the storage
         self.memory = self.weights.memory_usage()
         self.metadata.update(attrs)
         self.__synthesized__ = datetime.datetime.utcnow()
-                                      
- 
-
-    # =======
-    # Utility
-    # =======
-    
-    def _infer_association(self, X):
-        diagonal = np.diagonal(X)
-        diagonal_elements = set(diagonal)
-        assert len(diagonal_elements) == 1, "Cannot infer relationships from diagonal because multiple values"
-        assert diagonal_elements <= {0,1}, "Diagonal should be either 0.0 for dissimilarity or 1.0 for similarity"
-        return {0.0:"dissimilarity", 1.0:"similarity"}[list(diagonal_elements)[0]]
-
-    def _from_symmetric(self,data, name, node_type, edge_type, func_metric, association):
-        self.__dict__.update(data.__dict__)
-        # If there's no `name`, then get `name` of `data`
-        if self.name is None:
-            self.name = name            
-        # If there's no `node_type`, then get `node_type` of `data`
-        if self.node_type is None:
-            self.node_type = node_type
-        # If there's no `edge_type`, then get `edge_type` of `data`
-        if self.edge_type is None:
-            self.edge_type = edge_type
-        # If there's no `func_metric`, then get `func_metric` of `data`
-        if self.func_metric is None:
-            if func_metric is not None:
-                assert hasattr(func_metric, "__call__"), "`func_metric` must be a function"
-                self.func_metric = func_metric
-
-        # Infer associations
-        if self.association is None:
-            assert_acceptable_arguments(association, self._acceptable_associations)
-            if association != "infer":
-                self.association = association
-            
-    def _from_networkx(self, data, association):
-        # assert isinstance(data, (nx.Graph, nx.OrderedGraph, nx.DiGraph, nx.OrderedDiGraph)), "`If data` is a graph, it must be in {nx.Graph, nx.OrderedGraph, nx.DiGraph, nx.OrderedDiGraph}"
-        assert_acceptable_arguments(association, self._acceptable_associations)
-        if association == "infer":
-            if association is None:
-                association = "network"
-        assert_acceptable_arguments(association, self._acceptable_associations)
-        
-        # Propogate information from graph
-        for attr in ["name", "node_type", "edge_type", "func_metric"]:
-            if getattr(self, attr) is None:
-                if attr in data.graph:
-                    value = data.graph[attr]
-                    if bool(value):
-                        setattr(self, attr, value)
-                        
-        # Weights
-        edge_weights = dict()
-        for edge_data in data.edges(data=True):
-            edge = frozenset(edge_data[:-1])
-            weight = edge_data[-1]["weight"]
-            edge_weights[edge] = weight
-        data = pd.Series(edge_weights)
-        self._from_pandas_series(data=data, association=association)
-        
-    def _from_igraph(self, data, association):
-        if data.is_directed():
-            warnings.warn("Currently `Symmetric` objects cannot handle directed graphs and will force into undirected configuration")
-        # assert isinstance(data, (ig.Graph)), "`If data` is a graph, it must be in {ig.Graph}"
-        assert_acceptable_arguments(association, self._acceptable_associations)
-        if association == "infer":
-            if association is None:
-                association = "network"
-        assert_acceptable_arguments(association, self._acceptable_associations)
-        
-        
-        # Propogate information from graph
-        for attr in ["name", "node_type", "edge_type", "func_metric"]:
-            if getattr(self, attr) is None:
-                try: 
-                    setattr(self, attr, getattr(data, attr))
-                except (KeyError, AttributeError):
-                    pass
-         # Weights
-        weights = data.es["weight"]
-        nodes = np.asarray(g.vs["name"])
-        edges = list(map(lambda edge_indicies: frozenset(nodes[list(edge_indicies)]), data.get_edgelist()))
-        data = pd.Series(weights, index=edges)
-
-        self._from_pandas_series(data=data, association=association)
-        
-    def _from_pandas_dataframe(self, data:pd.DataFrame, association, assert_symmetry, nans_ok, tol):
-        if assert_symmetry:
-            assert is_symmetrical(data, tol=tol), "`X` is not symmetric.  Consider dropping the `tol` to a value such as `1e-10` or using `(X+X.T)/2` to force symmetry"
-        assert_acceptable_arguments(association, self._acceptable_associations)
-        if association == "infer":
-            association = self._infer_association(data)
-        self.association = association
-        self.nodes = pd.Index(data.index)
-        self.diagonal = pd.Series(np.diagonal(data), index=data.index, name="Diagonal")[self.nodes]
-        self.weights = dense_to_condensed(data, name="Weights", assert_symmetry=assert_symmetry, tol=tol)
-        self.edges = pd.Index(self.weights.index, name="Edges")
-                                      
-    def _from_pandas_series(self, data:pd.Series, association):
-        assert all(data.index.map(lambda edge: isinstance(edge, frozenset))), "If `data` is pd.Series then each key in the index must be a frozenset of size 2"
-        assert_acceptable_arguments(association, self._acceptable_associations)
-        if association == "infer":
-            association = None
-        self.association = association
-        # To ensure that the ordering is maintained and this is compatible with methods that use an unlabeled upper triangle, we must reindex and sort
-        self.nodes = pd.Index(sorted(frozenset.union(*data.index)))
-        
-        if self.remove_missing_values:
-            data = data.dropna()
-            self.edges = pd.Index(data.index, name="Edges")
-            self.weights = pd.Series(data, name="Weights")
-        else:
-            self.edges = pd.Index(map(frozenset, combinations(self.nodes, r=2)), name="Edges")
-            self.weights = pd.Series(data, name="Weights").reindex(self.edges)
-            if pd.notnull(self.fill_missing_values_with):
-                self.weights = self.weights.fillna(self.fill_missing_values_with)
         
+        
+    # Setting the diagonal
     def set_diagonal(self, diagonal):
         if diagonal is None:
             self.diagonal = None
         else:
             if is_number(diagonal):
                 diagonal = dict_build([(diagonal, self.nodes)])
             assert is_dict_like(diagonal), "`diagonal` must be dict-like"
@@ -953,41 +942,49 @@
     # =======
     # Built-in
     # =======
     def __repr__(self):
         pad = 4
         header = format_header("Symmetric(Name:{}, dtype: {})".format(self.name, self.weights.dtype),line_character="=")
         n = len(header.split("\n")[0])
+        expected_edges_if_square = 0.5*(self.number_of_nodes**2 - self.number_of_nodes)
         fields = [
             header,
             pad*" " + "* Number of nodes ({}): {}".format(self.node_type, self.number_of_nodes),
             pad*" " + "* Number of edges ({}): {}".format(self.edge_type, self.number_of_edges),
-            pad*" " + "* Association: {}".format(self.association),
+            pad*" " + "* Association: {}".format(self.association_type),
+            pad*" " + "* is_square: {}".format(expected_edges_if_square == self.number_of_edges),
             pad*" " + "* Memory: {}".format(format_memory(self.memory)),
+
             *map(lambda line:pad*" " + line, format_header("| Weights", "-", n=n-pad).split("\n")),
             *map(lambda line: pad*" " + line, repr(self.weights).split("\n")[1:-1]),
             ]
 
         return "\n".join(fields)
     
     def __getitem__(self, key):
         """
         `key` can be a node or non-string iterable of edges
         """
-
+    
         if is_nonstring_iterable(key):
-            assert len(key) >= 2, "`key` must have at least 2 identifiers. e.g. ('A','B')"
+            # assert len(key) >= 2, "`key` must have at least 2 identifiers. e.g. ('A','B')"
             key = frozenset(key)
+            
+            # Is it a diagonal value
             if len(key) == 1:
+                assert self.diagonal is not None, "Please use `set_diagonal` before querying single node edge weights"
                 return self.diagonal[list(key)[0]]
             else:
+                # A list of nodes
                 if len(key) > 2:
                     key = list(map(frozenset, combinations(key, r=2)))
-                return self.weights[key]
+            return self.weights[key]
         else:
+            # Get all edges connected to a node
             if key in self.nodes:
                 s = frozenset([key])
                 mask = self.edges.map(lambda x: bool(s & x))
                 return self.weights[mask]
             else:
                 raise KeyError("{} not in node list".format(key))
         
@@ -997,25 +994,24 @@
         """
         if hasattr(key, "__call__"):
             return self.weights.groupby(key).apply(func)
         else:
             return func(self[key])
         
     def __len__(self):
-        return self.number_of_nodes
+        return self.number_of_edges
     def __iter__(self):
         for v in self.weights:
             yield v
     def items(self):
         return self.weights.items()
     def iteritems(self):
         return self.weights.iteritems()
     def keys(self):
         return self.weights.keys()
-    
     def apply(self, func):
         return func(self.weights)
     def mean(self):
         return self.weights.mean()
     def median(self):
         return self.weights.median()
     def min(self):
@@ -1037,86 +1033,170 @@
     def describe(self, **kwargs):
         return self.weights.describe(**kwargs)
     def map(self, func):
         return self.weights.map(func)
     def entropy(self, base=2):
         assert np.all(self.weights > 0), "All weights must be greater than 0"
         return stats.entropy(self.weights, base=base)
-
+    
+    # ==========
+    # Network Metrics
+    # ==========
+    def edge_connectivity(self, node_subgraph=None, edge_subgraph=None, remove_self_interactions=True):
+        return self.to_pandas_series(node_subgraph=node_subgraph, edge_subgraph=edge_subgraph)
+    
+    def node_connectivity(self, node_subgraph=None, edge_subgraph=None, groups:pd.Series=None, remove_self_interactions=True):
+        """
+        Total node_connectivity is twice that of total edge_connectivity because of symmetry
+        """
+        data = self.to_pandas_dataframe(node_subgraph=node_subgraph, edge_subgraph=edge_subgraph)
+        assert np.all(data.values >= 0), "To use network metrics such as connectivity, density, centralization, and heterogeneity. All weights must ≥ 0."
+        return connectivity(data=data, groups=groups, remove_self_interactions=remove_self_interactions)
+    
+    def density(self, node_subgraph=None, edge_subgraph=None,  remove_self_interactions=True):
+        data = self.to_pandas_dataframe(node_subgraph=node_subgraph, edge_subgraph=edge_subgraph)
+        k = connectivity(data=data, remove_self_interactions=remove_self_interactions)
+        return density(k)
+    
+    def centralization(self, node_subgraph=None, edge_subgraph=None,  remove_self_interactions=True):
+        data = self.to_pandas_dataframe(node_subgraph=node_subgraph, edge_subgraph=edge_subgraph)
+        k = connectivity(data=data, remove_self_interactions=remove_self_interactions)
+        return centralization(k)
+    
+    def heterogeneity(self, node_subgraph=None, edge_subgraph=None,  remove_self_interactions=True):
+        data = self.to_pandas_dataframe(node_subgraph=node_subgraph, edge_subgraph=edge_subgraph)
+        k = connectivity(data=data, remove_self_interactions=remove_self_interactions)
+        return heterogeneity(k)
+    
+    def network_summary_statistics(self, node_subgraph=None, edge_subgraph=None,remove_self_interactions=True):
+        data = self.to_pandas_dataframe(node_subgraph=node_subgraph, edge_subgraph=edge_subgraph)
+        k = connectivity(data=data, remove_self_interactions=remove_self_interactions)
+        return pd.Series(OrderedDict([
+            
+            ("node_connectivity(∑)", k.sum()),
+            ("node_connectivity(µ)", k.mean()),
+            ("node_connectivity(σ)", k.std()),
+            ("density", density(k)),
+            ("centralization", centralization(k)),
+            ("heterogeneity", heterogeneity(k)),
+        ]), name=self.name)
+    
+    def topological_overlap_measure(self, into=pd.Series, node_subgraph=None, edge_subgraph=None, fill_diagonal=np.nan):
+        return topological_overlap_measure(
+            data=self.to_pandas_dataframe(node_subgraph=node_subgraph, edge_subgraph=edge_subgraph, fill_diagonal=np.nan), 
+            fill_diagonal=fill_diagonal,
+            node_type=self.node_type,
+        )
     # ==========
     # Conversion
     # ==========
-    def to_dense(self, index=None, fill_diagonal=None):
-        if fill_diagonal is None:
-            fill_diagonal=self.diagonal
-        if index is None:
-            index = self.nodes
-        return condensed_to_dense(y=self.weights, fill_diagonal=fill_diagonal, index=index)
+    # def to_dense(self, node_subgraph=None, fill_diagonal=None):
+    #     if fill_diagonal is None:
+    #         fill_diagonal = self.diagonal
+    #     if node_subgraph is None:
+    #         node_subgraph = self.nodes
+    #     return condensed_to_dense(y=self.weights, fill_diagonal=fill_diagonal, index=node_subgraph)
     
-    def to_pandas_dataframe(self, index=None, fill_diagonal=None, vertical=False):
-        df = self.to_dense(index=index, fill_diagonal=fill_diagonal)
+    def to_pandas_dataframe(self, node_subgraph=None, edge_subgraph=None, fill_diagonal=None, vertical=False, **convert_network_kws):
+        # df = self.to_dense(node_subgraph=node_subgraph, fill_diagonal=fill_diagonal)
+        if fill_diagonal is None:
+            fill_diagonal = self.diagonal
+        if (node_subgraph is None) & (edge_subgraph is None):
+            node_subgraph = self.nodes
+        
+        df = convert_network(
+            data=self.weights, 
+            into=pd.DataFrame,
+            node_subgraph=node_subgraph,
+            edge_subgraph=edge_subgraph,
+            fill_diagonal=fill_diagonal,
+            **convert_network_kws,
+        )
+            
         if not vertical:
             return df
         else:
             df = df.stack().to_frame().reset_index()
             df.columns = ["Node_A", "Node_B", "Weight"]
             df.index.name = "Edge_Index"
         return df
 
-    def to_condensed(self):
-        return self.weights
+#     def to_condensed(self):
+#         return self.weights
                                      
-    def to_pandas_series(self):
-        return self.to_condensed()
-
+    def to_pandas_series(self, node_subgraph=None, edge_subgraph=None, **convert_network_kws):
+        return convert_network(
+            data=self.weights, 
+            into=pd.Series,
+            node_subgraph=node_subgraph,
+            edge_subgraph=edge_subgraph,
+            **convert_network_kws,
+        )
 #     @check_packages(["ete3", "skbio"])
 #     def to_tree(self, method="average", into=None, node_prefix="y"):
 #         assert self.association == "dissimilarity", "`association` must be 'dissimilarity' to construct tree"
 #         if method in {"centroid", "median", "ward"}:
 #             warnings.warn("Methods ‘centroid’, ‘median’, and ‘ward’ are correctly defined only if Euclidean pairwise metric is used.\nSciPy Documentation - https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage") 
 #         if into is None:
 #             into = ete3.Tree
 #         if not hasattr(self,"Z"):
 #             self.Z = linkage(self.weights.values, metric="precomputed", method=method)
 #         if not hasattr(self,"newick"):
 #             self.newick = linkage_to_newick(self.Z, self.nodes)
 #         tree = into(newick=self.newick, name=self.name)
 #         return name_tree_nodes(tree, node_prefix)
 
-    def to_networkx(self, into=None, **attrs):
+    def to_networkx(self, into=None, node_subgraph=None, edge_subgraph=None, **attrs):
         if into is None:
             into = nx.Graph
-        metadata = { "node_type":self.node_type, "edge_type":self.edge_type, "func_metric":self.func_metric}
+        metadata = {"name":self.name, "node_type":self.node_type, "edge_type":self.edge_type, "func_metric":self.func_metric, "association_type":self.association_type}
         metadata.update(attrs)
-        graph = into(name=self.name, **metadata)
+#         graph = into(name=self.name, **metadata)
 
-        for (node_A, node_B), weight in self.weights.iteritems():
-            graph.add_edge(node_A, node_B, weight=weight)
+#         for (node_A, node_B), weight in self.weights.iteritems():
+#             graph.add_edge(node_A, node_B, weight=weight)
+        graph = convert_network(
+            data=self.weights, 
+            into=into,
+            node_subgraph=node_subgraph,
+            edge_subgraph=edge_subgraph,
+        )
+        graph.graph.update(metadata)
         return graph
     
-    @check_packages(["igraph"])
-    def to_igraph(self, directed=False, **attrs):
-        from igraph import Graph
-        graph = Graph(directed=directed)
-        graph.add_vertices(self.nodes)  # this adds adjacency.shape[0] vertices
-        graph.add_edges(self.edges.map(tuple))
-        graph.es['weight'] = self.weights.values
+    def to_igraph(self, directed=False, node_subgraph=None, edge_subgraph=None, **attrs):
+        metadata = {"name":self.name, "node_type":self.node_type, "edge_type":self.edge_type, "func_metric":self.func_metric, "association_type":self.association_type}
+        metadata.update(attrs)
+        
+        # graph = ig.Graph(directed=directed)
+        # graph.add_vertices(self.nodes)  # this adds adjacency.shape[0] vertices
+        # graph.add_edges(self.edges.map(tuple))
+        # graph.es['weight'] = self.weights.values
+        
+        graph = convert_network(
+            data=self.weights, 
+            into=ig.Graph,
+            node_subgraph=node_subgraph,
+            edge_subgraph=edge_subgraph,
+        )
+        if directed:
+            graph.to_directed()
         
-        for k, v in { "node_type":self.node_type, "edge_type":self.edge_type, "func_metric":self.func_metric}.items():
+        for k, v in metadata.items():
             graph[k] = v
+            
         return graph
     
     def to_file(self, path, **kwargs):
         write_object(obj=self, path=path, **kwargs)
 
     def copy(self):
         return copy.deepcopy(self)
 
 
-
 # =============================
 # Feature Engineering
 # =============================
 class CategoricalEngineeredFeature(object):
     """
     Combine features using multiple categories.
     
@@ -1571,26 +1651,26 @@
             if metric == "phi":
                 metric = pairwise_phi
             if metric == "biweight_midcorrelation":
                 metric = pairwise_biweight_midcorrelation
             if metric in {"spearman", "pearson", "kendall"}:
                 association = metric
                 metric = lambda X: self._pandas_association(X=X, metric=association)
+                # def metric(X, metric):
+                #     return self._pandas_association(X=X, metric=association)
 
                 
         assert hasattr(metric, "__call__"), "`metric` must be either one of the following: [{}], \
         a custom metric that returns an association (set `function_is_pairwise=False`), or a custom \
         metric that returns a 2D square/symmetric pd.DataFrame (set `function_is_pairwise=True`)".format(acceptable_metrics)
         # Transformations
-        acceptable_transformations = {"signed", "abs"}
+        acceptable_transformations = {"abs"}
         if transformation:
             if isinstance(transformation, str):
                 assert_acceptable_arguments(transformation, acceptable_transformations)
-                if transformation == "signed":
-                    transformation = signed
                 if transformation == "abs":
                     transformation = np.abs
             assert hasattr(transformation, "__call__"), "`transformation` must be either one of the following: [{}] or a function(pd.DataFrame) -> pd.DataFrame".format(acceptable_transformations)
             
        # Check statistics functions
         if self.assert_nan_safe_functions:
             if self.nans_ok:
@@ -1781,17 +1861,18 @@
         assert into in {Symmetric, pd.Series}
         sym_network = Symmetric(
             data=self.stats_[weight], 
             name=self.name, 
             node_type=self.node_type, 
             edge_type=self.edge_type, 
             func_metric=self.metric_, 
-            association="network", 
+            association_type="network", 
             assert_symmetry=self.assert_symmetry, 
-            nans_ok=self.nans_ok, tol=self.tol,
+            nans_ok=self.nans_ok, 
+            tol=self.tol,
         )
         if into == Symmetric:
             return sym_network
         if into == pd.Series:
             return sym_network.weights
         
     def to_dense(self, weight="mean", fill_diagonal=1):
@@ -1964,14 +2045,15 @@
         reference,
         metric="rho",
         n_iter=1000,
         sampling_size=0.6180339887,
         transformation=None,
         random_state=0,
         with_replacement=False,
+        include_reference_for_samplespecific=True,
         function_is_pairwise=True,
         stats_summary=[np.mean, np.var, stats.kurtosis, stats.skew], # Need to adjust for NaN robust
         stats_tests=[stats.normaltest],
         stats_summary_initial=None, 
         stats_tests_initial=None,
         copy_X=True,
         copy_y=True,
@@ -1989,16 +2071,50 @@
             stats_tests = [stats_tests]
 
         # Memory
         self.memory_ = 0
         
         assert reference in y.unique(), "`reference({}, type:{}) not in `y`".format(reference, type(reference))
         assert set(X.index) == set(y.index), "`X.index` must have same keys as `y.index`"
-        y = y[X.index]
- 
+        y = y[X.index].astype(str)
+
+        # Data
+        self.classes_ = y.value_counts()
+
+        if copy_X:
+            self.X_ = X.copy()
+            self.X_memory_ = X.memory_usage().sum()
+            self.memory_ += self.X_memory_ 
+
+        if copy_y:
+            self.y_ = y.copy()
+
+        # Checks for index
+        if isinstance(X.index, pd.MultiIndex): # https://github.com/jolespin/ensemble_networkx/issues/2
+            warnings.warn("SampleSpecificPerturbationNetwork cannot work with MultiIndex or tupled index.  Converting MultiIndex to flat index strings. (i.e., X.index = y.index = X.index.to_flat_index().map(str))")
+            X.index = y.index = X.index.to_flat_index().map(str)
+        X.index.name = y.index.name = None # https://github.com/jolespin/ensemble_networkx/issues/1
+
+        if isinstance(X.columns, pd.MultiIndex): # https://github.com/jolespin/ensemble_networkx/issues/2
+            warnings.warn("SampleSpecificPerturbationNetwork cannot work with MultiIndex or tupled index.  Converting MultiIndex to flat index strings (i.e., X.columns = X.columns.to_flat_index().map(str))")
+            X.columns = X.columns.to_flat_index().map(str)
+        X.columns.name = None # https://github.com/jolespin/ensemble_networkx/issues/1
+
+        if include_reference_for_samplespecific:
+            y_clone = y[y == reference]
+            y_clone[y_clone == reference] = f"Reference({reference}[clone])"
+            y_clone.index = y_clone.index.map(lambda x: f"{x}[clone]")
+            y = pd.concat([y, y_clone])
+
+            X_clone = X.loc[y[y == reference].index]
+            X_clone.index = X_clone.index.map(lambda x: f"{x}[clone]")
+            X = pd.concat([X, X_clone], axis=0)
+
+            reference = f"Reference({reference}[clone])"
+
         # Ensemble Reference 
         index_reference = sorted(y[lambda i: i == reference].index)
         ensemble_reference = EnsembleAssociationNetwork(
                 name=reference, 
                 node_type=self.node_type, 
                 edge_type=self.edge_type, 
                 observation_type=self.observation_type, 
@@ -2140,22 +2256,15 @@
                     "Edges":edges, 
                     "Statistics":stat_fields,
                 },
         )
         self.stats_memory_ = self.stats_.nbytes
         self.memory_ += self.stats_memory_ 
 
-        # Data
-        if copy_X:
-            self.X_ = X.copy()
-            self.X_memory_ = X.memory_usage().sum()
-            self.memory_ += self.X_memory_ 
 
-        if copy_y:
-            self.y_ = y.copy()
 
         # Reference ensemble
         self.ensemble_reference_ = ensemble_reference
         self.ensemble_reference_memory_ = ensemble_reference.memory_
         self.memory_ += self.ensemble_reference_memory_
 
         # Sample-specific ensembles
@@ -2166,17 +2275,17 @@
         # Ensemble
         if hasattr(self, "ensemble_"):
             self.ensemble_ = xr.DataArray(
                     data=self.ensemble_, 
                     name=self.name,
                     dims=["Samples", "Iterations", "Edges"], 
                     coords={
-                        "Samples":index_samplespecific, 
-                        "Iterations":range(n_iter),
-                        "Edges":edges, 
+                        "Samples":list(index_samplespecific), 
+                        "Iterations":list(range(n_iter)),
+                        "Edges":list(edges), 
                     },
             )
             self.ensemble_memory_ = self.ensemble_.nbytes
             self.memory_ += self.ensemble_memory_
         
         # Network
         self.n_ = n
@@ -2218,15 +2327,15 @@
         assert into in {Symmetric, pd.Series}
         sym_network = Symmetric(
             data=self.stats_.sel(Samples=sample, Statistics=weight).to_pandas(), 
             name=self.name, 
             node_type=self.node_type, 
             edge_type=self.edge_type, 
             func_metric=self.metric_, 
-            association="network", 
+            association_type="network", 
             assert_symmetry=self.assert_symmetry, 
             nans_ok=self.nans_ok, 
             tol=self.tol,
         )
         if into == Symmetric:
             return sym_network
         if into == pd.Series:
@@ -2588,15 +2697,15 @@
         assert into in {Symmetric, pd.Series}
         sym_network = Symmetric(
             data=self.ensemble_[weight], 
             name=self.name, 
             node_type=self.node_type, 
             edge_type=self.edge_type, 
             func_metric=self.metric_, 
-            association="network", 
+            association_type="network", 
             assert_symmetry=self.assert_symmetry, 
             nans_ok=self.nans_ok, 
             tol=self.tol,
         )
         if into == Symmetric:
             return sym_network
         if into == pd.Series:
```

### Comparing `ensemble_networkx-2022.2.9/setup.py` & `ensemble_networkx-2023.7.18/setup.py`

 * *Files identical despite different names*

