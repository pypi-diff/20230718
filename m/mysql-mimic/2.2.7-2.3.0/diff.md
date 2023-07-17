# Comparing `tmp/mysql-mimic-2.2.7.tar.gz` & `tmp/mysql-mimic-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-mimic-2.2.7.tar", last modified: Mon Jul 17 18:24:14 2023, max compression
+gzip compressed data, was "mysql-mimic-2.3.0.tar", last modified: Mon Jul 17 22:38:55 2023, max compression
```

## Comparing `mysql-mimic-2.2.7.tar` & `mysql-mimic-2.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/mysql_mimic/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/charset.py
--rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/intercept.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/prepared.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/mysql_mimic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/mysql_mimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-17 18:24:14.000000 mysql-mimic-2.2.7/mysql_mimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-17 18:24:14.000000 mysql-mimic-2.2.7/mysql_mimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:24:14.000000 mysql-mimic-2.2.7/mysql_mimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-17 18:24:14.000000 mysql-mimic-2.2.7/mysql_mimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 18:24:14.000000 mysql-mimic-2.2.7/mysql_mimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:24:14.131451 mysql-mimic-2.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-17 18:23:45.000000 mysql-mimic-2.2.7/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:55.820597 mysql-mimic-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-17 22:38:55.820597 mysql-mimic-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:55.816597 mysql-mimic-2.3.0/mysql_mimic/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/charset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19029 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/mysql_mimic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:55.816597 mysql-mimic-2.3.0/mysql_mimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-17 22:38:55.000000 mysql-mimic-2.3.0/mysql_mimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-17 22:38:55.000000 mysql-mimic-2.3.0/mysql_mimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:38:55.000000 mysql-mimic-2.3.0/mysql_mimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-17 22:38:55.000000 mysql-mimic-2.3.0/mysql_mimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 22:38:55.000000 mysql-mimic-2.3.0/mysql_mimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:38:55.820597 mysql-mimic-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:55.820597 mysql-mimic-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-17 22:38:15.000000 mysql-mimic-2.3.0/tests/test_version.py
```

### Comparing `mysql-mimic-2.2.7/LICENSE` & `mysql-mimic-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/PKG-INFO` & `mysql-mimic-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.7
+Version: 2.3.0
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.7/README.md` & `mysql-mimic-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/auth.py` & `mysql-mimic-2.3.0/mysql_mimic/auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/charset.py` & `mysql-mimic-2.3.0/mysql_mimic/charset.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/connection.py` & `mysql-mimic-2.3.0/mysql_mimic/connection.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/constants.py` & `mysql-mimic-2.3.0/mysql_mimic/constants.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/errors.py` & `mysql-mimic-2.3.0/mysql_mimic/errors.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/intercept.py` & `mysql-mimic-2.3.0/mysql_mimic/intercept.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/packets.py` & `mysql-mimic-2.3.0/mysql_mimic/packets.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/results.py` & `mysql-mimic-2.3.0/mysql_mimic/results.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/schema.py` & `mysql-mimic-2.3.0/mysql_mimic/schema.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/server.py` & `mysql-mimic-2.3.0/mysql_mimic/server.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/session.py` & `mysql-mimic-2.3.0/mysql_mimic/session.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
-from contextlib import contextmanager
+from dataclasses import dataclass
 from datetime import datetime, timezone as timezone_
 from typing import (
     Dict,
     List,
     TYPE_CHECKING,
     Optional,
     Callable,
     Awaitable,
     Type,
     Any,
-    Iterator,
 )
 
 from sqlglot import Dialect
 from sqlglot.dialects import MySQL
 from sqlglot import expressions as exp
 from sqlglot.executor import execute
 
@@ -43,15 +42,62 @@
     parse_timezone,
 )
 from mysql_mimic.results import AllowedResult
 
 if TYPE_CHECKING:
     from mysql_mimic.connection import Connection
 
-    Interceptor = Callable[[exp.Expression], Awaitable[AllowedResult]]
+
+Middleware = Callable[["Query"], Awaitable[AllowedResult]]
+
+
+@dataclass
+class Query:
+    """
+    Convenience class that wraps the parameters to middleware.
+
+    Args:
+        expression: current query expression
+        sql: the original SQL sent by the client
+        attrs: query attributes
+        _middlewares: subsequent middleware functions
+        _query: the ultimate query method
+    """
+
+    expression: exp.Expression
+    sql: str
+    attrs: Dict[str, str]
+    _middlewares: list[Middleware]
+    _query: Callable[[exp.Expression, str, dict[str, str]], Awaitable[AllowedResult]]
+
+    async def next(self) -> AllowedResult:
+        """
+        Call the next middleware in the chain of middlewares.
+
+        Returns:
+            The final query result.
+        """
+        if not self._middlewares:
+            return await self._query(self.expression, self.sql, self.attrs)
+        q = Query(
+            expression=self.expression,
+            sql=self.sql,
+            attrs=self.attrs,
+            _middlewares=self._middlewares[1:],
+            _query=self._query,
+        )
+        return await self._middlewares[0](q)
+
+    async def start(self) -> AllowedResult:
+        """
+        Start the middleware chain.
+
+        This should only be called by the framework code
+        """
+        return await self._middlewares[0](self)
 
 
 class BaseSession:
     """
     Session interface.
 
     This defines what the Connection object depends on.
@@ -116,25 +162,26 @@
     """
 
     dialect: Type[Dialect] = MySQL
 
     def __init__(self, variables: Variables | None = None):
         self.variables = variables or SessionVariables(GlobalVariables())
 
-        # Query interceptors.
-        # If any of these return a non-None value, the query will be cut short.
-        self.interceptors: list[Interceptor] = [
-            self._replace_variables_interceptor,
-            self._set_interceptor,
-            self._static_query_interceptor,
-            self._use_interceptor,
-            self._show_interceptor,
-            self._describe_interceptor,
-            self._rollback_interceptor,
-            self._info_schema_interceptor,
+        # Query middlewares.
+        # These allow queries to be intercepted or wrapped.
+        self.middlewares: list[Middleware] = [
+            self._set_var_middleware,
+            self._replace_variables_middleware,
+            self._set_middleware,
+            self._static_query_middleware,
+            self._use_middleware,
+            self._show_middleware,
+            self._describe_middleware,
+            self._rollback_middleware,
+            self._info_schema_middleware,
         ]
 
         # Information functions.
         # These will be replaced in the AST with their corresponding values.
         self._functions = {
             "CONNECTION_ID": lambda: self.connection.connection_id,
             "USER": lambda: self.variables.get("external_user"),
@@ -237,36 +284,38 @@
 
     async def handle_query(self, sql: str, attrs: Dict[str, str]) -> AllowedResult:
         self.timestamp = datetime.now(tz=self.timezone())
         result = None
         for expression in self._parse(sql):
             if not expression:
                 continue
-            with self._set_var_hint(expression):
-                result = await self._intercept(expression, sql, attrs)
-                if result is None:
-                    result = await self.query(expression, sql, attrs)
+            q = Query(
+                expression=expression,
+                sql=sql,
+                attrs=attrs,
+                _middlewares=self.middlewares,
+                _query=self.query,
+            )
+            result = await q.start()
         return result
 
     async def use(self, database: str) -> None:
         self.database = database
 
     def _parse(self, sql: str) -> List[exp.Expression]:
         return [e for e in self.dialect().parse(sql) if e]
 
     async def _query_info_schema(self, expression: exp.Expression) -> AllowedResult:
         return await ensure_info_schema(await self.schema()).query(expression)
 
-    @contextmanager
-    def _set_var_hint(self, expression: exp.Expression) -> Iterator[None]:
+    async def _set_var_middleware(self, q: Query) -> AllowedResult:
         """Handles any SET_VAR hints, which set system variables for a single statement"""
-        hint = expression.args.get("hint")
+        hint = q.expression.args.get("hint")
         if not hint:
-            yield
-            return
+            return await q.next()
 
         set_var_hint = None
         assignments = {}
         for e in hint.expressions:
             if isinstance(e, exp.Func) and e.name == "SET_VAR":
                 set_var_hint = e
                 for eq in e.expressions:
@@ -279,71 +328,60 @@
         if not hint.expressions:
             hint.pop()
 
         orig = {k: self.variables.get(k) for k in assignments}
         try:
             for k, v in assignments.items():
                 self.variables.set(k, v)
-            yield
+            return await q.next()
         finally:
             for k, v in orig.items():
                 self.variables.set(k, v)
 
-    async def _intercept(
-        self, expression: exp.Expression, sql: str, attrs: Dict[str, str]
-    ) -> AllowedResult:
-        """Run all the query interceptors."""
-        for interceptor in self.interceptors:
-            result = await interceptor(expression)
-            if result is not None:
-                return result
-        return None
-
-    async def _use_interceptor(self, expression: exp.Expression) -> AllowedResult:
+    async def _use_middleware(self, q: Query) -> AllowedResult:
         """Intercept USE statements"""
-        if isinstance(expression, exp.Use):
-            await self.use(expression.this.name)
+        if isinstance(q.expression, exp.Use):
+            await self.use(q.expression.this.name)
             return [], []
-        return None
+        return await q.next()
 
-    async def _show_interceptor(self, expression: exp.Expression) -> AllowedResult:
+    async def _show_middleware(self, q: Query) -> AllowedResult:
         """Intercept SHOW statements"""
-        if isinstance(expression, exp.Show):
-            kind = expression.name.upper()
-            if kind == "VARIABLES":
-                return self._show_variables(expression)
-            if kind == "STATUS":
-                return self._show_status(expression)
-            if kind == "WARNINGS":
-                return self._show_warnings(expression)
-            if kind == "ERRORS":
-                return self._show_errors(expression)
-            select = show_statement_to_info_schema_query(expression, self.database)
-            return await self._query_info_schema(select)
-        return None
+        if isinstance(q.expression, exp.Show):
+            return await self._show(q.expression)
+        return await q.next()
+
+    async def _show(self, expression: exp.Show) -> AllowedResult:
+        kind = expression.name.upper()
+        if kind == "VARIABLES":
+            return self._show_variables(expression)
+        if kind == "STATUS":
+            return self._show_status(expression)
+        if kind == "WARNINGS":
+            return self._show_warnings(expression)
+        if kind == "ERRORS":
+            return self._show_errors(expression)
+        select = show_statement_to_info_schema_query(expression, self.database)
+        return await self._query_info_schema(select)
 
-    async def _describe_interceptor(self, expression: exp.Expression) -> AllowedResult:
+    async def _describe_middleware(self, q: Query) -> AllowedResult:
         """Intercept DESCRIBE statements"""
-        if isinstance(expression, exp.Describe):
-            name = expression.this.name
+        if isinstance(q.expression, exp.Describe):
+            name = q.expression.this.name
             show = self.dialect().parse(f"SHOW COLUMNS FROM {name}")[0]
-            return (
-                await self._show_interceptor(show)
-                if isinstance(show, exp.Expression)
-                else None
-            )
-        return None
+            return await self._show(show) if isinstance(show, exp.Show) else None
+        return await q.next()
 
-    async def _rollback_interceptor(self, expression: exp.Expression) -> AllowedResult:
+    async def _rollback_middleware(self, q: Query) -> AllowedResult:
         """Intercept ROLLBACK statements"""
-        if isinstance(expression, exp.Rollback):
+        if isinstance(q.expression, exp.Rollback):
             return [], []
-        return None
+        return await q.next()
 
-    async def _replace_variables_interceptor(self, expression: exp.Expression) -> None:
+    async def _replace_variables_middleware(self, q: Query) -> AllowedResult:
         """Replace session variables and information functions with their corresponding values"""
 
         def _transform(node: exp.Expression) -> exp.Expression:
             new_node = None
 
             if isinstance(node, exp.Func):
                 if isinstance(node, exp.Anonymous):
@@ -366,46 +404,46 @@
                 and isinstance(node.parent, exp.Select)
                 and node.arg_key == "expressions"
             ):
                 new_node = exp.alias_(new_node, exp.to_identifier(node.sql()))
 
             return new_node or node
 
-        if isinstance(expression, exp.Set):
-            for setitem in expression.expressions:
+        if isinstance(q.expression, exp.Set):
+            for setitem in q.expression.expressions:
                 if isinstance(setitem.this, exp.Binary):
                     # In the case of statements like: SET @@foo = @@bar
                     # We only want to replace variables on the right
                     setitem.this.set(
                         "expression",
                         setitem.this.expression.transform(_transform, copy=True),
                     )
         else:
-            expression.transform(_transform, copy=False)
+            q.expression.transform(_transform, copy=False)
 
-    async def _static_query_interceptor(
-        self, expression: exp.Expression
-    ) -> AllowedResult:
+        return await q.next()
+
+    async def _static_query_middleware(self, q: Query) -> AllowedResult:
         """
         Handle static queries (e.g. SELECT 1).
 
         These very common, as many clients execute commands like SELECT DATABASE() when connecting.
         """
-        if isinstance(expression, exp.Select) and not any(
-            expression.args.get(a)
+        if isinstance(q.expression, exp.Select) and not any(
+            q.expression.args.get(a)
             for a in set(exp.Select.arg_types) - {"expressions", "limit", "hint"}
         ):
-            result = execute(expression)
+            result = execute(q.expression)
             return result.rows, result.columns
-        return None
+        return await q.next()
 
-    async def _set_interceptor(self, expression: exp.Expression) -> AllowedResult:
+    async def _set_middleware(self, q: Query) -> AllowedResult:
         """Intercept SET statements"""
-        if isinstance(expression, exp.Set):
-            expressions = expression.expressions
+        if isinstance(q.expression, exp.Set):
+            expressions = q.expression.expressions
             for item in expressions:
                 assert isinstance(item, exp.SetItem)
 
                 kind = setitem_kind(item)
 
                 if kind == "VARIABLE":
                     self._set_variable(item)
@@ -418,26 +456,24 @@
                 else:
                     raise MysqlError(
                         f"Unsupported SET statement: {kind}",
                         code=ErrorCode.NOT_SUPPORTED_YET,
                     )
 
             return [], []
-        return None
+        return await q.next()
 
-    async def _info_schema_interceptor(
-        self, expression: exp.Expression
-    ) -> AllowedResult:
+    async def _info_schema_middleware(self, q: Query) -> AllowedResult:
         """Intercept queries to INFORMATION_SCHEMA tables"""
-        dbs = find_dbs(expression)
+        dbs = find_dbs(q.expression)
         if (self.database and self.database.lower() in INFO_SCHEMA) or (
             dbs and all(db.lower() in INFO_SCHEMA for db in dbs)
         ):
-            return await self._query_info_schema(expression)
-        return None
+            return await self._query_info_schema(q.expression)
+        return await q.next()
 
     def _set_variable(self, setitem: exp.SetItem) -> None:
         assignment = setitem.this
         left = assignment.left
 
         if isinstance(left, exp.SessionParameter):
             scope = left.text("kind") or "SESSION"
```

### Comparing `mysql-mimic-2.2.7/mysql_mimic/stream.py` & `mysql-mimic-2.3.0/mysql_mimic/stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/types.py` & `mysql-mimic-2.3.0/mysql_mimic/types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/utils.py` & `mysql-mimic-2.3.0/mysql_mimic/utils.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic/variables.py` & `mysql-mimic-2.3.0/mysql_mimic/variables.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/mysql_mimic.egg-info/PKG-INFO` & `mysql-mimic-2.3.0/mysql_mimic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.7
+Version: 2.3.0
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.7/mysql_mimic.egg-info/SOURCES.txt` & `mysql-mimic-2.3.0/mysql_mimic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/setup.py` & `mysql-mimic-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/tests/test_auth.py` & `mysql-mimic-2.3.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/tests/test_query.py` & `mysql-mimic-2.3.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/tests/test_ssl.py` & `mysql-mimic-2.3.0/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/tests/test_stream.py` & `mysql-mimic-2.3.0/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/tests/test_types.py` & `mysql-mimic-2.3.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.7/tests/test_variables.py` & `mysql-mimic-2.3.0/tests/test_variables.py`

 * *Files identical despite different names*

