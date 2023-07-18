# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.936.tar", last modified: Mon Jul 17 00:23:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.937.tar", last modified: Tue Jul 18 00:22:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.936.tar` & `tencentcloud-sdk-python-dlc-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/dlc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82345 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   562352 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/dlc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:23:28.000000 tencentcloud-sdk-python-dlc-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82345 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   562386 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:22:31.000000 tencentcloud-sdk-python-dlc-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.936/setup.py` & `tencentcloud-sdk-python-dlc-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.936/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.937/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/dlc/v20210125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -17153,15 +17153,15 @@
         :type Id: str
         :param _UsedTime: 计算耗时，单位： ms
         :type UsedTime: int
         :param _OutputPath: 任务输出路径。
         :type OutputPath: str
         :param _CreateTime: 任务创建时间。
         :type CreateTime: str
-        :param _State: 任务状态：0 初始化， 1 执行中， 2 执行成功，-1 执行失败，-3 已取消。
+        :param _State: 任务状态：0 初始化， 1 执行中， 2 执行成功，3 数据写入中，4 排队中。-1 执行失败，-3 已取消。
         :type State: int
         :param _SQLType: 任务SQL类型，DDL|DML等
         :type SQLType: str
         :param _SQL: 任务SQL语句
         :type SQL: str
         :param _ResultExpired: 结果是否过期。
         :type ResultExpired: bool
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dlc-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.937/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.936/README.rst` & `tencentcloud-sdk-python-dlc-3.0.937/README.rst`

 * *Files identical despite different names*

