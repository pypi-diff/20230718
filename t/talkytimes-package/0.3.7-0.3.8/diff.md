# Comparing `tmp/talkytimes_package-0.3.7.tar.gz` & `tmp/talkytimes_package-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.3.7.tar", last modified: Tue Jul 18 01:49:21 2023, max compression
+gzip compressed data, was "talkytimes_package-0.3.8.tar", last modified: Tue Jul 18 02:01:16 2023, max compression
```

## Comparing `talkytimes_package-0.3.7.tar` & `talkytimes_package-0.3.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 01:49:21.525198 talkytimes_package-0.3.7/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.7/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-18 01:49:21.525198 talkytimes_package-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.7/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.7/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-18 01:49:21.526209 talkytimes_package-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:49:21.502001 talkytimes_package-0.3.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 01:49:21.509460 talkytimes_package-0.3.7/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.7/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      525 2023-07-18 01:47:45.000000 talkytimes_package-0.3.7/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     1950 2023-07-18 01:48:46.000000 talkytimes_package-0.3.7/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:49:21.511473 talkytimes_package-0.3.7/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-18 01:48:37.000000 talkytimes_package-0.3.7/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.7/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3955 2023-07-18 01:48:52.000000 talkytimes_package-0.3.7/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:49:21.525198 talkytimes_package-0.3.7/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-18 01:49:21.000000 talkytimes_package-0.3.7/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-18 01:49:21.000000 talkytimes_package-0.3.7/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 01:49:21.000000 talkytimes_package-0.3.7/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-18 01:49:21.000000 talkytimes_package-0.3.7/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-18 01:49:21.000000 talkytimes_package-0.3.7/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 02:01:16.729896 talkytimes_package-0.3.8/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-18 02:01:16.729896 talkytimes_package-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.8/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-18 02:01:16.731898 talkytimes_package-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:01:16.693898 talkytimes_package-0.3.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 02:01:16.702899 talkytimes_package-0.3.8/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.8/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      525 2023-07-18 01:47:45.000000 talkytimes_package-0.3.8/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     1676 2023-07-18 01:59:23.000000 talkytimes_package-0.3.8/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:01:16.706900 talkytimes_package-0.3.8/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-18 02:00:22.000000 talkytimes_package-0.3.8/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.8/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     3955 2023-07-18 01:48:52.000000 talkytimes_package-0.3.8/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:01:16.728898 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-18 02:01:16.000000 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-18 02:01:16.000000 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:01:16.000000 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-18 02:01:16.000000 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-18 02:01:16.000000 talkytimes_package-0.3.8/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.3.7/LICENSE` & `talkytimes_package-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.7/src/dynamodb/base.py` & `talkytimes_package-0.3.8/src/dynamodb/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.7/src/dynamodb/dynamodb.py` & `talkytimes_package-0.3.8/src/dynamodb/dynamodb.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Optional
 
 from dynamodb.base import AbstractDynamoDB
 
 
 class DynamoDB(AbstractDynamoDB):
     def get_user(self, *, external_id: str) -> Any:
-        data = dict(external_id=external_id)
+        data = dict(id=external_id)
         return self.get_item(key=data)
 
     def get_users(self) -> dict[str, Any]:
         response = self.table.scan()
         print(response)
         data = response.get("Items")
 
@@ -24,15 +24,15 @@
         *,
         external_id: str,
         status: str,
         messages: Optional[str] = "0",
         emails: Optional[str] = "0"
     ) -> Any:
         data = dict(
-            external_id=external_id,
+            id=external_id,
             user_info=json.dumps(
                 dict(
                     status=status,
                     messages=messages,
                     emails=emails
                 )
             )
@@ -51,24 +51,15 @@
             dict(
                 status=status,
                 messages=messages,
                 emails=emails
             )
         )
         self.table.update_item(
-            ExpressionAttributeNames={
-                '#AT': 'user_info',
-            },
-            ExpressionAttributeValues={
-                ':t': {
-                    'S': new_user_info,
-                },
-            },
             Key={
-                'external_id': {
-                    'S': external_id,
-                }
+                'id': external_id
             },
-            ReturnValues='ALL_NEW',
-            TableName=self.table_name,
-            UpdateExpression='SET #AT = :t',
+            UpdateExpression='SET user_info = :val1',
+            ExpressionAttributeValues={
+                ':val1': new_user_info
+            }
         )
```

### Comparing `talkytimes_package-0.3.7/src/talkytimes/base.py` & `talkytimes_package-0.3.8/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.7/src/talkytimes/talkytimes.py` & `talkytimes_package-0.3.8/src/talkytimes/talkytimes.py`

 * *Files identical despite different names*

