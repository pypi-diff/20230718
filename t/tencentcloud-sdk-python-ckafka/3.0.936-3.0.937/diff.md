# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.936.tar", last modified: Mon Jul 17 00:20:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.937.tar", last modified: Tue Jul 18 00:20:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.936.tar` & `tencentcloud-sdk-python-ckafka-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    71620 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)   766499 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-17 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    71620 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)   768834 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-18 00:20:22.000000 tencentcloud-sdk-python-ckafka-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.936/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.936/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.937/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13743,14 +13743,18 @@
         :type IndexType: str
         :param _DropCls: 当设置成员参数DropInvalidMessageToCls设置为true时,DropInvalidMessage参数失效
         :type DropCls: :class:`tencentcloud.ckafka.v20190819.models.DropCls`
         :param _DatabasePrimaryKey: 转储到ES的消息为Database的binlog时，如果需要同步数据库操作，即增删改的操作到ES时填写数据库表主键
         :type DatabasePrimaryKey: str
         :param _DropDlq: 死信队列
         :type DropDlq: :class:`tencentcloud.ckafka.v20190819.models.FailureParam`
+        :param _RecordMappingList: 使用数据订阅格式导入 es 时，消息与 es 索引字段映射关系。不填默认为默认字段匹配
+        :type RecordMappingList: list of EsRecordMapping
+        :param _DateField: 消息要映射为 es 索引中 @timestamp 的字段，如果当前配置为空，则使用消息的时间戳进行映射
+        :type DateField: str
         """
         self._Resource = None
         self._Port = None
         self._UserName = None
         self._Password = None
         self._SelfBuilt = None
         self._ServiceVip = None
@@ -13761,14 +13765,16 @@
         self._ContentKey = None
         self._DropInvalidJsonMessage = None
         self._DocumentIdField = None
         self._IndexType = None
         self._DropCls = None
         self._DatabasePrimaryKey = None
         self._DropDlq = None
+        self._RecordMappingList = None
+        self._DateField = None
 
     @property
     def Resource(self):
         return self._Resource
 
     @Resource.setter
     def Resource(self, Resource):
@@ -13898,14 +13904,30 @@
     def DropDlq(self):
         return self._DropDlq
 
     @DropDlq.setter
     def DropDlq(self, DropDlq):
         self._DropDlq = DropDlq
 
+    @property
+    def RecordMappingList(self):
+        return self._RecordMappingList
+
+    @RecordMappingList.setter
+    def RecordMappingList(self, RecordMappingList):
+        self._RecordMappingList = RecordMappingList
+
+    @property
+    def DateField(self):
+        return self._DateField
+
+    @DateField.setter
+    def DateField(self, DateField):
+        self._DateField = DateField
+
 
     def _deserialize(self, params):
         self._Resource = params.get("Resource")
         self._Port = params.get("Port")
         self._UserName = params.get("UserName")
         self._Password = params.get("Password")
         self._SelfBuilt = params.get("SelfBuilt")
@@ -13921,14 +13943,66 @@
         if params.get("DropCls") is not None:
             self._DropCls = DropCls()
             self._DropCls._deserialize(params.get("DropCls"))
         self._DatabasePrimaryKey = params.get("DatabasePrimaryKey")
         if params.get("DropDlq") is not None:
             self._DropDlq = FailureParam()
             self._DropDlq._deserialize(params.get("DropDlq"))
+        if params.get("RecordMappingList") is not None:
+            self._RecordMappingList = []
+            for item in params.get("RecordMappingList"):
+                obj = EsRecordMapping()
+                obj._deserialize(item)
+                self._RecordMappingList.append(obj)
+        self._DateField = params.get("DateField")
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
+class EsRecordMapping(AbstractModel):
+    """消息字段与 es 索引的映射关系
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ColumnName: es 索引成员名称
+        :type ColumnName: str
+        :param _JsonKey: 消息字段名称
+        :type JsonKey: str
+        """
+        self._ColumnName = None
+        self._JsonKey = None
+
+    @property
+    def ColumnName(self):
+        return self._ColumnName
+
+    @ColumnName.setter
+    def ColumnName(self, ColumnName):
+        self._ColumnName = ColumnName
+
+    @property
+    def JsonKey(self):
+        return self._JsonKey
+
+    @JsonKey.setter
+    def JsonKey(self, JsonKey):
+        self._JsonKey = JsonKey
+
+
+    def _deserialize(self, params):
+        self._ColumnName = params.get("ColumnName")
+        self._JsonKey = params.get("JsonKey")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.937/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.936/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.937/README.rst`

 * *Files identical despite different names*

