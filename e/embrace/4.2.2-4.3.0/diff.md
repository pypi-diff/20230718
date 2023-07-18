# Comparing `tmp/embrace-4.2.2.tar.gz` & `tmp/embrace-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embrace-4.2.2.tar", last modified: Tue Jun 20 15:31:49 2023, max compression
+gzip compressed data, was "embrace-4.3.0.tar", last modified: Tue Jul 18 11:28:41 2023, max compression
```

## Comparing `embrace-4.2.2.tar` & `embrace-4.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-06-20 15:31:49.298836 embrace-4.2.2/
--rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-06-20 15:30:49.000000 embrace-4.2.2/LICENSE.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)    12509 2023-06-20 15:31:49.299010 embrace-4.2.2/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)    11800 2023-06-20 15:30:49.000000 embrace-4.2.2/README.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-06-20 15:31:49.296341 embrace-4.2.2/embrace/
--rw-r--r--   0 oliver    (1001) wheel        (0)      804 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1938 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9891 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/module.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9156 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/parsing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     6260 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/pool.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1897 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/poolvalidators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    28346 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/query.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3682 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/util.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-06-20 15:31:49.297490 embrace-4.2.2/embrace.egg-info/
--rw-r--r--   0 oliver    (1001) wheel        (0)    12509 2023-06-20 15:31:48.000000 embrace-4.2.2/embrace.egg-info/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      450 2023-06-20 15:31:48.000000 embrace-4.2.2/embrace.egg-info/SOURCES.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-06-20 15:31:48.000000 embrace-4.2.2/embrace.egg-info/dependency_links.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       15 2023-06-20 15:31:48.000000 embrace-4.2.2/embrace.egg-info/requires.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        8 2023-06-20 15:31:48.000000 embrace-4.2.2/embrace.egg-info/top_level.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)      748 2023-06-20 15:31:49.299755 embrace-4.2.2/setup.cfg
--rwxr-xr-x   0 oliver    (1001) wheel        (0)      635 2023-06-20 15:30:49.000000 embrace-4.2.2/setup.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-06-20 15:31:49.298637 embrace-4.2.2/tests/
--rw-r--r--   0 oliver    (1001) wheel        (0)     6390 2023-06-20 15:30:49.000000 embrace-4.2.2/tests/test_module.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3518 2023-06-20 15:30:49.000000 embrace-4.2.2/tests/test_parsing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1626 2023-06-20 15:30:49.000000 embrace-4.2.2/tests/test_pool.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    19059 2023-06-20 15:30:49.000000 embrace-4.2.2/tests/test_query.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1010 2023-06-20 15:30:49.000000 embrace-4.2.2/tests/test_util.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-07-18 11:28:41.908312 embrace-4.3.0/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-07-18 11:27:44.000000 embrace-4.3.0/LICENSE.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)    13181 2023-07-18 11:28:41.908442 embrace-4.3.0/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)    12472 2023-07-18 11:27:44.000000 embrace-4.3.0/README.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-07-18 11:28:41.906013 embrace-4.3.0/embrace/
+-rw-r--r--   0 oliver    (1001) wheel        (0)      804 2023-07-18 11:27:44.000000 embrace-4.3.0/embrace/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1938 2023-07-18 11:27:44.000000 embrace-4.3.0/embrace/exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9891 2023-07-18 11:27:44.000000 embrace-4.3.0/embrace/module.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9156 2023-07-18 11:27:44.000000 embrace-4.3.0/embrace/parsing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     6260 2023-07-18 11:27:44.000000 embrace-4.3.0/embrace/pool.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1896 2023-07-18 11:27:44.000000 embrace-4.3.0/embrace/poolvalidators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    33294 2023-07-18 11:27:44.000000 embrace-4.3.0/embrace/query.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3682 2023-07-18 11:27:44.000000 embrace-4.3.0/embrace/util.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-07-18 11:28:41.907080 embrace-4.3.0/embrace.egg-info/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    13181 2023-07-18 11:28:41.000000 embrace-4.3.0/embrace.egg-info/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      450 2023-07-18 11:28:41.000000 embrace-4.3.0/embrace.egg-info/SOURCES.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-07-18 11:28:41.000000 embrace-4.3.0/embrace.egg-info/dependency_links.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       15 2023-07-18 11:28:41.000000 embrace-4.3.0/embrace.egg-info/requires.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        8 2023-07-18 11:28:41.000000 embrace-4.3.0/embrace.egg-info/top_level.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)      748 2023-07-18 11:28:41.909045 embrace-4.3.0/setup.cfg
+-rwxr-xr-x   0 oliver    (1001) wheel        (0)      635 2023-07-18 11:27:44.000000 embrace-4.3.0/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-07-18 11:28:41.908131 embrace-4.3.0/tests/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     6390 2023-07-18 11:27:44.000000 embrace-4.3.0/tests/test_module.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3518 2023-07-18 11:27:44.000000 embrace-4.3.0/tests/test_parsing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1626 2023-07-18 11:27:44.000000 embrace-4.3.0/tests/test_pool.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    22799 2023-07-18 11:27:44.000000 embrace-4.3.0/tests/test_query.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1010 2023-07-18 11:27:44.000000 embrace-4.3.0/tests/test_util.py
```

### Comparing `embrace-4.2.2/LICENSE.txt` & `embrace-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/PKG-INFO` & `embrace-4.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embrace
-Version: 4.2.2
+Version: 4.3.0
 Summary: Embrace SQL keeps your SQL queries in SQL files. An anti-ORM inspired by HugSQL and PugSQL
 Home-page: https://hg.sr.ht/~olly/embrace-sql
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: sql hugsql pugsql orm anti-orm files dapper
 Classifier: Development Status :: 4 - Beta
@@ -175,24 +175,24 @@
 
 Use ``resultset`` to get access to both the results and cursor metadata, for example::
 
     result = Query("SELECT * from mytable").resultset(conn)
     print(result.many())
     print(result.cursor.description)
 
-How do I return rows as dicts or named tuples?
-----------------------------------------------
+How do I return rows as dicts, namedtuples or dataclasses?
+----------------------------------------------------------
 
 Queries return rows directly from the underlying db-api driver.
 Many drivers have options to return data structures other than tuples (for
 example ``sqlite3.Row`` or ``psycopg2.extras.DictCursor``). You will need to
 configure these at the connection level.
 
 See the next section for how to use ``embrace.query.mapobject`` to map rows
-on to namedtuples, dicts or your own ORM-style model classes.
+to dicts, namedtuples, dataclasses or your own ORM-style model classes.
 
 How do I map rows onto objects?
 -------------------------------
 
 Embrace supports simple ORM style mapping.
 
 Example::
@@ -226,44 +226,66 @@
 map the returned columns onto objects::
 
     from embrace import mapobject
 
     query = queries.query(
         """
         SELECT posts.*, users.*
-        FROM posts JOIN users ON posts.user_id = users.id
+        FROM posts JOIN users ON posts.user_id = users.user_id
         """
     ).returning(
         (
             mapobject(Post, split="post_id"),
             mapobject(User, split="user_id")
         )
     )
     for post, user in query.many(conn):
         …
 
-``mapobject`` can also load columns into dicts and namedtuples::
+``mapobject`` can also load columns into dicts, namedtuples and dataclasses::
 
     from embrace import mapobject
 
     query = queries.query(
         """
-        SELECT posts.*, users.*
-        FROM posts JOIN users ON posts.user_id = users.id
+        SELECT posts.*, categories.*, users.*
+        FROM posts
+            JOIN categories ON posts.category_id = categories.id
+            JOIN users ON posts.user_id = users.id
         """
     ).returning(
         (
-            mapobject.dict(split="post_id"),
-            mapobject.namedtuple(split="user_id")
+            mapobject.dict(),
+            mapobject.namedtuple()
+            mapobject.dataclass()
         )
     )
-    for post, user in query.many(conn):
+    for post, category, user in query.many(conn):
         …
 
-and pass individual columns through unchanged::
+
+When mapping dataclasses, you can specify additional fields for the dataclass
+by providing a list of fields in the format expected by
+``dataclasses.make_dataclass``::
+
+    mapobject.dataclass(
+        [
+            ('owner', typing.Any),
+            ('images', list[Image], dataclasses.fields(default_factory=list))
+        ]
+    )
+
+Or as keyword arguments::
+
+    mapobject.dataclass(
+        owner=typing.Any,
+        images=(list[Image], dataclasses.fields(default_factory=list)),
+    )
+
+``mapobject.passthrough`` passes individual columns through unchanged::
 
     query = queries.query(
         """
         SELECT posts.*, count(*) as reply_count
         FROM posts JOIN replies ON posts.id = replies.post_id
         """
     ).returning(
```

### Comparing `embrace-4.2.2/README.rst` & `embrace-4.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -156,24 +156,24 @@
 
 Use ``resultset`` to get access to both the results and cursor metadata, for example::
 
     result = Query("SELECT * from mytable").resultset(conn)
     print(result.many())
     print(result.cursor.description)
 
-How do I return rows as dicts or named tuples?
-----------------------------------------------
+How do I return rows as dicts, namedtuples or dataclasses?
+----------------------------------------------------------
 
 Queries return rows directly from the underlying db-api driver.
 Many drivers have options to return data structures other than tuples (for
 example ``sqlite3.Row`` or ``psycopg2.extras.DictCursor``). You will need to
 configure these at the connection level.
 
 See the next section for how to use ``embrace.query.mapobject`` to map rows
-on to namedtuples, dicts or your own ORM-style model classes.
+to dicts, namedtuples, dataclasses or your own ORM-style model classes.
 
 How do I map rows onto objects?
 -------------------------------
 
 Embrace supports simple ORM style mapping.
 
 Example::
@@ -207,44 +207,66 @@
 map the returned columns onto objects::
 
     from embrace import mapobject
 
     query = queries.query(
         """
         SELECT posts.*, users.*
-        FROM posts JOIN users ON posts.user_id = users.id
+        FROM posts JOIN users ON posts.user_id = users.user_id
         """
     ).returning(
         (
             mapobject(Post, split="post_id"),
             mapobject(User, split="user_id")
         )
     )
     for post, user in query.many(conn):
         …
 
-``mapobject`` can also load columns into dicts and namedtuples::
+``mapobject`` can also load columns into dicts, namedtuples and dataclasses::
 
     from embrace import mapobject
 
     query = queries.query(
         """
-        SELECT posts.*, users.*
-        FROM posts JOIN users ON posts.user_id = users.id
+        SELECT posts.*, categories.*, users.*
+        FROM posts
+            JOIN categories ON posts.category_id = categories.id
+            JOIN users ON posts.user_id = users.id
         """
     ).returning(
         (
-            mapobject.dict(split="post_id"),
-            mapobject.namedtuple(split="user_id")
+            mapobject.dict(),
+            mapobject.namedtuple()
+            mapobject.dataclass()
         )
     )
-    for post, user in query.many(conn):
+    for post, category, user in query.many(conn):
         …
 
-and pass individual columns through unchanged::
+
+When mapping dataclasses, you can specify additional fields for the dataclass
+by providing a list of fields in the format expected by
+``dataclasses.make_dataclass``::
+
+    mapobject.dataclass(
+        [
+            ('owner', typing.Any),
+            ('images', list[Image], dataclasses.fields(default_factory=list))
+        ]
+    )
+
+Or as keyword arguments::
+
+    mapobject.dataclass(
+        owner=typing.Any,
+        images=(list[Image], dataclasses.fields(default_factory=list)),
+    )
+
+``mapobject.passthrough`` passes individual columns through unchanged::
 
     query = queries.query(
         """
         SELECT posts.*, count(*) as reply_count
         FROM posts JOIN replies ON posts.id = replies.post_id
         """
     ).returning(
```

### Comparing `embrace-4.2.2/embrace/__init__.py` & `embrace-4.3.0/embrace/__init__.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/embrace/exceptions.py` & `embrace-4.3.0/embrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/embrace/module.py` & `embrace-4.3.0/embrace/module.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/embrace/parsing.py` & `embrace-4.3.0/embrace/parsing.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/embrace/pool.py` & `embrace-4.3.0/embrace/pool.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/embrace/poolvalidators.py` & `embrace-4.3.0/embrace/poolvalidators.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def before_release(self, conn):
         conn.rollback()
         return self.validate(conn)
 
 
 try:
     from psycopg2 import extensions as psycopg2_ext
-    from psycopg2.extensions import connections as psycopg2_conn
+    from psycopg2.extensions import connection as psycopg2_conn
 except ImportError:
     pass
 else:
 
     @validator(psycopg2_conn)
     class Psycopg2ConnectionValidator(ConnectionValidator):
         def validate(self, conn):
```

### Comparing `embrace-4.2.2/embrace/query.py` & `embrace-4.3.0/embrace/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from collections import namedtuple
-from dataclasses import dataclass
-from dataclasses import InitVar
+import dataclasses
 from functools import partial
 from itertools import chain
 from itertools import islice
 from itertools import zip_longest
 from typing import Any
 from typing import Callable
 from typing import Dict
@@ -53,15 +52,14 @@
     pass
 
 
 NullObject = NullObjectType()
 
 
 def get_param_style(conn: Any) -> str:
-
     conncls = conn.__class__
     try:
         return known_styles[conncls]
     except KeyError:
         modname = conncls.__module__
         while modname:
             try:
@@ -73,15 +71,14 @@
                     modname = modname.rsplit(".", 1)[0]
                 else:
                     break
     raise TypeError(f"Can't find paramstyle for connection {conn!r}")
 
 
 class Query:
-
     name: Optional[str]
     source: Optional[str]
     lineno: Optional[int]
     result_type: str
     includes: List[str] = []
     includes_resolved = False
     get_row_mapper: Optional[Callable]
@@ -148,14 +145,55 @@
         joins: Optional[Union[_joinedload, Sequence[_joinedload]]] = None,
         positional=False,
         key_columns: Optional[List[Tuple[str]]] = None,
         split_on=[],
     ) -> "Query":
         """
         Return a copy of the query with a changed result type
+
+        :param row_spec:
+            One of:
+                - a single callable or :class:`mapobject` instance
+                - a sequence of callables and :class:`mapobject` instances
+
+            In the case that a single callable or mapobject is provided, the
+            values for each row will be passed to the callable as keyword
+            arguments, and each row will return a single python object.
+
+            If a sequence of items is provided, the row will be split up into
+            multiple objects at the columns indicated by the values of
+            ``split_on``, or configured in :attr:`mapobject.split_on`.
+
+        :param joins:
+            When multiple python objects are generated per-row, ``joins``
+            tells embrace how to construct relations between objects. See
+            :func:`one_to_one` and :func:`one_to_many`.
+
+        :param positional:
+            If True, pass column values to the items in ``row_spec`` as
+            positional parameters rather than keyword args.
+
+        :key_columns:
+            The list of primary key columns for each object mapped by ``row_spec``.
+            Rows with the same values in these columns will be mapped to the
+            same python object.
+
+            If key_columns is not provided, rows will be mapped to the same
+            python object if all values match.
+
+            It is an error to use this parameter if :class:`mapobject` is
+            used anywhere in ``row_spec``.
+
+        :split_on:
+            List of the column names that mark where new objects start
+            splitting a row into multiple python objects. If not provided,
+            the string ``'id'`` will be used.
+
+            It is an error to use this parameter if :class:`mapobject` is
+            used anywhere in ``row_spec``.
         """
         q = self.copy()
         if isinstance(joins, _joinedload):
             joins = [joins]
 
         row_spec = make_rowspec(row_spec, split_on or [], key_columns or [], positional)
         q.get_row_mapper = partial(make_row_mapper, row_spec, joins)
@@ -224,15 +262,16 @@
             compile_bind_parameters(paramstyle, s, params) for s in self.statements
         ]
         for sqltext, bind_params in prepared:
             if debug:
                 import textwrap
 
                 print(
-                    f"Executing \n{textwrap.indent(sqltext, '    ')} with {bind_params!r}",
+                    f"Executing \n{textwrap.indent(sqltext, '    ')} "
+                    f"with {bind_params!r}",
                     file=sys.stderr,
                 )
             try:
                 cursor.execute(sqltext, bind_params)
             except BaseException:
                 _handle_exception(conn, self.source, 1)
 
@@ -317,15 +356,14 @@
             pos_ = len(column_names)
         result.append(slice(pos, pos_))
         pos = pos_
     return result
 
 
 def make_row_mapper(row_spec: Sequence["mapobject"], joins, description):
-
     row_spec = list(row_spec)
     is_multi = len(row_spec) > 1
     column_names: List[str] = [d[0] for d in description]
     split_points = []
 
     if is_multi:
         split_points = get_split_points(row_spec, column_names)
@@ -388,15 +426,14 @@
     items = None
 
     multi_join_targets = [
         t_idx for t_idx, _, _, arity, _ in indexed_joins if arity == "*"
     ]
     seen: Set[Tuple[int, int]] = set()
     for irow, items in enumerate(object_rows):
-
         # When all columns change, emit a new object row (or single item)
         if irow > 0 and all(items[ix] != last[ix] for ix in multi_join_targets):
             if single_column:
                 yield cur[0]
             else:
                 yield tuple(cur[ix] for ix in return_columns)
             seen.clear()
@@ -456,18 +493,25 @@
                     append(cur[ix])
                 else:
                     append(make_object(items[ix]))
             yield tuple(rv)
 
 
 def one_to_one(target, attr, source):
+    """
+    Populate `<target>.<attr>` with
+    the item identified by `source`.
+    """
     return _joinedload(target, attr, source, "1")
 
 
 def one_to_many(target, attr, source):
+    """
+    Populate `<target>.<attr>` with the list of items identified by `source`.
+    """
     return _joinedload(target, attr, source, "*")
 
 
 def translate_to_column_indexes(
     row_spec, join_spec: List[_joinedload]
 ) -> Sequence[Tuple[int, str, int, str, bool]]:
     row_spec_indexes = {c.label: ix for ix, c in enumerate(row_spec)}
@@ -495,14 +539,15 @@
 
 def make_object_maker(
     mapped_column_names: List[Tuple[str, ...]],
     row_spec: List[Any],
 ) -> Callable[[Union[NullObjectType, Tuple]], Any]:
     """
     Return a function that constructs the target type from a group of columns.
+
     The returned function will cache objects (the same input returns the
     same object) so that object identity may be relied on within the scope of a
     single query.
     """
 
     key_column_positions: List[List[int]] = []
     row_spec_cols = list(zip(row_spec, mapped_column_names))
@@ -608,43 +653,40 @@
 
 def make_rowspec(
     row_spec: Union["mapobject", Callable, Sequence[Union["mapobject", Callable]]],
     split_on: Sequence[str],
     key_columns: Sequence[Tuple[str]],
     positional: bool,
 ) -> Sequence["mapobject"]:
-
     if not isinstance(row_spec, Sequence):
         row_spec = (row_spec,)
 
     if split_on and any(isinstance(i, mapobject) for i in row_spec):
         raise TypeError("Cannot combine mapobject with split_on")
 
     result = []
     for ix, item in enumerate(row_spec):
-
         if not isinstance(item, mapobject):
             item = mapobject(item)
 
             # Enable backwards compatibility for positional, split_on, key_columns
             item.positional = positional
             if 0 < ix < len(split_on) - 1:
                 item.split = split_on[ix - 1]
             if ix < len(key_columns):
                 item.key_columns = key_columns[ix]
 
         result.append(item)
     return result
 
 
-@dataclass
+@dataclasses.dataclass
 class mapobject:
-
     mapped: Callable
-    key: InitVar[Union[str, Sequence[str]]] = tuple()
+    key: dataclasses.InitVar[Union[str, Sequence[str]]] = tuple()
     split: str = "id"
     positional: bool = False
     column_count: Optional[int] = None
     join_as_dict: bool = False
     key_columns: Sequence[str] = tuple()
     label: Any = None
 
@@ -681,17 +723,92 @@
                 _nt = namedtuple(  # type: ignore
                     f"mapobject_namedtuple_{id(dynamicnamedtuple)}", tuple(kwargs)
                 )
             return _nt(**kwargs)  # type: ignore
 
         return cls(mapped=dynamicnamedtuple, **kwargs)
 
+    @classmethod
+    def dataclass(
+        cls,
+        fields: Sequence[
+            Union[
+                str,
+                Tuple[str, Union[str, type]],
+                Tuple[str, Union[str, type], dataclasses.Field],
+            ]
+        ]=[],
+        **kwargs: Any,
+    ):
+        """
+        Return a mapper that stores values in a dataclass.
 
-class ResultSet:
+        By default field names are be inferred from the returned column names,
+        and have a type of ``typing.Any``.
+
+        :param fields:
+            Additional fields which to be appended after fields loaded from the
+            database. This should be in the same format as expected by the
+            stdlib :func:`dataclasses.make_dataclass` function.
+
+            If a field has the same name as one of the returned
+            columns, it will be used instead of autogenerating a field.
+
+            If a field tuple does not contain a :class:`dataclasses.Field` item,
+            the value ``dataclasses.field(default=None)`` will be used.
+            Additional fields are not populated during data loading so
+            must have a default or default_factory specified.
+
+        :param kwargs:
+            Keyword arguments corresponding to :class:`mapobject` fields will be
+            passed through to the constructor (eg ``split``, ``label``, etc).
+            Other arguments will be taken as additional field names, and
+            specified as either a simple name-type mapping::
+
+                mapobject.dataclass(foo=list[str]|None)
+
+            or as a tuple of ``(type, Field)``::
+
+                mapobject.dataclass(
+                    foo=(list[str], dataclasses.field(default_factory=list))
+                )
+        """
+        datacls = None
+        mapobject_fields = {f.name for f in dataclasses.fields(cls)}
+        field_dict = {item[0]: item for item in fields}
+        field_dict.update(
+            (name, (name,) + (item if isinstance(item, tuple) else (item,)))
+            for name, item in kwargs.items()
+            if name not in mapobject_fields
+        )
+        mapobject_kwargs = {
+            k: v for k, v in kwargs.items() if k in mapobject_fields
+        }
+
+        def dynamicdataclass(**kwargs):
+            nonlocal datacls
+            if datacls is None:
+                dbfields = [field_dict.pop(k, k) for k in kwargs]
+                additionalfields = []
+                for item in field_dict.values():
+                    if isinstance(item, str):
+                        item = (item,)
+                    if len(item) < 3:
+                        item = item + (dataclasses.field(default=None),)
+                    additionalfields.append(item)
+                datacls = dataclasses.make_dataclass(
+                    f"mapobject_dataclass_{id(dynamicdataclass)}",
+                    dbfields + additionalfields
+                )
+            return datacls(**kwargs)
 
+        return cls(mapped=dynamicdataclass, **mapobject_kwargs)
+
+
+class ResultSet:
     __slots__ = ["cursor", "row_mapper"]
 
     def __init__(self, cursor, row_mapper):
         self.cursor = cursor
         self.row_mapper = row_mapper
 
     def __iter__(self):
@@ -738,15 +855,14 @@
             method = "fetchmany"
 
         row_getter = getattr(self, f"many_rows_{method}")
         if self.row_mapper:
             if limit_mapped:
 
                 def limited_rowmapper():
-
                     count = 0
                     rowcount = 0
 
                     if method == "fetchmany":
 
                         def _row_getter():
                             while True:
```

### Comparing `embrace-4.2.2/embrace/util.py` & `embrace-4.3.0/embrace/util.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/embrace.egg-info/PKG-INFO` & `embrace-4.3.0/embrace.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embrace
-Version: 4.2.2
+Version: 4.3.0
 Summary: Embrace SQL keeps your SQL queries in SQL files. An anti-ORM inspired by HugSQL and PugSQL
 Home-page: https://hg.sr.ht/~olly/embrace-sql
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: sql hugsql pugsql orm anti-orm files dapper
 Classifier: Development Status :: 4 - Beta
@@ -175,24 +175,24 @@
 
 Use ``resultset`` to get access to both the results and cursor metadata, for example::
 
     result = Query("SELECT * from mytable").resultset(conn)
     print(result.many())
     print(result.cursor.description)
 
-How do I return rows as dicts or named tuples?
-----------------------------------------------
+How do I return rows as dicts, namedtuples or dataclasses?
+----------------------------------------------------------
 
 Queries return rows directly from the underlying db-api driver.
 Many drivers have options to return data structures other than tuples (for
 example ``sqlite3.Row`` or ``psycopg2.extras.DictCursor``). You will need to
 configure these at the connection level.
 
 See the next section for how to use ``embrace.query.mapobject`` to map rows
-on to namedtuples, dicts or your own ORM-style model classes.
+to dicts, namedtuples, dataclasses or your own ORM-style model classes.
 
 How do I map rows onto objects?
 -------------------------------
 
 Embrace supports simple ORM style mapping.
 
 Example::
@@ -226,44 +226,66 @@
 map the returned columns onto objects::
 
     from embrace import mapobject
 
     query = queries.query(
         """
         SELECT posts.*, users.*
-        FROM posts JOIN users ON posts.user_id = users.id
+        FROM posts JOIN users ON posts.user_id = users.user_id
         """
     ).returning(
         (
             mapobject(Post, split="post_id"),
             mapobject(User, split="user_id")
         )
     )
     for post, user in query.many(conn):
         …
 
-``mapobject`` can also load columns into dicts and namedtuples::
+``mapobject`` can also load columns into dicts, namedtuples and dataclasses::
 
     from embrace import mapobject
 
     query = queries.query(
         """
-        SELECT posts.*, users.*
-        FROM posts JOIN users ON posts.user_id = users.id
+        SELECT posts.*, categories.*, users.*
+        FROM posts
+            JOIN categories ON posts.category_id = categories.id
+            JOIN users ON posts.user_id = users.id
         """
     ).returning(
         (
-            mapobject.dict(split="post_id"),
-            mapobject.namedtuple(split="user_id")
+            mapobject.dict(),
+            mapobject.namedtuple()
+            mapobject.dataclass()
         )
     )
-    for post, user in query.many(conn):
+    for post, category, user in query.many(conn):
         …
 
-and pass individual columns through unchanged::
+
+When mapping dataclasses, you can specify additional fields for the dataclass
+by providing a list of fields in the format expected by
+``dataclasses.make_dataclass``::
+
+    mapobject.dataclass(
+        [
+            ('owner', typing.Any),
+            ('images', list[Image], dataclasses.fields(default_factory=list))
+        ]
+    )
+
+Or as keyword arguments::
+
+    mapobject.dataclass(
+        owner=typing.Any,
+        images=(list[Image], dataclasses.fields(default_factory=list)),
+    )
+
+``mapobject.passthrough`` passes individual columns through unchanged::
 
     query = queries.query(
         """
         SELECT posts.*, count(*) as reply_count
         FROM posts JOIN replies ON posts.id = replies.post_id
         """
     ).returning(
```

### Comparing `embrace-4.2.2/setup.cfg` & `embrace-4.3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = embrace
-version = 4.2.2
+version = 4.3.0
 description = Embrace SQL keeps your SQL queries in SQL files. An anti-ORM inspired by HugSQL and PugSQL
 long_description = file: README.rst
 author = Oliver Cope
 author_email = oliver@redgecko.org
 keywords = sql hugsql pugsql orm anti-orm files dapper
 url = https://hg.sr.ht/~olly/embrace-sql
 license = Apache
```

### Comparing `embrace-4.2.2/setup.py` & `embrace-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/tests/test_module.py` & `embrace-4.3.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/tests/test_parsing.py` & `embrace-4.3.0/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/tests/test_pool.py` & `embrace-4.3.0/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.2/tests/test_query.py` & `embrace-4.3.0/tests/test_query.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import typing
 from typing import Any
 from typing import List
+import dataclasses
 from itertools import islice
 from unittest.mock import Mock
 from unittest.mock import call
 import string
 
 from embrace.query import Query
 from embrace.query import ResultSet
@@ -98,15 +100,14 @@
     test("scalar", [(1, 2, 3), (4, 5, 6)], 1)
     test("column", [(1, 2), (3, 4)], [1, 3])
     test("cursor", [], lambda conn: conn.cursor())
     test("affected", [], lambda conn: conn.cursor().rowcount)
 
 
 def test_mapped_objects_with_no_rows_returned():
-
     conn = mock_conn(rows=[])
     assert query("one_or_none").returning(dict)(conn) is None
     assert query("first").returning(dict)(conn) is None
 
 
 def test_can_override_return_type():
     def test(result_type, rows, expected):
@@ -218,15 +219,18 @@
             MockModel(id=2, x=[MockModel(id=1), MockModel(id=2)]),
             MockModel(id=3, x=[MockModel(id=1)]),
             MockModel(id=4, x=[MockModel(id=1)]),
         ]
 
         for method in ("fetchall", "fetchmany", "fetchone", "auto"):
             for limit in [1, 2, 3, 4, 5, 100]:
-                conn = mock_conn(rows=rows, description=[("id",), ("id",)],)
+                conn = mock_conn(
+                    rows=rows,
+                    description=[("id",), ("id",)],
+                )
                 rs = (
                     query("x")
                     .returning((MockModel, MockModel), joins=(one_to_many(0, "x", 1)))
                     .resultset(conn)
                 )
 
                 assert (
@@ -270,126 +274,265 @@
         b = Mock()
         result = query("").returning((a, b), positional=True).one(conn)
         assert a.call_args_list == [call(1, 2)]
         assert b.call_args_list == [call(3, 4)]
         assert result == (a(), b())
 
     def test_it_preserves_identity(self):
-        conn = mock_conn(rows=[(1, 5), (2, 6), (1, 6)], description=[("a",), ("b",)],)
+        conn = mock_conn(
+            rows=[(1, 5), (2, 6), (1, 6)],
+            description=[("a",), ("b",)],
+        )
         result = list(query("").returning((MockModel), key_columns=[("a",)]).many(conn))
         assert result[0] is result[2]
         assert result[0] is not result[1]
 
-        conn = mock_conn(rows=[(1, 5), (1, 6), (2, 6)], description=[("a",), ("b",)],)
+        conn = mock_conn(
+            rows=[(1, 5), (1, 6), (2, 6)],
+            description=[("a",), ("b",)],
+        )
         result = list(query("").returning((MockModel), key_columns=[("b",)]).many(conn))
         assert result[0] is not result[1]
         assert result[1] is result[2]
 
     def test_it_doesnt_preserve_identity(self):
-        conn = mock_conn(rows=[(1, 5), (1, 6), (2, 6)], description=[("a",), ("b",)],)
+        conn = mock_conn(
+            rows=[(1, 5), (1, 6), (2, 6)],
+            description=[("a",), ("b",)],
+        )
         result = list(query("").returning((MockModel)).many(conn))
         assert result[0] is not result[1]
         assert result[1] is not result[2]
 
-    def test_it_preserves_identity_on_consecutive_objects_without_key_columns(self,):
-        conn = mock_conn(rows=[(1, 5), (1, 6), (1, 6)], description=[("id",), ("id",)],)
+    def test_it_preserves_identity_on_consecutive_objects_without_key_columns(
+        self,
+    ):
+        conn = mock_conn(
+            rows=[(1, 5), (1, 6), (1, 6)],
+            description=[("id",), ("id",)],
+        )
         result = list(query("").returning((MockModel, MockModel)).many(conn))
         assert result[0][0] is result[1][0]
         assert result[0][0] is result[2][0]
         assert result[0][1] is not result[1][1]
         assert result[0][1] is not result[2][1]
         assert result[1][1] is result[2][1]
 
     def test_key_columns_has_a_helpful_error(self):
-
-        conn = mock_conn(rows=[], description=[("a",), ("b",)],)
+        conn = mock_conn(
+            rows=[],
+            description=[("a",), ("b",)],
+        )
         with pytest.raises(ValueError) as excinfo:
             query("").returning((MockModel), key_columns="c").many(conn)
         assert "'c' specified in key_columns does not exist" in str(excinfo.value)
 
     def test_object_identity_works_with_unhashable_objects(self):
-        conn = mock_conn(rows=[([1], 1), ([1], 1)], description=[("id",), ("id",)],)
+        conn = mock_conn(
+            rows=[([1], 1), ([1], 1)],
+            description=[("id",), ("id",)],
+        )
         result = list(
             query("")
             .returning((MockModel, MockModel), joins=(one_to_one(0, "x", 1),))
             .many(conn)
         )
         assert result[0] is result[1]
 
     def test_unfazed_by_empty_resultset(self):
-        conn = mock_conn(rows=[], description=[("id",)],)
+        conn = mock_conn(
+            rows=[],
+            description=[("id",)],
+        )
         result = list(query("").returning((MockModel)).many(conn))
         assert result == []
 
-        conn = mock_conn(rows=[], description=[("id",), ("id",)],)
+        conn = mock_conn(
+            rows=[],
+            description=[("id",), ("id",)],
+        )
         result = list(query("").returning((MockModel, MockModel)).many(conn))
         assert result == []
 
-        conn = mock_conn(rows=[], description=[("id",), ("id",)],)
+        conn = mock_conn(
+            rows=[],
+            description=[("id",), ("id",)],
+        )
         result = list(
             query("")
             .returning((MockModel, MockModel), joins=[one_to_many(0, "a", 1)])
             .many(conn)
         )
         assert result == []
 
-        conn = mock_conn(rows=[], description=[("id",), ("id",), ("id",)],)
+        conn = mock_conn(
+            rows=[],
+            description=[("id",), ("id",), ("id",)],
+        )
         result = list(
             query("")
             .returning(
-                (MockModel, MockModel, MockModel), joins=[one_to_many(1, "a", 2)],
+                (MockModel, MockModel, MockModel),
+                joins=[one_to_many(1, "a", 2)],
             )
             .many(conn)
         )
         assert result == []
 
     def test_passthrough(self):
-        conn = mock_conn(rows=[(1,), ("fish",)], description=[("id",), ("id",)],)
+        conn = mock_conn(
+            rows=[(1,), ("fish",)],
+            description=[("id",), ("id",)],
+        )
         result = list(query("").returning(mapobject.passthrough()).many(conn))
         assert result[0] == 1
         assert result[1] == "fish"
 
     def test_namedtuple(self):
-        conn = mock_conn(rows=[(1, 2)], description=[("a",), ("b",)],)
+        conn = mock_conn(
+            rows=[(1, 2)],
+            description=[("a",), ("b",)],
+        )
         result = list(query("").returning(mapobject.namedtuple()).many(conn))
         assert result[0] == (1, 2)
         assert result[0].a == 1
         assert result[0].b == 2
 
+    def test_dataclass(self):
+        conn = mock_conn(
+            rows=[(1, 2)],
+            description=[("a",), ("b",)],
+        )
+        result = list(query("").returning(mapobject.dataclass()).many(conn))
+        (ob,) = result
+        fields = dataclasses.fields(ob)
+        assert len(fields) == 2
+        assert fields[0].name == "a"
+        assert fields[1].name == "b"
+        assert ob.a == 1
+        assert ob.b == 2
+
+    def test_dataclass_accepts_custom_fields(self):
+        conn = mock_conn(
+            rows=[(1,)],
+            description=[("a",)],
+        )
+        result = list(query("").returning(mapobject.dataclass([("a", int)])).many(conn))
+        (ob,) = result
+        fields = dataclasses.fields(ob)
+        assert len(fields) == 1
+        assert fields[0].name == "a"
+        assert fields[0].type == int
+        assert ob.a == 1
+
+    def test_dataclass_accepts_additional_fields(self):
+        conn = mock_conn(
+            rows=[(1,)],
+            description=[("a",)],
+        )
+        result = list(
+            query("")
+            .returning(mapobject.dataclass([("foo", typing.Union[str, None])]))
+            .many(conn)
+        )
+        (ob,) = result
+        fields = dataclasses.fields(ob)
+        assert len(fields) == 2
+        assert fields[0].name == "a"
+        assert fields[1].name == "foo"
+        assert fields[1].type == typing.Union[str, None]
+        assert ob.a == 1
+        assert ob.foo is None
+
+    def test_dataclass_accepts_kw_fields(self):
+        conn = mock_conn(
+            rows=[(1,)],
+            description=[("a",)],
+        )
+        result = list(
+            query("")
+            .returning(mapobject.dataclass(a=int, foo=typing.Union[str, None]))
+            .many(conn)
+        )
+        (ob,) = result
+        fields = dataclasses.fields(ob)
+        assert len(fields) == 2
+        assert fields[0].name == "a"
+        assert fields[0].type is int
+        assert fields[1].name == "foo"
+        assert fields[1].type == typing.Union[str, None]
+        assert ob.a == 1
+        assert ob.foo is None
+
+    def test_dataclass_accepts_defaults_other_than_none(self):
+        conn = mock_conn(
+            rows=[(1,)],
+            description=[("a",)],
+        )
+        result = list(
+            query("")
+            .returning(
+                mapobject.dataclass(
+                    a=int, foo=(typing.List, dataclasses.field(default_factory=list))
+                )
+            )
+            .many(conn)
+        )
+        (ob,) = result
+        fields = dataclasses.fields(ob)
+        assert len(fields) == 2
+        assert fields[0].name == "a"
+        assert fields[0].type is int
+        assert fields[1].name == "foo"
+        assert fields[1].type == typing.List
+        assert ob.a == 1
+        assert ob.foo == []
+
 
 class TestJoiner:
     def check_result(
-        self, row_spec, join_spec, rows, positional, expected,
+        self,
+        row_spec,
+        join_spec,
+        rows,
+        positional,
+        expected,
     ):
         row_spec = make_rowspec(row_spec, join_spec, [], positional)
         result = list(
             group_by_and_join(
-                [], row_spec, join_spec, [[(item,) for item in row] for row in rows],
+                [],
+                row_spec,
+                join_spec,
+                [[(item,) for item in row] for row in rows],
             )
         )
         assert result == expected
 
     def test_one_to_one(self):
-
         self.check_result(
             (MockModel, int),
             [one_to_one(MockModel, "p", int)],
             [(1, 2)],
             True,
             [MockModel(a=1, p=2)],
         )
 
     def test_one_to_one_with_spare_column(self):
-
         self.check_result(
             (int, MockModel, int),
             [one_to_one(MockModel, "p", 2)],
             [(0, 1, 2)],
             True,
-            [(0, MockModel(a=1, p=2),)],
+            [
+                (
+                    0,
+                    MockModel(a=1, p=2),
+                )
+            ],
         )
 
         self.check_result(
             (int, MockModel, int),
             [one_to_one(MockModel, "p", 0)],
             [(0, 1, 2)],
             True,
@@ -417,15 +560,18 @@
     def test_one_to_many_multi_level(self):
         self.check_result(
             (MockModel, MockModel, int),
             [one_to_many(0, "xs", 1), one_to_many(1, "ys", 2)],
             [(0, 1, 2), (0, 1, 3), (0, 2, 4), (1, 5, 6)],
             True,
             [
-                MockModel(a=0, xs=[MockModel(a=1, ys=[2, 3]), MockModel(a=2, ys=[4])],),
+                MockModel(
+                    a=0,
+                    xs=[MockModel(a=1, ys=[2, 3]), MockModel(a=2, ys=[4])],
+                ),
                 MockModel(a=1, xs=[MockModel(a=5, ys=[6])]),
             ],
         )
 
     def test_it_handles_nulls_one_to_one(self):
         self.check_result(
             (MockModel, MockModel),
@@ -499,50 +645,62 @@
     def test_it_joins(self):
         class MockModelA(MockModel):
             pass
 
         class MockModelB(MockModel):
             pass
 
-        conn = mock_conn([(1, 2), (1, 3)], description=[("id",), ("id",)],)
+        conn = mock_conn(
+            [(1, 2), (1, 3)],
+            description=[("id",), ("id",)],
+        )
         result = list(
             query("")
             .returning(
-                (MockModelA, MockModelB), [one_to_many(MockModelA, "bs", MockModelB)],
+                (MockModelA, MockModelB),
+                [one_to_many(MockModelA, "bs", MockModelB)],
             )
             .many(conn)
         )
         assert result == [MockModelA(id=1, bs=[MockModelB(id=2), MockModelB(id=3)])]
 
     def test_it_handles_left_joins(self):
-        conn = mock_conn([(1, None), (1, 3)], description=[("id",), ("id",)],)
+        conn = mock_conn(
+            [(1, None), (1, 3)],
+            description=[("id",), ("id",)],
+        )
         result = list(
             query("")
-            .returning((MockModel, MockModel), [one_to_many(0, "items", 1)],)
+            .returning(
+                (MockModel, MockModel),
+                [one_to_many(0, "items", 1)],
+            )
             .many(conn)
         )
         assert result == [MockModel(id=1, items=[MockModel(id=3)])]
 
     def test_it_joins_as_dict(self):
-        conn = mock_conn([(1, 2), (1, 3)], description=[("id",), ("id",)],)
+        conn = mock_conn(
+            [(1, 2), (1, 3)],
+            description=[("id",), ("id",)],
+        )
         result = list(
             query("")
             .returning(
-                (mapobject.dict(), mapobject.dict()), [one_to_many(0, "items", 1)],
+                (mapobject.dict(), mapobject.dict()),
+                [one_to_many(0, "items", 1)],
             )
             .many(conn)
         )
         assert result == [{"id": 1, "items": [{"id": 2}, {"id": 3}]}]
 
 
 def test_get_split_points_by_split():
-
     assert get_split_points(
         [mapobject(str), mapobject(str, split="c")], ["a", "b", "c", "d"]
     ) == [slice(0, 2), slice(2, 4)]
 
 
 def test_get_split_points_by_count():
-
     assert get_split_points(
         [mapobject(str, column_count=3), mapobject(str)], ["a", "b", "c", "d"]
     ) == [slice(0, 3), slice(3, 4)]
```

### Comparing `embrace-4.2.2/tests/test_util.py` & `embrace-4.3.0/tests/test_util.py`

 * *Files identical despite different names*

