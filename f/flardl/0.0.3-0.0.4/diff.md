# Comparing `tmp/flardl-0.0.3.tar.gz` & `tmp/flardl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flardl-0.0.3.tar", max compression
+gzip compressed data, was "flardl-0.0.4.tar", max compression
```

## Comparing `flardl-0.0.3.tar` & `flardl-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1958 2023-07-11 15:17:41.761070 flardl-0.0.3/LICENSE
--rw-r--r--   0        0        0      243 2023-07-11 15:17:41.761070 flardl-0.0.3/LICENSE.logo.txt
--rw-r--r--   0        0        0     5376 2023-07-11 15:17:41.761070 flardl-0.0.3/README.md
--rw-r--r--   0        0        0     2762 2023-07-11 15:17:54.413354 flardl-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      624 2023-07-11 15:17:41.765070 flardl-0.0.3/src/flardl/__init__.py
--rw-r--r--   0        0        0     3380 2023-07-11 15:17:41.765070 flardl-0.0.3/src/flardl/common.py
--rw-r--r--   0        0        0     1581 2023-07-11 15:17:41.765070 flardl-0.0.3/src/flardl/dict_to_indexed_list.py
--rwxr-xr-x   0        0        0     8126 2023-07-11 15:17:54.413354 flardl-0.0.3/src/flardl/downloader.py
--rwxr-xr-x   0        0        0     4225 2023-07-11 15:17:41.769070 flardl-0.0.3/src/flardl/instrumented_streams.py
--rwxr-xr-x   0        0        0     7146 2023-07-11 15:17:54.413354 flardl-0.0.3/src/flardl/multidispatcher.py
--rw-r--r--   0        0        0        0 2023-07-11 15:17:41.769070 flardl-0.0.3/src/flardl/py.typed
--rwxr-xr-x   0        0        0    11622 2023-07-11 15:17:41.769070 flardl-0.0.3/src/flardl/stream_stats.py
--rw-r--r--   0        0        0     6716 1970-01-01 00:00:00.000000 flardl-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1958 2023-07-17 23:01:11.854476 flardl-0.0.4/LICENSE
+-rw-r--r--   0        0        0      243 2023-07-17 23:01:11.854476 flardl-0.0.4/LICENSE.logo.txt
+-rw-r--r--   0        0        0     5376 2023-07-17 23:01:11.854476 flardl-0.0.4/README.md
+-rw-r--r--   0        0        0     2762 2023-07-17 23:01:24.174634 flardl-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      673 2023-07-17 23:01:24.174634 flardl-0.0.4/src/flardl/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-17 23:01:11.858476 flardl-0.0.4/src/flardl/common.py
+-rw-r--r--   0        0        0     1581 2023-07-17 23:01:11.858476 flardl-0.0.4/src/flardl/dict_to_indexed_list.py
+-rwxr-xr-x   0        0        0     8195 2023-07-17 23:01:24.174634 flardl-0.0.4/src/flardl/downloader.py
+-rwxr-xr-x   0        0        0     4225 2023-07-17 23:01:11.858476 flardl-0.0.4/src/flardl/instrumented_streams.py
+-rwxr-xr-x   0        0        0     7304 2023-07-17 23:01:24.174634 flardl-0.0.4/src/flardl/multidispatcher.py
+-rw-r--r--   0        0        0        0 2023-07-17 23:01:11.858476 flardl-0.0.4/src/flardl/py.typed
+-rw-r--r--   0        0        0      613 2023-07-17 23:01:24.174634 flardl-0.0.4/src/flardl/server_defs.py
+-rwxr-xr-x   0        0        0    11622 2023-07-17 23:01:11.858476 flardl-0.0.4/src/flardl/stream_stats.py
+-rw-r--r--   0        0        0     6716 1970-01-01 00:00:00.000000 flardl-0.0.4/PKG-INFO
```

### Comparing `flardl-0.0.3/LICENSE` & `flardl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flardl-0.0.3/README.md` & `flardl-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `flardl-0.0.3/pyproject.toml` & `flardl-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flardl"
-version = "0.0.3"
+version = "0.0.4"
 description = "Flardl"
 authors = ["Joel Berendzen <joel@generisbio.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/hydrationdynamics/flardl"
 repository = "https://github.com/hydrationdynamics/flardl"
 documentation = "https://flardl.readthedocs.io"
```

### Comparing `flardl-0.0.3/src/flardl/__init__.py` & `flardl-0.0.4/src/flardl/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,9 +7,10 @@
 from .common import MAX  # noqa: F401
 from .common import MIN  # noqa: F401
 from .common import NOBS  # noqa: F401
 from .common import RAVG  # noqa: F401
 from .common import SUM  # noqa: F401
 from .common import VALUE  # noqa: F401
 from .multidispatcher import MultiDispatcher  # noqa: F401
+from .server_defs import ServerDef  # noqa: F401
 from .stream_stats import StreamStats  # noqa: F401
 from .stream_stats import WorkerStat  # noqa: F401
```

### Comparing `flardl-0.0.3/src/flardl/common.py` & `flardl-0.0.4/src/flardl/common.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.3/src/flardl/dict_to_indexed_list.py` & `flardl-0.0.4/src/flardl/dict_to_indexed_list.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.3/src/flardl/downloader.py` & `flardl-0.0.4/src/flardl/downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -204,22 +204,25 @@
 
     LAUNCH_RATE_MAX = 100.0
     TIME_ROUND = 4
 
     def __init__(
         self,
         *args,
-        server: str = "",
-        dir: str = "",
-        transport: str = "https",
-        transport_ver: str = "1",
-        **kwargs,
+        server: str,
+        dir: str,
+        transport: str,
+        transport_ver: str,
+        bw_limit_mbps: float,
+        queue_depth: int,
+        timeout_ms: float,
+        **super_kwargs,
     ):
         """Init with id number."""
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, **super_kwargs)
         self.hard_exceptions: tuple[()] | tuple[type[BaseException]] = (ValueError,)
         self.soft_exceptions: tuple[()] | tuple[type[BaseException]] = (
             ConnectionError,
         )
         self.launch_rate = self.LAUNCH_RATE_MAX
         self.base_url = transport + "://" + server + "/"
         if dir != "":
```

### Comparing `flardl-0.0.3/src/flardl/instrumented_streams.py` & `flardl-0.0.4/src/flardl/instrumented_streams.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.3/src/flardl/multidispatcher.py` & `flardl-0.0.4/src/flardl/multidispatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-"""Work is dispatched to multiple workers and results collected via AnyIO streams."""
+"""Dispatch work to multiple workers and collect results via AnyIO streams."""
 from __future__ import annotations
 
 import sys
 from typing import Any
-from typing import Optional
 
 # third-party imports
 import anyio
 import loguru
 from loguru import logger as mylogger
 
 from .common import DEFAULT_MAX_RETRIES
@@ -17,70 +16,82 @@
 from .dict_to_indexed_list import NonStringIterable
 from .dict_to_indexed_list import zip_dict_to_indexed_list
 from .downloader import Downloader
 from .downloader import MockDownloader
 from .instrumented_streams import ArgumentStream
 from .instrumented_streams import FailureStream
 from .instrumented_streams import ResultStream
+from .server_defs import ServerDef
 from .stream_stats import StreamStats
 
 
 class MultiDispatcher:
     """Runs multiple single-site dispatchers sharing streams."""
 
     def __init__(  # noqa: C901
         self,
-        all_worker_defs: list[dict[str, Any]],
+        all_worker_defs: list[ServerDef],
         /,
         worker_list: list[str] | None = None,
         max_retries: int = DEFAULT_MAX_RETRIES,
         logger: loguru.Logger | None = None,
         quiet: bool = False,
         history_len: int = 0,
         output_dir: str | None = None,
         mock: bool = False,
+        runner: str = "production",
     ) -> None:
         """Save list of dispatchers."""
         if logger is None:
             self._logger = mylogger
         else:
             self._logger = logger
-        all_worker_names = [w["name"] for w in all_worker_defs]
+        all_worker_names = [w.name for w in all_worker_defs]
         if worker_list is None:
             worker_defs = all_worker_defs
         else:
             worker_defs = []
             for worker_name in worker_list:
                 try:
                     worker_idx = all_worker_names.index(worker_name)
                 except ValueError:
                     self._logger.error(f"Worker name {worker_name} not found.")
                     sys.exit(1)
                 worker_defs.append(all_worker_defs[worker_idx])
         self.workers = []
+        worker_factory: type[MockDownloader | Downloader] = Downloader
         if mock:
             worker_factory = MockDownloader
-        else:
-            worker_factory = Downloader
         for i, worker_def in enumerate(worker_defs):
             try:
                 worker = worker_factory(
-                    i, self._logger, output_dir, quiet, **worker_def
+                    i, self._logger, output_dir, quiet, **worker_def.get_all()  # type: ignore
                 )
             except Exception as e:
-                self._logger.warning(
-                    f"Worker {worker_def['name']} failed to initialize."
-                )
+                self._logger.warning(f"Worker {worker_def.name} failed to initialize.")
                 self._logger.warning(e)
                 continue
             self.workers.append(worker)
         if len(self.workers) == 0:
             self._logger.error("No valid workers found.")
             sys.exit(1)
         self.max_retries = max_retries
+        self.backend_options = {}
+        if runner == "production":
+            self.backend = "asyncio"
+            if sys.platform != "win32":
+                self.backend_options = {"use_uvloop": True}
+        elif runner == "testing":
+            self.backend = "asyncio"
+            # asyncio.set_event_loop_policy(DeterministicEventLoopPolicy())
+        elif runner == "trio":
+            self.backend = "trio"
+        else:
+            self._logger.error(f"Unknown runner configuration {runner}")
+            sys.exit(1)
         self.exception_counter: dict[int, int] = {}
         self.n_too_many_retries = 0
         self.n_exceptions = 0
         self.quiet = quiet
         self.queue_stats = StreamStats(all_worker_names, history_len=history_len)
         self._lock = anyio.Lock()
         self.inflight: dict[str, SIMPLE_TYPES] = {}
@@ -165,25 +176,19 @@
                     idx, worker.name, worker_count, e, failure_q
                 )
             except Exception as e:
                 # unhandled errors go to unhandled exception handler
                 idx = kwargs[INDEX_KEY]
                 await worker.unhandled_exception_handler(idx, e)
 
-    def main(self, arg_list: list[dict[str, SIMPLE_TYPES]], config: str = "production"):
+    def main(
+        self,
+        arg_list: list[dict[str, SIMPLE_TYPES]]
+        | dict[str, NonStringIterable | SIMPLE_TYPES],
+    ):
         """Start the multidispatcher queue."""
-        backend_options = {}
-        if config == "production":
-            backend = "asyncio"
-            if sys.platform != "win32":
-                backend_options = {"use_uvloop": True}
-        elif config == "testing":
-            backend = "asyncio"
-            # asyncio.set_event_loop_policy(DeterministicEventLoopPolicy())
-        elif config == "trio":
-            backend = "trio"
-        else:
-            self._logger.error(f"Unknown configuration {config}")
-            sys.exit(1)
         return anyio.run(
-            self.run, arg_list, backend=backend, backend_options=backend_options
+            self.run,
+            arg_list,
+            backend=self.backend,
+            backend_options=self.backend_options,
         )
```

### Comparing `flardl-0.0.3/src/flardl/stream_stats.py` & `flardl-0.0.4/src/flardl/stream_stats.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.3/PKG-INFO` & `flardl-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flardl
-Version: 0.0.3
+Version: 0.0.4
 Summary: Flardl
 Home-page: https://github.com/hydrationdynamics/flardl
 License: BSD-3-Clause
 Keywords: downloads,adaptive,federated
 Author: Joel Berendzen
 Author-email: joel@generisbio.com
 Requires-Python: >=3.9,<4
```

