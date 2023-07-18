# Comparing `tmp/jax_enums-0.1.0.tar.gz` & `tmp/jax_enums-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_enums-0.1.0.tar", last modified: Wed Jul 12 14:14:05 2023, max compression
+gzip compressed data, was "jax_enums-0.1.1.tar", last modified: Tue Jul 18 15:22:14 2023, max compression
```

## Comparing `jax_enums-0.1.0.tar` & `jax_enums-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:14:05.007436 jax_enums-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:14:05.003435 jax_enums-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:14:05.007436 jax_enums-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-12 14:13:48.000000 jax_enums-0.1.0/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-12 14:13:48.000000 jax_enums-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 14:13:48.000000 jax_enums-0.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-12 14:13:48.000000 jax_enums-0.1.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 14:13:48.000000 jax_enums-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-12 14:13:48.000000 jax_enums-0.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-07-12 14:14:05.007436 jax_enums-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-12 14:13:48.000000 jax_enums-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:14:05.007436 jax_enums-0.1.0/jax_enums/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 14:13:48.000000 jax_enums-0.1.0/jax_enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-12 14:13:48.000000 jax_enums-0.1.0/jax_enums/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-12 14:13:48.000000 jax_enums-0.1.0/jax_enums/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:14:05.007436 jax_enums-0.1.0/jax_enums.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-07-12 14:14:04.000000 jax_enums-0.1.0/jax_enums.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 14:14:04.000000 jax_enums-0.1.0/jax_enums.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:14:04.000000 jax_enums-0.1.0/jax_enums.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 14:14:04.000000 jax_enums-0.1.0/jax_enums.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 14:14:04.000000 jax_enums-0.1.0/jax_enums.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-12 14:13:48.000000 jax_enums-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 14:13:48.000000 jax_enums-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:14:05.007436 jax_enums-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:22:14.289002 jax_enums-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:22:14.285002 jax_enums-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:22:14.289002 jax_enums-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-18 15:21:57.000000 jax_enums-0.1.1/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-18 15:21:57.000000 jax_enums-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 15:21:57.000000 jax_enums-0.1.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-18 15:21:57.000000 jax_enums-0.1.1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 15:21:57.000000 jax_enums-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-18 15:21:57.000000 jax_enums-0.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-07-18 15:22:14.289002 jax_enums-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-18 15:21:57.000000 jax_enums-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:22:14.289002 jax_enums-0.1.1/jax_enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 15:21:57.000000 jax_enums-0.1.1/jax_enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-18 15:21:57.000000 jax_enums-0.1.1/jax_enums/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-18 15:21:57.000000 jax_enums-0.1.1/jax_enums/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:22:14.289002 jax_enums-0.1.1/jax_enums.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-07-18 15:22:14.000000 jax_enums-0.1.1/jax_enums.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-18 15:22:14.000000 jax_enums-0.1.1/jax_enums.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:22:14.000000 jax_enums-0.1.1/jax_enums.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 15:22:14.000000 jax_enums-0.1.1/jax_enums.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:22:14.000000 jax_enums-0.1.1/jax_enums.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 15:21:58.000000 jax_enums-0.1.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-18 15:21:57.000000 jax_enums-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 15:21:57.000000 jax_enums-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:22:14.289002 jax_enums-0.1.1/setup.cfg
```

### Comparing `jax_enums-0.1.0/.github/workflows/CD.yml` & `jax_enums-0.1.1/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `jax_enums-0.1.0/.gitignore` & `jax_enums-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jax_enums-0.1.0/COPYRIGHT` & `jax_enums-0.1.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `jax_enums-0.1.0/LICENSE` & `jax_enums-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_enums-0.1.0/PKG-INFO` & `jax_enums-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax_enums
-Version: 0.1.0
+Version: 0.1.1
 Summary: JAX-compatible Enumerations.
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -249,18 +249,17 @@
 **[Installation](#installation)** | **[Examples](#example)** | **[Cite](#cite)**
 
 A Jax-compatible enumerable.
 
 
 
 ## Installation
-You can install `jax_enums` directly from GitHub:
 
 ```sh
-pip install git+https://github.com/epignatelli/jax_enums
+pip install jax_enums
 ```
 
 ## Example
 ```python
 class Foo(Enumerable):
     BAR = 0
     BAZ = 1
```

### Comparing `jax_enums-0.1.0/README.md` & `jax_enums-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 **[Installation](#installation)** | **[Examples](#example)** | **[Cite](#cite)**
 
 A Jax-compatible enumerable.
 
 
 
 ## Installation
-You can install `jax_enums` directly from GitHub:
 
 ```sh
-pip install git+https://github.com/epignatelli/jax_enums
+pip install jax_enums
 ```
 
 ## Example
 ```python
 class Foo(Enumerable):
     BAR = 0
     BAZ = 1
```

### Comparing `jax_enums-0.1.0/jax_enums/_version.py` & `jax_enums-0.1.1/jax_enums/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `jax_enums-0.1.0/jax_enums/enum.py` & `jax_enums-0.1.1/jax_enums/enum.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from __future__ import annotations
 
+from typing import Type, Any
 from enum import Enum, EnumMeta
+
 import jax
 import jax.numpy as jnp
-from typing import Type
 from dataclasses import dataclass
 
 
 @jax.tree_util.register_pytree_node_class
 @dataclass
 class EnumItem:
     name: str
@@ -38,14 +39,20 @@
 
     def __repr__(self):
         return str(self)
 
     def __hash__(self):
         return hash(tuple(jax.tree_util.tree_leaves(self)))
 
+    def __eq__(self, other):
+        if isinstance(other, EnumItem):
+            with jax.ensure_compile_time_eval():
+                return self.value == other.value
+        return hash(self) == hash(other)
+
     def tree_flatten(self):
         return jnp.asarray(self.value)[None], (self.name, self.obj_class)
 
     @classmethod
     def tree_unflatten(cls, aux, children) -> EnumItem:
         return cls(value=children[0], name=aux[0], obj_class=aux[1])
```

### Comparing `jax_enums-0.1.0/jax_enums.egg-info/PKG-INFO` & `jax_enums-0.1.1/jax_enums.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-enums
-Version: 0.1.0
+Version: 0.1.1
 Summary: JAX-compatible Enumerations.
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -249,18 +249,17 @@
 **[Installation](#installation)** | **[Examples](#example)** | **[Cite](#cite)**
 
 A Jax-compatible enumerable.
 
 
 
 ## Installation
-You can install `jax_enums` directly from GitHub:
 
 ```sh
-pip install git+https://github.com/epignatelli/jax_enums
+pip install jax_enums
 ```
 
 ## Example
 ```python
 class Foo(Enumerable):
     BAR = 0
     BAZ = 1
```

### Comparing `jax_enums-0.1.0/pyproject.toml` & `jax_enums-0.1.1/pyproject.toml`

 * *Files identical despite different names*

