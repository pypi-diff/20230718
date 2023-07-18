# Comparing `tmp/tencentcloud-sdk-python-wav-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-wav-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wav-3.0.936.tar", last modified: Mon Jul 17 00:39:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wav-3.0.937.tar", last modified: Tue Jul 18 00:35:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wav-3.0.936.tar` & `tencentcloud-sdk-python-wav-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud/wav/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud/wav/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud/wav/v20210129/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud/wav/v20210129/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud/wav/v20210129/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   229073 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud/wav/v20210129/models.py
--rw-r--r--   0 root         (0) root         (0)    25908 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud/wav/v20210129/wav_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud_sdk_python_wav.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud_sdk_python_wav.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud_sdk_python_wav.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud_sdk_python_wav.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/tencentcloud_sdk_python_wav.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:39:53.000000 tencentcloud-sdk-python-wav-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229425 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/models.py
+-rw-r--r--   0 root         (0) root         (0)    25908 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/wav_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:31.000000 tencentcloud-sdk-python-wav-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:35:30.000000 tencentcloud-sdk-python-wav-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-wav-3.0.936/setup.py` & `tencentcloud-sdk-python-wav-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wav-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wav-3.0.936/tencentcloud/wav/v20210129/errorcodes.py` & `tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.936/tencentcloud/wav/v20210129/models.py` & `tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1040,14 +1040,16 @@
         :param _SourceChannelName: 线索渠道名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type SourceChannelName: str
         :param _Gender: 0：未知，1：男，2：女
         :type Gender: int
         :param _CreateTime: 线索创建时间戳，单位：秒
         :type CreateTime: str
+        :param _UpdateTime: 线索创建时间戳，单位：秒
+        :type UpdateTime: str
         :param _LeadStatus: 线索所处状态，101-待分配 201-待建档 301-已建档 401-已邀约 501-跟进中 601-已下订单 701-已成交 801-战败申请中 901-已战败 1001-未知状态 1101-转移申请中 1201-已完成
         :type LeadStatus: int
         :param _LevelCode: 线索意向等级
         :type LevelCode: str
         :param _ImportAtTime: 线索成功导入的时间戳，单位：秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type ImportAtTime: int
@@ -1131,14 +1133,15 @@
         self._LeadUserType = None
         self._LeadType = None
         self._ChannelId = None
         self._ChannelName = None
         self._SourceChannelName = None
         self._Gender = None
         self._CreateTime = None
+        self._UpdateTime = None
         self._LeadStatus = None
         self._LevelCode = None
         self._ImportAtTime = None
         self._DistributeTime = None
         self._CreateAtTime = None
         self._WxId = None
         self._BrandCode = None
@@ -1338,14 +1341,22 @@
         return self._CreateTime
 
     @CreateTime.setter
     def CreateTime(self, CreateTime):
         self._CreateTime = CreateTime
 
     @property
+    def UpdateTime(self):
+        return self._UpdateTime
+
+    @UpdateTime.setter
+    def UpdateTime(self, UpdateTime):
+        self._UpdateTime = UpdateTime
+
+    @property
     def LeadStatus(self):
         return self._LeadStatus
 
     @LeadStatus.setter
     def LeadStatus(self, LeadStatus):
         self._LeadStatus = LeadStatus
 
@@ -1593,14 +1604,15 @@
         self._LeadUserType = params.get("LeadUserType")
         self._LeadType = params.get("LeadType")
         self._ChannelId = params.get("ChannelId")
         self._ChannelName = params.get("ChannelName")
         self._SourceChannelName = params.get("SourceChannelName")
         self._Gender = params.get("Gender")
         self._CreateTime = params.get("CreateTime")
+        self._UpdateTime = params.get("UpdateTime")
         self._LeadStatus = params.get("LeadStatus")
         self._LevelCode = params.get("LevelCode")
         self._ImportAtTime = params.get("ImportAtTime")
         self._DistributeTime = params.get("DistributeTime")
         self._CreateAtTime = params.get("CreateAtTime")
         self._WxId = params.get("WxId")
         self._BrandCode = params.get("BrandCode")
```

### Comparing `tencentcloud-sdk-python-wav-3.0.936/tencentcloud/wav/v20210129/wav_client.py` & `tencentcloud-sdk-python-wav-3.0.937/tencentcloud/wav/v20210129/wav_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.936/tencentcloud_sdk_python_wav.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wav-3.0.937/tencentcloud_sdk_python_wav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wav
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Wav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wav-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-wav-3.0.937/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wav
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Wav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wav-3.0.936/README.rst` & `tencentcloud-sdk-python-wav-3.0.937/README.rst`

 * *Files identical despite different names*

