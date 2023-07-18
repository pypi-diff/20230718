# Comparing `tmp/granian-0.5.1.tar.gz` & `tmp/granian-0.5.2.tar.gz`

## Comparing `granian-0.5.1.tar` & `granian-0.5.2.tar`

### file list

```diff
@@ -1,64 +1,63 @@
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 granian-0.5.1/Cargo.toml
--rw-r--r--   0     1001      123     1486 2023-07-06 22:45:53.000000 granian-0.5.1/LICENSE
--rw-r--r--   0     1001      123     5333 2023-07-06 22:45:53.000000 granian-0.5.1/README.md
--rw-r--r--   0     1001      123       54 2023-07-06 22:45:53.000000 granian-0.5.1/build.rs
--rw-r--r--   0     1001      123       28 2023-07-06 22:45:53.000000 granian-0.5.1/granian/__init__.py
--rw-r--r--   0     1001      123       35 2023-07-06 22:45:53.000000 granian-0.5.1/granian/__main__.py
--rw-r--r--   0     1001      123       22 2023-07-06 22:45:53.000000 granian-0.5.1/granian/__version__.py
--rw-r--r--   0     1001      123      261 2023-07-06 22:45:53.000000 granian-0.5.1/granian/_futures.py
--rw-r--r--   0     1001      123     2102 2023-07-06 22:45:53.000000 granian-0.5.1/granian/_granian.pyi
--rw-r--r--   0     1001      123     1677 2023-07-06 22:45:53.000000 granian-0.5.1/granian/_internal.py
--rw-r--r--   0     1001      123     2862 2023-07-06 22:45:53.000000 granian-0.5.1/granian/_loops.py
--rw-r--r--   0     1001      123       93 2023-07-06 22:45:53.000000 granian-0.5.1/granian/_types.py
--rw-r--r--   0     1001      123     4583 2023-07-06 22:45:53.000000 granian-0.5.1/granian/asgi.py
--rw-r--r--   0     1001      123     3774 2023-07-06 22:45:53.000000 granian-0.5.1/granian/cli.py
--rw-r--r--   0     1001      123      357 2023-07-06 22:45:53.000000 granian-0.5.1/granian/constants.py
--rw-r--r--   0     1001      123     1328 2023-07-06 22:45:53.000000 granian-0.5.1/granian/log.py
--rw-r--r--   0     1001      123      153 2023-07-06 22:45:53.000000 granian-0.5.1/granian/net.py
--rw-r--r--   0     1001      123        0 2023-07-06 22:45:53.000000 granian-0.5.1/granian/py.typed
--rw-r--r--   0     1001      123      462 2023-07-06 22:45:53.000000 granian-0.5.1/granian/rsgi.py
--rw-r--r--   0     1001      123    11447 2023-07-06 22:45:53.000000 granian-0.5.1/granian/server.py
--rw-r--r--   0     1001      123     2106 2023-07-06 22:45:53.000000 granian-0.5.1/granian/wsgi.py
--rw-r--r--   0     1001      123     1623 2023-07-06 22:45:53.000000 granian-0.5.1/pyproject.toml
--rw-r--r--   0     1001      123    10636 2023-07-06 22:45:53.000000 granian-0.5.1/src/asgi/callbacks.rs
--rw-r--r--   0     1001      123     2170 2023-07-06 22:45:53.000000 granian-0.5.1/src/asgi/errors.rs
--rw-r--r--   0     1001      123     5171 2023-07-06 22:45:53.000000 granian-0.5.1/src/asgi/http.rs
--rw-r--r--   0     1001      123    15937 2023-07-06 22:45:53.000000 granian-0.5.1/src/asgi/io.rs
--rw-r--r--   0     1001      123      329 2023-07-06 22:45:53.000000 granian-0.5.1/src/asgi/mod.rs
--rw-r--r--   0     1001      123     4636 2023-07-06 22:45:53.000000 granian-0.5.1/src/asgi/serve.rs
--rw-r--r--   0     1001      123     2708 2023-07-06 22:45:53.000000 granian-0.5.1/src/asgi/types.rs
--rw-r--r--   0     1001      123     9835 2023-07-06 22:45:53.000000 granian-0.5.1/src/callbacks.rs
--rw-r--r--   0     1001      123      415 2023-07-06 22:45:53.000000 granian-0.5.1/src/http.rs
--rw-r--r--   0     1001      123      550 2023-07-06 22:45:53.000000 granian-0.5.1/src/lib.rs
--rw-r--r--   0     1001      123     9755 2023-07-06 22:45:53.000000 granian-0.5.1/src/rsgi/callbacks.rs
--rw-r--r--   0     1001      123      565 2023-07-06 22:45:53.000000 granian-0.5.1/src/rsgi/errors.rs
--rw-r--r--   0     1001      123     5591 2023-07-06 22:45:53.000000 granian-0.5.1/src/rsgi/http.rs
--rw-r--r--   0     1001      123    12300 2023-07-06 22:45:53.000000 granian-0.5.1/src/rsgi/io.rs
--rw-r--r--   0     1001      123      665 2023-07-06 22:45:53.000000 granian-0.5.1/src/rsgi/mod.rs
--rw-r--r--   0     1001      123     4635 2023-07-06 22:45:53.000000 granian-0.5.1/src/rsgi/serve.rs
--rw-r--r--   0     1001      123     5538 2023-07-06 22:45:53.000000 granian-0.5.1/src/rsgi/types.rs
--rw-r--r--   0     1001      123     7978 2023-07-06 22:45:53.000000 granian-0.5.1/src/runtime.rs
--rw-r--r--   0     1001      123     4301 2023-07-06 22:45:53.000000 granian-0.5.1/src/tcp.rs
--rw-r--r--   0     1001      123     2431 2023-07-06 22:45:53.000000 granian-0.5.1/src/tls.rs
--rw-r--r--   0     1001      123      837 2023-07-06 22:45:53.000000 granian-0.5.1/src/utils.rs
--rw-r--r--   0     1001      123    16535 2023-07-06 22:45:53.000000 granian-0.5.1/src/workers.rs
--rw-r--r--   0     1001      123     3435 2023-07-06 22:45:53.000000 granian-0.5.1/src/ws.rs
--rw-r--r--   0     1001      123     1906 2023-07-06 22:45:53.000000 granian-0.5.1/src/wsgi/callbacks.rs
--rw-r--r--   0     1001      123      308 2023-07-06 22:45:53.000000 granian-0.5.1/src/wsgi/errors.rs
--rw-r--r--   0     1001      123     1626 2023-07-06 22:45:53.000000 granian-0.5.1/src/wsgi/http.rs
--rw-r--r--   0     1001      123      312 2023-07-06 22:45:53.000000 granian-0.5.1/src/wsgi/mod.rs
--rw-r--r--   0     1001      123     2228 2023-07-06 22:45:53.000000 granian-0.5.1/src/wsgi/serve.rs
--rw-r--r--   0     1001      123     5426 2023-07-06 22:45:53.000000 granian-0.5.1/src/wsgi/types.rs
--rw-r--r--   0     1001      123     3078 2023-07-06 22:45:53.000000 granian-0.5.1/tests/apps/asgi.py
--rw-r--r--   0     1001      123     2739 2023-07-06 22:45:53.000000 granian-0.5.1/tests/apps/rsgi.py
--rw-r--r--   0     1001      123     1120 2023-07-06 22:45:53.000000 granian-0.5.1/tests/apps/wsgi.py
--rw-r--r--   0     1001      123     1759 2023-07-06 22:45:53.000000 granian-0.5.1/tests/conftest.py
--rw-r--r--   0     1001      123     1139 2023-07-06 22:45:53.000000 granian-0.5.1/tests/fixtures/tls/cert.pem
--rw-r--r--   0     1001      123     1704 2023-07-06 22:45:53.000000 granian-0.5.1/tests/fixtures/tls/key.pem
--rw-r--r--   0     1001      123     1830 2023-07-06 22:45:53.000000 granian-0.5.1/tests/test_asgi.py
--rw-r--r--   0     1001      123     1851 2023-07-06 22:45:53.000000 granian-0.5.1/tests/test_https.py
--rw-r--r--   0     1001      123     1809 2023-07-06 22:45:53.000000 granian-0.5.1/tests/test_rsgi.py
--rw-r--r--   0     1001      123     2569 2023-07-06 22:45:53.000000 granian-0.5.1/tests/test_ws.py
--rw-r--r--   0     1001      123     1796 2023-07-06 22:45:53.000000 granian-0.5.1/tests/test_wsgi.py
--rw-r--r--   0     1001      123    30877 2023-07-06 22:45:53.000000 granian-0.5.1/Cargo.lock
--rw-r--r--   0        0        0     7122 1970-01-01 00:00:00.000000 granian-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 granian-0.5.2/Cargo.toml
+-rw-r--r--   0     1001      123     1486 2023-07-18 10:05:47.000000 granian-0.5.2/LICENSE
+-rw-r--r--   0     1001      123     5333 2023-07-18 10:05:47.000000 granian-0.5.2/README.md
+-rw-r--r--   0     1001      123       54 2023-07-18 10:05:47.000000 granian-0.5.2/build.rs
+-rw-r--r--   0     1001      123       28 2023-07-18 10:05:47.000000 granian-0.5.2/granian/__init__.py
+-rw-r--r--   0     1001      123       35 2023-07-18 10:05:47.000000 granian-0.5.2/granian/__main__.py
+-rw-r--r--   0     1001      123       22 2023-07-18 10:05:47.000000 granian-0.5.2/granian/__version__.py
+-rw-r--r--   0     1001      123      261 2023-07-18 10:05:47.000000 granian-0.5.2/granian/_futures.py
+-rw-r--r--   0     1001      123     1836 2023-07-18 10:05:47.000000 granian-0.5.2/granian/_granian.pyi
+-rw-r--r--   0     1001      123     1677 2023-07-18 10:05:47.000000 granian-0.5.2/granian/_internal.py
+-rw-r--r--   0     1001      123     2862 2023-07-18 10:05:47.000000 granian-0.5.2/granian/_loops.py
+-rw-r--r--   0     1001      123       93 2023-07-18 10:05:47.000000 granian-0.5.2/granian/_types.py
+-rw-r--r--   0     1001      123     3893 2023-07-18 10:05:47.000000 granian-0.5.2/granian/asgi.py
+-rw-r--r--   0     1001      123     3774 2023-07-18 10:05:47.000000 granian-0.5.2/granian/cli.py
+-rw-r--r--   0     1001      123      357 2023-07-18 10:05:47.000000 granian-0.5.2/granian/constants.py
+-rw-r--r--   0     1001      123     1328 2023-07-18 10:05:47.000000 granian-0.5.2/granian/log.py
+-rw-r--r--   0     1001      123      153 2023-07-18 10:05:47.000000 granian-0.5.2/granian/net.py
+-rw-r--r--   0     1001      123        0 2023-07-18 10:05:47.000000 granian-0.5.2/granian/py.typed
+-rw-r--r--   0     1001      123      462 2023-07-18 10:05:47.000000 granian-0.5.2/granian/rsgi.py
+-rw-r--r--   0     1001      123    11447 2023-07-18 10:05:47.000000 granian-0.5.2/granian/server.py
+-rw-r--r--   0     1001      123     1382 2023-07-18 10:05:47.000000 granian-0.5.2/granian/wsgi.py
+-rw-r--r--   0     1001      123     1623 2023-07-18 10:05:47.000000 granian-0.5.2/pyproject.toml
+-rw-r--r--   0     1001      123    10636 2023-07-18 10:05:47.000000 granian-0.5.2/src/asgi/callbacks.rs
+-rw-r--r--   0     1001      123     2170 2023-07-18 10:05:47.000000 granian-0.5.2/src/asgi/errors.rs
+-rw-r--r--   0     1001      123     5171 2023-07-18 10:05:47.000000 granian-0.5.2/src/asgi/http.rs
+-rw-r--r--   0     1001      123    15937 2023-07-18 10:05:47.000000 granian-0.5.2/src/asgi/io.rs
+-rw-r--r--   0     1001      123      329 2023-07-18 10:05:47.000000 granian-0.5.2/src/asgi/mod.rs
+-rw-r--r--   0     1001      123     4636 2023-07-18 10:05:47.000000 granian-0.5.2/src/asgi/serve.rs
+-rw-r--r--   0     1001      123     5220 2023-07-18 10:05:47.000000 granian-0.5.2/src/asgi/types.rs
+-rw-r--r--   0     1001      123     9835 2023-07-18 10:05:47.000000 granian-0.5.2/src/callbacks.rs
+-rw-r--r--   0     1001      123      415 2023-07-18 10:05:47.000000 granian-0.5.2/src/http.rs
+-rw-r--r--   0     1001      123      550 2023-07-18 10:05:47.000000 granian-0.5.2/src/lib.rs
+-rw-r--r--   0     1001      123     9755 2023-07-18 10:05:47.000000 granian-0.5.2/src/rsgi/callbacks.rs
+-rw-r--r--   0     1001      123      565 2023-07-18 10:05:47.000000 granian-0.5.2/src/rsgi/errors.rs
+-rw-r--r--   0     1001      123     5591 2023-07-18 10:05:47.000000 granian-0.5.2/src/rsgi/http.rs
+-rw-r--r--   0     1001      123    12300 2023-07-18 10:05:47.000000 granian-0.5.2/src/rsgi/io.rs
+-rw-r--r--   0     1001      123      665 2023-07-18 10:05:47.000000 granian-0.5.2/src/rsgi/mod.rs
+-rw-r--r--   0     1001      123     4635 2023-07-18 10:05:47.000000 granian-0.5.2/src/rsgi/serve.rs
+-rw-r--r--   0     1001      123     5538 2023-07-18 10:05:47.000000 granian-0.5.2/src/rsgi/types.rs
+-rw-r--r--   0     1001      123     7978 2023-07-18 10:05:47.000000 granian-0.5.2/src/runtime.rs
+-rw-r--r--   0     1001      123     4301 2023-07-18 10:05:47.000000 granian-0.5.2/src/tcp.rs
+-rw-r--r--   0     1001      123     2431 2023-07-18 10:05:47.000000 granian-0.5.2/src/tls.rs
+-rw-r--r--   0     1001      123      837 2023-07-18 10:05:47.000000 granian-0.5.2/src/utils.rs
+-rw-r--r--   0     1001      123    16535 2023-07-18 10:05:47.000000 granian-0.5.2/src/workers.rs
+-rw-r--r--   0     1001      123     3435 2023-07-18 10:05:47.000000 granian-0.5.2/src/ws.rs
+-rw-r--r--   0     1001      123     1301 2023-07-18 10:05:47.000000 granian-0.5.2/src/wsgi/callbacks.rs
+-rw-r--r--   0     1001      123     1982 2023-07-18 10:05:47.000000 granian-0.5.2/src/wsgi/http.rs
+-rw-r--r--   0     1001      123      219 2023-07-18 10:05:47.000000 granian-0.5.2/src/wsgi/mod.rs
+-rw-r--r--   0     1001      123     2196 2023-07-18 10:05:47.000000 granian-0.5.2/src/wsgi/serve.rs
+-rw-r--r--   0     1001      123     7829 2023-07-18 10:05:47.000000 granian-0.5.2/src/wsgi/types.rs
+-rw-r--r--   0     1001      123     3078 2023-07-18 10:05:47.000000 granian-0.5.2/tests/apps/asgi.py
+-rw-r--r--   0     1001      123     2739 2023-07-18 10:05:47.000000 granian-0.5.2/tests/apps/rsgi.py
+-rw-r--r--   0     1001      123     1120 2023-07-18 10:05:47.000000 granian-0.5.2/tests/apps/wsgi.py
+-rw-r--r--   0     1001      123     1759 2023-07-18 10:05:47.000000 granian-0.5.2/tests/conftest.py
+-rw-r--r--   0     1001      123     1139 2023-07-18 10:05:47.000000 granian-0.5.2/tests/fixtures/tls/cert.pem
+-rw-r--r--   0     1001      123     1704 2023-07-18 10:05:47.000000 granian-0.5.2/tests/fixtures/tls/key.pem
+-rw-r--r--   0     1001      123     1830 2023-07-18 10:05:47.000000 granian-0.5.2/tests/test_asgi.py
+-rw-r--r--   0     1001      123     1851 2023-07-18 10:05:47.000000 granian-0.5.2/tests/test_https.py
+-rw-r--r--   0     1001      123     1809 2023-07-18 10:05:47.000000 granian-0.5.2/tests/test_rsgi.py
+-rw-r--r--   0     1001      123     2569 2023-07-18 10:05:47.000000 granian-0.5.2/tests/test_ws.py
+-rw-r--r--   0     1001      123     1796 2023-07-18 10:05:47.000000 granian-0.5.2/tests/test_wsgi.py
+-rw-r--r--   0     1001      123    30877 2023-07-18 10:05:47.000000 granian-0.5.2/Cargo.lock
+-rw-r--r--   0        0        0     7122 1970-01-01 00:00:00.000000 granian-0.5.2/PKG-INFO
```

### Comparing `granian-0.5.1/Cargo.toml` & `granian-0.5.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "granian"
-version = "0.5.1"
+version = "0.5.2"
 description = "A Rust HTTP server for Python applications"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 edition = "2021"
 
 keywords = ["web", "asyncio"]
```

### Comparing `granian-0.5.1/LICENSE` & `granian-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/README.md` & `granian-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/granian/_granian.pyi` & `granian-0.5.2/granian/_granian.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 from typing import Any, Dict, List, Tuple, Optional
 
 from ._types import WebsocketMessage
 
 
 class ASGIScope:
-    client_ip: str
-    client_port: int
-    server_ip: str
-    server_port: int
-    http_version: str
-    method: str
-    path: str
-    proto: str
-    query_string: str
-    scheme: str
-
-    @property
-    def headers(self) -> List[Tuple[bytes, bytes]]: ...
+    def as_dict(self, root_path: str) -> Dict[str, Any]: ...
 
 
 class RSGIHeaders:
     def __contains__(self, key: str) -> bool: ...
     def keys(self) -> List[str]: ...
     def values(self) -> List[str]: ...
     def items(self) -> List[Tuple[str]]: ...
@@ -72,15 +60,8 @@
 
 
 class RSGIProtocolClosed(RuntimeError):
     ...
 
 
 class WSGIScope:
-    server: str
-    client: str
-    scheme: str
-    method: str
-    path: str
-    query_string: str
-    headers: Dict[str, str]
-    body: bytes
+    def to_environ(self, environ: Dict[str, Any]) -> Dict[str, Any]: ...
```

### Comparing `granian-0.5.1/granian/_internal.py` & `granian-0.5.2/granian/_internal.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/granian/_loops.py` & `granian-0.5.2/granian/_loops.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/granian/asgi.py` & `granian-0.5.2/granian/asgi.py`

 * *Files 17% similar despite different names*

```diff
@@ -113,29 +113,12 @@
 
 def _callback_wrapper(callback, scope_opts):
     root_url_path = scope_opts.get('url_path_prefix') or ''
 
     @wraps(callback)
     def wrapper(scope: Scope, proto):
         return callback(
-            {
-                "type": scope.proto,
-                "asgi": {
-                    "version": "3.0",
-                    "spec_version": "2.3"
-                },
-                "http_version": scope.http_version,
-                "server": (scope.server_ip, scope.server_port),
-                "client": (scope.client_ip, scope.client_port),
-                "scheme": scope.scheme,
-                "method": scope.method,
-                "root_path": root_url_path,
-                "path": scope.path,
-                "raw_path": scope.path.encode("ascii"),
-                "query_string": scope.query_string.encode('latin-1'),
-                "headers": scope.headers,
-                "extensions": {}
-            },
+            scope.as_dict(root_url_path),
             proto.receive,
             _send_wrapper(proto.send)
         )
     return wrapper
```

### Comparing `granian-0.5.1/granian/cli.py` & `granian-0.5.2/granian/cli.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/granian/log.py` & `granian-0.5.2/granian/log.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/granian/server.py` & `granian-0.5.2/granian/server.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/pyproject.toml` & `granian-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/asgi/callbacks.rs` & `granian-0.5.2/src/asgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/asgi/errors.rs` & `granian-0.5.2/src/asgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/asgi/http.rs` & `granian-0.5.2/src/asgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/asgi/io.rs` & `granian-0.5.2/src/asgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/asgi/serve.rs` & `granian-0.5.2/src/asgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/callbacks.rs` & `granian-0.5.2/src/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/lib.rs` & `granian-0.5.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/rsgi/callbacks.rs` & `granian-0.5.2/src/rsgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/rsgi/errors.rs` & `granian-0.5.2/src/rsgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/rsgi/http.rs` & `granian-0.5.2/src/rsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/rsgi/io.rs` & `granian-0.5.2/src/rsgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/rsgi/mod.rs` & `granian-0.5.2/src/rsgi/mod.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/rsgi/serve.rs` & `granian-0.5.2/src/rsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/rsgi/types.rs` & `granian-0.5.2/src/rsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/runtime.rs` & `granian-0.5.2/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/tcp.rs` & `granian-0.5.2/src/tcp.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/tls.rs` & `granian-0.5.2/src/tls.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/utils.rs` & `granian-0.5.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/workers.rs` & `granian-0.5.2/src/workers.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/ws.rs` & `granian-0.5.2/src/ws.rs`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/src/wsgi/callbacks.rs` & `granian-0.5.2/src/wsgi/callbacks.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,45 @@
 use hyper::Body;
 use pyo3::prelude::*;
 use tokio::task::JoinHandle;
 
 use crate::callbacks::CallbackWrapper;
-use super::{
-    errors::error_proto,
-    types::{WSGIScope as Scope, WSGIResponseBodyIter}
-};
+use super::types::{WSGIScope as Scope, WSGIResponseBodyIter};
 
 const WSGI_LIST_RESPONSE_BODY: i32 = 0;
 const WSGI_ITER_RESPONSE_BODY: i32 = 1;
 
 
-pub(crate) async fn call_rtb_http(
-    cb: CallbackWrapper,
+#[inline(always)]
+fn run_callback(
+    callback: PyObject,
     scope: Scope
 ) -> PyResult<(i32, Vec<(String, String)>, Body)> {
-    let callback = cb.callback.clone();
-
     Python::with_gil(|py| {
         let (status, headers, body_type, pybody) = callback.call1(py, (scope,))?
             .extract::<(i32, Vec<(String, String)>, i32, PyObject)>(py)?;
         let body = match body_type {
             WSGI_LIST_RESPONSE_BODY => Body::from(pybody.extract::<Vec<u8>>(py)?),
             WSGI_ITER_RESPONSE_BODY => Body::wrap_stream(WSGIResponseBodyIter::new(pybody)),
             _ => Body::empty()
         };
         Ok((status, headers, body))
     })
 }
 
-pub(crate) async fn call_rtt_http(
+pub(crate) fn call_rtb_http(
     cb: CallbackWrapper,
     scope: Scope
 ) -> PyResult<(i32, Vec<(String, String)>, Body)> {
+    run_callback(cb.callback.clone(), scope)
+}
+
+pub(crate) fn call_rtt_http(
+    cb: CallbackWrapper,
+    scope: Scope
+) -> JoinHandle<PyResult<(i32, Vec<(String, String)>, Body)>> {
     let callback = cb.callback.clone();
 
-    let fut: JoinHandle<PyResult<(i32, Vec<(String, String)>, Body)>> = tokio::task::spawn_blocking(move || {
-        Python::with_gil(|py| {
-            let (status, headers, body_type, pybody) = callback.call1(py, (scope,))?
-                .extract::<(i32, Vec<(String, String)>, i32, PyObject)>(py)?;
-            let body = match body_type {
-                WSGI_LIST_RESPONSE_BODY => Body::from(pybody.extract::<Vec<u8>>(py)?),
-                WSGI_ITER_RESPONSE_BODY => Body::wrap_stream(WSGIResponseBodyIter::new(pybody)),
-                _ => Body::empty()
-            };
-            Ok((status, headers, body))
-        })
-    });
-
-    match fut.await {
-        Ok(res) => res,
-        _ => {
-            log::error!("WSGI protocol failure");
-            error_proto!()
-        }
-    }
+    tokio::task::spawn_blocking(move || {
+        run_callback(callback, scope)
+    })
 }
```

### Comparing `granian-0.5.1/src/wsgi/http.rs` & `granian-0.5.2/src/wsgi/http.rs`

 * *Files 24% similar despite different names*

```diff
@@ -13,42 +13,63 @@
 };
 use super::{
     callbacks::{call_rtb_http, call_rtt_http},
     types::WSGIScope as Scope
 };
 
 
-macro_rules! handle_request {
-    ($func_name:ident, $handler:expr) => {
-        pub(crate) async fn $func_name(
-            _rt: RuntimeRef,
-            callback: CallbackWrapper,
-            server_addr: SocketAddr,
-            client_addr: SocketAddr,
-            req: Request<Body>,
-            scheme: &str
-        ) -> Response<Body> {
-            match $handler(
-                callback,
-                Scope::new(scheme, server_addr, client_addr, req).await
-            ).await {
-                Ok((status, pyheaders, body)) => {
-                    let mut res = Response::new(body);
-                    *res.status_mut() = hyper::StatusCode::from_u16(status as u16).unwrap();
-                    let headers = res.headers_mut();
-                    headers.insert(HK_SERVER, HV_SERVER);
-                    for (key, val) in pyheaders {
-                        headers.append(
-                            HeaderName::from_bytes(key.as_bytes()).unwrap(),
-                            HeaderValue::from_str(&val).unwrap()
-                        );
-                    }
-                    res
-                },
-                _ => response_500()
-            }
+#[inline(always)]
+fn build_response(status: i32, pyheaders: Vec<(String, String)>, body: Body) -> Response<Body> {
+    let mut res = Response::new(body);
+    *res.status_mut() = hyper::StatusCode::from_u16(status as u16).unwrap();
+    let headers = res.headers_mut();
+    headers.insert(HK_SERVER, HV_SERVER);
+    for (key, val) in pyheaders {
+        headers.append(
+            HeaderName::from_bytes(key.as_bytes()).unwrap(),
+            HeaderValue::from_str(&val).unwrap()
+        );
+    }
+    res
+}
+
+pub(crate) async fn handle_rtt(
+    _rt: RuntimeRef,
+    callback: CallbackWrapper,
+    server_addr: SocketAddr,
+    client_addr: SocketAddr,
+    req: Request<Body>,
+    scheme: &str
+) -> Response<Body> {
+    if let Ok(res) = call_rtt_http(
+        callback,
+        Scope::new(scheme, server_addr, client_addr, req).await
+    ).await {
+        if let Ok((status, headers, body)) = res {
+            return build_response(status, headers, body)
         }
-    };
+        log::warn!("Application callable raised an exception");
+    } else {
+        log::error!("WSGI protocol failure");
+    }
+    response_500()
 }
 
-handle_request!(handle_rtt, call_rtt_http);
-handle_request!(handle_rtb, call_rtb_http);
+pub(crate) async fn handle_rtb(
+    _rt: RuntimeRef,
+    callback: CallbackWrapper,
+    server_addr: SocketAddr,
+    client_addr: SocketAddr,
+    req: Request<Body>,
+    scheme: &str
+) -> Response<Body> {
+    match call_rtb_http(
+        callback,
+        Scope::new(scheme, server_addr, client_addr, req).await
+    ) {
+        Ok((status, headers, body)) => build_response(status, headers, body),
+        _ => {
+            log::warn!("Application callable raised an exception");
+            response_500()
+        }
+    }
+}
```

### Comparing `granian-0.5.1/src/wsgi/serve.rs` & `granian-0.5.2/src/wsgi/serve.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 use pyo3::prelude::*;
 
-use crate::{
-    workers::{
-        WorkerConfig,
-        serve_rth,
-        serve_wth,
-        serve_rth_ssl,
-        serve_wth_ssl
-    }
+use crate::workers::{
+    WorkerConfig,
+    serve_rth,
+    serve_wth,
+    serve_rth_ssl,
+    serve_wth_ssl
 };
 use super::http::{handle_rtb, handle_rtt};
 
 #[pyclass(module="granian._granian")]
 pub struct WSGIWorker {
     config: WorkerConfig
 }
```

### Comparing `granian-0.5.1/src/wsgi/types.rs` & `granian-0.5.2/src/asgi/types.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,178 @@
-use futures::Stream;
-use hyper::{body::Bytes, Body, Method, Request, Uri};
+use hyper::{Uri, Version, header::HeaderMap};
+use once_cell::sync::OnceCell;
 use pyo3::prelude::*;
-use pyo3::types::{PyBytes, PyList};
-use std::{collections::HashMap, net::SocketAddr, task::{Context, Poll}};
+use pyo3::types::{PyBytes, PyDict, PyList, PyString};
+use std::net::{IpAddr, SocketAddr};
 
-const LINE_SPLIT: u8 = u8::from_be_bytes(*b"\n");
 
+const SCHEME_HTTPS: &str = "https";
+const SCHEME_WS: &str = "ws";
+const SCHEME_WSS: &str = "wss";
 
-#[pyclass(module = "granian._granian")]
-pub(crate) struct WSGIBody {
-    inner: Bytes
-}
-
-impl WSGIBody {
-    pub fn new(body: Bytes) -> Self {
-        Self { inner: body }
-    }
-}
-
-#[pymethods]
-impl WSGIBody {
-    fn __iter__(pyself: PyRef<'_, Self>) -> PyRef<'_, Self> {
-        pyself
-    }
-
-    fn __next__<'p>(&mut self, py: Python<'p>) -> Option<&'p PyBytes> {
-        match self.inner.iter().position(|&c| c == LINE_SPLIT) {
-            Some(next_split) => {
-                let bytes = self.inner.split_to(next_split);
-                Some(PyBytes::new(py, &bytes[..]))
-            },
-            _ => None
-        }
-    }
+static ASGI_VERSION: OnceCell<PyObject> = OnceCell::new();
+static ASGI_EXTENSIONS: OnceCell<PyObject> = OnceCell::new();
 
-    #[pyo3(signature = (size=None))]
-    fn read<'p>(&mut self, py: Python<'p>, size: Option<usize>) -> &'p PyBytes {
-        match size {
-            None => {
-                let bytes = self.inner.split_to(self.inner.len());
-                PyBytes::new(py, &bytes[..])
-            },
-            Some(size) => {
-                match size {
-                    0 => PyBytes::new(py, b""),
-                    size => {
-                        let limit = self.inner.len();
-                        let rsize = if size > limit { limit } else { size };
-                        let bytes = self.inner.split_to(rsize);
-                        PyBytes::new(py, &bytes[..])
-                    }
-                }
-            }
-        }
-    }
-
-    fn readline<'p>(&mut self, py: Python<'p>) -> &'p PyBytes {
-        match self.inner.iter().position(|&c| c == LINE_SPLIT) {
-            Some(next_split) => {
-                let bytes = self.inner.split_to(next_split);
-                self.inner = self.inner.slice(1..);
-                PyBytes::new(py, &bytes[..])
-            },
-            _ => PyBytes::new(py, b"")
-        }
-    }
-
-    #[pyo3(signature = (_hint=None))]
-    fn readlines<'p>(&mut self, py: Python<'p>, _hint: Option<PyObject>) -> &'p PyList {
-        let lines: Vec<&PyBytes> = self.inner
-            .split(|&c| c == LINE_SPLIT)
-            .map(|item| PyBytes::new(py, &item[..]))
-            .collect();
-        self.inner.clear();
-        PyList::new(py, lines)
-    }
+pub(crate) enum ASGIMessageType {
+    HTTPStart,
+    HTTPBody,
+    WSAccept,
+    WSClose,
+    WSMessage
 }
 
-#[pyclass(module = "granian._granian")]
-pub(crate) struct WSGIScope {
-    #[pyo3(get)]
+#[pyclass(module="granian._granian")]
+pub(crate) struct ASGIScope {
+    http_version: Version,
     scheme: String,
-    #[pyo3(get)]
     method: String,
     uri: Uri,
-    #[pyo3(get)]
-    server: String,
-    #[pyo3(get)]
-    client: String,
-    #[pyo3(get)]
-    headers: HashMap<String, String>,
-    body: Bytes
+    server_ip: IpAddr,
+    server_port: u16,
+    client_ip: IpAddr,
+    client_port: u16,
+    headers: HeaderMap,
+    is_websocket: bool
 }
 
-impl WSGIScope {
-    pub async fn new(
+impl ASGIScope {
+    pub fn new(
+        http_version: Version,
         scheme: &str,
+        uri: Uri,
+        method: &str,
         server: SocketAddr,
         client: SocketAddr,
-        request: Request<Body>,
+        headers: &HeaderMap
     ) -> Self {
-        let headers = request.headers();
-        let mut pyheaders = HashMap::with_capacity(headers.keys_len());
-        for (key, val) in headers.iter() {
-            pyheaders.insert(
-                format!("HTTP_{}", key.as_str().replace("-", "_").to_uppercase()),
-                val.to_str().unwrap().into(),
-            );
-        }
-
-        let method = request.method().clone();
-        let uri = request.uri().clone();
-
-        let body = match &method {
-            &Method::HEAD | &Method::GET | &Method::OPTIONS => { Bytes::new() },
-            _ => {
-                hyper::body::to_bytes(request)
-                    .await
-                    .unwrap_or(Bytes::new())
-            }
-        };
-
         Self {
+            http_version: http_version,
             scheme: scheme.to_string(),
             method: method.to_string(),
-            uri,
-            server: server.to_string(),
-            client: client.to_string(),
-            headers: pyheaders,
-            body
+            uri: uri,
+            server_ip: server.ip(),
+            server_port: server.port(),
+            client_ip: client.ip(),
+            client_port: client.port(),
+            headers: headers.to_owned(),
+            is_websocket: false
         }
     }
-}
 
-#[pymethods]
-impl WSGIScope {
-    #[getter(path)]
-    fn get_path(&self) -> &str {
-        self.uri.path()
+    pub fn set_websocket(&mut self) {
+        self.is_websocket = true
     }
 
-    #[getter(query_string)]
-    fn get_query_string(&self) -> &str {
-        self.uri.query().unwrap_or("")
+    #[inline(always)]
+    fn py_proto(&self) -> &str {
+        match self.is_websocket {
+            false => "http",
+            true => "websocket"
+        }
     }
 
-    fn input(pyself: PyRef<'_, Self>) -> PyResult<Py<WSGIBody>> {
-        Py::new(pyself.py(), WSGIBody::new(pyself.body.to_owned()))
+    #[inline(always)]
+    fn py_http_version(&self) -> &str {
+        match self.http_version {
+            Version::HTTP_10 => "1",
+            Version::HTTP_11 => "1.1",
+            Version::HTTP_2 => "2",
+            _ => "1"
+        }
     }
-}
 
-pub(crate) struct WSGIResponseBodyIter {
-    inner: PyObject
-}
-
-impl WSGIResponseBodyIter {
-    pub fn new(body: PyObject) -> Self {
-        Self { inner: body }
+    #[inline(always)]
+    fn py_scheme(&self) -> &str {
+        let scheme = &self.scheme[..];
+        match self.is_websocket {
+            false => scheme,
+            true => {
+                match scheme {
+                    SCHEME_HTTPS => SCHEME_WSS,
+                    _ => SCHEME_WS
+                }
+            }
+        }
     }
 
-    fn close_inner(&self, py: Python) {
-        let _ = self.inner.call_method0(py, pyo3::intern!(py, "close"));
+    #[inline(always)]
+    fn py_headers<'p>(&self, py: Python<'p>) -> PyResult<&'p PyList> {
+        let rv = PyList::empty(py);
+        for (key, value) in self.headers.iter() {
+            rv.append((
+                PyBytes::new(py, key.as_str().as_bytes()),
+                PyBytes::new(py, value.as_bytes())
+            ))?;
+        }
+        Ok(rv)
     }
 }
 
-impl Stream for WSGIResponseBodyIter {
-    type Item = PyResult<Vec<u8>>;
-
-    fn poll_next(
-        self: std::pin::Pin<&mut Self>,
-        _cx: &mut Context<'_>
-    ) -> Poll<Option<Self::Item>> {
-        Python::with_gil(|py| {
-            match self.inner.call_method0(py, pyo3::intern!(py, "__next__")) {
-                Ok(chunk_obj) => {
-                    match chunk_obj.extract::<Vec<u8>>(py) {
-                        Ok(chunk) => Poll::Ready(Some(Ok(chunk))),
-                        _ => {
-                            self.close_inner(py);
-                            Poll::Ready(None)
-                        }
-                    }
-                },
-                Err(err) => {
-                    if err.is_instance_of::<pyo3::exceptions::PyStopIteration>(py) {
-                        self.close_inner(py);
-                    }
-                    Poll::Ready(None)
-                }
-            }
-        })
+#[pymethods]
+impl ASGIScope {
+    fn as_dict<'p>(&self, py: Python<'p>, url_path_prefix: &'p str) -> PyResult<&'p PyAny> {
+        let (
+            path,
+            query_string,
+            proto,
+            http_version,
+            server,
+            client,
+            scheme,
+            method
+        ) = py.allow_threads(|| {
+            let (path, query_string) = self.uri.path_and_query()
+                .map_or_else(|| ("", ""), |pq| (pq.path(), pq.query().unwrap_or("")));
+            (
+                path,
+                query_string,
+                self.py_proto(),
+                self.py_http_version(),
+                (self.server_ip.to_string(), self.server_port),
+                (self.client_ip.to_string(), self.client_port),
+                self.py_scheme(),
+                &self.method[..],
+            )
+        });
+        let dict: &PyDict = PyDict::new(py);
+        dict.set_item(
+            pyo3::intern!(py, "asgi"),
+            ASGI_VERSION.get_or_try_init(|| {
+                let rv = PyDict::new(py);
+                rv.set_item("version", "3.0")?;
+                rv.set_item("spec_version", "2.3")?;
+                Ok::<PyObject, PyErr>(rv.into())
+            })?.as_ref(py)
+        )?;
+        dict.set_item(
+            pyo3::intern!(py, "extensions"),
+            ASGI_EXTENSIONS.get_or_try_init(|| {
+                let rv = PyDict::new(py);
+                Ok::<PyObject, PyErr>(rv.into())
+            })?.as_ref(py)
+        )?;
+        dict.set_item(pyo3::intern!(py, "type"), proto)?;
+        dict.set_item(pyo3::intern!(py, "http_version"), http_version)?;
+        dict.set_item(pyo3::intern!(py, "server"), server)?;
+        dict.set_item(pyo3::intern!(py, "client"), client)?;
+        dict.set_item(pyo3::intern!(py, "scheme"), scheme)?;
+        dict.set_item(pyo3::intern!(py, "method"), method)?;
+        dict.set_item(pyo3::intern!(py, "root_path"), url_path_prefix)?;
+        dict.set_item(pyo3::intern!(py, "path"), path)?;
+        dict.set_item(
+            pyo3::intern!(py, "raw_path"),
+            PyString::new(py, path)
+                .call_method1(
+                    pyo3::intern!(py, "encode"), (pyo3::intern!(py, "ascii"),)
+                )?
+        )?;
+        dict.set_item(
+            pyo3::intern!(py, "query_string"),
+            PyString::new(py, query_string)
+                .call_method1(
+                    pyo3::intern!(py, "encode"), (pyo3::intern!(py, "latin-1"),)
+                )?
+        )?;
+        dict.set_item(pyo3::intern!(py, "headers"), self.py_headers(py)?)?;
+        Ok(dict)
     }
 }
```

### Comparing `granian-0.5.1/tests/apps/asgi.py` & `granian-0.5.2/tests/apps/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/tests/apps/rsgi.py` & `granian-0.5.2/tests/apps/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/tests/apps/wsgi.py` & `granian-0.5.2/tests/apps/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/tests/conftest.py` & `granian-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/tests/fixtures/tls/cert.pem` & `granian-0.5.2/tests/fixtures/tls/cert.pem`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/tests/fixtures/tls/key.pem` & `granian-0.5.2/tests/fixtures/tls/key.pem`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/tests/test_asgi.py` & `granian-0.5.2/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/tests/test_https.py` & `granian-0.5.2/tests/test_https.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/tests/test_rsgi.py` & `granian-0.5.2/tests/test_rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/tests/test_ws.py` & `granian-0.5.2/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/tests/test_wsgi.py` & `granian-0.5.2/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.5.1/Cargo.lock` & `granian-0.5.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "granian"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
  "bytes",
  "futures",
  "hyper",
  "log",
  "mimalloc",
  "once_cell",
```

### Comparing `granian-0.5.1/PKG-INFO` & `granian-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granian
-Version: 0.5.1
+Version: 0.5.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

