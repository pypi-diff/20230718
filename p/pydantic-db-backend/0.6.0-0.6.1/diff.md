# Comparing `tmp/pydantic_db_backend-0.6.0.tar.gz` & `tmp/pydantic_db_backend-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.6.0.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.6.1.tar", max compression
```

## Comparing `pydantic_db_backend-0.6.0.tar` & `pydantic_db_backend-0.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.6.0/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     7789 2023-07-14 09:24:44.711216 pydantic_db_backend-0.6.0/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.6.0/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0     8650 2023-07-14 10:07:43.763037 pydantic_db_backend-0.6.0/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.6.0/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0      990 2023-07-14 09:23:03.448444 pydantic_db_backend-0.6.0/pydantic_db_backend/exceptions/__init__.py
--rw-r--r--   0        0        0      768 2023-07-12 13:44:19.743864 pydantic_db_backend-0.6.0/pydantic_db_backend/indexes.py
--rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.6.0/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0      996 2023-07-14 10:12:23.112441 pydantic_db_backend-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.6.1/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     7842 2023-07-18 09:42:27.492675 pydantic_db_backend-0.6.1/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.6.1/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0     8681 2023-07-18 09:52:14.583217 pydantic_db_backend-0.6.1/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.6.1/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0      990 2023-07-14 09:23:03.448444 pydantic_db_backend-0.6.1/pydantic_db_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0      768 2023-07-12 13:44:19.743864 pydantic_db_backend-0.6.1/pydantic_db_backend/indexes.py
+-rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.6.1/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0      996 2023-07-18 09:52:39.482977 pydantic_db_backend-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.6.1/PKG-INFO
```

### Comparing `pydantic_db_backend-0.6.0/pydantic_db_backend/backend.py` & `pydantic_db_backend-0.6.1/pydantic_db_backend/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,23 +214,24 @@
             model=model,
             skip=skip,
             limit=limit,
             query_filter=query_filter,
             sort=sort,
             max_results=max_results
         )
+        max_results_value = None
         if max_results:
-            ids, max_results = cls.get_uids(**params)
+            ids, max_results_value = cls.get_uids(**params)
         else:
             ids = cls.get_uids(**params)
 
         instances = [cls.get_instance(model, uid=x) for x in ids]
 
-        if max_results:
-            return instances, max_results
+        if max_results is True:
+            return instances, max_results_value
         else:
             return instances
 
     @classmethod
     def delete_uid(cls, model: Type[BackendModel], uid: str) -> None:
         raise NotImplementedError
```

### Comparing `pydantic_db_backend-0.6.0/pydantic_db_backend/backends/couchdb.py` & `pydantic_db_backend-0.6.1/pydantic_db_backend/backends/couchdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     _indexes: Dict[str, List[dict]] = {}
     _connections: Dict[str, CouchDbConnectionModel] = {}
 
     @classmethod
     def startup(cls, alias: str | None = "default", uri: str | None = None):
         super().startup()
         if uri is None:
-            uri = os.environ.get('COUCHDB_URI', None)
-            if uri is None:
+            uri = os.environ.get('COUCHDB_URI', "")
+            if uri == "":
                 raise EnvironmentError("COUCHDB_URI not set.")
 
         cls._connections[alias] = CouchDbConnectionModel(
             alias=alias,
             uri=uri,
             server=couchdb.Server(uri)
         )
@@ -77,15 +77,16 @@
         else:
             pass
 
     @classmethod
     def view_from_aggregation_index(cls, db: couchdb.Database, collection_name: str, index: AggregationIndex):
         design_document = index.design_document
 
-        if design_document not in db:
+        in_db = f"_design/{design_document}" in db
+        if not in_db:
             field, func = next(iter(index.spec.items()))
             map_function = f"function (doc) {{ emit(doc.{field}, 1); }}"
             view_name = f"{index.view_name}"
             # reduce_function = f"function(keys, values, rereduce) {{ return sum(values); }}"
             data = {
                 "_id": f"_design/{design_document}",
                 "views": {
```

### Comparing `pydantic_db_backend-0.6.0/pydantic_db_backend/exceptions/__init__.py` & `pydantic_db_backend-0.6.1/pydantic_db_backend/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.6.0/pydantic_db_backend/indexes.py` & `pydantic_db_backend-0.6.1/pydantic_db_backend/indexes.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.6.0/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.6.1/pydantic_db_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.6.0/pyproject.toml` & `pydantic_db_backend-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^0.15.0"
```

### Comparing `pydantic_db_backend-0.6.0/PKG-INFO` & `pydantic_db_backend-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: couchdb
```

