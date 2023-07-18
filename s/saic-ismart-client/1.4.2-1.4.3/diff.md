# Comparing `tmp/saic_ismart_client-1.4.2.tar.gz` & `tmp/saic_ismart_client-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.4.2.tar", last modified: Tue Jul 18 08:21:43 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.4.3.tar", last modified: Tue Jul 18 18:02:11 2023, max compression
```

## Comparing `saic_ismart_client-1.4.2.tar` & `saic_ismart_client-1.4.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23536 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    45272 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 08:21:43.000000 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-18 08:21:43.000000 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:21:43.000000 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 08:21:43.000000 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 08:21:43.000000 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.937383 saic_ismart_client-1.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.941383 saic_ismart_client-1.4.3/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.937383 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.941383 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.941383 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.941383 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/common_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23497 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44179 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.941383 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 18:02:11.000000 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-18 18:02:11.000000 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:02:11.000000 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 18:02:11.000000 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 18:02:11.000000 saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:02:11.945383 saic_ismart_client-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-18 18:01:59.000000 saic_ismart_client-1.4.3/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.4.2/LICENSE` & `saic_ismart_client-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/PKG-INFO` & `saic_ismart_client-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.4.2
+Version: 1.4.3
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.2/README.md` & `saic_ismart_client-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/pyproject.toml` & `saic_ismart_client-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.4.2"
+version = "1.4.3"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.165.0",
     "requests >= 2.28.2",
     "urllib3 >= 1.26.14",
```

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.4.3/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.4.3/src/saic_ismart_client/common_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,7 +518,56 @@
 
     def init_from_dict(self, data: dict):
         self.mcc_network = data.get(FIELD_MCC_NETWORK)
         self.mnc_network = data.get(FIELD_MNC_NETWORK)
         self.mcc_sim = data.get(FIELD_MCC_SIM)
         self.mnc_sim = data.get(FIELD_MNC_SIM)
         self.signal_strength = data.get(FIELD_SIGNAL_STRENGTH)
+
+
+class TargetBatteryCode(Enum):
+    P_40 = 1
+    P_50 = 2
+    P_60 = 3
+    P_70 = 4
+    P_80 = 5
+    P_90 = 6
+    P_100 = 7
+
+    def get_percentage(self) -> int:
+        match self:
+            case TargetBatteryCode.P_40:
+                return 40
+            case TargetBatteryCode.P_50:
+                return 50
+            case TargetBatteryCode.P_60:
+                return 60
+            case TargetBatteryCode.P_70:
+                return 70
+            case TargetBatteryCode.P_80:
+                return 80
+            case TargetBatteryCode.P_90:
+                return 90
+            case TargetBatteryCode.P_100:
+                return 100
+            case _:
+                raise ValueError(f'Unknown target battery code: {self}')
+
+    @staticmethod
+    def from_percentage(percentage: int):
+        match percentage:
+            case 40:
+                return TargetBatteryCode.P_40
+            case 50:
+                return TargetBatteryCode.P_50
+            case 60:
+                return TargetBatteryCode.P_60
+            case 70:
+                return TargetBatteryCode.P_70
+            case 80:
+                return TargetBatteryCode.P_80
+            case 90:
+                return TargetBatteryCode.P_90
+            case 100:
+                return TargetBatteryCode.P_100
+            case _:  # default
+                raise ValueError(f'Unknown target battery percentage: {percentage}')
```

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.4.3/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from saic_ismart_client.common_model import ApplicationData, Asn1Type
-from saic_ismart_client.saic_api import TargetBatteryCode
+from saic_ismart_client.common_model import ApplicationData, Asn1Type, TargetBatteryCode
 
 
 class OtaChrgMangDataResp(ApplicationData):
     def __init__(self):
         super().__init__('OTAChrgMangDataResp')
         self.bmsReserCtrlDspCmd = None  # INTEGER(0..255),
         self.bmsReserStHourDspCmd = None  # INTEGER(0..255),
```

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.4.3/src/saic_ismart_client/saic_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import time
 import urllib.parse
 from enum import Enum
 from typing import cast
 
 import requests as requests
 
-from saic_ismart_client.common_model import AbstractMessage, AbstractMessageBody, Header, MessageBodyV2, MessageV2
+from saic_ismart_client.common_model import AbstractMessage, AbstractMessageBody, Header, MessageBodyV2, MessageV2, \
+    TargetBatteryCode
 from saic_ismart_client.ota_v1_1.Message import MessageCoderV11
 from saic_ismart_client.ota_v1_1.data_model import AbortSendMessageReq, AlarmSwitch, AlarmSwitchReq, Message, \
     MessageBodyV11, MessageListReq, MessageListResp, MessageV11, MpAlarmSettingType, MpUserLoggingInReq, \
     MpUserLoggingInRsp, StartEndNumber, Timestamp, VinInfo
 from saic_ismart_client.ota_v2_1.Message import MessageCoderV21
 from saic_ismart_client.ota_v2_1.data_model import OtaRvcReq, OtaRvcStatus25857, OtaRvmVehicleStatusReq, \
     OtaRvmVehicleStatusResp25857, RvcReqParam
@@ -27,63 +28,14 @@
 
 class ScheduledChargingMode(Enum):
     DISABLED = 2
     UNTIL_CONFIGURED_SOC = 3
     UNTIL_CONFIGURED_TIME = 1
 
 
-class TargetBatteryCode(Enum):
-    P_40 = 1
-    P_50 = 2
-    P_60 = 3
-    P_70 = 4
-    P_80 = 5
-    P_90 = 6
-    P_100 = 7
-
-    def get_percentage(self) -> int:
-        match self:
-            case TargetBatteryCode.P_40:
-                return 40
-            case TargetBatteryCode.P_50:
-                return 50
-            case TargetBatteryCode.P_60:
-                return 60
-            case TargetBatteryCode.P_70:
-                return 70
-            case TargetBatteryCode.P_80:
-                return 80
-            case TargetBatteryCode.P_90:
-                return 90
-            case TargetBatteryCode.P_100:
-                return 100
-            case _:
-                raise ValueError(f'Unknown target battery code: {self}')
-
-    @staticmethod
-    def from_percentage(percentage: int):
-        match percentage:
-            case 40:
-                return TargetBatteryCode.P_40
-            case 50:
-                return TargetBatteryCode.P_50
-            case 60:
-                return TargetBatteryCode.P_60
-            case 70:
-                return TargetBatteryCode.P_70
-            case 80:
-                return TargetBatteryCode.P_80
-            case 90:
-                return TargetBatteryCode.P_90
-            case 100:
-                return TargetBatteryCode.P_100
-            case _:  # default
-                raise ValueError(f'Unknown target battery percentage: {percentage}')
-
-
 class SaicMessage:
     def __init__(self, message_id: int, message_type: str, title: str, message_time: datetime, sender: str,
                  content: str, read_status: int, vin: str):
         self.message_id = message_id
         self.message_type = message_type
         self.title = title
         self.message_time = message_time
@@ -675,15 +627,15 @@
                                                   urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv30'))
         self.publish_raw_response(application_id, application_data_protocol_version, chrg_ctrl_rsp_msg_hex)
         chrg_ctrl_rsp_msg = MessageV30(MessageBodyV30(), OtaChrgCtrlStsResp())
         self.message_V3_0_coder.decode_response(chrg_ctrl_rsp_msg_hex, chrg_ctrl_rsp_msg)
         self.publish_json_response(application_id, application_data_protocol_version, chrg_ctrl_rsp_msg.get_data())
         return chrg_ctrl_rsp_msg
 
-    def control_charging(self, stop_charging: bool, vin_info: VinInfo, event_id: str = None):
+    def control_charging(self, stop_charging: bool, vin_info: VinInfo, event_id: str = None) -> MessageV30:
         chrg_ctrl_req = OtaChrgCtrlReq()
         chrg_ctrl_req.chrgCtrlReq = 2 if stop_charging else 1
         chrg_ctrl_req.tboxV2XReq = 0
         chrg_ctrl_req.tboxEleccLckCtrlReq = 0
         chrg_ctrl_req_msg = MessageV30(MessageBodyV30(), chrg_ctrl_req)
         application_id = '516'
         application_data_protocol_version = 768
@@ -698,14 +650,20 @@
                                                   urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv30'))
         self.publish_raw_response(application_id, application_data_protocol_version, chrg_ctrl_rsp_msg_hex)
         chrg_ctrl_rsp_msg = MessageV30(MessageBodyV30(), OtaChrgCtrlStsResp())
         self.message_V3_0_coder.decode_response(chrg_ctrl_rsp_msg_hex, chrg_ctrl_rsp_msg)
         self.publish_json_response(application_id, application_data_protocol_version, chrg_ctrl_rsp_msg.get_data())
         return chrg_ctrl_rsp_msg
 
+    def start_charging(self, vin_info: VinInfo, event_id: str = None) -> MessageV30:
+        return self.control_charging(False, vin_info, event_id)
+
+    def start_charging_with_retry(self, vin_info: VinInfo) -> MessageV30:
+        return self.handle_retry(self.start_charging, vin_info)
+
     def set_target_battery_soc(self, target_soc: TargetBatteryCode, vin_info: VinInfo, event_id: str = None):
         chrg_setng_req = OtaChrgSetngReq()
         chrg_setng_req.onBdChrgTrgtSOCReq = target_soc.value
         chrg_setng_req.altngChrgCrntReq = 4
         chrg_setng_req.tboxV2XSpSOCReq = 0
         chrg_setng_req_msg = MessageV30(MessageBodyV30(), chrg_setng_req)
         application_id = '516'
```

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.4.2
+Version: 1.4.3
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.4.3/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/tests/test_Message_v1_1.py` & `saic_ismart_client-1.4.3/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/tests/test_Message_v2_1.py` & `saic_ismart_client-1.4.3/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/tests/test_Message_v3_0.py` & `saic_ismart_client-1.4.3/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/tests/test_abrp_api.py` & `saic_ismart_client-1.4.3/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.2/tests/test_saic_api.py` & `saic_ismart_client-1.4.3/tests/test_saic_api.py`

 * *Files identical despite different names*

