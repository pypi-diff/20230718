# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.936.tar", last modified: Mon Jul 17 00:19:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.937.tar", last modified: Tue Jul 18 00:19:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.936.tar` & `tencentcloud-sdk-python-cdn-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/cdn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82139 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)    22160 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   854012 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/cdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:19:59.000000 tencentcloud-sdk-python-cdn-3.0.936/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82139 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)    22160 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   854003 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:19:25.000000 tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.936/setup.py` & `tencentcloud-sdk-python-cdn-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,15 +523,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDistrictIspData(self, request):
         """查询指定域名的区域、运营商明细数据
-        注意事项：接口尚未全量开放，未在内测名单中的账号不支持调用
+        注意事项：接口尚未全面开放，未在内测名单中的账号不支持调用
 
         :param request: Request instance for DescribeDistrictIspData.
         :type request: :class:`tencentcloud.cdn.v20180606.models.DescribeDistrictIspDataRequest`
         :rtype: :class:`tencentcloud.cdn.v20180606.models.DescribeDistrictIspDataResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -19001,15 +19001,15 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class MainlandConfig(AbstractModel):
-    """域名国内地区特殊配置。分地区特殊配置。UpdateDomainConfig接口只支持修改部分分地区配置，为了兼容旧版本配置，本类型会列出旧版本所有可能存在差异的配置列表，支持修改的配置列表如下：
+    """域名国内地区特殊配置。分地区特殊配置。UpdateDomainConfig接口只支持修改部分地区配置，为了兼容旧版本配置，本类型会列出旧版本所有可能存在差异的配置列表，支持修改的配置列表如下：
     + Authentication
     + BandwidthAlert
     + ErrorPage
     + IpFilter
     + Origin
     + Referer
 
@@ -20747,15 +20747,15 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class OverseaConfig(AbstractModel):
-    """域名海外地区特殊配置。UpdateDomainConfig接口只支持修改部分分地区配置，为了兼容旧版本配置，本类型会列出旧版本所有可能存在差异的配置列表，支持修改的配置列表如下：
+    """域名海外地区特殊配置。UpdateDomainConfig接口只支持修改部分地区配置，为了兼容旧版本配置，本类型会列出旧版本所有可能存在差异的配置列表，支持修改的配置列表如下：
     + Authentication
     + BandwidthAlert
     + ErrorPage
     + IpFilter
     + Origin
     + Referer
 
@@ -22533,15 +22533,15 @@
 directory 时填充路径，如 /xxx/test/
 path 时填充绝对路径，如 /xxx/test.html
         :type RulePaths: list of str
         :param _RefererType: referer 配置类型
 whitelist：白名单
 blacklist：黑名单
         :type RefererType: str
-        :param _Referers: referer 内容列表列表
+        :param _Referers: referer 内容列表
         :type Referers: list of str
         :param _AllowEmpty: 是否允许空 referer
 防盗链类型为白名单时，true表示允许空 referer，false表示不允许空 referer；
 防盗链类型为黑名单时，true表示拒绝空referer，false表示不拒绝空referer；
         :type AllowEmpty: bool
         """
         self._RuleType = None
@@ -28783,15 +28783,15 @@
         :type RealUrl: str
         :param _DownloadUrl: 快照路径，用于控制台展示违规内容快照
         :type DownloadUrl: str
         :param _UrlStatus: 违规资源当前状态
 forbid：已封禁
 release：已解封
 delay ： 延迟处理
-reject ：申诉驳回，状态仍为封禁态
+reject ：申诉驳回，状态仍为封禁状态
 complain：申诉进行中
         :type UrlStatus: str
         :param _CreateTime: 创建时间
         :type CreateTime: str
         :param _UpdateTime: 更新时间
         :type UpdateTime: str
         """
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.937/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.936/README.rst` & `tencentcloud-sdk-python-cdn-3.0.937/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.936/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.937/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

