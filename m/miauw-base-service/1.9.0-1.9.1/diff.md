# Comparing `tmp/miauw-base-service-1.9.0.tar.gz` & `tmp/miauw-base-service-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.9.0.tar", last modified: Tue Jul 18 06:47:12 2023, max compression
+gzip compressed data, was "miauw-base-service-1.9.1.tar", last modified: Tue Jul 18 07:31:34 2023, max compression
```

## Comparing `miauw-base-service-1.9.0.tar` & `miauw-base-service-1.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-18 06:47:12.845892 miauw-base-service-1.9.0/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-18 06:47:12.845892 miauw-base-service-1.9.0/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-18 06:47:12.845892 miauw-base-service-1.9.0/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)      110 2023-07-16 11:46:05.000000 miauw-base-service-1.9.0/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1154 2023-07-16 11:46:05.000000 miauw-base-service-1.9.0/base_service/email_worker.py
--rw-r--r--   0 leo       (1000) leo       (1000)      528 2023-07-16 11:46:05.000000 miauw-base-service-1.9.0/base_service/exceptions.py
--rw-r--r--   0 leo       (1000) leo       (1000)     4137 2023-07-18 06:41:20.000000 miauw-base-service-1.9.0/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)      875 2023-07-18 06:17:46.000000 miauw-base-service-1.9.0/base_service/utils.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2669 2023-07-18 06:00:14.000000 miauw-base-service-1.9.0/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-18 06:47:12.845892 miauw-base-service-1.9.0/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-18 06:47:12.000000 miauw-base-service-1.9.0/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      382 2023-07-18 06:47:12.000000 miauw-base-service-1.9.0/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-18 06:47:12.000000 miauw-base-service-1.9.0/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       44 2023-07-18 06:47:12.000000 miauw-base-service-1.9.0/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-18 06:47:12.000000 miauw-base-service-1.9.0/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      332 2023-07-18 06:38:20.000000 miauw-base-service-1.9.0/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-18 06:47:12.845892 miauw-base-service-1.9.0/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-18 06:39:06.000000 miauw-base-service-1.9.0/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-18 07:31:34.338226 miauw-base-service-1.9.1/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-18 07:31:34.338226 miauw-base-service-1.9.1/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-18 07:31:34.338226 miauw-base-service-1.9.1/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)      110 2023-07-16 11:46:05.000000 miauw-base-service-1.9.1/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1154 2023-07-16 11:46:05.000000 miauw-base-service-1.9.1/base_service/email_worker.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      528 2023-07-16 11:46:05.000000 miauw-base-service-1.9.1/base_service/exceptions.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     3277 2023-07-18 07:29:01.000000 miauw-base-service-1.9.1/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      875 2023-07-18 07:21:57.000000 miauw-base-service-1.9.1/base_service/utils.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2669 2023-07-18 07:21:57.000000 miauw-base-service-1.9.1/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-18 07:31:34.338226 miauw-base-service-1.9.1/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-18 07:31:34.000000 miauw-base-service-1.9.1/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      382 2023-07-18 07:31:34.000000 miauw-base-service-1.9.1/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-18 07:31:34.000000 miauw-base-service-1.9.1/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       44 2023-07-18 07:31:34.000000 miauw-base-service-1.9.1/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-18 07:31:34.000000 miauw-base-service-1.9.1/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      332 2023-07-18 07:30:42.000000 miauw-base-service-1.9.1/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-18 07:31:34.338226 miauw-base-service-1.9.1/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-18 07:30:42.000000 miauw-base-service-1.9.1/setup.py
```

### Comparing `miauw-base-service-1.9.0/base_service/email_worker.py` & `miauw-base-service-1.9.1/base_service/email_worker.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.9.0/base_service/exceptions.py` & `miauw-base-service-1.9.1/base_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.9.0/base_service/service.py` & `miauw-base-service-1.9.1/base_service/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from base_service.email_worker import EmailTemplates, EMailWorker
+from base_service.email_worker import EMailWorker
 from base_service.worker import RabbitMQWorker
-from base_service.utils import get_file_paths, build_prepared_statement
+from base_service.utils import run_async
 from psycopg_pool import AsyncConnectionPool
-from psycopg import AsyncConnection
 import asyncio
 import typing
 import logging
 import os
 
 
 class BaseService:
@@ -38,20 +37,22 @@
         self.logger.setLevel(logging.DEBUG)
         self.log_filehandler.setLevel(logging.DEBUG)
         self.log_streamhandler.setLevel(logging.INFO)
         self.log_filehandler.setFormatter(self.log_formatter)
         self.log_streamhandler.setFormatter(self.log_formatter)
         self.logger.addHandler(self.log_filehandler)
         self.logger.addHandler(self.log_streamhandler)
+        # run init db
+        if postgres_url:
+            run_async(self.init_db())
 
     def start(self):
         """starts the service"""
         self.logger.info("starting")
         loop = asyncio.get_event_loop()
-
         for ev in self.events:
             self.logger.info(f"listening for event '{ev}'")
         loop.run_until_complete(
             asyncio.gather(
                 *[self.worker.listen(event, handler) for a in self.m.values() for event, handler in a.items()])
         )
 
@@ -59,38 +60,19 @@
                       prepare_statements: bool = True,
                       path: str = "./sql/",
                       include_sub_dirs: bool = True,
                       exclude_files: list[str] = [],
                       min_size: int = 5,
                       max_size: int = 15):
         """initialises the connection with the database and prepares the statements."""
-        self._pool = AsyncConnectionPool(self.postgres_url, min_size=5, max_size=15)
-        # statements: list[str] = []
-        # if prepare_statements:
-        #     files = get_file_paths(path, walk_sub_dirs=include_sub_dirs)
-        #     for file in files:
-        #         if file in exclude_files:
-        #             continue
-        #         else:
-        #             with open(file) as f:
-        #                 statements.append(build_prepared_statement(file.lstrip(f"{path}"), f.read()))
-        # conn: AsyncConnection
-        # for statement in statements:
-        #     print(statement)
-        # async with self.pool.connection() as conn:
-        #     for statement in statements:
-        #         await conn.execute(statement)
-        #         await conn.commit()
-        #         print("prepared statement", statement)
+        self.__setattr__("_pool", AsyncConnectionPool(self.postgres_url, min_size=5, max_size=15))
 
     @property
     def pool(self):
         """returns the database connection pool of the service"""
-        if not self._pool:
-            raise AttributeError("You need to call BaseService.init_db() first.")
         return self._pool
 
     def event(self, event: str, event_type: str = "rpc"):
         """adds a new event handler for event"""
 
         def wrapper(handler: typing.Callable[[dict], typing.Awaitable[dict]]):
             self.logger.debug(f"add handler {handler} for event '{event}'")
```

### Comparing `miauw-base-service-1.9.0/base_service/utils.py` & `miauw-base-service-1.9.1/base_service/utils.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.9.0/base_service/worker.py` & `miauw-base-service-1.9.1/base_service/worker.py`

 * *Files identical despite different names*

