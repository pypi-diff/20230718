# Comparing `tmp/expiringsqlitedict-6.2.0.tar.gz` & `tmp/expiringsqlitedict-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expiringsqlitedict-6.2.0.tar", last modified: Wed May  3 15:44:21 2023, max compression
+gzip compressed data, was "expiringsqlitedict-7.0.0.tar", last modified: Tue Jul 18 21:40:23 2023, max compression
```

## Comparing `expiringsqlitedict-6.2.0.tar` & `expiringsqlitedict-7.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-6.2.0/.gitignore
--rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-6.2.0/.travis.yml
--rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-6.2.0/CHANGELOG.txt
--rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-6.2.0/LICENSE.apache
--rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-6.2.0/LICENSE.rst
--rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-6.2.0/Makefile
--rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-6.2.0/README.rst
--rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-6.2.0/bench.py
--rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-6.2.0/docs/Makefile
--rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-6.2.0/docs/conf.py
--rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-6.2.0/docs/expiringsqlitedict.rst
--rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-6.2.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-6.2.0/docs/make.bat
--rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-6.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     1030 2023-05-03 15:44:11.565641 expiringsqlitedict-6.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     1327 2023-05-02 19:49:18.673775 expiringsqlitedict-6.2.0/run_all_tests.sh
--rwxr-xr-x   0        0        0    18087 2023-05-03 15:38:04.335548 expiringsqlitedict-6.2.0/src/expiringsqlitedict/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-6.2.0/src/expiringsqlitedict/py.typed
--rwxr-xr-x   0        0        0    14334 2023-05-03 15:37:32.783024 expiringsqlitedict-6.2.0/test.py
--rw-r--r--   0        0        0     4961 1970-01-01 00:00:00.000000 expiringsqlitedict-6.2.0/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-7.0.0/.gitignore
+-rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-7.0.0/.travis.yml
+-rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-7.0.0/CHANGELOG.txt
+-rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-7.0.0/LICENSE.apache
+-rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-7.0.0/LICENSE.rst
+-rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-7.0.0/Makefile
+-rw-r--r--   0        0        0     3702 2023-07-18 21:30:52.504076 expiringsqlitedict-7.0.0/README.md
+-rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-7.0.0/bench.py
+-rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-7.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-7.0.0/docs/conf.py
+-rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-7.0.0/docs/expiringsqlitedict.rst
+-rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-7.0.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-7.0.0/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-7.0.0/docs/requirements.txt
+-rwxr-xr-x   0        0        0     2834 2023-07-18 20:38:10.693561 expiringsqlitedict-7.0.0/justfile
+-rw-r--r--   0        0        0     1253 2023-07-18 21:29:04.584042 expiringsqlitedict-7.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0    23484 2023-07-18 21:28:36.612515 expiringsqlitedict-7.0.0/src/expiringsqlitedict/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-7.0.0/src/expiringsqlitedict/py.typed
+-rwxr-xr-x   0        0        0    14185 2023-07-18 21:27:44.412531 expiringsqlitedict-7.0.0/test.py
+-rw-r--r--   0        0        0     4876 1970-01-01 00:00:00.000000 expiringsqlitedict-7.0.0/PKG-INFO
```

### Comparing `expiringsqlitedict-6.2.0/CHANGELOG.txt` & `expiringsqlitedict-7.0.0/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.2.0/LICENSE.apache` & `expiringsqlitedict-7.0.0/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.2.0/README.rst` & `expiringsqlitedict-7.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,105 @@
-expiringsqlitedict -- expiring file-backed ``dict``
-===================================================
-
-.. _Downloads: https://pypi.python.org/pypi/expiringsqlitedict
-.. _License: https://pypi.python.org/pypi/expiringsqlitedict
+# expiringsqlitedict -- expiring file-backed `dict`
 
 A lightweight wrapper around Python's sqlite3 database with a MutableMapping
-interface::
+interface:
 
-  from expiringsqlitedict import SqliteDict
-  with SqliteDict('./my_db.sqlite') as mydict:
-      mydict['some_key'] = any_picklable_object
-      print(mydict['some_key'])  # prints the new value
-      for key, value in mydict.items():
-          print((key, value))
-      print(len(mydict)) # etc... all dict functions work
+```python
+from expiringsqlitedict import SqliteDict
+with SqliteDict('./my_db.sqlite') as mydict:
+    mydict['some_key'] = any_picklable_object
+    print(mydict['some_key'])  # prints the new value
+    for key, value in mydict.items():
+        print((key, value))
+    print(len(mydict)) # etc... all dict functions work
+```
 
 json is used internally by default to serialize the values. Keys are
 arbitrary strings, values arbitrary json-able objects.  This must be used
 within a context manager, and serialization can be overridden with your own.
 The database is wrapped with a transaction, and any exception thrown out of the
 context manager rolls back all changes.
 
-This was forked off of `sqlitedict <https://github.com/RaRe-Technologies/sqlitedict>`_
+This was forked off of [sqlitedict](https://github.com/RaRe-Technologies/sqlitedict)
 in order to add auto-expiring functionality, and initially was quite similar to
 it.  Version 2.0 split of completely and takes the module into a complete
 rewrite, mostly to remove unnecessary Python 2 compatibility, simplify the API,
 completely enforce a context manager for typical cases, add full typing
 throughout, and use sqlite triggers for expiration cleanup.
 
 Version 3 set the default encoding to json, and made many other API refinements.
 
 This version also does not vacuum at all automatically.  It did in previous
 versions, but this was kind of a silly behavior to put into the library itself.
 If you want your database file intermittently vacuumed, you should put such
-behavior into a crontab or use the ``sqlite3`` module to do it yourself
+behavior into a crontab or use the `sqlite3` module to do it yourself
 intermittently.
 
-Features
---------
+## Features
 
 * Values can be any json-capable objects (this can be customized to be as
   flexible as you need, through custom serializers)
 * Support for access from multiple programs or threads, with locking fully
   managed by sqlite itself.
 * A very simple codebase that is easy to read, relying on sqlite for as much
   behavior as possible.
-* A simple autocommit wrapper (``SimpleSqliteDict``), if you really can't
+* A simple autocommit wrapper (`SimpleSqliteDict`), if you really can't
   handle a context manager and need something that fully handles like a dict.
-  You can specify a ``isolation_level`` on this to have to commit and roll back
+  You can specify a `isolation_level` on this to have to commit and roll back
   yourself.
-* An on-demand wrapper (``OnDemand``), for situations where you want to open and
+* An on-demand wrapper (`OnDemand`), for situations where you want to open and
   close the database in as narrow a window as possible.
 * Support for custom serialization or compression:
 
-.. code-block:: python
-
-  import json
-    
-  with SqliteDict('some.db', serializer=json) as mydict:
-      mydict['some_key'] = some_json_encodable_object
-      print(mydict['some_key'])
+```python
+import orjson
+  
+with SqliteDict('some.db', serializer=orjson) as mydict:
+    mydict['some_key'] = some_json_encodable_object
+    print(mydict['some_key'])
+```
 
-Installation
-------------
+## Installation
 
 The module has no dependencies beyond Python itself.
 
-Install or upgrade with::
-
-    pip install expiringsqlitedict
-
-or from the `source tar.gz <http://pypi.python.org/pypi/expiringsqlitedict>`_::
+Install with pip as usual:
 
-    python setup.py install
+```sh
+pip install expiringsqlitedict
+```
 
-This module is a single file, so you could also easily import the module in your
-own tree, if your workflow needs that.
+## Testing
 
-Testing
--------
-
-You may test this by running ``test.py`` with ``PYTHONPATH`` set to the current
-working directory.  There is a convenience makefile to do this for you when you
+You may test this by running `test.py` with `PYTHONPATH` set to the current
+working directory.  There is a convenience justfile to do this for you when you
 run:
 
-.. code-block:: sh
+```sh
+just test
+```
 
-  make test
+This will run all tests against all supported versions of Python (and 3.6), as
+well as all supported versions of Alpine, CentOS, Debian, Fedora, and Ubuntu
+Linux.
 
-Documentation
--------------
+## Documentation
 
-Standard Python document strings are inside the module::
+[Documentation is available on readthedocs](https://expiringsqlitedict.readthedocs.io/)
 
-  >>> import expiringsqlitedict
-  >>> help(expiringsqlitedict)
+Standard Python document strings are inside the module
 
-Comments, bug reports
----------------------
+```python
+>>> import expiringsqlitedict
+>>> help(expiringsqlitedict)
+```
 
-``expiringsqlitedict`` resides on `github <https://github.com/absperf/expiringsqlitedict>`_. You can file issues or pull
-requests there.
+## Comments, bug reports
 
+`expiringsqlitedict` resides on [github](https://github.com/absperf/expiringsqlitedict). You can file issues or pull
+requests there.
 
 ----
 
-``expiringsqlitedict`` is open source software released under the
-`Apache 2.0 license <http://opensource.org/licenses/apache2.0.php>`_.
-Version <2 Copyright (c) 2011-2018 `Radim Řehůřek <http://radimrehurek.com>`_ and contributors.
-All versions copyright (c) 2018-2022 Absolute Performance, Inc.
+`expiringsqlitedict` is open source software released under the
+[Mozilla Public License 2.0](https://opensource.org/license/mpl-2-0/)
+All versions copyright (c) 2018-2023 Absolute Performance, Inc.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `expiringsqlitedict-6.2.0/bench.py` & `expiringsqlitedict-7.0.0/bench.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.2.0/docs/Makefile` & `expiringsqlitedict-7.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.2.0/docs/conf.py` & `expiringsqlitedict-7.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.2.0/docs/index.rst` & `expiringsqlitedict-7.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.2.0/docs/make.bat` & `expiringsqlitedict-7.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.2.0/src/expiringsqlitedict/__init__.py` & `expiringsqlitedict-7.0.0/src/expiringsqlitedict/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,67 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# This code is distributed under the terms and conditions
-# from the Apache License, Version 2.0
-#
-# http://opensource.org/licenses/apache2.0.php
-#
-# This code was inspired by:
-#  * http://code.activestate.com/recipes/576638-draft-for-an-sqlite3-based-dbm/
-#  * http://code.activestate.com/recipes/526618/
-
 
 import json
+from re import DEBUG
 import sqlite3
-from collections.abc import MutableMapping
+from sqlite3 import sqlite_version_info
 from contextlib import ExitStack, closing, contextmanager
 from datetime import timedelta
 from types import TracebackType
-from typing import Any, Generator, Iterable, Iterator, Optional, Reversible, Tuple, Type
+from typing import Any, Generator, Iterable, Iterator, Optional, Reversible, Tuple, Type, Union, MutableMapping
 from weakref import finalize
 from enum import unique, Enum
 
+class Identifier:
+    '''An auto-escaping identifier similar to a string.
+    '''
+    __slots__ = (
+        '__value',
+    )
+
+    def __init__(self, value: str) -> None:
+        self.__value = value
+
+    @property
+    def value(self) -> str:
+        return self.__value
+
+    def __add__(self, other: Union['Identifier', str]) -> 'Identifier':
+        if isinstance(other, Identifier):
+            other = other.__value
+        return Identifier(self.__value + other)
+
+    def __radd__(self, other: Union['Identifier', str]) -> 'Identifier':
+        if isinstance(other, Identifier):
+            other = other.__value
+        return Identifier(other + self.__value)
+
+    def __iadd__(self, other: Union['Identifier', str]) -> 'Identifier':
+        if isinstance(other, Identifier):
+            other = other.__value
+        self.__value += other
+        return self
+
+    def __contains__(self, other: Union['Identifier', str]) -> bool:
+        if isinstance(other, Identifier):
+            other = other.__value
+        return self.__value.__contains__(other)
+
+    def __hash__(self) -> int:
+        return hash(self.__value)
+
+    def __repr__(self) -> str:
+        return f'<Identifier {self}>'
+
+    def __str__(self) -> str:
+        if b'\x00' in self.__value.encode('utf-8'):
+            raise ValueError("sqlite Identifer must not contain any null bytes")
+
+        return '"' + self.__value.replace('"', '""') + '"'
+
 @unique
 class Order(str, Enum):
     '''An ordering enum for iteration methods.
     '''
 
     ID = 'id'
     KEY = 'key'
@@ -70,15 +107,15 @@
         self._connection = connection
         self._table = table
         self._order = order
     
     def _iterator(self, order: str) -> Iterator[str]:
         with closing(self._connection.cursor()) as cursor:
             for row in cursor.execute(
-                f'SELECT key FROM "{self._table}" ORDER BY {self._order} {order}',
+                f'SELECT key FROM {self._table} ORDER BY {self._order} {order}',
             ):
                 yield row[0]
 
     def __iter__(self) -> Iterator[str]:
         return self._iterator('ASC')
 
     def __reversed__(self) -> Iterator[str]:
@@ -104,15 +141,15 @@
         self._table = table
         self._serializer = serializer
         self._order = order
 
     def _iterator(self, order: str) -> Iterator[Any]:
         with closing(self._connection.cursor()) as cursor:
             for row in cursor.execute(
-                f'SELECT value FROM "{self._table}" ORDER BY {self._order} {order}',
+                f'SELECT value FROM {self._table} ORDER BY {self._order} {order}',
             ):
                 yield self._serializer.loads(row[0])
 
     def __iter__(self) -> Iterator[Any]:
         return self._iterator('ASC')
 
     def __reversed__(self) -> Iterator[Any]:
@@ -137,79 +174,79 @@
         self._table = table
         self._serializer = serializer
         self._order = order
     
     def _iterator(self, order: str) -> Iterator[Tuple[str, Any]]:
         with closing(self._connection.cursor()) as cursor:
             for row in cursor.execute(f'''
-                SELECT key, value FROM "{self._table}"
+                SELECT key, value FROM {self._table}
                     ORDER BY {self._order} {order}
             '''):
                 yield row[0], self._serializer.loads(row[1])
 
     def __iter__(self) -> Iterator[Tuple[str, Any]]:
         return self._iterator('ASC')
 
     def __reversed__(self) -> Iterator[Tuple[str, Any]]:
         return self._iterator('DESC')
 
-class SqliteDict:
-    """
-    Set up the sqlite dictionary manager.
 
-    This needs to be used as a context manager.  It will not operate at all
-    otherwise. args and kwargs are directly passed to sqlite3.connect.  Use
-    these to customize your connection, such as making it read-only.
+class ConnectionManager:
+    """
+    Opens a SQLite connection and yields a TransactionManager.
 
-    This is lazy, and won't even open the database until it is entered.  It may
-    be re-opened after it has closed.
+    On close, this closes the SQLite connection.  This may be entered more than once.
     """
 
     __slots__ = (
         '_args',
         '_kwargs',
         '_connection',
         '_exit_stack',
         '_serializer',
         '_lifespan',
-        '_begin',
+        '_transaction',
         '_table',
-        '__weakref__'
     )
 
     def __init__(self,
         *args,
         serializer: Any = json,
         lifespan: timedelta = timedelta(weeks=1),
         transaction: str = 'IMMEDIATE',
-        table: str = 'expiringsqlitedict',
+        table: Union[str, Identifier] = Identifier('expiringsqlitedict'),
         **kwargs,
     ) -> None:
+        if isinstance(table, str):
+            table = Identifier(table)
+
         self._args = args
         self._kwargs = kwargs
         self._serializer = serializer
         self._lifespan = lifespan
-        self._begin = f'BEGIN {transaction} TRANSACTION'
+        self._transaction = transaction
         self._table = table
 
     @property
     def lifespan(self) -> timedelta:
         '''The current lifespan.
 
         Changing this will change the calculated expiration time of future set
-        items.  It will not retroactively apply to existing items unless you explicitly
-        postpone them.
+        items.  It will not retroactively apply to existing items unless you
+        explicitly postpone them.
         '''
         return self._lifespan
 
     @lifespan.setter
     def lifespan(self, value: timedelta) -> None:
         self._lifespan = value
 
-    def __enter__(self) -> 'Connection':
+    def __enter__(self) -> 'TransactionManager':
+        assert not hasattr(self, '_exit_stack'), 'Can not be entered more than once at a time'
+
         with ExitStack() as exit_stack:
             self._connection = exit_stack.enter_context(closing(sqlite3.connect(
                 *self._args,
                 isolation_level=None,
                 **self._kwargs,
             )))
 
@@ -220,14 +257,89 @@
             def optimize() -> None:
                 with closing(self._connection.cursor()) as cursor:
                     cursor.execute('PRAGMA analysis_limit=8192')
                     cursor.execute('PRAGMA optimize')
 
             exit_stack.callback(optimize)
 
+            transaction_manager = TransactionManager(
+                connection=self._connection,
+                serializer=self._serializer,
+                lifespan=self._lifespan,
+                transaction=self._transaction,
+                table=self._table,
+            )
+                
+            self._exit_stack = exit_stack.pop_all()
+
+            return transaction_manager
+
+        assert False, 'UNREACHABLE'
+
+    def __exit__(
+        self,
+        type: Optional[Type[BaseException]],
+        value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> bool:
+        try:
+            return self._exit_stack.__exit__(type, value, traceback)
+        finally:
+            del self._connection, self._exit_stack
+
+class TransactionManager:
+    """
+    Enters and leaves a transaction for a SQLite dict.
+
+    On close, commits or abandons the transaction.
+    """
+
+    __slots__ = (
+        '_connection',
+        '_exit_stack',
+        '_serializer',
+        '_lifespan',
+        '_begin',
+        '_table',
+    )
+
+    def __init__(self,
+        connection: sqlite3.Connection,
+        serializer: Any = json,
+        lifespan: timedelta = timedelta(weeks=1),
+        transaction: str = 'IMMEDIATE',
+        table: Union[str, Identifier] = Identifier('expiringsqlitedict'),
+    ) -> None:
+        if isinstance(table, str):
+            table = Identifier(table)
+
+        self._connection = connection
+        self._serializer = serializer
+        self._lifespan = lifespan
+        self._begin = f'BEGIN {transaction} TRANSACTION'
+        self._table = table
+
+    @property
+    def lifespan(self) -> timedelta:
+        '''The current lifespan.
+
+        Changing this will change the calculated expiration time of future set
+        items.  It will not retroactively apply to existing items unless you
+        explicitly postpone them.
+        '''
+        return self._lifespan
+
+    @lifespan.setter
+    def lifespan(self, value: timedelta) -> None:
+        self._lifespan = value
+
+    def __enter__(self) -> 'Connection':
+        assert not hasattr(self, '_exit_stack'), 'Can not be entered more than once at a time'
+
+        with ExitStack() as exit_stack:
             exit_stack.enter_context(_transaction(self._connection, self._begin))
 
             connection = Connection(
                 self._connection,
                 serializer=self._serializer,
                 lifespan=self._lifespan,
                 table=self._table,
@@ -244,34 +356,103 @@
         traceback: Optional[TracebackType],
     ) -> bool:
         try:
             return self._exit_stack.__exit__(type, value, traceback)
         finally:
             del self._connection, self._exit_stack
 
-def SimpleSqliteDict(
+class Manager:
+    """
+    Combines ConnectionManager and TransactionManager.
+
+    When entered, this opens the database and starts a transaction, and on exit,
+    it will commit or roll back the transaction and close the database.
+    """
+
+    __slots__ = (
+        '_connection_manager',
+        '_exit_stack',
+    )
+
+    def __init__(self,
+        *args,
+        serializer: Any = json,
+        lifespan: timedelta = timedelta(weeks=1),
+        transaction: str = 'IMMEDIATE',
+        table: Union[str, Identifier] = Identifier('expiringsqlitedict'),
+        **kwargs,
+    ) -> None:
+        self._connection_manager = ConnectionManager(
+            *args,
+            serializer=serializer,
+            lifespan=lifespan,
+            transaction=transaction,
+            table=table,
+            **kwargs
+        )
+
+    @property
+    def lifespan(self) -> timedelta:
+        '''The current lifespan.
+
+        Changing this will change the calculated expiration time of future set
+        items.  It will not retroactively apply to existing items unless you
+        explicitly postpone them.
+        '''
+        return self._connection_manager.lifespan
+
+    @lifespan.setter
+    def lifespan(self, value: timedelta) -> None:
+        self._connection_manager.lifespan = value
+
+    def __enter__(self) -> 'Connection':
+        assert not hasattr(self, '_exit_stack'), 'Can not be entered more than once at a time'
+
+        with ExitStack() as exit_stack:
+            transaction_manager = exit_stack.enter_context(self._connection_manager)
+            connection = exit_stack.enter_context(transaction_manager)
+            self._exit_stack = exit_stack.pop_all()
+            return connection
+
+        assert False, 'UNREACHABLE'
+
+    def __exit__(
+        self,
+        type: Optional[Type[BaseException]],
+        value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> bool:
+        try:
+            return self._exit_stack.__exit__(type, value, traceback)
+        finally:
+            del self._connection_manager, self._exit_stack
+
+def Simple(
     *args,
     serializer: Any = json,
     lifespan: timedelta = timedelta(weeks=1),
     isolation_level: Optional[str] = None,
-    table: str = 'expiringsqlitedict',
+    table: Union[str, Identifier] = Identifier('expiringsqlitedict'),
     **kwargs,
 ) -> 'Connection':
     """
     Set up the sqlite dictionary manager as a non-contextmanager with a finalizer.
 
     If you set the isolation_level, you will be responsible for calling
     d.connection.commit() and d.connection.rollback() appropriately.
     """
 
     db = sqlite3.connect(*args, isolation_level=isolation_level, **kwargs)
     with closing(db.cursor()) as cursor:
         cursor.execute('PRAGMA journal_mode=WAL')
         cursor.execute('PRAGMA synchronous=NORMAL')
 
+    if isinstance(table, str):
+        table = Identifier(table)
+
     connection = Connection(
         db,
         serializer=serializer,
         lifespan=lifespan,
         table=table,
     )
 
@@ -284,56 +465,57 @@
 
     finalize(connection, _close)
 
     return connection
 
 _trailers = []
 
-if sqlite3.sqlite_version_info >= (3, 37):
+if sqlite_version_info >= (3, 37):
     _trailers.append('STRICT')
     _valuetype = 'ANY'
 else:
     _valuetype = 'BLOB'
 
 _trailer = ', '.join(_trailers)
 
-if sqlite3.sqlite_version_info >= (3, 38):
+if sqlite_version_info >= (3, 38):
     _unixepoch = 'UNIXEPOCH()'
 else:
     _unixepoch = "CAST(strftime('%s', 'now') AS INTEGER)"
 
 APPLICATION_ID = 1820903862
 
-class Connection(MutableMapping):
-    '''The actual connection object, as a MutableMapping[str, Any].
+class Connection(MutableMapping[str, Any]):
+    '''The actual connection object.
 
     Items are expired when a value is inserted or updated.  Deletion or
     postponement does not expire items.
     '''
 
     __slots__ = (
         '_lifespan',
         '_serializer',
         '_connection',
         '_table',
-        '_safe_table',
         '__weakref__',
     )
 
     def __init__(self,
         connection: sqlite3.Connection,
         serializer: Any = json,
         lifespan: timedelta = timedelta(weeks=1),
-        table: str = 'expiringsqlitedict',
+        table: Union[str, Identifier] = Identifier('expiringsqlitedict'),
     ) -> None:
+        if isinstance(table, str):
+            table = Identifier(table)
+
         self._lifespan = lifespan.total_seconds()
         self._serializer = serializer
         self._connection = connection
         self._table = table
-        self._safe_table = table.replace('"', '""')
 
         with closing(self._connection.cursor()) as cursor:
             application_id = next(cursor.execute('PRAGMA application_id'))[0]
             if application_id == 0:
                 cursor.execute(f'PRAGMA application_id = {APPLICATION_ID}')
             elif application_id != APPLICATION_ID:
                 raise ValueError(f'illegal application ID {application_id}')
@@ -342,75 +524,76 @@
 
             if user_version < 1:
                 # Attempt to migrate, because of pre-6.1 versions.  We can't
                 # otherwise tell the difference between a fresh database and a
                 # pre-set one.
                 cursor.execute(
                     "SELECT 1 FROM sqlite_master WHERE type='table' AND name=?",
-                    (self._table,),
+                    (self._table.value,),
                 )
                 migrate = bool(cursor.fetchall())
 
                 if migrate:
                     cursor.execute(f'''
-                        DROP INDEX IF EXISTS "{self._safe_table}_expire_index"
+                        DROP INDEX IF EXISTS {self._table + "_expire_index"}
                     ''')
                     cursor.execute(f'''
-                        DROP TRIGGER IF EXISTS "{self._safe_table}_insert_trigger"
+                        DROP TRIGGER IF EXISTS {self._table + "_insert_trigger"}
                     ''')
                     cursor.execute(f'''
-                        DROP TRIGGER IF EXISTS "{self._safe_table}_update_trigger"
+                        DROP TRIGGER IF EXISTS {self._table + "_update_trigger"}
                     ''')
                     cursor.execute(f'''
-                        ALTER TABLE "{self._safe_table}"
-                        RENAME TO "{self._safe_table}_v0"
+                        ALTER TABLE {self._table}
+                        RENAME TO {self._table + "_v0"}
                     ''')
 
-
+                # Use autoincrement to make this sort like a standard python
+                # dictionary, with new keys always coming last.
                 cursor.execute(f'''
-                    CREATE TABLE "{self._safe_table}" (
+                    CREATE TABLE {self._table} (
                         id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL,
                         key TEXT UNIQUE NOT NULL,
                         expire INTEGER NOT NULL,
                         value {_valuetype} NOT NULL){_trailer}
                 ''')
 
                 cursor.execute(f'''
-                    CREATE INDEX "{self._safe_table}_expire_index"
-                     ON "{self._safe_table}" (expire)
+                    CREATE INDEX {self._table + "_expire_index"}
+                     ON {self._table} (expire)
                 ''')
 
                 cursor.execute(
                     f'''
-                    CREATE TRIGGER "{self._safe_table}_insert_trigger"
-                        AFTER INSERT ON "{self._safe_table}"
+                    CREATE TRIGGER {self._table + "_insert_trigger"}
+                        AFTER INSERT ON {self._table}
                     BEGIN
-                        DELETE FROM "{self._safe_table}" WHERE expire <= {_unixepoch};
+                        DELETE FROM {self._table} WHERE expire <= {_unixepoch};
                     END
                     '''
                 )
 
                 cursor.execute(
                     f'''
-                    CREATE TRIGGER "{self._safe_table}_update_trigger"
-                        AFTER UPDATE OF value ON "{self._safe_table}"
+                    CREATE TRIGGER {self._table + "_update_trigger"}
+                        AFTER UPDATE OF value ON {self._table}
                     BEGIN
-                        DELETE FROM "{self._safe_table}" WHERE expire <= {_unixepoch};
+                        DELETE FROM {self._table} WHERE expire <= {_unixepoch};
                     END
                     '''
                 )
 
                 if migrate:
                     cursor.execute(f'''
-                        INSERT INTO "{self._safe_table}"
+                        INSERT INTO {self._table}
                             (key, expire, value)
                         SELECT key, expire, value
-                            FROM "{self._safe_table}_v0"
+                            FROM {self._table + "_v0"}
                     ''')
-                    cursor.execute(f'DROP TABLE "{self._safe_table}_v0"')
+                    cursor.execute(f'DROP TABLE {self._table + "_v0"}')
 
                 cursor.execute('PRAGMA user_version = 1')
 
                 user_version = 1
 
             if user_version > 1:
                 raise ValueError(
@@ -436,30 +619,30 @@
         self._lifespan = value.total_seconds()
 
     def __len__(self) -> int:
         '''Get the count of keys in the table.
         '''
 
         with closing(self._connection.cursor()) as cursor:
-            for row in cursor.execute(f'SELECT COUNT(*) FROM "{self._safe_table}"'):
+            for row in cursor.execute(f'SELECT COUNT(*) FROM {self._table}'):
                 return row[0]
         return 0
 
     def __bool__(self) -> bool:
         '''Check if the table is not empty.'''
 
         return len(self) > 0
 
     def keys(self, order: Order = Order.ID) -> _Keys:
         '''Iterate over keys in the table.
         '''
 
         return _Keys(
             connection=self._connection,
-            table=self._safe_table,
+            table=self._table,
             order=order,
         )
 
     def __iter__(self) -> Iterator[str]:
         return iter(self.keys())
 
     def __reversed__(self) -> Iterator[str]:
@@ -467,112 +650,112 @@
 
     def values(self, order: Order = Order.ID) -> _Values:
         '''Iterate over values in the table.
         '''
 
         return _Values(
             connection=self._connection,
-            table=self._safe_table,
+            table=self._table,
             serializer=self._serializer,
             order=order,
         )
 
     def items(self, order: Order = Order.ID) -> _Items:
         '''Iterate over keys and values in the table.
         '''
 
         return _Items(
             connection=self._connection,
-            table=self._safe_table,
+            table=self._table,
             serializer=self._serializer,
             order=order,
         )
 
     def __contains__(self, key: str) -> bool:
         '''Check if the table contains the given key.
         '''
 
         with closing(self._connection.cursor()) as cursor:
             for _ in cursor.execute(
-                f'SELECT 1 FROM "{self._safe_table}" WHERE key = ?',
+                f'SELECT 1 FROM {self._table} WHERE key = ?',
                 (key,),
             ):
                 return True
         return False
 
     def __getitem__(self, key: str) -> Any:
         '''Fetch the key.
         '''
 
         with closing(self._connection.cursor()) as cursor:
             for row in cursor.execute(
-                f'SELECT value FROM "{self._safe_table}" WHERE key = ?', (key,)
+                f'SELECT value FROM {self._table} WHERE key = ?', (key,)
             ):
                 return self._serializer.loads(row[0])
         raise KeyError(key)
 
     def __setitem__(self, key: str, value: Any) -> None:
         '''Set or replace the item.
 
         This also triggers cleaning up expired values.
         '''
 
         with closing(self._connection.cursor()) as cursor:
-            if sqlite3.sqlite_version_info >= (3, 24):
+            if sqlite_version_info >= (3, 24):
                 cursor.execute(f'''
-                        INSERT INTO "{self._safe_table}" (key, expire, value)
+                        INSERT INTO {self._table} (key, expire, value)
                             VALUES (?, {_unixepoch} + ?, ?)
                             ON CONFLICT (key) DO UPDATE
                             SET value=excluded.value, expire=excluded.expire
                     ''',
                     (key, self._lifespan, self._serializer.dumps(value)),
                 )
             elif key in self:
                 cursor.execute(f'''
-                        UPDATE "{self._safe_table}"
+                        UPDATE {self._table}
                             SET expire={_unixepoch} + ?,
                                 value=?
                             WHERE key=?
                     ''',
                     (self._lifespan, self._serializer.dumps(value), key),
                 )
             else:
                 cursor.execute(f'''
-                        INSERT INTO "{self._safe_table}" (key, expire, value)
+                        INSERT INTO {self._table} (key, expire, value)
                             VALUES (?, {_unixepoch} + ?, ?)
                     ''',
                     (key, self._lifespan, self._serializer.dumps(value)),
                 )
 
     def __delitem__(self, key: str) -> None:
         '''Delete an item from the table.
         '''
 
         with closing(self._connection.cursor()) as cursor:
-            cursor.execute(f'DELETE FROM "{self._safe_table}" WHERE key=?', (key,))
+            cursor.execute(f'DELETE FROM {self._table} WHERE key=?', (key,))
             if cursor.rowcount != 1:
                 raise KeyError(key)
 
     def clear(self) -> None:
         '''Delete all items from the table.
         '''
 
         with closing(self._connection.cursor()) as cursor:
-            cursor.execute(f'DELETE FROM "{self._safe_table}"')
+            cursor.execute(f'DELETE FROM {self._table}')
 
     def postpone(self, key: str) -> None:
         '''Push back the expiration date of the given entry, if it exists.
         '''
         with closing(self._connection.cursor()) as cursor:
             cursor.execute(
-                f'UPDATE "{self._safe_table}" SET expire={_unixepoch} + ? WHERE key=?',
+                f'UPDATE {self._table} SET expire={_unixepoch} + ? WHERE key=?',
                 (self._lifespan, key),
             )
 
     def postpone_all(self) -> None:
         '''Push back the expiration date of all entries at once.
         '''
         with closing(self._connection.cursor()) as cursor:
             cursor.execute(
-                f'UPDATE "{self._safe_table}" SET expire={_unixepoch} + ?',
+                f'UPDATE {self._table} SET expire={_unixepoch} + ?',
                 (self._lifespan,),
             )
```

