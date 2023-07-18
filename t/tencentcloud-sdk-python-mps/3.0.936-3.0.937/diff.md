# Comparing `tmp/tencentcloud-sdk-python-mps-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-mps-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.936.tar", last modified: Mon Jul 17 00:31:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.937.tar", last modified: Tue Jul 18 00:27:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mps-3.0.936.tar` & `tencentcloud-sdk-python-mps-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud/mps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99031 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)    13373 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud/mps/v20190612/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1229741 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud/mps/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud_sdk_python_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:31:27.000000 tencentcloud-sdk-python-mps-3.0.936/tencentcloud_sdk_python_mps.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99031 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1229741 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:27:39.000000 tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-mps-3.0.936/setup.py` & `tencentcloud-sdk-python-mps-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mps-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mps-3.0.936/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/mps_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.936/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,17 @@
 
 # 参数错误：Definitions。
 INVALIDPARAMETERVALUE_DEFINITIONS = 'InvalidParameterValue.Definitions'
 
 # 参数值错误：不允许删除默认模板。
 INVALIDPARAMETERVALUE_DELETEDEFAULTTEMPLATE = 'InvalidParameterValue.DeleteDefaultTemplate'
 
+# DestinationLanguage参数错误
+INVALIDPARAMETERVALUE_DESTINATIONLANGUAGE = 'InvalidParameterValue.DestinationLanguage'
+
 # 无效的禁止码率低转高开关值。
 INVALIDPARAMETERVALUE_DISABLEHIGHERVIDEOBITRATE = 'InvalidParameterValue.DisableHigherVideoBitrate'
 
 # 无效的禁止分辨率低转高开关值。
 INVALIDPARAMETERVALUE_DISABLEHIGHERVIDEORESOLUTION = 'InvalidParameterValue.DisableHigherVideoResolution'
 
 # 参数值错误：人脸重复。
@@ -286,14 +289,17 @@
 
 # SessionId 过长。
 INVALIDPARAMETERVALUE_SESSIONIDTOOLONG = 'InvalidParameterValue.SessionIdTooLong'
 
 # 参数错误：音频通道方式。
 INVALIDPARAMETERVALUE_SOUNDSYSTEM = 'InvalidParameterValue.SoundSystem'
 
+# SourceLanguage参数错误
+INVALIDPARAMETERVALUE_SOURCELANGUAGE = 'InvalidParameterValue.SourceLanguage'
+
 # 源文件错误。
 INVALIDPARAMETERVALUE_SRCFILE = 'InvalidParameterValue.SrcFile'
 
 # 参数值错误：SubtitleFormat 参数非法。
 INVALIDPARAMETERVALUE_SUBTITLEFORMAT = 'InvalidParameterValue.SubtitleFormat'
 
 # 参数值错误：SVG 为空。
```

### Comparing `tencentcloud-sdk-python-mps-3.0.936/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-mps-3.0.937/tencentcloud/mps/v20190612/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.937/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.936/README.rst` & `tencentcloud-sdk-python-mps-3.0.937/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.936/tencentcloud_sdk_python_mps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.937/tencentcloud_sdk_python_mps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

