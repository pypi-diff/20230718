# Comparing `tmp/alibabacloud_xrengine20230313-1.0.0.tar.gz` & `tmp/alibabacloud_xrengine20230313-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_xrengine20230313-1.0.0.tar", last modified: Mon Jul 17 11:31:51 2023, max compression
+gzip compressed data, was "dist/alibabacloud_xrengine20230313-1.0.1.tar", last modified: Tue Jul 18 07:01:06 2023, max compression
```

## Comparing `alibabacloud_xrengine20230313-1.0.0.tar` & `alibabacloud_xrengine20230313-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48489 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313/client.py
--rw-r--r--   0 root         (0) root         (0)   166652 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      447 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2023-07-17 11:31:51.000000 alibabacloud_xrengine20230313-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51357 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/client.py
+-rw-r--r--   0 root         (0) root         (0)   170675 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-07-18 07:01:06.000000 alibabacloud_xrengine20230313-1.0.1/setup.py
```

### Comparing `alibabacloud_xrengine20230313-1.0.0/LICENSE` & `alibabacloud_xrengine20230313-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-1.0.0/PKG-INFO` & `alibabacloud_xrengine20230313-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_xrengine20230313
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-1.0.0/README-CN.md` & `alibabacloud_xrengine20230313-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-1.0.0/README.md` & `alibabacloud_xrengine20230313-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313/client.py` & `alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1186,7 +1186,81 @@
 
     async def pop_object_project_detail_async(
         self,
         request: xr_engine_20230313_models.PopObjectProjectDetailRequest,
     ) -> xr_engine_20230313_models.PopObjectProjectDetailResponse:
         runtime = util_models.RuntimeOptions()
         return await self.pop_object_project_detail_with_options_async(request, runtime)
+
+    def pop_video_save_source_with_options(
+        self,
+        request: xr_engine_20230313_models.PopVideoSaveSourceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopVideoSaveSourceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.project_id):
+            query['ProjectId'] = request.project_id
+        if not UtilClient.is_unset(request.source_type):
+            query['SourceType'] = request.source_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='PopVideoSaveSource',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopVideoSaveSourceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def pop_video_save_source_with_options_async(
+        self,
+        request: xr_engine_20230313_models.PopVideoSaveSourceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopVideoSaveSourceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.project_id):
+            query['ProjectId'] = request.project_id
+        if not UtilClient.is_unset(request.source_type):
+            query['SourceType'] = request.source_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='PopVideoSaveSource',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopVideoSaveSourceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def pop_video_save_source(
+        self,
+        request: xr_engine_20230313_models.PopVideoSaveSourceRequest,
+    ) -> xr_engine_20230313_models.PopVideoSaveSourceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.pop_video_save_source_with_options(request, runtime)
+
+    async def pop_video_save_source_async(
+        self,
+        request: xr_engine_20230313_models.PopVideoSaveSourceRequest,
+    ) -> xr_engine_20230313_models.PopVideoSaveSourceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.pop_video_save_source_with_options_async(request, runtime)
```

### Comparing `alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313/models.py` & `alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4981,7 +4981,141 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PopObjectProjectDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PopVideoSaveSourceRequest(TeaModel):
+    def __init__(
+        self,
+        project_id: str = None,
+        source_type: str = None,
+    ):
+        self.project_id = project_id
+        self.source_type = source_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.project_id is not None:
+            result['ProjectId'] = self.project_id
+        if self.source_type is not None:
+            result['SourceType'] = self.source_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ProjectId') is not None:
+            self.project_id = m.get('ProjectId')
+        if m.get('SourceType') is not None:
+            self.source_type = m.get('SourceType')
+        return self
+
+
+class PopVideoSaveSourceResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        error_name: str = None,
+        http_code: int = None,
+        message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.error_name = error_name
+        self.http_code = http_code
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.error_name is not None:
+            result['ErrorName'] = self.error_name
+        if self.http_code is not None:
+            result['HttpCode'] = self.http_code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('ErrorName') is not None:
+            self.error_name = m.get('ErrorName')
+        if m.get('HttpCode') is not None:
+            self.http_code = m.get('HttpCode')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class PopVideoSaveSourceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PopVideoSaveSourceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = PopVideoSaveSourceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_xrengine20230313-1.0.0/alibabacloud_xrengine20230313.egg-info/PKG-INFO` & `alibabacloud_xrengine20230313-1.0.1/alibabacloud_xrengine20230313.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-xrengine20230313
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-1.0.0/setup.py` & `alibabacloud_xrengine20230313-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_xrengine20230313.
 
-Created on 17/07/2023
+Created on 18/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_xrengine20230313"
 NAME = "alibabacloud_xrengine20230313" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud xrEngine (20230313) SDK Library for Python"
```

