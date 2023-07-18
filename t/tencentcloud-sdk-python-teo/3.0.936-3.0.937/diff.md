# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.936.tar", last modified: Mon Jul 17 00:37:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.937.tar", last modified: Tue Jul 18 00:32:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.936.tar` & `tencentcloud-sdk-python-teo-3.0.937.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60328 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)    23221 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   605318 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    38737 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:37:02.000000 tencentcloud-sdk-python-teo-3.0.936/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60328 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)    23798 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   605318 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    38737 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:32:34.000000 tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-teo-3.0.936/setup.py` & `tencentcloud-sdk-python-teo-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,17 @@
 
 # 无效的token鉴权参数。
 INVALIDPARAMETER_INVALIDAUTHENTICATIONTYPESIGNPARAM = 'InvalidParameter.InvalidAuthenticationTypeSignParam'
 
 # 无效的token鉴权时间格式。
 INVALIDPARAMETER_INVALIDAUTHENTICATIONTYPETIMEFORMAT = 'InvalidParameter.InvalidAuthenticationTypeTimeFormat'
 
+# 无效的token鉴权时间参数。
+INVALIDPARAMETER_INVALIDAUTHENTICATIONTYPETIMEPARAM = 'InvalidParameter.InvalidAuthenticationTypeTimeParam'
+
 # 无效的第三方对象存储。
 INVALIDPARAMETER_INVALIDAWSPRIVATEACCESS = 'InvalidParameter.InvalidAwsPrivateAccess'
 
 # 无效的备源回源Host。
 INVALIDPARAMETER_INVALIDBACKUPSERVERNAME = 'InvalidParameter.InvalidBackupServerName'
 
 # 无效的节点缓存。
@@ -322,14 +325,17 @@
 
 # 无效的回源Host。
 INVALIDPARAMETER_INVALIDSERVERNAME = 'InvalidParameter.InvalidServerName'
 
 # 无效的客户端ip或ip段。
 INVALIDPARAMETER_INVALIDSTANDARDDEBUGCLIENTIP = 'InvalidParameter.InvalidStandardDebugClientIp'
 
+# 有效期超过限制。
+INVALIDPARAMETER_INVALIDSTANDARDDEBUGEXPIRETIMELIMIT = 'InvalidParameter.InvalidStandardDebugExpireTimeLimit'
+
 # 无效的回源请求参数设置-无效查询字符串值。
 INVALIDPARAMETER_INVALIDUPSTREAMREQUESTQUERYSTRINGVALUE = 'InvalidParameter.InvalidUpstreamRequestQueryStringValue'
 
 # URL重写的目标HOST无效。
 INVALIDPARAMETER_INVALIDURLREDIRECTHOST = 'InvalidParameter.InvalidUrlRedirectHost'
 
 # URL重写的目标URL无效。
@@ -340,14 +346,17 @@
 
 # 无效的缓存键。
 INVALIDPARAMETER_KEYRULESINVALIDQUERYSTRINGVALUE = 'InvalidParameter.KeyRulesInvalidQueryStringValue'
 
 # 参数长度超过限制。
 INVALIDPARAMETER_LENGTHEXCEEDSLIMIT = 'InvalidParameter.LengthExceedsLimit'
 
+# 不支持智能路由
+INVALIDPARAMETER_MULTIPLYLAYERNOTSUPPORTSMARTROUTING = 'InvalidParameter.MultiplyLayerNotSupportSmartRouting'
+
 # 源站是内网IP。
 INVALIDPARAMETER_ORIGINISINNERIP = 'InvalidParameter.OriginIsInnerIp'
 
 # 修改源站操作中源站组Id必填。
 INVALIDPARAMETER_ORIGINORIGINGROUPIDISREQUIRED = 'InvalidParameter.OriginOriginGroupIdIsRequired'
 
 # 参数错误: 无效 "结束时间", 不在允许的查询范围内: [开始时间, 开始+ 7天]
@@ -433,14 +442,17 @@
 
 # 操作被拒绝。
 OPERATIONDENIED = 'OperationDenied'
 
 # 功能内测中，请联系商务开启「中国大陆网络优化(国际加速)」功能。
 OPERATIONDENIED_ACCELERATEMAINLANDDISABLE = 'OperationDenied.AccelerateMainlandDisable'
 
+# 中国大陆加速与IPv6冲突，不能同时配置。
+OPERATIONDENIED_ACCELERATEMAINLANDIPV6CONFLICT = 'OperationDenied.AccelerateMainlandIpv6Conflict'
+
 # 站点停用未完毕，请稍后再试。
 OPERATIONDENIED_DISABLEZONENOTCOMPLETED = 'OperationDenied.DisableZoneNotCompleted'
 
 # 有域名在共享cname组内，不可切换接入类型。
 OPERATIONDENIED_DOMAININSHARECNAMEGROUP = 'OperationDenied.DomainInShareCnameGroup'
 
 # 域名被封禁，暂时无法操作。
```

### Comparing `tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.936/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.937/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.937/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.936/README.rst` & `tencentcloud-sdk-python-teo-3.0.937/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.936/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.936/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.937/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

