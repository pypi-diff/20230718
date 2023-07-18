# Comparing `tmp/napari-graph-0.1.1.tar.gz` & `tmp/napari-graph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-graph-0.1.1.tar", last modified: Thu Jun 29 15:46:58 2023, max compression
+gzip compressed data, was "napari-graph-0.2.0.tar", last modified: Tue Jul 18 17:54:25 2023, max compression
```

## Comparing `napari-graph-0.1.1.tar` & `napari-graph-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.774985 napari-graph-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.762983 napari-graph-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.770984 napari-graph-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-29 15:46:42.000000 napari-graph-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 15:46:42.000000 napari-graph-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-29 15:46:58.774985 napari-graph-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 15:46:42.000000 napari-graph-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.770984 napari-graph-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-29 15:46:42.000000 napari-graph-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.770984 napari-graph-0.1.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 15:46:42.000000 napari-graph-0.1.1/docs/api/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-29 15:46:42.000000 napari-graph-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 15:46:42.000000 napari-graph-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-29 15:46:42.000000 napari-graph-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-29 15:46:42.000000 napari-graph-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-29 15:46:58.774985 napari-graph-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.766984 napari-graph-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.770984 napari-graph-0.1.1/src/napari_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.774985 napari-graph-0.1.1/src/napari_graph/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/_tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/_tests/test_interops.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    29561 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/directed_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/interops.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-29 15:46:42.000000 napari-graph-0.1.1/src/napari_graph/undirected_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:46:58.774985 napari-graph-0.1.1/src/napari_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 15:46:58.000000 napari-graph-0.1.1/src/napari_graph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-29 15:46:42.000000 napari-graph-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:54:25.420630 napari-graph-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-18 17:54:07.000000 napari-graph-0.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:54:25.412630 napari-graph-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:54:25.416630 napari-graph-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-18 17:54:07.000000 napari-graph-0.2.0/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-18 17:54:07.000000 napari-graph-0.2.0/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-18 17:54:07.000000 napari-graph-0.2.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-18 17:54:07.000000 napari-graph-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-18 17:54:07.000000 napari-graph-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-18 17:54:07.000000 napari-graph-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-18 17:54:25.420630 napari-graph-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 17:54:07.000000 napari-graph-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:54:25.416630 napari-graph-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-18 17:54:07.000000 napari-graph-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:54:25.416630 napari-graph-0.2.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 17:54:07.000000 napari-graph-0.2.0/docs/api/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-07-18 17:54:07.000000 napari-graph-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 17:54:07.000000 napari-graph-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-18 17:54:07.000000 napari-graph-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 17:54:07.000000 napari-graph-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-18 17:54:25.420630 napari-graph-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:54:25.412630 napari-graph-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:54:25.416630 napari-graph-0.2.0/src/napari_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-18 17:54:07.000000 napari-graph-0.2.0/src/napari_graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:54:25.420630 napari-graph-0.2.0/src/napari_graph/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-18 17:54:07.000000 napari-graph-0.2.0/src/napari_graph/_tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-18 17:54:07.000000 napari-graph-0.2.0/src/napari_graph/_tests/test_interops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-18 17:54:25.000000 napari-graph-0.2.0/src/napari_graph/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29553 2023-07-18 17:54:07.000000 napari-graph-0.2.0/src/napari_graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14274 2023-07-18 17:54:07.000000 napari-graph-0.2.0/src/napari_graph/directed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-18 17:54:07.000000 napari-graph-0.2.0/src/napari_graph/interops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-18 17:54:07.000000 napari-graph-0.2.0/src/napari_graph/numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-07-18 17:54:07.000000 napari-graph-0.2.0/src/napari_graph/undirected_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:54:25.420630 napari-graph-0.2.0/src/napari_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-18 17:54:25.000000 napari-graph-0.2.0/src/napari_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-18 17:54:25.000000 napari-graph-0.2.0/src/napari_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:54:25.000000 napari-graph-0.2.0/src/napari_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 17:54:25.000000 napari-graph-0.2.0/src/napari_graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 17:54:25.000000 napari-graph-0.2.0/src/napari_graph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-18 17:54:07.000000 napari-graph-0.2.0/tox.ini
```

### Comparing `napari-graph-0.1.1/.github/workflows/build-docs.yml` & `napari-graph-0.2.0/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/.github/workflows/deploy-docs.yml` & `napari-graph-0.2.0/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/.github/workflows/test_and_deploy.yml` & `napari-graph-0.2.0/.github/workflows/test_and_deploy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,25 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools tox tox-gh-actions
           python -m pip install .[testing]
 
       # this runs the platform-specific tests declared in tox.ini
-      - name: Test with tox
+      - name: Test without numba
+        run: |
+          python -m tox
+        env:
+          PLATFORM: ${{ matrix.platform }}
+
+      - name: Install numba
+        run: |
+          pip install .[fast]
+
+      - name: Test with numba
         run: |
           python -m tox
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
         uses: codecov/codecov-action@v3
```

### Comparing `napari-graph-0.1.1/.gitignore` & `napari-graph-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/.pre-commit-config.yaml` & `napari-graph-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/LICENSE` & `napari-graph-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/PKG-INFO` & `napari-graph-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-graph
-Version: 0.1.1
+Version: 0.2.0
 Summary: Fast editable graphs in Python and numba
 Home-page: https://github.com/napari/napari-graph
 Author: Jordão Bragantini, Jonas Windhager & Juan Nunez-Iglesias
 Author-email: jordao.bragantini@czbiohub.org
 License: BSD-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: fast
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 # napari-graph
 
 Efficient graph data structures and algorithms for fast slicing, visualization, and editing.
```

### Comparing `napari-graph-0.1.1/docs/Makefile` & `napari-graph-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/docs/conf.py` & `napari-graph-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/docs/make.bat` & `napari-graph-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/pyproject.toml` & `napari-graph-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/setup.cfg` & `napari-graph-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,24 @@
 package_dir = 
 	=src
 include_package_data = True
 packages = find:
 setup_requires = setuptools_scm
 install_requires = 
 	networkx
-	numba
 	numpy
 	pandas
 python_requires = >=3.8
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
+fast = 
+	numba
 testing = 
 	coverage
 	pytest
 	pytest-cov
 docs = 
 	sphinx-material
 	sphinx
```

### Comparing `napari-graph-0.1.1/src/napari_graph/_tests/test_graph.py` & `napari-graph-0.2.0/src/napari_graph/_tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/src/napari_graph/_tests/test_interops.py` & `napari-graph-0.2.0/src/napari_graph/_tests/test_interops.py`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/src/napari_graph/base_graph.py` & `napari-graph-0.2.0/src/napari_graph/base_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from abc import abstractmethod
 from typing import Callable, List, Optional, Tuple, Union
 
 import networkx as nx
 import numpy as np
 import pandas as pd
-from numba import njit, typed
-from numba.core import types
 from numpy.typing import ArrayLike
 
+from napari_graph.numba import njit, typed, types
+
 """
 _NODE_EMPTY_PTR is used to fill the values of uninitialized/empty/removed nodes
 """
 _NODE_EMPTY_PTR = -1
 
 """
 _EDGE_EMPTY_PTR is used to fill the values of uninitialized/empty/removed edges
```

### Comparing `napari-graph-0.1.1/src/napari_graph/directed_graph.py` & `napari-graph-0.2.0/src/napari_graph/directed_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
-from numba import njit, typed
 from numpy.typing import ArrayLike
 
 from napari_graph.base_graph import (
     _EDGE_EMPTY_PTR,
     _NODE_EMPTY_PTR,
     BaseGraph,
     _iterate_edges,
     _remove_edge,
 )
+from napari_graph.numba import njit, typed
 from napari_graph.undirected_graph import _UN_EDGE_SIZE
 
 """
 Directed edge constants for accessing the directed graph buffer data.
 Each edge occupies _DI_EDGE_SIZE spaces on the graph buffer.
 _LL_DI_EDGE_POS indicates the displacement between the edge initial index and
 the **target** edge directed linked list position.
```

### Comparing `napari-graph-0.1.1/src/napari_graph/interops.py` & `napari-graph-0.2.0/src/napari_graph/interops.py`

 * *Files identical despite different names*

### Comparing `napari-graph-0.1.1/src/napari_graph/undirected_graph.py` & `napari-graph-0.2.0/src/napari_graph/undirected_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
-from numba import njit, typed
 from numpy.typing import ArrayLike
 
 from napari_graph.base_graph import (
     _EDGE_EMPTY_PTR,
     BaseGraph,
     _iterate_edges,
     _remove_edge,
 )
+from napari_graph.numba import njit, typed
 
 """
 Undirected edge constants for accessing the directed graph buffer data.
 Each edge occupies _UN_EDGE_SIZE spaces on the graph buffer.
 _LL_UN_EDGE_POS indicates the displacement between the edge initial index and
 the edge undirected linked list position.
```

### Comparing `napari-graph-0.1.1/src/napari_graph.egg-info/PKG-INFO` & `napari-graph-0.2.0/src/napari_graph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-graph
-Version: 0.1.1
+Version: 0.2.0
 Summary: Fast editable graphs in Python and numba
 Home-page: https://github.com/napari/napari-graph
 Author: Jordão Bragantini, Jonas Windhager & Juan Nunez-Iglesias
 Author-email: jordao.bragantini@czbiohub.org
 License: BSD-3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: fast
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 # napari-graph
 
 Efficient graph data structures and algorithms for fast slicing, visualization, and editing.
```

### Comparing `napari-graph-0.1.1/src/napari_graph.egg-info/SOURCES.txt` & `napari-graph-0.2.0/src/napari_graph.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 docs/make.bat
 docs/api/api.md
 src/napari_graph/__init__.py
 src/napari_graph/_version.py
 src/napari_graph/base_graph.py
 src/napari_graph/directed_graph.py
 src/napari_graph/interops.py
+src/napari_graph/numba.py
 src/napari_graph/undirected_graph.py
 src/napari_graph.egg-info/PKG-INFO
 src/napari_graph.egg-info/SOURCES.txt
 src/napari_graph.egg-info/dependency_links.txt
 src/napari_graph.egg-info/requires.txt
 src/napari_graph.egg-info/top_level.txt
 src/napari_graph/_tests/test_graph.py
```

### Comparing `napari-graph-0.1.1/tox.ini` & `napari-graph-0.2.0/tox.ini`

 * *Files identical despite different names*

