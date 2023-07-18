# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.936.tar", last modified: Mon Jul 17 00:33:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.937.tar", last modified: Tue Jul 18 00:29:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.936.tar` & `tencentcloud-sdk-python-redis-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud_sdk_python_redis.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87353 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   467404 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-17 00:33:06.000000 tencentcloud-sdk-python-redis-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87353 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   467524 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:29:07.000000 tencentcloud-sdk-python-redis-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-redis-3.0.936/setup.py` & `tencentcloud-sdk-python-redis-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.936/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.937/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.936/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/redis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.936/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.936/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.937/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,21 +468,21 @@
 class BackupDownloadInfo(AbstractModel):
     """备份文件下载信息
 
     """
 
     def __init__(self):
         r"""
-        :param _FileName: 备份文件名称
+        :param _FileName: 备份文件名称。
         :type FileName: str
-        :param _FileSize: 备份文件大小，单位B，如果为0，表示无效
+        :param _FileSize: 备份文件大小，单位B，如果为0，表示无效。
         :type FileSize: int
-        :param _DownloadUrl: 备份文件外网下载地址（6小时）
+        :param _DownloadUrl: 备份文件外网下载地址。下载地址的有效时长为6小时，过期后请重新获取。
         :type DownloadUrl: str
-        :param _InnerDownloadUrl: 备份文件内网下载地址（6小时）
+        :param _InnerDownloadUrl: 备份文件内网下载地址。下载地址的有效时长为6小时，过期后请重新获取。
         :type InnerDownloadUrl: str
         """
         self._FileName = None
         self._FileSize = None
         self._DownloadUrl = None
         self._InnerDownloadUrl = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.937/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.936/README.rst` & `tencentcloud-sdk-python-redis-3.0.937/README.rst`

 * *Files identical despite different names*

