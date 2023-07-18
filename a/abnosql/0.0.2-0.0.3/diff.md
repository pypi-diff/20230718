# Comparing `tmp/abnosql-0.0.2.tar.gz` & `tmp/abnosql-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abnosql-0.0.2.tar", last modified: Fri Jul  7 02:13:49 2023, max compression
+gzip compressed data, was "abnosql-0.0.3.tar", last modified: Tue Jul 18 02:48:48 2023, max compression
```

## Comparing `abnosql-0.0.2.tar` & `abnosql-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-07 02:13:33.000000 abnosql-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-07 02:13:49.814130 abnosql-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-07 02:13:33.000000 abnosql-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/abnosql/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4078 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/abnosql/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/mocks/mock_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/mocks/mock_dynamodbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/abnosql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/abnosql/plugins/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugins/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugins/table/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugins/table/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/plugins/table/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-07 02:13:33.000000 abnosql-0.0.2/abnosql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:13:49.814130 abnosql-0.0.2/abnosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 02:13:49.000000 abnosql-0.0.2/abnosql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 02:13:49.814130 abnosql-0.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2325 2023-07-07 02:13:33.000000 abnosql-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-18 02:48:34.000000 abnosql-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-07-18 02:48:48.687415 abnosql-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-07-18 02:48:34.000000 abnosql-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4095 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/kms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/mocks/mock_azure_kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/mocks/mock_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/mocks/mock_dynamodbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql/plugins/kms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/kms/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/kms/azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql/plugins/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/table/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/table/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/table/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 02:48:48.691414 abnosql-0.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-07-18 02:48:34.000000 abnosql-0.0.3/setup.py
```

### Comparing `abnosql-0.0.2/LICENSE` & `abnosql-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.2/abnosql/cli.py` & `abnosql-0.0.3/abnosql/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,16 @@
 @click.option('--parameters', '-p')
 @click.option('--database', '-d')
 @click.option('--config', '-c')
 def query_sql(table, statement, parameters, database, config):
     tb = _table(table, get_config(config), database=database)
     dump(tb.query_sql(
         statement=statement,
-        parameters=parameters
+        parameters=parameters,
+        limit=1
     )['items'])
 
 
 cli.add_command(get_item)
 cli.add_command(put_item)
 cli.add_command(put_items)
 cli.add_command(delete_item)
```

### Comparing `abnosql-0.0.2/abnosql/mocks/mock_cosmos.py` & `abnosql-0.0.3/abnosql/mocks/mock_cosmos.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,25 +2,32 @@
 import json
 import re
 import typing as t
 from urllib import parse as urlparse
 
 import responses  # type: ignore
 
+from abnosql.plugins.table.memory import get_table_count
 from abnosql import table
 
 
 KEY_ATTRS: t.Dict[str, t.List[str]] = {}
+CRYPTO_ATTRS: t.Dict[str, t.List[str]] = {}
 
 
 def set_keyattrs(key_attrs: t.Dict[str, t.List[str]]):
     global KEY_ATTRS
     KEY_ATTRS = key_attrs
 
 
+def set_crypto_attrs(attrs: t.Dict[str, t.List[str]]):
+    global CRYPTO_ATTRS
+    CRYPTO_ATTRS = attrs
+
+
 def mock_cosmos(f):
 
     def _get_key(headers, key_attrs, doc_id):
         hk = key_attrs[0]
         rk = key_attrs[1] if len(key_attrs) > 1 else None
         _part_keys = headers.get('x-ms-documentdb-partitionkey')
         if isinstance(_part_keys, str) and len(_part_keys) > 0:
@@ -69,17 +76,25 @@
         table_name = parts[3]
         global KEY_ATTRS
         key_attrs = KEY_ATTRS.get(table_name)
         if key_attrs is None:
             return _response(404)
 
         # use memory table to mock cosmos
+        global CRYPTO_ATTRS
+        crypto_attrs = CRYPTO_ATTRS.get(table_name)
+        config = {'key_attrs': key_attrs}
+        if crypto_attrs is not None:
+            config['crypto'] = {
+                'attrs': crypto_attrs,
+                'key_attrs': key_attrs
+            }
         tb = table(
             table_name,
-            config={'key_attrs': key_attrs},
+            config=config,
             database='memory'
         )
 
         # /dbs/{database}/colls/{table}/docs/{docid}
         if len(parts) == 6 and parts[-2] == 'docs':
             key = _get_key(headers, key_attrs, parts[-1])
             if request.method == 'GET':
@@ -92,22 +107,28 @@
 
         # /dbs/{database}/colls/{table}/docs
         elif len(parts) == 5 and parts[-1] == 'docs':
             if request.method == 'POST':
                 is_query = headers.get('x-ms-documentdb-isquery') == 'true'
                 item = json.loads(request.body)
                 if is_query is True:
-                    # TODO(x-ms-continuation)
-                    # {'initial_headers': {'x-ms-continuation': 'sometoken'}}
                     items = tb.query_sql(
                         item['query'],
-                        {_['name']: _['value'] for _ in item['parameters']}
+                        {
+                            _['name']: _['value']
+                            for _ in item.get('parameters', {})
+                        }
                     )
+                    headers = {
+                        'x-ms-resource-usage': 'documentsCount=%s' % (
+                            get_table_count(table_name)
+                        )
+                    }
                     return _response(
-                        200, {'Documents': items}
+                        200, {'Documents': items}, headers
                     )
                 else:
                     tb.put_item(item)
                 return _response(201, None)
 
         # upsert_item() reads the collection
         # /dbs/{database}/colls/{table}
```

### Comparing `abnosql-0.0.2/abnosql/mocks/mock_dynamodbx.py` & `abnosql-0.0.3/abnosql/mocks/mock_dynamodbx.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.2/abnosql/plugin.py` & `abnosql-0.0.3/abnosql/plugin.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.2/abnosql/plugins/table/cosmos.py` & `abnosql-0.0.3/abnosql/plugins/table/cosmos.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 import os
 import typing as t
 
 import pluggy  # type: ignore
 
 import abnosql.exceptions as ex
 from abnosql.plugin import PM
+from abnosql.table import add_audit
 from abnosql.table import get_sql_params
+from abnosql.table import kms_decrypt_item
+from abnosql.table import kms_encrypt_item
+from abnosql.table import kms_process_query_items
+from abnosql.table import parse_connstr
 from abnosql.table import TableBase
 from abnosql.table import validate_query_attrs
 
 hookimpl = pluggy.HookimplMarker('abnosql.table')
 
 try:
     from azure.cosmos import CosmosClient  # type: ignore
@@ -82,21 +87,31 @@
             config = t.cast(t.Dict, _config)
         self.config = config
 
     def _database_client(self):
         _client = self.config.get('database_client', self.database_client)
         if _client is not None:
             return _client
+        pc = parse_connstr()
         cf = {}
+        if pc is not None:
+            cf.update({
+                'account': pc.username,
+                'database': pc.hostname,
+                'credential': pc.password
+            })
         required = ['endpoint', 'credential', 'database']
         for attr in ['account'] + required:
-            cf[attr] = self.config.get(
+            val = self.config.get(
                 attr, os.environ.get('ABNOSQL_COSMOS_' + attr.upper())
             )
-        if cf['endpoint'] is None and cf['account'] is not None:
+            # override
+            if val is not None:
+                cf[attr] = val
+        if cf.get('endpoint') is None and cf['account'] is not None:
             cf['endpoint'] = 'https://%s.documents.azure.com' % cf['account']
         missing = [_ for _ in required if cf[_] is None]
         if len(missing):
             raise ex.ConfigException('missing config: ' + ', '.join(missing))
         self.database_client = CosmosClient(
             url=cf['endpoint'], credential=cf['credential']
         ).get_database_client(cf['database'])
@@ -111,44 +126,60 @@
             self._container(self.name).read_item(
                 **get_key_kwargs(**kwargs)
             )
         )
         _item = self.pm.hook.get_item_post(table=self.name, item=item)
         if _item:
             item = _item
+        item = kms_decrypt_item(self.config, item)
         return item
 
     @cosmos_ex_handler()
-    def put_item(self, item: t.Dict):
+    def put_item(
+        self,
+        item: t.Dict,
+        user: t.Optional[str] = None
+    ):
+        if user:
+            item = add_audit(item, user)
+        _item = self.pm.hook.put_item_pre(table=self.name, item=item)
+        if _item:
+            item = _item[0]
+        item = kms_encrypt_item(self.config, item)
         self._container(self.name).upsert_item(item)
         self.pm.hook.put_item_post(table=self.name, item=item)
 
     @cosmos_ex_handler()
-    def put_items(self, items: t.Iterable[t.Dict]):
+    def put_items(
+        self,
+        items: t.Iterable[t.Dict],
+        user: t.Optional[str] = None
+    ):
         # TODO(batch)
         for item in items:
-            self.put_item(item)
+            self.put_item(item, user)
         self.pm.hook.put_items_post(table=self.name, items=items)
 
     @cosmos_ex_handler()
     def delete_item(self, **kwargs):
         self._container(self.name).delete_item(
             **get_key_kwargs(**kwargs)
         )
         self.pm.hook.delete_item_post(table=self.name, key=dict(kwargs))
 
     @cosmos_ex_handler()
     def query(
         self,
-        key: t.Dict[str, t.Any],
+        key: t.Optional[t.Dict[str, t.Any]] = None,
         filters: t.Optional[t.Dict[str, t.Any]] = None,
         limit: t.Optional[int] = None,
         next: t.Optional[str] = None
     ) -> t.Dict[str, t.Any]:
         filters = filters or {}
+        key = key or {}
         validate_query_attrs(key, filters)
         parameters = {
             f'@{k}': v
             for k, v in filters.items()
         }
         parameters.update({
             f'@{k}': v
@@ -156,20 +187,22 @@
         })
         statement = f'SELECT * FROM {self.name}'
         op = 'WHERE'
         for param in parameters.keys():
             statement += f' {op} {self.name}.{param[1:]} = {param}'
             op = 'AND'
 
-        return self.query_sql(
+        resp = self.query_sql(
             statement,
             parameters,
             limit=limit,
             next=next
         )
+        resp['items'] = kms_process_query_items(self.config, resp['items'])
+        return resp
 
     @cosmos_ex_handler()
     def query_sql(
         self,
         statement: str,
         parameters: t.Optional[t.Dict[str, t.Any]] = None,
         limit: t.Optional[int] = None,
@@ -186,27 +219,51 @@
 
         kwargs: t.Dict[str, t.Any] = {
             'query': statement,
             'enable_cross_partition_query': True
         }
         if len(params):
             kwargs['parameters'] = params
-        if limit:
-            kwargs['max_item_count'] = limit
-        # TODO(x-ms-continuation)
-        # from microsoft / planetary-computer-tasks on github
-        # The Python SDK does not support continuation tokens
-        # for cross-partition queries.
-        #
-        # response_hook callable doesnt show x-ms-continuation
-        # header with or without enable_cross_partition_query
-        # even when max_item_count = 1
-        # print(f'KWARGS: {kwargs}')
+        # python cosmos SDK doesnt support
+        # kwargs['max_item_count'] = limit
+        limit = limit or 100
+        next = next or '0'
+
+        # Python SDK does not support continuation
+        # for cross-partition queries - see limitations https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos  # noqa
+        # so add OFFSET and LIMIT if not already present
+        if (
+            ' OFFSET ' not in statement.upper()
+            and ' LIMIT ' not in statement.upper()
+        ):
+            kwargs['query'] += f' OFFSET {next} LIMIT {limit}'
         container = self._container(self.name)
         items = list(container.query_items(**kwargs))
+        headers = container.client_connection.last_response_headers
+        # continuation = headers.get('x-ms-continuation')
+        # total size in 'x-ms-resource-usage' eg ;documentsCount=3
+        resource_usage = {
+            _.split('=', 1)[0]: _.split('=', 1)[1]
+            for _ in headers.get('x-ms-resource-usage', '').split(';')
+            if '=' in _
+        }
+        doc_count = None
+        try:
+            doc_count = int(resource_usage['documentsCount'])
+        except Exception:
+            doc_count = None
+
         for i in range(len(items)):
             items[i] = strip_cosmos_attrs(items[i])
+        items = kms_process_query_items(self.config, items)
+        _next = None
+        try:
+            _next = limit + int(next)
+        except Exception:
+            _next = None
+        if doc_count is not None and _next is not None and _next >= doc_count:
+            _next = None
 
         return {
             'items': items,
-            'next': None
+            'next': str(_next) if _next and len(items) else None
         }
```

### Comparing `abnosql-0.0.2/abnosql/plugins/table/dynamodb.py` & `abnosql-0.0.3/abnosql/plugins/table/dynamodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+from base64 import b64decode
+from base64 import b64encode
 from datetime import datetime
 import functools
 import json
 import os
 import typing as t
 
-from boto3.dynamodb.types import Binary  # type: ignore
-from boto3.dynamodb.types import Decimal  # type: ignore
-from botocore.exceptions import ClientError  # type: ignore
-from botocore.exceptions import NoCredentialsError  # type: ignore
-from dynamodb_json import json_util  # type: ignore
 import pluggy  # type: ignore
 
 import abnosql.exceptions as ex
 from abnosql.plugin import PM
+from abnosql.table import add_audit
 from abnosql.table import get_sql_params
+from abnosql.table import kms_decrypt_item
+from abnosql.table import kms_encrypt_item
+from abnosql.table import kms_process_query_items
 from abnosql.table import TableBase
 from abnosql.table import validate_query_attrs
 
 hookimpl = pluggy.HookimplMarker('abnosql.table')
 
 AWS_DEFAULT_REGION = os.environ.get('AWS_DEFAULT_REGION', 'us-east-1')
 
 try:
     import boto3  # type: ignore
-    # import botocore.client
-    # import botocore.exceptions
+    from boto3.dynamodb.types import Binary  # type: ignore
+    from boto3.dynamodb.types import Decimal  # type: ignore
+    from botocore.exceptions import ClientError  # type: ignore
+    from botocore.exceptions import NoCredentialsError  # type: ignore
+    from dynamodb_json import json_util  # type: ignore
 except ImportError:
     MISSING_DEPS = True
 
 
 # http://stackoverflow.com/questions/11875770/how-to-overcome-datetime-datetime-not-json-serializable-in-python  # noqa
 # see https://github.com/Alonreznik/dynamodb-json/blob/master/dynamodb_json/json_util.py  # noqa
 def json_serial(obj):
@@ -88,41 +92,46 @@
         else 'NULL' if val is None
         else 'BOOL' if isinstance(val, bool)
         else 'S'
     )
     return {_type: str(val)}
 
 
-def get_dynamodb_query_kwargs(
+def get_dynamodb_kwargs(
     name: str,
-    key: t.Dict[str, t.Any],
+    key: t.Optional[t.Dict[str, t.Any]] = None,
     filters: t.Optional[t.Dict[str, t.Any]] = None
 ) -> t.Dict:
-    if len(key) > 2 or len(key) == 0:
+    key = key or {}
+    if len(key) > 2:
         raise ValueError('key length must be 1 or 2')
     filters = filters or {}
     validate_query_attrs(key, filters)
 
-    _values = {
-        f':{k}': v
-        for k, v in key.items()
-    }
+    _values = {}
+    if len(key):
+        _values = {
+            f':{k}': v
+            for k, v in key.items()
+        }
     _names = {}
     for k, v in filters.items():
         _names[f'#{k}'] = k
         _values[f':{k}'] = v
 
-    kwargs = {
+    kwargs: t.Dict[str, t.Any] = {
         'TableName': name,
-        'Select': 'ALL_ATTRIBUTES',
-        'KeyConditionExpression': ' AND '.join([
-            f'{k} = :{k}' for k in key.keys()
-        ]),
-        'ExpressionAttributeValues': _values
+        'Select': 'ALL_ATTRIBUTES'
     }
+    if len(key):
+        kwargs['KeyConditionExpression'] = ' AND '.join([
+            f'{k} = :{k}' for k in key.keys()
+        ])
+    if len(_values):
+        kwargs['ExpressionAttributeValues'] = _values
     if len(_names):
         kwargs['ExpressionAttributeNames'] = _names
     if len(filters):
         kwargs['FilterExpression'] = ' AND '.join([
             f'{k} = :{k}' for k in filters.keys()
         ])
     return kwargs
@@ -158,53 +167,77 @@
             TableName=self.name,
             Key=get_key(**kwargs)
         ), self.config.get('deserializer'))
         item = response.get('Item')
         _item = self.pm.hook.get_item_post(table=self.name, item=item)
         if _item:
             item = _item
+        item = kms_decrypt_item(self.config, item)
         return item
 
     @dynamodb_ex_handler()
-    def put_item(self, item: t.Dict):
+    def put_item(
+        self, item:
+        t.Dict,
+        user: t.Optional[str] = None
+    ):
+        if user:
+            item = add_audit(item, user)
+        _item = self.pm.hook.put_item_pre(table=self.name, item=item)
+        if _item:
+            item = _item[0]
+        item = kms_encrypt_item(self.config, item)
         self.table.put_item(Item=item)
         self.pm.hook.put_item_post(table=self.name, item=item)
 
     @dynamodb_ex_handler()
-    def put_items(self, items: t.Iterable[t.Dict]):
+    def put_items(
+        self,
+        items: t.Iterable[t.Dict],
+        user: t.Optional[str] = None
+    ):
         # TODO(batch)
         for item in items:
-            self.put_item(item)
+            self.put_item(item, user)
         self.pm.hook.put_items_post(table=self.name, items=items)
 
     @dynamodb_ex_handler()
     def delete_item(self, **kwargs):
         key = get_key(**kwargs)
         self.table.delete_item(Key=key)
         self.pm.hook.delete_item_post(table=self.name, key=key)
 
     @dynamodb_ex_handler()
     def query(
         self,
-        key: t.Dict[str, t.Any],
+        key: t.Optional[t.Dict[str, t.Any]] = None,
         filters: t.Optional[t.Dict[str, t.Any]] = None,
         limit: t.Optional[int] = None,
         next: t.Optional[str] = None
     ) -> t.Dict[str, t.Any]:
-        kwargs = get_dynamodb_query_kwargs(
+        kwargs = get_dynamodb_kwargs(
             self.name, key, filters
         )
         if next is not None:
-            kwargs['ExclusiveStartKey'] = next
+            kwargs['ExclusiveStartKey'] = json.loads(b64decode(next).decode())
         if limit is not None:
             kwargs['Limit'] = limit
-        response = self.table.query(**kwargs)
+        response = None
+        if key is not None:
+            response = self.table.query(**kwargs)
+        else:
+            response = self.table.scan(**kwargs)
+        items = response.get('Items', [])
+        items = kms_process_query_items(self.config, items)
+        last = response.get('LastEvaluatedKey')
+        if last is not None:
+            last = b64encode(json.dumps(last).encode()).decode()
         return {
-            'items': deserialize(response.get('Items', [])),
-            'next': response.get('LastEvaluatedKey')
+            'items': deserialize(items),
+            'next': last
         }
 
     @dynamodb_ex_handler()
     def query_sql(
         self,
         statement: str,
         parameters: t.Optional[t.Dict[str, t.Any]] = None,
@@ -225,14 +258,15 @@
             kwargs['Limit'] = limit
         if len(params):
             kwargs['Parameters'] = params
 
         response = client.execute_statement(**kwargs)
         items = []
         _items = response.get('Items', [])
+        _items = kms_process_query_items(self.config, _items)
         for item in _items:
             items.append(json_util.loads(json.dumps(item)))
 
         return {
             'items': items,
             'next': response.get('NextToken')
         }
```

### Comparing `abnosql-0.0.2/abnosql/plugins/table/memory.py` & `abnosql-0.0.3/abnosql/plugins/table/memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import functools
 import json
 import typing as t
 
 import pluggy  # type: ignore
 import sqlglot  # type: ignore
 from sqlglot.executor import execute  # type: ignore
+from sqlglot import exp  # type: ignore
+from sqlglot import parse_one  # type: ignore
 
 import abnosql.exceptions as ex
 from abnosql.plugin import PM
+from abnosql.table import add_audit
 from abnosql.table import get_sql_params
+from abnosql.table import kms_decrypt_item
+from abnosql.table import kms_encrypt_item
+from abnosql.table import kms_process_query_items
 from abnosql.table import quote_str
 from abnosql.table import TableBase
 from abnosql.table import validate_query_attrs
 
 
 hookimpl = pluggy.HookimplMarker('abnosql.table')
 
@@ -35,14 +41,19 @@
     return str(next(
         sqlglot.parse_one(statement).find_all(  # type: ignore
             sqlglot.exp.Table
         )
     ))
 
 
+def get_table_count(name: str) -> int:
+    global TABLES
+    return len(list(TABLES.get(name, {}).values()))
+
+
 def query_items(
     statement: str,
     items: t.List[t.Dict[str, t.Any]],
     parameters: t.Optional[t.List[t.Dict[str, t.Any]]] = None,
     table_name: t.Optional[str] = None
 ) -> t.List[t.Dict]:
     parameters = parameters or []
@@ -65,23 +76,42 @@
                 _val = quote_str(_val)
             statement = statement.replace(_param, str(_val))
 
     if table_name is None:
         table_name = get_table_name(statement)
 
     # sqlglot execute can't handle dict or list keys...
+    _items = []
     _unpack = {}
-    for i in range(len(items)):
-        for k, v in items[i].items():
+    for item in items:
+        new_item = item.copy()
+        for k in item.keys():
+            v = item[k]
             if type(v) in [dict, list]:
                 _unpack[k] = True
-                items[i][k] = json.dumps(v)
+                new_item[k] = json.dumps(v)
+        _items.append(new_item)
+
+    # get any offset supplied
+    offset = None
+    for _offset in parse_one(statement).find_all(exp.Offset):  # type: ignore
+        offset = _offset
+        break
+    if offset:
+        try:
+            offset = int(str(offset).split(' ')[-1])  # type: ignore
+        except Exception:
+            offset = None
+
+    # slice the data via offset
+    if isinstance(offset, int) and offset > 0 and offset < len(_items):
+        _items = _items[offset:]
 
     # query the data
-    resp = execute(statement, tables={table_name: items})
+    resp = execute(statement, tables={table_name: _items})
     rows = [
         dict(zip(resp.columns, row))
         for row in resp.rows
     ]
 
     # unpack
     if len(_unpack):
@@ -138,32 +168,44 @@
             item = self.items.get(key)
         else:
             global TABLES
             item = TABLES.get(self.name, {}).get(key)
         _item = self.pm.hook.get_item_post(table=self.name, item=item)
         if _item:
             item = _item
+        item = kms_decrypt_item(self.config, item)
         return item
 
     @memory_ex_handler()
-    def put_item(self, item: t.Dict):
+    def put_item(
+        self,
+        item: t.Dict,
+        user: t.Optional[str] = None
+    ):
+        if user:
+            item = add_audit(item, user)
         key = ':'.join([item[_] for _ in self.key_attrs])
+        item = kms_encrypt_item(self.config, item)
         if self.items:
             self.items[key] = item
         else:
             global TABLES
             if self.name not in TABLES:
                 TABLES[self.name] = {}
             TABLES[self.name][key] = item
         self.pm.hook.put_item_post(table=self.name, item=item)
 
     @memory_ex_handler()
-    def put_items(self, items: t.Iterable[t.Dict]):
+    def put_items(
+        self,
+        items: t.Iterable[t.Dict],
+        user: t.Optional[str] = None
+    ):
         for item in items:
-            self.put_item(item)
+            self.put_item(item, user)
         self.pm.hook.put_items_post(table=self.name, items=items)
 
     @memory_ex_handler()
     def delete_item(self, **kwargs):
         key = get_key(**kwargs)
         if self.items:
             self.items.pop(key, None)
@@ -192,14 +234,15 @@
         })
         statement = f'SELECT * FROM {self.name}'
         op = 'WHERE'
         for param in parameters.keys():
             statement += f' {op} {self.name}.{param[1:]} = {param}'
             op = 'AND'
         items = self.query_sql(statement)
+        items = kms_process_query_items(self.config, items)
         return {
             'items': items,
             'next': None
         }
 
     @memory_ex_handler()
     def query_sql(
@@ -219,8 +262,10 @@
         )
         items = []
         if self.items:
             items = list(self.items.values())
         else:
             global TABLES
             items = list(TABLES.get(self.name, {}).values())
-        return query_items(statement, items, params, self.name)
+        items = query_items(statement, items, params, self.name)
+        items = kms_process_query_items(self.config, items)
+        return items
```

### Comparing `abnosql-0.0.2/abnosql.egg-info/SOURCES.txt` & `abnosql-0.0.3/abnosql.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 abnosql/__init__.py
 abnosql/cli.py
 abnosql/exceptions.py
+abnosql/kms.py
 abnosql/plugin.py
 abnosql/table.py
 abnosql/version.py
 abnosql.egg-info/PKG-INFO
 abnosql.egg-info/SOURCES.txt
 abnosql.egg-info/dependency_links.txt
 abnosql.egg-info/entry_points.txt
 abnosql.egg-info/requires.txt
 abnosql.egg-info/top_level.txt
 abnosql/mocks/__init__.py
+abnosql/mocks/mock_azure_kms.py
 abnosql/mocks/mock_cosmos.py
 abnosql/mocks/mock_dynamodbx.py
 abnosql/plugins/__init__.py
+abnosql/plugins/kms/__init__.py
+abnosql/plugins/kms/aws.py
+abnosql/plugins/kms/azure.py
 abnosql/plugins/table/__init__.py
 abnosql/plugins/table/cosmos.py
 abnosql/plugins/table/dynamodb.py
 abnosql/plugins/table/memory.py
```

### Comparing `abnosql-0.0.2/setup.py` & `abnosql-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,36 +20,55 @@
     return parts[2].strip('\'"')
 
 
 __version__ = get_version()
 
 
 base_deps = [
+    'pluggy'
+]
+cli_deps = [
     'click',
-    'pluggy',
-    'sqlglot',
     'tabulate'
 ]
-dynamodb_deps = [
+aws_kms_deps = [
+    'boto3',
+    'aws-encryption-sdk',
+]
+aws_dynamodb_deps = [
     'boto3',
     'dynamodb_json'
 ]
-cosmos_deps = [
+azure_cosmos_deps = [
     'azure-cosmos'
 ]
-all_deps = base_deps + dynamodb_deps + cosmos_deps
-tests_require = all_deps + [
+azure_kms_deps = [
+    'azure-identity',
+    'azure-keyvault-keys',
+    'cryptography'  # already used by azure-identity
+]
+all_deps = (
+    base_deps
+    + cli_deps
+    + aws_dynamodb_deps
+    + aws_kms_deps
+    + azure_cosmos_deps
+    + azure_kms_deps
+)
+test_deps = all_deps + [
     'coverage',
     'moto[dynamodb]',
+    'moto[kms]',
     'mypy',
     'pytest',
     'pytest-cov',
-    'responses'
+    'responses',
+    'sqlglot'
 ]
-dev_require = tests_require + [
+dev_deps = test_deps + [
     'pdoc',
     'pre-commit'
 ]
 
 setup(
     name='abnosql',
     version=__version__,
@@ -65,35 +84,40 @@
     download_url='http://pypi.python.org/pypi/abnosql',
     keywords='nosql, azure cosmos, aws dynamodb',
 
     license='MIT',
     platforms='any',
     packages=find_packages(exclude=['tests']),
 
-    tests_require=tests_require,
+    tests_require=test_deps,
     extras_require={
-        'dev': dev_require,
-        'test': tests_require,
-        'dynamodb': dynamodb_deps,
-        'cosmos': cosmos_deps
+        'dev': dev_deps,
+        'test': test_deps,
+        'cli': cli_deps,
+        'aws': aws_dynamodb_deps + aws_kms_deps,
+        'azure': azure_cosmos_deps + azure_kms_deps,
+        'dynamodb': aws_dynamodb_deps,
+        'cosmos': azure_cosmos_deps,
+        'aws-kms': aws_kms_deps,
+        'azure-kms': azure_kms_deps
     },
-    python_requires='>=3.8,<4.0',
+    python_requires='>=3.9,<4.0',
     test_suite='tests',
 
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Topic :: System :: Distributed Computing',
         'Topic :: Database :: Front-Ends',
         'Typing :: Typed'
     ],
     entry_points={
         'console_scripts': [
-            'abnosql = abnosql:cli',
+            'abnosql = abnosql:cli.cli',
         ]
     }
 )
```

