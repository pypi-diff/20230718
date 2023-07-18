# Comparing `tmp/pytreeclass-0.3.8.tar.gz` & `tmp/pytreeclass-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.3.8.tar", last modified: Mon Jun 12 18:31:08 2023, max compression
+gzip compressed data, was "pytreeclass-0.4.0.tar", last modified: Tue Jul 18 19:30:40 2023, max compression
```

## Comparing `pytreeclass-0.3.8.tar` & `pytreeclass-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.022609 pytreeclass-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-12 18:31:08.022609 pytreeclass-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.018608 pytreeclass-0.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.018608 pytreeclass-0.3.8/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.018608 pytreeclass-0.3.8/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/_src/code_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    25307 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/_src/tree_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26345 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    23013 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/_src/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.018608 pytreeclass-0.3.8/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:31:08.022609 pytreeclass-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.022609 pytreeclass-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17367 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:40.725926 pytreeclass-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-07-18 19:30:40.725926 pytreeclass-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:40.721926 pytreeclass-0.4.0/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:40.725926 pytreeclass-0.4.0/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/code_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/tree_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/tree_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/tree_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32764 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18528 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/pytreeclass/_src/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:40.721926 pytreeclass-0.4.0/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-07-18 19:30:40.000000 pytreeclass-0.4.0/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-18 19:30:40.000000 pytreeclass-0.4.0/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:30:40.000000 pytreeclass-0.4.0/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 19:30:40.000000 pytreeclass-0.4.0/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 19:30:40.000000 pytreeclass-0.4.0/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:30:40.725926 pytreeclass-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:30:40.725926 pytreeclass-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11274 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21260 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-18 19:30:22.000000 pytreeclass-0.4.0/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.3.8/LICENSE` & `pytreeclass-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.8/PKG-INFO` & `pytreeclass-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pytreeclass
-Version: 0.3.8
-Summary: JAX compatible dataclass.
-Home-page: https://github.com/ASEM000/pytreeclass
-Author: Mahmoud Asem
-Author-email: asem00@kaist.ac.kr
-License: Apache-2.0
-Keywords: python machine-learning pytorch jax
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- <h1 align="center" style="font-family:Monospace" >Py🌲Class</h1> -->
 <h5 align="center">
 <img width="250px" src="https://user-images.githubusercontent.com/48389287/227880173-bf78c02c-d28b-4cf4-95e6-fa49b82a43a1.svg"> <br>
 
 <br>
 
 [**Installation**](#installation)
@@ -105,27 +82,27 @@
 # ├── .a=100.0
 # ├── .b:tuple
 # │   ├── [0]=10.0
 # │   └── [1]=3.0
 # └── .c=f32[3](μ=36.33, σ=45.02, ∈[4.00,100.00])
 
 print(pytc.tree_summary(tree))
-# ┌─────┬──────┬─────┐
-# │Name │Type  │Count│
-# ├─────┼──────┼─────┤
-# │.a   │float │1    │
-# ├─────┼──────┼─────┤
-# │.b[0]│float │1    │
-# ├─────┼──────┼─────┤
-# │.b[1]│float │1    │
-# ├─────┼──────┼─────┤
-# │.c   │f32[3]│3    │
-# ├─────┼──────┼─────┤
-# │Σ    │Tree  │6    │
-# └─────┴──────┴─────┘
+# ┌─────┬──────┬─────┬──────┐
+# │Name │Type  │Count│Size  │
+# ├─────┼──────┼─────┼──────┤
+# │.a   │float │1    │      │
+# ├─────┼──────┼─────┼──────┤
+# │.b[0]│float │1    │      │
+# ├─────┼──────┼─────┼──────┤
+# │.b[1]│float │1    │      │
+# ├─────┼──────┼─────┼──────┤
+# │.c   │f32[3]│3    │12.00B│
+# ├─────┼──────┼─────┼──────┤
+# │Σ    │Tree  │6    │12.00B│
+# └─────┴──────┴─────┴──────┘
 
 # ** pass it to jax transformations **
 # works with jit, grad, vmap, etc.
 
 @jax.jit
 @jax.grad
 def sum_tree(tree: Tree, x):
```

### Comparing `pytreeclass-0.3.8/pytreeclass/_src/__init__.py` & `pytreeclass-0.4.0/pytreeclass/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.8/pytreeclass/_src/code_build.py` & `pytreeclass-0.4.0/pytreeclass/_src/code_build.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,74 +7,77 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 """Constructor code generation from type annotations."""
 
 from __future__ import annotations
 
 import functools as ft
 import sys
+from collections import defaultdict
 from collections.abc import Callable, MutableMapping, MutableSequence, MutableSet
 from types import FunctionType, MappingProxyType
 from typing import Any, Literal, NamedTuple, Sequence, TypeVar, get_args
 
 T = TypeVar("T")
 PyTree = Any
 EllipsisType = type(Ellipsis)
-ArgKindType = Literal["POS_ONLY", "POS_OR_KW", "KW_ONLY"]
+ArgKindType = Literal["POS_ONLY", "POS_OR_KW", "VAR_POS", "KW_ONLY", "VAR_KW"]
 ArgKind = get_args(ArgKindType)
 NULL = type("NULL", (), {"__repr__": lambda _: "NULL"})()
 MUTABLE_TYPES = (MutableSequence, MutableMapping, MutableSet)
 # https://github.com/google/jax/issues/14295
 
 
 class Field(NamedTuple):
     name: str | None = None
     type: type | None = None
     default: Any = NULL
     init: bool = True
     repr: bool = True
     kind: ArgKindType = "POS_OR_KW"
     metadata: dict[str, Any] | None = None
-    callbacks: Sequence[Any] = ()
+    callbacks: Sequence[Callable[[Any], Any]] = ()
     alias: str | None = None
 
     def __call__(self, value: Any):
-        """Call the field's callbacks on `value`."""
+        """Call the callbacks on `value`."""
         for callback in self.callbacks:
             try:
                 value = callback(value)
             except Exception as e:
                 cname = getattr(callback, "__name__", callback)
                 raise type(e)(f"On applying {cname} for field=`{self.name}`:\n{e}")
         return value
 
 
 def field(
-    default: Any = NULL,
     *,
+    default: Any = NULL,
     init: bool = True,
     repr: bool = True,
     kind: ArgKindType = "POS_OR_KW",
     metadata: dict[str, Any] | None = None,  # type: ignore
     callbacks: Sequence[Any] = (),
     alias: str | None = None,
 ) -> Field:
-    """
+    """Field placeholder for type hinted attributes.
+
     Args:
         default: The default value of the field.
         init: Whether the field is included in the object's __init__ function.
         repr: Whether the field is included in the object's __repr__ function.
-        kind: Argument kind, one of 'POS_ONLY', 'KW_ONLY', or 'POS_OR_KW'.
+        kind: Argument kind, one of 'POS_ONLY', 'VAR_POS', 'KW_ONLY', 'VAR_KW'.
         metadata: A mapping of user-defined data for the field.
-        callbacks: A sequence of functions to called on `setattr` during
+        callbacks: A sequence of functions to called on ``__setattr__`` during
             initialization to modify the field value.
         alias: An a alias for the field name in the constructor.
 
     Example:
         >>> import pytreeclass as pytc
         >>> class IsInstance(pytc.TreeClass):
         ...    klass: type
@@ -84,19 +87,19 @@
         >>> class Range(pytc.TreeClass):
         ...    start: int|float = float("-inf")
         ...    stop: int|float = float("inf")
         ...    def __call__(self, x):
         ...        assert self.start <= x <= self.stop
         ...        return x
         >>> class Employee(pytc.TreeClass):
-        ...    # assert employee `name` is str
+        ...    # assert employee ``name`` is str
         ...    name: str = pytc.field(callbacks=[IsInstance(str)])
-        ...    # use callback compostion to assert employee `age` is int and positive
+        ...    # use callback compostion to assert employee ``age`` is int and positive
         ...    age: int = pytc.field(callbacks=[IsInstance(int), Range(1)])
-        ...    # use `id` in the constructor for `_id` attribute
+        ...    # use ``id`` in the constructor for ``_id`` attribute
         ...    # this is useful for private attributes that are not supposed
         ...    # to be accessed directly and hide it from the repr
         ...    _id: int = pytc.field(alias="id", repr=False)
         >>> employee = Employee(name="Asem", age=10, id=1)
         >>> print(employee)  # _id is not shown
         Employee(name=Asem, age=10)
         >>> assert employee._id == 1  # this is the private attribute
@@ -122,15 +125,15 @@
         callbacks=callbacks,
         alias=alias,
     )
 
 
 @ft.lru_cache(maxsize=128)
 def _build_field_map(klass: type) -> MappingProxyType[str, Field]:
-    field_map = dict()  # type: dict[str, Field]
+    field_map: dict[str, Field] = dict()
 
     if klass is object:
         return MappingProxyType(field_map)
 
     for base in reversed(klass.__mro__[1:]):
         field_map.update(_build_field_map(base))
 
@@ -159,57 +162,69 @@
                 raise TypeError(f"Mutable {value=} is not allowed")
             # case: `x: int = 1` or `x: Any`
             field_map[name] = Field(name=name, type=hint, default=value)
     return MappingProxyType(field_map)
 
 
 def fields(x: Any) -> Sequence[Field]:
-    """Returns a tuple of `Field` objects for the given instance or class.
+    """Returns a tuple of ``Field`` objects for the given instance or class.
 
-    `Field` objects are generated from the class type hints and contains
-    the information about the field `name`, `type`, `default` value, and other
-    information (`init`, `repr`, `kind`, `metadata`,
-    `callbacks`, `alias`) if the user uses the `pytreeclass.field`to annotate.
+    ``Field`` objects are generated from the class type hints and contains
+    the information about the field information.if the user uses
+    the ``pytreeclass.field`` to annotate.
 
     Note:
         - If the class is not annotated, an empty tuple is returned.
-        - The `Field` generation is cached for class and its bases.
+        - The ``Field`` generation is cached for class and its bases.
     """
     return tuple(_build_field_map(x if isinstance(x, type) else type(x)).values())
 
 
 def _build_init_method(klass: type) -> FunctionType:
     # generate a code object for the __init__ method and compile it
     # for the given class and return the function object
-    body = []
-    hints = dict()
+    body: list[str] = []
+    hints: dict[str, str | type | None] = dict()
     head = ["self"]
-    heads = dict(zip(ArgKind, ([], [], [])))
+    heads: dict[str, list[str]] = defaultdict(list)
     has_post = "__post_init__" in vars(klass)
 
+    seen = set()
+
     for field in (field_map := _build_field_map(klass)).values():
         dref = "" if field.default is NULL else f"=field_map['{field.name}'].default"
 
         if field.init:
+            if field.kind in ("VAR_POS", "VAR_KW"):
+                # disallow multiple `VAR_POS` and `VAR_KW`
+                if field.kind in seen:
+                    raise TypeError(f"Duplicate {field.kind=} for {field.name=}")
+                seen.add(field.kind)
+
             alias = field.alias or field.name
             hints[field.name] = field.type
             body += [f"self.{field.name}={alias}"]
             heads[field.kind] += [f"{alias}{dref}"]
         else:
             body += [f"self.{field.name}{dref}"]
 
     hints["return"] = None
     # add the post init call if the class has it, otherwise add a pass
     # in case all fields are not initialized in the __init__ method
     body += ["self.__post_init__()"] if has_post else ["pass"]
 
-    # organize the arguments order (POS_ONLY, POS_OR_KW, KW_ONLY)
+    # organize the arguments order:
+    # (POS_ONLY, POS_OR_KW, VAR_POS, KW_ONLY, VAR_KW)
     head += (heads["POS_ONLY"] + ["/"]) if heads["POS_ONLY"] else []
     head += heads["POS_OR_KW"]
-    head += (["*"] + heads["KW_ONLY"]) if heads["KW_ONLY"] else []
+    head += ["*" + "".join(heads["VAR_POS"])] if heads["VAR_POS"] else []
+    # case for ...(*a, b) and ...(a, *, b)
+    head += ["*"] if (heads["KW_ONLY"] and not heads["VAR_POS"]) else []
+    head += heads["KW_ONLY"]
+    head += ["**" + "".join(heads["VAR_KW"])] if heads["VAR_KW"] else []
 
     # generate the code for the __init__ method
     code = "def closure(field_map):\n"
     code += f"\tdef __init__({','.join(head)}):"
     code += f"\n\t\t{';'.join(body)}"
     code += f"\n\t__init__.__qualname__ = '{klass.__qualname__}.__init__'"
     code += "\n\treturn __init__"
```

### Comparing `pytreeclass-0.3.8/pytreeclass/_src/tree_base.py` & `pytreeclass-0.4.0/pytreeclass/_src/tree_index.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,103 +7,412 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Define a class that convert a class to a JAX compatible tree structure"""
+
+"""Define lens-like indexing/masking for pytrees."""
 
 from __future__ import annotations
 
 import abc
-from collections.abc import Callable
-from contextlib import contextmanager
-from typing import Any, Generic, Hashable, NamedTuple, TypeVar
+import functools as ft
+import re
+from typing import Any, Callable, Hashable, NamedTuple, Tuple, TypeVar, Union
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
-from typing_extensions import dataclass_transform
-
-from pytreeclass._src.code_build import (
-    Field,
-    _build_field_map,
-    _build_init_method,
-    field,
-)
-from pytreeclass._src.tree_pprint import tree_repr, tree_str
-from pytreeclass._src.tree_util import (
-    IsLeafType,
-    NamedSequenceKey,
-    WhereAtomType,
-    WhereType,
-    _leafwise_transform,
-    _resolve_where,
-    is_tree_equal,
-    tree_copy,
-    tree_hash,
-)
 
-T = TypeVar("T", bound=Hashable)
+T = TypeVar("T")
+S = TypeVar("S")
 PyTree = Any
-EllipsisType = type(Ellipsis)
+# TODO: swich to EllipsisType for python 3.10
+EllipsisType = TypeVar("EllipsisType")
+KeyEntry = TypeVar("KeyEntry", bound=Hashable)
+TypeEntry = TypeVar("TypeEntry", bound=type)
+TraceEntry = Tuple[KeyEntry, TypeEntry]
+KeyPath = Tuple[KeyEntry, ...]
+TypePath = Tuple[TypeEntry, ...]
+TraceType = Tuple[KeyPath, TypePath]
+IsLeafType = Union[None, Callable[[Any], bool]]
 _no_initializer = object()
 
-# allow methods in mutable context to be called without raising `AttributeError`
-# the instances are registered  during initialization and using `at`  property
-# with `__call__ this is done by registering the instance id in a set before
-# entering the mutable context and removing it after exiting the context
-_mutable_instance_registry: set[int] = set()
-
-
-@contextmanager
-def _mutable_context(tree, *, kopy: bool = False):
-    tree = tree_copy(tree) if kopy else tree
-    _mutable_instance_registry.add(id(tree))
-    yield tree
-    _mutable_instance_registry.discard(id(tree))
-
-
-def _register_treeclass(klass: type[T]) -> type[T]:
-    # handle all registration logic for `treeclass`
-
-    def tree_unflatten(keys: tuple[str, ...], leaves: tuple[Any, ...]) -> T:
-        # unflatten rule to use with `jax.tree_unflatten`
-        tree = getattr(object, "__new__")(klass)
-        vars(tree).update(zip(keys, leaves))
-        return tree
-
-    def tree_flatten(tree: T) -> tuple[tuple[Any, ...], tuple[str, ...]]:
-        # flatten rule to use with `jax.tree_flatten`
-        dynamic = vars(tree)
-        return tuple(dynamic.values()), tuple(dynamic.keys())
-
-    def tree_flatten_with_keys(tree: T):
-        # flatten rule to use with `jax.tree_util.tree_flatten_with_path`
-        dynamic = dict(vars(tree))
-        for idx, key in enumerate(vars(tree)):
-            entry = NamedSequenceKey(idx, key)
-            dynamic[key] = (entry, dynamic[key])
-        return tuple(dynamic.values()), tuple(dynamic.keys())
-
-    jtu.register_pytree_with_keys(
-        nodetype=klass,
-        flatten_func=tree_flatten,
-        flatten_with_keys=tree_flatten_with_keys,
-        unflatten_func=tree_unflatten,
-    )
-    return klass
+
+class BaseKey(abc.ABC):
+    """Parent class for all match classes.
+
+    - Subclass this class to create custom match keys by implementing
+      the `__eq__` method. The ``__eq__`` method should return True if the
+      key matches the given path entry and False otherwise. The path entry
+      refers to the entry defined in the ``tree_flatten_with_keys`` method of
+      the pytree class.
+
+    - Typical path entries are:
+
+        - ``jax.tree_util.GetAttrKey`` for attributes
+        - ``jax.tree_util.DictKey`` for mapping keys
+        - ``jax.tree_util.SequenceKey`` for sequence indices
+
+    - When implementing the ``__eq__`` method you can use the ``singledispatchmethod``
+      to unpack the path entry for example:
+
+        - ``jax.tree_util.GetAttrKey`` -> `key.name`
+        - ``jax.tree_util.DictKey`` -> `key.key`
+        - ``jax.tree_util.SequenceKey`` -> `key.index`
+
+
+        See Examples for more details.
+
+    Example:
+        >>> # define an match strategy to match a leaf with a given name and type
+        >>> import pytreeclass as pytc
+        >>> from typing import NamedTuple
+        >>> import jax
+        >>> class NameTypeContainer(NamedTuple):
+        ...     name: str
+        ...     type: type
+        >>> @jax.tree_util.register_pytree_with_keys_class
+        ... class Tree:
+        ...    def __init__(self, a, b) -> None:
+        ...        self.a = a
+        ...        self.b = b
+        ...    def tree_flatten_with_keys(self):
+        ...        ak = (NameTypeContainer("a", type(self.a)), self.a)
+        ...        bk = (NameTypeContainer("b", type(self.b)), self.b)
+        ...        return (ak, bk), None
+        ...    @classmethod
+        ...    def tree_unflatten(cls, aux_data, children):
+        ...        return cls(*children)
+        ...    @property
+        ...    def at(self):
+        ...        return pytc.AtIndexer(self)
+        >>> tree = Tree(1, 2)
+        >>> class MatchNameType(pytc.BaseKey):
+        ...    def __init__(self, name, type):
+        ...        self.name = name
+        ...        self.type = type
+        ...    def __eq__(self, other):
+        ...        if isinstance(other, NameTypeContainer):
+        ...            return other == (self.name, self.type)
+        ...        return False
+        >>> tree = tree.at[MatchNameType("a", int)].get()
+        >>> assert jax.tree_util.tree_leaves(tree) == [1]
+
+    Note:
+        - use ``BaseKey.def_alias(type, func)`` to define an index type alias
+          for `BaseKey` subclasses. This is useful for convience when
+          creating new match strategies.
+
+            >>> import pytreeclass as pytc
+            >>> import functools as ft
+            >>> from types import FunctionType
+            >>> import jax.tree_util as jtu
+            >>> # lets define a new match strategy called `FuncKey` that applies
+            >>> # a function to the path entry and returns True if the function
+            >>> # returns True and False otherwise.
+            >>> # for example `FuncKey(lambda x: x.startswith("a"))` will match
+            >>> # all leaves that start with "a".
+            >>> class FuncKey(pytc.BaseKey):
+            ...    def __init__(self, func):
+            ...        self.func = func
+            ...    @ft.singledispatchmethod
+            ...    def __eq__(self, key):
+            ...        return self.func(key)
+            ...    @__eq__.register(jtu.GetAttrKey)
+            ...    def _(self, key: jtu.GetAttrKey):
+            ...        # unpack the GetAttrKey
+            ...        return self.func(key.name)
+            ...    @__eq__.register(jtu.DictKey)
+            ...    def _(self, key: jtu.DictKey):
+            ...        # unpack the DictKey
+            ...        return self.func(key.key)
+            ...    @__eq__.register(jtu.SequenceKey)
+            ...    def _(self, key: jtu.SequenceKey):
+            ...        return self.func(key.index)
+
+            >>> # instead of using ``FuncKey(function)`` we can define an alias
+            >>> # for `FuncKey`, for this example we will define any FunctionType
+            >>> # as a `FuncKey` by default.
+            >>> @pytc.BaseKey.def_alias(FunctionType)
+            ... def _(func):
+            ...    return FuncKey(func)
+            >>> # create a simple pytree
+            >>> class Tree(pytc.TreeClass):
+            ...    a: int
+            ...    b: str
+            >>> tree = Tree(1, "string")
+            >>> # now we can use the `FuncKey` alias to match all leaves that
+            >>> # are strings and start with "a"
+            >>> tree.at[lambda x: isinstance(x, str) and x.startswith("a")].get()
+            Tree(a=1, b=None)
+    """
+
+    @abc.abstractmethod
+    def __eq__(self, entry: KeyEntry) -> bool:
+        pass
+
+
+class IntKey(BaseKey):
+    def __init__(self, idx: int) -> None:
+        self.idx = idx
+
+    @ft.singledispatchmethod
+    def __eq__(self, _: KeyEntry) -> bool:
+        return False
+
+    @__eq__.register(int)
+    def _(self, other: int) -> bool:
+        return self.idx == other
+
+    @__eq__.register(jtu.SequenceKey)
+    def _(self, other: jtu.SequenceKey) -> bool:
+        return self.idx == other.idx
+
+
+class NameKey(BaseKey):
+    def __init__(self, name: str) -> None:
+        self.name = name
+
+    @ft.singledispatchmethod
+    def __eq__(self, _: KeyEntry) -> bool:
+        return False
+
+    @__eq__.register(str)
+    def _(self, other: str) -> bool:
+        return self.name == other
+
+    @__eq__.register(jtu.GetAttrKey)
+    def _(self, other: jtu.GetAttrKey) -> bool:
+        return self.name == other.name
+
+    @__eq__.register(jtu.DictKey)
+    def _(self, other: jtu.__doc__) -> bool:
+        return self.name == other.key
+
+
+class EllipsisKey(BaseKey):
+    def __init__(self, _):
+        del _
+
+    def __eq__(self, _: KeyEntry) -> bool:
+        return True
+
+
+class MultiKey(BaseKey):
+    """Match a leaf with multiple keys at the same level."""
+
+    def __init__(self, *keys: tuple[BaseKey, ...]):
+        self.keys = tuple(keys)
+
+    def __eq__(self, entry) -> bool:
+        return any(entry == key for key in self.keys)
+
+
+class RegexKey(BaseKey):
+    """Match a leaf with a regex pattern inside 'at' property.
+
+    Args:
+        pattern: regex pattern to match.
+
+    Example:
+        >>> import pytreeclass as pytc
+        >>> import re
+        >>> class Tree(pytc.TreeClass):
+        ...     weight_1: float = 1.0
+        ...     weight_2: float = 2.0
+        ...     weight_3: float = 3.0
+        ...     bias: float = 0.0
+        >>> tree = Tree()
+        >>> tree.at[re.compile(r"weight_.*")].set(100.0)  # set all weights to 100.0
+        Tree(weight_1=100.0, weight_2=100.0, weight_3=100.0, bias=0.0)
+    """
+
+    def __init__(self, pattern: str) -> None:
+        self.pattern = pattern
+
+    @ft.singledispatchmethod
+    def __eq__(self, _: KeyEntry) -> bool:
+        return False
+
+    @__eq__.register(str)
+    def _(self, other: str) -> bool:
+        return re.fullmatch(self.pattern, other) is not None
+
+    @__eq__.register(jtu.GetAttrKey)
+    def _(self, other) -> bool:
+        return re.fullmatch(self.pattern, other.name) is not None
+
+    @__eq__.register(jtu.DictKey)
+    def _(self, other) -> bool:
+        return re.fullmatch(self.pattern, other.key) is not None
+
+
+# dispatch on type of indexer to convert input item to at indexer
+# `__getitem__` to the appropriate key
+# avoid using container pytree types to avoid conflict between
+# matching as a mask or as an instance of `BaseKey`
+indexer_dispatcher = ft.singledispatch(lambda x: x)
+indexer_dispatcher.register(type(...), EllipsisKey)
+indexer_dispatcher.register(int, IntKey)
+indexer_dispatcher.register(str, NameKey)
+indexer_dispatcher.register(re.Pattern, RegexKey)
+
+BaseKey.def_alias = indexer_dispatcher.register
+
+
+_NOT_IMPLEMENTED_INDEXING = """Indexing with {} is not implemented, supported indexing types are:
+- `str` for mapping keys or class attributes.
+- `int` for positional indexing for sequences.
+- `...` to select all leaves.
+- Boolean mask of the same structure as the tree
+- `re.Pattern` to index all keys matching a regex pattern.
+- Instance of `BaseKey` with custom logic to index a pytree.
+- `tuple` of the above types to match multiple leaves at the same level.
+"""
+
+
+def _generate_path_mask(
+    tree: PyTree,
+    where: tuple[BaseKey, ...],
+    is_leaf: IsLeafType = None,
+) -> PyTree:
+    # generate a boolean mask for `where` path in `tree`
+    # where path is a tuple of indices or keys, for example
+    # where=("a",) wil set all leaves of `tree` with key "a" to True and
+    # all other leaves to False
+    match = False
+
+    def map_func(path, _: Any):
+        if len(where) > len(path):
+            # path is shorter than `where` path. for example
+            # where=("a", "b") and the current path is ("a",) then
+            # the current path is not a match
+            return False
+        for wi, ki in zip(where, path):
+            if not (wi == ki):
+                return False
+
+        nonlocal match
+        match = True
+        return match
+
+    mask = jtu.tree_map_with_path(map_func, tree, is_leaf=is_leaf)
+
+    if not match:
+        raise LookupError(f"No leaf match is found for {where=}.")
+
+    return mask
+
+
+def _combine_bool_leaves(*leaves):
+    verdict = True
+    for leaf in leaves:
+        verdict &= leaf
+    return verdict
+
+
+def _is_bool_leaf(leaf: Any) -> bool:
+    if hasattr(leaf, "dtype"):
+        return leaf.dtype == "bool"
+    return isinstance(leaf, bool)
+
+
+def _resolve_where(
+    tree: T,
+    where: tuple[Any, ...],  # type: ignore
+    is_leaf: IsLeafType = None,
+) -> T | None:
+    mask = None
+    bool_masks: list[T] = []
+    path_masks: list[BaseKey] = []
+    treedef0 = jtu.tree_structure(tree, is_leaf=is_leaf)
+    seen_tuple = False  # handle multiple keys at the same level
+    level_paths = []
+
+    def verify_and_aggregate_is_leaf(x) -> bool:
+        # use is_leaf with non-local to traverse the tree depth-first manner
+        # required for verifying if a pytree is a valid indexing pytree
+        nonlocal seen_tuple, level_paths, bool_masks
+        # used to check if a pytree is a valid indexing pytree
+        # used with `is_leaf` argument of any `jtu.tree_*` function
+        leaves, treedef = jtu.tree_flatten(x)
+
+        if treedef == treedef0 and all(map(_is_bool_leaf, leaves)):
+            # boolean pytrees of same structure as `tree` is a valid indexing pytree
+            bool_masks += [x]
+            return True
+
+        if isinstance(resolved_key := indexer_dispatcher(x), BaseKey):
+            # valid resolution of `BaseKey` is a valid indexing leaf
+            # makes it possible to dispatch on multi-leaf pytree
+            level_paths += [resolved_key]
+            return False
+
+        if type(x) is tuple and seen_tuple is False:
+            # e.g. `at[1,2,3]` but not `at[1,(2,3)]``
+            seen_tuple = True
+            return False
+
+        # not a container of other keys or a pytree of same structure
+        raise NotImplementedError(_NOT_IMPLEMENTED_INDEXING.format(x))
+
+    for level_keys in where:
+        # each for loop iteration is a level in the where path
+        jtu.tree_leaves(level_keys, is_leaf=verify_and_aggregate_is_leaf)
+        path_masks += [MultiKey(*level_paths)] if len(level_paths) > 1 else level_paths
+        level_paths = []
+        seen_tuple = False
+
+    if path_masks:
+        mask = _generate_path_mask(tree, path_masks, is_leaf=is_leaf)
+
+    if bool_masks:
+        all_masks = [mask, *bool_masks] if mask else bool_masks
+        mask = jax.tree_map(_combine_bool_leaves, *all_masks)
+
+    return mask
 
 
 class AtIndexer(NamedTuple):
-    """Adds `.at` indexing abilities to a PyTree.
+    """Index a pytree at a given path using a path or mask.
+
+    Args:
+        tree: pytree to index
+        where: one of the following:
+
+            - ``str`` for mapping keys or class attributes.
+            - ``int`` for positional indexing for sequences.
+            - ``...`` to select all leaves.
+            - a boolean mask of the same structure as the tree
+            - ``re.Pattern`` to index all keys matching a regex pattern.
+            - an instance of ``BaseKey`` with custom logic to index a pytree.
+            - a tuple of the above to match multiple keys at the same level.
 
     Example:
+        >>> # use `AtIndexer` on a pytree (e.g. dict,list,tuple,etc.)
+        >>> import jax
+        >>> import pytreeclass as pytc
+        >>> tree = {"level1_0": {"level2_0": 100, "level2_1": 200}, "level1_1": 300}
+        >>> tree = pytc.AtIndexer(tree)
+        >>> tree.at["level1_0"].at["level2_0"].get()
+        {'level1_0': {'level2_0': 100, 'level2_1': None}, 'level1_1': None}
+        >>> # get multiple keys at once at the same level
+        >>> tree.at["level1_0"].at["level2_0", "level2_1"].get()
+        {'level1_0': {'level2_0': 100, 'level2_1': 200}, 'level1_1': None}
+        >>> # get with a mask
+        >>> mask = {"level1_0": {"level2_0": True, "level2_1": False}, "level1_1": True}
+        >>> tree.at[mask].get()
+        {'level1_0': {'level2_0': 100, 'level2_1': None}, 'level1_1': 300}
+
+    Example:
+        >>> # use ``AtIndexer`` in a class
         >>> import jax.tree_util as jtu
         >>> import pytreeclass as pytc
         >>> @jax.tree_util.register_pytree_with_keys_class
         ... class Tree:
         ...    def __init__(self, a, b):
         ...        self.a = a
         ...        self.b = b
@@ -112,66 +421,60 @@
         ...        kvb = (jtu.GetAttrKey("b"), self.b)
         ...        return (kva, kvb), None
         ...    @classmethod
         ...    def tree_unflatten(cls, aux_data, children):
         ...        return cls(*children)
         ...    @property
         ...    def at(self):
-        ...        return pytc.AtIndexer(self, where=())
+        ...        return pytc.AtIndexer(self)
         ...    def __repr__(self) -> str:
         ...        return f"{self.__class__.__name__}(a={self.a}, b={self.b})"
-
         >>> Tree(1, 2).at["a"].get()
         Tree(a=1, b=None)
     """
 
     tree: PyTree
-    where: tuple[str | int] | PyTree = ()
+    where: tuple[BaseKey | PyTree] | tuple[()] = ()
 
-    def __getitem__(self, where: WhereType) -> AtIndexer:
-        if isinstance(where, (type(self.tree), *WhereAtomType)):
-            return AtIndexer(self.tree, (*self.where, where))
-
-        raise NotImplementedError(
-            f"Indexing with {type(where).__name__} is not implemented.\n"
-            "Example of supported indexing:\n\n"
-            ">>> import jax\n"
-            ">>> import pytreeclass as pytc\n"
-            f"class {type(self.tree).__name__}(pytc.TreeClass):\n"
-            "    ...\n\n"
-            f">>> tree = {type(self.tree).__name__}(...)\n"
-            ">>> # indexing by boolean pytree\n"
-            ">>> mask = jax.tree_map(lambda x: x > 0, tree)\n"
-            ">>> tree.at[mask].get()\n\n"
-            ">>> # indexing by attribute name\n"
-            ">>> tree.at[`attribute_name`].get()\n\n"
-            ">>> # indexing by leaf index\n"
-            ">>> tree.at[index].get()\n"
-            ">>> # indexing by regex pattern\n"
-            ">>> tree.at[pytc.RegexKey(`pattern`)].get()\n"
-        )
+    def __getitem__(self, where: Any) -> AtIndexer:
+        return type(self)(self.tree, (*self.where, where))
+
+    def __getattr__(self, name: str) -> AtIndexer:
+        """Support nested indexing."""
+        if name == "at":
+            # pass the current tree and the current path to the next `.at`
+            return type(self)(tree=self.tree, where=self.where)
+
+        raise AttributeError(f"`{self!r}` has no attribute {name!r}.")
 
     def get(self, *, is_leaf: IsLeafType = None) -> PyTree:
         """Get the leaf values at the specified location.
 
         Args:
             is_leaf: a predicate function to determine if a value is a leaf.
 
         Returns:
-            A PyTree of leaf values at the specified location, with the
+            A _new_ pytree of leaf values at the specified location, with the
             non-selected leaf values set to None if the leaf is not an array.
 
         Example:
             >>> import pytreeclass as pytc
+            >>> tree = {"level1_0": {"level2_0": 100, "level2_1": 200}, "level1_1": 300}
+            >>> tree = pytc.AtIndexer(tree)
+            >>> tree.at["level1_0"].at["level2_0"].get()
+            {'level1_0': {'level2_0': 100, 'level2_1': None}, 'level1_1': None}
+
+        Example:
+            >>> import pytreeclass as pytc
             >>> class Tree(pytc.TreeClass):
             ...     a: int
             ...     b: int
             >>> tree = Tree(a=1, b=2)
-            >>> # get `a` and return a new instance
-            >>> # with `None` for all other leaves
+            >>> # get ``a`` and return a new instance
+            >>> # with ``None`` for all other leaves
             >>> tree.at['a'].get()
             Tree(a=1, b=None)
         """
         where = _resolve_where(self.tree, self.where, is_leaf)
 
         def leaf_get(leaf: Any, where: Any):
             if isinstance(where, (jax.Array, np.ndarray)) and where.ndim != 0:
@@ -184,41 +487,48 @@
         """Set the leaf values at the specified location.
 
         Args:
             set_value: the value to set at the specified location.
             is_leaf: a predicate function to determine if a value is a leaf.
 
         Returns:
-            A PyTree with the leaf values at the specified location
-            set to `set_value`.
+            A pytree with the leaf values at the specified location
+            set to ``set_value``.
+
+        Example:
+            >>> import pytreeclass as pytc
+            >>> tree = {"level1_0": {"level2_0": 100, "level2_1": 200}, "level1_1": 300}
+            >>> tree = pytc.AtIndexer(tree)
+            >>> tree.at["level1_0"].at["level2_0"].set('SET')
+            {'level1_0': {'level2_0': 'SET', 'level2_1': 200}, 'level1_1': 300}
 
         Example:
             >>> import pytreeclass as pytc
             >>> class Tree(pytc.TreeClass):
             ...     a: int
             ...     b: int
             >>> tree = Tree(a=1, b=2)
-            >>> # set `a` and return a new instance
+            >>> # set ``a`` and return a new instance
             >>> # with all other leaves unchanged
             >>> tree.at['a'].set(100)
             Tree(a=100, b=2)
         """
         where = _resolve_where(self.tree, self.where, is_leaf)
 
         def leaf_set(leaf: Any, where: Any, set_value: Any):
             if isinstance(where, (jax.Array, np.ndarray)):
                 return jnp.where(where, set_value, leaf)
             return set_value if where else leaf
 
-        if jtu.tree_structure(self.tree) == jtu.tree_structure(set_value):
+        if jtu.tree_structure(self.tree, is_leaf) == jtu.tree_structure(set_value):
             # do not broadcast set_value if it is a pytree of same structure
             # for example tree.at[where].set(tree2) will set all tree leaves
             # to tree2 leaves if tree2 is a pytree of same structure as tree
             # instead of making each leaf of tree a copy of tree2
-            # is design is similar to `numpy` design `Array.at[...].set(Array)`
+            # is design is similar to ``numpy`` design `Array.at[...].set(Array)`
             return jtu.tree_map(leaf_set, self.tree, where, set_value, is_leaf=is_leaf)
 
         # set_value is broadcasted to tree leaves
         # for example tree.at[where].set(1) will set all tree leaves to 1
         partial_leaf_set = lambda leaf, where: leaf_set(leaf, where, set_value)
         return jtu.tree_map(partial_leaf_set, self.tree, where, is_leaf=is_leaf)
 
@@ -226,459 +536,151 @@
         """Apply a function to the leaf values at the specified location.
 
         Args:
             func: the function to apply to the leaf values.
             is_leaf: a predicate function to determine if a value is a leaf.
 
         Returns:
-            A PyTree with the leaf values at the specified location set to
-            the result of applying `func` to the leaf values.
+            A pytree with the leaf values at the specified location set to
+            the result of applying ``func`` to the leaf values.
+
+        Example:
+            >>> import pytreeclass as pytc
+            >>> tree = {"level1_0": {"level2_0": 100, "level2_1": 200}, "level1_1": 300}
+            >>> tree = pytc.AtIndexer(tree)
+            >>> tree.at["level1_0"].at["level2_0"].apply(lambda _: 'SET')
+            {'level1_0': {'level2_0': 'SET', 'level2_1': 200}, 'level1_1': 300}
 
         Example:
             >>> import pytreeclass as pytc
             >>> class Tree(pytc.TreeClass):
             ...     a: int
             ...     b: int
             >>> tree = Tree(a=1, b=2)
-            >>> # apply to `a` and return a new instance
+            >>> # apply to ``a`` and return a new instance
             >>> # with all other leaves unchanged
             >>> tree.at['a'].apply(lambda _: 100)
             Tree(a=100, b=2)
         """
         where = _resolve_where(self.tree, self.where, is_leaf)
 
         def leaf_apply(leaf: Any, where: bool):
             if isinstance(where, (jax.Array, np.ndarray)):
                 return jnp.where(where, func(leaf), leaf)
             return func(leaf) if where else leaf
 
         return jtu.tree_map(leaf_apply, self.tree, where, is_leaf=is_leaf)
 
-    def reduce(
+    def scan(
         self,
-        func: Callable[[Any, Any], Any],
+        func: Callable[[Any, S], tuple[Any, S]],
+        state: S,
         *,
-        initializer: Any = _no_initializer,
         is_leaf: IsLeafType = None,
-    ) -> Any:
-        """Reduce the leaf values at the specified location.
+    ) -> tuple[PyTree, S]:
+        """Apply a function with carrtying a state.
 
         Args:
-            func: the function to reduce the leaf values.
-            initializer: the initializer value for the reduction.
-            is_leaf: a predicate function to determine if a value is a leaf.
+            func: the function to apply to the leaf values. the function accepts
+                a running state and leaf value and returns a tuple of the new
+                leaf value and the new state.
+            state: the initial state to carry.
+            is_leaf: a predicate function to determine if a value is a leaf. for
+                example, ``lambda x: isinstance(x, list)`` will treat all lists
+                as leaves and will not recurse into list items.
 
         Returns:
-            The result of reducing the leaf values at the specified location.
+            A tuple of the final state and pytree with the leaf values at the
+            specified location set to the result of applying ``func`` to the leaf
+            values.
 
         Example:
             >>> import pytreeclass as pytc
-            >>> class Tree(pytc.TreeClass):
-            ...     a: int
-            ...     b: int
-            >>> tree = Tree(a=1, b=2)
-            >>> tree.at[...].reduce(lambda a, b: a + b, initializer=0)
-            3
-        """
-        where = _resolve_where(self.tree, self.where, is_leaf)
-        tree = self.tree.at[where].get(is_leaf=is_leaf)  # type: ignore
-        if initializer is _no_initializer:
-            return jtu.tree_reduce(func, tree)
-        return jtu.tree_reduce(func, tree, initializer)
-
-    def __getattr__(self, name: str) -> AtIndexer:
-        """Support nested indexing"""
-        if name == "at":
-            # pass the current tree and the current path to the next `.at`
-            return AtIndexer(tree=self.tree, where=self.where)
-
-        raise AttributeError(f"`{type(self).__name__!r}` has no attribute {name!r}.")
-
-    def __call__(self, *a, **k) -> tuple[Any, PyTree]:
-        """
-        Call the function at the specified location and return a **copy**
-        of the tree. with the result of the function call.
-
-        Returns:
-            A tuple of the result of the function call and a copy of the a
-            new instance of the tree with the modified values.
+            >>> tree = {"level1_0": {"level2_0": 100, "level2_1": 200}, "level1_1": 300}
+            >>> def scan_func(leaf, state):
+            ...     return 'SET', state + 1
+            >>> init_state = 0
+            >>> tree = pytc.AtIndexer(tree)
+            >>> tree.at["level1_0"].at["level2_0"].scan(scan_func, state=init_state)
+            ({'level1_0': {'level2_0': 'SET', 'level2_1': 200}, 'level1_1': 300}, 1)
 
         Example:
             >>> import pytreeclass as pytc
+            >>> from typing import NamedTuple
+            >>> class State(NamedTuple):
+            ...     func_evals: int = 0
             >>> class Tree(pytc.TreeClass):
             ...     a: int
-            ...     def add(self, x:int) -> int:
-            ...         self.a += x
-            ...         return self.a
-            >>> tree = Tree(a=1)
-            >>> # call `add` and return a tuple of
-            >>> # (return value, new instance)
-            >>> tree.at['add'](99)
-            (100, Tree(a=100))
+            ...     b: int
+            ...     c: int
+            >>> tree = Tree(a=1, b=2, c=3)
+            >>> def scan_func(leaf, state: State):
+            ...     state = State(state.func_evals + 1)
+            ...     return leaf + 1, state
+            >>> # apply to ``a`` and ``b`` and return a new instance with all other
+            >>> # leaves unchanged and the new state that counts the number of
+            >>> # function evaluations
+            >>> tree.at['a','b'].scan(scan_func, state=State())
+            (Tree(a=2, b=3, c=3), State(func_evals=2))
 
         Note:
-            - `AttributeError` is raised, If the function mutates the instance.
-            - Use .at["method_name"](*, **) to call a method that mutates the instance.
+            ``scan`` applies a binary ``func`` to the leaf values while carrying
+            a state and returning a tree leaves with the the ``func`` applied to
+            them with final state. While ``reduce`` applies a binary ``func`` to the
+            leaf values while carrying a state and returning a single value.
         """
+        where = _resolve_where(self.tree, self.where, is_leaf)
 
-        def recursive_getattr(tree: Any, where: tuple[str, ...]):
-            if len(where) == 1:
-                return getattr(tree, where[0])
-            return recursive_getattr(getattr(tree, where[0]), where[1:])
-
-        with _mutable_context(self.tree, kopy=True) as tree:
-            value = recursive_getattr(tree, self.where)(*a, **k)  # type: ignore
-        return value, tree
-
-
-class TreeClassMeta(abc.ABCMeta):
-    def __call__(klass: type[T], *a, **k) -> T:
-        self = getattr(klass, "__new__")(klass, *a, **k)
-
-        with _mutable_context(self):
-            # initialize the instance under the mutable context
-            # to allow setting instance attributes without
-            # throwing an `AttributeError`
-            getattr(klass, "__init__")(self, *a, **k)
-
-        if keys := set(_build_field_map(klass)) - set(vars(self)):
-            raise AttributeError(f"Found uninitialized fields {keys}.")
-        return self
-
-
-@dataclass_transform(field_specifiers=(field, Field))
-class TreeClass(metaclass=TreeClassMeta):
-    """Convert a class to a JAX compatible tree structure.
+        running_state = state
 
-    Example:
-        >>> import jax
-        >>> import pytreeclass as pytc
+        def stateless_func(leaf):
+            nonlocal running_state
+            leaf, running_state = func(leaf, running_state)
+            return leaf
 
-        >>> # Tree leaves are instance attributes
-        >>> class Tree(pytc.TreeClass):
-        ...     a:int = 1
-        ...     b:float = 2.0
-        >>> tree = Tree()
-        >>> jax.tree_util.tree_leaves(tree)
-        [1, 2.0]
+        def leaf_apply(leaf: Any, where: bool):
+            if isinstance(where, (jax.Array, np.ndarray)):
+                return jnp.where(where, stateless_func(leaf), leaf)
+            return stateless_func(leaf) if where else leaf
 
-        >>> # Leaf-wise math operations are supported by setting `leafwise=True`
-        >>> class Tree(pytc.TreeClass, leafwise=True):
-        ...     a:int = 1
-        ...     b:float = 2.0
-        >>> tree = Tree()
-        >>> tree + 1
-        Tree(a=2, b=3.0)
+        out = jtu.tree_map(leaf_apply, self.tree, where, is_leaf=is_leaf)
+        return out, running_state
 
-        >>> # Advanced indexing is supported using `at` property
-        >>> class Tree(pytc.TreeClass):
-        ...     a:int = 1
-        ...     b:float = 2.0
-        >>> tree = Tree()
-        >>> tree.at["a"].get()
-        Tree(a=1, b=None)
-        >>> tree.at[0].get()
-        Tree(a=1, b=None)
-
-    Note:
-        ``leafwise=True`` adds the following methods to the class
+    def reduce(
+        self,
+        func: Callable[[Any, Any], Any],
+        *,
+        initializer: Any = _no_initializer,
+        is_leaf: IsLeafType = None,
+    ) -> Any:
+        """Reduce the leaf values at the specified location.
 
-        ==================      ============
-        Method                  Operator
-        ==================      ============
-        ``__add__``              ``+``
-        ``__and__``              ``&``
-        ``__ceil__``             ``math.ceil``
-        ``__divmod__``           ``divmod``
-        ``__eq__``               ``==``
-        ``__floor__``            ``math.floor``
-        ``__floordiv__``         ``//``
-        ``__ge__``               ``>=``
-        ``__gt__``               ``>``
-        ``__invert__``           ``~``
-        ``__le__``               ``<=``
-        ``__lshift__``           ``<<``
-        ``__lt__``               ``<``
-        ``__matmul__``           ``@``
-        ``__mod__``              ``%``
-        ``__mul__``              ``*``
-        ``__ne__``               ``!=``
-        ``__neg__``              ``-``
-        ``__or__``               ``|``
-        ``__pos__``              ``+``
-        ``__pow__``              ``**``
-        ``__round__``            ``round``
-        ``__sub__``              ``-``
-        ``__truediv__``          ``/``
-        ``__trunc__``            ``math.trunc``
-        ``__xor__``              ``^``
-        ==================      ============
+        Args:
+            func: the function to reduce the leaf values.
+            initializer: the initializer value for the reduction.
+            is_leaf: a predicate function to determine if a value is a leaf.
 
-    """
+        Returns:
+            The result of reducing the leaf values at the specified location.
 
-    def __init_subclass__(
-        klass: type[T],
-        *a,
-        leafwise: bool = False,
-        **k,
-    ) -> None:
-        if "__setattr__" in vars(klass) or "__delattr__" in vars(klass):
-            raise TypeError(
-                f"Unable to transform the class `{klass.__name__}` "
-                "with resereved methods: `__setattr__` or `__delattr__` "
-                "defined.\nReserved `setters` and `deleters` implements "
-                "the immutable functionality and cannot be overriden."
-            )
-
-        super().__init_subclass__(*a, **k)
-
-        if "__init__" not in vars(klass):
-            # generate the init method if not defined similar to `dataclass`
-            setattr(klass, "__init__", _build_init_method(klass))
-
-        if leafwise:
-            # transform the class to support leafwise operations
-            # useful to use with `bcmap` and creating masks by comparisons.
-            klass = _leafwise_transform(klass)
-
-        klass = _register_treeclass(klass)
-
-    def __setattr__(self, key: str, value: Any) -> None:
-        if id(self) not in _mutable_instance_registry:
-            # instance is not under a mutable context
-            # mutable context is used for setting instance attributes
-            # during initialization and when using the `at` property
-            # with call method.
-            raise AttributeError(
-                f"Cannot set attribute {value=} to `{key=}`  "
-                f"on an immutable instance of `{type(self).__name__}`.\n"
-                f"Use `.at['{key}'].set({value})` "
-                "to set the value immutably.\nExample:\n"
-                f">>> tree1 = {type(self).__name__}(...)\n"
-                f">>> tree2 = tree1.at['{key}'].set({value!r})\n"
-                ">>> assert not tree1 is tree2\n"
-                f">>> tree2.{key}\n{value}"
-            )
-
-        if key in (field_map := _build_field_map(type(self))):
-            # apply field callbacks on the value before setting
-            value = field_map[key](value)
-
-        getattr(object, "__setattr__")(self, key, value)
-
-    def __delattr__(self, key: str) -> None:
-        if id(self) not in _mutable_instance_registry:
-            # instance is not under a mutable context
-            raise AttributeError(
-                f"Cannot delete attribute `{key}` "
-                f"on immutable instance of `{type(self).__name__}`.\n"
-                f"Use `.at['{key}'].set(None)` instead."
-            )
-
-        getattr(object, "__delattr__")(self, key)
-
-    @property
-    def at(self) -> AtIndexer:
-        """Immutable out-of-place indexing
-
-        - `.at[***].get()`:
-            Return a new instance with the value at the index otherwise None.
-        - `.at[***].set(value)`:
-            Set the `value` and return a new instance with the updated value.
-        - `.at[***].apply(func)`:
-            Apply a `func` and return a new instance with the updated value.
-        - `.at['method'](*a, **k)`:
-            Call a `method` and return a (return value, new instance) tuple.
-
-        `***` acceptable index types are `str` for mapping keys or
-        class attributes, `int` for positional indexing, `...` to select all leaves,
-        , a boolean mask of the same structure as the tree.
+        Note:
+            - If ``initializer`` is not specified, the first leaf value is used as
+              the initializer.
+            - ``reduce`` applies a binary ``func`` to each leaf values while accumulating
+              a state a returns the final result. while ``scan`` applies ``func`` to each
+              leaf value while carrying a state and returns the final state and
+              the leaves of the tree with the result of applying ``func`` to each leaf.
 
         Example:
             >>> import pytreeclass as pytc
             >>> class Tree(pytc.TreeClass):
-            ...     a:int = 1
-            ...     b:float = 2.0
-            ...     def add(self, x:int) -> int:
-            ...         self.a += x
-            ...         return self.a
-            >>> tree = Tree()
-            >>> # get `a` and return a new instance
-            >>> # with `None` for all other leaves
-            >>> tree.at["a"].get()
-            Tree(a=1, b=None)
-            >>> # set `a` and return a new instance
-            >>> # with all other leaves unchanged
-            >>> tree.at["a"].set(100)
-            Tree(a=100, b=2.0)
-            >>> # apply to `a` and return a new instance
-            >>> # with all other leaves unchanged
-            >>> tree.at["a"].apply(lambda x: 100)
-            Tree(a=100, b=2.0)
-            >>> # call `add` and return a tuple of
-            >>> # (return value, new instance)
-            >>> tree.at["add"](99)
-            (100, Tree(a=100, b=2.0))
+            ...     a: int
+            ...     b: int
+            >>> tree = Tree(a=1, b=2)
+            >>> tree.at[...].reduce(lambda a, b: a + b, initializer=0)
+            3
         """
-        return AtIndexer(self)
-
-    def __repr__(self) -> str:
-        return tree_repr(self)
-
-    def __str__(self) -> str:
-        return tree_str(self)
-
-    def __copy__(self):
-        return tree_copy(self)
-
-    def __hash__(self) -> int:
-        return tree_hash(self)
-
-    def __eq__(self, other: Any) -> bool | jax.Array:
-        return is_tree_equal(self, other)
-
-
-def _frozen_error(opname: str, tree):
-    raise NotImplementedError(
-        f"Cannot apply `{opname}` operation to a frozen object `{tree!r}`.\n"
-        "Unfreeze the object first to apply operations to it\n"
-        "Example:\n"
-        ">>> import jax\n"
-        ">>> import pytreeclass as pytc\n"
-        ">>> tree = jax.tree_map(pytc.unfreeze, tree, is_leaf=pytc.is_frozen)"
-    )
-
-
-class _Frozen(Generic[T]):
-    __slots__ = ("__wrapped__", "__weakref__")
-    __wrapped__: T
-
-    def __init__(self, x: T) -> None:
-        object.__setattr__(self, "__wrapped__", x)
-
-    def __setattr__(self, _, __) -> None:
-        raise AttributeError("Cannot assign to frozen instance.")
-
-    def __delattr__(self, _: str) -> None:
-        raise AttributeError("Cannot delete from frozen instance.")
-
-    def __repr__(self) -> str:
-        return "#" + tree_repr(self.__wrapped__)
-
-    def __str__(self) -> str:
-        return "#" + tree_str(self.__wrapped__)
-
-    def __copy__(self) -> _Frozen[T]:
-        return _Frozen(tree_copy(self.__wrapped__))
-
-    def __eq__(self, rhs: Any) -> bool | jax.Array:
-        if not isinstance(rhs, _Frozen):
-            return False
-        return is_tree_equal(self.__wrapped__, rhs.__wrapped__)
-
-    def __hash__(self) -> int:
-        return tree_hash(self.__wrapped__)
-
-    # raise helpful error message when trying to interact with frozen object
-    __add__ = __radd__ = __iadd__ = lambda x, _: _frozen_error("+", x)
-    __sub__ = __rsub__ = __isub__ = lambda x, _: _frozen_error("-", x)
-    __mul__ = __rmul__ = __imul__ = lambda x, _: _frozen_error("*", x)
-    __matmul__ = __rmatmul__ = __imatmul__ = lambda x, _: _frozen_error("@", x)
-    __truediv__ = __rtruediv__ = __itruediv__ = lambda x, _: _frozen_error("/", x)
-    __floordiv__ = __rfloordiv__ = __ifloordiv__ = lambda x, _: _frozen_error("//", x)
-    __mod__ = __rmod__ = __imod__ = lambda x, _: _frozen_error("%", x)
-    __pow__ = __rpow__ = __ipow__ = lambda x, _: _frozen_error("**", x)
-    __lshift__ = __rlshift__ = __ilshift__ = lambda x, _: _frozen_error("<<", x)
-    __rshift__ = __rrshift__ = __irshift__ = lambda x, _: _frozen_error(">>", x)
-    __and__ = __rand__ = __iand__ = lambda x, _: _frozen_error("and", x)
-    __xor__ = __rxor__ = __ixor__ = lambda x, _: _frozen_error("xor", x)
-    __or__ = __ror__ = __ior__ = lambda x, _: _frozen_error("or", x)
-    __neg__ = __pos__ = __abs__ = __invert__ = lambda x: _frozen_error("unary op", x)
-    __call__ = lambda x, *_, **__: _frozen_error("call", x)
-
-
-jtu.register_pytree_node(
-    nodetype=_Frozen,
-    flatten_func=lambda tree: ((), tree),
-    unflatten_func=lambda treedef, _: treedef,
-)
-
-
-def freeze(wrapped: _Frozen[T] | T) -> _Frozen[T]:
-    """Freeze a value to avoid updating it by `jax` transformations.
-
-    Example:
-        >>> import jax
-        >>> import pytreeclass as pytc
-        >>> import jax.tree_util as jtu
-        >>> # Usage with `jax.tree_util.tree_leaves`
-        >>> # no leaves for a wrapped value
-        >>> jtu.tree_leaves(pytc.freeze(2.))
-        []
-
-        >>> # retrieve the frozen wrapper value using `is_leaf=pytc.is_frozen`
-        >>> jtu.tree_leaves(pytc.freeze(2.), is_leaf=pytc.is_frozen)
-        [#2.0]
-
-        >>> # Usage with `jax.tree_util.tree_map`
-        >>> a= [1,2,3]
-        >>> a[1] = pytc.freeze(a[1])
-        >>> jtu.tree_map(lambda x:x+100, a)
-        [101, #2, 103]
-    """
-    return wrapped if is_frozen(wrapped) else _Frozen(wrapped)  # type: ignore
-
-
-def is_frozen(wrapped: Any) -> bool:
-    """Returns True if the value is a frozen wrapper."""
-    return isinstance(wrapped, _Frozen)
-
-
-def unfreeze(wrapped: _Frozen[T] | T) -> T:
-    """Unfreeze `frozen` value, otherwise return the value itself.
-
-    - use `is_leaf=pytc.is_frozen` with `jax.tree_map` to unfreeze a tree.**
-
-    Example:
-        >>> import pytreeclass as pytc
-        >>> import jax
-        >>> frozen_value = pytc.freeze(1)
-        >>> pytc.unfreeze(frozen_value)
-        1
-        >>> # usage with `jax.tree_map`
-        >>> frozen_tree = jax.tree_map(pytc.freeze, {"a": 1, "b": 2})
-        >>> unfrozen_tree = jax.tree_map(pytc.unfreeze, frozen_tree, is_leaf=pytc.is_frozen)
-        >>> unfrozen_tree
-        {'a': 1, 'b': 2}
-    """
-    return getattr(wrapped, "__wrapped__") if is_frozen(wrapped) else wrapped
-
-
-def is_nondiff(wrapped: Any) -> bool:
-    """
-    Returns True if the node is a non-differentiable node, and False for if the
-    node is of type float, complex number, or a numpy array of floats or
-    complex numbers.
-
-    Example:
-        >>> import pytreeclass as pytc
-        >>> import jax.numpy as jnp
-        >>> pytc.is_nondiff(jnp.array(1))  # int array is non-diff type
-        True
-        >>> pytc.is_nondiff(jnp.array(1.))  # float array is diff type
-        False
-        >>> pytc.is_nondiff(1)  # int is non-diff type
-        True
-        >>> pytc.is_nondiff(1.)  # float is diff type
-        False
-
-    Note:
-        This function is meant to be used with `jax.tree_map` to
-        create a mask for non-differentiable nodes in a tree, that can be used
-        to freeze the non-differentiable nodes before passing the tree to a
-        `jax` transformation.
-    """
-    if hasattr(wrapped, "dtype") and np.issubdtype(wrapped.dtype, np.inexact):
-        return False
-    if isinstance(wrapped, (float, complex)):
-        return False
-    return True
+        where = _resolve_where(self.tree, self.where, is_leaf)
+        tree = self.at[where].get(is_leaf=is_leaf)  # type: ignore
+        if initializer is _no_initializer:
+            return jtu.tree_reduce(func, tree)
+        return jtu.tree_reduce(func, tree, initializer)
```

### Comparing `pytreeclass-0.3.8/pytreeclass/_src/tree_util.py` & `pytreeclass-0.4.0/pytreeclass/_src/tree_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,85 +7,51 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 """Utility functions for pytrees."""
 
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
 import operator as op
-import re
-from collections import defaultdict
 from math import ceil, floor, trunc
-from typing import (
-    Any,
-    Callable,
-    Hashable,
-    Iterator,
-    NamedTuple,
-    Sequence,
-    Tuple,
-    TypeVar,
-    Union,
-)
+from typing import Any, Callable, Hashable, Iterator, Sequence, Tuple, TypeVar, Union
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from jax._src.tree_util import _registry, _registry_with_keypaths
 from jax.util import unzip2
 
 T = TypeVar("T")
 PyTree = Any
-# TODO: swich to type(Ellipsis) for python 3.10
+# TODO: swich to EllipsisType for python 3.10
 EllipsisType = TypeVar("EllipsisType")
 KeyEntry = TypeVar("KeyEntry", bound=Hashable)
 TypeEntry = TypeVar("TypeEntry", bound=type)
 TraceEntry = Tuple[KeyEntry, TypeEntry]
 KeyPath = Tuple[KeyEntry, ...]
 TypePath = Tuple[TypeEntry, ...]
 TraceType = Tuple[KeyPath, TypePath]
 IsLeafType = Union[None, Callable[[Any], bool]]
 
 
-class RegexKey(NamedTuple):
-    """Match a leaf with a regex pattern inside 'at' property.
-
-    Args:
-        pattern: regex pattern to match.
-
-
-    Example:
-        >>> import pytreeclass as pytc
-        >>> class Tree(pytc.TreeClass):
-        ...     weight_1: float = 1.0
-        ...     weight_2: float = 2.0
-        ...     weight_3: float = 3.0
-        ...     bias: float = 0.0
-        >>> tree = Tree()
-        >>> tree.at[pytc.RegexKey(r"weight_.*")].set(100.0)  # set all weights to 100.0
-        Tree(weight_1=100.0, weight_2=100.0, weight_3=100.0, bias=0.0)
-    """
-
-    pattern: str
-
-    def __eq__(self, other: Any) -> bool:
-        """Return True if other fully matches the regex pattern."""
-        if not isinstance(other, str):
-            return False
-        return re.fullmatch(self.pattern, other) is not None
-
-
-WhereAtomType = (int, str, type(...), RegexKey)
-WhereType = Union[int, str, RegexKey, PyTree, EllipsisType]
+@dc.dataclass(frozen=True)
+class NamedSequenceKey(jtu.GetAttrKey, jtu.SequenceKey):
+    # inherit from both `jtu.GetAttrKey` and `jtu.SequenceKey`
+    # in case the user perform isinstance check to unpack the name/index
+    # `TreeClass` is modeled as a `NamedTuple`` with both `name` and `idx` identifiers
+    def __str__(self):
+        return f".{self.name}"
 
 
 def tree_hash(*trees: PyTree) -> int:
     leaves, treedef = jtu.tree_flatten(trees)
     return hash((*leaves, treedef))
 
 
@@ -114,30 +80,28 @@
 
     Note:
         trees are compared using their leaves and treedefs.
 
     Note:
         Under `jit` the return type is boolean `jax.Array` instead of `bool`.
     """
-
     tree0, *rest = trees
     leaves0, treedef0 = jtu.tree_flatten(tree0)
     verdict = True
 
     for tree in rest:
         leaves, treedef = jtu.tree_flatten(tree)
         if (treedef != treedef0) or verdict is False:
             return False
         verdict = ft.reduce(op.and_, map(_is_leaf_rhs_equal, leaves0, leaves), verdict)
     return verdict
 
 
 class Partial:
-    """
-    jaxable Partial function with support for positional partial application.
+    """jaxable Partial function with support for positional partial application.
 
     Example:
         >>> import pytreeclass as pytc
         >>> def f(a, b, c):
         ...     print(f"a: {a}, b: {b}, c: {c}")
         ...     return a + b + c
 
@@ -153,25 +117,20 @@
         a: 1, b: 2, c: 3
         6
 
     Note:
         - The `...` is used to indicate a placeholder for positional arguments.
         - See: https://stackoverflow.com/a/7811270
         - `Partial` is used internally by `bcmap` which maps a function over pytrees
-            leaves with automatic broadcasting for scalar arguments.
+          leaves with automatic broadcasting for scalar arguments.
     """
 
-    __slots__ = ("func", "args", "kwargs", "__weakref__")  # type: ignore
+    __slots__ = ["func", "args", "kwargs", "__weakref__"]  # type: ignore
 
-    def __init__(
-        self,
-        func: Callable[..., Any],
-        *args: Any,
-        **kwargs: Any,
-    ):
+    def __init__(self, func: Callable[..., Any], *args: Any, **kwargs: Any):
         """Initialize a `Partial` function.
 
         Args:
             func: The function to be partially applied.
             args: Positional arguments to be partially applied. use `...` as a
                 placeholder for positional arguments.
             kwargs: Keyword arguments to be partially applied.
@@ -198,22 +157,16 @@
 jtu.register_pytree_node(
     nodetype=Partial,
     flatten_func=lambda x: ((x.func, x.args, x.kwargs), None),
     unflatten_func=lambda _, xs: Partial(*xs),
 )
 
 
-def bcmap(
-    func: Callable,
-    *,
-    is_leaf: IsLeafType = None,
-) -> Callable:
-    """
-    (map)s a function over pytrees leaves with automatic (b)road(c)asting
-    for scalar arguments
+def bcmap(func: Callable, *, is_leaf: IsLeafType = None) -> Callable:
+    """Map a function over pytree leaves with automatic broadcasting for scalar arguments.
 
     Args:
         func: the function to be mapped over the pytree
         is_leaf: a predicate function that returns True if the node is a leaf
 
     Example:
         >>> import jax
@@ -306,186 +259,90 @@
     name = getattr(func, "__name__", func)
 
     docs = f"Broadcasted version of {name}\n{func.__doc__}"
     wrapper.__doc__ = docs
     return wrapper
 
 
-def _unary_op(func):
+def uop(func):
     def wrapper(self):
         return jtu.tree_map(func, self)
 
     return ft.wraps(func)(wrapper)
 
 
-def _binary_op(func):
+def bop(func):
     def wrapper(leaf, rhs=None):
         if isinstance(rhs, type(leaf)):
             return jtu.tree_map(func, leaf, rhs)
         return jtu.tree_map(lambda x: func(x, rhs), leaf)
 
     return ft.wraps(func)(wrapper)
 
 
-def _swop(func):
+def swop(func):
     # swaping the arguments of a two-arg function
     return ft.wraps(func)(lambda leaf, rhs: func(rhs, leaf))
 
 
 def _leafwise_transform(klass: type[T]) -> type[T]:
     # add leafwise transform methods to the class
     # that enable the user to apply a function to
     # all the leaves of the tree
     for key, method in (
-        ("__abs__", _unary_op(abs)),
-        ("__add__", _binary_op(op.add)),
-        ("__and__", _binary_op(op.and_)),
-        ("__ceil__", _unary_op(ceil)),
-        ("__divmod__", _binary_op(divmod)),
-        ("__eq__", _binary_op(op.eq)),
-        ("__floor__", _unary_op(floor)),
-        ("__floordiv__", _binary_op(op.floordiv)),
-        ("__ge__", _binary_op(op.ge)),
-        ("__gt__", _binary_op(op.gt)),
-        ("__invert__", _unary_op(op.invert)),
-        ("__le__", _binary_op(op.le)),
-        ("__lshift__", _binary_op(op.lshift)),
-        ("__lt__", _binary_op(op.lt)),
-        ("__matmul__", _binary_op(op.matmul)),
-        ("__mod__", _binary_op(op.mod)),
-        ("__mul__", _binary_op(op.mul)),
-        ("__ne__", _binary_op(op.ne)),
-        ("__neg__", _unary_op(op.neg)),
-        ("__or__", _binary_op(op.or_)),
-        ("__pos__", _unary_op(op.pos)),
-        ("__pow__", _binary_op(op.pow)),
-        ("__radd__", _binary_op(_swop(op.add))),
-        ("__rand__", _binary_op(_swop(op.and_))),
-        ("__rdivmod__", _binary_op(_swop(divmod))),
-        ("__rfloordiv__", _binary_op(_swop(op.floordiv))),
-        ("__rlshift__", _binary_op(_swop(op.lshift))),
-        ("__rmatmul__", _binary_op(_swop(op.matmul))),
-        ("__rmod__", _binary_op(_swop(op.mod))),
-        ("__rmul__", _binary_op(_swop(op.mul))),
-        ("__ror__", _binary_op(_swop(op.or_))),
-        ("__round__", _binary_op(round)),
-        ("__rpow__", _binary_op(_swop(op.pow))),
-        ("__rrshift__", _binary_op(_swop(op.rshift))),
-        ("__rshift__", _binary_op(op.rshift)),
-        ("__rsub__", _binary_op(_swop(op.sub))),
-        ("__rtruediv__", _binary_op(_swop(op.truediv))),
-        ("__rxor__", _binary_op(_swop(op.xor))),
-        ("__sub__", _binary_op(op.sub)),
-        ("__truediv__", _binary_op(op.truediv)),
-        ("__trunc__", _unary_op(trunc)),
-        ("__xor__", _binary_op(op.xor)),
+        ("__abs__", uop(abs)),
+        ("__add__", bop(op.add)),
+        ("__and__", bop(op.and_)),
+        ("__ceil__", uop(ceil)),
+        ("__divmod__", bop(divmod)),
+        ("__eq__", bop(op.eq)),
+        ("__floor__", uop(floor)),
+        ("__floordiv__", bop(op.floordiv)),
+        ("__ge__", bop(op.ge)),
+        ("__gt__", bop(op.gt)),
+        ("__invert__", uop(op.invert)),
+        ("__le__", bop(op.le)),
+        ("__lshift__", bop(op.lshift)),
+        ("__lt__", bop(op.lt)),
+        ("__matmul__", bop(op.matmul)),
+        ("__mod__", bop(op.mod)),
+        ("__mul__", bop(op.mul)),
+        ("__ne__", bop(op.ne)),
+        ("__neg__", uop(op.neg)),
+        ("__or__", bop(op.or_)),
+        ("__pos__", uop(op.pos)),
+        ("__pow__", bop(op.pow)),
+        ("__radd__", bop(swop(op.add))),
+        ("__rand__", bop(swop(op.and_))),
+        ("__rdivmod__", bop(swop(divmod))),
+        ("__rfloordiv__", bop(swop(op.floordiv))),
+        ("__rlshift__", bop(swop(op.lshift))),
+        ("__rmatmul__", bop(swop(op.matmul))),
+        ("__rmod__", bop(swop(op.mod))),
+        ("__rmul__", bop(swop(op.mul))),
+        ("__ror__", bop(swop(op.or_))),
+        ("__round__", bop(round)),
+        ("__rpow__", bop(swop(op.pow))),
+        ("__rrshift__", bop(swop(op.rshift))),
+        ("__rshift__", bop(op.rshift)),
+        ("__rsub__", bop(swop(op.sub))),
+        ("__rtruediv__", bop(swop(op.truediv))),
+        ("__rxor__", bop(swop(op.xor))),
+        ("__sub__", bop(op.sub)),
+        ("__truediv__", bop(op.truediv)),
+        ("__trunc__", uop(trunc)),
+        ("__xor__", bop(op.xor)),
     ):
         if key not in vars(klass):
             # do not override any user defined methods
             # this behavior similar is to `dataclasses.dataclass`
             setattr(klass, key, method)
     return klass
 
 
-@dc.dataclass(frozen=True)
-class NamedSequenceKey(jtu.GetAttrKey, jtu.SequenceKey):
-    # inherit from both `jtu.GetAttrKey` and `jtu.SequenceKey`
-    # in case the user perform isinstance check to unpack the name/index
-    # `TreeClass` is modeled as a `NamedTuple`` with both `name` and `idx` identifiers
-    def __str__(self):
-        return f".{self.name}"
-
-
-# indexing matching registry
-# define rule for indexing matching through `at` property
-# for example, `jax` internals uses `jtu.GetAttrKey` to index an attribute,
-# however its not ergonomic to use `tree.at[jtu.GetAttrKey("attr")]`
-# to index an attribute instead `tree.at['attr']` is more ergonomic
-match_registry: dict[type, Callable] = defaultdict(lambda entry: (entry,))  # type: ignore
-match_registry[jtu.GetAttrKey] = lambda entry: (entry.name,)
-match_registry[jtu.SequenceKey] = lambda entry: (entry.idx,)
-match_registry[NamedSequenceKey] = lambda entry: (entry.idx, entry.name)
-match_registry[jtu.DictKey] = lambda entry: (entry.key,)
-match_registry[jtu.FlattenedIndexKey] = lambda entry: (entry.key,)
-
-
-def _generate_path_mask(
-    tree: PyTree,
-    where: tuple[WhereType, ...],
-    is_leaf: IsLeafType = None,
-) -> PyTree:
-    # generate a mask for `where` path in `tree`
-    # where path is a tuple of indices or keys, for example
-    # where=("a",) wil set all leaves of `tree` with key "a" to True and
-    # all other leaves to False
-    match = False
-
-    def map_func(path, _: Any):
-        if len(where) > len(path):
-            # path is shorter than `where` path. for example
-            # where=("a", "b") and the current path is ("a",) then
-            # the current path is not a match
-            return False
-        for wi, ki in zip(where, path):
-            if not any(wi == ei for ei in (..., *match_registry[type(ki)](ki))):
-                # use equality instead of `in` to trigger regex matching
-                # for the overloaded `RegexKey` __eq__ method.
-                return False
-
-        nonlocal match
-
-        return (match := True)
-
-    mask = jtu.tree_map_with_path(map_func, tree, is_leaf=is_leaf)
-
-    if not match:
-        raise LookupError(f"No leaf match is found for {where=}.")
-
-    return mask
-
-
-def _combine_maybe_bool_masks(*masks: PyTree) -> PyTree:
-    # combine boolean masks with `&` operator if all masks are boolean
-    # otherwise raise an error
-    def check_and_return_bool_leaf(leaf: Any) -> bool:
-        if hasattr(leaf, "dtype"):
-            if leaf.dtype == "bool":
-                return leaf
-            raise TypeError(f"Expected boolean array mask, got {leaf=}")
-
-        if isinstance(leaf, bool):
-            return leaf
-        raise TypeError(f"Expected boolean mask, got {leaf=}")
-
-    def map_func(*leaves):
-        verdict = True
-        for leaf in leaves:
-            verdict &= check_and_return_bool_leaf(leaf)
-        return verdict
-
-    return jtu.tree_map(map_func, *masks)
-
-
-def _resolve_where(
-    tree: PyTree,
-    where: tuple[WhereType, ...],  # type: ignore
-    is_leaf: IsLeafType = None,
-):
-    mask = None
-
-    if path := tuple(i for i in where if isinstance(i, WhereAtomType)):
-        mask = _generate_path_mask(tree, path, is_leaf=is_leaf)
-
-    if maybe_bool_masks := tuple(i for i in where if isinstance(i, type(tree))):
-        all_masks = (mask, *maybe_bool_masks) if mask else maybe_bool_masks
-        mask = _combine_maybe_bool_masks(*all_masks)
-
-    return mask
-
-
 def flatten_one_trace_level(
     trace: TraceType,
     tree: PyTree,
     is_leaf: IsLeafType,
     is_trace_leaf: Callable[[TraceType], bool] | None,
 ):
     # the code style of `tree_{...} is heavilty influenced by `jax.tree_util`
@@ -575,15 +432,16 @@
     func: Callable[..., Any],
     tree: Any,
     *rest: Any,
     is_leaf: IsLeafType = None,
 ) -> Any:
     # the code style of `tree_{...} is heavilty influenced by `jax.tree_util`
     # https://github.com/google/jax/blob/main/jax/_src/tree_util.py
-    """
+    """Map a function over a pytree, with trace and type path.
+
     Similar to `jax.tree_util.tree_map_with_path` that accept a function
     that takes a two-item tuple for key path and type path.
 
     Args:
         func: A function that takes a trace and a leaf and returns a new leaf.
         tree: The tree to be mapped over.
         rest: Additional trees to be mapped over.
@@ -619,15 +477,15 @@
     traces_leaves = list(zip(*traces_leaves))
     traces_leaves += [treedef.flatten_up_to(r) for r in rest]
     return treedef.unflatten(func(*xs) for xs in zip(*traces_leaves))
 
 
 class Node:
     # mainly used for visualization
-    __slots__ = ("data", "parent", "children", "__weakref__")
+    __slots__ = ["data", "parent", "children", "__weakref__"]
 
     def __init__(
         self,
         data: tuple[TraceEntry, Any],
         parent: Node | None = None,
     ):
         self.data = data
@@ -667,15 +525,15 @@
     traces_leaves = tree_leaves_with_trace(
         tree,
         is_leaf=is_leaf,
         is_trace_leaf=is_trace_leaf,
     )
 
     ti = (None, type(tree))
-    vi = tree if len(traces_leaves) == 1 else None
+    vi = tree
     root = Node(data=(ti, vi))
 
     for trace, leaf in traces_leaves:
         keys, types = trace
         cur = root
         for i, ti in enumerate(zip(keys, types)):
             if ti in cur:
```

### Comparing `pytreeclass-0.3.8/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.4.0/pytreeclass.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 LICENSE
 README.md
-setup.py
-docs/conf.py
+pyproject.toml
 pytreeclass/__init__.py
 pytreeclass.egg-info/PKG-INFO
 pytreeclass.egg-info/SOURCES.txt
 pytreeclass.egg-info/dependency_links.txt
-pytreeclass.egg-info/not-zip-safe
 pytreeclass.egg-info/requires.txt
 pytreeclass.egg-info/top_level.txt
 pytreeclass/_src/__init__.py
 pytreeclass/_src/code_build.py
 pytreeclass/_src/tree_base.py
+pytreeclass/_src/tree_index.py
+pytreeclass/_src/tree_mask.py
 pytreeclass/_src/tree_pprint.py
 pytreeclass/_src/tree_util.py
-tests/__init__.py
 tests/test_indexing.py
 tests/test_nn.py
 tests/test_tree_freeze.py
 tests/test_tree_operator.py
 tests/test_tree_pprint.py
 tests/test_tree_viz_util.py
 tests/test_treeclass.py
```

### Comparing `pytreeclass-0.3.8/tests/test_indexing.py` & `pytreeclass-0.4.0/tests/test_indexing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,26 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 
+import re
 from collections import namedtuple
-from typing import Any
+from typing import Any, NamedTuple
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 
@@ -61,15 +76,15 @@
     C = level2(
         d=level1(a=None, b=None, c=jnp.array([], dtype=int)),
         e=level1(a=None, b=None, c=jnp.array([], dtype=int)),
     )
 
     assert pytc.is_tree_equal(B, C)
 
-    with pytest.raises(TypeError):
+    with pytest.raises(NotImplementedError):
         B = A.at[A].get()
 
     # with pytest.raises(NotImplementedError):
     #     B = A.at[0].get()
 
 
 def test_getter_by_param():
@@ -120,15 +135,15 @@
         e=level1(a=2, b=20, c=jnp.array([100, 100, 100, 100, 100])),
     )
 
     assert pytc.is_tree_equal(B, C)
 
     A = Tree(10, 20, 30, jnp.array([1, 2, 3, 4, 5]), ("A"))
 
-    with pytest.raises(TypeError):
+    with pytest.raises(NotImplementedError):
         B = A.at[A].set(0)
 
     # with pytest.raises(NotImplementedError):
     #     B = A.at[0].set(0)
 
     class L0(TreeClass, leafwise=True):
         a: int = 1
@@ -183,15 +198,15 @@
     rhs = init.at[init == init].apply(lambda x: (x + 1) * 10)
     assert pytc.is_tree_equal(lhs, rhs)
 
     lhs = A(20, 30, jnp.array([20, 30, 40, 50, 60]))
     rhs = init.at[...].apply(lambda x: (x + 1) * 10)
     assert pytc.is_tree_equal(lhs, rhs)
 
-    with pytest.raises(TypeError):
+    with pytest.raises(NotImplementedError):
         init.at[init].apply(lambda x: (x + 1) * 10)
 
     class L0(TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
         c: int = 3
 
@@ -291,15 +306,15 @@
 
     init = B(1, 2, jnp.array([1, 2, 3, 4, 5]), (10, 20, 30))
 
     lhs = 2 + 2 + 3 + 4 + 5 + 10 + 20 + 30
     rhs = init.at[init > 1].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
     assert lhs == rhs
 
-    with pytest.raises(TypeError):
+    with pytest.raises(NotImplementedError):
         init.at[init].reduce(lambda x, y: x + jnp.sum(y), initializer=0)
 
     class Tree(TreeClass, leafwise=True):
         a: tuple[int]
 
     lhs = Tree((1, 2, 3)).at["a"].reduce(lambda x, y: x + y, initializer=0)
     assert lhs == 6
@@ -342,15 +357,15 @@
         ),
         1.3969219,
     )
     npt.assert_allclose(
         tree.at[tree > 0].reduce(lambda x, y: x + jnp.sum(y), initializer=0), 10.6970625
     )
     npt.assert_allclose(
-        tree.at[tree > 0].reduce(lambda x, y: x * jnp.product(y), initializer=1),
+        tree.at[tree > 0].reduce(lambda x, y: x * jnp.prod(y), initializer=1),
         1.8088213,
     )
 
 
 def test_is_leaf():
     class Tree(TreeClass, leafwise=True):
         a: int
@@ -602,17 +617,17 @@
 def test_repr_str():
     class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: int = 2
 
     t = Tree()
 
-    assert repr(t.at["a"]) == "AtIndexer(tree=Tree(a=1, b=2), where=('a',))"
-    assert str(t.at["a"]) == "AtIndexer(tree=Tree(a=1, b=2), where=('a',))"
-    assert repr(t.at[...]) == "AtIndexer(tree=Tree(a=1, b=2), where=(Ellipsis,))"
+    assert repr(t.at["a"]) == "TreeClassIndexer(tree=Tree(a=1, b=2), where=('a',))"
+    assert str(t.at["a"]) == "TreeClassIndexer(tree=Tree(a=1, b=2), where=('a',))"
+    assert repr(t.at[...]) == "TreeClassIndexer(tree=Tree(a=1, b=2), where=(Ellipsis,))"
 
 
 def test_not_equal():
     class Tree(TreeClass, leafwise=True):
         a: int = 1
         b: float = 1.0
 
@@ -683,28 +698,97 @@
     assert jtu.tree_leaves(tree.at["a"].at[1].at["b"].get())[0] == Dict({"c": 1})
     assert jtu.tree_leaves(tree.at[0].at[1].at["b"].get())[0] == Dict({"c": 1})
 
 
 def test_construct_tree():
     tree = construct_tree([1, 2, [3, 4]])
 
-    assert repr(tree) == "Node(data=((None, <class 'list'>), None))"
+    assert repr(tree) == "Node(data=((None, <class 'list'>), [1, 2, [3, 4]]))"
 
     with pytest.raises(TypeError):
         tree.add_child("a")
 
 
 def test_regexkey():
     class Tree(pytc.TreeClass):
         weight_1: float = 1.0
         weight_2: float = 2.0
         weight_3: float = 3.0
         bias: float = 0.0
 
     tree = Tree()
 
-    tree = tree.at[pytc.RegexKey(r"weight_.*")].set(100.0)
+    tree = tree.at[re.compile(r"weight_.*")].set(100.0)
     # Tree(weight_1=100.0, weight_2=100.0, weight_3=100.0, bias=0.0)
     assert jtu.tree_leaves(tree) == [100.0, 100.0, 100.0, 0.0]
+    tree = pytc.AtIndexer({"a": 1, "b": 2}).at[re.compile(r"a")].set(100.0)
+    assert tree == {"a": 100.0, "b": 2}
+
+
+def test_custom_key():
+    class NameTypeContainer(NamedTuple):
+        name: str
+        type: type
+
+    @jax.tree_util.register_pytree_with_keys_class
+    class Tree:
+        def __init__(self, a, b) -> None:
+            self.a = a
+            self.b = b
+
+        def tree_flatten_with_keys(self):
+            ak = (NameTypeContainer("a", type(self.a)), self.a)
+            bk = (NameTypeContainer("b", type(self.b)), self.b)
+            return (ak, bk), None
+
+        @classmethod
+        def tree_unflatten(cls, aux_data, children):
+            return cls(*children)
+
+        @property
+        def at(self):
+            return pytc.AtIndexer(self)
+
+    tree = Tree(1, 2)
+
+    class MatchNameType(pytc.BaseKey):
+        def __init__(self, name, type):
+            self.name = name
+            self.type = type
+
+        def __eq__(self, other):
+            if isinstance(other, NameTypeContainer):
+                return other == (self.name, self.type)
+            return False
+
+    assert jax.tree_util.tree_leaves(tree.at[MatchNameType("a", int)].get()) == [1]
+
+
+def test_multi_key():
+    class Tree(pytc.TreeClass):
+        a: int = 1
+        b: int = 2
+        c: int = 3
+
+    tree = Tree()
+    assert pytc.is_tree_equal(
+        tree.at["a"].set(100).at["b"].set(100),
+        tree.at["a", "b"].set(100),
+    )
+
+
+def test_scan():
+    class Tree(pytc.TreeClass):
+        a: int = 1
+        b: int = 2
+        c: int = 3
+        d: jax.Array = jnp.array([4, 5])
+
+    tree = Tree()
+
+    def func_with_state(x, state):
+        return x + 1, state + 1
+
+    tree, state = tree.at["a", "b", "d"].scan(func_with_state, state=1)
 
-    assert pytc.RegexKey(r"w.*") == "woof"
-    assert pytc.RegexKey(r"w.*") != "meow"
+    assert pytc.is_tree_equal(tree, Tree(a=2, b=3, c=3, d=jnp.array([5, 6])))
+    assert state == 4
```

### Comparing `pytreeclass-0.3.8/tests/test_nn.py` & `pytreeclass-0.4.0/tests/test_nn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,79 @@
-from typing import Callable, Sequence
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 import jax.tree_util as jtu
 import numpy as np
+import optax
 import pytest
 
 import pytreeclass as pytc
 
 
 def test_nn():
-    class Linear(pytc.TreeClass, leafwise=True):
-        weight: jax.Array
-        bias: jax.Array
-
+    class Linear(pytc.TreeClass):
         def __init__(self, key, in_dim, out_dim):
             self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
-    class StackedLinear(pytc.TreeClass, leafwise=True):
-        layers: Sequence[Linear]
-
+    class StackedLinear(pytc.TreeClass):
         def __init__(self, key, layers):
             keys = jr.split(key, len(layers) - 1)
 
-            self.layers = []
+            self.layers = ()
 
             for ki, in_dim, out_dim in zip(keys, layers[:-1], layers[1:]):
-                self.layers += [Linear(ki, in_dim, out_dim)]
+                self.layers += (Linear(ki, in_dim, out_dim),)
 
         def __call__(self, x):
-            for layer in self.layers[:-1]:
+            *layers, last = self.layers
+            for layer in layers:
                 x = layer(x)
                 x = jax.nn.tanh(x)
-
-            return self.layers[-1](x)
+            return last(x)
 
     x = jnp.linspace(0, 1, 100)[:, None]
     y = x**3 + jr.uniform(jr.PRNGKey(0), (100, 1)) * 0.01
 
-    NN = StackedLinear(layers=[1, 128, 128, 1], key=jr.PRNGKey(0))
+    nn = StackedLinear(layers=[1, 128, 128, 1], key=jr.PRNGKey(0))
 
-    def loss_func(NN, x, y):
-        return jnp.mean((NN(x) - y) ** 2)
+    def loss_func(nn, x, y):
+        return jnp.mean((nn(x) - y) ** 2)
 
     @jax.jit
-    def update(NN, x, y):
-        value, grads = jax.value_and_grad(loss_func)(NN, x, y)
-        return value, jax.tree_map(lambda x, y: x - 1e-3 * y, NN, grads)
+    def update(nn, x, y):
+        value, grads = jax.value_and_grad(loss_func)(nn, x, y)
+        return value, jax.tree_map(lambda x, y: x - 1e-3 * y, nn, grads)
 
     for _ in range(1, 2001):
-        value, NN = update(NN, x, y)
+        value, nn = update(nn, x, y)
 
     np.testing.assert_allclose(value, jnp.array(0.00103019), atol=1e-5)
 
 
 def test_nn_with_func_input():
-    class Linear(pytc.TreeClass, leafwise=True):
-        weight: jax.Array
-        bias: jax.Array
-        act_func: Callable
-
+    class Linear(pytc.TreeClass):
         def __init__(self, key, in_dim, out_dim, act_func):
             self.act_func = act_func
             self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
 
         def __call__(self, x):
             return self.act_func(x @ self.weight + self.bias)
@@ -77,18 +82,15 @@
     x = jnp.linspace(0, 1, 100)[:, None]
     # y = x**3 + jr.uniform(jr.PRNGKey(0), (100, 1)) * 0.01
     layer(x)
     return True
 
 
 def test_compact_nn():
-    class Linear(pytc.TreeClass, leafwise=True):
-        weight: jax.Array
-        bias: jax.Array
-
+    class Linear(pytc.TreeClass):
         def __init__(self, key, in_dim, out_dim):
             self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
@@ -108,59 +110,47 @@
             x = self.l3(x)
 
             return x
 
     x = jnp.linspace(0, 1, 100)[:, None]
     y = x**3 + jr.uniform(jr.PRNGKey(0), (100, 1)) * 0.01
 
-    NN = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jr.PRNGKey(0))
+    nn = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jr.PRNGKey(0))
 
-    def loss_func(NN, x, y):
-        return jnp.mean((NN(x) - y) ** 2)
+    def loss_func(nn, x, y):
+        return jnp.mean((nn(x) - y) ** 2)
 
     @jax.jit
-    def update(NN, x, y):
-        value, grads = jax.value_and_grad(loss_func)(NN, x, y)
+    def update(nn, x, y):
+        value, grads = jax.value_and_grad(loss_func)(nn, x, y)
 
-        # no need to use `jax.tree_map` to update the NN
-        #  as it NN is wrapped by @ft.partial(pytc.treeclass, leafwise=True)
-        return value, NN - 1e-3 * grads
+        # no need to use `jax.tree_map` to update the nn
+        #  as it nn is wrapped by @ft.partial(pytc.treeclass, leafwise=True)
+        return value, nn - 1e-3 * grads
 
     for _ in range(1, 10_001):
-        value, NN = update(NN, x, y)
+        value, nn = update(nn, x, y)
 
     np.testing.assert_allclose(value, jnp.array(0.0031012), atol=1e-5)
 
 
 def test_freeze_nondiff():
     class Linear(pytc.TreeClass, leafwise=True):
-        weight: jax.Array
-        bias: jax.Array
-        count: int
-        use_bias: bool
-
         def __init__(self, key, in_dim, out_dim):
             self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
             self.bias = jnp.ones((1, out_dim))
             self.use_bias = True
             self.count = 0
 
         def __call__(self, x):
             return x @ self.weight + self.bias
 
     class StackedLinear(pytc.TreeClass, leafwise=True):
-        name: str
-        # exact_array: jax.Array
-        # bool_array: jax.Array
-
         def __init__(self, key, in_dim, out_dim, hidden_dim):
             self.name = "stack"
-            # self.exact_array = jnp.array([1, 2, 3])
-            # self.bool_array = jnp.array([True, True])
-
             keys = jr.split(key, 3)
 
             self.l1 = Linear(key=keys[0], in_dim=in_dim, out_dim=hidden_dim)
             self.l2 = Linear(key=keys[1], in_dim=hidden_dim, out_dim=hidden_dim)
             self.l3 = Linear(key=keys[2], in_dim=hidden_dim, out_dim=out_dim)
 
         def __call__(self, x):
@@ -171,47 +161,82 @@
             x = self.l3(x)
 
             return x
 
     x = jnp.linspace(0, 1, 100)[:, None]
     y = x**3 + jr.uniform(jr.PRNGKey(0), (100, 1)) * 0.01
 
-    NN = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jr.PRNGKey(0))
+    nn = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jr.PRNGKey(0))
 
-    def loss_func(NN, x, y):
-        return jnp.mean((NN(x) - y) ** 2)
+    def loss_func(nn, x, y):
+        return jnp.mean((nn(x) - y) ** 2)
 
     with pytest.raises(TypeError):
 
         @jax.jit
-        def update(NN, x, y):
-            value, grads = jax.value_and_grad(loss_func)(NN, x, y)
-            return value, NN - 1e-3 * grads
+        def update(nn, x, y):
+            value, grads = jax.value_and_grad(loss_func)(nn, x, y)
+            return value, nn - 1e-3 * grads
 
         for _ in range(1, 10_001):
-            value, NN = update(NN, x, y)
+            value, nn = update(nn, x, y)
 
     @jax.jit
-    def update(NN, x, y):
-        value, grads = jax.value_and_grad(loss_func)(NN, x, y)
-        return value, NN - 1e-3 * grads
+    def update(nn, x, y):
+        value, grads = jax.value_and_grad(loss_func)(nn, x, y)
+        return value, nn - 1e-3 * grads
 
-    mask = jtu.tree_map(pytc.is_nondiff, NN)
-    freezeed_NN = NN.at[mask].apply(pytc.freeze)
+    mask = jtu.tree_map(pytc.is_nondiff, nn)
+    freezeed_nn = nn.at[mask].apply(pytc.freeze)
 
     for _ in range(1, 10_001):
-        value, freezeed_NN = update(freezeed_NN, x, y)
+        value, freezeed_nn = update(freezeed_nn, x, y)
 
     np.testing.assert_allclose(value, jnp.array(0.0031012), atol=1e-5)
 
-    X = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jr.PRNGKey(0))
+    nn = StackedLinear(in_dim=1, out_dim=1, hidden_dim=10, key=jr.PRNGKey(0))
 
-    frozen_ = jtu.tree_map(pytc.freeze, X)
+    frozen_ = jtu.tree_map(pytc.freeze, nn)
     unfrozen_ = jtu.tree_map(pytc.unfreeze, frozen_, is_leaf=pytc.is_frozen)
-    assert jtu.tree_leaves(X) == jtu.tree_leaves(unfrozen_)
+    assert jtu.tree_leaves(nn) == jtu.tree_leaves(unfrozen_)
+
+    class Linear(pytc.TreeClass):
+        def __init__(self, key, in_dim, out_dim):
+            self.weight = jr.normal(key, shape=(in_dim, out_dim)) * jnp.sqrt(2 / in_dim)
+            self.bias = jnp.ones((1, out_dim))
+
+        def __call__(self, x):
+            return x @ self.weight + self.bias
+
+    nn = Linear(jr.PRNGKey(0), 1, 1)
+    nn_ = nn
+    nn = nn.at["weight"].apply(pytc.freeze)
+
+    optim = optax.sgd(1e-3)
+    optim_state = optim.init(nn)
+
+    x = jnp.linspace(0, 1, 100)[:, None]
+    y = x**3 + jr.uniform(jr.PRNGKey(0), (100, 1)) * 0.01
+
+    def loss_func(nn, x, y):
+        nn = pytc.tree_unmask(nn)
+        return jnp.mean((nn(x) - y) ** 2)
+
+    @jax.jit
+    def train_step(nn, optim_state, x, y):
+        value, dnn = jax.value_and_grad(loss_func)(nn, x, y)
+        dnn, optim_state = optim.update(dnn, optim_state)
+        nn = optax.apply_updates(nn, dnn)
+        return nn, optim_state, value
+
+    for _ in range(1, 100):
+        nn, optim_state, value = train_step(nn, optim_state, x, y)
+
+    nn = pytc.tree_unmask(nn)
+    assert nn_.weight == nn.weight, nn
 
 
 @pytest.mark.benchmark
 def test_nn_benchmark(benchmark):
     benchmark(test_nn)
```

### Comparing `pytreeclass-0.3.8/tests/test_tree_freeze.py` & `pytreeclass-0.4.0/tests/test_tree_freeze.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import copy
 from typing import Any, Callable
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import pytest
 
@@ -240,15 +255,15 @@
     assert jtu.tree_leaves(t) == [10, 20, 30, 1, 2, 3, 3]
 
 
 def test_non_dataclass_input_to_freeze():
     assert jtu.tree_leaves(pytc.freeze(1)) == []
 
 
-def test_tree_freeze():
+def test_tree_mask():
     class l0(pytc.TreeClass, leafwise=True):
         x: int = 2
         y: int = 3
 
     class l1(pytc.TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
@@ -265,15 +280,15 @@
 
     assert jtu.tree_leaves(tree.at["a"].apply(pytc.freeze)) == [2, 3]
     assert jtu.tree_leaves(tree.at["b"].apply(pytc.freeze)) == [1]
     assert jtu.tree_leaves(tree.at["b"].at["x"].apply(pytc.freeze)) == [1, 3]
     assert jtu.tree_leaves(tree.at["b"].at["y"].apply(pytc.freeze)) == [1, 2]
 
 
-def test_tree_unfreeze():
+def test_tree_unmask():
     class l0(pytc.TreeClass, leafwise=True):
         x: int = 2
         y: int = 3
 
     class l1(pytc.TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
@@ -294,15 +309,15 @@
     unfrozen_tree = frozen_tree.at["a"].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)  # fmt: skip
     assert jtu.tree_leaves(unfrozen_tree) == [1]
 
     unfrozen_tree = frozen_tree.at["b"].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)  # fmt: skip
     assert jtu.tree_leaves(unfrozen_tree) == [2, 3]
 
 
-def test_tree_freeze_unfreeze():
+def test_tree_mask_unfreeze():
     class l0(pytc.TreeClass, leafwise=True):
         x: int = 2
         y: int = 3
 
     class l1(pytc.TreeClass, leafwise=True):
         a: int = 1
         b: l0 = l0()
@@ -379,7 +394,35 @@
 
     wrapped = pytc.freeze(1)
 
     with pytest.raises(AttributeError):
         delattr(wrapped, "__wrapped__")
 
     assert wrapped != 1
+
+
+def test_tree_mask_tree_unmask():
+    tree = [1, 2, 3.0]
+    assert jtu.tree_leaves(pytc.tree_mask(tree)) == [3.0]
+    assert jtu.tree_leaves(pytc.tree_unmask(pytc.tree_mask(tree))) == [1, 2, 3.0]
+
+    mask_func = lambda x: x < 2
+    assert jtu.tree_leaves(pytc.tree_mask(tree, mask_func)) == [2, 3.0]
+
+    frozen_array = pytc.tree_mask(jnp.ones((5, 5)), mask=lambda _: True)
+
+    assert frozen_array == frozen_array
+    assert not (frozen_array == pytc.freeze(jnp.ones((5, 6))))
+    assert not (frozen_array == pytc.freeze(jnp.ones((5, 5)).astype(jnp.uint8)))
+    assert hash(frozen_array) == hash(frozen_array)
+
+    assert pytc.freeze(pytc.freeze(1)) == pytc.freeze(1)
+
+    assert pytc.tree_mask({"a": 1}, mask={"a": True}) == {"a": pytc.freeze(1)}
+
+    with pytest.raises(ValueError):
+        pytc.tree_mask({"a": 1}, mask=1.0)
+
+    assert copy.copy(pytc.freeze(1)) == pytc.freeze(1)
+
+    with pytest.raises(NotImplementedError):
+        pytc.freeze(1) + 1
```

### Comparing `pytreeclass-0.3.8/tests/test_tree_operator.py` & `pytreeclass-0.4.0/tests/test_tree_operator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 
 import math
 
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import pytest
```

### Comparing `pytreeclass-0.3.8/tests/test_tree_pprint.py` & `pytreeclass-0.4.0/tests/test_tree_pprint.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,37 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 
 import dataclasses as dc
+import re
 from collections import namedtuple
 
 # import jax
 import jax.tree_util as jtu
 import pytest
 from jax import numpy as jnp
 
 import pytreeclass as pytc
 from pytreeclass import (
     TreeClass,
     tree_diagram,
-    tree_indent,
+    tree_graph,
     tree_mermaid,
     tree_repr,
     tree_repr_with_trace,
     tree_str,
     tree_summary,
 )
 
@@ -51,21 +66,21 @@
 r1 = Repr1()
 
 
 def test_repr():
     assert (
         tree_repr(r1)
         # trunk-ignore(flake8/E501)
-        == "Repr1(\n  a=1, \n  b='string', \n  c=1.0, \n  d='aaaaa', \n  e=[10, 10, 10, 10, 10], \n  f={1, 2, 3}, \n  g={\n    a:'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa', \n    b:'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb', \n    c:f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n  }, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=a(b=1, c=2), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[], \n  o=c64[2]\n)"
+        == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[10, 10, 10, 10, 10], \n  f={1, 2, 3}, \n  g={\n    a:aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa, \n    b:bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb, \n    c:f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n  }, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=a(b=1, c=2), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[], \n  o=c64[2]\n)"
     )
 
     assert (
         tree_repr(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == "Repr1(\n  a=1, \n  b='string', \n  c=1.0, \n  d='aaaaa', \n  e=[...], \n  f={...}, \n  g={...}, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=a(...), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[], \n  o=c64[2]\n)"
+        == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[...], \n  f={...}, \n  g={...}, \n  h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  l=a(...), \n  m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00]), \n  n=bool[], \n  o=c64[2]\n)"
     )
 
     assert tree_repr(r1, depth=0) == "Repr1(...)"
 
 
 def test_str():
     assert (
@@ -80,43 +95,39 @@
         == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[...], \n  f={...}, \n  g={...}, \n  h=[[1.] [1.] [1.] [1.] [1.]], \n  i=[[1. 1. 1. 1. 1. 1.]], \n  j=[[[[1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]]]], \n  l=a(...), \n  m=[[1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]], \n  n=True, \n  o=[1.+0.j 2.+0.j]\n)"
     )
 
 
 def test_tree_summary():
     assert (
         tree_summary(r1, depth=0)
-        == "┌────┬─────┬─────┐\n│Name│Type │Count│\n├────┼─────┼─────┤\n│Σ   │Repr1│1    │\n└────┴─────┴─────┘"
+        # trunk-ignore(flake8/E501)
+        == "┌────┬─────┬─────┬───────┐\n│Name│Type │Count│Size   │\n├────┼─────┼─────┼───────┤\n│Σ   │Repr1│101  │341.00B│\n└────┴─────┴─────┴───────┘"
     )
 
     assert (
         tree_summary(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == "┌────┬────────────┬─────┐\n│Name│Type        │Count│\n├────┼────────────┼─────┤\n│.a  │int         │1    │\n├────┼────────────┼─────┤\n│.b  │str         │1    │\n├────┼────────────┼─────┤\n│.c  │float       │1    │\n├────┼────────────┼─────┤\n│.d  │str         │1    │\n├────┼────────────┼─────┤\n│.e  │list        │1    │\n├────┼────────────┼─────┤\n│.f  │set         │1    │\n├────┼────────────┼─────┤\n│.g  │dict        │1    │\n├────┼────────────┼─────┤\n│.h  │f32[5,1]    │5    │\n├────┼────────────┼─────┤\n│.i  │f32[1,6]    │6    │\n├────┼────────────┼─────┤\n│.j  │f32[1,1,4,5]│20   │\n├────┼────────────┼─────┤\n│.k  │tuple       │1    │\n├────┼────────────┼─────┤\n│.l  │a           │1    │\n├────┼────────────┼─────┤\n│.m  │f32[5,5]    │25   │\n├────┼────────────┼─────┤\n│.n  │bool[]      │1    │\n├────┼────────────┼─────┤\n│.o  │c64[2]      │2    │\n├────┼────────────┼─────┤\n│Σ   │Repr1       │68   │\n└────┴────────────┴─────┘"
+        == "┌────┬────────────┬─────┬───────┐\n│Name│Type        │Count│Size   │\n├────┼────────────┼─────┼───────┤\n│.a  │int         │1    │       │\n├────┼────────────┼─────┼───────┤\n│.b  │str         │1    │       │\n├────┼────────────┼─────┼───────┤\n│.c  │float       │1    │       │\n├────┼────────────┼─────┼───────┤\n│.d  │str         │1    │       │\n├────┼────────────┼─────┼───────┤\n│.e  │list        │5    │       │\n├────┼────────────┼─────┼───────┤\n│.f  │set         │1    │       │\n├────┼────────────┼─────┼───────┤\n│.g  │dict        │27   │100.00B│\n├────┼────────────┼─────┼───────┤\n│.h  │f32[5,1]    │5    │20.00B │\n├────┼────────────┼─────┼───────┤\n│.i  │f32[1,6]    │6    │24.00B │\n├────┼────────────┼─────┼───────┤\n│.j  │f32[1,1,4,5]│20   │80.00B │\n├────┼────────────┼─────┼───────┤\n│.k  │tuple       │3    │       │\n├────┼────────────┼─────┼───────┤\n│.l  │a           │2    │       │\n├────┼────────────┼─────┼───────┤\n│.m  │f32[5,5]    │25   │100.00B│\n├────┼────────────┼─────┼───────┤\n│.n  │bool[]      │1    │1.00B  │\n├────┼────────────┼─────┼───────┤\n│.o  │c64[2]      │2    │16.00B │\n├────┼────────────┼─────┼───────┤\n│Σ   │Repr1       │101  │341.00B│\n└────┴────────────┴─────┴───────┘"
     )
 
     assert (
         tree_summary(r1, depth=2)
         == tree_summary(r1)
         # trunk-ignore(flake8/E501)
-        == "┌───────┬────────────┬─────┐\n│Name   │Type        │Count│\n├───────┼────────────┼─────┤\n│.a     │int         │1    │\n├───────┼────────────┼─────┤\n│.b     │str         │1    │\n├───────┼────────────┼─────┤\n│.c     │float       │1    │\n├───────┼────────────┼─────┤\n│.d     │str         │1    │\n├───────┼────────────┼─────┤\n│.e[0]  │int         │1    │\n├───────┼────────────┼─────┤\n│.e[1]  │int         │1    │\n├───────┼────────────┼─────┤\n│.e[2]  │int         │1    │\n├───────┼────────────┼─────┤\n│.e[3]  │int         │1    │\n├───────┼────────────┼─────┤\n│.e[4]  │int         │1    │\n├───────┼────────────┼─────┤\n│.f     │set         │1    │\n├───────┼────────────┼─────┤\n│.g['a']│str         │1    │\n├───────┼────────────┼─────┤\n│.g['b']│str         │1    │\n├───────┼────────────┼─────┤\n│.g['c']│f32[5,5]    │25   │\n├───────┼────────────┼─────┤\n│.h     │f32[5,1]    │5    │\n├───────┼────────────┼─────┤\n│.i     │f32[1,6]    │6    │\n├───────┼────────────┼─────┤\n│.j     │f32[1,1,4,5]│20   │\n├───────┼────────────┼─────┤\n│.k[0]  │int         │1    │\n├───────┼────────────┼─────┤\n│.k[1]  │int         │1    │\n├───────┼────────────┼─────┤\n│.k[2]  │int         │1    │\n├───────┼────────────┼─────┤\n│.l.b   │int         │1    │\n├───────┼────────────┼─────┤\n│.l.c   │int         │1    │\n├───────┼────────────┼─────┤\n│.m     │f32[5,5]    │25   │\n├───────┼────────────┼─────┤\n│.n     │bool[]      │1    │\n├───────┼────────────┼─────┤\n│.o     │c64[2]      │2    │\n├───────┼────────────┼─────┤\n│Σ      │Repr1       │101  │\n└───────┴────────────┴─────┘"
+        == "┌───────┬────────────┬─────┬───────┐\n│Name   │Type        │Count│Size   │\n├───────┼────────────┼─────┼───────┤\n│.a     │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.b     │str         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.c     │float       │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.d     │str         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.e[0]  │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.e[1]  │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.e[2]  │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.e[3]  │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.e[4]  │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.f     │set         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.g['a']│str         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.g['b']│str         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.g['c']│f32[5,5]    │25   │100.00B│\n├───────┼────────────┼─────┼───────┤\n│.h     │f32[5,1]    │5    │20.00B │\n├───────┼────────────┼─────┼───────┤\n│.i     │f32[1,6]    │6    │24.00B │\n├───────┼────────────┼─────┼───────┤\n│.j     │f32[1,1,4,5]│20   │80.00B │\n├───────┼────────────┼─────┼───────┤\n│.k[0]  │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.k[1]  │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.k[2]  │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.l.b   │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.l.c   │int         │1    │       │\n├───────┼────────────┼─────┼───────┤\n│.m     │f32[5,5]    │25   │100.00B│\n├───────┼────────────┼─────┼───────┤\n│.n     │bool[]      │1    │1.00B  │\n├───────┼────────────┼─────┼───────┤\n│.o     │c64[2]      │2    │16.00B │\n├───────┼────────────┼─────┼───────┤\n│Σ      │Repr1       │101  │341.00B│\n└───────┴────────────┴─────┴───────┘"
     )
 
 
-def _tree_to_indent(str):
-    return str.replace("├── ", "    ").replace("└── ", "    ").replace("│", " ")
-
-
 def test_tree_diagram():
-    assert tree_diagram(r1, depth=0) == tree_indent(r1, depth=0) == "Repr1(...)"
+    assert tree_diagram(r1, depth=0) == "Repr1(...)"
 
     # trunk-ignore(flake8/E501)
-    out = "Repr1\n├── .a=1\n├── .b='string'\n├── .c=1.0\n├── .d='aaaaa'\n├── .e=[...]\n├── .f={...}\n├── .g={...}\n├── .h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .k=(...)\n├── .l=a(...)\n├── .m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .n=bool[]\n└── .o=c64[2]"
+    out = "Repr1\n├── .a=1\n├── .b=string\n├── .c=1.0\n├── .d=aaaaa\n├── .e=[...]\n├── .f={...}\n├── .g={...}\n├── .h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .k=(...)\n├── .l=a(...)\n├── .m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])\n├── .n=bool[]\n└── .o=c64[2]"
 
     assert tree_diagram(r1, depth=1) == out
-    assert tree_indent(r1, depth=1) == _tree_to_indent(out)
 
 
 def test_custom_jax_class():
     @jtu.register_pytree_node_class
     class Test:
         def __init__(self):
             self.a = 1
@@ -130,37 +141,35 @@
             return cls(*children)
 
     t = Test()
 
     out = "Test\n├── .leaf_0=1\n└── .leaf_1=2"
     assert tree_diagram(t) == tree_diagram(t, depth=3) == out
 
-    assert tree_indent(t) == tree_indent(t, depth=3) == _tree_to_indent(out)
     assert (
         tree_summary(t)
         == tree_summary(t, depth=4)
         # trunk-ignore(flake8/E501)
-        == "┌───────┬────┬─────┐\n│Name   │Type│Count│\n├───────┼────┼─────┤\n│.leaf_0│int │1    │\n├───────┼────┼─────┤\n│.leaf_1│int │1    │\n├───────┼────┼─────┤\n│Σ      │Test│2    │\n└───────┴────┴─────┘"
+        == "┌───────┬────┬─────┬────┐\n│Name   │Type│Count│Size│\n├───────┼────┼─────┼────┤\n│.leaf_0│int │1    │    │\n├───────┼────┼─────┼────┤\n│.leaf_1│int │1    │    │\n├───────┼────┼─────┼────┤\n│Σ      │Test│2    │    │\n└───────┴────┴─────┴────┘"
     )
 
     assert tree_repr(Test) == repr(Test)
     assert tree_str(Test) == str(Test)
 
 
-@pytest.mark.skip(reason="depends on object id")
 def test_tree_mermaid():
     assert (
-        tree_mermaid(r1, depth=1)
+        re.sub(r"id\d*", "***", tree_mermaid(r1, depth=1))
         # trunk-ignore(flake8/E501)
-        == 'flowchart LR\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>.a=1</b>")\n    id0 --- id2("</b>.b=\'string\'</b>")\n    id0 --- id3("</b>.c=1.0</b>")\n    id0 --- id4("</b>.d=\'aaaaa\'</b>")\n    id0 --- id5("</b>.e=[...]</b>")\n    id0 --- id6("</b>.f={...}</b>")\n    id0 --- id7("</b>.g={...}</b>")\n    id0 --- id8("</b>.h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id9("</b>.i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id10("</b>.j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id11("</b>.k=(...)</b>")\n    id0 --- id12("</b>.l=a(...)</b>")\n    id0 --- id13("</b>.m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id14("</b>.n=bool[]</b>")\n    id0 --- id15("</b>.o=c64[2]</b>")\n'
+        == 'flowchart LR\n    ***("<b>Repr1</b>")\n    *** --- ***("<b>.a=1</b>")\n    *** --- ***("<b>.b=string</b>")\n    *** --- ***("<b>.c=1.0</b>")\n    *** --- ***("<b>.d=aaaaa</b>")\n    *** --- ***("<b>.e=[...]</b>")\n    *** --- ***("<b>.f={...}</b>")\n    *** --- ***("<b>.g={...}</b>")\n    *** --- ***("<b>.h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    *** --- ***("<b>.i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    *** --- ***("<b>.j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    *** --- ***("<b>.k=(...)</b>")\n    *** --- ***("<b>.l=a(...)</b>")\n    *** --- ***("<b>.m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    *** --- ***("<b>.n=bool[]</b>")\n    *** --- ***("<b>.o=c64[2]</b>")'
     )
     assert (
-        tree_mermaid(r1, depth=2)
+        re.sub(r"id\d*", "***", tree_mermaid(r1, depth=2))
         # trunk-ignore(flake8/E501)
-        == 'flowchart LR\n    id5 --- id6("</b>[0]=10</b>")\n    id5 --- id7("</b>[1]=10</b>")\n    id5 --- id8("</b>[2]=10</b>")\n    id5 --- id9("</b>[3]=10</b>")\n    id5 --- id10("</b>[4]=10</b>")\n    id12 --- id13("</b>[\'a\']=\'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\'</b>")\n    id12 --- id14("</b>[\'b\']=\'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb\'</b>")\n    id12 --- id15("</b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id19 --- id20("</b>[0]=1</b>")\n    id19 --- id21("</b>[1]=2</b>")\n    id19 --- id22("</b>[2]=3</b>")\n    id23 --- id24("</b>.b=1</b>")\n    id23 --- id25("</b>.c=2</b>")\n    id0(<b>Repr1</b>)\n    id0 --- id1("</b>.a=1</b>")\n    id0 --- id2("</b>.b=\'string\'</b>")\n    id0 --- id3("</b>.c=1.0</b>")\n    id0 --- id4("</b>.d=\'aaaaa\'</b>")\n    id0 --- id5("</b>.e:list</b>")\n    id0 --- id11("</b>.f={...}</b>")\n    id0 --- id12("</b>.g:dict</b>")\n    id0 --- id16("</b>.h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id17("</b>.i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id18("</b>.j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id19("</b>.k:tuple</b>")\n    id0 --- id23("</b>.l:a</b>")\n    id0 --- id26("</b>.m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    id0 --- id27("</b>.n=bool[]</b>")\n    id0 --- id28("</b>.o=c64[2]</b>")\n'
+        == 'flowchart LR\n    ***("<b>Repr1</b>")\n    *** --- ***("<b>.a=1</b>")\n    *** --- ***("<b>.b=string</b>")\n    *** --- ***("<b>.c=1.0</b>")\n    *** --- ***("<b>.d=aaaaa</b>")\n    *** --- ***("<b>.e:list</b>")\n    *** --- ***("<b>[0]=10</b>")\n    *** --- ***("<b>[1]=10</b>")\n    *** --- ***("<b>[2]=10</b>")\n    *** --- ***("<b>[3]=10</b>")\n    *** --- ***("<b>[4]=10</b>")\n    *** --- ***("<b>.f={...}</b>")\n    *** --- ***("<b>.g:dict</b>")\n    *** --- ***("<b>[\'a\']=aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa</b>")\n    *** --- ***("<b>[\'b\']=bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb</b>")\n    *** --- ***("<b>[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    *** --- ***("<b>.h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    *** --- ***("<b>.i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    *** --- ***("<b>.j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    *** --- ***("<b>.k:tuple</b>")\n    *** --- ***("<b>[0]=1</b>")\n    *** --- ***("<b>[1]=2</b>")\n    *** --- ***("<b>[2]=3</b>")\n    *** --- ***("<b>.l:a</b>")\n    *** --- ***("<b>.b=1</b>")\n    *** --- ***("<b>.c=2</b>")\n    *** --- ***("<b>.m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])</b>")\n    *** --- ***("<b>.n=bool[]</b>")\n    *** --- ***("<b>.o=c64[2]</b>")'
     )
 
 
 def test_misc():
     x = (1, 2, 3)
     assert tree_repr(x) == tree_str(x) == "(1, 2, 3)"
 
@@ -205,16 +214,14 @@
 
     tree = L2()
     # trunk-ignore(flake8/E501)
     out = "L2\n├── .e=4\n├── .f:L1\n│   ├── .c:L0\n│   │   ├── .a=1\n│   │   └── .b=2\n│   └── .d=3\n├── .g:L0\n│   ├── .a=1\n│   └── .b=2\n└── .h=5"
 
     assert (tree_diagram(tree)) == out
 
-    assert tree_indent(tree) == _tree_to_indent(out)
-
     class L0(TreeClass):
         a: int = 1
 
     class L1(TreeClass):
         b: L0 = L0()
 
     tree = L1()
@@ -245,7 +252,14 @@
     )
 
     assert (
         str(tree_repr_with_trace(tree, transpose=True))
         # trunk-ignore(flake8/E501)
         == "Test(\n  a=\n    ┌─────┬─────────┬─────────┐\n    │Value│Name path│Type path│\n    ├─────┼─────────┼─────────┤\n    │1    │.a       │int      │\n    └─────┴─────────┴─────────┘, \n  b=\n    ┌─────┬─────────┬─────────┐\n    │Value│Name path│Type path│\n    ├─────┼─────────┼─────────┤\n    │2.0  │.b       │float    │\n    └─────┴─────────┴─────────┘\n)"
     )
+
+
+def test_tree_graph():
+    assert (
+        re.sub(r"\b\d{10,}", "***", tree_graph(r1))
+        == 'digraph G {\n    *** [label="Repr1", shape=box];\n    *** [label=".a=1", shape=box];\n    *** -> ***;\n    *** [label=".b=string", shape=box];\n    *** -> ***;\n    *** [label=".c=1.0", shape=box];\n    *** -> ***;\n    *** [label=".d=aaaaa", shape=box];\n    *** -> ***;\n    *** [label=".e:list", shape=box];\n    *** -> ***;\n    *** [label="[0]=10", shape=box];\n    *** -> ***;\n    *** [label="[1]=10", shape=box];\n    *** -> ***;\n    *** [label="[2]=10", shape=box];\n    *** -> ***;\n    *** [label="[3]=10", shape=box];\n    *** -> ***;\n    *** [label="[4]=10", shape=box];\n    *** -> ***;\n    *** [label=".f={...}", shape=box];\n    *** -> ***;\n    *** [label=".g:dict", shape=box];\n    *** -> ***;\n    *** [label="[\'a\']=aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa", shape=box];\n    *** -> ***;\n    *** [label="[\'b\']=bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb", shape=box];\n    *** -> ***;\n    *** [label="[\'c\']=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])", shape=box];\n    *** -> ***;\n    *** [label=".h=f32[5,1](μ=1.00, σ=0.00, ∈[1.00,1.00])", shape=box];\n    *** -> ***;\n    *** [label=".i=f32[1,6](μ=1.00, σ=0.00, ∈[1.00,1.00])", shape=box];\n    *** -> ***;\n    *** [label=".j=f32[1,1,4,5](μ=1.00, σ=0.00, ∈[1.00,1.00])", shape=box];\n    *** -> ***;\n    *** [label=".k:tuple", shape=box];\n    *** -> ***;\n    *** [label="[0]=1", shape=box];\n    *** -> ***;\n    *** [label="[1]=2", shape=box];\n    *** -> ***;\n    *** [label="[2]=3", shape=box];\n    *** -> ***;\n    *** [label=".l:a", shape=box];\n    *** -> ***;\n    *** [label=".b=1", shape=box];\n    *** -> ***;\n    *** [label=".c=2", shape=box];\n    *** -> ***;\n    *** [label=".m=f32[5,5](μ=1.00, σ=0.00, ∈[1.00,1.00])", shape=box];\n    *** -> ***;\n    *** [label=".n=bool[]", shape=box];\n    *** -> ***;\n    *** [label=".o=c64[2]", shape=box];\n    *** -> ***;\n}'
+    )
```

### Comparing `pytreeclass-0.3.8/tests/test_treeclass.py` & `pytreeclass-0.4.0/tests/test_treeclass.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,24 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import copy
 import dataclasses as dc
+import inspect
 from typing import Any
 
 import jax
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 from jax import numpy as jnp
@@ -541,7 +556,42 @@
     assert f_a(1) == 6
 
     f_b = pytc.Partial(f, 1, ..., 3)
     assert f_b(2) == 6
 
     assert f_b == f_b
     assert hash(f_b) == hash(f_b)
+
+
+def test_kind():
+    class Tree(pytc.TreeClass):
+        a: int = pytc.field(kind="VAR_POS")
+        b: int = pytc.field(kind="POS_ONLY")
+        c: int = pytc.field(kind="VAR_KW")
+        d: int
+
+    params = dict(inspect.signature(Tree.__init__).parameters)
+
+    assert params["a"].kind is inspect.Parameter.VAR_POSITIONAL
+    assert params["b"].kind is inspect.Parameter.POSITIONAL_ONLY
+    assert params["c"].kind is inspect.Parameter.VAR_KEYWORD
+    assert params["d"].kind is inspect.Parameter.POSITIONAL_OR_KEYWORD
+
+    class Tree(pytc.TreeClass):
+        a: int = pytc.field(kind="VAR_POS")
+        b: int = pytc.field(kind="KW_ONLY")
+
+    params = dict(inspect.signature(Tree.__init__).parameters)
+    assert params["a"].kind is inspect.Parameter.VAR_POSITIONAL
+    assert params["b"].kind is inspect.Parameter.KEYWORD_ONLY
+
+    with pytest.raises(TypeError):
+
+        class Tree(pytc.TreeClass):
+            a: int = pytc.field(kind="VAR_POS")
+            b: int = pytc.field(kind="VAR_POS")
+
+    with pytest.raises(TypeError):
+
+        class Tree(pytc.TreeClass):
+            a: int = pytc.field(kind="VAR_KW")
+            b: int = pytc.field(kind="VAR_KW")
```

### Comparing `pytreeclass-0.3.8/tests/test_under_jit.py` & `pytreeclass-0.4.0/tests/test_under_jit.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+
 import jax
 from jax import numpy as jnp
 
 import pytreeclass as pytc
 
 
 def test_ops_with_jit():
```

