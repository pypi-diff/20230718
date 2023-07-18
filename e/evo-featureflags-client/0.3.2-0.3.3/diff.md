# Comparing `tmp/evo-featureflags-client-0.3.2.tar.gz` & `tmp/evo-featureflags-client-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/evo-featureflags-client-0.3.2.tar", last modified: Fri Feb 11 10:18:19 2022, max compression
+gzip compressed data, was "evo-featureflags-client-0.3.3.tar", last modified: Tue Jul 18 14:14:39 2023, max compression
```

## Comparing `evo-featureflags-client-0.3.2.tar` & `evo-featureflags-client-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/evo_featureflags_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/evo_featureflags_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/evo_featureflags_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/evo_featureflags_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/evo_featureflags_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/evo_featureflags_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/featureflags/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/featureflags/client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/client/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     5361 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/client/conditions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6278 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/client/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/featureflags/client/managers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/client/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3939 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/client/managers/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/client/managers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/client/managers/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/client/state.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/featureflags/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-11 10:18:19.000000 evo-featureflags-client-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-02-11 10:18:11.000000 evo-featureflags-client-0.3.2/setup.py
+-rw-r--r--   0        0        0       56 2023-07-18 14:14:17.778050 evo-featureflags-client-0.3.3/featureflags/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 14:14:17.778050 evo-featureflags-client-0.3.3/featureflags/client/__init__.py
+-rw-r--r--   0        0        0      567 2023-07-18 14:14:17.778050 evo-featureflags-client-0.3.3/featureflags/client/compat.py
+-rw-r--r--   0        0        0     5361 2023-07-18 14:14:17.778050 evo-featureflags-client-0.3.3/featureflags/client/conditions.py
+-rw-r--r--   0        0        0     6942 2023-07-18 14:14:17.778050 evo-featureflags-client-0.3.3/featureflags/client/flags.py
+-rw-r--r--   0        0        0        0 2023-07-18 14:14:17.778050 evo-featureflags-client-0.3.3/featureflags/client/managers/__init__.py
+-rw-r--r--   0        0        0     4561 2023-07-18 14:14:17.778050 evo-featureflags-client-0.3.3/featureflags/client/managers/asyncio.py
+-rw-r--r--   0        0        0      541 2023-07-18 14:14:17.778050 evo-featureflags-client-0.3.3/featureflags/client/managers/dummy.py
+-rw-r--r--   0        0        0     3156 2023-07-18 14:14:17.778050 evo-featureflags-client-0.3.3/featureflags/client/managers/sync.py
+-rw-r--r--   0        0        0     1776 2023-07-18 14:14:17.778050 evo-featureflags-client-0.3.3/featureflags/client/state.py
+-rw-r--r--   0        0        0      420 2023-07-18 14:14:17.782050 evo-featureflags-client-0.3.3/featureflags/client/utils.py
+-rw-r--r--   0        0        0      862 2023-07-18 14:14:17.782050 evo-featureflags-client-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      519 2023-07-18 14:14:17.782050 evo-featureflags-client-0.3.3/tests/conftest.py
+-rw-r--r--   0        0        0     7758 2023-07-18 14:14:17.782050 evo-featureflags-client-0.3.3/tests/test_conditions.py
+-rw-r--r--   0        0        0     6174 2023-07-18 14:14:17.782050 evo-featureflags-client-0.3.3/tests/test_flags.py
+-rw-r--r--   0        0        0     2983 2023-07-18 14:14:17.782050 evo-featureflags-client-0.3.3/tests/test_managers_asyncio.py
+-rw-r--r--   0        0        0      314 2023-07-18 14:14:17.782050 evo-featureflags-client-0.3.3/tests/test_managers_dummy.py
+-rw-r--r--   0        0        0     1396 2023-07-18 14:14:17.782050 evo-featureflags-client-0.3.3/tests/test_utils.py
+-rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 evo-featureflags-client-0.3.3/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `evo-featureflags-client-0.3.2/featureflags/client/compat.py` & `evo-featureflags-client-0.3.3/featureflags/client/compat.py`

 * *Files identical despite different names*

### Comparing `evo-featureflags-client-0.3.2/featureflags/client/conditions.py` & `evo-featureflags-client-0.3.3/featureflags/client/conditions.py`

 * *Files identical despite different names*

### Comparing `evo-featureflags-client-0.3.2/featureflags/client/flags.py` & `evo-featureflags-client-0.3.3/featureflags/client/flags.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,23 @@
                 interval_pb.FromDatetime(interval)
                 stats.append(FlagUsage(
                     name=flag_name, interval=interval_pb,
                     negative_count=neg_count, positive_count=pos_count,
                 ))
         return stats
 
+    @staticmethod
+    def from_defaults(defaults):
+        interval_pb = Timestamp()
+        interval_pb.FromDatetime(datetime.utcnow())
+        return [
+            FlagUsage(name=name, interval=interval_pb, positive_count=0, negative_count=0)
+            for name in defaults
+        ]
+
 
 class Tracer:
     """
     Accumulates request/flag/values
     """
     values = None
     interval = None
@@ -212,7 +221,16 @@
         try:
             with Tracer() as tracer:
                 yield Flags(self._defaults, self._manager, tracer, ctx,
                             overrides)
         finally:
             if tracer is not None:
                 self._manager.add_trace(tracer)
+
+    def preload(self, timeout=None):
+        """Preload flags from server.
+        This method syncs all flags with server"""
+        self._manager.preload(timeout=timeout, defaults=self._defaults)
+
+    async def preload_async(self, timeout=None):
+        """Async version of `preload` method"""
+        await self._manager.preload(timeout=timeout, defaults=self._defaults)
```

### Comparing `evo-featureflags-client-0.3.2/featureflags/client/managers/asyncio.py` & `evo-featureflags-client-0.3.3/featureflags/client/managers/asyncio.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,16 +62,28 @@
         if loop:
             warnings.warn(
                 "The loop arguments is deprecated because it's not necessary.",
                 DeprecationWarning,
                 stacklevel=2,
             )
 
-    async def preload(self, *, timeout=None):
-        await self._exchange(timeout)
+    async def preload(self, *, timeout=None, defaults=None):
+        """
+        Preload flags from the server.
+        :param timeout: timeout in seconds (for grpclib)
+        :param defaults: dict with default values for feature flags.
+                         If passed, all feature flags will be synced with server,
+                         otherwise flags will be synced only when they are accessed
+                         for the first time.
+        """
+        stats = None
+        if defaults is not None:
+            stats = self._stats.from_defaults(defaults)
+
+        await self._exchange(timeout, stats)
 
     def start(self):
         if self._exchange_task is not None:
             raise RuntimeError('Manager is already started')
         self._exchange_task = self._loop.create_task(self._exchange_coro())
 
     def close(self):
@@ -101,16 +113,19 @@
                 break
             except Exception as exc:
                 interval = self._int_gen.send(False)
                 log.error('Failed to exchange: %r, retry in %ss', exc, interval)
                 await asyncio.sleep(interval)
                 continue
 
-    async def _exchange(self, timeout):
-        request = self._state.get_request(self._stats.flush())
+    async def _exchange(self, timeout, flags_usage=None):
+        if flags_usage is None:
+            flags_usage = self._stats.flush()
+
+        request = self._state.get_request(flags_usage)
         log.debug('Exchange request, project: %r, version: %r, stats: %r',
                   request.project, request.version, request.flags_usage)
         reply = await self._stub.Exchange(request, timeout=timeout)
         log.debug('Exchange reply: %r', reply)
         self._state.apply_reply(reply)
 
     def get(self, name):
```

### Comparing `evo-featureflags-client-0.3.2/featureflags/client/managers/dummy.py` & `evo-featureflags-client-0.3.3/featureflags/client/managers/dummy.py`

 * *Files identical despite different names*

### Comparing `evo-featureflags-client-0.3.2/featureflags/client/managers/sync.py` & `evo-featureflags-client-0.3.3/featureflags/client/managers/sync.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,19 +42,34 @@
         self._stats = StatsCollector()
         self._stub = FeatureFlagsStub(channel)
 
         self._int_gen = intervals_gen()
         self._int_gen.send(None)
         self._next_exchange = datetime.utcnow()
 
-    def preload(self, timeout=None):
-        self._exchange(timeout)
+    def preload(self, timeout=None, defaults=None):
+        """
+        Preload flags from the server.
+        :param timeout: timeout in seconds (for grpcio)
+        :param defaults: dict with default values for feature flags.
+                         If passed, all feature flags will be synced with server,
+                         otherwise flags will be synced only when they are accessed
+                         for the first time.
+        """
+        stats = None
+        if defaults is not None:
+            stats = self._stats.from_defaults(defaults)
 
-    def _exchange(self, timeout):
-        request = self._state.get_request(self._stats.flush())
+        self._exchange(timeout, stats)
+
+    def _exchange(self, timeout, flags_usage=None):
+        if flags_usage is None:
+            flags_usage = self._stats.flush()
+
+        request = self._state.get_request(flags_usage)
         log.debug('Exchange request, project: %r, version: %r, stats: %r',
                   request.project, request.version, request.flags_usage)
         reply = self._stub.Exchange(request, timeout=timeout)
         log.debug('Exchange reply: %r', reply)
         self._state.apply_reply(reply)
 
     def get(self, name):
```

### Comparing `evo-featureflags-client-0.3.2/featureflags/client/state.py` & `evo-featureflags-client-0.3.3/featureflags/client/state.py`

 * *Files identical despite different names*

