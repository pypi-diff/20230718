# Comparing `tmp/python-exports-1.0.0.tar.gz` & `tmp/python_exports-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-exports-1.0.0.tar", max compression
+gzip compressed data, was "python_exports-1.1.0.tar", max compression
```

## Comparing `python-exports-1.0.0.tar` & `python_exports-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1068 2022-03-15 19:48:00.774000 python-exports-1.0.0/LICENSE
--rw-r--r--   0        0        0     1174 2022-03-16 13:04:12.558957 python-exports-1.0.0/README.md
--rw-r--r--   0        0        0     2926 2022-03-16 12:49:10.082098 python-exports-1.0.0/exports/__init__.py
--rw-r--r--   0        0        0        0 2022-03-16 12:49:10.070098 python-exports-1.0.0/exports/py.typed
--rw-r--r--   0        0        0      653 2022-03-16 13:12:38.447650 python-exports-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1844 2022-03-16 13:13:14.415309 python-exports-1.0.0/setup.py
--rw-r--r--   0        0        0     1802 2022-03-16 13:13:14.415515 python-exports-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 14:52:52.037451 python_exports-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1581 2023-07-18 14:31:56.732701 python_exports-1.1.0/README.md
+-rw-r--r--   0        0        0     2561 2023-07-18 14:45:12.054910 python_exports-1.1.0/exports/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-16 12:49:10.070098 python_exports-1.1.0/exports/py.typed
+-rw-r--r--   0        0        0      722 2023-07-18 14:56:28.931000 python_exports-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 python_exports-1.1.0/PKG-INFO
```

### Comparing `python-exports-1.0.0/LICENSE` & `python_exports-1.1.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2023 Joren Hammudoglu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `python-exports-1.0.0/README.md` & `python_exports-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # Explicit module exports
 
+`@export` - The DRY alternative to `__all__`
 
+-----
 
-## Installation
+[![PyPI version shields.io](https://img.shields.io/pypi/v/python-exports.svg)](https://pypi.python.org/pypi/python-exports/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/python-exports.svg)](https://pypi.python.org/pypi/python-exports/)
+[![PyPI license](https://img.shields.io/pypi/l/python-exports.svg)](https://pypi.python.org/pypi/python-exports/)
+
+-----
 
-*Requires python>=3.8*
+## Installation
 
-`pip install exports`
+`pip install python-exports`
 
 
 ## Usage
 
 ```pycon
 >>> from exports import export
 ```
```

### Comparing `python-exports-1.0.0/exports/__init__.py` & `python_exports-1.1.0/exports/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 import contextlib
 import inspect
 import threading
 import warnings
 from typing import (
+    Any,
     Callable,
-    ContextManager,
     Final,
+    Sequence,
+    cast,
     overload,
-    Type,
     TypeVar,
     Union,
 )
 
 
-_T = TypeVar('_T', bound=Union[Callable, Type])
+_T = TypeVar('_T', bound=Union[Callable[..., Any], type, object])
+_V  = TypeVar('_V')
 
 _lock: Final[threading.Lock] = threading.Lock()
 
 
+def _identity(_obj: _V) -> _V:
+    return _obj
+
+
 @overload
 def export(obj: str, *, threadsafe: bool = ...) -> Callable[[_T], _T]: ...
 @overload
 def export(obj: _T, *, threadsafe: bool = ...) -> _T: ...
 
 
 def export(
     obj: Union[_T, str],
     *,
     threadsafe: bool = False
-) -> Union[_T, Callable[[_T], _T]]:
+) -> Union[Callable[[_T], _T], _T]:
     """Add a function, class or name to __all__.
 
     If the module has no __all__, it is created. Otherwise, the export is
     appended.
 
     Can be used as function decorator:
 
@@ -76,56 +82,33 @@
     """
     module = inspect.getmodule(inspect.stack()[1][0])
     if module is None:
         raise ModuleNotFoundError(f'could not find module of {obj!r}')
 
     if isinstance(obj, str):
         name = obj
-        res = lambda _obj: _obj
+        res = _identity
     else:
         res = obj
-        name = obj.__name__
-
-    lock: ContextManager
-    if threadsafe:
-        lock = _lock
-    else:
-        lock = contextlib.nullcontext()
+        name = cast(str, getattr(obj, '__name__', None) or str(obj))
 
-    with lock:
+    with _lock if threadsafe else contextlib.nullcontext():
         if hasattr(module, '__all__'):
             if not isinstance(module.__all__, list):
                 setattr(module, '__all__', list(module.__all__))
-            exports = module.__all__[:]
+            exports = list(cast(Sequence[str], module.__all__[:]))
         else:
             setattr(module, '__all__', [])
             exports = []
 
         if name in exports:
             warnings.warn(f'{name!r} already exported')
 
         else:
             exports.append(name)
             getattr(module, '__all__')[:] = exports
 
     return res
 
 
-# you can't decorate yourself; it's a chicken/egg situation
+# effectively self-decoration
 export(export)
-
-
-@overload
-def export_threadsafe(obj: str) -> Callable[[_T], _T]: ...
-@overload
-def export_threadsafe(obj: _T) -> _T: ...
-
-
-@export
-def export_threadsafe(obj: Union[_T, str]) -> Union[_T, Callable[[_T], _T]]:
-    """Thread-safe version of export().
-
-    Uses threading.Lock when modifying __all__.
-
-    This negatively impacts performance: Don't use if not needed!
-    """
-    return export(obj, threadsafe=True)
```

### Comparing `python-exports-1.0.0/PKG-INFO` & `python_exports-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: python-exports
-Version: 1.0.0
+Version: 1.1.0
 Summary: @export decorator that adds a function or class to __all__
 Home-page: https://github.com/jorenham/exports
 License: MIT
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/jorenham/exports
 Description-Content-Type: text/markdown
 
 # Explicit module exports
 
+`@export` - The DRY alternative to `__all__`
 
+-----
 
-## Installation
+[![PyPI version shields.io](https://img.shields.io/pypi/v/python-exports.svg)](https://pypi.python.org/pypi/python-exports/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/python-exports.svg)](https://pypi.python.org/pypi/python-exports/)
+[![PyPI license](https://img.shields.io/pypi/l/python-exports.svg)](https://pypi.python.org/pypi/python-exports/)
 
-*Requires python>=3.8*
+-----
+
+## Installation
 
-`pip install exports`
+`pip install python-exports`
 
 
 ## Usage
 
 ```pycon
 >>> from exports import export
 ```
```

