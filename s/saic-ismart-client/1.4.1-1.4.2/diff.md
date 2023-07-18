# Comparing `tmp/saic_ismart_client-1.4.1.tar.gz` & `tmp/saic_ismart_client-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.4.1.tar", last modified: Sun Jul  9 13:43:24 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.4.2.tar", last modified: Tue Jul 18 08:21:43 2023, max compression
```

## Comparing `saic_ismart_client-1.4.1.tar` & `saic_ismart_client-1.4.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.787799 saic_ismart_client-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.787799 saic_ismart_client-1.4.1/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.787799 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.787799 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23240 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.787799 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-09 13:43:24.000000 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-09 13:43:24.000000 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:43:24.000000 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-09 13:43:24.000000 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-09 13:43:24.000000 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/common_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23536 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45272 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.917804 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 08:21:43.000000 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-18 08:21:43.000000 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:21:43.000000 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 08:21:43.000000 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 08:21:43.000000 saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:21:43.921804 saic_ismart_client-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-18 08:21:32.000000 saic_ismart_client-1.4.2/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.4.1/LICENSE` & `saic_ismart_client-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/PKG-INFO` & `saic_ismart_client-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.4.1
+Version: 1.4.2
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.1/README.md` & `saic_ismart_client-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/pyproject.toml` & `saic_ismart_client-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.165.0",
     "requests >= 2.28.2",
     "urllib3 >= 1.26.14",
```

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.4.2/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.4.2/src/saic_ismart_client/common_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.4.2/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from saic_ismart_client.common_model import ApplicationData, Asn1Type
+from saic_ismart_client.saic_api import TargetBatteryCode
 
 
 class OtaChrgMangDataResp(ApplicationData):
     def __init__(self):
         super().__init__('OTAChrgMangDataResp')
         self.bmsReserCtrlDspCmd = None  # INTEGER(0..255),
         self.bmsReserStHourDspCmd = None  # INTEGER(0..255),
@@ -153,14 +154,21 @@
 
     def get_voltage(self) -> float:
         return self.bmsPackVol * 0.25
 
     def get_power(self) -> float:
         return self.get_current() * self.get_voltage() / 1000.0
 
+    def get_charge_target_soc(self) -> TargetBatteryCode | None:
+        raw_target_soc = self.bmsOnBdChrgTrgtSOCDspCmd
+        try:
+            return TargetBatteryCode(raw_target_soc)
+        except ValueError:
+            return None
+
 
 class RvsChargingStatus(Asn1Type):
     def __init__(self):
         super().__init__('RvsChargingStatus')
         self.real_time_power = None  # INTEGER(0..65535),
         self.charging_gun_state = None  # BOOLEAN,
         self.fuel_Range_elec = None  # INTEGER(0..65535),
```

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.4.2/src/saic_ismart_client/saic_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,53 @@
     P_50 = 2
     P_60 = 3
     P_70 = 4
     P_80 = 5
     P_90 = 6
     P_100 = 7
 
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
+
 
 class SaicMessage:
     def __init__(self, message_id: int, message_type: str, title: str, message_time: datetime, sender: str,
                  content: str, read_status: int, vin: str):
         self.message_id = message_id
         self.message_type = message_type
         self.title = title
```

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.4.1
+Version: 1.4.2
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.4.2/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/tests/test_Message_v1_1.py` & `saic_ismart_client-1.4.2/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/tests/test_Message_v2_1.py` & `saic_ismart_client-1.4.2/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/tests/test_Message_v3_0.py` & `saic_ismart_client-1.4.2/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/tests/test_abrp_api.py` & `saic_ismart_client-1.4.2/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.1/tests/test_saic_api.py` & `saic_ismart_client-1.4.2/tests/test_saic_api.py`

 * *Files identical despite different names*

