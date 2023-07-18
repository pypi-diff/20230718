# Comparing `tmp/litequeue-0.6.tar.gz` & `tmp/litequeue-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litequeue-0.6.tar", last modified: Sun Feb 12 22:34:27 2023, max compression
+gzip compressed data, was "litequeue-0.7.tar", last modified: Tue Jul 18 10:47:58 2023, max compression
```

## Comparing `litequeue-0.6.tar` & `litequeue-0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-12 22:34:27.481936 litequeue-0.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1066 2023-02-12 22:34:02.000000 litequeue-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-02-12 22:34:27.481936 litequeue-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-02-12 22:34:02.000000 litequeue-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-12 22:34:27.481936 litequeue-0.6/litequeue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-02-12 22:34:27.000000 litequeue-0.6/litequeue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-02-12 22:34:27.000000 litequeue-0.6/litequeue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-12 22:34:27.000000 litequeue-0.6/litequeue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-02-12 22:34:27.000000 litequeue-0.6/litequeue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    17703 2023-02-12 22:34:02.000000 litequeue-0.6/litequeue.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-12 22:34:27.481936 litequeue-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      747 2023-02-12 22:34:02.000000 litequeue-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:47:58.813739 litequeue-0.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1066 2023-07-18 10:47:24.000000 litequeue-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-07-18 10:47:58.813739 litequeue-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-07-18 10:47:24.000000 litequeue-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:47:58.813739 litequeue-0.7/litequeue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-07-18 10:47:58.000000 litequeue-0.7/litequeue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-07-18 10:47:58.000000 litequeue-0.7/litequeue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 10:47:58.000000 litequeue-0.7/litequeue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-18 10:47:58.000000 litequeue-0.7/litequeue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    17840 2023-07-18 10:47:24.000000 litequeue-0.7/litequeue.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 10:47:58.813739 litequeue-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2023-07-18 10:47:24.000000 litequeue-0.7/setup.py
```

### Comparing `litequeue-0.6/LICENSE` & `litequeue-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `litequeue-0.6/PKG-INFO` & `litequeue-0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litequeue
-Version: 0.6
+Version: 0.7
 Summary: Simple queue built on top of SQLite
 Home-page: https://github.com/litements/litequeue
 Author: Ricardo Ander-Egg Aguilar
 Author-email: rsubacc@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 
 > Queue implemented on top of SQLite
 
 ## Why?
 
 You can use this to implement a persistent queue. It also has extra timing
 metrics for the messages/tasks, and the api to set a message as **done** lets
-you specifiy the `task_id` to be set as done.
+you specifiy the `message_id` to be set as done.
 
 Since it's all based on SQLite / SQL, it is easily extendable.
 
 Messages are always passed as strings, so you can use json data as messages.
 Messages are interpreted as tasks, so after you `pop` a message, you need to
 mark it as done when you finish processing it. When you run the `.prune()`
 method, it will remove all the finished tasks from the database.
@@ -76,16 +76,16 @@
 - Easy to extend using SQL
 
 ## Examples and bechmarks and bechmarks
 
 You can have a look at the `test.py` file. The tests are short and showcase
 different usage scenarios.
 
-The `benchmarks.ipynb` file contains some benchmarks comparing `litequeue` to
-the built-in Python `Queue`.
+The `benchmark.ipynb` file contains some benchmarks comparing `litequeue` to
+the built-in Python `queue.Queue`.
 
 ## Meta
 
 Ricardo Ander-Egg Aguilar – [@ricardoanderegg](https://twitter.com/ricardoanderegg) –
 
 - [ricardoanderegg.com](http://ricardoanderegg.com/)
 - [github.com/polyrand](https://github.com/polyrand/)
@@ -102,9 +102,9 @@
 - In version 0.4 the database schema has changed and the column `task_id` is now `message_id`.
 
 ## Contributing
 
 The only hard rules for the project are:
 
 - No extra dependencies allowed
-- No extra files, everything must be inside the main module's `.py` file.
-- Tests must be inside the `tests.ipynb` notebook.
+- No extra files, everything must be inside `litequeue.py` file.
+- Tests must be inside the `test.py` file.
```

### Comparing `litequeue-0.6/README.md` & `litequeue-0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 > Queue implemented on top of SQLite
 
 ## Why?
 
 You can use this to implement a persistent queue. It also has extra timing
 metrics for the messages/tasks, and the api to set a message as **done** lets
-you specifiy the `task_id` to be set as done.
+you specifiy the `message_id` to be set as done.
 
 Since it's all based on SQLite / SQL, it is easily extendable.
 
 Messages are always passed as strings, so you can use json data as messages.
 Messages are interpreted as tasks, so after you `pop` a message, you need to
 mark it as done when you finish processing it. When you run the `.prune()`
 method, it will remove all the finished tasks from the database.
@@ -64,16 +64,16 @@
 - Easy to extend using SQL
 
 ## Examples and bechmarks and bechmarks
 
 You can have a look at the `test.py` file. The tests are short and showcase
 different usage scenarios.
 
-The `benchmarks.ipynb` file contains some benchmarks comparing `litequeue` to
-the built-in Python `Queue`.
+The `benchmark.ipynb` file contains some benchmarks comparing `litequeue` to
+the built-in Python `queue.Queue`.
 
 ## Meta
 
 Ricardo Ander-Egg Aguilar – [@ricardoanderegg](https://twitter.com/ricardoanderegg) –
 
 - [ricardoanderegg.com](http://ricardoanderegg.com/)
 - [github.com/polyrand](https://github.com/polyrand/)
@@ -90,9 +90,9 @@
 - In version 0.4 the database schema has changed and the column `task_id` is now `message_id`.
 
 ## Contributing
 
 The only hard rules for the project are:
 
 - No extra dependencies allowed
-- No extra files, everything must be inside the main module's `.py` file.
-- Tests must be inside the `tests.ipynb` notebook.
+- No extra files, everything must be inside `litequeue.py` file.
+- Tests must be inside the `test.py` file.
```

### Comparing `litequeue-0.6/litequeue.egg-info/PKG-INFO` & `litequeue-0.7/litequeue.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litequeue
-Version: 0.6
+Version: 0.7
 Summary: Simple queue built on top of SQLite
 Home-page: https://github.com/litements/litequeue
 Author: Ricardo Ander-Egg Aguilar
 Author-email: rsubacc@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 
 > Queue implemented on top of SQLite
 
 ## Why?
 
 You can use this to implement a persistent queue. It also has extra timing
 metrics for the messages/tasks, and the api to set a message as **done** lets
-you specifiy the `task_id` to be set as done.
+you specifiy the `message_id` to be set as done.
 
 Since it's all based on SQLite / SQL, it is easily extendable.
 
 Messages are always passed as strings, so you can use json data as messages.
 Messages are interpreted as tasks, so after you `pop` a message, you need to
 mark it as done when you finish processing it. When you run the `.prune()`
 method, it will remove all the finished tasks from the database.
@@ -76,16 +76,16 @@
 - Easy to extend using SQL
 
 ## Examples and bechmarks and bechmarks
 
 You can have a look at the `test.py` file. The tests are short and showcase
 different usage scenarios.
 
-The `benchmarks.ipynb` file contains some benchmarks comparing `litequeue` to
-the built-in Python `Queue`.
+The `benchmark.ipynb` file contains some benchmarks comparing `litequeue` to
+the built-in Python `queue.Queue`.
 
 ## Meta
 
 Ricardo Ander-Egg Aguilar – [@ricardoanderegg](https://twitter.com/ricardoanderegg) –
 
 - [ricardoanderegg.com](http://ricardoanderegg.com/)
 - [github.com/polyrand](https://github.com/polyrand/)
@@ -102,9 +102,9 @@
 - In version 0.4 the database schema has changed and the column `task_id` is now `message_id`.
 
 ## Contributing
 
 The only hard rules for the project are:
 
 - No extra dependencies allowed
-- No extra files, everything must be inside the main module's `.py` file.
-- Tests must be inside the `tests.ipynb` notebook.
+- No extra files, everything must be inside `litequeue.py` file.
+- Tests must be inside the `test.py` file.
```

### Comparing `litequeue-0.6/litequeue.py` & `litequeue-0.7/litequeue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-import pprint
+import os
 import pathlib
-from typing import Callable, Dict, Iterable, Optional, Union, Any, cast
+import pprint
 import sqlite3
-from contextlib import contextmanager
-from enum import Enum
-from dataclasses import dataclass
 import sys
 import time
-import os
+from contextlib import contextmanager
+from dataclasses import dataclass
+from enum import Enum
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import Iterable
+from typing import Optional
+from typing import Union
+from typing import cast
 
 _DKW: Dict[str, Any] = {}
 if sys.version_info >= (3, 10):
     _DKW["slots"] = True
 
-__version__ = "0.6"
+__version__ = "0.7"
 
 # Extracted from https://github.com/stevesimmons/uuid7 under MIT license
 
 # Expose function used by uuid7() to get current time in nanoseconds
 # since the Unix epoch.
 time_ns = time.time_ns
 
 
-def _now() -> int:
-    return time_ns()
-
-
 def uuid7(
-    time_func: Callable[[], int] = time_ns,
     _last=[0, 0, 0, 0],  # noqa
     _last_as_of=[0, 0, 0, 0],  # noqa
 ) -> str:
     """
     UUID v7, following the proposed extension to RFC4122 described in
     https://www.ietf.org/id/draft-peabody-dispatch-new-uuid-format-02.html.
     All representations sort chronologically, with a potential time resolution
@@ -75,15 +76,15 @@
     Examples
     --------
     >>> uuid7()
     '061cb26a-54b8-7a52-8000-2124e7041024'
     >>> uuid7(0)
     '00000000-0000-0000-0000-00000000000'
     """
-    ns = time_func()
+    ns = time_ns()
     last = _last
 
     if ns == 0:
         # Special cose for all-zero uuid. Strictly speaking not a UUIDv7.
         t1 = t2 = t3 = t4 = 0
         rand = b"\0" * 6
     else:
@@ -196,22 +197,22 @@
 
         if self.maxsize is not None:
             self.conn.execute(
                 f"""
 CREATE TRIGGER IF NOT EXISTS maxsize_control
    BEFORE INSERT
    ON Queue
-   WHEN (SELECT COUNT(*) FROM Queue WHERE status = {MessageStatus.READY}) >= {self.maxsize}
+   WHEN (SELECT COUNT(*) FROM Queue WHERE status = {MessageStatus.READY.value}) >= {self.maxsize}
 BEGIN
     SELECT RAISE (ABORT,'Max queue length reached: {self.maxsize}');
 END;"""
             )
 
     def get_sqlite_version(self) -> int:
-        sqlite_ver = sqlite3.sqlite_version.split(".")
+        sqlite_ver = sqlite3.sqlite_version_info
 
         v_major = int(sqlite_ver[0])
         v_min = int(sqlite_ver[1])
         # _v_bug = int(sqlite_ver[2])
 
         assert v_major == 3
 
@@ -236,21 +237,21 @@
 
     def put(self, data: str) -> Message:
         """
         Insert a new message
         """
         # timeout: int = None
         message_id: str = cast(str, uuid7())
-        now = _now()
+        now = time_ns()
 
         _cursor = self.conn.execute(  # noqa
             f"""
             INSERT INTO
-              Queue(  data,  message_id, status,                 in_time, lock_time, done_time )
-            VALUES ( :data, :message_id, {MessageStatus.READY}, :now    , NULL     , NULL      )
+              Queue(  data,  message_id, status,                      in_time, lock_time, done_time )
+            VALUES ( :data, :message_id, {MessageStatus.READY.value}, :now    , NULL     , NULL      )
             """.strip(),
             {"data": data, "message_id": message_id, "now": now},
         )
 
         return Message(
             data=data,
             message_id=message_id,
@@ -262,23 +263,23 @@
 
     def _pop_returning(self) -> Optional[Message]:
         # this should happen all inside a single transaction
         with self.transaction(mode="IMMEDIATE"):
             message = self.conn.execute(
                 f"""
                  UPDATE Queue
-                 SET status = {MessageStatus.LOCKED}, lock_time = :now
+                 SET status = {MessageStatus.LOCKED.value}, lock_time = :now
                  WHERE rowid = (SELECT rowid
                                 FROM Queue
-                                WHERE status = {MessageStatus.READY}
+                                WHERE status = {MessageStatus.READY.value}
                                 ORDER BY message_id
                                 LIMIT 1)
                  RETURNING *
                  """,
-                {"now": _now()},
+                {"now": time_ns()},
             ).fetchone()
 
             if not message:
                 return None
 
             return Message(**message)
 
@@ -303,32 +304,32 @@
             # * Using the "IMMEDIATE" mode for the transaction, which locks the database immediately.
             # * When doing the UPDATE statement, the condition checks the status again.
             message = self.conn.execute(
                 f"""
             SELECT * FROM Queue
             WHERE rowid = (SELECT rowid
                            FROM Queue
-                           WHERE status = {MessageStatus.READY}
+                           WHERE status = {MessageStatus.READY.value}
                            ORDER BY message_id
                            LIMIT 1)
             """.strip(),
-                {"status": MessageStatus.READY},
+                {"status": MessageStatus.READY.value},
             ).fetchone()
 
             if message is None:
                 return None
 
-            lock_time = _now()
+            lock_time = time_ns()
 
             self.conn.execute(
                 f"""
                 UPDATE Queue SET
-                  status = {MessageStatus.LOCKED}
+                  status = {MessageStatus.LOCKED.value}
                   , lock_time = :lock_time
-                WHERE message_id = :message_id AND status = {MessageStatus.READY}
+                WHERE message_id = :message_id AND status = {MessageStatus.READY.value}
                 """.strip(),
                 {
                     "lock_time": lock_time,
                     "message_id": message["message_id"],
                 },
             )
 
@@ -343,99 +344,97 @@
                 done_time=message["done_time"],
             )
 
     def peek(self) -> Optional[Message]:
         "Show next message to be popped, if any."
 
         value = self.conn.execute(
-            f"SELECT * FROM Queue WHERE status = {MessageStatus.READY} ORDER BY message_id LIMIT 1",
+            f"SELECT * FROM Queue WHERE status = {MessageStatus.READY.value} ORDER BY message_id LIMIT 1",
         ).fetchone()
 
         return Message(**value) if value is not None else None
 
     def get(self, message_id: str) -> Optional[Message]:
         "Get a message by its `message_id`"
 
         value = self.conn.execute(
             "SELECT * FROM Queue WHERE message_id = :message_id",
             {"message_id": message_id},
         ).fetchone()
 
         return Message(**value) if value is not None else None
 
-    def done(self, message_id) -> int:
+    def done(self, message_id) -> Optional[int]:
         """
         Mark message as done.
         If executed multiple times, `done_time` will be
         the last time this function is called.
         """
 
-        now = _now()
+        now = time_ns()
 
         x = self.conn.execute(
             f"""
             UPDATE Queue SET
-              status = {MessageStatus.DONE}
+              status = {MessageStatus.DONE.value}
               , done_time = :now
             WHERE message_id = :message_id
             """.strip(),
             {"now": now, "message_id": message_id},
         ).lastrowid
 
-        assert x
         return x
 
-    def mark_failed(self, message_id) -> int:
+    def mark_failed(self, message_id) -> Optional[int]:
         """
         Mark a message as failed.
         """
 
         x = self.conn.execute(
             f"""
             UPDATE Queue SET
-              status = {MessageStatus.FAILED}
+              status = {MessageStatus.FAILED.value}
               , done_time = :now
             WHERE message_id = :message_id
             """.strip(),
-            {"now": _now(), "message_id": message_id},
+            {"now": time_ns(), "message_id": message_id},
         ).lastrowid
 
-        assert x
         return x
 
     def list_locked(self, threshold_seconds: int) -> Iterable[Message]:
         """
         Return all the tasks that have been in the `LOCKED` state for more than
         `threshold_seconds` seconds.
         """
 
         threshold_nanoseconds = threshold_seconds * 1e9
 
         cursor = self.conn.execute(
             f"""
             SELECT * FROM Queue
             WHERE
-              status = {MessageStatus.LOCKED}
+              status = {MessageStatus.LOCKED.value}
               AND  lock_time < :time_value
             """.strip(),
-            {"time_value": _now() - threshold_nanoseconds},
+            {"time_value": time_ns() - threshold_nanoseconds},
         )
 
         for result in cursor:
             yield Message(**result)
 
     def retry(self, message_id) -> int:
         """
         Mark a locked message as free again.
         """
 
         x = self.conn.execute(
             f"""
             UPDATE Queue SET
-              status = {MessageStatus.READY}
+              status = {MessageStatus.READY.value}
               , done_time = NULL
             WHERE message_id = :message_id
             """.strip(),
             {"message_id": message_id},
         ).lastrowid
 
         assert x
@@ -445,56 +444,56 @@
         """
         Get current size of the queue.
         """
 
         cursor = self.conn.execute(
             f"""
         SELECT COUNT(*) FROM Queue
-        WHERE status NOT IN ({MessageStatus.DONE}, {MessageStatus.FAILED})
+        WHERE status NOT IN ({MessageStatus.DONE.value}, {MessageStatus.FAILED.value})
         """.strip()
         )
 
         return next(cursor)[0]
 
     def empty(self) -> bool:
         """
         Return True if the queue is empty.
         """
 
         value = self.conn.execute(
-            f"SELECT COUNT(*) as cnt FROM Queue WHERE status = {MessageStatus.READY}"
+            f"SELECT COUNT(*) as cnt FROM Queue WHERE status = {MessageStatus.READY.value}"
         ).fetchone()
         return not bool(value["cnt"])
 
     def full(self) -> bool:
         """
         Return True if the queue is full.
         """
 
         # Here I need to check compared to the maxsize value
         # If maxsize is not set, the queue can grow forever
         if self.maxsize is None:
             return False
 
         value = self.conn.execute(
-            f"SELECT COUNT(*) as cnt FROM Queue WHERE status = {MessageStatus.READY}"
+            f"SELECT COUNT(*) as cnt FROM Queue WHERE status = {MessageStatus.READY.value}"
         ).fetchone()
 
         if value["cnt"] >= self.maxsize:
             return True
         else:
             return False
 
     def prune(self):
         """
         Delete `done` and `failed` messages. # TODO: maybe not failed ones
         """
 
         self.conn.execute(
-            f"DELETE FROM Queue WHERE status IN ({MessageStatus.DONE}, {MessageStatus.FAILED})"
+            f"DELETE FROM Queue WHERE status IN ({MessageStatus.DONE.value}, {MessageStatus.FAILED.value})"
         )
 
         return
 
     def vacuum(self):
         """
         Vacuum the database.
```

### Comparing `litequeue-0.6/setup.py` & `litequeue-0.7/setup.py`

 * *Files identical despite different names*

