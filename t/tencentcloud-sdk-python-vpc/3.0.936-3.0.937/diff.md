# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.936.tar", last modified: Mon Jul 17 00:39:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.937.tar", last modified: Tue Jul 18 00:35:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.936.tar` & `tencentcloud-sdk-python-vpc-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   332400 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42398 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1312049 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:39:38.000000 tencentcloud-sdk-python-vpc-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332400 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42690 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1312049 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:35:01.000000 tencentcloud-sdk-python-vpc-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.936/setup.py` & `tencentcloud-sdk-python-vpc-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
 # 账户余额不足。
 FAILEDOPERATION_BALANCEINSUFFICIENT = 'FailedOperation.BalanceInsufficient'
 
 # 不支持的地域。
 FAILEDOPERATION_INVALIDREGION = 'FailedOperation.InvalidRegion'
 
+# 不支持的IP类型。
+FAILEDOPERATION_IPTYPENOTPERMIT = 'FailedOperation.IpTypeNotPermit'
+
 # 未找到实例的主网卡。
 FAILEDOPERATION_MASTERENINOTFOUND = 'FailedOperation.MasterEniNotFound'
 
 # 网络探测超时，请稍后重试。
 FAILEDOPERATION_NETDETECTTIMEOUT = 'FailedOperation.NetDetectTimeOut'
 
 # 任务执行失败。
@@ -754,14 +757,17 @@
 
 # 该种类型地址不支持此操作。
 UNSUPPORTEDOPERATION_INCORRECTADDRESSRESOURCETYPE = 'UnsupportedOperation.IncorrectAddressResourceType'
 
 # 用户配置的实例和路由表不匹配。
 UNSUPPORTEDOPERATION_INSTANCEANDRTBNOTMATCH = 'UnsupportedOperation.InstanceAndRtbNotMatch'
 
+# 当前云联网`%(value)s`的CdcId与传入实例的CdcId不一致，不支持关联。
+UNSUPPORTEDOPERATION_INSTANCECDCIDNOTMATCHCCNCDCID = 'UnsupportedOperation.InstanceCdcIdNotMatchCcnCdcId'
+
 # 指定实例资源不匹配。
 UNSUPPORTEDOPERATION_INSTANCEMISMATCH = 'UnsupportedOperation.InstanceMismatch'
 
 # 跨账号场景下不支持普通账号实例关联自驾云账号云联网。
 UNSUPPORTEDOPERATION_INSTANCEORDINARYACCOUNTREFUSEATTACH = 'UnsupportedOperation.InstanceOrdinaryAccountRefuseAttach'
 
 # 该地址绑定的实例状态不支持此操作。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/vpc/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.937/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.936/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.937/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.936/README.rst` & `tencentcloud-sdk-python-vpc-3.0.937/README.rst`

 * *Files identical despite different names*

