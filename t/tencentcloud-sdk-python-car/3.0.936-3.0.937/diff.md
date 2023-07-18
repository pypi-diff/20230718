# Comparing `tmp/tencentcloud-sdk-python-car-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-car-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-car-3.0.936.tar", last modified: Mon Jul 17 00:19:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-car-3.0.937.tar", last modified: Tue Jul 18 00:18:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-car-3.0.936.tar` & `tencentcloud-sdk-python-car-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud/car/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud/car/v20220110/
--rw-r--r--   0 root         (0) root         (0)     5256 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud/car/v20220110/car_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud/car/v20220110/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud/car/v20220110/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    13624 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud/car/v20220110/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud/car/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud_sdk_python_car.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud_sdk_python_car.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud_sdk_python_car.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud_sdk_python_car.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:19:16.000000 tencentcloud-sdk-python-car-3.0.936/tencentcloud_sdk_python_car.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud/car/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud/car/v20220110/
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud/car/v20220110/car_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud/car/v20220110/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud/car/v20220110/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    13624 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud/car/v20220110/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud/car/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud_sdk_python_car.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud_sdk_python_car.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud_sdk_python_car.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud_sdk_python_car.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:18:51.000000 tencentcloud-sdk-python-car-3.0.937/tencentcloud_sdk_python_car.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-car-3.0.936/setup.py` & `tencentcloud-sdk-python-car-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.936/tencentcloud/car/v20220110/car_client.py` & `tencentcloud-sdk-python-car-3.0.937/tencentcloud/car/v20220110/car_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.936/tencentcloud/car/v20220110/errorcodes.py` & `tencentcloud-sdk-python-car-3.0.937/tencentcloud/car/v20220110/errorcodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 # Json 解析失败。
 INVALIDPARAMETER_JSONPARSEERROR = 'InvalidParameter.JsonParseError'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
+# 【多人互动】对应的角色人数超过限制。
+LIMITEXCEEDED_ROLE = 'LimitExceeded.Role'
+
 # 操作被拒绝。
 OPERATIONDENIED = 'OperationDenied'
 
 # 没有空闲并发。
 RESOURCENOTFOUND_NOIDLE = 'ResourceNotFound.NoIdle'
 
 # 未找到会话。
```

### Comparing `tencentcloud-sdk-python-car-3.0.936/tencentcloud/car/v20220110/models.py` & `tencentcloud-sdk-python-car-3.0.937/tencentcloud/car/v20220110/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-car-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-car-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-car-3.0.937/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-car
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Car SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-car-3.0.936/README.rst` & `tencentcloud-sdk-python-car-3.0.937/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-car-3.0.936/tencentcloud_sdk_python_car.egg-info/PKG-INFO` & `tencentcloud-sdk-python-car-3.0.937/tencentcloud_sdk_python_car.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-car
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Car SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

