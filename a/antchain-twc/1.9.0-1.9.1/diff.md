# Comparing `tmp/antchain_twc-1.9.0.tar.gz` & `tmp/antchain_twc-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_twc-1.9.0.tar", last modified: Wed May 24 03:05:49 2023, max compression
+gzip compressed data, was "dist/antchain_twc-1.9.1.tar", last modified: Mon Jun  5 01:48:17 2023, max compression
```

## Comparing `antchain_twc-1.9.0.tar` & `antchain_twc-1.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/
--rw-r--r--   0 root         (0) root         (0)      213 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2162 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_sdk_twc/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/antchain_sdk_twc/__init__.py
--rw-r--r--   0 root         (0) root         (0)   736938 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/antchain_sdk_twc/client.py
--rw-r--r--   0 root         (0) root         (0)  1932157 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/antchain_sdk_twc/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2162 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:48:17.000000 antchain_twc-1.9.1/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-06-05 01:48:16.000000 antchain_twc-1.9.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-05 01:48:16.000000 antchain_twc-1.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 01:48:16.000000 antchain_twc-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-06-05 01:48:17.000000 antchain_twc-1.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-05 01:48:16.000000 antchain_twc-1.9.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-06-05 01:48:16.000000 antchain_twc-1.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:48:17.000000 antchain_twc-1.9.1/antchain_sdk_twc/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 01:48:16.000000 antchain_twc-1.9.1/antchain_sdk_twc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   736938 2023-06-05 01:48:16.000000 antchain_twc-1.9.1/antchain_sdk_twc/client.py
+-rw-r--r--   0 root         (0) root         (0)  1932029 2023-06-05 01:48:16.000000 antchain_twc-1.9.1/antchain_sdk_twc/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 01:48:17.000000 antchain_twc-1.9.1/antchain_twc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-06-05 01:48:17.000000 antchain_twc-1.9.1/antchain_twc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-05 01:48:17.000000 antchain_twc-1.9.1/antchain_twc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 01:48:17.000000 antchain_twc-1.9.1/antchain_twc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-05 01:48:17.000000 antchain_twc-1.9.1/antchain_twc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-05 01:48:17.000000 antchain_twc-1.9.1/antchain_twc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-05 01:48:17.000000 antchain_twc-1.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-06-05 01:48:16.000000 antchain_twc-1.9.1/setup.py
```

### Comparing `antchain_twc-1.9.0/LICENSE` & `antchain_twc-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_twc-1.9.0/PKG-INFO` & `antchain_twc-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_twc
-Version: 1.9.0
+Version: 1.9.1
 Summary: Ant Chain TWC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_twc-1.9.0/README-CN.md` & `antchain_twc-1.9.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_twc-1.9.0/README.md` & `antchain_twc-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_twc-1.9.0/antchain_sdk_twc/client.py` & `antchain_twc-1.9.1/antchain_sdk_twc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.9.0',
+                    'sdk_version': '1.9.1',
                     '_prod_code': 'TWC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'twc-openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.9.0',
+                    'sdk_version': '1.9.1',
                     '_prod_code': 'TWC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'twc-openapi.antchain.antgroup.com'),
```

### Comparing `antchain_twc-1.9.0/antchain_sdk_twc/models.py` & `antchain_twc-1.9.1/antchain_sdk_twc/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -23280,16 +23280,14 @@
         # 按次使用时需要为整数
         self.usage = usage
         # 用作幂等，防重调用
         self.client_token = client_token
 
     def validate(self):
         self.validate_required(self.order_id, 'order_id')
-        self.validate_required(self.payment_id, 'payment_id')
-        self.validate_required(self.payment_type, 'payment_type')
         self.validate_required(self.usage, 'usage')
         self.validate_required(self.client_token, 'client_token')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `antchain_twc-1.9.0/antchain_twc.egg-info/PKG-INFO` & `antchain_twc-1.9.1/antchain_twc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-twc
-Version: 1.9.0
+Version: 1.9.1
 Summary: Ant Chain TWC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_twc-1.9.0/setup.py` & `antchain_twc-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_twc.
 
-Created on 24/05/2023
+Created on 05/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_twc"
 NAME = "antchain_twc" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain TWC SDK Library for Python"
```

