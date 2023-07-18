# Comparing `tmp/tencentcloud-sdk-python-trro-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-trro-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trro-3.0.936.tar", last modified: Mon Jul 17 00:38:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trro-3.0.937.tar", last modified: Tue Jul 18 00:34:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trro-3.0.936.tar` & `tencentcloud-sdk-python-trro-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud/trro/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud/trro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud/trro/v20220325/
--rw-r--r--   0 root         (0) root         (0)    21281 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud/trro/v20220325/trro_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud/trro/v20220325/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud/trro/v20220325/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    98550 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud/trro/v20220325/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud_sdk_python_trro.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud_sdk_python_trro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud_sdk_python_trro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud_sdk_python_trro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:38:41.000000 tencentcloud-sdk-python-trro-3.0.936/tencentcloud_sdk_python_trro.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/
+-rw-r--r--   0 root         (0) root         (0)    21281 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/trro_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   103053 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-18 00:34:06.000000 tencentcloud-sdk-python-trro-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:34:07.000000 tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trro-3.0.936/setup.py` & `tencentcloud-sdk-python-trro-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.936/tencentcloud/trro/v20220325/trro_client.py` & `tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/trro_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.936/tencentcloud/trro/v20220325/errorcodes.py` & `tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.936/tencentcloud/trro/v20220325/models.py` & `tencentcloud-sdk-python-trro-3.0.937/tencentcloud/trro/v20220325/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3187,14 +3187,50 @@
         :type MemUsed: list of float
         :param _TimeOffset: 时间偏移量，单位：秒
         :type TimeOffset: list of int non-negative
         :param _ProjectId: 项目ID
         :type ProjectId: str
         :param _DeviceId: 设备ID
         :type DeviceId: str
+        :param _Ver: sdk版本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Ver: str
+        :param _SdkMode: 模式(p2p/server)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SdkMode: str
+        :param _DecodeCost: 解码耗时，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DecodeCost: list of int
+        :param _RenderConst: 渲染耗时，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RenderConst: list of int
+        :param _K100: 卡顿k100
+注意：此字段可能返回 null，表示取不到有效值。
+        :type K100: list of float
+        :param _K150: 卡顿k150
+注意：此字段可能返回 null，表示取不到有效值。
+        :type K150: list of float
+        :param _NACK: nack请求数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NACK: list of int
+        :param _BitRateEstimate: 服务端调控码率,单位：kbps
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BitRateEstimate: list of int
+        :param _Width: 宽度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Width: int
+        :param _Height: 高度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Height: int
+        :param _EncodeCost: 编码耗时，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EncodeCost: list of int
+        :param _CaptureCost: 采集耗时，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CaptureCost: list of int
         """
         self._DeviceType = None
         self._StartTime = None
         self._EndTime = None
         self._SessionId = None
         self._Rate = None
         self._Fps = None
@@ -3202,14 +3238,26 @@
         self._NetworkLatency = None
         self._VideoLatency = None
         self._CpuUsed = None
         self._MemUsed = None
         self._TimeOffset = None
         self._ProjectId = None
         self._DeviceId = None
+        self._Ver = None
+        self._SdkMode = None
+        self._DecodeCost = None
+        self._RenderConst = None
+        self._K100 = None
+        self._K150 = None
+        self._NACK = None
+        self._BitRateEstimate = None
+        self._Width = None
+        self._Height = None
+        self._EncodeCost = None
+        self._CaptureCost = None
 
     @property
     def DeviceType(self):
         return self._DeviceType
 
     @DeviceType.setter
     def DeviceType(self, DeviceType):
@@ -3315,14 +3363,110 @@
     def DeviceId(self):
         return self._DeviceId
 
     @DeviceId.setter
     def DeviceId(self, DeviceId):
         self._DeviceId = DeviceId
 
+    @property
+    def Ver(self):
+        return self._Ver
+
+    @Ver.setter
+    def Ver(self, Ver):
+        self._Ver = Ver
+
+    @property
+    def SdkMode(self):
+        return self._SdkMode
+
+    @SdkMode.setter
+    def SdkMode(self, SdkMode):
+        self._SdkMode = SdkMode
+
+    @property
+    def DecodeCost(self):
+        return self._DecodeCost
+
+    @DecodeCost.setter
+    def DecodeCost(self, DecodeCost):
+        self._DecodeCost = DecodeCost
+
+    @property
+    def RenderConst(self):
+        return self._RenderConst
+
+    @RenderConst.setter
+    def RenderConst(self, RenderConst):
+        self._RenderConst = RenderConst
+
+    @property
+    def K100(self):
+        return self._K100
+
+    @K100.setter
+    def K100(self, K100):
+        self._K100 = K100
+
+    @property
+    def K150(self):
+        return self._K150
+
+    @K150.setter
+    def K150(self, K150):
+        self._K150 = K150
+
+    @property
+    def NACK(self):
+        return self._NACK
+
+    @NACK.setter
+    def NACK(self, NACK):
+        self._NACK = NACK
+
+    @property
+    def BitRateEstimate(self):
+        return self._BitRateEstimate
+
+    @BitRateEstimate.setter
+    def BitRateEstimate(self, BitRateEstimate):
+        self._BitRateEstimate = BitRateEstimate
+
+    @property
+    def Width(self):
+        return self._Width
+
+    @Width.setter
+    def Width(self, Width):
+        self._Width = Width
+
+    @property
+    def Height(self):
+        return self._Height
+
+    @Height.setter
+    def Height(self, Height):
+        self._Height = Height
+
+    @property
+    def EncodeCost(self):
+        return self._EncodeCost
+
+    @EncodeCost.setter
+    def EncodeCost(self, EncodeCost):
+        self._EncodeCost = EncodeCost
+
+    @property
+    def CaptureCost(self):
+        return self._CaptureCost
+
+    @CaptureCost.setter
+    def CaptureCost(self, CaptureCost):
+        self._CaptureCost = CaptureCost
+
 
     def _deserialize(self, params):
         self._DeviceType = params.get("DeviceType")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._SessionId = params.get("SessionId")
         self._Rate = params.get("Rate")
@@ -3331,14 +3475,26 @@
         self._NetworkLatency = params.get("NetworkLatency")
         self._VideoLatency = params.get("VideoLatency")
         self._CpuUsed = params.get("CpuUsed")
         self._MemUsed = params.get("MemUsed")
         self._TimeOffset = params.get("TimeOffset")
         self._ProjectId = params.get("ProjectId")
         self._DeviceId = params.get("DeviceId")
+        self._Ver = params.get("Ver")
+        self._SdkMode = params.get("SdkMode")
+        self._DecodeCost = params.get("DecodeCost")
+        self._RenderConst = params.get("RenderConst")
+        self._K100 = params.get("K100")
+        self._K150 = params.get("K150")
+        self._NACK = params.get("NACK")
+        self._BitRateEstimate = params.get("BitRateEstimate")
+        self._Width = params.get("Width")
+        self._Height = params.get("Height")
+        self._EncodeCost = params.get("EncodeCost")
+        self._CaptureCost = params.get("CaptureCost")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-trro-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trro-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trro-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-trro-3.0.937/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trro
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Trro SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trro-3.0.936/README.rst` & `tencentcloud-sdk-python-trro-3.0.937/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.936/tencentcloud_sdk_python_trro.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trro-3.0.937/tencentcloud_sdk_python_trro.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trro
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Trro SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

