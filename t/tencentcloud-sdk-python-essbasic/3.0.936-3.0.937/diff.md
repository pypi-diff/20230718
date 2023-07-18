# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.936.tar", last modified: Mon Jul 17 00:24:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.937.tar", last modified: Tue Jul 18 00:23:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.936.tar` & `tencentcloud-sdk-python-essbasic-3.0.937.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54861 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   386414 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:24:57.000000 tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54861 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   386802 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:23:52.000000 tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2179,20 +2179,23 @@
         :type FlowId: str
         :param _FlowApproverInfos: 流程签署人，其中Name和Mobile必传，其他可不传，ApproverType目前只支持PERSON类型的签署人，如果不传默认为该值。还需注意签署人只能有手写签名和时间类型的签署控件，其他类型的填写控件和签署控件暂时都未支持。
         :type FlowApproverInfos: list of FlowApproverInfo
         :param _Operator: 用户信息，暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         :param _Organization: 机构信息，暂未开放
         :type Organization: :class:`tencentcloud.essbasic.v20210526.models.OrganizationInfo`
+        :param _JumpUrl: 签署完之后的H5页面的跳转链接，此链接支持http://和https://，最大长度1000个字符。
+        :type JumpUrl: str
         """
         self._Agent = None
         self._FlowId = None
         self._FlowApproverInfos = None
         self._Operator = None
         self._Organization = None
+        self._JumpUrl = None
 
     @property
     def Agent(self):
         return self._Agent
 
     @Agent.setter
     def Agent(self, Agent):
@@ -2234,14 +2237,22 @@
 
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
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
         self._FlowId = params.get("FlowId")
         if params.get("FlowApproverInfos") is not None:
@@ -2252,14 +2263,15 @@
                 self._FlowApproverInfos.append(obj)
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.937/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.937/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.936/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.937/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

