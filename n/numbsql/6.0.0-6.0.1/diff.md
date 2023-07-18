# Comparing `tmp/numbsql-6.0.0.tar.gz` & `tmp/numbsql-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbsql-6.0.0.tar", max compression
+gzip compressed data, was "numbsql-6.0.1.tar", max compression
```

## Comparing `numbsql-6.0.0.tar` & `numbsql-6.0.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    11352 2022-12-06 17:32:16.589495 numbsql-6.0.0/LICENSE
--rw-r--r--   0        0        0     2946 2022-12-06 17:32:16.589495 numbsql-6.0.0/README.md
--rw-r--r--   0        0        0     6920 2022-12-06 17:33:48.814575 numbsql-6.0.0/numbsql/__init__.py
--rw-r--r--   0        0        0     4667 2022-12-06 17:32:16.589495 numbsql-6.0.0/numbsql/aggregate.py
--rw-r--r--   0        0        0      955 2022-12-06 17:32:16.589495 numbsql-6.0.0/numbsql/exceptions.py
--rw-r--r--   0        0        0    19140 2022-12-06 17:32:16.589495 numbsql-6.0.0/numbsql/numbaext.py
--rw-r--r--   0        0        0     1996 2022-12-06 17:32:16.589495 numbsql-6.0.0/numbsql/scalar.py
--rw-r--r--   0        0        0     9168 2022-12-06 17:32:16.589495 numbsql-6.0.0/numbsql/sqlite.py
--rw-r--r--   0        0        0     2850 2022-12-06 17:32:16.589495 numbsql-6.0.0/numbsql/tests/conftest.py
--rw-r--r--   0        0        0    10372 2022-12-06 17:32:16.589495 numbsql-6.0.0/numbsql/tests/test_aggregate.py
--rw-r--r--   0        0        0      933 2022-12-06 17:32:16.589495 numbsql-6.0.0/numbsql/tests/test_numbaext.py
--rw-r--r--   0        0        0     8320 2022-12-06 17:32:16.589495 numbsql-6.0.0/numbsql/tests/test_scalar.py
--rw-r--r--   0        0        0      166 2022-12-06 17:32:16.589495 numbsql-6.0.0/numbsql/tests/test_version.py
--rw-r--r--   0        0        0     2110 2022-12-06 17:33:50.974599 numbsql-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     3863 1970-01-01 00:00:00.000000 numbsql-6.0.0/setup.py
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 numbsql-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11352 2023-07-18 11:56:04.414511 numbsql-6.0.1/LICENSE
+-rw-r--r--   0        0        0     2946 2023-07-18 11:56:04.414511 numbsql-6.0.1/README.md
+-rw-r--r--   0        0        0     6956 2023-07-18 11:57:01.366348 numbsql-6.0.1/numbsql/__init__.py
+-rw-r--r--   0        0        0     4772 2023-07-18 11:56:04.414511 numbsql-6.0.1/numbsql/aggregate.py
+-rw-r--r--   0        0        0      991 2023-07-18 11:56:04.414511 numbsql-6.0.1/numbsql/exceptions.py
+-rw-r--r--   0        0        0    18928 2023-07-18 11:56:04.414511 numbsql-6.0.1/numbsql/numbaext.py
+-rw-r--r--   0        0        0     1971 2023-07-18 11:56:04.414511 numbsql-6.0.1/numbsql/scalar.py
+-rw-r--r--   0        0        0     9247 2023-07-18 11:56:04.414511 numbsql-6.0.1/numbsql/sqlite.py
+-rw-r--r--   0        0        0     2886 2023-07-18 11:56:04.414511 numbsql-6.0.1/numbsql/tests/conftest.py
+-rw-r--r--   0        0        0    10499 2023-07-18 11:56:04.414511 numbsql-6.0.1/numbsql/tests/test_aggregate.py
+-rw-r--r--   0        0        0      969 2023-07-18 11:56:04.414511 numbsql-6.0.1/numbsql/tests/test_numbaext.py
+-rw-r--r--   0        0        0     8356 2023-07-18 11:56:04.414511 numbsql-6.0.1/numbsql/tests/test_scalar.py
+-rw-r--r--   0        0        0      202 2023-07-18 11:56:04.414511 numbsql-6.0.1/numbsql/tests/test_version.py
+-rw-r--r--   0        0        0     2045 2023-07-18 11:57:04.078333 numbsql-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 numbsql-6.0.1/PKG-INFO
```

### Comparing `numbsql-6.0.0/LICENSE` & `numbsql-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `numbsql-6.0.0/README.md` & `numbsql-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `numbsql-6.0.0/numbsql/__init__.py` & `numbsql-6.0.1/numbsql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sqlite3
 from ctypes import byref, c_bool, py_object, pythonapi
 from typing import Any, Callable
 
 from numba import cfunc
 from numba.types import ClassType, void, voidptr
 
@@ -39,15 +41,15 @@
 __all__ = (
     "create_function",
     "create_aggregate",
     "sqlite_udf",
     "sqlite_udaf",
 )
 
-__version__ = "6.0.0"
+__version__ = "6.0.1"
 
 
 def create_function(
     con: sqlite3.Connection,
     name: str,
     num_params: int,
     func: Callable[..., Any],
```

### Comparing `numbsql-6.0.0/numbsql/aggregate.py` & `numbsql-6.0.1/numbsql/aggregate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import inspect
+from __future__ import annotations
+
+import typing
 from typing import Tuple, Type
 
 from numba import cfunc, types, void
 from numba.types import CPointer, intc, voidptr
 
 from .exceptions import UnsupportedAggregateTypeError
 from .numbaext import (
     init,
     is_not_null_pointer,
     make_arg_tuple,
-    python_signature_to_numba_signature,
+    python_type_hints_to_numba_signature,
     reset_init,
     sizeof,
     sqlite3_result,
     unsafe_cast,
 )
 from .sqlite import sqlite3_aggregate_context, sqlite3_result_null, sqlite3_user_data
 
@@ -39,22 +41,22 @@
     for field, typ in class_type.struct.items():
         if typ not in _SUPPORTED_AGGREGATE_TYPES:
             raise UnsupportedAggregateTypeError(typ)
 
     instance_type = class_type.instance_type
 
     init_func = class_type.jit_methods["__init__"]
-    init_signature = python_signature_to_numba_signature(
-        inspect.signature(cls.__init__), self_type=instance_type
+    init_signature = python_type_hints_to_numba_signature(
+        typing.get_type_hints(class_type.methods["__init__"]), self_type=instance_type
     )
     init_func.compile(init_signature)
 
     step_func = class_type.jit_methods["step"]
-    step_signature = python_signature_to_numba_signature(
-        inspect.signature(cls.step),
+    step_signature = python_type_hints_to_numba_signature(
+        typing.get_type_hints(class_type.methods["step"]),
         self_type=instance_type,
     )
     step_func.compile(step_signature)
 
     @cfunc(void(voidptr, intc, CPointer(voidptr)))  # type: ignore[misc]
     def step(  # type: ignore[no-untyped-def]
         ctx, argc: int, argv
@@ -65,16 +67,16 @@
             agg_ctx = unsafe_cast(raw_pointer, cls)
             is_initialized = sqlite3_user_data(ctx)
             init(agg_ctx, is_initialized)
             args = make_arg_tuple(step_func, argv)
             agg_ctx.step(*args)
 
     finalize_func = class_type.jit_methods["finalize"]
-    finalize_signature = python_signature_to_numba_signature(
-        inspect.signature(cls.finalize), self_type=instance_type
+    finalize_signature = python_type_hints_to_numba_signature(
+        typing.get_type_hints(class_type.methods["finalize"]), self_type=instance_type
     )
     finalize_func.compile(finalize_signature)
 
     @cfunc(void(voidptr))  # type: ignore[misc]
     def finalize(ctx) -> None:  # type: ignore[no-untyped-def]  # pragma: no cover
         raw_pointer = sqlite3_aggregate_context(ctx, 0)
         if is_not_null_pointer(raw_pointer):
```

### Comparing `numbsql-6.0.0/numbsql/exceptions.py` & `numbsql-6.0.1/numbsql/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Type, TypeVar
 
 from numba import types
 
 T = TypeVar("T")
```

### Comparing `numbsql-6.0.0/numbsql/numbaext.py` & `numbsql-6.0.1/numbsql/numbaext.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Welcome to hell, or heaven, depending.
 
 This module is a collection of numba extensions that perform operations
 of varying levels of danger and complexity needed to make this monstrosity
 work correctly.
 """
 
+from __future__ import annotations
+
 import contextlib
-import inspect
-from typing import Any, Callable, Generator, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Generator, MutableMapping, Tuple
 
 import numba
 from llvmlite import ir
 from llvmlite.ir.instructions import (
     CallInstr,
     Constant,
     ICMPInstr,
     InsertValue,
     LoadInstr,
     Value,
 )
-from llvmlite.llvmpy.core import Builder
 from numba import extending, types
 from numba.core import cgutils, imputils, pythonapi
 from numba.core.base import BaseContext
 from numba.core.typing import ctypes_utils
 from numba.core.typing.context import Context
 from numba.core.typing.templates import Signature
 
@@ -31,14 +31,17 @@
     SQLITE3_RESULT_SETTERS,
     SQLITE3_VALUE_EXTRACTORS,
     SQLITE_NULL,
     sqlite3_value_type,
     strlen,
 )
 
+if TYPE_CHECKING:
+    from llvmlite.ir.builder import IRBuilder
+
 
 def _add_linking_libs(context: BaseContext, call: CallInstr) -> None:
     """Add the required libs for the callable to allow inlining."""
 
     try:
         libs = call.libs
     except AttributeError:
@@ -60,15 +63,15 @@
 @extending.intrinsic  # type: ignore[misc]
 def unsafe_cast(
     typingctx: Context,
     src: types.Integer,
     dst: types.ClassType,
 ) -> Tuple[
     Signature,
-    Callable[[BaseContext, Builder, Signature, Tuple[Value, Value]], LoadInstr],
+    Callable[[BaseContext, IRBuilder, Signature, Tuple[Value, Value]], LoadInstr],
 ]:
     """Cast a void pointer to a `jitclass` type.
 
     Parameters
     ----------
     typingctx
     src
@@ -84,15 +87,15 @@
     """
     if isinstance(src, types.Integer) and isinstance(dst, types.ClassType):
         inst_typ = dst.instance_type
         sig = inst_typ(types.voidptr, dst)
 
         def codegen(
             context: BaseContext,
-            builder: Builder,
+            builder: IRBuilder,
             signature: Signature,
             args: Tuple[Value, Value],
         ) -> LoadInstr:
             ptr, _ = args
 
             # get the llvm type of the thing that would be allocated
             alloc_type = context.get_data_type(inst_typ.get_data_type())
@@ -125,25 +128,25 @@
 @extending.intrinsic  # type: ignore[misc]
 def init(
     typingctx: Context,
     inst_typ: types.ClassInstanceType,
     user_data: types.Integer,
 ) -> Tuple[
     Signature,
-    Callable[[BaseContext, Builder, Signature, Tuple[Value, Value]], None],
+    Callable[[BaseContext, IRBuilder, Signature, Tuple[Value, Value]], None],
 ]:
     """Initialize a `jitclass` by calling its constructor."""
     if isinstance(inst_typ, types.ClassInstanceType) and isinstance(
         user_data, types.Integer
     ):
         sig = types.void(inst_typ, types.voidptr)
 
         def codegen(
             context: BaseContext,
-            builder: Builder,
+            builder: IRBuilder,
             signature: Signature,
             args: Tuple[Value, Value],
         ) -> None:
             instance, user_data = args
 
             # cast the user-defined void* payload to bool*
             raw = builder.bitcast(user_data, cgutils.bool_t.as_pointer())
@@ -167,60 +170,44 @@
                 # call the constructor on the instance
                 fn(builder, [instance])
 
         return sig, codegen
     raise TypeError(f"Unable to initialize type {inst_typ}")
 
 
-def python_signature_to_numba_signature(
-    signature: inspect.Signature,
-    *,
-    self_type: Optional[types.ClassInstanceType] = None,
+def python_type_hints_to_numba_signature(
+    type_hints: MutableMapping[str, Any], *, self_type: types.ClassInstanceType
 ) -> Signature:
     """Convert a Python `inspect.Signature` object into a numba `Signature`."""
-    input_types = []
-    parameters = iter(signature.parameters.items())
-
-    try:
-        first_name, first_type = next(parameters)
-    except StopIteration:
-        pass
-    else:
-        input_types.append(
-            extending.as_numba_type(self_type if first_name == "self" else first_type)
-        )
-
-    return_ann = signature.return_annotation
-    return_type = extending.as_numba_type(
-        return_ann if return_ann is not None else types.void
+    return_type = extending.as_numba_type(type_hints.pop("return"))
+    return return_type(
+        extending.as_numba_type(self_type),
+        *map(extending.as_numba_type, type_hints.values()),
     )
 
-    input_types.extend(
-        extending.as_numba_type(param.annotation) for _, param in parameters
-    )
-    return return_type(*input_types)
-
 
 @extending.intrinsic  # type: ignore[misc]
 def reset_init(
     typingctx: Context,
     user_data: types.Integer,
-) -> Tuple[Signature, Callable[[BaseContext, Builder, Signature, Tuple[Value]], None]]:
+) -> Tuple[
+    Signature, Callable[[BaseContext, IRBuilder, Signature, Tuple[Value]], None]
+]:
     """Reset the user data when `finalize` is called.
 
     This call ensures that the constructor is called the next time the `step`
     method is invoked.
 
     """
     if isinstance(user_data, types.Integer):
         sig = types.void(types.voidptr)
 
         def codegen(
             context: BaseContext,
-            builder: Builder,
+            builder: IRBuilder,
             signature: Signature,
             args: Tuple[Value],
         ) -> None:
             (user_data,) = args
             # cast the user defined data structure, (which is current a pointer
             # to a boolean indicating whether the constructor has been called)
             # to a pointer to bool
@@ -235,15 +222,17 @@
     raise TypeError(f"Unable to uninitialize flag of type `{user_data}`")
 
 
 @extending.intrinsic  # type: ignore[misc]
 def safe_decref(
     typingctx: Context,
     pyobject_type: types.RawPointer,
-) -> Tuple[Signature, Callable[[BaseContext, Builder, Signature, Tuple[Value]], None]]:
+) -> Tuple[
+    Signature, Callable[[BaseContext, IRBuilder, Signature, Tuple[Value]], None]
+]:
     """Safely decrement the reference count of a Python object.
 
     Notes
     -----
     This function holds the GIL.
 
     There is no cause for concerns about performance here: this function is
@@ -253,15 +242,15 @@
     Additionally the GIL is only held if the user data is not a null pointer.
     """
     if isinstance(pyobject_type, types.RawPointer):
         sig = types.void(types.voidptr)
 
         def codegen(
             context: BaseContext,
-            builder: Builder,
+            builder: IRBuilder,
             signature: Signature,
             args: Tuple[Value],
         ) -> None:
             (user_data,) = args
             pyapi = context.get_python_api(builder)
             # check whether the pyobject is null, (likely not)
             with cgutils.if_likely(builder, cgutils.is_not_null(builder, user_data)):
@@ -278,15 +267,15 @@
 
 @extending.intrinsic  # type: ignore[misc]
 def make_arg_tuple(
     typingctx: Context, func: types.Callable, argv: types.CPointer
 ) -> Tuple[
     Signature,
     Callable[
-        [BaseContext, Builder, Signature, Tuple[Value, Value]],
+        [BaseContext, IRBuilder, Signature, Tuple[Value, Value]],
         InsertValue,
     ],
 ]:
     """Construct a typed argument tuple to pass to a user-defined function."""
     (func_type,), _ = func.get_call_signatures()
     first_arg, *_ = args = func_type.args
 
@@ -294,15 +283,15 @@
     first_argument_position = int(isinstance(first_arg, types.ClassInstanceType))
     argtypes = args[first_argument_position:]
     tuple_type = types.Tuple(argtypes)
     sig = tuple_type(func, types.CPointer(types.voidptr))
 
     def codegen(
         context: BaseContext,
-        builder: Builder,
+        builder: IRBuilder,
         signature: Signature,
         args: Tuple[Value, Value],
     ) -> InsertValue:
         # first argument is the instance, and we don't need it here
         _, argv = args
 
         # initialize a list to hold the converted function arguments
@@ -433,15 +422,15 @@
         return imputils.impl_ret_untracked(context, builder, tuple_type, arg_tuple)
 
     return sig, codegen
 
 
 def map_sqlite_string_to_numba_uni_str(
     context: BaseContext,
-    builder: Builder,
+    builder: IRBuilder,
     *,
     data: Value,
 ) -> LoadInstr:
     """Construct a Numba string from a raw C string coming from SQLite.
 
     There's no way this implementation is correct.
 
@@ -490,34 +479,38 @@
     #
     # We cannot bake in the hash value because of hashseed
     # randomization.
     uni_str.hash = uni_str.hash.type(-1)
     return uni_str._getvalue()
 
 
-@numba.generated_jit(nopython=True, nogil=True)  # type: ignore[misc]
-def sqlite3_result(ctx: types.Integer, value: Any) -> Callable[[Any, Any], Any]:
+def sqlite3_result(ctx: types.Integer, value: Any):  # type: ignore[no-untyped-def]
+    raise NotImplementedError(type(value))
+
+
+@extending.overload(sqlite3_result)  # type: ignore[misc]
+def ol_sqlite3_result(ctx, value):  # type: ignore[no-untyped-def]
     func = SQLITE3_RESULT_SETTERS[value]
     return lambda ctx, value: func(ctx, value)
 
 
 @extending.intrinsic  # type: ignore[misc]
 def sizeof(
     typingctx: Context, src: types.ClassType
 ) -> Tuple[
     Signature,
-    Callable[[BaseContext, Builder, Signature, Tuple[Value]], Constant],
+    Callable[[BaseContext, IRBuilder, Signature, Tuple[Value]], Constant],
 ]:
     """Return the size in bytes of a type."""
     if isinstance(src, types.ClassType):
         sig = types.int64(src)
 
         def codegen(
             context: BaseContext,
-            builder: Builder,
+            builder: IRBuilder,
             signature: Signature,
             args: Tuple[Value],
         ) -> Constant:
             data_type = context.get_data_type(src.instance_type)
             size_of_data_type = context.get_abi_sizeof(data_type)
             return context.get_constant(sig.return_type, size_of_data_type)
 
@@ -527,22 +520,22 @@
 
 
 @extending.intrinsic  # type: ignore[misc]
 def is_not_null_pointer(
     typingctx: Context, raw_pointer_type: types.Integer
 ) -> Tuple[
     Signature,
-    Callable[[BaseContext, Builder, Signature, Tuple[Value]], ICMPInstr],
+    Callable[[BaseContext, IRBuilder, Signature, Tuple[Value]], ICMPInstr],
 ]:
     if isinstance(raw_pointer_type, types.Integer):
         sig = types.boolean(raw_pointer_type)
 
         def codegen(
             context: BaseContext,
-            builder: Builder,
+            builder: IRBuilder,
             signature: Signature,
             args: Tuple[Value],
         ) -> ICMPInstr:
             return cgutils.is_not_null(builder, *args)
 
         return sig, codegen
```

### Comparing `numbsql-6.0.0/numbsql/scalar.py` & `numbsql-6.0.1/numbsql/scalar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 import functools
-import inspect
+import typing
 from typing import Any, Callable, Optional
 
 from numba import cfunc, njit
 from numba.core.ccallback import CFunc
 from numba.extending import as_numba_type
 from numba.types import CPointer, intc, void, voidptr
 
@@ -41,20 +43,17 @@
     >>> add_one(None) is None
     True
 
     """
     if func is None:
         return functools.partial(sqlite_udf, nogil=nogil, **njit_kwargs)
 
-    python_signature = inspect.signature(func)
-    return_type = as_numba_type(python_signature.return_annotation)
-    argument_types = (
-        as_numba_type(param.annotation)
-        for param in python_signature.parameters.values()
-    )
+    python_signature = typing.get_type_hints(func)
+    return_type = as_numba_type(python_signature.pop("return"))
+    argument_types = map(as_numba_type, python_signature.values())
     numba_signature = return_type(*argument_types)
     compiled_func = njit(numba_signature, nogil=nogil, **njit_kwargs)(func)
 
     @cfunc(void(voidptr, intc, CPointer(voidptr)))  # type: ignore[misc]
     def scalar(  # type: ignore[no-untyped-def]
         ctx, argc: int, argv
     ):  # pragma: no cover
```

### Comparing `numbsql-6.0.0/numbsql/sqlite.py` & `numbsql-6.0.1/numbsql/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import ctypes
 import ctypes.util
 import sqlite3
 import sys
 from ctypes import (
     CFUNCTYPE,
     POINTER,
@@ -10,26 +12,28 @@
     c_int,
     c_int64,
     c_size_t,
     c_ssize_t,
     c_ubyte,
     c_void_p,
 )
-from typing import Any, Callable, Optional, Tuple
+from typing import Any, Callable, Optional, Tuple, TYPE_CHECKING
 
 from llvmlite.ir.instructions import ExtractValue, Value
-from llvmlite.llvmpy.core import Builder
 from numba import cfunc, extending, float64, int32, int64, optional, types
 from numba.core.base import BaseContext
 from numba.core.typing.context import Context
 from numba.core.typing.templates import Signature
 from numba.types import string, void, voidptr
 
 from .exceptions import MissingLibrary
 
+if TYPE_CHECKING:
+    from llvmlite.ir.builder import IRBuilder
+
 SQLITE_OK = sqlite3.SQLITE_OK
 SQLITE_VERSION = sqlite3.sqlite_version
 SQLITE_UTF8 = 1
 SQLITE_UTF16LE = 2
 SQLITE_UTF16BE = 3
 SQLITE_UTF16 = 4
 SQLITE_NULL = 5
@@ -100,23 +104,23 @@
 
 @extending.intrinsic  # type: ignore[misc]
 def extract_raw_unicode_data(
     typingctx: Context,
     raw_chars_type: types.UnicodeType,
 ) -> Tuple[
     Signature,
-    Callable[[BaseContext, Builder, Signature, Tuple[Value]], ExtractValue],
+    Callable[[BaseContext, IRBuilder, Signature, Tuple[Value]], ExtractValue],
 ]:
     """Pull out the data and length from a Numba unicode string."""
     if isinstance(raw_chars_type, types.UnicodeType):
         sig = types.Tuple((voidptr, int64))(raw_chars_type)
 
         def codegen(
             context: BaseContext,
-            builder: Builder,
+            builder: IRBuilder,
             signature: Signature,
             args: Tuple[Value],
         ) -> ExtractValue:
             # get the first and only argument
             (arg,) = args
 
             # access the data and length fields of the unicode type struct
```

### Comparing `numbsql-6.0.0/numbsql/tests/conftest.py` & `numbsql-6.0.1/numbsql/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import itertools
 import random
 import sqlite3
 import string as strings
 from typing import Generator
 
 import pytest
```

### Comparing `numbsql-6.0.0/numbsql/tests/test_aggregate.py` & `numbsql-6.0.1/numbsql/tests/test_aggregate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import pathlib
 import sqlite3
 import sys
 from typing import List, Optional, Tuple
 
 import pytest
 from numba.experimental import jitclass
-from pkg_resources import parse_version
+from packaging.version import parse as parse_version
 from pytest_benchmark.fixture import BenchmarkFixture
 from testbook import testbook
 from testbook.client import TestbookNotebookClient
 
 from numbsql import create_aggregate, sqlite_udaf
 from numbsql.exceptions import UnsupportedAggregateTypeError
 from numbsql.sqlite import SQLITE_VERSION
@@ -194,15 +196,15 @@
 
 
 @pytest.fixture(scope="session")  # type: ignore[misc]
 def con(con: sqlite3.Connection) -> sqlite3.Connection:
     create_aggregate(con, "avg_numba", 1, Avg)
     create_aggregate(con, "bogus_count", 0, BogusCount)
     create_aggregate(con, "winavg_numba", 1, WinAvg)
-    con.create_aggregate("winavg_python", 1, WinAvgPython)
+    con.create_aggregate("winavg_python", 1, WinAvgPython)  # type: ignore[arg-type]
     return con
 
 
 def test_aggregates_with_string_fields_fail() -> None:
     with pytest.raises(
         UnsupportedAggregateTypeError,
         match=r"Aggregates with field type `unicode_type` are not yet implemented",
@@ -278,16 +280,16 @@
     )
 
 
 @pytest.fixture(scope="session")  # type: ignore[misc]
 def large_con(large_con: sqlite3.Connection) -> sqlite3.Connection:
     create_aggregate(large_con, "avg_numba", 1, Avg)
     create_aggregate(large_con, "winavg_numba", 1, WinAvg)
-    large_con.create_aggregate("avg_python", 1, AvgPython)
-    large_con.create_aggregate("winavg_python", 1, WinAvgPython)
+    large_con.create_aggregate("avg_python", 1, AvgPython)  # type: ignore[arg-type]
+    large_con.create_aggregate("winavg_python", 1, WinAvgPython)  # type: ignore[arg-type]
     return large_con
 
 
 def run_agg_low_card_group_by(
     con: sqlite3.Connection, func: str
 ) -> List[Tuple[str, Optional[float]]]:
     return con.execute(
```

### Comparing `numbsql-6.0.0/numbsql/tests/test_numbaext.py` & `numbsql-6.0.1/numbsql/tests/test_numbaext.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 from numba import TypingError, boolean, int64, njit
 
 from numbsql.numbaext import is_not_null_pointer, sizeof, unsafe_cast
 
 
 def test_sizeof_invalid() -> None:
```

### Comparing `numbsql-6.0.0/numbsql/tests/test_scalar.py` & `numbsql-6.0.1/numbsql/tests/test_scalar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sqlite3
 from typing import Callable, List, Optional, Tuple, TypeVar
 
 import pytest
 from pytest_benchmark.fixture import BenchmarkFixture
 
 from numbsql import create_function, sqlite_udf
```

### Comparing `numbsql-6.0.0/pyproject.toml` & `numbsql-6.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,62 @@
 [tool.poetry]
 name = "numbsql"
 homepage = "https://github.com/cpcloud/numbsql"
 repository = "https://github.com/cpcloud/numbsql"
-version = "6.0.0"
+version = "6.0.1"
 description = "JITted SQLite user-defined scalar and aggregate functions"
 readme = "README.md"
 authors = ["Phillip Cloud <417981+cpcloud@users.noreply.github.com>"]
 maintainers = ["Phillip Cloud <417981+cpcloud@users.noreply.github.com>"]
 classifiers = [
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4"
-llvmlite = ">=0.36,<0.40"
-numba = ">=0.53,<0.57"
+python = ">=3.8,<4"
+llvmlite = ">=0.36,<0.41"
+numba = ">=0.53,<0.58"
 
 [tool.poetry.dev-dependencies]
-black = "^22"
-flake8 = "^6"
-pathspec = "^0.10.1"
-ipykernel = "^6"
-isort = "^5.9.3"
-mypy = "^0.991"
-pydocstyle = "^6.1.1"
-pyupgrade = "^3"
-pytest = "^7"
-pytest-benchmark = "^4"
-pytest-randomly = "^3.10.1"
-pytest-xdist = "^3"
-testbook = "^0.4.2"
+black = { version = "^23.1.0", extras = ["jupyter"] }
+ipykernel = "^6.22.0"
+mypy = "^1.1.1"
+packaging = "^23.0"
+pytest = "^7.2.2"
+pytest-benchmark = "^4.0.0"
+pytest-randomly = "^3.12.0"
+pytest-xdist = "^3.2.1"
+ruff = ">=0.0.262,<1"
+testbook = ">=0.4.2,<1"
+
+[tool.ruff]
+ignore = ["E501"]
 
 [tool.pytest.ini_options]
 xfail_strict = true
 addopts = [
-  "--ignore=site-packages",
-  "--ignore=dist-packages",
   "--ignore=.direnv",
   "--ignore=examples",
   "--strict-markers",
   "--doctest-modules",
   "--benchmark-disable",
-  "--durations=10",
 ]
-norecursedirs = ["site-packages", "dist-packages", ".direnv", "examples"]
+norecursedirs = [".direnv", "examples"]
+filterwarnings = [
+  "error",
+  "ignore:Jupyter is migrating:DeprecationWarning",
+  "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
+]
 
 [tool.poetry2conda]
 name = "numbsql"
 
-[tool.isort]
-line_length = 88
-profile = "black"
-
-[tool.pydocstyle]
-convention = "numpy"
-add_ignore = ["D105", "D213", "D203"]
-match-dir = "numbsql"
-
 [tool.mypy]
 ignore_missing_imports = true
 # untyped things
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
```

### Comparing `numbsql-6.0.0/setup.py` & `numbsql-6.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,156 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: numbsql
+Version: 6.0.1
+Summary: JITted SQLite user-defined scalar and aggregate functions
+Home-page: https://github.com/cpcloud/numbsql
+Author: Phillip Cloud
+Author-email: 417981+cpcloud@users.noreply.github.com
+Maintainer: Phillip Cloud
+Maintainer-email: 417981+cpcloud@users.noreply.github.com
+Requires-Python: >=3.8,<4
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: llvmlite (>=0.36,<0.41)
+Requires-Dist: numba (>=0.53,<0.58)
+Project-URL: Repository, https://github.com/cpcloud/numbsql
+Description-Content-Type: text/markdown
 
-packages = \
-['numbsql', 'numbsql.tests']
+# Put some Numba in your SQLite
 
-package_data = \
-{'': ['*']}
+## Fair Warning
 
-install_requires = \
-['llvmlite>=0.36,<0.40', 'numba>=0.53,<0.57']
-
-setup_kwargs = {
-    'name': 'numbsql',
-    'version': '6.0.0',
-    'description': 'JITted SQLite user-defined scalar and aggregate functions',
-    'long_description': '# Put some Numba in your SQLite\n\n## Fair Warning\n\nThis library does unsafe things like pass around function pointer addresses\nas integers.  **Use at your own risk**.\n\nIf you\'re unfamiliar with why passing function pointers\' addresses around as\nintegers might be unsafe, then you shouldn\'t use this library.\n\n## Requirements\n\n* Python `>=3.7`\n* `numba`\n\nUse `nix-shell` from the repository to avoid dependency hell.\n\n## Installation\n\n* `poetry install`\n\n## Examples\n\n### Scalar Functions\n\nThese are almost the same as decorating a Python function with `numba.jit`.\n\n```python\nfrom typing import Optional\n\nfrom numbsql import sqlite_udf\n\n\n@sqlite_udf\ndef add_one(x: Optional[int]) -> Optional[int]:\n    """Add one to `x` if `x` is not NULL."""\n\n    if x is not None:\n        return x + 1\n    return None\n```\n\n\n### Aggregate Functions\n\nThese follow the API of the Python standard library\'s\n`sqlite3.Connection.create_aggregate` method. The difference with numbsql\naggregates is that they require two decorators: `numba.experimental.jit_class` and\n`numbsql.sqlite_udaf`. Let\'s define the `avg` (arithmetic mean) function for\n64-bit floating point numbers.\n\n```python\nfrom typing import Optional\n\nfrom numba.experimental import jitclass\n\nfrom numbsql import sqlite_udaf\n\n\n@sqlite_udaf\n@jitclass\nclass Avg:\n    total: float\n    count: int\n\n    def __init__(self):\n        self.total = 0.0\n        self.count = 0\n\n    def step(self, value: Optional[float]) -> None:\n        if value is not None:\n            self.total += value\n            self.count += 1\n\n    def finalize(self) -> Optional[float]:\n        if not self.count:\n            return None\n        return self.total / self.count\n```\n\n### Window Functions\n\nYou can also define window functions for use with SQLite\'s `OVER` construct:\n\n```python\nfrom typing import Optional\n\nfrom numba.experimental import jitclass\n\nfrom numbsql import sqlite_udaf\n\n\n@sqlite_udaf\n@jitclass\nclass WinAvg:  # pragma: no cover\n    total: float\n    count: int\n\n    def __init__(self) -> None:\n        self.total = 0.0\n        self.count = 0\n\n    def step(self, value: Optional[float]) -> None:\n        if value is not None:\n            self.total += value\n            self.count += 1\n\n    def finalize(self) -> Optional[float]:\n        count = self.count\n        if count:\n            return self.total / count\n        return None\n\n    def value(self) -> Optional[float]:\n        return self.finalize()\n\n    def inverse(self, value: Optional[float]) -> None:\n        if value is not None:\n            self.total -= value\n            self.count -= 1\n```\n\n#### Calling your aggregate function\n\nSimilar to scalar functions, we register the function with a `sqlite3.Connection` object:\n\n```python\n>>> import sqlite3\n>>> from numbsql import create_aggregate, create_function\n>>> con = sqlite3.connect(":memory:")\n>>> create_function(con, "add_one", 1, add_one)\n>>> con.execute("SELECT add_one(1)").fetchall()\n[(2,)]\n```\n',
-    'author': 'Phillip Cloud',
-    'author_email': '417981+cpcloud@users.noreply.github.com',
-    'maintainer': 'Phillip Cloud',
-    'maintainer_email': '417981+cpcloud@users.noreply.github.com',
-    'url': 'https://github.com/cpcloud/numbsql',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.1,<4',
-}
+This library does unsafe things like pass around function pointer addresses
+as integers.  **Use at your own risk**.
 
+If you're unfamiliar with why passing function pointers' addresses around as
+integers might be unsafe, then you shouldn't use this library.
+
+## Requirements
+
+* Python `>=3.7`
+* `numba`
+
+Use `nix-shell` from the repository to avoid dependency hell.
+
+## Installation
+
+* `poetry install`
+
+## Examples
+
+### Scalar Functions
+
+These are almost the same as decorating a Python function with `numba.jit`.
+
+```python
+from typing import Optional
+
+from numbsql import sqlite_udf
+
+
+@sqlite_udf
+def add_one(x: Optional[int]) -> Optional[int]:
+    """Add one to `x` if `x` is not NULL."""
+
+    if x is not None:
+        return x + 1
+    return None
+```
+
+
+### Aggregate Functions
+
+These follow the API of the Python standard library's
+`sqlite3.Connection.create_aggregate` method. The difference with numbsql
+aggregates is that they require two decorators: `numba.experimental.jit_class` and
+`numbsql.sqlite_udaf`. Let's define the `avg` (arithmetic mean) function for
+64-bit floating point numbers.
+
+```python
+from typing import Optional
+
+from numba.experimental import jitclass
+
+from numbsql import sqlite_udaf
+
+
+@sqlite_udaf
+@jitclass
+class Avg:
+    total: float
+    count: int
+
+    def __init__(self):
+        self.total = 0.0
+        self.count = 0
+
+    def step(self, value: Optional[float]) -> None:
+        if value is not None:
+            self.total += value
+            self.count += 1
+
+    def finalize(self) -> Optional[float]:
+        if not self.count:
+            return None
+        return self.total / self.count
+```
+
+### Window Functions
+
+You can also define window functions for use with SQLite's `OVER` construct:
+
+```python
+from typing import Optional
+
+from numba.experimental import jitclass
+
+from numbsql import sqlite_udaf
+
+
+@sqlite_udaf
+@jitclass
+class WinAvg:  # pragma: no cover
+    total: float
+    count: int
+
+    def __init__(self) -> None:
+        self.total = 0.0
+        self.count = 0
+
+    def step(self, value: Optional[float]) -> None:
+        if value is not None:
+            self.total += value
+            self.count += 1
+
+    def finalize(self) -> Optional[float]:
+        count = self.count
+        if count:
+            return self.total / count
+        return None
+
+    def value(self) -> Optional[float]:
+        return self.finalize()
+
+    def inverse(self, value: Optional[float]) -> None:
+        if value is not None:
+            self.total -= value
+            self.count -= 1
+```
+
+#### Calling your aggregate function
+
+Similar to scalar functions, we register the function with a `sqlite3.Connection` object:
+
+```python
+>>> import sqlite3
+>>> from numbsql import create_aggregate, create_function
+>>> con = sqlite3.connect(":memory:")
+>>> create_function(con, "add_one", 1, add_one)
+>>> con.execute("SELECT add_one(1)").fetchall()
+[(2,)]
+```
 
-setup(**setup_kwargs)
```

