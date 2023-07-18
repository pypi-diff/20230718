# Comparing `tmp/tencentcloud-sdk-python-vrs-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-vrs-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.936.tar", last modified: Mon Jul 17 00:39:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vrs-3.0.937.tar", last modified: Tue Jul 18 00:35:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vrs-3.0.936.tar` & `tencentcloud-sdk-python-vrs-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud_sdk_python_vrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/vrs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/vrs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/vrs/v20200824/
--rw-r--r--   0 root         (0) root         (0)     5710 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/vrs/v20200824/vrs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/vrs/v20200824/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/vrs/v20200824/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    22279 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/vrs/v20200824/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:39:44.000000 tencentcloud-sdk-python-vrs-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/vrs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28696 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:35:21.000000 tencentcloud-sdk-python-vrs-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:35:20.000000 tencentcloud-sdk-python-vrs-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.936/setup.py` & `tencentcloud-sdk-python-vrs-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vrs-3.0.936/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.937/tencentcloud_sdk_python_vrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/vrs/v20200824/vrs_client.py` & `tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/vrs_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,37 @@
 
 class VrsClient(AbstractClient):
     _apiVersion = '2020-08-24'
     _endpoint = 'vrs.tencentcloudapi.com'
     _service = 'vrs'
 
 
+    def CancelVRSTask(self, request):
+        """声音复刻取消任务接口
+
+        :param request: Request instance for CancelVRSTask.
+        :type request: :class:`tencentcloud.vrs.v20200824.models.CancelVRSTaskRequest`
+        :rtype: :class:`tencentcloud.vrs.v20200824.models.CancelVRSTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CancelVRSTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.CancelVRSTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateVRSTask(self, request):
         """本接口服务对提交音频进行声音复刻任务创建接口，异步返回复刻结果。
         • 请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
         • 签名方法参考 公共参数 中签名方法v3。
 
         :param request: Request instance for CreateVRSTask.
         :type request: :class:`tencentcloud.vrs.v20200824.models.CreateVRSTaskRequest`
@@ -97,14 +120,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DownloadVRSModel(self, request):
+        """下载声音复刻离线模型
+
+        :param request: Request instance for DownloadVRSModel.
+        :type request: :class:`tencentcloud.vrs.v20200824.models.DownloadVRSModelRequest`
+        :rtype: :class:`tencentcloud.vrs.v20200824.models.DownloadVRSModelResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DownloadVRSModel", params, headers=headers)
+            response = json.loads(body)
+            model = models.DownloadVRSModelResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetTrainingText(self, request):
         """本接口用于获取声音复刻训练文本信息。
          请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"
         • 签名方法参考 公共参数 中签名方法v3。
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/vrs/v20200824/errorcodes.py` & `tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/errorcodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,32 +10,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+# 任务状态错误。
+FAILEDOPERATION_ERRORINVALIDTASKSTATUS = 'FailedOperation.ErrorInvalidTaskStatus'
+
 # 任务不存在。
 FAILEDOPERATION_NOSUCHTASK = 'FailedOperation.NoSuchTask'
 
 # 检测失败。
 FAILEDOPERATION_VOICEEVALUATEFAILED = 'FailedOperation.VoiceEvaluateFailed'
 
 # 音频质量差。
 FAILEDOPERATION_VOICENOTQUALIFIED = 'FailedOperation.VoiceNotQualified'
 
+# 内部错误。
+INTERNALERROR_FAILACCESSDATABASE = 'InternalError.FailAccessDatabase'
+
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 音频数据错误。
 INVALIDPARAMETERVALUE_AUDIODATA = 'InvalidParameterValue.AudioData'
 
+# 音频时长超限，时长不可超过15s
+INVALIDPARAMETERVALUE_AUDIODURATIONEXCEEDSLIMIT = 'InvalidParameterValue.AudioDurationExceedsLimit'
+
 # Codec非法，请参考Codec参数说明。
 INVALIDPARAMETERVALUE_CODEC = 'InvalidParameterValue.Codec'
 
+# 无效TaskId。
+INVALIDPARAMETERVALUE_ERRORINVALIDTASKID = 'InvalidParameterValue.ErrorInvalidTaskId'
+
 # SampleRate非法，请参考SampleRate参数说明。
 INVALIDPARAMETERVALUE_SAMPLERATE = 'InvalidParameterValue.SampleRate'
 
 # 音色性别错误。
 INVALIDPARAMETERVALUE_VOICEGENDER = 'InvalidParameterValue.VoiceGender'
 
 # 音色语言错误。
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.936/tencentcloud/vrs/v20200824/models.py` & `tencentcloud-sdk-python-vrs-3.0.937/tencentcloud/vrs/v20200824/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,92 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class CancelVRSTaskRequest(AbstractModel):
+    """CancelVRSTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 任务ID
+        :type TaskId: str
+        """
+        self._TaskId = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CancelVRSTaskResponse(AbstractModel):
+    """CancelVRSTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 任务ID
+        :type Data: :class:`tencentcloud.vrs.v20200824.models.CancelVRSTaskRsp`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = CancelVRSTaskRsp()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
+class CancelVRSTaskRsp(AbstractModel):
+    """取消任务响应
+
+    """
+
+
 class CreateVRSTaskRequest(AbstractModel):
     """CreateVRSTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -46,23 +124,26 @@
         :param _Codec: 音频格式，音频类型(wav,mp3,aac,m4a)
         :type Codec: str
         :param _AudioIdList: 音频ID集合
         :type AudioIdList: list of str
         :param _CallbackUrl: 回调 URL，用户自行搭建的用于接收结果的服务URL。如果用户使用轮询方式获取识别结果，则无需提交该参数。
 回调采用POST请求方式，Content-Type为application/json，回调数据格式如下:{"TaskId":"xxxxxxxxxxxxxx","Status":2,"StatusStr":"success","VoiceType":xxxxx,"ErrorMsg":""}
         :type CallbackUrl: str
+        :param _ModelType: 任务类型 1:在线 2:离线  默认为1
+        :type ModelType: int
         """
         self._SessionId = None
         self._VoiceName = None
         self._SampleRate = None
         self._VoiceGender = None
         self._VoiceLanguage = None
         self._Codec = None
         self._AudioIdList = None
         self._CallbackUrl = None
+        self._ModelType = None
 
     @property
     def SessionId(self):
         return self._SessionId
 
     @SessionId.setter
     def SessionId(self, SessionId):
@@ -120,24 +201,33 @@
     def CallbackUrl(self):
         return self._CallbackUrl
 
     @CallbackUrl.setter
     def CallbackUrl(self, CallbackUrl):
         self._CallbackUrl = CallbackUrl
 
+    @property
+    def ModelType(self):
+        return self._ModelType
+
+    @ModelType.setter
+    def ModelType(self, ModelType):
+        self._ModelType = ModelType
+
 
     def _deserialize(self, params):
         self._SessionId = params.get("SessionId")
         self._VoiceName = params.get("VoiceName")
         self._SampleRate = params.get("SampleRate")
         self._VoiceGender = params.get("VoiceGender")
         self._VoiceLanguage = params.get("VoiceLanguage")
         self._Codec = params.get("Codec")
         self._AudioIdList = params.get("AudioIdList")
         self._CallbackUrl = params.get("CallbackUrl")
+        self._ModelType = params.get("ModelType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -573,14 +663,174 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DownloadVRSModelRequest(AbstractModel):
+    """DownloadVRSModel请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 任务ID
+        :type TaskId: str
+        """
+        self._TaskId = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DownloadVRSModelResponse(AbstractModel):
+    """DownloadVRSModel返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 响应
+        :type Data: :class:`tencentcloud.vrs.v20200824.models.DownloadVRSModelRsp`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = DownloadVRSModelRsp()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
+class DownloadVRSModelRsp(AbstractModel):
+    """离线声音复刻模型下载响应
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Model: 模型cos地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Model: str
+        :param _VoiceName: 音色名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VoiceName: str
+        :param _VoiceGender: 音色性别:
+1-male
+2-female
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VoiceGender: int
+        :param _VoiceLanguage: 语言类型：
+1-中文
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VoiceLanguage: int
+        :param _TaskId: 任务ID
+        :type TaskId: str
+        """
+        self._Model = None
+        self._VoiceName = None
+        self._VoiceGender = None
+        self._VoiceLanguage = None
+        self._TaskId = None
+
+    @property
+    def Model(self):
+        return self._Model
+
+    @Model.setter
+    def Model(self, Model):
+        self._Model = Model
+
+    @property
+    def VoiceName(self):
+        return self._VoiceName
+
+    @VoiceName.setter
+    def VoiceName(self, VoiceName):
+        self._VoiceName = VoiceName
+
+    @property
+    def VoiceGender(self):
+        return self._VoiceGender
+
+    @VoiceGender.setter
+    def VoiceGender(self, VoiceGender):
+        self._VoiceGender = VoiceGender
+
+    @property
+    def VoiceLanguage(self):
+        return self._VoiceLanguage
+
+    @VoiceLanguage.setter
+    def VoiceLanguage(self, VoiceLanguage):
+        self._VoiceLanguage = VoiceLanguage
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+
+    def _deserialize(self, params):
+        self._Model = params.get("Model")
+        self._VoiceName = params.get("VoiceName")
+        self._VoiceGender = params.get("VoiceGender")
+        self._VoiceLanguage = params.get("VoiceLanguage")
+        self._TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class GetTrainingTextRequest(AbstractModel):
     """GetTrainingText请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-vrs-3.0.937/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vrs
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Vrs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vrs-3.0.936/README.rst` & `tencentcloud-sdk-python-vrs-3.0.937/README.rst`

 * *Files identical despite different names*

