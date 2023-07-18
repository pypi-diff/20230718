# Comparing `tmp/aws_secrets_cache-0.1.0.tar.gz` & `tmp/aws_secrets_cache-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_secrets_cache-0.1.0.tar", max compression
+gzip compressed data, was "aws_secrets_cache-0.2.0.tar", max compression
```

## Comparing `aws_secrets_cache-0.1.0.tar` & `aws_secrets_cache-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1399 2023-06-29 16:33:29.492144 aws_secrets_cache-0.1.0/LICENSE
--rw-r--r--   0        0        0      386 2023-06-29 16:33:29.492144 aws_secrets_cache-0.1.0/README.md
--rw-r--r--   0        0        0     1729 2023-06-29 16:33:29.492144 aws_secrets_cache-0.1.0/aws_secrets_cache/__init__.py
--rw-r--r--   0        0        0      499 2023-06-29 16:33:29.496144 aws_secrets_cache-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 aws_secrets_cache-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1399 2023-07-18 13:24:45.732550 aws_secrets_cache-0.2.0/LICENSE
+-rw-r--r--   0        0        0      386 2023-07-18 13:24:45.732550 aws_secrets_cache-0.2.0/README.md
+-rw-r--r--   0        0        0     1922 2023-07-18 13:24:45.732550 aws_secrets_cache-0.2.0/aws_secrets_cache/__init__.py
+-rw-r--r--   0        0        0      509 2023-07-18 13:24:45.732550 aws_secrets_cache-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 aws_secrets_cache-0.2.0/PKG-INFO
```

### Comparing `aws_secrets_cache-0.1.0/LICENSE` & `aws_secrets_cache-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_secrets_cache-0.1.0/aws_secrets_cache/__init__.py` & `aws_secrets_cache-0.2.0/aws_secrets_cache/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,23 +14,31 @@
     def needs_refresh(self, ttl):
         now = time.monotonic()
         return (now - self.ctime) > ttl
 
 
 class Secrets:
 
-    __slots__ = ('client', 'kms_key_id', 'cache', 'ttl')
+    __slots__ = ('client', 'kms_key_id', 'cache', 'ttl', 'prefix')
 
-    def __init__(self, client, kms_key_id='alias/aws/secretsmanager', ttl=300):
+    def __init__(
+        self,
+        client,
+        kms_key_id='alias/aws/secretsmanager',
+        ttl=300,
+        prefix="",
+    ):
         self.client = client
         self.kms_key_id = kms_key_id
         self.cache = dict()
         self.ttl = ttl
+        self.prefix = prefix
 
     def __setitem__(self, key, val):
+        key = self.prefix + key
         secret_type = 'SecretBinary' if type(val) == bytes else 'SecretString'
         try:
             self.client.put_secret_value(**{'SecretId': key, secret_type: val})
         except botocore.exceptions.ClientError as err:
             if err.response['Error']['Code'] == 'ResourceNotFoundException':
                 self.client.create_secret(**{
                     'Name': key,
@@ -38,19 +46,21 @@
                     'KmsKeyId': self.kms_key_id
                 })
             else:
                 raise err
         self.cache[key] = CacheEntry(value=val)
 
     def fetch_secret(self, key):
+        key = self.prefix + key
         found = self.client.get_secret_value(SecretId=key)
         value = found.get('SecretString') or found['SecretBinary']
         return CacheEntry(value=value)
 
     def __getitem__(self, key):
+        key = self.prefix + key
         try:
             found = self.cache[key]
             if found.needs_refresh(self.ttl):
                 self.cache[key] = self.fetch_secret(key)
             return found.value
         except KeyError:
             found = self.fetch_secret(key)
```

### Comparing `aws_secrets_cache-0.1.0/PKG-INFO` & `aws_secrets_cache-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-secrets-cache
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: BSD-3-Clause
 Author: Łukasz Kostka
 Author-email: lukasz.kostka@mirumee.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

