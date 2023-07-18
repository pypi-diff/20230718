# Comparing `tmp/pyairtable-1.4.0.tar.gz` & `tmp/pyairtable-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyairtable-1.4.0.tar", last modified: Wed Dec 14 15:35:39 2022, max compression
+gzip compressed data, was "pyairtable-1.5.0.tar", last modified: Sun May 14 23:52:46 2023, max compression
```

## Comparing `pyairtable-1.4.0.tar` & `pyairtable-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,46 @@
-drwxr-xr-x   0 gtalarico   (501) staff       (20)        0 2022-12-14 15:35:39.692193 pyairtable-1.4.0/
--rw-r--r--   0 gtalarico   (501) staff       (20)     1056 2022-12-14 15:35:26.000000 pyairtable-1.4.0/LICENSE
--rw-r--r--   0 gtalarico   (501) staff       (20)       77 2022-12-14 15:35:26.000000 pyairtable-1.4.0/MANIFEST.in
--rw-r--r--   0 gtalarico   (501) staff       (20)     2024 2022-12-14 15:35:39.692290 pyairtable-1.4.0/PKG-INFO
--rw-r--r--   0 gtalarico   (501) staff       (20)     1223 2022-12-14 15:35:26.000000 pyairtable-1.4.0/README.md
-drwxr-xr-x   0 gtalarico   (501) staff       (20)        0 2022-12-14 15:35:39.687662 pyairtable-1.4.0/pyairtable/
--rw-r--r--   0 gtalarico   (501) staff       (20)      114 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/__init__.py
-drwxr-xr-x   0 gtalarico   (501) staff       (20)        0 2022-12-14 15:35:39.691143 pyairtable-1.4.0/pyairtable/api/
--rw-r--r--   0 gtalarico   (501) staff       (20)       93 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/api/__init__.py
--rw-r--r--   0 gtalarico   (501) staff       (20)     8073 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/api/abstract.py
--rw-r--r--   0 gtalarico   (501) staff       (20)    10543 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/api/api.py
--rw-r--r--   0 gtalarico   (501) staff       (20)     4620 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/api/base.py
--rw-r--r--   0 gtalarico   (501) staff       (20)     3013 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/api/params.py
--rw-r--r--   0 gtalarico   (501) staff       (20)     1618 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/api/retrying.py
--rw-r--r--   0 gtalarico   (501) staff       (20)     5118 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/api/table.py
--rw-r--r--   0 gtalarico   (501) staff       (20)      202 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/compat.py
--rw-r--r--   0 gtalarico   (501) staff       (20)     5448 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/formulas.py
--rw-r--r--   0 gtalarico   (501) staff       (20)     3736 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/metadata.py
-drwxr-xr-x   0 gtalarico   (501) staff       (20)        0 2022-12-14 15:35:39.691985 pyairtable-1.4.0/pyairtable/orm/
--rw-r--r--   0 gtalarico   (501) staff       (20)       33 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/orm/__init__.py
--rw-r--r--   0 gtalarico   (501) staff       (20)     9073 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/orm/fields.py
--rw-r--r--   0 gtalarico   (501) staff       (20)    11491 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/orm/model.py
--rw-r--r--   0 gtalarico   (501) staff       (20)        0 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/py.typed
--rw-r--r--   0 gtalarico   (501) staff       (20)     2453 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyairtable/utils.py
-drwxr-xr-x   0 gtalarico   (501) staff       (20)        0 2022-12-14 15:35:39.689182 pyairtable-1.4.0/pyairtable.egg-info/
--rw-r--r--   0 gtalarico   (501) staff       (20)     2024 2022-12-14 15:35:39.000000 pyairtable-1.4.0/pyairtable.egg-info/PKG-INFO
--rw-r--r--   0 gtalarico   (501) staff       (20)      621 2022-12-14 15:35:39.000000 pyairtable-1.4.0/pyairtable.egg-info/SOURCES.txt
--rw-r--r--   0 gtalarico   (501) staff       (20)        1 2022-12-14 15:35:39.000000 pyairtable-1.4.0/pyairtable.egg-info/dependency_links.txt
--rw-r--r--   0 gtalarico   (501) staff       (20)       12 2022-12-14 15:35:39.000000 pyairtable-1.4.0/pyairtable.egg-info/requires.txt
--rw-r--r--   0 gtalarico   (501) staff       (20)       11 2022-12-14 15:35:39.000000 pyairtable-1.4.0/pyairtable.egg-info/top_level.txt
--rw-r--r--   0 gtalarico   (501) staff       (20)      168 2022-12-14 15:35:26.000000 pyairtable-1.4.0/pyproject.toml
--rw-r--r--   0 gtalarico   (501) staff       (20)     1082 2022-12-14 15:35:39.692832 pyairtable-1.4.0/setup.cfg
--rw-r--r--   0 gtalarico   (501) staff       (20)      101 2022-12-14 15:35:26.000000 pyairtable-1.4.0/setup.py
--rw-r--r--   0 gtalarico   (501) staff       (20)      890 2022-12-14 15:35:29.000000 pyairtable-1.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:52:46.146901 pyairtable-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-14 23:52:34.000000 pyairtable-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-14 23:52:34.000000 pyairtable-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-14 23:52:46.146901 pyairtable-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-14 23:52:34.000000 pyairtable-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:52:46.138901 pyairtable-1.5.0/pyairtable/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:52:46.142901 pyairtable-1.5.0/pyairtable/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/api/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/api/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/api/retrying.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/api/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/formulas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:52:46.142901 pyairtable-1.5.0/pyairtable/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/orm/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/orm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyairtable/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:52:46.138901 pyairtable-1.5.0/pyairtable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-14 23:52:46.000000 pyairtable-1.5.0/pyairtable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-14 23:52:46.000000 pyairtable-1.5.0/pyairtable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 23:52:46.000000 pyairtable-1.5.0/pyairtable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-14 23:52:46.000000 pyairtable-1.5.0/pyairtable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 23:52:46.000000 pyairtable-1.5.0/pyairtable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-14 23:52:34.000000 pyairtable-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-14 23:52:46.146901 pyairtable-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-14 23:52:34.000000 pyairtable-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 23:52:46.142901 pyairtable-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_api_retrying.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_api_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_formulas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_orm_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_request_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_url_escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-14 23:52:34.000000 pyairtable-1.5.0/tox.ini
```

### Comparing `pyairtable-1.4.0/LICENSE` & `pyairtable-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyairtable-1.4.0/pyairtable/api/api.py` & `pyairtable-1.5.0/pyairtable/api/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,74 @@
 from typing import List, Optional
-from .abstract import ApiAbstract, TimeoutTuple
 
-from .. import compat
+from .abstract import ApiAbstract, TimeoutTuple
+from .retrying import Retry
 
 
 class Api(ApiAbstract):
     """
     Represents an Airtable Api.
 
-    The Api Key is provided on init and ``base_id`` and ``table_id``
+    The Api Key or Authorization Token is provided on init and ``base_id`` and ``table_id``
     can be provided on each method call.
 
     If you are only operating on one Table, or one Base, consider using
     :class:`Base` or :class:`Table`.
 
     Usage:
-        >>> api = Api('apikey')
+        >>> api = Api('auth_token')
         >>> api.all('base_id', 'table_name')
     """
 
     def __init__(
         self,
         api_key: str,
         *,
         timeout: Optional[TimeoutTuple] = None,
-        retry_strategy: Optional["compat.Retry"] = None,
+        retry_strategy: Optional[Retry] = None,
+        endpoint_url: str = "https://api.airtable.com",
     ):
         """
 
         Args:
             api_key: |arg_api_key|
 
         Keyword Args:
             timeout (``Tuple``): |arg_timeout|
             retry_strategy (``Retry``): |arg_retry_strategy|
-
+            endpoint_url (``str``): |arg_endpoint_url|
         """
-        super().__init__(api_key, timeout=timeout, retry_strategy=retry_strategy)
+        super().__init__(
+            api_key,
+            timeout=timeout,
+            retry_strategy=retry_strategy,
+            endpoint_url=endpoint_url,
+        )
 
     def get_table(self, base_id: str, table_name: str) -> "Table":
         """
         Returns a new :class:`Table` instance using all shared
         attributes from :class:`Api`
         """
-        return Table(self.api_key, base_id, table_name, timeout=self.timeout)
+        return Table(
+            self.api_key,
+            base_id,
+            table_name,
+            timeout=self.timeout,
+            endpoint_url=self.endpoint_url,
+        )
 
     def get_base(self, base_id: str) -> "Base":
         """
         Returns a new :class:`Base` instance using all shared
         attributes from :class:`Api`
         """
-        return Base(self.api_key, base_id, timeout=self.timeout)
+        return Base(
+            self.api_key, base_id, timeout=self.timeout, endpoint_url=self.endpoint_url
+        )
 
     def get_record_url(self, base_id: str, table_name: str, record_id: str):
         """
         Returns a url for the provided record
 
         Args:
             base_id: |arg_base_id|
@@ -131,14 +145,18 @@
             table_name: |arg_table_name|
 
         Keyword Args:
             view: |kwarg_view|
             fields: |kwarg_fields|
             sort: |kwarg_sort|
             formula: |kwarg_formula|
+            cell_format: |kwarg_cell_format|
+            user_locale: |kwarg_user_locale|
+            time_zone: |kwarg_time_zone|
+            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
         """
         return super()._first(base_id, table_name, **options)
 
     def all(self, base_id: str, table_name: str, **options):
         """
         Retrieves all records repetitively and returns a single list.
 
@@ -167,59 +185,87 @@
             records (``list``): List of Records
 
         >>> records = all(max_records=3, view='All')
 
         """
         return super()._all(base_id, table_name, **options)
 
-    def create(self, base_id: str, table_name: str, fields: dict, typecast=False):
+    def create(
+        self,
+        base_id: str,
+        table_name: str,
+        fields: dict,
+        typecast=False,
+        return_fields_by_field_id=False,
+    ):
         """
         Creates a new record
 
         >>> record = {'Name': 'John'}
         >>> api.create('base_id', 'table_name', record)
 
         Args:
             base_id: |arg_base_id|
             table_name: |arg_table_name|
             fields(``dict``): Fields to insert.
                 Must be dictionary with Column names as Key.
 
         Keyword Args:
             typecast: |kwarg_typecast|
+            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
 
         Returns:
             record (``dict``): Inserted record
 
         """
-        return super()._create(base_id, table_name, fields, typecast=typecast)
+        return super()._create(
+            base_id,
+            table_name,
+            fields,
+            typecast=typecast,
+            return_fields_by_field_id=return_fields_by_field_id,
+        )
 
-    def batch_create(self, base_id: str, table_name: str, records, typecast=False):
+    def batch_create(
+        self,
+        base_id: str,
+        table_name: str,
+        records,
+        typecast=False,
+        return_fields_by_field_id=False,
+    ):
         """
         Breaks records into chunks of 10 and inserts them in batches.
         Follows the set API rate.
         To change the rate limit you can change ``API_LIMIT = 0.2``
         (5 per second)
 
         >>> records = [{'Name': 'John'}, {'Name': 'Marc'}]
-        >>> api.batch_insert('base_id', 'table_name', records)
+        >>> api.batch_create('base_id', 'table_name', records)
 
         Args:
             base_id: |arg_base_id|
             table_name: |arg_table_name|
             records(``List[dict]``): List of dictionaries representing
                 records to be created.
 
         Keyword Args:
             typecast: |kwarg_typecast|
+            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
 
         Returns:
             records (``list``): list of added records
         """
-        return super()._batch_create(base_id, table_name, records, typecast=typecast)
+        return super()._batch_create(
+            base_id,
+            table_name,
+            records,
+            typecast=typecast,
+            return_fields_by_field_id=return_fields_by_field_id,
+        )
 
     def update(
         self,
         base_id: str,
         table_name: str,
         record_id: str,
         fields: dict,
@@ -236,15 +282,15 @@
         {id:'recwPQIfs4wKPyc9D', fields': {"Age": 21}}
 
         Args:
             base_id: |arg_base_id|
             table_name: |arg_table_name|
             record_id: |arg_record_id|
             fields(``dict``): Fields to update.
-                Must be dictionary with Column names as Key
+                Must be a dict with column names or IDs as keys
 
         Keyword Args:
             replace (``bool``, optional): If ``True``, record is replaced in its entirety
                 by provided fields - eg. if a field is not included its value will
                 bet set to null. If False, only provided fields are updated.
                 Default is ``False``.
             typecast: |kwarg_typecast|
@@ -265,14 +311,15 @@
     def batch_update(
         self,
         base_id: str,
         table_name: str,
         records: List[dict],
         replace=False,
         typecast=False,
+        return_fields_by_field_id=False,
     ):
         """
         Updates a records by their record id's in batch.
 
         Args:
             base_id: |arg_base_id|
             table_name: |arg_table_name|
@@ -280,20 +327,71 @@
 
         Keyword Args:
             replace (``bool``, optional): If ``True``, record is replaced in its entirety
                 by provided fields - eg. if a field is not included its value will
                 bet set to null. If False, only provided fields are updated.
                 Default is ``False``.
             typecast: |kwarg_typecast|
+            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
 
         Returns:
             records(``list``): list of updated records
         """
         return super()._batch_update(
-            base_id, table_name, records, replace=replace, typecast=typecast
+            base_id,
+            table_name,
+            records,
+            replace=replace,
+            typecast=typecast,
+            return_fields_by_field_id=return_fields_by_field_id,
+        )
+
+    def batch_upsert(
+        self,
+        base_id: str,
+        table_name: str,
+        records: List[dict],
+        key_fields: List[str],
+        replace=False,
+        typecast=False,
+        return_fields_by_field_id=False,
+    ):
+        """
+        Updates or creates records in batches, either using ``id`` (if given) or using a set of
+        fields (``key_fields``) to look for matches. For more information on how this operation
+        behaves, see Airtable's API documentation for `Update multiple records <https://airtable.com/developers/web/api/update-multiple-records#request-performupsert-fieldstomergeon>`_.
+
+        .. versionadded:: 1.5.0
+
+        Args:
+            base_id: |arg_base_id|
+            table_name: |arg_table_name|
+            records (``list``): List of dict: [{"id": record_id, "fields": fields_to_update_dict}]
+            key_fields (``list``): List of field names that Airtable should use to match
+                records in the input with existing records on the server.
+
+        Keyword Args:
+            replace (``bool``, optional): If ``True``, record is replaced in its entirety
+                by provided fields - e.g. if a field is not included its value will
+                bet set to null. If False, only provided fields are updated.
+                Default is ``False``.
+            typecast: |kwarg_typecast|
+            return_fields_by_field_id: |kwarg_return_fields_by_field_id|
+
+        Returns:
+            records (``list``): list of updated records
+        """
+        return super()._batch_upsert(
+            base_id=base_id,
+            table_name=table_name,
+            records=records,
+            key_fields=key_fields,
+            replace=replace,
+            typecast=typecast,
+            return_fields_by_field_id=return_fields_by_field_id,
         )
 
     def delete(self, base_id: str, table_name: str, record_id: str):
         """
         Deletes a record by its id
 
         >>> record = api.match('base_id', 'table_name', 'Employee Id', 'DD13332454')
@@ -330,9 +428,9 @@
         """
         return super()._batch_delete(base_id, table_name, record_ids)
 
     def __repr__(self) -> str:
         return "<pyairtable.Api>"
 
 
-from pyairtable.api.table import Table  # noqa
 from pyairtable.api.base import Base  # noqa
+from pyairtable.api.table import Table  # noqa
```

### Comparing `pyairtable-1.4.0/pyairtable/api/retrying.py` & `pyairtable-1.5.0/pyairtable/api/retrying.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 from requests import Session
 from requests.adapters import HTTPAdapter
-
-from .. import compat
-
+from urllib3.util.retry import Retry
 
 DEFAULT_RETRIABLE_STATUS_CODES = (429, 500, 502, 503, 504)
 DEFAULT_BACKOFF_FACTOR = 0.3
 DEFAULT_MAX_RETRIES = 5
 
 
 def retry_strategy(
     *,
     status_forcelist=DEFAULT_RETRIABLE_STATUS_CODES,
     backoff_factor=DEFAULT_BACKOFF_FACTOR,
     total=DEFAULT_MAX_RETRIES,
     **kwargs,
-) -> "compat.Retry":
+) -> Retry:
     """
     Creates a ``Retry`` instance with optional default values.
     See `urllib3 Retry docs <https://urllib3.readthedocs.io/en/stable/reference/urllib3.util.html>`_
     for more details.
 
     .. versionadded:: 1.4.0
 
     Keyword Args:
         status_forcelist (``Tuple[int]``): list status code which should be retried.
         backoff_factor (``float``): backoff factor.
         total (``int``): max. number of retries. Note ``0`` means no retries,
             while``1`` will exececute a total of two requests (1 + 1 retry).
         **kwargs: All parameters supported by ``urllib3.util.Retry`` can be used.
     """
-
-    try:
-        from urllib3.util import Retry
-    except ImportError:
-        raise ImportError(
-            "urllib3.util.Retry not found. Install newer urllib3 to use `Retry`."
-        )
-
     return Retry(
         total=total,
         backoff_factor=backoff_factor,
         status_forcelist=status_forcelist,
         **kwargs,
     )
 
 
 class _RetryingSession(Session):
-    def __init__(self, retry_strategy: "compat.Retry"):
+    def __init__(self, retry_strategy: Retry):
         super().__init__()
 
         adapter = HTTPAdapter(max_retries=retry_strategy)
 
         self.mount("https://", adapter)
         self.mount("http://", adapter)
```

### Comparing `pyairtable-1.4.0/pyairtable/api/table.py` & `pyairtable-1.5.0/pyairtable/api/table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 from typing import List, Optional
 
 from .abstract import ApiAbstract, TimeoutTuple
-from .. import compat
+from .retrying import Retry
 
 
 class Table(ApiAbstract):
     """
-    Represents an Airtable Table. This calss is similar to :class:`~pyairtable.api.Api`,
+    Represents an Airtable Table. This class is similar to :class:`~pyairtable.api.Api`,
     except ``base_id`` and ``table_id`` are provided on init instead of provided
     on each method call.
 
     Usage:
-        >>> table = Table('apikey', 'base_id', 'table_name')
+        >>> table = Table('apikey/accesstoken', 'base_id', 'table_name')
         >>> table.all()
     """
 
     base_id: str
     table_name: str
 
     def __init__(
         self,
         api_key: str,
         base_id: str,
         table_name: str,
         *,
         timeout: Optional[TimeoutTuple] = None,
-        retry_strategy: Optional["compat.Retry"] = None,
+        retry_strategy: Optional[Retry] = None,
+        endpoint_url: str = "https://api.airtable.com",
     ):
         """
         Args:
             api_key: |arg_api_key|
             base_id: |arg_base_id|
             table_name: |arg_table_name|
 
         Keyword Args:
             timeout (``Tuple``): |arg_timeout|
             retry_strategy (``Retry``): |arg_retry_strategy|
         """
         self.base_id = base_id
         self.table_name = table_name
-        super().__init__(api_key, timeout=timeout, retry_strategy=retry_strategy)
+        super().__init__(
+            api_key,
+            timeout=timeout,
+            retry_strategy=retry_strategy,
+            endpoint_url=endpoint_url,
+        )
 
     @property
     def table_url(self):
         """Returns the table URL"""
         return super().get_table_url(self.base_id, self.table_name)
 
     def get_base(self) -> "Base":
@@ -86,59 +92,104 @@
     def all(self, **options):
         """
         Same as :meth:`Api.all <pyairtable.api.Api.all>`
         but without ``base_id`` and ``table_name`` arg.
         """
         return super()._all(self.base_id, self.table_name, **options)
 
-    def create(self, fields: dict, typecast=False, **options):
+    def create(
+        self,
+        fields: dict,
+        typecast=False,
+        return_fields_by_field_id=False,
+    ):
         """
         Same as :meth:`Api.create <pyairtable.api.Api.create>`
         but without ``base_id`` and ``table_name`` arg.
         """
-        return super()._create(self.base_id, self.table_name, fields, typecast=typecast, **options)
+        return super()._create(
+            self.base_id,
+            self.table_name,
+            fields,
+            typecast=typecast,
+            return_fields_by_field_id=return_fields_by_field_id,
+        )
 
-    def batch_create(self, records, typecast=False, **options):
+    def batch_create(
+        self,
+        records,
+        typecast=False,
+        return_fields_by_field_id=False,
+    ):
         """
         Same as :meth:`Api.batch_create <pyairtable.api.Api.batch_create>`
         but without ``base_id`` and ``table_name`` arg.
         """
         return super()._batch_create(
-            self.base_id, self.table_name, records, typecast=typecast, **options
+            self.base_id,
+            self.table_name,
+            records,
+            typecast=typecast,
+            return_fields_by_field_id=return_fields_by_field_id,
         )
 
-    def update(
-        self,
-        record_id: str,
-        fields: dict,
-        replace=False,
-        typecast=False,
-        **options
-    ):
+    def update(self, record_id: str, fields: dict, replace=False, typecast=False):
         """
         Same as :meth:`Api.update <pyairtable.api.Api.update>`
         but without ``base_id`` and ``table_name`` arg.
         """
         return super()._update(
             self.base_id,
             self.table_name,
             record_id,
             fields,
             replace=replace,
             typecast=typecast,
-            **options
         )
 
-    def batch_update(self, records: List[dict], replace=False, typecast=False, **options):
+    def batch_update(
+        self,
+        records: List[dict],
+        replace=False,
+        typecast=False,
+        return_fields_by_field_id=False,
+    ):
         """
         Same as :meth:`Api.batch_update <pyairtable.api.Api.batch_update>`
         but without ``base_id`` and ``table_name`` arg.
         """
         return super()._batch_update(
-            self.base_id, self.table_name, records, replace=replace, typecast=typecast, **options
+            self.base_id,
+            self.table_name,
+            records,
+            replace=replace,
+            typecast=typecast,
+            return_fields_by_field_id=return_fields_by_field_id,
+        )
+
+    def batch_upsert(
+        self,
+        records: List[dict],
+        key_fields: List[str],
+        replace=False,
+        typecast=False,
+        return_fields_by_field_id=False,
+    ):
+        """
+        Same as :meth:`Api.batch_upsert <pyairtable.api.Api.batch_upsert>`
+        but without ``base_id`` and ``table_name`` arg.
+        """
+        return super()._batch_upsert(
+            self.base_id,
+            self.table_name,
+            records,
+            key_fields=key_fields,
+            replace=replace,
+            typecast=typecast,
+            return_fields_by_field_id=return_fields_by_field_id,
         )
 
     def delete(self, record_id: str):
         """
         Same as :meth:`Api.delete <pyairtable.api.Api.delete>`
         but without ``base_id`` and ``table_name`` arg.
         """
```

### Comparing `pyairtable-1.4.0/pyairtable/formulas.py` & `pyairtable-1.5.0/pyairtable/formulas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from datetime import datetime, date
 import re
+from datetime import date, datetime
 from typing import Any
 
 from .utils import date_to_iso_str, datetime_to_iso_str
 
 
 def match(dict_values, *, match_any=False):
     """
@@ -29,15 +29,15 @@
         match_any: matches if **any** of the provided values match. Default is ``False``
             (all values must match)
 
     Usage:
         >>> match({"First Name": "John", "Age": 21})
         "AND({First Name}='John',{Age}=21)"
         >>> match({"First Name": "John", "Age": 21}, match_any=True)
-        "AND({First Name}='John',{Age}=21)"
+        "OR({First Name}='John',{Age}=21)"
         >>> match({"First Name": "John"})
         "{First Name}='John'"
         >>> match({"Registered": True})
         "{Registered}=1"
         >>> match({"Owner's Name": "Mike"})
         "{Owner\\'s Name}='Mike'"
```

### Comparing `pyairtable-1.4.0/pyairtable/metadata.py` & `pyairtable-1.5.0/pyairtable/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import posixpath
-from typing import Union, Optional
+from typing import Optional, Union
+
 from pyairtable.api import Api, Base, Table
 
 
 def get_api_bases(api: Union[Api, Base]) -> dict:
     """
     Return list of Bases from an Api or Base instance.
     For More Details `Metadata Api Documentation <https://airtable.com/api/meta>`_
@@ -24,15 +24,15 @@
                         "id": "appSW9R5uCNmRmfl6",
                         "name": "Project Tracker",
                         "permissionLevel": "edit"
                     }
                 ]
             }
     """
-    base_list_url = posixpath.join(api.API_URL, "meta", "bases")
+    base_list_url = api.build_url("meta", "bases")
     return api._request("get", base_list_url)
 
 
 def get_base_schema(base: Union[Base, Table]) -> dict:
     """
     Returns Schema of a Base
     For More Details `Metadata Api Documentation <https://airtable.com/api/meta>`_
@@ -72,17 +72,15 @@
                                 "type": "grid"
                             }
                         ]
                     }
                 ]
             }
     """
-    base_schema_url = posixpath.join(
-        base.API_URL, "meta", "bases", base.base_id, "tables"
-    )
+    base_schema_url = base.build_url("meta", "bases", base.base_id, "tables")
     return base._request("get", base_schema_url)
 
 
 def get_table_schema(table: Table) -> Optional[dict]:
     """
     Returns the specific table schema record provided by base schema list
```

### Comparing `pyairtable-1.4.0/pyairtable/orm/fields.py` & `pyairtable-1.5.0/pyairtable/orm/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,24 +48,15 @@
 >>> contact.company.name # outputs value of Company.name attribute
 
 -----------
 
 """
 import abc
 from datetime import date, datetime
-from typing import (
-    Any,
-    TypeVar,
-    Type,
-    Generic,
-    Optional,
-    List,
-    TYPE_CHECKING,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Generic, List, Optional, Type, TypeVar, Union
 
 from pyairtable import utils
 
 if TYPE_CHECKING:
     from pyairtable.orm import Model  # noqa
 
 T_Linked = TypeVar("T_Linked", bound="Model")
@@ -209,14 +200,42 @@
         if not isinstance(value, date):
             raise ValueError("DateField value must be 'date'")
 
     def __get__(self, *args, **kwargs) -> Optional[datetime]:
         return super().__get__(*args, **kwargs)
 
 
+class LookupField(Field):
+    """
+    Airtable Lookup Fields. Uses ``list`` to store value
+
+    .. versionadded:: 1.5.0
+    """
+
+    def __init__(self, field_name, model: Optional[Type[T_Linked]] = None) -> None:
+        if isinstance(model, str):
+            raise NotImplementedError("path import not implemented")
+            # model = cast(Type[T_Linked], locate(model))
+
+    def to_record_value(self, value: Any) -> list:
+        return list(value)
+
+    def to_internal_value(self, value: list) -> list:
+        return list(value)
+
+    def valid_or_raise(self, value) -> None:
+        if not isinstance(value, list):
+            raise ValueError(
+                f"LookupField '{self.field_name}' value ({value}) must be a 'list'"
+            )
+
+    def __get__(self, *args, **kwargs) -> Optional[list]:
+        return super().__get__(*args, **kwargs)
+
+
 class LinkField(Field, Generic[T_Linked]):
     """Airtable Link field. Uses ``List[Model]`` to store value"""
 
     def __init__(
         self, field_name: str, model: Union[str, Type[T_Linked]], lazy=True
     ) -> None:
         """
@@ -283,15 +302,15 @@
 - [ ] externalSyncSource
 - [ ] formula
 - [ ] lastModifiedBy
 - [ ] lastModifiedTime
 - [ ] multilineText
 - [ ] multipleAttachments
 - [ ] multipleCollaborators
-- [ ] multipleLookupValues
+- [x] multipleLookupValues
 - [ ] multipleRecordLinks
 - [ ] multipleSelects
 - [x] number
 - [ ] percent
 - [ ] phoneNumber
 - [ ] rating
 - [ ] richText
```

### Comparing `pyairtable-1.4.0/pyairtable/orm/model.py` & `pyairtable-1.5.0/pyairtable/orm/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,17 @@
 Finally, you can use :meth:`~pyairtable.orm.model.Model.delete` to delete the record:
 
 >>> contact.delete()
 True
 
 """
 import abc
+from typing import List, Type, TypeVar
+
 from pyairtable import Table
-from typing import TypeVar, Type, List
 
 from .fields import Field
 
 T = TypeVar("T", bound="Model")
 
 
 class Model(metaclass=abc.ABCMeta):
@@ -211,15 +212,15 @@
         record = self.to_record()
         fields = record["fields"]
 
         if not self.id:
             record = table.create(fields, typecast=self.typecast)
             did_create = True
         else:
-            record = table.update(self.id, fields, replace=True, typecast=self.typecast)
+            record = table.update(self.id, fields, typecast=self.typecast)
             did_create = False
 
         self.id = record["id"]
         self.created_time = record["createdTime"]
         return did_create
 
     def delete(self) -> bool:
@@ -255,23 +256,22 @@
         return {"id": self.id, "createdTime": self.created_time, "fields": fields}
 
     @classmethod
     def from_record(cls: Type[T], record: dict) -> T:
         """Create instance from record dictionary"""
         name_attr_map = cls._field_name_attribute_map()
         name_field_map = cls._field_name_descriptor_map()
-        try:
-            # Convert Column Names into model field names
-            # Use field's to_internal to cast into model fields
-            kwargs = {
-                name_attr_map[k]: name_field_map[k].to_internal_value(v)
-                for k, v in record["fields"].items()
-            }
-        except KeyError as exc:
-            raise ValueError("Invalid Field Name: {} for model {}".format(exc, cls))
+        # Convert Column Names into model field names
+        kwargs = {
+            # Use field's to_internal_value to cast into model fields
+            name_attr_map[k]: name_field_map[k].to_internal_value(v)
+            for k, v in record["fields"].items()
+            # Silently proceed if Airtable returns fields we don't recognize
+            if k in name_attr_map
+        }
         instance = cls(**kwargs)
         instance.created_time = record["createdTime"]
         instance.id = record["id"]
         return instance
 
     @classmethod
     def from_id(cls: Type[T], record_id: str, fetch=True) -> T:
```

### Comparing `pyairtable-1.4.0/pyairtable/utils.py` & `pyairtable-1.5.0/pyairtable/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime, date
+from datetime import date, datetime
 from typing import Union
 
 
 def datetime_to_iso_str(value: datetime) -> str:
     """
     Converts ``datetime`` object into Airtable compatible ISO 8601 string
     e.g. "2014-09-05T12:34:56.000Z"
```

### Comparing `pyairtable-1.4.0/setup.cfg` & `pyairtable-1.5.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 version = attr: pyairtable.__version__
 description = Python Client for the Airtable API
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Gui Talarico
 url = https://github.com/gtalarico/pyairtable
 authoremail = gtalarico.dev@gmail.com
-license = The MIT License (MIT)
+license = MIT
 copyright = Copyright 2021 Gui Talarico
 keywords = airtable, api, client, pyairtable
 classifiers = 
 	Intended Audience :: Developers
-	Programming Language :: Python
-	Topic :: Software Development
+	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
+	Topic :: Software Development
 
 [options]
 packages = find:
 install_requires = 
-	requests >= 2
+	requests >= 2.22.0
+	urllib3 < 2
 
 [aliases]
 test = pytest
 
 [mypy]
 mypy_path = pyairtable
 python_version = 3.8
```

