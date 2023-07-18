# Comparing `tmp/tencentcloud-sdk-python-apm-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-apm-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apm-3.0.936.tar", last modified: Mon Jul 17 00:17:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apm-3.0.937.tar", last modified: Tue Jul 18 00:17:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apm-3.0.936.tar` & `tencentcloud-sdk-python-apm-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud/apm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud/apm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud/apm/v20210622/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud/apm/v20210622/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8295 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud/apm/v20210622/apm_client.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud/apm/v20210622/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    69138 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud/apm/v20210622/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud_sdk_python_apm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud_sdk_python_apm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud_sdk_python_apm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud_sdk_python_apm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/tencentcloud_sdk_python_apm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:17:14.000000 tencentcloud-sdk-python-apm-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8295 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/apm_client.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    70014 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:17:03.000000 tencentcloud-sdk-python-apm-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-apm-3.0.936/setup.py` & `tencentcloud-sdk-python-apm-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.936/tencentcloud/apm/v20210622/apm_client.py` & `tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/apm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.936/tencentcloud/apm/v20210622/errorcodes.py` & `tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.936/tencentcloud/apm/v20210622/models.py` & `tencentcloud-sdk-python-apm-3.0.937/tencentcloud/apm/v20210622/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,14 +398,17 @@
         :type TotalCount: int
         :param _LogSet: CLS日志集 | ES集群ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type LogSet: str
         :param _MetricDuration: Metric数据保存时长
 注意：此字段可能返回 null，表示取不到有效值。
         :type MetricDuration: int
+        :param _CustomShowTags: 用户自定义展示标签列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CustomShowTags: list of str
         """
         self._AmountOfUsedStorage = None
         self._Name = None
         self._Tags = None
         self._InstanceId = None
         self._CreateUin = None
         self._ServiceCount = None
@@ -425,14 +428,15 @@
         self._LogSource = None
         self._IsRelatedLog = None
         self._LogTopicID = None
         self._ClientCount = None
         self._TotalCount = None
         self._LogSet = None
         self._MetricDuration = None
+        self._CustomShowTags = None
 
     @property
     def AmountOfUsedStorage(self):
         return self._AmountOfUsedStorage
 
     @AmountOfUsedStorage.setter
     def AmountOfUsedStorage(self, AmountOfUsedStorage):
@@ -634,14 +638,22 @@
     def MetricDuration(self):
         return self._MetricDuration
 
     @MetricDuration.setter
     def MetricDuration(self, MetricDuration):
         self._MetricDuration = MetricDuration
 
+    @property
+    def CustomShowTags(self):
+        return self._CustomShowTags
+
+    @CustomShowTags.setter
+    def CustomShowTags(self, CustomShowTags):
+        self._CustomShowTags = CustomShowTags
+
 
     def _deserialize(self, params):
         self._AmountOfUsedStorage = params.get("AmountOfUsedStorage")
         self._Name = params.get("Name")
         if params.get("Tags") is not None:
             self._Tags = []
             for item in params.get("Tags"):
@@ -667,14 +679,15 @@
         self._LogSource = params.get("LogSource")
         self._IsRelatedLog = params.get("IsRelatedLog")
         self._LogTopicID = params.get("LogTopicID")
         self._ClientCount = params.get("ClientCount")
         self._TotalCount = params.get("TotalCount")
         self._LogSet = params.get("LogSet")
         self._MetricDuration = params.get("MetricDuration")
+        self._CustomShowTags = params.get("CustomShowTags")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2023,14 +2036,16 @@
         :type LogRegion: str
         :param _LogTopicID: CLS日志主题ID | ES 索引名
         :type LogTopicID: str
         :param _LogSet: CLS日志集 | ES集群ID
         :type LogSet: str
         :param _LogSource: CLS | ES
         :type LogSource: str
+        :param _CustomShowTags: 用户自定义展示标签列表
+        :type CustomShowTags: list of str
         """
         self._InstanceId = None
         self._Name = None
         self._Tags = None
         self._Description = None
         self._TraceDuration = None
         self._OpenBilling = None
@@ -2040,14 +2055,15 @@
         self._ErrorSample = None
         self._SlowRequestSavedThreshold = None
         self._IsRelatedLog = None
         self._LogRegion = None
         self._LogTopicID = None
         self._LogSet = None
         self._LogSource = None
+        self._CustomShowTags = None
 
     @property
     def InstanceId(self):
         return self._InstanceId
 
     @InstanceId.setter
     def InstanceId(self, InstanceId):
@@ -2169,14 +2185,22 @@
     def LogSource(self):
         return self._LogSource
 
     @LogSource.setter
     def LogSource(self, LogSource):
         self._LogSource = LogSource
 
+    @property
+    def CustomShowTags(self):
+        return self._CustomShowTags
+
+    @CustomShowTags.setter
+    def CustomShowTags(self, CustomShowTags):
+        self._CustomShowTags = CustomShowTags
+
 
     def _deserialize(self, params):
         self._InstanceId = params.get("InstanceId")
         self._Name = params.get("Name")
         if params.get("Tags") is not None:
             self._Tags = []
             for item in params.get("Tags"):
@@ -2192,14 +2216,15 @@
         self._ErrorSample = params.get("ErrorSample")
         self._SlowRequestSavedThreshold = params.get("SlowRequestSavedThreshold")
         self._IsRelatedLog = params.get("IsRelatedLog")
         self._LogRegion = params.get("LogRegion")
         self._LogTopicID = params.get("LogTopicID")
         self._LogSet = params.get("LogSet")
         self._LogSource = params.get("LogSource")
+        self._CustomShowTags = params.get("CustomShowTags")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-apm-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apm-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apm-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-apm-3.0.937/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apm
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Apm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apm-3.0.936/tencentcloud_sdk_python_apm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apm-3.0.937/tencentcloud_sdk_python_apm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apm
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Apm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apm-3.0.936/README.rst` & `tencentcloud-sdk-python-apm-3.0.937/README.rst`

 * *Files identical despite different names*

