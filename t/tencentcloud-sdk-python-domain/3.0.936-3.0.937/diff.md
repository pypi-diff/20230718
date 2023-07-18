# Comparing `tmp/tencentcloud-sdk-python-domain-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-domain-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.936.tar", last modified: Mon Jul 17 00:23:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.937.tar", last modified: Tue Jul 18 00:22:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-domain-3.0.936.tar` & `tencentcloud-sdk-python-domain-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud/domain/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud/domain/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8787 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud/domain/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25103 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud/domain/v20180808/domain_client.py
--rw-r--r--   0 root         (0) root         (0)   121267 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud/domain/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud_sdk_python_domain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/tencentcloud_sdk_python_domain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-17 00:23:39.000000 tencentcloud-sdk-python-domain-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8787 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25103 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/domain_client.py
+-rw-r--r--   0 root         (0) root         (0)   121377 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:22:45.000000 tencentcloud-sdk-python-domain-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-domain-3.0.936/setup.py` & `tencentcloud-sdk-python-domain-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-domain-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-domain-3.0.936/tencentcloud/domain/v20180808/errorcodes.py` & `tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.936/tencentcloud/domain/v20180808/domain_client.py` & `tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/domain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.936/tencentcloud/domain/v20180808/models.py` & `tencentcloud-sdk-python-domain-3.0.937/tencentcloud/domain/v20180808/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2847,14 +2847,16 @@
 pendingDelete：删除期
 serverTransferProhibited：注册局禁止转移
 serverUpdateProhibited：注册局禁止更新
 serverDeleteProhibited：注册局禁止删除
 clientTransferProhibited：注册商禁止转移
 clientUpdateProhibited：注册商禁止更新
 clientDeleteProhibited：注册商禁止删除
+serverRenewProhibited: 注册局禁止续费
+clientRenewProhobited: 注册商禁止续费
         :type DomainStatus: list of str
         :param _BuyStatus: 域名购买状态。
 ok：正常
 RegisterPending：待注册
 RegisterDoing：注册中
 RegisterFailed：注册失败
 AboutToExpire: 即将过期
@@ -3661,15 +3663,15 @@
 class SetDomainAutoRenewRequest(AbstractModel):
     """SetDomainAutoRenew请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _DomainId: 域名ID。
+        :param _DomainId: 域名ID 例如：domain-123abc
         :type DomainId: str
         :param _AutoRenew: AutoRenew 有三个可选值：
  0：不设置自动续费
 1：设置自动续费
 2：设置到期后不续费
         :type AutoRenew: int
         """
```

### Comparing `tencentcloud-sdk-python-domain-3.0.936/tencentcloud_sdk_python_domain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.937/tencentcloud_sdk_python_domain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.937/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.936/README.rst` & `tencentcloud-sdk-python-domain-3.0.937/README.rst`

 * *Files identical despite different names*

