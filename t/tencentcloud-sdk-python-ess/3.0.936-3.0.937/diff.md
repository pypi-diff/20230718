# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.936.tar", last modified: Mon Jul 17 00:24:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.937.tar", last modified: Tue Jul 18 00:23:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.936.tar` & `tencentcloud-sdk-python-ess-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    61830 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24834 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   430546 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:24:51.000000 tencentcloud-sdk-python-ess-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    61830 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   431046 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:23:47.000000 tencentcloud-sdk-python-ess-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.936/setup.py` & `tencentcloud-sdk-python-ess-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,14 +460,17 @@
 
 # 资源id超过使用上限限制，请联系客服了解规则，并在修改后重试。
 OPERATIONDENIED_MANYRESOURCEID = 'OperationDenied.ManyResourceId'
 
 # 没有API权限。
 OPERATIONDENIED_NOAPIAUTH = 'OperationDenied.NoApiAuth'
 
+# 没有手机号查看的权限
+OPERATIONDENIED_NOAPPROVERMOBILECHECKPERMISSION = 'OperationDenied.NoApproverMobileCheckPermission'
+
 # 无权限操作签署流程，请联系客服了解权限，并在修改后重试。
 OPERATIONDENIED_NOFLOWPERMISSION = 'OperationDenied.NoFlowPermission'
 
 # 未通过个人实名认证。
 OPERATIONDENIED_NOIDENTITYVERIFY = 'OperationDenied.NoIdentityVerify'
 
 # 用户未登录,请先登录后再操作。
@@ -517,14 +520,17 @@
 
 # 该用户已关闭或者未开启自动签服务，请检查后重试。
 OPERATIONDENIED_PERSONNOOPENSERVERSIGN = 'OperationDenied.PersonNoOpenServerSign'
 
 # 拒绝个人静默签，请检查个人静默签签署人，并在修改后重试。
 OPERATIONDENIED_PERSONSERVERSIGNFORBID = 'OperationDenied.PersonServerSignForbid'
 
+# 出证计费额度不足
+OPERATIONDENIED_PROVENOQUOTA = 'OperationDenied.ProveNoQuota'
+
 # 签署二维码已过期，请检查后重试。
 OPERATIONDENIED_QRHASEXPIRE = 'OperationDenied.QrHasExpire'
 
 # 签署二维码不可用，请检查后重试。
 OPERATIONDENIED_QRINVALID = 'OperationDenied.QrInvalid'
 
 # 必填控件未设置填写内容，将检查修改后重试。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.936/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.937/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,18 +189,20 @@
         :param _CustomApproverTag: 客户自定义签署人标识，64位长度，保证唯一，非企微场景不使用此字段
         :type CustomApproverTag: str
         :param _ApproverOption: 签署人个性化能力值
         :type ApproverOption: :class:`tencentcloud.ess.v20201111.models.ApproverOption`
         :param _ApproverVerifyTypes: 签署人查看合同时认证方式, 
 1-实名查看 2-短信验证码查看(企业签署方不支持该方式)
 如果不传默认为1
+模板发起的时候,认证方式以模版配置为主
         :type ApproverVerifyTypes: list of int
         :param _ApproverSignTypes: 签署人签署合同时的认证方式
 1-人脸认证 2-签署密码 3-运营商三要素(默认为1,2)
 合同签署认证方式的优先级 verifyChannel>approverSignTypes
+模板发起的时候,认证方式以模版配置为主
         :type ApproverSignTypes: list of int
         :param _ApproverNeedSignReview: 当前签署方进行签署操作是否需要企业内部审批，true 则为需要。为个人签署方时则由发起方企业审核。	
         :type ApproverNeedSignReview: bool
         """
         self._ApproverType = None
         self._ApproverName = None
         self._ApproverMobile = None
@@ -3666,20 +3668,23 @@
         :type FlowApproverInfos: list of FlowCreateApprover
         :param _Operator: 用户信息，此结构体UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _Organization: 机构信息，暂未开放
         :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
+        :param _JumpUrl: 签署完之后的H5页面的跳转链接，此链接支持http://和https://，最大长度1000个字符。
+        :type JumpUrl: str
         """
         self._FlowId = None
         self._FlowApproverInfos = None
         self._Operator = None
         self._Agent = None
         self._Organization = None
+        self._JumpUrl = None
 
     @property
     def FlowId(self):
         return self._FlowId
 
     @FlowId.setter
     def FlowId(self, FlowId):
@@ -3717,14 +3722,22 @@
 
     @Organization.setter
     def Organization(self, Organization):
         warnings.warn("parameter `Organization` is deprecated", DeprecationWarning) 
 
         self._Organization = Organization
 
+    @property
+    def JumpUrl(self):
+        return self._JumpUrl
+
+    @JumpUrl.setter
+    def JumpUrl(self, JumpUrl):
+        self._JumpUrl = JumpUrl
+
 
     def _deserialize(self, params):
         self._FlowId = params.get("FlowId")
         if params.get("FlowApproverInfos") is not None:
             self._FlowApproverInfos = []
             for item in params.get("FlowApproverInfos"):
                 obj = FlowCreateApprover()
@@ -3735,14 +3748,15 @@
             self._Operator._deserialize(params.get("Operator"))
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
         if params.get("Organization") is not None:
             self._Organization = OrganizationInfo()
             self._Organization._deserialize(params.get("Organization"))
+        self._JumpUrl = params.get("JumpUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.936/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.937/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.937/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.936/README.rst` & `tencentcloud-sdk-python-ess-3.0.937/README.rst`

 * *Files identical despite different names*

