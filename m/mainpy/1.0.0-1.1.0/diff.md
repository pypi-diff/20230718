# Comparing `tmp/mainpy-1.0.0.tar.gz` & `tmp/mainpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainpy-1.0.0.tar", max compression
+gzip compressed data, was "mainpy-1.1.0.tar", max compression
```

## Comparing `mainpy-1.0.0.tar` & `mainpy-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1068 2022-03-15 19:48:00.774000 mainpy-1.0.0/LICENSE
--rw-r--r--   0        0        0     1445 2022-04-02 20:43:58.185815 mainpy-1.0.0/README.md
--rw-r--r--   0        0        0     2624 2022-04-02 20:32:22.892412 mainpy-1.0.0/mainpy/__init__.py
--rw-r--r--   0        0        0        0 2022-04-02 14:23:11.563699 mainpy-1.0.0/mainpy/py.typed
--rw-r--r--   0        0        0      719 2022-04-02 20:43:58.193815 mainpy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2212 2022-04-02 20:44:01.081334 mainpy-1.0.0/setup.py
--rw-r--r--   0        0        0     2187 2022-04-02 20:44:01.081544 mainpy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-03-15 19:48:00.774000 mainpy-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2844 2023-07-18 14:23:56.162028 mainpy-1.1.0/README.md
+-rw-r--r--   0        0        0     3142 2023-07-18 14:23:56.162028 mainpy-1.1.0/mainpy/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-02 14:23:11.563699 mainpy-1.1.0/mainpy/py.typed
+-rw-r--r--   0        0        0     1017 2023-07-18 14:24:41.527017 mainpy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3829 1970-01-01 00:00:00.000000 mainpy-1.1.0/PKG-INFO
```

### Comparing `mainpy-1.0.0/LICENSE` & `mainpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mainpy-1.0.0/mainpy/__init__.py` & `mainpy-1.1.0/mainpy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
-__all__ = ('main', )
+__all__ = ('main',)
 
 import asyncio
 import functools
 import os
 import sys
+from types import FrameType
 
 from typing import (
     Any,
     Awaitable,
     Callable,
     cast,
     Coroutine,
-    overload,
     TypeVar,
-    Union
+    Union,
+    Optional,
 )
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 _T = TypeVar('_T')
-_F = TypeVar('_F', bound=Callable)
 _R = TypeVar('_R', bound=object)
 
 _SCallable: TypeAlias = Union[Callable[..., _T], Callable[[], _T]]
 _ACallable: TypeAlias = _SCallable[Awaitable[_R]]
 _XCallable: TypeAlias = Union[_SCallable[_R], _ACallable[_R]]
 
 
@@ -40,83 +40,92 @@
 
     if '--debug' in sys.argv[1:]:
         return True
 
     env_debug = os.environ.get('DEBUG', '0')
     try:
         env_debug = int(env_debug)
-    except ValueError:
-        pass
+    except ValueError as e:
+        raise EnvironmentError('failed to parse the `DEBUG` env var') from e
+
     return bool(env_debug)
 
 
 # noinspection PyPackageRequirements
 def _infer_uvloop() -> bool:
     try:
-        import uvloop
+        import uvloop  # pyright: ignore [reportUnusedImport]
     except ImportError:
         return False
     else:
         return True
 
 
 def _enable_debug():
     env = os.environ
 
     if not env.get('PYTHONWARNINGS'):
         import warnings
+
         warnings.simplefilter('always')
 
     if not (env.get('PYTHONDEVMODE') or env.get('PYTHONFAULTHANDLER')):
         import faulthandler
+
         faulthandler.enable()
 
 
-# noinspection PyPackageRequirements,PyUnresolvedReferences
 def main(
     function: _XCallable[_R] | None = None,
     *,
     debug: bool | None = None,
     is_async: bool | None = None,
     use_uvloop: bool | None = None,
-) -> Union[Callable[[_XCallable[_R]], _R], _R]:
+) -> Union[_XCallable[_R], _R]:
     if function is None:
         return cast(
             Callable[[_XCallable[_R]], _R],
             functools.partial(
-                main,
-                debug=debug,
-                is_async=is_async,
-                use_uvloop=use_uvloop
-            )
+                main, debug=debug, is_async=is_async, use_uvloop=use_uvloop
+            ),
         )
 
     if not callable(function):
         raise TypeError(f'expected a callable, got {type(function).__name__}')
 
-    if function.__module__ != '__main__':
+    if function.__module__ == '__main__':
+        pass
+    elif hasattr(sys, '_getframe'):
+        # Get current frame, effectively identical to `inspect.currentframe()`
+        frame: Optional[FrameType] = \
+            sys._getframe(1)  # type: ignore[attr-defined]
+
+        # Make sure we have a frame
+        if not frame:
+            return function
+        # Get the name from the frame's globals and check if it's '__main__'
+        if frame.f_globals.get('__name__') != '__main__':
+            return function
+    else:
         return function
 
     if debug is None:
         debug = _infer_debug()
 
     if debug:
         _enable_debug()
 
     if is_async or is_async is None and asyncio.iscoroutinefunction(function):
         if use_uvloop or use_uvloop is None and _infer_uvloop():
             import uvloop
-            uvloop.install()
 
-        return asyncio.run(
-            cast(Coroutine[Any, Any, _R], function()),
-            debug=debug
-        )
+            uvloop.install()  # pyright: ignore [reportUnknownMemberType]
 
-    else:
-        return function()
+        return asyncio.run(cast(Coroutine[Any, Any, _R], function()), debug=debug)
+
+    return cast(_R, function())
 
 
 @main
-def __main():
+def __main():  # pyright: ignore [reportUnusedFunction]
     # this should never run
     assert False
```

### Comparing `mainpy-1.0.0/PKG-INFO` & `mainpy-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,128 @@
-Metadata-Version: 2.1
-Name: mainpy
-Version: 1.0.0
-Summary: Simplify your project's main entrypoint definition with @main
-Home-page: https://github.com/jorenham/mainpy
-License: MIT
-Author: Joren Hammudoglu
-Author-email: jhammudoglu@gmail.com
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: typing_extensions (>=4.1,<5.0); python_version < "3.10"
-Project-URL: Repository, https://github.com/jorenham/mainpy
-Description-Content-Type: text/markdown
-
 # `@main`.py
 
 -----
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/mainpy.svg)](https://pypi.python.org/pypi/mainpy/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mainpy.svg)](https://pypi.python.org/pypi/mainpy/)
 [![PyPI license](https://img.shields.io/pypi/l/mainpy.svg)](https://pypi.python.org/pypi/mainpy/)
 
 -----
 
-## Installation
+## Basic Examples
 
-```bash
-pip install mainpy
-```
+Instead of the verbose "boilerplate"
 
-*requires python > 3.7*
+```python
+def main(): ...
+
+if __name__ == '__main__':
+    main()
+```
 
-## Usage
+mainpy can be used to write it as:
 
 ```python
 from mainpy import main
 
 @main
 def app(): ...
 ```
 
-Async functions will be automatically wrapped in `asyncio.run`.
+Similarly, the async boilerplate
+
+```python
+import asyncio
+
+async def main(): ...
+
+if __name__ == '__main__':
+    asyncio.run(main())
+```
+
+can be replaced with
 
 ```python
 @main
 async def async_app(): ...
 ```
 
-# Automatic uvloop usage
+If, for some reason, you cannot or don't want to use a decorator, you can also call the decorator with the function as an argument:
+
+```python
+import mainpy
+
+
+def main(): ...
+
+
+mainpy.main(main)
+```
+
+## External Libraries
+
+
+### Click
+
+With `click` you can simply add the decorator as usual, as long as you keep in mind that it has to be the first decorator (i.e. above the `@click.command()`):
+
+```python
+import click
+
+import mainpy
+
+
+@mainpy.main
+@click.command()
+def click_command():
+    click.echo('Hello from click_command')
+```
+
+If you want to use `@click.group` you probably don't want to decorate the group because the decorator will immediately execute. In those cases you probably want to move the `mainpy.main(...)` execution to the bottom of the file:
+
+
+```python
+import click
+
+import mainpy
+
+
+@click.group()
+def group(): ...
+    
+
+@group.command()
+def command(): ...
+
+
+mainpy.main(group)
+```
+
+### Typer
+
+When using `typer` you also need to use the regular call instead of the decorator:
+
+```python
+import typer
+
+import mainpy
+
+
+app = typer.Typer()
+
+
+@app.command()
+def command():
+    typer.echo('typer.Typer()')
+
+
+mainpy.main(app)
+```
+
+## Automatic uvloop usage
 
 If you have [uvloop](https://github.com/MagicStack/uvloop) installed, mainpy
 will automatically call `uvloop.install()` before running your async main 
 function. This can be disabled by setting `use_uvloop=False`, e.g.:
 
 ```python
 @main(use_uvloop=False)
@@ -72,7 +139,15 @@
 [asyncio debug mode](https://docs.python.org/3/library/asyncio-dev.html#asyncio-debug-mode):
 
 ```python
 @main(debug=True)
 def app(): ...
 ```
 
+
+## Installation
+
+```bash
+pip install mainpy
+```
+
+*requires python > 3.7*
```

