# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.936.tar", last modified: Mon Jul 17 00:23:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.937.tar", last modified: Tue Jul 18 00:22:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.936.tar` & `tencentcloud-sdk-python-dnspod-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/dnspod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/dnspod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    60713 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23664 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   340184 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-17 00:23:34.000000 tencentcloud-sdk-python-dnspod-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    60713 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24039 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   340184 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:22:38.000000 tencentcloud-sdk-python-dnspod-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.936/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 # 域名已经使用过该类型的礼券了，不能重复使用。
 FAILEDOPERATION_COUPONTYPEALREADYUSED = 'FailedOperation.CouponTypeAlreadyUsed'
 
 # 该域名已在您的列表中，无需重复添加。
 FAILEDOPERATION_DOMAINEXISTS = 'FailedOperation.DomainExists'
 
+# 该域名属于企业邮用户
+FAILEDOPERATION_DOMAININENTERPRISEMAILACCOUNT = 'FailedOperation.DomainInEnterpriseMailAccount'
+
 # 该域名为腾讯云 DNSPod 重点保护资源，为了避免误操作造成的业务影响，域名禁止自行操作删除。如果您确认需要删除域名，请先联系您的客户经理，我们将竭诚为您提供技术支持。
 FAILEDOPERATION_DOMAINISKEYDOMAIN = 'FailedOperation.DomainIsKeyDomain'
 
 # 锁定域名不能进行此操作。
 FAILEDOPERATION_DOMAINISLOCKED = 'FailedOperation.DomainIsLocked'
 
 # 域名已升级为个人套餐，但目前位于企业账号，请与销售联系。
@@ -202,26 +205,32 @@
 
 # 别名编号错误。
 INVALIDPARAMETER_DOMAINALIASIDINVALID = 'InvalidParameter.DomainAliasIdInvalid'
 
 # 域名编号不正确。
 INVALIDPARAMETER_DOMAINIDINVALID = 'InvalidParameter.DomainIdInvalid'
 
+# 该域名涉及违法违规黑名单，无法进行该操作
+INVALIDPARAMETER_DOMAININBLACKLIST = 'InvalidParameter.DomainInBlackList'
+
 # 不允许操作生效中或失效中的域名。
 INVALIDPARAMETER_DOMAININEFFECTORINVALIDATED = 'InvalidParameter.DomainInEffectOrInvalidated'
 
 # 域名不正确，请输入主域名，如 dnspod.cn。
 INVALIDPARAMETER_DOMAININVALID = 'InvalidParameter.DomainInvalid'
 
 # 此域名是其它域名的别名。
 INVALIDPARAMETER_DOMAINISALIASER = 'InvalidParameter.DomainIsAliaser'
 
 # 该域名已有同类型操作未完成，无法执行该操作。
 INVALIDPARAMETER_DOMAINISMODIFYINGDNS = 'InvalidParameter.DomainIsModifyingDns'
 
+# 此域名是自己域名的别名
+INVALIDPARAMETER_DOMAINISMYALIAS = 'InvalidParameter.DomainIsMyAlias'
+
 # 域名没有锁定。
 INVALIDPARAMETER_DOMAINISNOTLOCKED = 'InvalidParameter.DomainIsNotlocked'
 
 # 暂停域名不支持锁定。
 INVALIDPARAMETER_DOMAINNOTALLOWEDLOCK = 'InvalidParameter.DomainNotAllowedLock'
 
 # 处于生效中/失效中的域名，不允许变更解析记录。
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud/dnspod/v20210323/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.937/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.936/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.937/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.936/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.937/README.rst`

 * *Files identical despite different names*

