# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.936.tar", last modified: Mon Jul 17 00:39:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.937.tar", last modified: Tue Jul 18 00:34:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.936.tar` & `tencentcloud-sdk-python-vod-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud/vod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud/vod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   182739 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25111 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1854207 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:39:30.000000 tencentcloud-sdk-python-vod-3.0.936/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   182739 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25211 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1854207 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:55.000000 tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-vod-3.0.936/setup.py` & `tencentcloud-sdk-python-vod-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.936/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.936/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -616,15 +616,15 @@
 
 # 超过限制值：新旧打点信息个数和超过限制值。
 LIMITEXCEEDED_KEYFRAMEDESCCOUNTREACHMAX = 'LimitExceeded.KeyFrameDescCountReachMax'
 
 # 超过限制值：新旧标签个数和超过限制值。
 LIMITEXCEEDED_TAGCOUNTREACHMAX = 'LimitExceeded.TagCountReachMax'
 
-# 超过限制值：模板数超限。
+# 超过限制值：模板数超过上限 100 个，如需更多请[提交工单](https://console.cloud.tencent.com/workorder/category)。
 LIMITEXCEEDED_TOOMUCHTEMPLATE = 'LimitExceeded.TooMuchTemplate'
 
 # 缺少参数错误。
 MISSINGPARAMETER = 'MissingParameter'
 
 # 请求的次数超过了频率限制。
 REQUESTLIMITEXCEEDED = 'RequestLimitExceeded'
```

### Comparing `tencentcloud-sdk-python-vod-3.0.936/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.937/tencentcloud/vod/v20180717/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.937/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.936'
+__version__ = '3.0.937'
```

### Comparing `tencentcloud-sdk-python-vod-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.937/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.936/README.rst` & `tencentcloud-sdk-python-vod-3.0.937/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.936/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.937/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

