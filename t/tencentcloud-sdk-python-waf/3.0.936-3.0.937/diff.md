# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.936.tar", last modified: Mon Jul 17 00:39:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.937.tar", last modified: Tue Jul 18 00:35:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.936.tar` & `tencentcloud-sdk-python-waf-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3129 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    47458 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)   309127 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/tencentcloud_sdk_python_waf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:39:48.000000 tencentcloud-sdk-python-waf-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    47458 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)   309127 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:25.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:35:24.000000 tencentcloud-sdk-python-waf-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-waf-3.0.936/setup.py` & `tencentcloud-sdk-python-waf-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.936/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
 # 根据ID查询证书失败。
 INVALIDPARAMETER_QUERYCERTBYSSLIDFAILED = 'InvalidParameter.QueryCertBySSLIDFailed'
 
 # 语法错误：逻辑表达式语法解析出错
 INVALIDPARAMETER_QUERYSTRINGSYNTAXERR = 'InvalidParameter.QueryStringSyntaxErr'
 
+# 数据类型错误：SQL检索语句中的数据类型必须与数据库中的数据类型匹配，否则会导致错误。例如，将字符串与整数进行比较、将日期格式不正确等。
+INVALIDPARAMETER_TYPEMISMATCH = 'InvalidParameter.TypeMismatch'
+
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
 
 # SpecificationErr
```

### Comparing `tencentcloud-sdk-python-waf-3.0.936/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/waf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.936/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.937/tencentcloud/waf/v20180125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.937/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.936/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.937/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.936/README.rst` & `tencentcloud-sdk-python-waf-3.0.937/README.rst`

 * *Files identical despite different names*

