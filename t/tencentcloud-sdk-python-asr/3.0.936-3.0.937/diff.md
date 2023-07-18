# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.936.tar", last modified: Mon Jul 17 00:17:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.937.tar", last modified: Tue Jul 18 00:17:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.936.tar` & `tencentcloud-sdk-python-asr-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud_sdk_python_asr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29291 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     7371 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   110960 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:17:19.000000 tencentcloud-sdk-python-asr-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29321 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   111858 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:17:10.000000 tencentcloud-sdk-python-asr-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:17:09.000000 tencentcloud-sdk-python-asr-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-asr-3.0.936/setup.py` & `tencentcloud-sdk-python-asr-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.936/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.937/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.936/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/asr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateRecTask(self, request):
         """本接口服务对时长5小时以内的录音文件进行识别，异步返回识别全部结果。
-        • 支持中文普通话、英语、粤语、日语、越南语、马来语、印度尼西亚语、菲律宾语、葡萄牙语、土耳其语、上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话。
+        • 支持中文普通话、英语、粤语、日语、越南语、马来语、印度尼西亚语、菲律宾语、葡萄牙语、土耳其语、阿拉伯语、上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话。
         • 支持wav、mp3、m4a、flv、mp4、wma、3gp、amr、aac、ogg-opus、flac格式。
         • 支持语音 URL 和本地语音文件两种请求方式。语音 URL 的音频时长不能长于5小时，文件大小不超过1GB。本地语音文件调用不能大于5MB。推荐使用 [ 腾讯云COS](https://cloud.tencent.com/document/product/436/38484) 来存储&生成URL提交任务，无外网&流量下行费用，节约成本、提升任务速度。(COS桶权限需要设置公有读私有写，或URL设置外部可访问)
         • 提交录音文件识别请求后，在3小时内完成识别（大多数情况下1小时音频约3分钟以内完成识别，半小时内发送超过1000小时录音或者2万条识别任务的除外），识别结果在服务端可保存7天。
         • 支持回调或轮询的方式获取结果，结果获取请参考[ 录音文件识别结果查询](https://cloud.tencent.com/document/product/1093/37822)。
         •   生成字幕场景可设置参数ResTextFormat为3，解析ResultDetail结构生成字幕，可参考 [生成字幕最佳实践](https://cloud.tencent.com/document/product/1093/84291)。
         •   签名方法参考 [公共参数](https://cloud.tencent.com/document/api/1093/35640) 中签名方法v3。
         • 默认接口请求频率限制：20次/秒。
@@ -440,15 +440,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def SentenceRecognition(self, request):
-        """本接口用于对60秒之内的短音频文件进行识别。<br>•   支持中文普通话、英语、粤语、日语、越南语、马来语、印度尼西亚语、菲律宾语、泰语、葡萄牙语、土耳其语、上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话。<br>•   支持本地语音文件上传和语音URL上传两种请求方式，音频时长不能超过60s，音频文件大小不能超过3MB。<br>•   音频格式支持wav、pcm、ogg-opus、speex、silk、mp3、m4a、aac。<br>•   请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"<br>•   签名方法参考 [公共参数](https://cloud.tencent.com/document/api/1093/35640) 中签名方法v3。<br>•   默认接口请求频率限制：30次/秒，如您有提高请求频率限制的需求，请[前往购买](https://buy.cloud.tencent.com/asr)。
+        """本接口用于对60秒之内的短音频文件进行识别。<br>•   支持中文普通话、英语、粤语、日语、越南语、马来语、印度尼西亚语、菲律宾语、泰语、葡萄牙语、土耳其语、阿拉伯语、上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话。<br>•   支持本地语音文件上传和语音URL上传两种请求方式，音频时长不能超过60s，音频文件大小不能超过3MB。<br>•   音频格式支持wav、pcm、ogg-opus、speex、silk、mp3、m4a、aac。<br>•   请求方法为 HTTP POST , Content-Type为"application/json; charset=utf-8"<br>•   签名方法参考 [公共参数](https://cloud.tencent.com/document/api/1093/35640) 中签名方法v3。<br>•   默认接口请求频率限制：30次/秒，如您有提高请求频率限制的需求，请[前往购买](https://buy.cloud.tencent.com/asr)。
 
         :param request: Request instance for SentenceRecognition.
         :type request: :class:`tencentcloud.asr.v20190614.models.SentenceRecognitionRequest`
         :rtype: :class:`tencentcloud.asr.v20190614.models.SentenceRecognitionResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-asr-3.0.936/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,17 @@
 
 # 访问数据库失败。
 INTERNALERROR_FAILACCESSDATABASE = 'InternalError.FailAccessDatabase'
 
 # 访问Redis失败。
 INTERNALERROR_FAILACCESSREDIS = 'InternalError.FailAccessRedis'
 
+# 说话人音频解码失败
+INTERNALERROR_FAILEDVOICEPRINTDECODE = 'InternalError.FailedVoicePrintDecode'
+
 # 说话人注册接口失败
 INTERNALERROR_FAILEDVOICEPRINTENROLL = 'InternalError.FailedVoicePrintEnroll'
 
 # 说话人验证接口失败
 INTERNALERROR_FAILEDVOICEPRINTVERIFY = 'InternalError.FailedVoicePrintVerify'
 
 # 请求标签接口出错
```

### Comparing `tencentcloud-sdk-python-asr-3.0.936/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.937/tencentcloud/asr/v20190614/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,15 @@
 • 16k_en：英语；
 • 16k_yue：粤语；
 • 16k_id：印度尼西亚语；
 • 16k_fil：菲律宾语；
 • 16k_th：泰语；
 • 16k_pt：葡萄牙语；
 • 16k_tr：土耳其语；
+• 16k_ar：阿拉伯语；
         :type EngineType: str
         :param _Url: 语音流地址，支持rtmp、rtsp等流媒体协议，以及各类基于http协议的直播流(不支持hls, m3u8)
         :type Url: str
         :param _CallbackUrl: 支持HTTP和HTTPS协议，用于接收识别结果，您需要自行搭建公网可调用的服务。回调格式&内容详见：[语音流异步识别回调说明](https://cloud.tencent.com/document/product/1093/52633)
         :type CallbackUrl: str
         :param _SignToken: 用于生成回调通知中的签名
         :type SignToken: str
@@ -601,14 +602,15 @@
 • 16k_vi：越南语；
 • 16k_ms：马来语；
 • 16k_id：印度尼西亚语；
 • 16k_fil：菲律宾语；
 • 16k_th：泰语；
 • 16k_pt：葡萄牙语；
 • 16k_tr：土耳其语；
+• 16k_ar：阿拉伯语；
 • 16k_zh_dialect：多方言，支持23种方言（上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话）；
         :type EngineModelType: str
         :param _ChannelNum: 识别声道数。1：单声道（非电话场景，直接选择单声道即可，忽略音频声道数）；2：双声道（仅支持8k_zh电话场景，双声道应分别对应通话双方）。注意：双声道的电话音频已物理分离说话人，无需再开启说话人分离功能。
         :type ChannelNum: int
         :param _ResTextFormat: 识别结果返回形式。0： 识别结果文本(含分段时间戳)； 1：词级别粒度的[详细识别结果](https://cloud.tencent.com/document/api/1093/37824#SentenceDetail)(不含标点，含语速值)；2：词级别粒度的详细识别结果（包含标点、语速值）；3: 标点符号分段，包含每段时间戳，特别适用于字幕场景（包含词级时间、标点、语速值）。4：【增值付费功能】对识别结果按照语义分段，并展示词级别粒度的详细识别结果，仅支持8k_zh、16k_zh引擎，需购买对应资源包使用（注意：如果账号后付费功能开启并使用此功能，将[自动计费](https://cloud.tencent.com/document/product/1093/35686)）
         :type ResTextFormat: int
         :param _SourceType: 语音数据来源。0：语音 URL；1：语音数据（post body）。
@@ -2279,14 +2281,15 @@
 • 16k_vi：越南语；
 • 16k_ms：马来语；
 • 16k_id：印度尼西亚语；
 • 16k_fil：菲律宾语；
 • 16k_th：泰语；
 • 16k_pt：葡萄牙语；
 • 16k_tr：土耳其语；
+• 16k_ar：阿拉伯语；
 • 16k_zh_dialect：多方言，支持23种方言（上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话）；
         :type EngSerViceType: str
         :param _SourceType: 语音数据来源。0：语音 URL；1：语音数据（post body）。
         :type SourceType: int
         :param _VoiceFormat: 识别音频的音频格式，支持wav、pcm、ogg-opus、speex、silk、mp3、m4a、aac、amr。
         :type VoiceFormat: str
         :param _ProjectId: 腾讯云项目 ID，废弃参数，填写0即可。
@@ -2316,14 +2319,16 @@
         :param _CustomizationId: 自学习模型 id。如设置了该参数，将生效对应的自学习模型。
         :type CustomizationId: str
         :param _ReinforceHotword: 热词增强功能。1:开启后（仅支持8k_zh,16k_zh），将开启同音替换功能，同音字、词在热词中配置。举例：热词配置“蜜制”并开启增强功能后，与“蜜制”同拼音（mizhi）的“秘制”、“蜜汁”的识别结果会被强制替换成“蜜制”。因此建议客户根据自己的实际情况开启该功能。
         :type ReinforceHotword: int
         :param _HotwordList: 临时热词：用于提升识别准确率，临时热词规则：“热词|权重”，热词不超过30个字符（最多10个汉字），权重1-10，最多传入128个热词。举例："腾讯云|10,语音识别|5,ASR|10"。
 “临时热词”和“热词id”的区别：热词id需要先在控制台或通过接口创建热词表，得到热词表id后才可以使用热词功能，本字段可以在每次请求时直接传入热词使用，但每次请求后云端不会保留相关的热词数据，需要客户自行维护相关数据
         :type HotwordList: str
+        :param _InputSampleRate: 支持pcm格式的8k音频在与引擎采样率不匹配的情况下升采样到16k后识别，能有效提升识别准确率。仅支持：8000。如：传入 8000 ，则pcm音频采样率为8k，当引擎选用16k_zh， 那么该8k采样率的pcm音频可以在16k_zh引擎下正常识别。 注：此参数仅适用于pcm格式音频，不传入值将维持默认状态，即默认调用的引擎采样率等于pcm音频采样率。
+        :type InputSampleRate: int
         """
         self._EngSerViceType = None
         self._SourceType = None
         self._VoiceFormat = None
         self._ProjectId = None
         self._SubServiceType = None
         self._Url = None
@@ -2335,14 +2340,15 @@
         self._FilterModal = None
         self._FilterPunc = None
         self._ConvertNumMode = None
         self._HotwordId = None
         self._CustomizationId = None
         self._ReinforceHotword = None
         self._HotwordList = None
+        self._InputSampleRate = None
 
     @property
     def EngSerViceType(self):
         return self._EngSerViceType
 
     @EngSerViceType.setter
     def EngSerViceType(self, EngSerViceType):
@@ -2492,14 +2498,22 @@
     def HotwordList(self):
         return self._HotwordList
 
     @HotwordList.setter
     def HotwordList(self, HotwordList):
         self._HotwordList = HotwordList
 
+    @property
+    def InputSampleRate(self):
+        return self._InputSampleRate
+
+    @InputSampleRate.setter
+    def InputSampleRate(self, InputSampleRate):
+        self._InputSampleRate = InputSampleRate
+
 
     def _deserialize(self, params):
         self._EngSerViceType = params.get("EngSerViceType")
         self._SourceType = params.get("SourceType")
         self._VoiceFormat = params.get("VoiceFormat")
         self._ProjectId = params.get("ProjectId")
         self._SubServiceType = params.get("SubServiceType")
@@ -2512,14 +2526,15 @@
         self._FilterModal = params.get("FilterModal")
         self._FilterPunc = params.get("FilterPunc")
         self._ConvertNumMode = params.get("ConvertNumMode")
         self._HotwordId = params.get("HotwordId")
         self._CustomizationId = params.get("CustomizationId")
         self._ReinforceHotword = params.get("ReinforceHotword")
         self._HotwordList = params.get("HotwordList")
+        self._InputSampleRate = params.get("InputSampleRate")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-asr-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.937/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.936/README.rst` & `tencentcloud-sdk-python-asr-3.0.937/README.rst`

 * *Files identical despite different names*

