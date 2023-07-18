# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.936.tar", last modified: Mon Jul 17 00:32:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.937.tar", last modified: Tue Jul 18 00:28:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.936.tar` & `tencentcloud-sdk-python-postgres-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/postgres/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20749 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    85776 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)   446339 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-17 00:32:41.000000 tencentcloud-sdk-python-postgres-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20749 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    85776 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)   446339 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-18 00:28:45.000000 tencentcloud-sdk-python-postgres-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.936/setup.py` & `tencentcloud-sdk-python-postgres-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.936/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.937/tencentcloud/postgres/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.936/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.937/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.937/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.936/README.rst` & `tencentcloud-sdk-python-postgres-3.0.937/README.rst`

 * *Files identical despite different names*
