# Comparing `tmp/mysqlx-1.5.4.tar.gz` & `tmp/mysqlx-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.5.4.tar", last modified: Sun Jul 16 06:59:38 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.5.5.tar", last modified: Tue Jul 18 09:48:03 2023, max compression
```

## Comparing `mysqlx-1.5.4.tar` & `mysqlx-1.5.5.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:38.000000 mysqlx-1.5.4/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.5.4/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx/
--rw-rw-rw-   0        0        0      693 2023-07-15 12:20:26.000000 mysqlx-1.5.4/mysqlx/constant.py
--rw-rw-rw-   0        0        0    19264 2023-07-15 12:24:01.000000 mysqlx-1.5.4/mysqlx/db.py
--rw-rw-rw-   0        0        0    13298 2023-07-14 21:56:44.000000 mysqlx-1.5.4/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 mysqlx-1.5.4/mysqlx/log_support.py
--rw-rw-rw-   0        0        0    37397 2023-07-16 02:08:48.000000 mysqlx-1.5.4/mysqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.4/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0     4077 2023-07-13 04:01:58.000000 mysqlx-1.5.4/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6416 2023-07-15 12:25:21.000000 mysqlx-1.5.4/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.4/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 04:06:39.000000 mysqlx-1.5.4/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4329 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      365 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4329 2023-07-16 06:59:38.000000 mysqlx-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     3804 2023-07-16 02:24:38.000000 mysqlx-1.5.4/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-16 06:59:38.000000 mysqlx-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1211 2023-07-16 06:59:10.000000 mysqlx-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:48:03.000000 mysqlx-1.5.5/
+drwxrwxrwx   0        0        0        0 2023-07-18 09:48:03.000000 mysqlx-1.5.5/mysqlx/
+-rw-rw-rw-   0        0        0      703 2023-07-18 09:45:34.000000 mysqlx-1.5.5/mysqlx/constant.py
+-rw-rw-rw-   0        0        0    19262 2023-07-16 17:16:35.000000 mysqlx-1.5.5/mysqlx/db.py
+-rw-rw-rw-   0        0        0    13298 2023-07-14 21:56:44.000000 mysqlx-1.5.5/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 mysqlx-1.5.5/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0    38032 2023-07-18 09:45:34.000000 mysqlx-1.5.5/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.5/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     4077 2023-07-13 04:01:58.000000 mysqlx-1.5.5/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     6461 2023-07-17 09:31:46.000000 mysqlx-1.5.5/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.5/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:48:03.000000 mysqlx-1.5.5/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-18 09:48:03.000000 mysqlx-1.5.5/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 09:48:03.000000 mysqlx-1.5.5/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4306 2023-07-18 09:48:03.000000 mysqlx-1.5.5/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-18 09:48:03.000000 mysqlx-1.5.5/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      357 2023-07-18 09:48:03.000000 mysqlx-1.5.5/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 09:48:03.000000 mysqlx-1.5.5/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4306 2023-07-18 09:48:03.000000 mysqlx-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3804 2023-07-16 02:24:38.000000 mysqlx-1.5.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-18 09:48:03.000000 mysqlx-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1211 2023-07-18 09:47:35.000000 mysqlx-1.5.5/setup.py
```

### Comparing `mysqlx-1.5.4/mysqlx/db.py` & `mysqlx-1.5.5/mysqlx/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,20 +43,19 @@
         kwargs['pool_size'] = pool_size
         if 'pool_name' not in kwargs:
             kwargs['pool_name'] = "{}_pool".format(database)
 
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
-
         if MAPPER_PATH in kwargs:
             from .dbx import load_mapper
             load_mapper(kwargs.pop(MAPPER_PATH))
-
         _DB_CTX = DBCtx(connect=lambda: connect(**kwargs), use_mysql_connector=use_mysql_connector)
+
     if is_pool:
         logger.info('Init db engine <%s> ok with connection pool size: %d.' % (hex(id(_DB_CTX)), pool_size))
     else:
         logger.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
 
 
 def connection():
```

### Comparing `mysqlx-1.5.4/mysqlx/dbx.py` & `mysqlx-1.5.5/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.4/mysqlx/log_support.py` & `mysqlx-1.5.5/mysqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.4/mysqlx/orm.py` & `mysqlx-1.5.5/mysqlx/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from datetime import datetime
 from .snowflake import get_id
 from enum import Enum, IntEnum
 from functools import lru_cache
-from .support import DBError, simple_sql
+from .support import DBError, simple_sql, NotFoundError
 from typing import Sequence, Union, List, Tuple
-from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, SYMBOLS, BETWEEN, LIKE, IN, PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY, \
+from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, SYMBOLS, BETWEEN, LIKE, IN, IS, PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY, \
     COLUMN_SQL, CONFIG_DICT, CACHE_SIZE
 from .db import do_get_limit, do_query, do_query_one_limit, do_execute, insert, save, do_select, do_select_one_limit, transaction, batch_insert, \
     do_query_page, do_select_page, do_get
 from .log_support import logger, orm_page_log, orm_insert_log, orm_by_log, orm_delete_by_id_log, orm_by_page_log, orm_inst_log, orm_find_by_id_log, \
     orm_logical_delete_by_ids_log, orm_count_log, orm_find_log, orm_find_by_ids_log
 
 
@@ -94,29 +94,32 @@
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
         pk = self._get_pk()
         _id = self.save(**kv)
         if pk not in kv:
             self.__dict__.update({pk: _id})
         return _id
 
-    def update(self):
+    def update(self, ignored_none=True):
         """
         user = User(id=1, name='李四', age=66)
         rowcount = user.update()
         :return: Effect rowcount
         """
         orm_inst_log('update', self.__class__.__name__)
         pk, table = self._get_pk_and_table()
-        kv = {k: v for k, v in self.__dict__.items() if v is not None}
-        if pk not in kv:
-            raise KeyError("Not primary key.")
+        if ignored_none:
+            kv = {k: v for k, v in self.__dict__.items() if v is not None}
+        else:
+            kv = {k: v for k, v in self.__dict__.items()}
 
+        _id = kv[pk]
+        assert _id is not None, 'Primary key must not be None.'
         update_kv = {k: v for k, v in kv.items() if k != pk}
         if update_kv:
-            return self.update_by_id(kv[pk], **update_kv)
+            return self.update_by_id(_id, **update_kv)
         else:
             logger.warning("Exec func 'mysqlx.orm.Model.%s' not set fields, Class: '%s:'\n\t   %s" % ('update', self.__class__.__name__, self))
             return 0
 
     def load(self, *fields):
         """
         Return new object from database and update itself.
@@ -124,68 +127,62 @@
         user = User(id=1)
         user2 = user.load()
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
         pk = self._get_pk()
         kv = self.__dict__
         _id = kv.get(pk)
-        if _id is not None:
-            if not fields:
-                fields, _ = zip(*kv.items())
-            m = self.query_by_id(_id, *fields)
-            if m:
-                self.__dict__.update(m)
-                return self
-            else:
-                msg = "Exec func 'mysqlx.orm.Model.%s' load none, Class: '%s', %s=%d." % ('load', self.__class__.__name__, pk, _id)
-                logger.error(msg)
-                raise DBError(msg)
+        assert _id is not None, 'Primary key must not be None.'
+        if not fields:
+            fields, _ = zip(*kv.items())
+        result = self.query_by_id(_id, *fields)
+        if result:
+            self.__dict__.update(result)
+            return self
         else:
-            raise KeyError("Not primary key.")
+            raise NotFoundError("Load not found from db, Class: '%s', %s=%d." % (self.__class__.__name__, pk, _id))
 
     def logical_delete(self):
         """
         Logic delete only update the del flag
         user = User(id=1)
         rowcount = user.logical_delete()
         """
         orm_inst_log('logical_delete', self.__class__.__name__)
         pk = self._get_pk()
-        _id = self.__dict__.get(pk)
-        update_by = self.__dict__.get(self._get_update_by_field())
-        if _id is None:
-            raise KeyError("Not primary key.")
-
+        kv = self.__dict__
+        _id = kv.get(pk)
+        assert _id is not None, 'Primary key must not be None.'
+        update_by = kv.get(self._get_update_by_field())
         return self.logical_delete_by_id(_id, update_by)
 
     def un_logical_delete(self):
         """
         Logic un delete only update the del flag
         user = User(id=1)
         rowcount = user.un_logical_delete()
         """
         orm_inst_log('un_logical_delete', self.__class__.__name__)
         pk = self._get_pk()
-        _id = self.__dict__.get(pk)
-        update_by = self.__dict__.get(self._get_update_by_field())
-        if _id is None:
-            raise KeyError("Not primary key.")
+        kv = self.__dict__
+        _id = kv.get(pk)
+        assert _id is not None, 'Primary key must not be None.'
+        update_by = kv.get(self._get_update_by_field())
         return self.un_logical_delete_by_id(_id, update_by)
 
     def delete(self):
         """
         Physical delete
         user = User(id=1)
         rowcount = user.delete()
         """
         orm_inst_log('delete', self.__class__.__name__)
         pk = self._get_pk()
         _id = self.__dict__.get(pk)
-        if _id is None:
-            raise KeyError("Not primary key.")
+        assert _id is not None, 'Primary key must not be None.'
         return self.delete_by_id(_id)
 
     # ----------------------------------------------------------Class method------------------------------------------------------------------
     @classmethod
     def insert(cls, **kwargs):
         """
         rowcount = User.insert(name='张三', age=20)
@@ -825,51 +822,62 @@
 @lru_cache(maxsize=CONFIG_DICT[CACHE_SIZE])
 def _get_table_columns(table: str):
     return do_get_limit(COLUMN_SQL, table, LIMIT_1)
 
 
 def _get_condition_arg(k: str, v: object):
     if k.endswith("__eq"):
-        return "`{}`=?".format(k[:-4]), v
+        return "{}=?".format(k[:-4]), v
+    if k.endswith("__ne"):
+        return "{}!=?".format(k[:-4]), v
     if k.endswith("__gt"):
-        return "`{}`>?".format(k[:-4]), v
+        return "{}>?".format(k[:-4]), v
     if k.endswith("__lt"):
-        return "`{}`<?".format(k[:-4]), v
+        return "{}<?".format(k[:-4]), v
     if k.endswith("__ge"):
-        return "`{}`>=?".format(k[:-4]), v
+        return "{}>=?".format(k[:-4]), v
     if k.endswith("__gte"):
-        return "`{}`>=?".format(k[:-5]), v
+        return "{}>=?".format(k[:-5]), v
     if k.endswith("__le"):
-        return "`{}`<=?".format(k[:-4]), v
+        return "{}<=?".format(k[:-4]), v
     if k.endswith("__lte"):
-        return "`{}`<=?".format(k[:-5]), v
+        return "{}<=?".format(k[:-5]), v
+    if k.endswith("__isnull"):
+        return "{} is {}".format(k[:-8], 'null' if v else 'not null'), None
     if k.endswith("__in") and isinstance(v, Sequence) and not isinstance(v, str):
-        return "`{}` in ({})".format(k[:-4], ','.join(['?' for _ in v])), v
+        return "{} in({})".format(k[:-4], ','.join(['?' for _ in v])), v
     if k.endswith("__in"):
-        return "`{}` in ({})".format(k[:-4], '?'), v
+        return "{} in({})".format(k[:-4], '?'), v
+    if k.endswith("__not_in") and isinstance(v, Sequence) and not isinstance(v, str):
+        return "{} not in({})".format(k[:-8], ','.join(['?' for _ in v])), v
+    if k.endswith("__not_in"):
+        return "{} not in({})".format(k[:-8], '?'), v
     if k.endswith("__startswith"):
-        return "`{}` like ?".format(k[:-12]), '{}%'.format(v)
+        return "{} like ?".format(k[:-12]), '{}%'.format(v)
     if k.endswith("__endswith"):
-        return "`{}` like ?".format(k[:-10]), '%{}'.format(v)
+        return "{} like ?".format(k[:-10]), '%{}'.format(v)
     if k.endswith("__contains"):
-        return "`{}` like ?".format(k[:-10]), '%{}%'.format(v)
+        return "{} like ?".format(k[:-10]), '%{}%'.format(v)
+    if k.endswith("__range") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
+        col = k[:-7]
+        return "{}>=? and {}<=?".format(col, col), v
     if k.endswith("__between") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
-        return "`{}` between ? and ?".format(k[:-9]), v
-    if k.endswith("__between"):
-        return ValueError("Must is instance of Sequence with length 2 when use between statement")
+        return "{} between ? and ?".format(k[:-9]), v
+    if k.endswith("__range") or k.endswith("__between"):
+        return ValueError("Must is instance of Sequence with length 2 when use range or between statement")
 
     if not isinstance(v, str):
-        return "`{}`=?".format(k), v
+        return "{}=?".format(k), v
     lower_v = v.lower()
     if any([symbol in SYMBOLS for symbol in lower_v]):
-        return "`{}`{}".format(k, v), None
-    elif BETWEEN in lower_v or LIKE in lower_v or IN in lower_v:
-        return "`{}` {}".format(k, v), None
+        return "{}{}".format(k, v), None
+    elif BETWEEN in lower_v or LIKE in lower_v or IN in lower_v or IS in lower_v:
+        return "{} {}".format(k, v), None
     else:
-        return "`{}`=?".format(k), v
+        return "{}=?".format(k), v
 
 
 def _get_where_arg_limit(**kwargs):
     where, args, limit = '', [], 0
     if 'limit' in kwargs:
         limit = kwargs.pop('limit')
```

### Comparing `mysqlx-1.5.4/mysqlx/snowflake.py` & `mysqlx-1.5.5/mysqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.4/mysqlx/sql_mapper.py` & `mysqlx-1.5.5/mysqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.4/mysqlx/support.py` & `mysqlx-1.5.5/mysqlx/support.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,18 @@
     pass
 
 
 class MapperError(DBError):
     pass
 
 
+class NotFoundError(DBError):
+    pass
+
+
 class MultiColumnsError(DBError):
     pass
 
 
 class Dict(dict):
     def __init__(self, names=(), values=(), **kw):
         super(Dict, self).__init__(**kw)
```

### Comparing `mysqlx-1.5.4/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.5.5/mysqlx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.4
+Version: 1.5.5
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 Mapper file
 '''''''''''
 
 Create a mapper file in 'mapper' folder, you can named
 'user_mapper.xml', like follow:
```

### Comparing `mysqlx-1.5.4/PKG-INFO` & `mysqlx-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.4
+Version: 1.5.5
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 Mapper file
 '''''''''''
 
 Create a mapper file in 'mapper' folder, you can named
 'user_mapper.xml', like follow:
```

### Comparing `mysqlx-1.5.4/README.rst` & `mysqlx-1.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.4/setup.py` & `mysqlx-1.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.5.4',
+    version='1.5.5',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

