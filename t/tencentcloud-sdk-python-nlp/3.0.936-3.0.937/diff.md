# Comparing `tmp/tencentcloud-sdk-python-nlp-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-nlp-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.936.tar", last modified: Mon Jul 17 00:31:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.937.tar", last modified: Tue Jul 18 00:28:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-nlp-3.0.936.tar` & `tencentcloud-sdk-python-nlp-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/nlp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/nlp/v20190408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/nlp/v20190408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49107 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/nlp/v20190408/nlp_client.py
--rw-r--r--   0 root         (0) root         (0)     6090 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/nlp/v20190408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   134541 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/nlp/v20190408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud_sdk_python_nlp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:31:53.000000 tencentcloud-sdk-python-nlp-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49107 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/nlp_client.py
+-rw-r--r--   0 root         (0) root         (0)     6090 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   134539 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:28:08.000000 tencentcloud-sdk-python-nlp-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.936/setup.py` & `tencentcloud-sdk-python-nlp-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/nlp/v20190408/nlp_client.py` & `tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/nlp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/nlp/v20190408/errorcodes.py` & `tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.936/tencentcloud/nlp/v20190408/models.py` & `tencentcloud-sdk-python-nlp-3.0.937/tencentcloud/nlp/v20190408/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3429,15 +3429,15 @@
 class SentenceCorrectionRequest(AbstractModel):
     """SentenceCorrection请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TextList: 待纠错的句子列表。可以以数组方式在一次请求中填写多个待纠错的句子。文本统一使用utf-8格式编码，每个中文句子的长度不超过150字符，每个英文句子的长度不超过100个单词，且数组长度需小于150，即句子总数需少于150句。
+        :param _TextList: 待纠错的句子列表。可以以数组方式在一次请求中填写多个待纠错的句子。文本统一使用utf-8格式编码，每个中文句子的长度不超过150字符，每个英文句子的长度不超过100个单词，且数组长度需小于30，即句子总数需少于30句。
         :type TextList: list of str
         """
         self._TextList = None
 
     @property
     def TextList(self):
         return self._TextList
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.936/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.937/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.937/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.936/README.rst` & `tencentcloud-sdk-python-nlp-3.0.937/README.rst`

 * *Files identical despite different names*

