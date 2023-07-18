# Comparing `tmp/tap-exactonline-0.2.8.tar.gz` & `tmp/tap-exactonline-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-exactonline-0.2.8.tar", max compression
+gzip compressed data, was "tap-exactonline-0.2.9.tar", max compression
```

## Comparing `tap-exactonline-0.2.8.tar` & `tap-exactonline-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      889 2023-01-13 14:07:23.970445 tap-exactonline-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-22 12:31:43.648865 tap-exactonline-0.2.8/tap_exactonline/__init__.py
--rw-r--r--   0        0        0     4458 2023-01-13 13:58:24.733227 tap-exactonline-0.2.8/tap_exactonline/client.py
--rw-r--r--   0        0        0     1700 2022-09-23 12:05:18.001392 tap-exactonline-0.2.8/tap_exactonline/helpers/ExactApiWrapper.py
--rw-r--r--   0        0        0      592 2022-08-22 12:31:43.649457 tap-exactonline-0.2.8/tap_exactonline/helpers/parser.py
--rw-r--r--   0        0        0      593 2022-09-23 12:53:38.265155 tap-exactonline-0.2.8/tap_exactonline/helpers/secretsManager.py
--rw-r--r--   0        0        0    41899 2023-01-13 14:07:15.496466 tap-exactonline-0.2.8/tap_exactonline/streams.py
--rw-r--r--   0        0        0     3152 2023-01-13 13:49:14.237489 tap-exactonline-0.2.8/tap_exactonline/tap.py
--rw-r--r--   0        0        0       38 2022-08-22 12:31:43.650147 tap-exactonline-0.2.8/tap_exactonline/tests/__init__.py
--rw-r--r--   0        0        0      663 2022-08-22 12:31:43.650332 tap-exactonline-0.2.8/tap_exactonline/tests/test_core.py
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 tap-exactonline-0.2.8/setup.py
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 tap-exactonline-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      889 2023-01-13 14:11:42.821377 tap-exactonline-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-22 12:31:43.648865 tap-exactonline-0.2.9/tap_exactonline/__init__.py
+-rw-r--r--   0        0        0     4458 2023-01-13 13:58:24.733227 tap-exactonline-0.2.9/tap_exactonline/client.py
+-rw-r--r--   0        0        0     1700 2022-09-23 12:05:18.001392 tap-exactonline-0.2.9/tap_exactonline/helpers/ExactApiWrapper.py
+-rw-r--r--   0        0        0      592 2022-08-22 12:31:43.649457 tap-exactonline-0.2.9/tap_exactonline/helpers/parser.py
+-rw-r--r--   0        0        0      593 2022-09-23 12:53:38.265155 tap-exactonline-0.2.9/tap_exactonline/helpers/secretsManager.py
+-rw-r--r--   0        0        0    41883 2023-01-13 14:11:38.336989 tap-exactonline-0.2.9/tap_exactonline/streams.py
+-rw-r--r--   0        0        0     3152 2023-01-13 13:49:14.237489 tap-exactonline-0.2.9/tap_exactonline/tap.py
+-rw-r--r--   0        0        0       38 2022-08-22 12:31:43.650147 tap-exactonline-0.2.9/tap_exactonline/tests/__init__.py
+-rw-r--r--   0        0        0      663 2022-08-22 12:31:43.650332 tap-exactonline-0.2.9/tap_exactonline/tests/test_core.py
+-rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 tap-exactonline-0.2.9/setup.py
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 tap-exactonline-0.2.9/PKG-INFO
```

### Comparing `tap-exactonline-0.2.8/pyproject.toml` & `tap-exactonline-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exactonline"
-version = "0.2.8"
+version = "0.2.9"
 description = "`tap-exactonline` is a Singer tap for ExactOnline, built with the Meltano SDK for Singer Taps."
 authors = ["Hidde Stokvis"]
 keywords = [
     "ELT",
     "ExactOnline",
 ]
 license = "Apache 2.0"
```

### Comparing `tap-exactonline-0.2.8/tap_exactonline/client.py` & `tap-exactonline-0.2.9/tap_exactonline/client.py`

 * *Files identical despite different names*

### Comparing `tap-exactonline-0.2.8/tap_exactonline/helpers/ExactApiWrapper.py` & `tap-exactonline-0.2.9/tap_exactonline/helpers/ExactApiWrapper.py`

 * *Files identical despite different names*

### Comparing `tap-exactonline-0.2.8/tap_exactonline/helpers/parser.py` & `tap-exactonline-0.2.9/tap_exactonline/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `tap-exactonline-0.2.8/tap_exactonline/helpers/secretsManager.py` & `tap-exactonline-0.2.9/tap_exactonline/helpers/secretsManager.py`

 * *Files identical despite different names*

### Comparing `tap-exactonline-0.2.8/tap_exactonline/streams.py` & `tap-exactonline-0.2.9/tap_exactonline/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """Stream type classes for tap-exactonline."""
-import logging
-
 from singer_sdk import typing as th  # JSON Schema typing helpers
 from tap_exactonline.client import ExactOnlineStream
 
 
 class ContactsStream(ExactOnlineStream):
     name = "contacts"
     path = "sync/CRM/Contacts"
@@ -674,15 +672,15 @@
     ).to_dict()
 
 
 class DocumentAttachementsStream(ExactOnlineStream):
     name = "document_attachements"
     path = "bulk/Documents/DocumentAttachments"
     primary_keys = ["ID"]
-    replication_key="Timestmap"
+    replication_key="Timestamp"
     schema = th.PropertiesList(
         th.Property("Timestamp", th.IntegerType),
         th.Property("ID", th.UUIDType),
         th.Property("Attachment", th.StringType),
         th.Property("Document", th.UUIDType),
         th.Property("FileName", th.StringType),
         th.Property("FileSize", th.NumberType),
```

### Comparing `tap-exactonline-0.2.8/tap_exactonline/tap.py` & `tap-exactonline-0.2.9/tap_exactonline/tap.py`

 * *Files identical despite different names*

### Comparing `tap-exactonline-0.2.8/tap_exactonline/tests/test_core.py` & `tap-exactonline-0.2.9/tap_exactonline/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap-exactonline-0.2.8/setup.py` & `tap-exactonline-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 entry_points = \
 {'console_scripts': ['tap-exactonline = '
                      'tap_exactonline.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exactonline',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': '`tap-exactonline` is a Singer tap for ExactOnline, built with the Meltano SDK for Singer Taps.',
     'long_description': 'None',
     'author': 'Hidde Stokvis',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap-exactonline-0.2.8/PKG-INFO` & `tap-exactonline-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exactonline
-Version: 0.2.8
+Version: 0.2.9
 Summary: `tap-exactonline` is a Singer tap for ExactOnline, built with the Meltano SDK for Singer Taps.
 License: Apache 2.0
 Keywords: ELT,ExactOnline
 Author: Hidde Stokvis
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

